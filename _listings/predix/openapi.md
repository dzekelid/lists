swagger: "2.0"
x-collection-name: Predix
x-complete: 1
info:
  title: VIEWS
  version: 1.0.0
host: thetaray-anomaly-service.run.aws-usw02-pr.ice.predix.io
basePath: /v1
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
      summary: List all data collections for a customer
      description: |-
        Returns an array containing the names of all data collections for the
        specified customer.
      operationId: returns-an-array-containing-the-names-of-all-data-collections-for-thespecified-customer
      x-api-path-slug: v1collections-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - List
      - ""
      - Data
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
  /flow-templates/{flowTemplateId}/list:
    get:
      summary: Get Flow Templates Flowtemplateid List
      description: Get flow templates flowtemplateid list.
      operationId: listFlowTemplateAnalyticFileUsingGET
      x-api-path-slug: flowtemplatesflowtemplateidlist-get
      parameters:
      - in: path
        name: flowTemplateId
        description: flowTemplateId
      responses:
        200:
          description: Successful response
      tags:
      - Flow
      - Templates
      - Flowtemplateid
      - List
  /v1/maps:
    get:
      summary: List all maps for a customer
      description: |-
        Returns an array of maps for the specified customer. The array contains
        the name and identifier for each map.
      operationId: returns-an-array-of-maps-for-the-specified-customer-the-array-containsthe-name-and-identifier-for-ea
      x-api-path-slug: v1maps-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - List
      - ""
      - Mapsa
      - Customer
  /v1/tenant/{tenantName}:
    get:
      summary: Retrieve a tenant and its list of services
      description: Retrieve a tenant and its list of services.
      operationId: getTenantUsingGET
      x-api-path-slug: v1tenanttenantname-get
      parameters:
      - in: header
        name: Predix-Zone-Id
      - in: path
        name: tenantName
        description: tenantName
      responses:
        200:
          description: Successful response
      tags:
      - Retrieve
      - Tenant
      - Its
      - List
      - Of
      - Services