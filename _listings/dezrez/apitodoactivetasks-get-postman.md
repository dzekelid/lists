{
  "info": {
    "name": "Dezrez Get the list of active tasks of a Todo",
    "_postman_id": "bf94ae17-a5ad-4ba0-af0e-5e4fc9ec91eb",
    "description": "Get the list of active tasks of a todo.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "SystemStatus",
      "item": [
        {
          "id": "a9927c2a-6690-4f72-baa6-05f1ba467db1",
          "name": "Branch_UpdateScheduledTaskStatusByidBysystemStatus",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.dezrez.com",
              "path": [
                "api/branch/updatescheduledtaskstatus/:id"
              ],
              "query": [
                {
                  "key": "systemStatus",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "header": [
              {
                "key": "Rezi-Api-Version",
                "value": "{}",
                "description": "Specifies which version of the API to call",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Update systemstatus of scheduledtask to active, inactive, deleted or archived.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cebaad79-9482-4bdc-ac49-5d7b3e71406d"
            }
          ]
        }
      ]
    },
    {
      "name": "List",
      "item": [
        {
          "id": "723c218e-4193-4219-8eb0-6cb53345926b",
          "name": "DefaultToDo_ActiveTasksBytoDoIdByignoreDueDateBypageSizeBypageNumber",
          "request": {
            "url": "http://api.dezrez.com/api/todo/activetasks?ignoreDueDate=%7B%7D&pageNumber=%7B%7D&pageSize=%7B%7D&toDoId=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "Rezi-Api-Version",
                "value": "{}",
                "description": "Specifies which version of the API to call",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get the list of active tasks of a todo."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e03b8285-243c-41e9-acd5-55390ea6cf2b"
            }
          ]
        }
      ]
    }
  ]
}