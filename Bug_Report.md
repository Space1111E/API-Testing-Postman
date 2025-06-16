# 🐞 Detailed Bug Report – API Testing

## 📌 Overview
This document tracks detailed bug reports discovered during API testing. The structure ensures clarity and thoroughness for efficient troubleshooting.

---

## 🐛 Bug List

| ID      | Title                        | Environment          | Steps to Reproduce                                                                 | Expected Result          | Actual Result                  | Priority | Severity | Assigned To | Status  | Date Reported | Reporter |
|---------|------------------------------|----------------------|------------------------------------------------------------------------------------|--------------------------|-------------------------------|----------|----------|-------------|---------|---------------|----------|
| BUG-001 | POST request with no data    | Dev environment v1.2  | 1. Open Postman  <br> 2. Send empty POST to `/users`                               | Should return status 400  | Returns status 500             | High     | Critical | John D.     | Open    | 2025-06-16    | Elena B.   |
| BUG-002 | GET with invalid user ID     | Prod environment v1.2 | Send GET request to `/users/999`                                                  | Should return status 404  | Returns status 200 with `{}`   | Medium   | Major    | Mark S.    | Open    | 2025-06-15    | Elena B.   |

---

## 📝 Field Definitions

- **ID**: Unique bug identifier  
- **Title**: Short summary of the bug  
- **Environment**: Server/version where bug was found (dev, staging, prod)  
- **Steps to Reproduce**: Step-by-step instructions to recreate the issue  
- **Expected Result**: What should happen when following the steps  
- **Actual Result**: What actually happens  
- **Priority**: Importance to fix (High, Medium, Low)  
- **Severity**: Impact level (Critical, Major, Minor)  
- **Assigned To**: Developer responsible for fixing the bug  
- **Status**: Current state (Open, In Progress, Resolved, Closed)  
- **Date Reported**: When the bug was reported  
- **Reporter**: Person who reported the bug  

---
