{
  "info": {
    "name": "Plentymarkets List categories",
    "_postman_id": "49dc55d4-2ce0-4486-a53c-5aa2b0d35379",
    "description": "List categories.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "List",
      "item": [
        {
          "id": "a58da54b-8809-4682-9374-a6c2e8199457",
          "name": "getRestCategories",
          "request": {
            "url": "http://example.com/rest/categories?categoryId=%7B%7D&itemsPerPage=%7B%7D&lang=%7B%7D&level=%7B%7D&linklist=%7B%7D&name=%7B%7D&page=%7B%7D&parentId=%7B%7D&plentyId=%7B%7D&type=%7B%7D&updatedAt=%7B%7D&with=%7B%7D",
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
            "description": "List categories."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "62a7e04b-ddeb-4ad7-b24f-143e668cfe7a"
            }
          ]
        }
      ]
    }
  ]
}