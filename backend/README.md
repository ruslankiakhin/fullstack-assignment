# Task Description

Your task is to prepare backend written on swagger (python, flask) to replace mock-server.

Endpoints:

- Get services for fontend
  Request: GET /services
  Response Code: 200
  Response Data: JSON output taken from db.json
- Update/Add service to db.json
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
- Use decorators, classes for reusable parts

## Bonus Tasks:

- Protect PUT endpoint using JWT 
- Track all requests to endpoints in a log file
- Write tests for your endpoints (unit, codestyle, api tests)

