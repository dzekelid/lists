{
  "info": {
    "name": "Plentymarkets List comments",
    "_postman_id": "3507f409-4517-40f6-bd23-0c81cab412e7",
    "description": "Lists comments. The reference type and the reference value must be specified (e.g. the reference type is 'order' and the reference value is the ID of the order).",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "List",
      "item": [
        {
          "id": "14c6c9d4-53aa-4522-97e7-565ef7cd6b66",
          "name": "getRestCommentsReferencetypeReferencevalue",
          "request": {
            "url": {
              "protocol": "http",
              "host": "example.com",
              "path": [
                "rest/comments/:referenceType/:referenceValue"
              ],
              "query": [
                {
                  "key": "isVisibleForContact",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "userId",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "referenceType",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "referenceValue",
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
            "description": "Lists comments. The reference type and the reference value must be specified (e.g. the reference type is 'order' and the reference value is the ID of the order)."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3894b272-aee9-4d20-ad4a-9fe15b4973bf"
            }
          ]
        }
      ]
    }
  ]
}