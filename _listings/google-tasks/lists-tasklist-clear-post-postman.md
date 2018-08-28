{
  "info": {
    "name": "Google Tasks API Add Lists Task List Clear",
    "_postman_id": "90bd48b1-d5d6-46e9-89c1-0ea27717dde3",
    "description": "Clears all completed tasks from the specified task list. The affected tasks will be marked as 'hidden' and no longer be returned by default when retrieving all tasks for a task list.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "lists",
      "item": [
        {
          "id": "d0340787-c7e3-4461-a070-612f5ee2a4d4",
          "name": "tasks.tasks.clear",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.googleapis.com",
              "path": [
                "tasks",
                "v1",
                "lists/:tasklist/clear"
              ],
              "variable": [
                {
                  "id": "tasklist",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Clears all completed tasks from the specified task list"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a9c062d5-d779-4dad-93f4-c65fb659b1f4"
            }
          ]
        }
      ]
    }
  ]
}