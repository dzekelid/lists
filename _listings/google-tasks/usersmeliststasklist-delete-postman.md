{
  "info": {
    "name": "Google Tasks API Delete Users Task List",
    "_postman_id": "7c88d745-7bc1-471c-b2b5-9b05a3a08f65",
    "description": "Deletes the authenticated user's specified task list.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "users",
      "item": [
        {
          "id": "8b3ca4b5-557a-4bde-99ca-158350405868",
          "name": "tasks.tasklists.delete",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.googleapis.com",
              "path": [
                "tasks",
                "v1",
                "users/@me/lists/:tasklist"
              ],
              "variable": [
                {
                  "id": "tasklist",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the authenticated user's specified task list"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8a7f23aa-1760-401b-9854-0010aa364b7a"
            }
          ]
        }
      ]
    }
  ]
}