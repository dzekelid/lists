{
  "info": {
    "name": "Viddler  API Playlists List",
    "_postman_id": "59052675-6e4c-41c8-9ac8-516afc040866",
    "description": "List all playlists for an account.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Viddler",
      "item": [
        {
          "id": "2d647c6c-4005-48fa-814e-b9238a52e205",
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
              "id": "ba7d8041-694d-4555-94fb-468b3270439d"
            }
          ]
        },
        {
          "id": "04fdbe39-f5d4-4873-9689-eaf02c46b409",
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
              "id": "8772e8a4-b286-4eac-84b5-8a4f3034d45f"
            }
          ]
        },
        {
          "id": "7809e483-0925-4b79-8263-2bc0211f9426",
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
              "id": "73b54a6f-bb6a-47e5-9780-3c6ed2036d25"
            }
          ]
        }
      ]
    }
  ]
}