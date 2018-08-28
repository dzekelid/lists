{
  "info": {
    "name": "Elastic Email SMTP API Delete Existing Subscriber",
    "_postman_id": "f798248d-7b40-49be-908e-5ec09c9735d4",
    "description": "Delete Existing Subscriber",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Attachments",
      "item": [
        {
          "id": "54710289-3180-4c41-9cae-85b91f6a4059",
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
              "id": "301bfb1c-5ef2-4b45-ac4d-3278d7fabafa"
            }
          ]
        }
      ]
    },
    {
      "name": "Lists",
      "item": [
        {
          "id": "8c63fd2f-5cb7-45d7-8748-6345064e29c6",
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
              "id": "dd3ac873-58ec-4e1d-97b8-4f2730066cbd"
            }
          ]
        },
        {
          "id": "32b08bb7-7ef4-47b5-bfec-e1bcd1ed3e14",
          "name": "getListsCreateContact",
          "request": {
            "url": "http://api.elasticemail.com/lists/create-contact?api_key=%7B%7D&birthdate=%7B%7D&city=%7B%7D&country=%7B%7D&email=%7B%7D&firstname=%7B%7D&gender=%7B%7D&lastname=%7B%7D&listname=%7B%7D&organizationname=%7B%7D&phone=%7B%7D&postalcode=%7B%7D&state=%7B%7D&the zip or postal code of the subscriber=%7B%7D&title=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Create New Subscriber"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cd2c23b2-546a-42b5-9fdf-7a5e2affabbf"
            }
          ]
        },
        {
          "id": "0e53f500-de6b-449d-afa3-a1d1d9a89331",
          "name": "getListsCreateLists",
          "request": {
            "url": "http://api.elasticemail.com/lists/create-lists?api_key=%7B%7D&listname=%7B%7D&username=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Create New List"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "794f3aed-c00c-48b6-bd5b-07c8a98ab619"
            }
          ]
        },
        {
          "id": "97bee973-dab5-48a7-aa7b-1ce5e9aadfb1",
          "name": "getListsDelete",
          "request": {
            "url": "http://api.elasticemail.com/lists/delete?api_key=%7B%7D&listname=%7B%7D&username=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Delete Existing List"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f1b34fe2-4c4a-4ec2-aca8-ba61f2a5e17e"
            }
          ]
        },
        {
          "id": "6da52154-6982-4420-9de2-efd0515a74c0",
          "name": "getListsDeleteContact",
          "request": {
            "url": "http://api.elasticemail.com/lists/delete-contact?api_key=%7B%7D&email=%7B%7D&username=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Delete Existing Subscriber"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8348c6f2-f12b-4d8e-985c-b5de141859d0"
            }
          ]
        }
      ]
    }
  ]
}