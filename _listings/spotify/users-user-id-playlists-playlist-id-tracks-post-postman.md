{
  "info": {
    "name": "Spotify Add User Playlist Track",
    "_postman_id": "1aa988e5-f40a-4b90-a059-a12027b3f1a0",
    "description": "[Add Tracks to a Playlist](https://developer.spotify.com/web-api/add-tracks-to-playlist/)",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "music",
      "item": [
        {
          "id": "18cb6e82-8b1a-4338-bc57-40e841dfdaff",
          "name": "add-tracks-to-a-playlisthttpsdeveloperspotifycomwebapiaddtrackstoplaylist",
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
                  "key": "position",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "uris",
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
            "method": "POST",
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
            "description": "[Add Tracks to a Playlist](https://developer"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8208cb9b-9eb2-4884-a636-2e6365800093"
            }
          ]
        }
      ]
    }
  ]
}