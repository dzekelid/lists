{
  "info": {
    "name": "Elastic Email SMTP API Add Existing Subscriber To List",
    "_postman_id": "55580438-862c-4f0a-9018-ce520801ebe3",
    "description": "Add Existing Subscriber To List",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Attachments",
      "item": [
        {
          "id": "d578eeb1-16ab-480f-a5df-6aab99741b46",
          "name": "getAttachmentsUpload",
          "request": {
            "url": "http://api.elasticemail.com/attachments/upload/?api_key=%7B%7D&file=%7B%7D&username=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "The upload attachment command is used to upload an attachment for sending."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "58426121-568f-4ac6-9319-57643b58b68c"
            }
          ]
        }
      ]
    },
    {
      "name": "Lists",
      "item": [
        {
          "id": "f7d6ddd9-dde4-4d67-986e-c682122986cb",
          "name": "getListsAddContact",
          "request": {
            "url": "http://api.elasticemail.com/lists/add-contact?api_key=%7B%7D&listname=%7B%7D&username=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Add Existing Subscriber To List"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d6b862c7-af3b-4a2f-943e-dbc46697bc17"
            }
          ]
        }
      ]
    }
  ]
}