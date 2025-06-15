## Test Cases

# ✅ Test Cases – API Testing

| ID     | Përshkrimi                     | Metoda | Endpoint | Të Dhënat            | Rezultati i Pritshëm           | Statusi     |
| ------ | ------------------------------ | ------ | -------- | -------------------- | ------------------------------ | ----------- |
| TC-001 | Marrja e të gjithë përdoruesve | GET    | /users   | -                    | Status 200, listë përdoruesish | Kaloi       |
| TC-002 | Marrja e një përdoruesi me ID  | GET    | /users/1 | -                    | Status 200, info përdorues     | Kaloi       |
| TC-003 | Krijimi i përdoruesit të ri    | POST   | /users   | JSON me emër/email   | Status 201, user i ri          | Kaloi       |
| TC-004 | Kërkesë me fushë bosh          | POST   | /users   | JSON bosh            | Status 400, error validimi     | Në shqyrtim |
| TC-005 | Përditësimi i një përdoruesi   | PUT    | /users/1 | JSON me info të reja | Status 200, info përditësuar   | Kaloi       |
| TC-006 | Fshirja e një përdoruesi       | DELETE | /users/1 | -                    | Status 200 ose 204             | Kaloi       |
