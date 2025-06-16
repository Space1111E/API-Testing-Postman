# 🧪 API Testing with Postman

This project covers the **functional testing** of an API using Postman.

---

## 🔧 What Has Been Tested:

- **GET** – Retrieving data  
- **POST** – Creating a new resource  
- **PUT** – Updating existing data  
- **DELETE** – Deleting a resource  

---

## ✅ Testing Goals:

- Verify HTTP status codes  
- Validate response content  
- Perform negative testing to ensure API handles incorrect inputs properly  

---

## 📦 API Used:

- **JSONPlaceholder** – Fake REST API for testing and prototyping  

---

## 📋 Requirements

- [Postman](https://www.postman.com/downloads/) installed  
- Access to the internet (for the public API)  
- Optional: [Newman](https://www.npmjs.com/package/newman) for running tests via command line  

---

## ▶️ How to Run Tests

1. Import the Postman collection from the `collections/` folder into Postman.  
2. Set up any required environment variables if necessary.  
3. Run individual requests or the entire collection using Postman’s Collection Runner.  
4. (Optional) Use Newman to run the collection via CLI:  
   ```bash
   newman run collections/YourCollectionName.postman_collection.json
  
   ```

   
   # 📎 Postman Collection
 🔗 https://www.postman.com
---

## 📄 Included Documents
- `Test_Cases.md` – List of test scenarios  
- `Bug_Report.md` – Bugs discovered during testing  


