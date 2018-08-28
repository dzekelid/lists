{
  "info": {
    "name": "Rotten Tomatoes Get Lists",
    "_postman_id": "9115a916-d8af-408e-8215-fbf8ff85c321",
    "description": "Get lists.json.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Lists",
      "item": [
        {
          "id": "2c069d20-7b4f-44d3-a5e9-8c6eb49152e7",
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
              "id": "54cfd9f3-c7cf-43c6-9795-5e4dbfb90d57"
            }
          ]
        }
      ]
    }
  ]
}