# SMS API Testing Collection

This Postman collection automates testing for an SMS Gateway API. It covers both positive and negative test cases to ensure robust messaging functionality.

## ✅ Covered Scenarios

- **Send SMS**
- **Send SMS with:**
  - Images (MMS-style)
  - 1–3 custom fields
  - Custom `line_id` parameter
  - Emojis
  - Languages

### Negative Test Cases:

- Missing fields (from, to, message)
- Invalid token
- Invalid custom field types
- Non-existing `line_id`

---

## 🧠 Why This Matters

This collection helps QA and developers verify the API's behavior for all critical messaging flows, ensuring reliable communication and graceful error handling.

---

## 🛠️ Features

- **Dynamic Variables** – Handle real-time data inputs (e.g., locations like “South Kirafort”).
- **Environment-driven Requests** – Easily configure API tokens, `from`, and `to` values.
- **Assertions** – Verify HTTP status codes, message contents, and error fields.
- **Extendable** – Easily extend for international numbers, bulk sending, or rate-limiting tests.

---
## 📦 Custom Packages Setup

Postman currently **does not support exporting custom packages** directly. To ensure the functionality of this test collection, all custom packages used are included in this repository as standalone JSON files.

### Included Packages

- `messages_language.json` – Contains functions to generate multilingual messages with and without emojis.
- `assertions.json` – Includes reusable test assertions like `expect202()` and `expectSuccessMessage()`.

### 🧰 How to Use These Packages

1. **Manually Create Packages in Postman**  
   Postman does not allow importing packages via JSON, so you’ll need to manually create them:

   - Open **Postman** and go to your **Scratch Pad** or desired **workspace**.
   - In the sidebar, click **“Packages”** > **“+ New Package”** > **JavaScript library**.
   - Copy the contents of `messages_language.json` or `assertions.json` and paste into the Postman package editor.
   - Set the package name exactly as follows:
     - `messages_language`
     - `assertions`

2. **Save and Publish**  
   - Save the package. Once it’s in your workspace, Postman will resolve the `pm.require(...)` calls inside the collection automatically.

### ⚠️ Notes

- The Postman collection only contains **references** to these packages (by name and ID), not the actual code.
- If the package names or IDs are incorrect or not created in your workspace, the scripts will fail with a `require is not defined` or `module not found` error.
- You can rename the packages, but you must also update the references in the collection’s `"packages"` field.


## 🚀 How to Use

1. **Import the Collection & Environment**: 
   - Import the collection and environment into Postman.

2. **Set Up**:
   - Set your API base URL and token in the environment variables.

3. **Run Tests**:
   - Run requests manually or use the **Collection Runner** for all tests.

4. **Review Results**:
   - Review test results and assertions in the "Test Results" tab.

---

## 🛡️ Note

This is a sanitized version of the test suite. Sensitive credentials and URLs have been removed or masked.

---

## 👤 Created by: Heghine Shmavonyan

🔧 _Made for POST/CON 2025 Community Challenge_
