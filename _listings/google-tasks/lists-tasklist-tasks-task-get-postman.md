{
  "info": {
    "name": "Google Tasks API Get Lists Task List Tasks Task",
    "_postman_id": "fc582067-6517-4896-9571-299ca4f976c6",
    "description": "Returns the specified task.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "lists",
      "item": [
        {
          "id": "45eeb181-1ce0-4512-9e59-7f3fdd1c3860",
          "name": "tasks.tasks.get",
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
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the specified task"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dfec7bc3-268c-41ed-8755-f563df93e2b7"
            }
          ]
        }
      ]
    }
  ]
}