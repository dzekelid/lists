{
  "info": {
    "name": "Vinli List all Odometer Triggers for a Vehicle",
    "_postman_id": "884a076e-3bfe-48ab-a8f0-761133e2e677",
    "description": "List all odometer triggers for a vehicle.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "List",
      "item": [
        {
          "id": "3492c2c1-b969-4748-b738-9e3884b5b511",
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
              "id": "576de958-8a15-4993-8cc0-77557e7dcb3e"
            }
          ]
        },
        {
          "id": "2735dd28-fe9a-4827-aa76-ddacf9562d21",
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
              "id": "02753b26-fe5a-48ee-92e7-e25f344096d5"
            }
          ]
        },
        {
          "id": "a755537d-32f2-41dc-bbbf-ee564577a1d4",
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
              "id": "a4f5f309-b98b-4c72-bae3-d40cb1c3a5dd"
            }
          ]
        },
        {
          "id": "bfd8393f-8368-418b-9dd0-0fc6214a82d0",
          "name": "Vehicles9aa35c64B04643cc9cd84c353a6d0b30OdometerTriggersGet",
          "request": {
            "url": "http://events.vin.li/api/v1/vehicles/9aa35c64-b046-43cc-9cd8-4c353a6d0b30/odometer_triggers",
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
            "description": "List all odometer triggers for a vehicle."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bd9271d5-c091-4108-8339-9d91b826e322"
            }
          ]
        },
        {
          "id": "2b6ec0a2-32bd-4c0b-92a2-2a53905fe449",
          "name": "Vehicles428bc62116e7489bA02aEb98526d01efCollisionsGet",
          "request": {
            "url": "http://events.vin.li/api/v1/vehicles/428bc621-16e7-489b-a02a-eb98526d01ef/collisions",
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
            "description": "Get a list of collisions for a vehicle."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f797c7d3-e6dd-4632-90d0-a33e53836776"
            }
          ]
        },
        {
          "id": "eb086084-3d9b-4c18-b0de-1711fdb92213",
          "name": "Vehicles9aa35c64B04643cc9cd84c353a6d0b30OdometersGet",
          "request": {
            "url": "http://events.vin.li/api/v1/vehicles/9aa35c64-b046-43cc-9cd8-4c353a6d0b30/odometers",
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
            "description": "List all odometer reports for a vehicle."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "03eaf667-03d3-43bc-9639-c5c30b8f771c"
            }
          ]
        }
      ]
    },
    {
      "name": "Vehicle",
      "item": [
        {
          "id": "ffe0028d-2e5c-4b30-98c6-d5e200ff6506",
          "name": "VehiclesAa44769b3c0a46629bad25481cf5198fGet",
          "request": {
            "url": "http://events.vin.li/api/v1/vehicles/aa44769b-3c0a-4662-9bad-25481cf5198f",
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
            "description": "Get vehicle details."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6ab14854-c4b5-4d4c-9a5f-43a359c504c6"
            }
          ]
        }
      ]
    },
    {
      "name": "Devices",
      "item": [
        {
          "id": "60a03e11-3c6d-440a-bd2c-36ec973e075b",
          "name": "Devices821374c0D6d811e39c1a0800200c9a66VehiclesLatestGet",
          "request": {
            "url": "http://events.vin.li/api/v1/devices/821374c0-d6d8-11e3-9c1a-0800200c9a66/vehicles/_latest",
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
            "description": "Get device's latest vehicle."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1bd9ef85-a9d8-4379-bce2-cae2da689854"
            }
          ]
        }
      ]
    },
    {
      "name": "Report",
      "item": [
        {
          "id": "a4caed04-c853-40f9-b609-1cb00b1b8200",
          "name": "Vehicles8480c5b76f3e40b3A78e3555617d44b0ReportCardsGet",
          "request": {
            "url": "http://events.vin.li/api/v1/vehicles/8480c5b7-6f3e-40b3-a78e-3555617d44b0/report_cards",
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
            "description": "Report cards for a vehicle."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "417ba26a-6b06-411d-b0f1-654b7a7f104a"
            }
          ]
        }
      ]
    }
  ]
}