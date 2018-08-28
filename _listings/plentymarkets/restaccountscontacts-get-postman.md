{
  "info": {
    "name": "Plentymarkets List contacts",
    "_postman_id": "abf701e5-eaca-4905-a071-f5f8337d7402",
    "description": "List contacts.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "List",
      "item": [
        {
          "id": "61e3f7e3-6777-4eae-87d3-7f8e71700c75",
          "name": "getRestAccountsContacts",
          "request": {
            "url": "http://example.com/rest/accounts/contacts?billingAddressId=%7B%7D&contactAddress=%7B%7D&contactEmail=%7B%7D&contactId=%7B%7D&countryId=%7B%7D&createdAtAfter=%7B%7D&createdAtBefore=%7B%7D&deliveryAddressId=%7B%7D&email=%7B%7D&externalId=%7B%7D&fullText=%7B%7D&itemsPerPage=%7B%7D&name=%7B%7D&newsletterAllowance=%7B%7D&newsletterAllowanceAfter=%7B%7D&newsletterAllowanceBefore=%7B%7D&number=%7B%7D&page=%7B%7D&plentyId=%7B%7D&postalCode=%7B%7D&privatePhone=%7B%7D&referrerId=%7B%7D&town=%7B%7D&typeId=%7B%7D&updatedAtAfter=%7B%7D&updatedAtBefore=%7B%7D&userId=%7B%7D&with=%7B%7D",
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
            "description": "List contacts."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0e7e0844-1c6d-401f-a4f6-bce15cc7669a"
            }
          ]
        }
      ]
    }
  ]
}