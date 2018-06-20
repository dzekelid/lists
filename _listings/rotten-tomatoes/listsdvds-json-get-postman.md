{
  "info": {
    "name": "Rotten Tomatoes Get Lists Dvds",
    "_postman_id": "e49e153b-4692-4257-9cff-62e014b3f041",
    "description": "Get lists dvds.json.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Lists",
      "item": [
        {
          "id": "3ee4465e-413a-47df-88df-2207d60cec42",
          "name": "getLists.json",
          "request": {
            "url": "http://api.rottentomatoes.com/api/public/v1.0/lists.json",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get lists.json."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "98b0d53d-dd93-4ff8-8c2d-cc7c9ec799fd"
            }
          ]
        },
        {
          "id": "5e4c6726-ccfe-4197-a52b-b146aec7e7af",
          "name": "getListsDvds.json",
          "request": {
            "url": "http://api.rottentomatoes.com/api/public/v1.0/lists/dvds.json",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get lists dvds.json."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1b5aa103-e263-4017-af08-f83a6a81e62a"
            }
          ]
        }
      ]
    }
  ]
}