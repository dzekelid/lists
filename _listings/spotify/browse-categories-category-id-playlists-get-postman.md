{
  "info": {
    "name": "Spotify Browse Category Playlists",
    "_postman_id": "7334fafa-40fb-40ec-bed1-bc207e8cda57",
    "description": "[Get a Category's playlists](https://developer.spotify.com/web-api/get-categorys-playlists/)",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "music",
      "item": [
        {
          "id": "62f15313-4100-40d6-b990-95646ddf33ba",
          "name": "get-a-categorys-playlistshttpsdeveloperspotifycomwebapigetcategorysplaylists",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.spotify.com",
              "path": [
                "v1",
                "browse/categories/:category_id/playlists"
              ],
              "query": [
                {
                  "key": "country",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "limit",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "offset",
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
            "description": "[Get a Category's playlists](https://developer"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e354f272-40f3-4305-b71c-0e2ee1cafca4"
            }
          ]
        }
      ]
    }
  ]
}