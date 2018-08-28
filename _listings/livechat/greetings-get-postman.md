{
  "info": {
    "name": "LiveChat List all greetings",
    "_postman_id": "42619ae8-0eec-4dd3-97b3-df63e1add65f",
    "description": "Returns the list of all greetings.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Webhook",
      "item": [
        {
          "id": "1e703f73-ee96-4c5c-be6b-4d6ab141a738",
          "name": "Webhooks12345Delete",
          "request": {
            "url": "http://api.livechatinc.com/webhooks/12345",
            "method": "DELETE",
            "header": [
              {
                "key": "X-API-Version",
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
            "description": "Deletes a webhook with the given ID."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c41d043a-e8f5-4904-8b79-c01efa617416"
            }
          ]
        }
      ]
    },
    {
      "name": "Chat",
      "item": [
        {
          "id": "6ea51ba8-640b-496c-bf05-9d4f109d3218",
          "name": "ReportsChatsRatingsGet",
          "request": {
            "url": "http://api.livechatinc.com/reports/chats/ratings?date_from=%7B%7D&date_to=%7B%7D&group=%7B%7D&group_by=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "X-API-Version",
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
            "description": "Shows how many chats have been rated and how they have been rated during a specified period."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ac1e9234-06ab-44fc-822a-c49fef3a3657"
            }
          ]
        },
        {
          "id": "5589934c-1438-4850-9cca-3df58b528c32",
          "name": "ReportsChatsEngagementGet",
          "request": {
            "url": "http://api.livechatinc.com/reports/chats/engagement?agent=%7B%7D&date_from=%7B%7D&date_to=%7B%7D&group_by=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "X-API-Version",
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
            "description": "This report shows you where you get your chats from. They can come from i.e. automatic invitations, manual invitations or the visitors can start the chats by themselves."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ff8cad77-7825-49ba-995b-20f3f0c3aa3b"
            }
          ]
        }
      ]
    },
    {
      "name": "List",
      "item": [
        {
          "id": "0fec325a-e539-472b-a361-50c4cca2e2ae",
          "name": "CannedResponsesABC123Get",
          "request": {
            "url": "http://api.livechatinc.com/canned_responses/ABC123",
            "method": "GET",
            "header": [
              {
                "key": "X-API-Version",
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
            "description": "Returns the list of all currently set canned responses."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2bce278d-ba32-4d48-8549-49221071faa7"
            }
          ]
        },
        {
          "id": "34377f48-1c28-4621-87a2-669a189bb545",
          "name": "GreetingsGet",
          "request": {
            "url": "http://api.livechatinc.com/greetings?groups=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "X-API-Version",
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
            "description": "Returns the list of all greetings."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "88a57997-7d7a-4c2d-bef0-4bd34159631f"
            }
          ]
        }
      ]
    },
    {
      "name": "Canned",
      "item": [
        {
          "id": "f0078247-39ca-49e8-aaf7-cbdd6d3e2e33",
          "name": "CannedResponsesABC123Put",
          "request": {
            "url": "http://api.livechatinc.com/canned_responses/ABC123",
            "method": "PUT",
            "header": [
              {
                "key": "X-API-Version",
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
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "tags[0]",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                }
              ]
            },
            "description": "Updates the specified canned response by setting the values of the parameters passed. Any parameters not provided will be left unchanged."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8bc48cbe-56e8-4e04-a699-3bd49a84cfc3"
            }
          ]
        }
      ]
    },
    {
      "name": "Remove",
      "item": [
        {
          "id": "6971d3fc-2f3d-46c2-843a-d8bd7b19162a",
          "name": "CannedResponsesABC123Delete",
          "request": {
            "url": "http://api.livechatinc.com/canned_responses/ABC123",
            "method": "DELETE",
            "header": [
              {
                "key": "X-API-Version",
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
            "description": "Removes a canned response with the given CANNED_RESPONSE_ID."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "542dcf27-cf63-41c8-bb0f-9e8116aeb449"
            }
          ]
        },
        {
          "id": "61558e6a-2c3a-4e17-981a-43c37844b607",
          "name": "GroupsABC123Delete2",
          "request": {
            "url": "http://api.livechatinc.com/groups/ABC123",
            "method": "DELETE",
            "header": [
              {
                "key": "X-API-Version",
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
            "description": "Removes a group with the given GROUP_ID."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2671b605-a31f-4d51-b140-d9fd86b44b9f"
            }
          ]
        }
      ]
    },
    {
      "name": "Group",
      "item": [
        {
          "id": "edff7134-c1bb-4e44-993a-d5e7907cdead",
          "name": "GroupsABC123Put",
          "request": {
            "url": "http://api.livechatinc.com/groups/ABC123",
            "method": "PUT",
            "header": [
              {
                "key": "X-API-Version",
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
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "agents[0]",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "agents[1]",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "name",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                }
              ]
            },
            "description": "Updates the specified group by setting the values of the parameters passed. Any parameters not provided will be left unchanged."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9759b573-3fbc-4223-9a72-ad047068e65a"
            }
          ]
        }
      ]
    }
  ]
}