For some reason POST method wasnt working with curl, but the following command works as required:
Invoke-RestMethod -Uri "http://localhost:8080/user" `
  -Headers @{"X-API-Key"="secret123"; "Content-Type"="application/json"} `
  -Method Post `
  -Body '{"name":"Alice"}'
