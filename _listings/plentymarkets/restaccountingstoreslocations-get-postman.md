{
  "info": {
    "name": "Plentymarkets List all accounting locations",
    "_postman_id": "c7284c46-dcb1-49c2-a738-0b1191192fb0",
    "description": "List all accounting locations.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "List",
      "item": [
        {
          "id": "c2ee34c6-1e27-4de6-a5f3-911dbc588b7d",
          "name": "getRestAccountingStoresLocations",
          "request": {
            "url": "http://example.com/rest/accounting/stores/locations",
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
            "description": "List all accounting locations."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c2c1a35a-61c8-4711-8bac-edcd585f04ff"
            }
          ]
        }
      ]
    }
  ]
}