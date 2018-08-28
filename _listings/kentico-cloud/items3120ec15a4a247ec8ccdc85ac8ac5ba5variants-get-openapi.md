---
swagger: "2.0"
x-collection-name: Kentico Cloud
x-complete: 0
info:
  title: Kentico Cloud List language variants
  description: Retrieve a list of language variants of a content item specified by
    its internal ID.
  version: 1.0.0
host: deliver.kenticocloud.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /visitor/569030c7-52a5-44f5-a243-c5285b3eb24e/7888c9a3824a11f1/segments:
    get:
      summary: List segments of a visitor
      description: Retrieve the names of segments that the specified visitor belongs
        to.
      operationId: Visitor569030c752a544f5A243C5285b3eb24e7888c9a3824a11f1SegmentsGet
      x-api-path-slug: visitor569030c752a544f5a243c5285b3eb24e7888c9a3824a11f1segments-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Segments
      - Of
      - Visitor
  /assets:
    get:
      summary: List assets
      description: Retrieve a dynamically paginated list of assets.
      operationId: AssetsGet
      x-api-path-slug: assets-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - List
      - Assets
  /items/codename/on_roasts/variants:
    get:
      summary: List language variants
      description: Retrieve a list of language variants of a content item specified
        by its codename.
      operationId: ItemsCodenameOnRoastsVariantsGet
      x-api-path-slug: itemscodenameon-roastsvariants-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - List
      - Language
      - Variants
  /items/3120ec15-a4a2-47ec-8ccd-c85ac8ac5ba5/variants:
    get:
      summary: List language variants
      description: Retrieve a list of language variants of a content item specified
        by its internal ID.
      operationId: Items3120ec15A4a247ec8ccdC85ac8ac5ba5VariantsGet
      x-api-path-slug: items3120ec15a4a247ec8ccdc85ac8ac5ba5variants-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - List
      - Language
      - Variants
  /segment/569030c7-52a5-44f5-a243-c5285b3eb24e/{SegmentName}/visitors:
    get:
      summary: List visitors of a segment
      description: Retrieve visitors that match the specified segment.
      operationId: Segment569030c752a544f5A243C5285b3eb24eVisitorsBySegmentNameGet
      x-api-path-slug: segment569030c752a544f5a243c5285b3eb24esegmentnamevisitors-get
      parameters:
      - in: path
        name: SegmentName
      responses:
        200:
          description: OK
      tags:
      - List
      - Visitors
      - Of
      - Segment
  /items:
    get:
      summary: List content items
      description: Retrieve a dynamically paginated list of content items.
      operationId: ItemsGet
      x-api-path-slug: items-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - List
      - Content
      - Items
  /975bf280-fd91-488c-994c-2f04416e5ee3/taxonomies:
    get:
      summary: List taxonomy groups
      description: |-
        Retrieve a paginated list of taxonomy groups in your project.

        By default, the API returns all taxonomy groups ordered alphabetically by codename, but [pagination can be customized](https://developer.kenticocloud.com/v1/reference#listing-response).

        See <https://developer.kenticocloud.com/v1/reference#list-taxonomy-groups> for more details.
      operationId: 975bf280Fd91488c994c2f04416e5ee3TaxonomiesGet
      x-api-path-slug: 975bf280fd91488c994c2f04416e5ee3taxonomies-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - List
      - Taxonomy
      - Groups
  /975bf280-fd91-488c-994c-2f04416e5ee3/types:
    get:
      summary: List content types
      description: |-
        Retrieve a list of content types in your project.

        See <https://developer.kenticocloud.com/v1/reference#list-content-types> for more details.
      operationId: 975bf280Fd91488c994c2f04416e5ee3TypesGet
      x-api-path-slug: 975bf280fd91488c994c2f04416e5ee3types-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - List
      - Content
      - Types
  /items/external-id/59713/variants:
    get:
      summary: List language variants
      description: Retrieve a list of language variants of a content item specified
        by its external ID.
      operationId: ItemsExternalId59713VariantsGet
      x-api-path-slug: itemsexternalid59713variants-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - List
      - Language
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