{
  "info": {
    "name": "LiveChat List all canned responses1",
    "_postman_id": "a9ccff7c-5f24-445c-8927-197df837a45b",
    "description": "Returns the list of all currently set canned responses.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Webhook",
      "item": [
        {
          "id": "472b3c40-a88f-4c4b-b4de-198145b28fd8",
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
              "id": "fb2cf4af-b49d-46e2-8349-faf7654588d6"
            }
          ]
        }
      ]
    },
    {
      "name": "Chat",
      "item": [
        {
          "id": "b49f9428-e11c-4cf7-aa20-3445f1df83ed",
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
              "id": "09c7a113-238e-4eca-99b9-d4481ec98f79"
            }
          ]
        }
      ]
    },
    {
      "name": "List",
      "item": [
        {
          "id": "bd04629a-8c67-4566-b9c2-d4ca6ff70e08",
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
              "id": "e92296ed-3c19-4cf7-ad50-81ab0d74b504"
            }
          ]
        }
      ]
    }
  ]
}