{
  "info": {
    "name": "Mailjet Messages API Message List",
    "_postman_id": "37858211-b73c-4f2d-a05f-4f7452d58838",
    "description": "Allows you to list messages.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Message",
      "item": [
        {
          "id": "e3e6b5a6-9f11-4cbe-98e9-30bf1ebdf2b4",
          "name": "getMessage",
          "request": {
            "url": "http://api.mailjet.com/v3/REST/message/?Campaign=%7B%7D&Contact=%7B%7D&MessageState=%7B%7D&PlanSubscription=%7B%7D&Sender=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Allows you to list messages."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5cae9d71-7e75-476e-8354-40f1fc949da0"
            }
          ]
        }
      ]
    }
  ]
}