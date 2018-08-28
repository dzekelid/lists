{
  "info": {
    "name": "Vinli Get list of  a Vehicles Distances",
    "_postman_id": "835ec68e-20a0-40bb-a958-130b3245b5a3",
    "description": "Get list of  a vehicles distances.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "List",
      "item": [
        {
          "id": "f2106760-b8f1-4c42-80b4-25349195d69e",
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
              "id": "24ddacd9-10f0-40a5-a14b-03f47ef2c9fb"
            }
          ]
        },
        {
          "id": "adcea88f-0322-483e-ab81-acf9520e20ee",
          "name": "Vehicles9aa35c64B04643cc9cd84c353a6d0b30TripsGet",
          "request": {
            "url": "http://events.vin.li/api/v1/vehicles/9aa35c64-b046-43cc-9cd8-4c353a6d0b30/trips",
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
            "description": "List all of a vehicle's trips."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a56ef8cc-5241-455d-9362-5c33947cfc83"
            }
          ]
        },
        {
          "id": "5d899ce5-3484-4a79-9776-c9c8925c4362",
          "name": "Vehicles9aa35c64B04643cc9cd84c353a6d0b30DistancesGet",
          "request": {
            "url": "http://events.vin.li/api/v1/vehicles/9aa35c64-b046-43cc-9cd8-4c353a6d0b30/distances",
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
            "description": "Get list of  a vehicles distances."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "35ce019a-15ad-4fc1-925a-f01a2a7c44b9"
            }
          ]
        }
      ]
    }
  ]
}