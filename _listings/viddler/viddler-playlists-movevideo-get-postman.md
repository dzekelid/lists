{
  "info": {
    "name": "Viddler  API Playlists MoveVideo",
    "_postman_id": "88af6971-4ad2-422a-941f-c3e953a8d008",
    "description": "Reorder videos in regular playlist.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Viddler",
      "item": [
        {
          "id": "eb13fd46-eeaa-4831-93d2-dcae85220034",
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
              "id": "53a0dde3-ecd5-4b66-964f-df99d2dc31b7"
            }
          ]
        },
        {
          "id": "92e6ed43-6d17-4333-99e8-913954d5ecb6",
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
              "id": "9335104a-9121-4202-a082-6cfc7b7c75c0"
            }
          ]
        },
        {
          "id": "9ad12566-8ed4-4d3f-8e05-8c8b5f45d37a",
          "name": "playlists-list",
          "request": {
            "url": "http://api.viddler.com/api/v2/viddler.playlists.list?page=%7B%7D&per_page=%7B%7D&sessionid=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List all playlists for an account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "812012e0-6b30-4efd-9c6f-61c6b98c2ce0"
            }
          ]
        },
        {
          "id": "1c23139d-e0d8-479b-a9fb-aad74bdb0af9",
          "name": "playlists-movevideo",
          "request": {
            "url": "http://api.viddler.com/api/v2/viddler.playlists.moveVideo?from=%7B%7D&playlist_id=%7B%7D&sessionid=%7B%7D&to=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Reorder videos in regular playlist."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1ae16083-a8bb-4cca-8bca-8ce86ed3bc2a"
            }
          ]
        }
      ]
    }
  ]
}