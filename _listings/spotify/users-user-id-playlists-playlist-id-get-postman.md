{
  "info": {
    "name": "Spotify Get User Playlist",
    "_postman_id": "d62680a2-2bb7-4ea0-b110-03ada28f70d3",
    "description": "[Get a Playlist](https://developer.spotify.com/web-api/get-playlist/)",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "music",
      "item": [
        {
          "id": "415a1907-b704-43a5-a125-37218351cb64",
          "name": "get-a-playlisthttpsdeveloperspotifycomwebapigetplaylist",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.spotify.com",
              "path": [
                "v1",
                "users/:user_id/playlists/:playlist_id"
              ],
              "query": [
                {
                  "key": "fields",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "market",
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
            "description": "[Get a Playlist](https://developer"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ea0799c5-2e1a-418b-bc7c-28ccf1fe3d0f"
            }
          ]
        }
      ]
    }
  ]
}