swagger: "2.0"
x-collection-name: BigCommerce
x-complete: 1
info:
  title: BigCommerce API V3
  description: collection-of-requests-for-interacting-with-bigcommerces-v3-api
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