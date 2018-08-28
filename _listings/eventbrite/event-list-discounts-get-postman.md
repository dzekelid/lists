{
  "info": {
    "name": "Eventbrite Get Event List Discounts",
    "_postman_id": "9a59b779-2194-400a-99ab-680ec074a08d",
    "description": "This method returns a list of discounts for a given event.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Checkout",
      "item": [
        {
          "id": "86c7ed3d-a01c-41c3-a9d9-00aaf083be9d",
          "name": "getCheckoutSettingsCountriesCurrencies",
          "request": {
            "url": "http://www.eventbrite.com/%7Bdata-type%7D/checkout_settings/countries_currencies/",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Get the countries and currencies which are supported by Eventbrite for ticket payment"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "165780d4-c24c-492d-995d-3ca5e7568c98"
            }
          ]
        }
      ]
    },
    {
      "name": "Discounts",
      "item": [
        {
          "id": "9d986137-505f-47f9-a90e-c47500e9165c",
          "name": "getDiscountsDiscount",
          "request": {
            "url": "http://www.eventbrite.com/%7Bdata-type%7D/discounts/:discount_id/",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns the cross_event_discount with the specified :discount_id."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3c1d1268-cd97-4008-832e-ecbd89a939ef"
            }
          ]
        },
        {
          "id": "995493f4-1e90-4865-aefd-0c0a9156c0c6",
          "name": "postDiscountsDiscount",
          "request": {
            "url": "http://www.eventbrite.com/%7Bdata-type%7D/discounts/:discount_id/?discount.amount_off=%7B%7D&discount.code=%7B%7D&discount.end_date=%7B%7D&discount.end_date_relative=%7B%7D&discount.hold_ids=%7B%7D&discount.percent_off=%7B%7D&discount.quantity_available=%7B%7D&discount.start_date=%7B%7D&discount.start_date_relative=%7B%7D&discount.ticket_class_ids=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Updates the discount with the specified :discount_id. Returns the updated cross_event_discount. The fields sent are the ones that are going to be updated, the fields that are not sent will be unchanged. The same conditions and notes for the discount creation apply."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "25432d55-2b38-4eed-b983-0ab79c3346c3"
            }
          ]
        },
        {
          "id": "7c2c5a4d-65a2-4727-a2e1-8d85581c514e",
          "name": "deleteDiscountsDiscount",
          "request": {
            "url": "http://www.eventbrite.com/%7Bdata-type%7D/discounts/:discount_id/",
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes the cross_event_discount with the specified :discount_id.\nOnly unused discounts can be deleted."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c4a6743e-1c49-465c-b119-7dbc7cd4fd95"
            }
          ]
        },
        {
          "id": "40d2a441-e54f-4e10-8664-7427a94297fe",
          "name": "postDiscounts",
          "request": {
            "url": "http://www.eventbrite.com/%7Bdata-type%7D/discounts/?discount.amount_off=%7B%7D&discount.code=%7B%7D&discount.end_date=%7B%7D&discount.end_date_relative=%7B%7D&discount.event_id=%7B%7D&discount.hold_ids=%7B%7D&discount.percent_off=%7B%7D&discount.quantity_available=%7B%7D&discount.start_date=%7B%7D&discount.start_date_relative=%7B%7D&discount.ticket_class_ids=%7B%7D&discount.ticket_group_id=%7B%7D&discount.type=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Creates a discount. Returns the created cross_event_discount."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1047ffbc-e1d0-4fcb-b112-7935972ca2c9"
            }
          ]
        }
      ]
    },
    {
      "name": "Events",
      "item": [
        {
          "id": "a8518bda-64ff-4774-9c8c-6fe5852ccec4",
          "name": "getEventsDiscounts",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.eventbrite.com",
              "path": [
                "%7Bdata-type%7D",
                "events/:id/discounts/"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Please use https://www.eventbrite.com/developer/v3/endpoints/users/#ebapi-get-users-user-id-discounts"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ceb1009b-a006-4c2e-acab-5614ee4016af"
            }
          ]
        },
        {
          "id": "950973b1-3637-4f5e-87b9-58f83f9382de",
          "name": "postEventsDiscounts",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.eventbrite.com",
              "path": [
                "%7Bdata-type%7D",
                "events/:id/discounts/"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Please use https://www.eventbrite.com/developer/v3/endpoints/cross_event_discounts/#ebapi-post-discounts"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "80df6e52-2b82-41d7-81ec-521308462e6f"
            }
          ]
        },
        {
          "id": "075fbba1-d36c-40b5-be1b-c93c5d24acb9",
          "name": "getEventsDiscountsDiscount",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.eventbrite.com",
              "path": [
                "%7Bdata-type%7D",
                "events/:id/discounts/:discount_id/"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Please use https://www.eventbrite.com/developer/v3/endpoints/cross_event_discounts/#ebapi-get-discounts-discount-id"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f0721eb6-b623-4d39-8f5e-77bd3ed3e7d6"
            }
          ]
        },
        {
          "id": "4b1cd55f-b0c9-40f2-b5b6-a4510ce33e6a",
          "name": "postEventsDiscountsDiscount",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.eventbrite.com",
              "path": [
                "%7Bdata-type%7D",
                "events/:id/discounts/:discount_id/"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Please use https://www.eventbrite.com/developer/v3/endpoints/cross_event_discounts/#ebapi-post-discounts-discount-id"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a9d1b67f-348f-4d9d-9cfa-07de9ec55cf2"
            }
          ]
        },
        {
          "id": "fdfc573c-5bb1-404f-b9a3-8f72adabab8b",
          "name": "deleteEventsDiscountsDiscount",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.eventbrite.com",
              "path": [
                "%7Bdata-type%7D",
                "events/:id/discounts/:discount_id/"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Please use https://www.eventbrite.com/developer/v3/endpoints/cross_event_discounts/#ebapi-delete-discounts-discount-id"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fc1387cd-80dd-48a5-b36b-02815cab975f"
            }
          ]
        },
        {
          "id": "608a9069-31fd-482e-9c84-52bee49a7af9",
          "name": "getEventsPublicDiscounts",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.eventbrite.com",
              "path": [
                "%7Bdata-type%7D",
                "events/:id/public_discounts/"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Please use https://www.eventbrite.com/developer/v3/endpoints/users/#ebapi-get-users-user-id-discounts"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6c616da6-70d8-4d97-97f0-7701385a89d2"
            }
          ]
        },
        {
          "id": "c180fc88-23d3-4100-a5e1-e4f43aa52d86",
          "name": "postEventsPublicDiscounts",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.eventbrite.com",
              "path": [
                "%7Bdata-type%7D",
                "events/:id/public_discounts/"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Please use https://www.eventbrite.com/developer/v3/endpoints/cross_event_discounts/#ebapi-post-discounts"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ea959f32-ad37-4797-ba8f-dd5d02710e1c"
            }
          ]
        },
        {
          "id": "5f98f6cd-b587-4e72-968b-9e50477a8870",
          "name": "getEventsPublicDiscountsDiscount",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.eventbrite.com",
              "path": [
                "%7Bdata-type%7D",
                "events/:id/public_discounts/:discount_id/"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Please use https://www.eventbrite.com/developer/v3/endpoints/cross_event_discounts/#ebapi-get-discounts-discount-id"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b47cb4c3-a4df-4e4c-998c-bf99d52f36c8"
            }
          ]
        },
        {
          "id": "3115fa8b-8716-419a-9a94-9a28392c2e45",
          "name": "postEventsPublicDiscountsDiscount",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.eventbrite.com",
              "path": [
                "%7Bdata-type%7D",
                "events/:id/public_discounts/:discount_id/"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Please use https://www.eventbrite.com/developer/v3/endpoints/cross_event_discounts/#ebapi-post-discounts-discount-id"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "805ea2dc-929f-449a-9461-bc922a7717fa"
            }
          ]
        },
        {
          "id": "325f2831-95fa-4682-95a7-3098ee9fdc7c",
          "name": "deleteEventsPublicDiscountsDiscount",
          "request": {
            "url": {
              "protocol": "http",
              "host": "www.eventbrite.com",
              "path": [
                "%7Bdata-type%7D",
                "events/:id/public_discounts/:discount_id/"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "id",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Please use https://www.eventbrite.com/developer/v3/endpoints/cross_event_discounts/#ebapi-delete-discounts-discount-id"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c6d246ec-2adc-4f1f-a93d-baa669891f34"
            }
          ]
        }
      ]
    },
    {
      "name": "System",
      "item": [
        {
          "id": "79566e46-35d2-405b-8a0e-4da1edd16cb6",
          "name": "getSystemCountries",
          "request": {
            "url": "http://www.eventbrite.com/%7Bdata-type%7D/system/countries/",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a single page response with a key of countries,\ncontaining a list of countries."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9b434d05-52e0-4c2a-8299-25600a85ef60"
            }
          ]
        }
      ]
    },
    {
      "name": "Users",
      "item": [
        {
          "id": "e06b977b-1af4-4885-bdc7-9506f690a9c7",
          "name": "getUsersUserDiscounts",
          "request": {
            "url": "http://www.eventbrite.com/%7Bdata-type%7D/users/:user_id/discounts/?code=%7B%7D&code_filter=%7B%7D&event_id=%7B%7D&order_by=%7B%7D&page_size=%7B%7D&scope=%7B%7D&ticket_group_id=%7B%7D&type=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a paginated response of cross_event_discount for the specified user.\nThis operation is only supported for the currently authenticated user. The alias me (/users/me/) may be used."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1a0a6ba4-0b0f-4481-98bc-92440e1d2b71"
            }
          ]
        }
      ]
    },
    {
      "name": "Event",
      "item": [
        {
          "id": "2c11ba69-9c15-4206-9712-c61e506899c7",
          "name": "Get_event_list_discounts_",
          "request": {
            "url": "http://www.eventbrite.com/%7Bdata-type%7D/event_list_discounts?data-type=%7B%7D&id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "This method returns a list of discounts for a given event."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "565ce59c-d490-4746-bf5e-dbbd4ea3d655"
            }
          ]
        }
      ]
    }
  ]
}