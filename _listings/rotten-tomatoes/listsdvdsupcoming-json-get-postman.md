{
  "info": {
    "name": "Rotten Tomatoes Get Lists Dvds Upcoming",
    "_postman_id": "c0e5e47d-698f-4640-89b4-d6122e5b30e0",
    "description": "Get lists dvds upcoming.json.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Lists",
      "item": [
        {
          "id": "d62951da-1821-416b-8957-0e9fb84cb58f",
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
              "id": "88e9e587-47b1-4c49-a99b-efd22bff6e12"
            }
          ]
        },
        {
          "id": "487d0e1b-3186-41ac-ad1c-2d1edd3d66cb",
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
              "id": "441b4ff3-9ef9-40c7-80fc-8d95272369c7"
            }
          ]
        },
        {
          "id": "81a67862-dfd5-4c94-8b75-0f94baa87fa2",
          "name": "getListsDvdsCurrentReleases.json",
          "request": {
            "url": "http://api.rottentomatoes.com/api/public/v1.0/lists/dvds/current_releases.json?country=%7B%7D&page=%7B%7D&page_limit=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get lists dvds current releases.json."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ae26bcc7-118f-4db7-bf57-838d5d7cfc12"
            }
          ]
        },
        {
          "id": "e72c39ab-5dbb-4c7d-9fa7-65a579eb900e",
          "name": "getListsDvdsNewReleases.json",
          "request": {
            "url": "http://api.rottentomatoes.com/api/public/v1.0/lists/dvds/new_releases.json?country=%7B%7D&page=%7B%7D&page_limit=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get lists dvds new releases.json."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "81cdc458-7d6a-4641-98e5-d8cc54957057"
            }
          ]
        },
        {
          "id": "76741bc6-6169-4ae0-a2e9-15d89263b92a",
          "name": "getListsDvdsTopRentals.json",
          "request": {
            "url": "http://api.rottentomatoes.com/api/public/v1.0/lists/dvds/top_rentals.json?country=%7B%7D&limit=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get lists dvds top rentals.json."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e96c474a-52ff-4324-816b-b2dac0df05c4"
            }
          ]
        },
        {
          "id": "6d2cc9ef-f457-41a0-b245-8cce255c6226",
          "name": "getListsDvdsUpcoming.json",
          "request": {
            "url": "http://api.rottentomatoes.com/api/public/v1.0/lists/dvds/upcoming.json?country=%7B%7D&page=%7B%7D&page_limit=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get lists dvds upcoming.json."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a4df8d80-c372-4100-8fdc-d273dbd8837c"
            }
          ]
        }
      ]
    }
  ]
}