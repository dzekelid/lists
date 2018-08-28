{
  "info": {
    "name": "Spotify Get User Playlist Followers Contains",
    "_postman_id": "006b4847-230d-4d5a-ac56-29b1e73b01f3",
    "description": "[Check if Users Follow a Playlist](https://developer.spotify.com/web-api/check-user-following-playlist/)",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "music",
      "item": [
        {
          "id": "cf57509e-3024-4d3a-a2b9-286ad69289cb",
          "name": "check-if-users-follow-a-playlisthttpsdeveloperspotifycomwebapicheckuserfollowingplaylist",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.spotify.com",
              "path": [
                "v1",
                "users/:user_id/playlists/:playlist_id/followers/contains"
              ],
              "query": [
                {
                  "key": "ids",
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
            "body": {
              "mode": "raw"
            },
            "description": "[Check if Users Follow a Playlist](https://developer"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0b116b28-306e-4919-a4d4-3d1fd1861ff1"
            }
          ]
        }
      ]
    }
  ]
}