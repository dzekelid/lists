swagger: "2.0"
x-collection-name: moltin
x-complete: 1
info:
  title: Moltin
  description: -welcomethis-is-a-place-to-put-general-notes-and-extra-information-for-internal-use-to-get-started-designingdocumenting-this-api-select-a-version-on-the-left-
  version: 1.0.0
host: api.moltin.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v2/collections:
    get:
      summary: Get Collections List
      description: Get collections list.
      operationId: V2CollectionsGet
      x-api-path-slug: v2collections-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Collections
      - List
  /v2/fields:
    get:
      summary: Get a field list
      description: Get a field list.
      operationId: V2FieldsGet
      x-api-path-slug: v2fields-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Field
      - List
  /v2/customers:
    get:
      summary: Get Customers List
      description: Get customers list.
      operationId: V2CustomersGet
      x-api-path-slug: v2customers-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: query
        name: filter
      - in: query
        name: page[limit]
      - in: query
        name: page[offset]
      - in: query
        name: sort
      responses:
        200:
          description: Successful response
      tags:
      - Customers
      - List
  /v2/variations:
    get:
      summary: Get Product Variations List
      description: Get product variations list.
      operationId: V2VariationsGet
      x-api-path-slug: v2variations-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Products
      - Variations
      - List
  /v2/currencies:
    get:
      summary: Get Currencies List
      description: Get currencies list.
      operationId: V2CurrenciesGet
      x-api-path-slug: v2currencies-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Currencies
      - List
  /v2/integrations:
    get:
      summary: Get Integrations list
      description: Get integrations list.
      operationId: V2IntegrationsGet
      x-api-path-slug: v2integrations-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Integrations
      - List
  /v2/categories:
    get:
      summary: Get Categories List
      description: Get categories list.
      operationId: V2CategoriesGet
      x-api-path-slug: v2categories-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      responses:
        200:
          description: Successful response
      tags:
      - Categories
      - List
  /v2/products:
    get:
      summary: Get Products List
      description: Get products list.
      operationId: V2ProductsGet
      x-api-path-slug: v2products-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: query
        name: filter
      - in: query
        name: include
      - in: query
        name: page[limit]
      - in: query
        name: page[offset]
      - in: query
        name: sort
      responses:
        200:
          description: Successful response
      tags:
      - Productss
      - List