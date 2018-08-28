{
  "info": {
    "name": "Plentymarkets List contact classes",
    "_postman_id": "71d923b3-f332-4dc9-8628-4ce036980f82",
    "description": "List contact classes.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "List",
      "item": [
        {
          "id": "12d25687-f9c1-4b6d-bbfc-3e0f834bac4e",
          "name": "getRestAccountsContactsClasses",
          "request": {
            "url": "http://example.com/rest/accounts/contacts/classes",
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
            "description": "List contact classes."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "43e8f460-a584-4b43-847f-741d3d2406af"
            }
          ]
        }
      ]
    }
  ]
}