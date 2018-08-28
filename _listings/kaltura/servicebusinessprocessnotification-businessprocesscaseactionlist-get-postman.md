{
  "info": {
    "name": "Kaltura VPaaS Get Service Businessprocessnotification Businessprocesscase Action List",
    "_postman_id": "0f05c236-0c1d-4b7f-a964-ca451ced9e8d",
    "description": "list business-process cases",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Service",
      "item": [
        {
          "id": "2e25758a-8821-47ef-b970-8a0d4ef5a817",
          "name": "businessProcessCase.abort",
          "request": {
            "url": "http://www.kaltura.com/api_v3/service/businessprocessnotification_businessprocesscase/action/abort?businessProcessStartNotificationTemplateId=%7B%7D&No Name=%7B%7D&objectId=%7B%7D&objectType=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Abort business-process case"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d934c142-51d8-4494-ae23-aaec02e51ebf"
            }
          ]
        },
        {
          "id": "f1f80867-942f-462f-8bbd-bc2d643b4654",
          "name": "businessProcessCase.list",
          "request": {
            "url": "http://www.kaltura.com/api_v3/service/businessprocessnotification_businessprocesscase/action/list?No Name=%7B%7D&objectId=%7B%7D&objectType=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "list business-process cases"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f0578ced-88a4-460a-902c-02ddc1d58159"
            }
          ]
        }
      ]
    }
  ]
}