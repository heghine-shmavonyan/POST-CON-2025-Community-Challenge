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
