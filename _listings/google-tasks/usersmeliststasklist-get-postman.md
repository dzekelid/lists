{
  "info": {
    "name": "Google Tasks API Get Users Task List",
    "_postman_id": "f87c38a5-4b95-4fe2-a3d3-a9fa5175efcb",
    "description": "Returns the authenticated user's specified task list.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "users",
      "item": [
        {
          "id": "3908618d-567a-4cd1-8a61-d557db854f74",
          "name": "tasks.tasklists.get",
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
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the authenticated user's specified task list"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6a0e752c-6b46-4d7d-8d5c-d498d685f9e5"
            }
          ]
        }
      ]
    }
  ]
}