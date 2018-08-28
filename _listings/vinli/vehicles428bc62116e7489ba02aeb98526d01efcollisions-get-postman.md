{
  "info": {
    "name": "Vinli Get a List of Collisions for a Vehicle",
    "_postman_id": "cd16512f-e0fb-4df5-a5e7-d811811bf300",
    "description": "Get a list of collisions for a vehicle.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "List",
      "item": [
        {
          "id": "0a206c0b-c77e-4bd3-b70f-9f4eff34aaae",
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
              "id": "6021d976-b2bd-45e6-a59e-90413528cbd0"
            }
          ]
        },
        {
          "id": "f68d4b67-2968-4ca2-9c50-3f1eed8f0e07",
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
              "id": "547d8e0d-41fd-4d70-ac01-9459c8bf8dd9"
            }
          ]
        },
        {
          "id": "437b92a7-2b35-4bc9-9fe3-5a8a4c270ca3",
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
              "id": "7c817a18-c4f4-4557-9484-8223d89b3cb0"
            }
          ]
        },
        {
          "id": "7bd050ae-28a4-43f6-b96e-9d7c81da1af1",
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
              "id": "ebf38588-498e-4e36-a7e1-3550ed153e4b"
            }
          ]
        },
        {
          "id": "6792fdaa-da60-48a1-a885-bd77e1864556",
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
              "id": "b0f850e8-dd43-42d0-8bbe-685c503038b1"
            }
          ]
        },
        {
          "id": "831eaacb-9698-4171-bf4e-6f332142e9de",
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
              "id": "52899764-6d7e-4611-a890-a53d48a26830"
            }
          ]
        }
      ]
    },
    {
      "name": "Vehicle",
      "item": [
        {
          "id": "fc258036-6103-4b4c-884c-80e8e05c49f7",
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
              "id": "e0e2e4bb-fe2e-4b3f-8d6a-5d2660669dd6"
            }
          ]
        }
      ]
    },
    {
      "name": "Devices",
      "item": [
        {
          "id": "02316164-21a8-4322-b83d-73727f8e07c8",
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
              "id": "35647d04-d6c0-43f2-9ca9-36c92a6aaf27"
            }
          ]
        }
      ]
    },
    {
      "name": "Report",
      "item": [
        {
          "id": "92af89ca-958e-414f-8009-7683c0ca3089",
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
              "id": "21fa6782-066d-489f-a3fb-0bcf3a29d191"
            }
          ]
        }
      ]
    }
  ]
}