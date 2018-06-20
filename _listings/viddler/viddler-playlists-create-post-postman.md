{
  "info": {
    "name": "Viddler  API Playlists Create",
    "_postman_id": "06abe4f0-3f87-4397-81e6-116ec442fea0",
    "description": "Create a playlist. Regular playlist represents user defined videos. Smart playlist updates in realtime returning videos matching selected filtering rules.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Viddler",
      "item": [
        {
          "id": "ea1c50c9-2de8-4589-a578-523480bd3841",
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
              "id": "a66a849f-c22b-4d6d-b3a3-dd828b45f753"
            }
          ]
        }
      ]
    }
  ]
}