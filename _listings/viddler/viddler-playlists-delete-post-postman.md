{
  "info": {
    "name": "Viddler  API Playlists Delete",
    "_postman_id": "6d0b81be-e470-48b9-8e0a-908e8a472962",
    "description": "Delete a playlist.u00a0Caution: This operation cannot be undone.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Viddler",
      "item": [
        {
          "id": "a8450772-0645-4252-b6ba-692eb961d71b",
          "name": "playlists-create",
          "request": {
            "url": "http://api.viddler.com/api/v2/viddler.playlists.create?max_age=%7B%7D&max_update_date=%7B%7D&max_views=%7B%7D&min_update_date=%7B%7D&min_views=%7B%7D&name=%7B%7D&playlist_visibility=%7B%7D&Regular Playlist Params (all optional)nnvideo_ids=%7B%7D&sessionid=%7B%7D&Smart Playlist Params (all optional)nnusers=%7B%7D&sort=%7B%7D&tags=%7B%7D&type=%7B%7D&visibility=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Create a playlist. Regular playlist represents user defined videos. Smart playlist updates in realtime returning videos matching selected filtering rules."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "90267abe-bc53-4596-95b7-a25cba7fd2fa"
            }
          ]
        },
        {
          "id": "825fb767-7b8e-4935-8b62-e6e86fe78d5f",
          "name": "playlists-delete",
          "request": {
            "url": "http://api.viddler.com/api/v2/viddler.playlists.delete?playlist_id=%7B%7D&sessionid=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Delete a playlist.u00a0Caution: This operation cannot be undone."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ff74fe94-8d16-46d6-a608-49d8e3bd00bf"
            }
          ]
        }
      ]
    }
  ]
}