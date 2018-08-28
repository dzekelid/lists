{
  "info": {
    "name": "Dezrez Return list of tasks, corresponding to task ids passed in.",
    "_postman_id": "e5231402-a679-49b4-b522-9fda2e942d2c",
    "description": "Return list of tasks, corresponding to task ids passed in..",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Count",
      "item": [
        {
          "id": "44d263bf-a44c-416f-8929-1d22595090a1",
          "name": "Chat_UnreadSummary",
          "request": {
            "url": "http://api.dezrez.com/api/chat/unreadsummary",
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
            "description": "Get a count of unread chat messages for the negotiator plus a list of corresponding message id's which are unread.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dd996df2-a284-4098-9cd5-d27d12c59d4b"
            }
          ]
        }
      ]
    },
    {
      "name": "Return",
      "item": [
        {
          "id": "7ca17740-ac4b-46d6-a328-5006107d7d26",
          "name": "DefaultToDo_GetTodosByIdByids",
          "request": {
            "url": "http://api.dezrez.com/api/todo/gettodosbyid?ids=%7B%7D",
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
            "description": "Return list of tasks, corresponding to task ids passed in.."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9ab9ce0a-0125-407e-b3e5-7a27b13d1738"
            }
          ]
        }
      ]
    }
  ]
}