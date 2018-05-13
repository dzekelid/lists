{
  "info": {
    "name": "Spotify Browse Featured Playlists",
    "_postman_id": "ac6917ca-5e43-419a-874e-32913004aca2",
    "description": "[Get a List of Featured Playlists](https://developer.spotify.com/web-api/get-list-featured-playlists/)",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "music",
      "item": [
        {
          "id": "07a962a3-2dea-4c73-8cb5-dd41e7d57cba",
          "name": "get-a-list-of-featured-playlistshttpsdeveloperspotifycomwebapigetlistfeaturedplaylists",
          "request": {
            "url": "http://api.spotify.com/v1/browse/featured-playlists?country=%7B%7D&limit=%7B%7D&locale=%7B%7D&offset=%7B%7D&timestamp=%7B%7D",
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
            "description": "[Get a List of Featured Playlists](https://developer"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d92693e6-0c08-4bbc-aa96-a2d387d95806"
            }
          ]
        }
      ]
    }
  ]
}