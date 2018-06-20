{
  "info": {
    "name": "Spotify Get User Playlist Tracks",
    "_postman_id": "ad3e5058-db99-4106-bf6a-b216d2bbe131",
    "description": "[Get a Playlist's Tracks](https://developer.spotify.com/web-api/get-playlists-tracks/)",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "music",
      "item": [
        {
          "id": "4006c0d8-33e2-4755-8a50-c0f3ebe01fde",
          "name": "get-a-playlists-trackshttpsdeveloperspotifycomwebapigetplayliststracks",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.spotify.com",
              "path": [
                "v1",
                "users/:user_id/playlists/:playlist_id/tracks"
              ],
              "query": [
                {
                  "key": "fields",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "limit",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "market",
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
                  "id": "playlist_id",
                  "value": "{}",
                  "type": "string"
                },
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
            "description": "[Get a Playlist's Tracks](https://developer"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4601e7f0-b4db-4a94-9f78-dfc463595154"
            }
          ]
        }
      ]
    }
  ]
}