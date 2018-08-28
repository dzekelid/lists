{
  "info": {
    "name": "Foursquare Get Campaigns List",
    "_postman_id": "7b8db1bb-c954-450c-bf14-734489639a73",
    "description": "/campaigns/add",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Campaigns",
      "item": [
        {
          "id": "b4547fea-cb0d-4505-a916-be80eb7a0642",
          "name": "campaignscampaign-id",
          "request": {
            "url": "http://api.foursquare.com/v2/campaigns/add?campaignId=%7B%7D&endAt=%7B%7D&groupId=%7B%7D&specialId=%7B%7D&startAt=%7B%7D&v=%7B%7D&venueId=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "/campaigns/{CAMPAIGN_ID}"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f2ec4ea2-f825-4fd3-b9b4-c5977d658c16"
            }
          ]
        },
        {
          "id": "515b94b5-f441-4cec-a072-d2d4ae290d89",
          "name": "campaignsadd",
          "request": {
            "url": "http://api.foursquare.com/v2/campaigns/list?groupId=%7B%7D&specialId=%7B%7D&status=%7B%7D&v=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "/campaigns/add"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0310975a-7af7-4d08-8153-56bcb95e8fa5"
            }
          ]
        }
      ]
    }
  ]
}