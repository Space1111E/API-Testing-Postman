# ✅ API Test Cases – User Endpoints

## 📌 Overview
This document contains the API test cases for the user-related endpoints in the system. The goal is to verify that core user functionalities—such as creating, retrieving, updating, and deleting users—perform as expected and return proper HTTP responses.

---

## 🧰 Tools Used
- **Postman** – For creating and executing API requests
- **JSON** – As the data format for requests and responses
- **Newman** *(optional)* – For automated test runs via CLI

---

## ▶️ How to Use
1. Import the collection located in the `collections/` directory into Postman.
2. Load the appropriate environment from the `environments/` folder.
3. Use Postman's Collection Runner or Newman to execute tests.
4. Refer to the test table below for the expected results of each scenario.

---

## 🧪 Test Cases Table

| ID     | Description                           | Method | Endpoint     | Data                     | Expected Result                          | Status        |
|--------|---------------------------------------|--------|--------------|--------------------------|------------------------------------------|---------------|
| TC-001 | Retrieve all users                    | GET    | /users       | -                        | Status 200, list of users                | Passed        |
| TC-002 | Retrieve a single user by ID          | GET    | /users/1     | -                        | Status 200, user info                    | Passed        |
| TC-003 | Create a new user                     | POST   | /users       | JSON with name/email     | Status 201, new user created             | Passed        |
| TC-004 | Request with empty fields             | POST   | /users       | Empty JSON               | Status 400, validation error             | Under Review  |
| TC-005 | Update existing user                  | PUT    | /users/1     | JSON with updated info   | Status 200, user updated                 | Passed        |
| TC-006 | Delete a user                         | DELETE | /users/1     | -                        | Status 200 or 204                        | Passed        |

---

## 🟢 Status Legend
- **Passed** – Test completed successfully, and the result matches expectations.
- **Under Review** – Test has not been finalized or needs clarification.
- **Failed** – Test was executed but did not produce the expected result. *(None currently)*

---

## 📌 Notes
- Ensure your environment includes a valid `baseUrl` variable.
- Authentication is not required for these test cases; if added later, update headers accordingly.
- More edge case scenarios will be added in future versions (e.g., invalid ID format, unauthorized access).

