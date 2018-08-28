{
  "info": {
    "name": "Google Tasks API Get Users @me Lists",
    "_postman_id": "ef5e2322-236f-4d6b-9c49-b177acad998a",
    "description": "Returns all the authenticated user's task lists.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "users",
      "item": [
        {
          "id": "6d1f628c-720c-4f3c-a0a5-0a557460ab86",
          "name": "tasks.tasklists.list",
          "request": {
            "url": "http://www.googleapis.com/tasks/v1/users/@me/lists?maxResults=%7B%7D&pageToken=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns all the authenticated user's task lists"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "437034e8-428f-4900-8c36-6d4810d5f1fc"
            }
          ]
        }
      ]
    }
  ]
}