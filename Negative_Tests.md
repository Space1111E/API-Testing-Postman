# Negative Test Scenarios - API Testing

Ky dokument përmbledh skenarët negativë të testimit për të siguruar që API reagon siç duhet ndaj kërkesave të pasakta, të paplota ose të paautorizuara.

| ID      | Përshkrimi                           | Metoda | Endpoint    | Të Dhënat                  | Rezultati i Pritshëm            | Statusi |
| ------- | ------------------------------------ | ------ | ----------- | -------------------------- | ------------------------------- | ------- |
| TC-NEG1 | POST pa `email`                      | POST   | /users      | `{ "name": "Test" }`       | Status 400 – error validimi     | Kaloi   |
| TC-NEG2 | GET me ID që nuk ekziston            | GET    | /users/9999 | -                          | Status 404 – Not Found          | Kaloi   |
| TC-NEG3 | DELETE pa ID (endpoint jo i plotë)   | DELETE | /users      | -                          | Status 405 – Method Not Allowed | Kaloi   |
| TC-NEG4 | POST me format të gabuar të JSON     | POST   | /users      | `{ name: Test }` (invalid) | Status 400 – invalid syntax     | Kaloi   |
| TC-NEG5 | PUT me ID jo ekzistues               | PUT    | /users/9999 | JSON me emër               | Status 404 – Not Found          | Kaloi   |
| TC-NEG6 | GET në endpoint që nuk ekziston fare | GET    | /unknown    | -                          | Status 404 – endpoint not found | Kaloi   |
