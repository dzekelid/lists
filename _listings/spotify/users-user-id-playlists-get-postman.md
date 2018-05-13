{
  "info": {
    "name": "Spotify Get User Playlists",
    "_postman_id": "18843523-0a81-4993-9710-443f66909f09",
    "description": "[Get a List of a User's Playlists](https://developer.spotify.com/web-api/get-list-users-playlists/)",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "music",
      "item": [
        {
          "id": "206d5837-5f40-48ff-9aeb-c4aee0c7f000",
          "name": "get-a-list-of-a-users-playlistshttpsdeveloperspotifycomwebapigetlistusersplaylists",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.spotify.com",
              "path": [
                "v1",
                "users/:user_id/playlists"
              ],
              "query": [
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
                  "id": "user_id",
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
            "description": "[Get a List of a User's Playlists](https://developer"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "de59edba-7153-4116-9d27-2861a7abaace"
            }
          ]
        }
      ]
    }
  ]
}