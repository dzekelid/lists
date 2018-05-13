{
  "info": {
    "name": "Google Tasks API Get Lists Task List Tasks",
    "_postman_id": "d1be4750-864e-43a5-9a27-2bff34114cd1",
    "description": "Returns all tasks in the specified task list.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "lists",
      "item": [
        {
          "id": "86a1674c-456a-49a2-b3bd-42a8d1e10a8b",
          "name": "tasks.tasks.list",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.googleapis.com",
              "path": [
                "tasks",
                "v1",
                "lists/:tasklist/tasks"
              ],
              "query": [
                {
                  "key": "completedMax",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "completedMin",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "dueMax",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "dueMin",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "maxResults",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "pageToken",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "showCompleted",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "showDeleted",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "showHidden",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "updatedMin",
                  "value": "%7B%7D",
                  "disabled": false
                }
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
            "description": "Returns all tasks in the specified task list"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d8b1598a-e141-45ec-ba80-5a97edbe40ff"
            }
          ]
        }
      ]
    }
  ]
}