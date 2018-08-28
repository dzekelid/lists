{
  "info": {
    "name": "Microsoft Graph API List Range Border Collection",
    "_postman_id": "8a5ac712-1edb-422e-84ff-34bd02aa9918",
    "description": "List RangeBorderCollection Retrieve a list of rangeborder objects.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Attachment",
      "item": [
        {
          "id": "a9d8442f-ff18-4189-a5ac-5308dd81c74e",
          "name": "GetAttachment",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "me/events/:id/attachments/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get attachment\nRead the properties and relationships of an attachment, attached to an event,\nmessage, or post."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "953a176f-c90a-4157-a178-aa1f04962f54"
            }
          ]
        },
        {
          "id": "59620b11-c538-401d-81ea-3cc0b049c144",
          "name": "GetAttachment",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "users/:id | userPrincipalName/events/:id/attachments/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                },
                {
                  "id": "id | userPrincipalName",
                  "value": "id | userPrincipalName",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get attachment\nRead the properties and relationships of an attachment, attached to an event,\nmessage, or post."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2dbed8e6-68e7-4974-aab2-eac01d76cc6e"
            }
          ]
        },
        {
          "id": "82b5b38a-9b28-45e2-a75c-0a594b330d4c",
          "name": "GetAttachment1",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "groups/:id/events/:id/attachments/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get attachment\nRead the properties and relationships of an attachment, attached to an event,\nmessage, or post."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e559654d-a0f9-4d91-947d-92208c6b2e2c"
            }
          ]
        },
        {
          "id": "f22bba10-39ed-42d7-82ac-f493622189e6",
          "name": "GetAttachment2",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "me/calendar/:id/events/:id/attachments/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get attachment\nRead the properties and relationships of an attachment, attached to an event,\nmessage, or post."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "598a89e8-3ed0-406a-9e7b-8600f8d8d65e"
            }
          ]
        },
        {
          "id": "90126075-ac9c-483e-a0a4-f0fbe2cdcd3c",
          "name": "GetAttachment1",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "users/:id | userPrincipalName/calendar/events/:id/attachments/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                },
                {
                  "id": "id | userPrincipalName",
                  "value": "id | userPrincipalName",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get attachment\nRead the properties and relationships of an attachment, attached to an event,\nmessage, or post."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4b9d6e6f-0991-471f-afec-e15f3d9a2134"
            }
          ]
        },
        {
          "id": "17ec38e6-df86-4de8-9851-b87439c9dc1e",
          "name": "GetAttachment3",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "groups/:id/calendar/events/:id/attachments/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get attachment\nRead the properties and relationships of an attachment, attached to an event,\nmessage, or post."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b8d6db71-bd4b-422a-a488-58fedc66863f"
            }
          ]
        },
        {
          "id": "630fcba6-20b5-40f4-af19-73d838ef49ed",
          "name": "GetAttachment4",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "me/calendars/:id/events/:id/attachments/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get attachment\nRead the properties and relationships of an attachment, attached to an event,\nmessage, or post."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "61ecec6c-fb9d-421b-a93a-0877716b29e1"
            }
          ]
        },
        {
          "id": "f1f75aa9-7b6b-4fda-8a01-d12532a18255",
          "name": "GetAttachment2",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "users/:id | userPrincipalName/calendars/:id/events/:id/attachments/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                },
                {
                  "id": "id | userPrincipalName",
                  "value": "id | userPrincipalName",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get attachment\nRead the properties and relationships of an attachment, attached to an event,\nmessage, or post."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ba137f3a-59b9-4ebc-897e-3d9b433611e6"
            }
          ]
        },
        {
          "id": "83eac630-c407-4a34-a49d-89f8d8351097",
          "name": "GetAttachment5",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "me/calendargroup/calendars/:id/events/:id/attachments/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get attachment\nRead the properties and relationships of an attachment, attached to an event,\nmessage, or post."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "80705ab1-93f0-4b3f-88a4-40177f7b0e3d"
            }
          ]
        },
        {
          "id": "99d919dc-8eba-4011-a3b8-3f2c9d840701",
          "name": "GetAttachment3",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "users/:id | userPrincipalName/calendargroup/calendars/:id/events/:id/attachments/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                },
                {
                  "id": "id | userPrincipalName",
                  "value": "id | userPrincipalName",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get attachment\nRead the properties and relationships of an attachment, attached to an event,\nmessage, or post."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bf8208db-cdc4-4187-a8d7-bd33b137db87"
            }
          ]
        },
        {
          "id": "c18cbcb5-6f29-47f1-a061-8fd7454f7be6",
          "name": "GetAttachment6",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "me/calendargroups/:id/calendars/:id/events/:id/attachments/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get attachment\nRead the properties and relationships of an attachment, attached to an event,\nmessage, or post."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "71b9b3c8-3c22-460e-a50a-be143f4f33d9"
            }
          ]
        },
        {
          "id": "a5bd2253-a001-4da8-830f-e292c27458fd",
          "name": "GetAttachment4",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "users/:id | userPrincipalName/calendargroups/:id/calendars/:id/events/:id/attachments/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                },
                {
                  "id": "id | userPrincipalName",
                  "value": "id | userPrincipalName",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get attachment\nRead the properties and relationships of an attachment, attached to an event,\nmessage, or post."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "aba5a25c-96d2-4783-a300-f3292b68d0e9"
            }
          ]
        },
        {
          "id": "5257a130-3ed4-47ba-be06-1b7f5600461f",
          "name": "GetAttachment7",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "me/messages/:id/attachments/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get attachment\nRead the properties and relationships of an attachment, attached to an event,\nmessage, or post."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0066b08b-5a59-4f61-901f-2b86a00d6dfe"
            }
          ]
        },
        {
          "id": "796275ec-bb73-4c9f-81e4-c72eee7c6ef4",
          "name": "GetAttachment5",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "users/:id | userPrincipalName/messages/:id/attachments/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                },
                {
                  "id": "id | userPrincipalName",
                  "value": "id | userPrincipalName",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get attachment\nRead the properties and relationships of an attachment, attached to an event,\nmessage, or post."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b9e4fa22-edac-406b-a294-0cadd8d7f669"
            }
          ]
        },
        {
          "id": "de00d42b-b69f-4a9c-a8bc-57b62e1c2b51",
          "name": "GetAttachment8",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "me/mailFolders/:id/messages/:id/attachments/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get attachment\nRead the properties and relationships of an attachment, attached to an event,\nmessage, or post."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "de18bed8-d936-4930-a5d2-7c682a2eebd7"
            }
          ]
        },
        {
          "id": "d1c6c1f0-7911-46a4-a09a-d87be8685109",
          "name": "GetAttachment6",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "users/:id | userPrincipalName/mailFolders/:id/messages/:id/attachments/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                },
                {
                  "id": "id | userPrincipalName",
                  "value": "id | userPrincipalName",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get attachment\nRead the properties and relationships of an attachment, attached to an event,\nmessage, or post."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b2c95f14-799f-437b-b7ef-5ffc7499eb18"
            }
          ]
        },
        {
          "id": "33ad7a00-c050-4f9e-87f5-0b8ce8544550",
          "name": "AddAttachment",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "me/mailFolders/:id/childFolders/:id/.../messages/:id/attachments/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "Content-Type",
                "description": "Nature of the data in the body of an entity",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Add attachment Use this API to add an attachment to a message."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "87b2b3b8-5921-4cfc-bee9-55fcf7e2798c"
            }
          ]
        },
        {
          "id": "37e964d6-2cb9-4eb8-8cbd-8f96bd828893",
          "name": "AddAttachment",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "users/:id | userPrincipalName/mailFolders/:id/childFolders/:id/messages/:id/attachments/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                },
                {
                  "id": "id | userPrincipalName",
                  "value": "id | userPrincipalName",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "Content-Type",
                "description": "Nature of the data in the body of an entity",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Add attachment Use this API to add an attachment to a message."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8e610e40-f787-4f01-8155-0dd3f977989b"
            }
          ]
        },
        {
          "id": "5fd8889b-1f2a-4b0d-a6b2-2ab4e5b29305",
          "name": "GetAttachment9",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "groups/:id/threads/:id/posts/:id/attachments/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get attachment\nRead the properties and relationships of an attachment, attached to an event,\nmessage, or post."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b41fd621-6cba-4de9-8c2f-0b92c6f4c3cb"
            }
          ]
        },
        {
          "id": "d4b28fd0-f2bd-4fd3-a21f-3a49d12dbe8b",
          "name": "GetAttachment10",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "groups/:id/conversations/:id/threads/:id/posts/:id/attachments/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Get attachment\nRead the properties and relationships of an attachment, attached to an event,\nmessage, or post."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3e9080b3-6aed-4eb7-8b5e-443c60d3fb77"
            }
          ]
        },
        {
          "id": "e4357264-789f-4230-8ddf-4ec379ba8b23",
          "name": "AddAttachment1",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "me/events/:id/attachments"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "Content-Type",
                "description": "Nature of the data in the body of an entity",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Add attachment Use this API to add an attachment to an event. Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c84ee781-a897-4a1c-83f4-e9bff5d9e9d9"
            }
          ]
        },
        {
          "id": "e9986e5f-5dd1-4618-8248-0fb762572857",
          "name": "AddAttachment1",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "users/:id | userPrincipalName/events/:id/attachments"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                },
                {
                  "id": "id | userPrincipalName",
                  "value": "id | userPrincipalName",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "Content-Type",
                "description": "Nature of the data in the body of an entity",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Add attachment Use this API to add an attachment to an event. Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1c8ba245-cdc0-408d-a683-b516ff5c39d6"
            }
          ]
        },
        {
          "id": "2b265dc8-5bea-477e-969a-9e54b7a56952",
          "name": "AddAttachment2",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "groups/:id/events/:id/attachments"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "Content-Type",
                "description": "Nature of the data in the body of an entity",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Add attachment Use this API to add an attachment to an event. Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "aec0a49c-263d-4081-aa2d-db6d4ad506ac"
            }
          ]
        },
        {
          "id": "e1bf9c3b-78e1-429d-9bbc-f0ac93a48681",
          "name": "AddAttachment3",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "me/calendar/events/:id/attachments"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "Content-Type",
                "description": "Nature of the data in the body of an entity",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Add attachment Use this API to add an attachment to an event. Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c5ceaa21-88ec-46d9-a101-425f0c72d60b"
            }
          ]
        },
        {
          "id": "21bdf321-ba90-4796-b7f3-29e9976b7d13",
          "name": "AddAttachment2",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "users/:id | userPrincipalName/calendar/events/:id/attachments"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                },
                {
                  "id": "id | userPrincipalName",
                  "value": "id | userPrincipalName",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "Content-Type",
                "description": "Nature of the data in the body of an entity",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Add attachment Use this API to add an attachment to an event. Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c84af8d1-3125-4d97-9eaa-f48da892707a"
            }
          ]
        },
        {
          "id": "da6e0fb5-dd3e-4b12-94dc-d37e9b2220e3",
          "name": "AddAttachment4",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "groups/:id/calendar/events/:id/attachments"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "Content-Type",
                "description": "Nature of the data in the body of an entity",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Add attachment Use this API to add an attachment to an event. Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "edc7f963-4376-47d4-bd1b-f63d134228b4"
            }
          ]
        },
        {
          "id": "bcf36bfc-5166-40dc-9624-1ce0cc049d9a",
          "name": "AddAttachment5",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "me/calendars/:id/events/:id/attachments"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "Content-Type",
                "description": "Nature of the data in the body of an entity",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Add attachment Use this API to add an attachment to an event. Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "db09f035-21fd-41f1-b150-1dfa19da1c81"
            }
          ]
        },
        {
          "id": "0b481e18-6f08-42cd-a2d1-504a09c5f9de",
          "name": "AddAttachment3",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "users/:id | userPrincipalName/calendars/:id/events/:id/attachments"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                },
                {
                  "id": "id | userPrincipalName",
                  "value": "id | userPrincipalName",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "Content-Type",
                "description": "Nature of the data in the body of an entity",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Add attachment Use this API to add an attachment to an event. Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9c1cfeb2-b2af-43a4-9ea0-486eb362fb0d"
            }
          ]
        },
        {
          "id": "5cf5107e-cab7-42af-b3f1-bc06060df45a",
          "name": "AddAttachment6",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "me/calendargroup/calendars/:id/events/:id/attachments"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "Content-Type",
                "description": "Nature of the data in the body of an entity",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Add attachment Use this API to add an attachment to an event. Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "72785698-6bb8-4fe0-81f2-4f43a9671d2a"
            }
          ]
        },
        {
          "id": "889c161d-e0c8-4dc9-bb62-e2f94e150221",
          "name": "AddAttachment4",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "users/:id | userPrincipalName/calendargroup/calendars/:id/events/:id/attachments"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                },
                {
                  "id": "id | userPrincipalName",
                  "value": "id | userPrincipalName",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "Content-Type",
                "description": "Nature of the data in the body of an entity",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Add attachment Use this API to add an attachment to an event. Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c35570b3-6ff0-42a4-82ec-ea55dcfcd1ab"
            }
          ]
        },
        {
          "id": "4722d1f8-0066-4fae-b1f9-620e3a457c37",
          "name": "AddAttachment7",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "me/calendargroups/:id/calendars/:id/events/:id/attachments"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "Content-Type",
                "description": "Nature of the data in the body of an entity",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Add attachment Use this API to add an attachment to an event. Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "afe467dd-a765-46f3-b91c-d826741cf4db"
            }
          ]
        },
        {
          "id": "f65933a6-51b4-4d18-ab5b-d06c4912194b",
          "name": "AddAttachment5",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "users/:id | userPrincipalName/calendargroups/:id/calendars/:id/events/:id/attachments"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                },
                {
                  "id": "id | userPrincipalName",
                  "value": "id | userPrincipalName",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "Content-Type",
                "description": "Nature of the data in the body of an entity",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Add attachment Use this API to add an attachment to an event. Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fb82ac09-a28d-46ff-9e16-f62f8c3f4437"
            }
          ]
        },
        {
          "id": "31954ef0-1468-42d3-a5ca-d2be063c3359",
          "name": "AddAttachment8",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "me/messages/:id/attachments"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "Content-Type",
                "description": "Nature of the data in the body of an entity",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Add attachment Use this API to add an attachment to a message."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a0b51357-ff25-4dd2-8f02-6eb6d0a3804d"
            }
          ]
        },
        {
          "id": "87a50147-e909-4b53-ab10-5a0cb111de1c",
          "name": "AddAttachment6",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "users/:id | userPrincipalName/messages/:id/attachments"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                },
                {
                  "id": "id | userPrincipalName",
                  "value": "id | userPrincipalName",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "Content-Type",
                "description": "Nature of the data in the body of an entity",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Add attachment Use this API to add an attachment to a message."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1dec601b-025b-4d8e-9cb7-8e5502a954a5"
            }
          ]
        },
        {
          "id": "172addf8-6f92-43a4-b28f-b27e3c1e3d0f",
          "name": "AddAttachment9",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "me/mailFolders/:id/messages/:id/attachments"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "Content-Type",
                "description": "Nature of the data in the body of an entity",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Add attachment Use this API to add an attachment to a message."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0c9cc19f-42e9-4373-aa19-382fb9cae39e"
            }
          ]
        },
        {
          "id": "197ac7b2-9a25-4ad1-89f5-6288cad9abef",
          "name": "AddAttachment7",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "users/:id | userPrincipalName/mailFolders/:id/messages/:id/attachments"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                },
                {
                  "id": "id | userPrincipalName",
                  "value": "id | userPrincipalName",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "Content-Type",
                "description": "Nature of the data in the body of an entity",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Add attachment Use this API to add an attachment to a message."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3621a9d5-57fb-4d4c-a190-ef069f5d8dfe"
            }
          ]
        },
        {
          "id": "a3070adb-50bb-463a-a284-6f369aa4aab3",
          "name": "AddAttachment",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "groups/:id/threads/:id/posts/:id/attachments"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "header": [
              {
                "key": "Authorization",
                "value": "{}",
                "description": "Bearer",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Add attachment Use this API to add an attachment to a post. Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "97138672-c6a3-4224-b4da-8abdc585604e"
            }
          ]
        },
        {
          "id": "05f40d60-8b16-4ec3-bb7e-806262b24303",
          "name": "AddAttachment1",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "groups/:id/conversations/:id/threads/:id/posts/:id/attachments"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "header": [
              {
                "key": "Authorization",
                "value": "{}",
                "description": "Bearer",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Add attachment Use this API to add an attachment to a post. Since there is currently a limit of 4MB on the total size of each REST request, this limits the size of the attachment you can add to under 4MB."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6d1e5ee0-d0de-4bec-a759-7d55a241dea3"
            }
          ]
        }
      ]
    },
    {
      "name": "List",
      "item": [
        {
          "id": "bfb64f1d-ca64-4bff-ae96-13eeff14cbae",
          "name": "ListAttachments",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "me/mailFolders/:id/childFolders/:id/.../messages/:id/attachments/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "List attachments Retrieve a list of attachment objects attached to a message."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cdd426f3-6aa5-4313-8e51-2baa29afbb1f"
            }
          ]
        },
        {
          "id": "5d0706e5-26a8-48e9-a322-86678a5da087",
          "name": "ListAttachments",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "users/:id | userPrincipalName/mailFolders/:id/childFolders/:id/messages/:id/attachments/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                },
                {
                  "id": "id | userPrincipalName",
                  "value": "id | userPrincipalName",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "List attachments Retrieve a list of attachment objects attached to a message."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9c720ee1-9b5e-4ae0-b24f-836c7fc5f58c"
            }
          ]
        },
        {
          "id": "7d761f24-0fe3-40a3-b399-58ce93cee6d0",
          "name": "ListCalendarView",
          "request": {
            "url": "http://graph.microsoft.com/me/calendar/calendarView?endDateTime=endDateTime&startDateTime=startDateTime",
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "Authorization",
                "description": "Bearer",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "Content-Type",
                "description": "application/json",
                "disabled": false
              },
              {
                "key": "Prefer",
                "value": "Prefer",
                "description": "",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "List calendarView\nGet the occurrences, exceptions, and single instances of events in a calendar view defined by a time range,\nfrom the default calendar (../me/calendarview) of a user or group, or some other calendar of the user's."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b37c3dc8-ce4e-4cae-ae78-18d2a7360d41"
            }
          ]
        },
        {
          "id": "94683d99-26bb-441e-9bea-ae850bcced6a",
          "name": "ListCalendarView",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "users/:id | userPrincipalName/calendar/calendarView"
              ],
              "query": [
                {
                  "key": "endDateTime",
                  "value": "endDateTime",
                  "disabled": false
                },
                {
                  "key": "startDateTime",
                  "value": "startDateTime",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id | userPrincipalName",
                  "value": "id | userPrincipalName",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "{}",
                "description": "Bearer",
                "disabled": false
              },
              {
                "key": "Prefer",
                "value": "{}",
                "description": "outlook",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "List calendarView\nGet the occurrences, exceptions, and single instances of events in a calendar view defined by a time range,\nfrom the default calendar (../me/calendarview) of a user or group, or some other calendar of the user's."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fb469140-8b98-4064-aa48-dceb4b34eb5a"
            }
          ]
        },
        {
          "id": "9bd20f62-595d-4f78-ae72-b76e63a11969",
          "name": "ListCalendarView",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "groups/:id/calendar/calendarView"
              ],
              "query": [
                {
                  "key": "endDateTime",
                  "value": "endDateTime",
                  "disabled": false
                },
                {
                  "key": "startDateTime",
                  "value": "startDateTime",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Authorization",
                "value": "{}",
                "description": "Bearer",
                "disabled": false
              },
              {
                "key": "Prefer",
                "value": "{}",
                "description": "outlook",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "List calendarView\nGet the occurrences, exceptions, and single instances of events in a calendar view defined by a time range,\nfrom the default calendar (../me/calendarview) of a user or group, or some other calendar of the user's."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f27230c8-8a9e-4f92-bd11-ccb8684a4fd1"
            }
          ]
        },
        {
          "id": "1e199eb1-5f7c-496a-8c70-167c822a7c43",
          "name": "ListCalendarView",
          "request": {
            "url": {
              "protocol": "http",
              "host": "graph.microsoft.com",
              "path": [
                "me/calendars/:id/calendarView"
              ],
              "query": [
                {
                  "key": "endDateTime",
                  "value": "endDateTime",
                  "disabled": false
      