{
  "info": {
    "name": "Spotify Delete User Playlist Followers",
    "_postman_id": "225131bf-a532-4024-85aa-eae66aa7af73",
    "description": "[Unfollow a Playlist](https://developer.spotify.com/web-api/unfollow-playlist/)",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "music",
      "item": [
        {
          "id": "6dda1be4-417d-4109-98a9-2c25b8a27730",
          "name": "unfollow-a-playlisthttpsdeveloperspotifycomwebapiunfollowplaylist",
          "request": {
            "url": {
              "protocol": "http",
              "host": "api.spotify.com",
              "path": [
                "v1",
                "users/:user_id/playlists/:playlist_id/followers"
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
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "[Unfollow a Playlist](https://developer"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "aaec0c5b-85df-453b-8505-d6a38a16c6bf"
            }
          ]
        }
      ]
    }
  ]
}