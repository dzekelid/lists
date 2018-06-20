---
name: Square
x-slug: square
description: Square helps millions of sellers run their business- from secure credit
  card processing to point of sale solutions. Get paid faster with Square and sign
  up today!
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/2176-square.jpg
x-kinRank: "9"
x-alexaRank: "2436"
tags: Lists
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/square/apis.md
specificationVersion: "0.14"
apis:
- name: Square Connect API Lists all of a location's item categories.
  x-api-slug: square-connect-api
  description: Lists all of a location's item categories.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/2176-square.jpg
  humanURL: http://squareup.com
  baseURL: https://connect.squareup.com////v1/{location_id}/categories
  tags: Lists,,Of,Locations,Item,Categories
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/square/v1location-idcategories-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/square/v1location-idcategories-get-openapi.md
- name: Square Connect API Lists all of a location's discounts.
  x-api-slug: square-connect-api
  description: Lists all of a location's discounts.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/2176-square.jpg
  humanURL: http://squareup.com
  baseURL: https://connect.squareup.com////v1/{location_id}/discounts
  tags: Lists,,Of,Locations,Discounts
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/square/v1location-iddiscounts-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/square/v1location-iddiscounts-get-openapi.md
- name: Square Connect API Lists all of a location's fees (taxes).
  x-api-slug: square-connect-api
  description: Lists all of a location's fees (taxes).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/2176-square.jpg
  humanURL: http://squareup.com
  baseURL: https://connect.squareup.com////v1/{location_id}/fees
  tags: Lists,,Of,Locations,Fees,(taxes)
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/square/v1location-idfees-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/square/v1location-idfees-get-openapi.md
- name: Square Connect API Provides the details for a single item, including associated
    modifier lists and fees.
  x-api-slug: square-connect-api
  description: Provides the details for a single item, including associated modifier
    lists and fees.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/2176-square.jpg
  humanURL: http://squareup.com
  baseURL: https://connect.squareup.com////v1/{location_id}/items/{item_id}
  tags: Provides,Detailsa,Single,Item,,Including,Associated,Modifier,Lists,Fees
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/square/v1location-iditemsitem-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/square/v1location-iditemsitem-id-get-openapi.md
- name: Square Connect API Lists all of a location's modifier lists.
  x-api-slug: square-connect-api
  description: Lists all of a location's modifier lists.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/2176-square.jpg
  humanURL: http://squareup.com
  baseURL: https://connect.squareup.com////v1/{location_id}/modifier-lists
  tags: Lists,,Of,Locations,Modifier,Lists
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/square/v1location-idmodifierlists-get-openapi.md
- name: Square Connect API Lists all of a location's Favorites pages in Square Register.
  x-api-slug: square-connect-api
  description: Lists all of a location's Favorites pages in Square Register.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/2176-square.jpg
  humanURL: http://squareup.com
  baseURL: https://connect.squareup.com////v1/{location_id}/pages
  tags: Lists,,Of,Locations,Favorites,Pages,In,Square,Register
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/square/v1location-idpages-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/square/v1location-idpages-get-openapi.md
- name: Square Connect API UpdateItemModifierLists
  x-api-slug: square-connect-api
  description: |-
    Updates the [CatalogModifierList](#type-catalogmodifierlist) objects
    that apply to the targeted [CatalogItem](#type-catalogitem) without having
    to perform an upsert on the entire item.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/2176-square.jpg
  humanURL: http://squareup.com
  baseURL: https://connect.squareup.com////v2/catalog/update-item-modifier-lists
  tags: ItemModifierLists
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/square/v2catalogupdateitemmodifierlists-post-openapi.md
- name: Square Connect API
  x-api-slug: square-connect-api
  description: Square helps millions of sellers run their business- from secure credit
    card processing to point of sale solutions. Get paid faster with Square and sign
    up today!
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/2176-square.jpg
  humanURL: http://squareup.com
  baseURL: https://connect.squareup.com//
  tags: Lists
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/square/openapi.md
x-common:
- type: x-base
  url: https://connect.squareup.com
- type: x-crunchbase
  url: http://www.crunchbase.com/company/square
- type: x-crunchbase
  url: https://crunchbase.com/organization/square
- type: x-developer
  url: https://connect.squareup.com/
- type: x-email
  url: press@squareup.com
- type: x-email
  url: security@squareup.com
- type: x-email
  url: lawenforcement@squareup.com
- type: x-email
  url: redemption@squareup.com
- type: x-email
  url: privacy@squareup.com
- type: x-email
  url: community@squareup.com
- type: x-email
  url: noreply@messaging.squareup.com
- type: x-email
  url: ir@squareup.com
- type: x-email
  url: takedowns@squareup.com
- type: x-github
  url: https://github.com/square
- type: x-twitter
  url: https://twitter.com/Square
- type: x-website
  url: http://squareup.com
- type: x-website
  url: https://squareup.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---