# Task Description

Your task is to implement an API server with Swagger (python, flask) to replace the `mock-server` from the frontend assignment.

The server will provide the following endpoints:

- Get list of services
  ```
  Request: GET /services
  Response Code: 200
  Response Data: JSON output taken from db.json
  ```
- Update/Add a service to db.json
  ```
  Request: PUT /services, 
   {
      "service": "Service New",
      "ip": "10.55.55.55",
      "servers": [
        { "name": "lin-pra-111", "status": "running" },
        { "name": "lin-pra-222", "status": "error" },
        { "name": "lin-pra-333", "status": "running" },
        { "name": "lin-pra-444", "status": "error" }
      ]
    }
  Response Code: 200 or 201
  ```
- Use decorators, classes for reusable parts
- Use the `db.json` file to store data

## Bonus Tasks:

- Protect the PUT endpoint using JWT (Json Web Token)
- Track all requests to endpoints in a log file
- Write tests for your endpoints (unit, codestyle, api tests)
