{
  "info": {
    "name": "Google Tasks API Delete Lists Task List Tasks Task",
    "_postman_id": "84345a9e-9f41-474c-ab1c-8ea3f876c3be",
    "description": "Deletes the specified task from the task list.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "lists",
      "item": [
        {
          "id": "9345fbd4-a8c3-4781-8f9b-524d59366227",
          "name": "tasks.tasks.delete",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.googleapis.com",
              "path": [
                "tasks",
                "v1",
                "lists/:tasklist/tasks/:task"
              ],
              "variable": [
                {
                  "id": "task",
                  "value": "{}",
                  "type": "string"
                },
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
            "description": "Deletes the specified task from the task list"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "56dd46d8-4c8e-4b81-92f4-2eaf68109cd5"
            }
          ]
        }
      ]
    }
  ]
}