{
  "info": {
    "name": "Vinli List All Odometer Reports for a Vehicle",
    "_postman_id": "ae88d97f-31df-4bd5-b15d-92c31c5321a9",
    "description": "List all odometer reports for a vehicle.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "List",
      "item": [
        {
          "id": "61719d50-7bc3-4892-8115-1a875cdb6b27",
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
              "id": "109edbc9-d4d9-48cb-aca5-be04784f6018"
            }
          ]
        },
        {
          "id": "d25a699f-561d-4a58-90ef-9f2be48e5139",
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
              "id": "3e1b4748-1133-458b-b7c2-762cc449f513"
            }
          ]
        },
        {
          "id": "750b54ee-e68b-4d11-98e3-89672c762ccd",
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
              "id": "479f6712-96d7-49f4-9855-0a9d9c011d7f"
            }
          ]
        },
        {
          "id": "966b2857-6149-456e-8590-e63b6aaea380",
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
              "id": "58f88e49-f6eb-4a9c-97f4-f06be46664d5"
            }
          ]
        },
        {
          "id": "4a10b8c0-7f2f-4393-a837-1a79b5afd2ee",
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
              "id": "4059892b-de71-4be7-a4ea-7a115f556e09"
            }
          ]
        },
        {
          "id": "cc320ae2-4a74-4347-a3d8-837bd56722af",
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
              "id": "d2f98307-981e-4386-bc02-cd5f93f323bb"
            }
          ]
        }
      ]
    },
    {
      "name": "Vehicle",
      "item": [
        {
          "id": "8d3a4920-9e5c-41f0-ab60-384f78c84c52",
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
              "id": "ac31716c-f852-4dc4-ac4c-c5d83725835b"
            }
          ]
        }
      ]
    },
    {
      "name": "Devices",
      "item": [
        {
          "id": "b0591081-f6fa-4166-a3c9-1c6dc0152111",
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
              "id": "fd0e9153-c32c-4852-b58b-70fb51fa9d17"
            }
          ]
        }
      ]
    },
    {
      "name": "Report",
      "item": [
        {
          "id": "6136b432-0e78-4e8f-96be-1b83a2d598a2",
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
              "id": "28624c6b-d66a-4f8e-bc5e-2d0c96ef7393"
            }
          ]
        }
      ]
    }
  ]
}