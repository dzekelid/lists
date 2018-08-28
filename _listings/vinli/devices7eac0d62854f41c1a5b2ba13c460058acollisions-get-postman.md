{
  "info": {
    "name": "Vinli Get a List of Collisions for a Device",
    "_postman_id": "9396e86c-bb3e-4cf7-ae71-3c50c445a7f2",
    "description": "Get a list of collisions for a device.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Eventsa",
      "item": [
        {
          "id": "aa9a5733-52c6-49fc-84a8-7698c1bf055f",
          "name": "Devices62976d30B6dc40f18422Ccc367572101EventsGet",
          "request": {
            "url": "http://events.vin.li/api/v1/devices/62976d30-b6dc-40f1-8422-ccc367572101/events",
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
            "description": "Get all events for a device."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b90cc197-d5be-48b3-bbb1-487dc257f3ff"
            }
          ]
        }
      ]
    },
    {
      "name": "List",
      "item": [
        {
          "id": "1310715f-f1cf-4ec8-bbaf-a5d017f413f7",
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
              "id": "d87ebd86-4720-442e-925d-7502adbc5f21"
            }
          ]
        },
        {
          "id": "2161313c-d56b-4a12-96a3-8c1ff119972b",
          "name": "Devices7eac0d62854f41c1A5b2Ba13c460058aCollisionsGet",
          "request": {
            "url": "http://events.vin.li/api/v1/devices/7eac0d62-854f-41c1-a5b2-ba13c460058a/collisions",
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
            "description": "Get a list of collisions for a device."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3f632a2d-c74a-4103-af20-29838219415d"
            }
          ]
        }
      ]
    },
    {
      "name": "Specific",
      "item": [
        {
          "id": "66cbb8fd-a98e-4af5-a50b-1394491f2246",
          "name": "RulesB7ad3604C79546af9d5f71be30ed4143Get",
          "request": {
            "url": "http://events.vin.li/api/v1/rules/b7ad3604-c795-46af-9d5f-71be30ed4143",
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
            "description": "Get a specific rule."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1ea4880e-715f-4cf1-8733-40a62d960a84"
            }
          ]
        }
      ]
    }
  ]
}