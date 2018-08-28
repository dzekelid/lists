---
swagger: "2.0"
x-collection-name: Predix
x-complete: 0
info:
  title: Predix Fingerprint of Things Object Tagging Service List Groups
  description: List groups
  contact:
    name: NEC
  version: 1.0.0
host: fingerprint-of-things-ga1-dast.run.aws-usw02-pr.ice.predix.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/resource:
    get:
      summary: Retrieves the list of all resources for the given zone.
      description: Retrieves the list of all resources for the given zone..
      operationId: getResourcesUsingGET
      x-api-path-slug: v1resource-get
      responses:
        200:
          description: Successful response
      tags:
      - Retrieves
      - List
      - Of
      - ""
      - Resourcesthe
      - Given
      - Zone
    post:
      summary: Creates a list of resources for the given zone. Existing resources
        will be updated with the provided values.
      description: Creates a list of resources for the given zone. existing resources
        will be updated with the provided values..
      operationId: appendResourcesUsingPOST
      x-api-path-slug: v1resource-post
      parameters:
      - in: body
        name: resources
        description: resources
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - Creates
      - List
      - Of
      - Resourcesthe
      - Given
      - Zone
      - ""
      - Existing
      - Resources
      - Will
      - Be
      - Updated
      - Provided
      - Values
  /v1/subject:
    get:
      summary: Retrieves the list of subjects for the given zone.
      description: Retrieves the list of subjects for the given zone..
      operationId: getSubjectsUsingGET_1
      x-api-path-slug: v1subject-get
      responses:
        200:
          description: Successful response
      tags:
      - Retrieves
      - List
      - Of
      - Subjectsthe
      - Given
      - Zone
    post:
      summary: Creates a list of subjects. Existing subjects will be updated with
        the provided values.
      description: Creates a list of subjects. existing subjects will be updated with
        the provided values..
      operationId: appendsubjectsUsingPOST_1
      x-api-path-slug: v1subject-post
      parameters:
      - in: body
        name: subjects
        description: subjects
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: Successful response
      tags:
      - Creates
      - List
      - Of
      - Subjects
      - ""
      - Existing
      - Subjects
      - Will
      - Be
      - Updated
      - Provided
      - Values
  /v1/collections:
    get:
      summary: List all asset collections for a customer
      description: |-
        Returns an array containing the names of all asset collections for the
        specified customer.
      operationId: returns-an-array-containing-the-names-of-all-asset-collections-for-thespecified-customer
      x-api-path-slug: v1collections-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: Successful response
      tags:
      - List
      - ""
      - Asset
      - Collectionsa
      - Customer
  /v1/object/listObjects:
    post:
      summary: List Registered Objects
      description: List registered Objects.
      operationId: reference
      x-api-path-slug: v1objectlistobjects-post
      parameters:
      - in: header
        name: 'Authorization: Bearer'
        description: OAuth2 token
      - in: body
        name: body
        description: Request body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Predix-Zone-Id
        description: Zone ID
      responses:
        200:
          description: OK
      tags:
      - List
      - Registered
      - Objects
  /v1/group/listGroups:
    post:
      summary: List Groups
      description: List groups
      operationId: groupReference
      x-api-path-slug: v1grouplistgroups-post
      parameters:
      - in: header
        name: 'Authorization: Bearer'
        description: OAuth2 token
      - in: body
        name: body
        description: Request body
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Predix-Zone-Id
        description: Zone ID
      responses:
        200:
          description: OK
      tags:
      - List
      - Groups
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