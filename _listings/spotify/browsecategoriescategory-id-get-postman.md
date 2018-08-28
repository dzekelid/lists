{
  "info": {
    "name": "Spotify Browse Category",
    "_postman_id": "e301cd7b-437b-4c9f-85c6-9f740915081e",
    "description": "[Get a Single Browse Category](https://developer.spotify.com/web-api/get-category/)",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "music",
      "item": [
        {
          "id": "4bd70aa7-a0aa-4315-9a83-06b36514916f",
          "name": "get-a-single-browse-categoryhttpsdeveloperspotifycomwebapigetcategory",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.spotify.com",
              "path": [
                "v1",
                "browse/categories/:category_id"
              ],
              "query": [
                {
                  "key": "country",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "locale",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "category_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "{}",
                "description": "It is used to set specified media type",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "[Get a Single Browse Category](https://developer"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "808152b0-17af-499b-a9f1-0dd600ac82bb"
            }
          ]
        }
      ]
    }
  ]
}