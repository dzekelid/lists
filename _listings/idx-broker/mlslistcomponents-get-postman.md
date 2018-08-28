{
  "info": {
    "name": "IDX Broker Get Mls List Components",
    "_postman_id": "0ff3edee-8711-4665-af25-a3bb57637ad8",
    "description": "This is a simple, access anywhere, method for getting a list of all API components available.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Mls",
      "item": [
        {
          "id": "bda09908-4887-4610-8919-431f4c3097a8",
          "name": "MlsListcomponentsGet",
          "request": {
            "url": "http://example.com/mls/listcomponents",
            "method": "GET",
            "header": [
              {
                "key": "accesskey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "ancillarykey",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "apiversion",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "outputtype",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "This is a simple, access anywhere, method for getting a list of all API components available."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "23c11553-de31-4526-a419-55cc632c13fb"
            }
          ]
        }
      ]
    }
  ]
}