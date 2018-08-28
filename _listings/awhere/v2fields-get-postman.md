{
  "info": {
    "name": "aWhere Get Fields List",
    "_postman_id": "75228dc5-3ffb-4a27-a4f8-06a1d6b6618b",
    "description": "####Request\nThis API call retrieves the list of fields in your account. \n\n[Get Fields Documentation](http://developer.awhere.com/api/reference/fields/get-fields)\n\n\n####Security\nThis API call uses the security Access Token that is retrieved with the \"Get a Token\" request. If you run that request first, it will save a token to Postman and this API will use it automatically. You can also see where the token should normally go by clicking the \"Headers\" tab below. The Authorization header holds the token, replacing the \"{{aWhereAccessToken}}\" part.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Agriculture",
      "item": [
        {
          "id": "9d9246f0-7193-4541-b5ff-9e4fab29b0a1",
          "name": "V2AgronomicsFieldsField1Agronomicvalues2015080120150803Get",
          "request": {
            "url": "http://api.awhere.com/v2/agronomics/fields/field1/agronomicvalues/2015-08-01,2015-08-03",
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
            "description": "####Request\nThis API call gets calculated agronomics and accumulations at a field location. \n\nThe URL used here will get the values for a certain range of days. This is a very flexible API and so you're encouraged to review the [Agronomics Documentation](http://developer.awhere.com/api/reference/agronomics/values).\n\n_Tip: Remember to use a field ID that exists in your account. By default, this collection uses a default field ID of 'field1'_\n\n\n####Security\nThis API call uses the security Access Token that is retrieved with the \"Get a Token\" request. If you run that request first, it will save a token to Postman and this API will use it automatically. You can also see where the token should normally go by clicking the \"Headers\" tab below. The Authorization header holds the token, replacing the \"{{aWhereAccessToken}}\" part."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fbb67cf6-2782-4511-aded-e09c3a0e8484"
            }
          ]
        },
        {
          "id": "c4dc680f-0e8d-416f-a2cf-2d63eaaebc1b",
          "name": "V2AgronomicsFieldsField1Agronomicnorms08010803Years20102014Get",
          "request": {
            "url": "http://api.awhere.com/v2/agronomics/fields/field1/agronomicnorms/08-01,08-03/years/2010,2014",
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
            "description": "####Request\nThis API call gets the long term averages for agronomic values and accumulations at a field location. \n\nThe URL used here will get the values for a certain range of days over a certain range of years. This is a very flexible API and so you're encouraged to review the [Agronomics Documentation](http://developer.awhere.com/api/reference/agronomics/norms).\n\n_Tip: Remember to use a field ID that exists in your account. By default, this collection uses a default field ID of 'field1'_\n\n\n####Security\nThis API call uses the security Access Token that is retrieved with the \"Get a Token\" request. If you run that request first, it will save a token to Postman and this API will use it automatically. You can also see where the token should normally go by clicking the \"Headers\" tab below. The Authorization header holds the token, replacing the \"{{aWhereAccessToken}}\" part."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ca8868c3-1ef2-41a3-ae05-fbc4dcdd38d8"
            }
          ]
        },
        {
          "id": "30ce3623-af96-4635-bc56-e161d5b55cc2",
          "name": "V2FieldsGet",
          "request": {
            "url": "http://api.awhere.com/v2/fields",
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
            "description": "####Request\nThis API call retrieves the list of fields in your account. \n\n[Get Fields Documentation](http://developer.awhere.com/api/reference/fields/get-fields)\n\n\n####Security\nThis API call uses the security Access Token that is retrieved with the \"Get a Token\" request. If you run that request first, it will save a token to Postman and this API will use it automatically. You can also see where the token should normally go by clicking the \"Headers\" tab below. The Authorization header holds the token, replacing the \"{{aWhereAccessToken}}\" part."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5813893b-e8aa-450f-8680-1586bbe12873"
            }
          ]
        }
      ]
    }
  ]
}