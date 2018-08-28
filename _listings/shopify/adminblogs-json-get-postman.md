{
  "info": {
    "name": "Shopify Get a list of all blogs",
    "_postman_id": "c5c1f0b7-da2c-493b-94fc-38df8d8cd90c",
    "description": "Get a list of all blogs.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Commerce",
      "item": [
        {
          "id": "c110c900-9c39-4c50-bcab-9d1e4e5ebeb9",
          "name": "getAdminBlogs.json",
          "request": {
            "url": "http://DefaultParameterValue:DefaultParameterValue@DefaultParameterValue.myshopify.com/admin/blogs.json",
            "method": "GET",
            "header": [
              {
                "key": "Content-Type",
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
            "description": "Get a list of all blogs."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8e5fe9d2-cba9-459d-8691-90ca2e19241b"
            }
          ]
        }
      ]
    }
  ]
}