# ❌ Negative Test Scenarios – API Testing

## 📌 Overview
This document summarizes negative test cases designed to ensure that the API responds correctly to invalid, incomplete, or unauthorized requests. These tests help validate robustness and proper error handling.

---

## 🧪 Negative Test Cases Table

| ID       | Description                                  | Method | Endpoint     | Data                         | Expected Result                         | Status  |
|----------|----------------------------------------------|--------|--------------|------------------------------|------------------------------------------|---------|
| TC-NEG1  | POST without email                           | POST   | /users       | `{ "name": "Test" }`         | Status 400 – validation error            | Passed  |
| TC-NEG2  | GET with non-existent ID                     | GET    | /users/9999  | -                            | Status 404 – Not Found                   | Passed  |
| TC-NEG3  | DELETE with missing ID (incomplete endpoint) | DELETE | /users       | -                            | Status 405 – Method Not Allowed          | Passed  |
| TC-NEG4  | POST with invalid JSON format                | POST   | /users       | `{ name: Test }` *(invalid)* | Status 400 – invalid syntax              | Passed  |
| TC-NEG5  | PUT with non-existent ID                     | PUT    | /users/9999  | JSON with name               | Status 404 – Not Found                   | Passed  |
| TC-NEG6  | GET request to completely unknown endpoint   | GET    | /unknown     | -                            | Status 404 – endpoint not found          | Passed  |

---

## ✅ Notes
- All tests are designed to simulate incorrect or unexpected client behavior.
- These scenarios are essential for hardening the API against misuse and poor input validation.
- Validation errors follow RESTful conventions using HTTP status codes (400, 404, 405).

