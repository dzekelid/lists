---
swagger: "2.0"
x-collection-name: BigCommerce
x-complete: 0
info:
  title: BigCommerce Retrieve a list of variants
  description: Returns a `Variant` object list from the BigCommerce Catalog.
  version: 1.0.0
host: api.bigcommerce.com
basePath: /stores
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{store_hash}/v3/catalog/products/{id}/variants:
    get:
      summary: Retrieve a list of variants
      description: Returns a `Variant` object list from the BigCommerce Catalog.
      operationId: V3CatalogProductsVariantsByStoreHashAndIdGet
      x-api-path-slug: store-hashv3catalogproductsidvariants-get
      parameters:
      - in: path
        name: id
      - in: path
        name: store_hash
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Retrieve
      - List
      - Of
      - Variants
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---