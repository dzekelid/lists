{
  "info": {
    "name": "Kentico Cloud List segments of a visitor",
    "_postman_id": "1c8e89b3-dcd0-41ed-8e83-21aa9108f8b8",
    "description": "Retrieve the names of segments that the specified visitor belongs to.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "List",
      "item": [
        {
          "id": "b1de116f-4fbb-4c83-9920-4faab39b813f",
          "name": "Segment569030c752a544f5A243C5285b3eb24eVisitorsBySegmentNameGet",
          "request": {
            "url": {
              "protocol": "http",
              "host": "deliver.kenticocloud.com",
              "path": [
                "segment/569030c7-52a5-44f5-a243-c5285b3eb24e/:SegmentName/visitors"
              ],
              "variable": [
                {
                  "id": "SegmentName",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve visitors that match the specified segment."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c83f4ccd-5237-40b0-9c3f-b8769dcb1a93"
            }
          ]
        },
        {
          "id": "2464cff5-1eb8-41ac-b3fb-eba85fe45ab6",
          "name": "Visitor569030c752a544f5A243C5285b3eb24e7888c9a3824a11f1SegmentsGet",
          "request": {
            "url": "http://deliver.kenticocloud.com/visitor/569030c7-52a5-44f5-a243-c5285b3eb24e/7888c9a3824a11f1/segments",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve the names of segments that the specified visitor belongs to."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "672f5c33-f9f5-48dd-9f4d-1fe711a5a720"
            }
          ]
        }
      ]
    },
    {
      "name": "Retrieving",
      "item": [
        {
          "id": "e4ee3e4f-e629-422d-8f22-c87d410a7c10",
          "name": "Visitor569030c752a544f5A243C5285b3eb24eE3e9e191a12b9257SegmentGet",
          "request": {
            "url": "http://deliver.kenticocloud.com/visitor/569030c7-52a5-44f5-a243-c5285b3eb24e/e3e9e191a12b9257/segment",
            "method": "GET",
            "header": [
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "",
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
            "description": "Use the Personalization API to retrieve the list of segments that the specified visitor belongs to.\n\n* Authenticate the request using your Personalization API Key.\n* Specify the User ID of the visitor you are asking about.\n \nSee <https://developer.kenticocloud.com/docs/personalizing-content#section-retrieving-visitor-s-segments> for more details."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "92c7dd05-1c8d-41e8-8fc9-5eaa26081661"
            }
          ]
        }
      ]
    },
    {
      "name": "View",
      "item": [
        {
          "id": "cdc79ff0-7998-4b8c-b531-b2b569f4bfa0",
          "name": "Uid7888c9a3824a11f1Get",
          "request": {
            "url": "http://deliver.kenticocloud.com/uid/7888c9a3824a11f1",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "View data of visitor by ID"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "80c4cce2-0e45-499f-a7b8-eaf0a516a6a5"
            }
          ]
        },
        {
          "id": "f8b9547c-9857-4c5a-a6fc-4b10753e36e5",
          "name": "EmailLolaMiraBlablaComGet",
          "request": {
            "url": "http://deliver.kenticocloud.com/email/lola.mira@blabla.com",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "View data of visitor by email"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8441e98d-3830-45b0-9260-af93a7533bba"
            }
          ]
        }
      ]
    },
    {
      "name": "Data",
      "item": [
        {
          "id": "57dc2524-f55b-4dd5-873c-c7bbffbd7e07",
          "name": "Uid7888c9a3824a11f1Delete",
          "request": {
            "url": "http://deliver.kenticocloud.com/uid/7888c9a3824a11f1",
            "method": "DELETE",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Delete data of visitor by ID"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ec62ad80-c0ec-4f65-afd9-08c5c402482d"
            }
          ]
        },
        {
          "id": "7811f31e-7f41-4b85-a754-0ebff268721e",
          "name": "EmailLolaMiraBlablaComDelete",
          "request": {
            "url": "http://deliver.kenticocloud.com/email/lola.mira@blabla.com",
            "method": "DELETE",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Delete data of visitor by email"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f7098356-5418-4bf2-98cf-285474e7dde4"
            }
          ]
        }
      ]
    }
  ]
}