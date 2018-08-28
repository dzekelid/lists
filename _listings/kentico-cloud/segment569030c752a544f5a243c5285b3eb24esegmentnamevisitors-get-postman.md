{
  "info": {
    "name": "Kentico Cloud List visitors of a segment",
    "_postman_id": "c9693f67-3183-416d-ad5c-717c4b91184e",
    "description": "Retrieve visitors that match the specified segment.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "List",
      "item": [
        {
          "id": "3de34ff4-c62c-4557-823d-adcd25251691",
          "name": "Segment569030c752a544f5A243C5285b3eb24eVisitorsBySegmentNameGet",
          "request": {
            "url": {
              "protocol": "http",
              "host": "deliver.kenticocloud.com",
              "path": [
                "segment/569030c7-52a5-44f5-a243-c5285b3eb24e/:SegmentName/visitors"
              ],
              "variable": [
                {
                  "id": "SegmentName",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
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
            "description": "Retrieve visitors that match the specified segment."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0700f0a6-c4b9-405d-9a08-487dd566ea03"
            }
          ]
        }
      ]
    }
  ]
}