## Raporti i Bug-eve

# 🐞 Bug Report – API Testing

| ID      | Përshkrimi              | Hapat për Riprodhim                  | Rezultati i Pritshëm | Rezultati Aktual      | Prioriteti | Statusi |
| ------- | ----------------------- | ------------------------------------ | -------------------- | --------------------- | ---------- | ------- |
| BUG-001 | POST pa të dhëna        | 1. Hap Postman<br>2. Dërgo POST bosh | Duhet status 400     | Merr status 500       | High       | Hapës   |
| BUG-002 | GET me ID që s’ekziston | GET /users/999                       | Duhet status 404     | Merr status 200 me {} | Medium     | Hapës   |
