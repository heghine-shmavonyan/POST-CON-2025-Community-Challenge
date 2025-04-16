# POST-CON-2025-Community-Challenge

📄 SMS API Testing Collection
This Postman collection automates testing for an SMS Gateway API. It covers both positive and negative cases to ensure robust messaging functionality.
✅ Covered Scenarios:
Send SMS
Send SMS with:
Images (MMS-style)
1–3 custom fields
Custom line_id parameter
Emojis
Languages

Negative test cases:
Missing fields (from, to, message)
Invalid token
Invalid custom field types
Non-existing line_id


🧠 Why This Matters
This collection helps QA and developers verify API behavior for all critical messaging flows, ensuring reliable communication and graceful error handling.
🛠️ Features
Dynamic variables (Odio eligendi dolorem voluptas sequi et., South Kirafort, etc.)
Environment-driven requests (api_token, from, to)
Assertions for HTTP status codes, message contents, and error fields
Easily extendable for international numbers, bulk sending, or rate-limiting tests

🚀 How to Use
Import the collection and environment into Postman.
Set your API base URL and token in the environment.
Run requests manually, or use Collection Runner for all tests.
Review test results and assertions in the “Test Results” tab.

🛡️ Note: This is a sanitized version of the test suite. Sensitive credentials and URLs have been removed or masked.
👤 Created by: Heghine Shmavonyan
🔧 _Made for POST/CON 2025 Community Challenge
