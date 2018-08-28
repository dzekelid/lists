{
  "info": {
    "name": "Vinli List a Device's Vehicles",
    "_postman_id": "81085a81-1fde-45ee-bcba-ab207aa3c91e",
    "description": "List a device's vehicles.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "List",
      "item": [
        {
          "id": "79bfb6c6-2b5d-4ea5-a364-299e80cdbb41",
          "name": "DevicesCf217c2dDf3c41f7B6108bc3e11b4b79VehiclesGet",
          "request": {
            "url": "http://events.vin.li/api/v1/devices/cf217c2d-df3c-41f7-b610-8bc3e11b4b79/vehicles",
            "method": "GET",
            "header": [
              {
                "key": "Accept",
                "value": "{}",
                "description": "",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "List a device's vehicles."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "89af93b7-6526-4ed3-988d-b052f99bc819"
            }
          ]
        }
      ]
    }
  ]
}