{
  "info": {
    "name": "Plentymarkets List newsletter entries",
    "_postman_id": "49f11ac8-2e07-42c5-8b3a-2e79a89d259d",
    "description": "List newsletter entries.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "List",
      "item": [
        {
          "id": "745e3629-1529-4158-b9ce-066050131b36",
          "name": "getRestNewsletters",
          "request": {
            "url": "http://example.com/rest/newsletters",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "List newsletter entries."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e8e283c7-c4d3-4712-a018-df9e59e528fb"
            }
          ]
        }
      ]
    }
  ]
}