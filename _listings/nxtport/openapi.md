swagger: "2.0"
x-collection-name: NxtPort
x-complete: 1
info:
  title: Portcall+ API (sandbox)
  description: portplus-api
  version: 1.0.0
host: api-sb.nxtport.eu
basePath: /PortCallPlus/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/containers:
    get:
      summary: List Containers
      description: Get all containers currently in the database. Only Containers accessible
        by the user will be reported.
      operationId: getApiV1Containers
      x-api-path-slug: apiv1containers-get
      parameters:
      - in: query
        name: api_token
        description: authentication token of user making the request
      responses:
        200:
          description: OK
      tags:
      - List
      - Containers
  /api/v1/pickup_rights/:
    get:
      summary: List PickupRights
      description: Get all PickupRights that are assigned / transferred to the users's
        Organization.
      operationId: getApiV1PickupRights
      x-api-path-slug: apiv1pickup-rights-get
      parameters:
      - in: query
        name: api_token
        description: authentication token of user making the request
      responses:
        200:
          description: OK
      tags:
      - List
      - PickupRights
  /api/v1/locations:
    get:
      summary: List
      description: List all Locations with their details. Locations have a type, name
        and the ISRS Locode.
      operationId: getApiV1Locations
      x-api-path-slug: apiv1locations-get
      parameters:
      - in: query
        name: api_token
        description: authentication token of user making the request
      responses:
        200:
          description: OK
      tags:
      - List
  /api/v1/container_types:
    get:
      summary: List
      description: List all ContainerTypes
      operationId: getApiV1ContainerTypes
      x-api-path-slug: apiv1container-types-get
      parameters:
      - in: query
        name: api_token
        description: authentication token of user making the request
      responses:
        200:
          description: OK
      tags:
      - List
  /api/v1/organizations:
    get:
      summary: List
      description: List all registered organizations.
      operationId: getApiV1Organizations
      x-api-path-slug: apiv1organizations-get
      parameters:
      - in: query
        name: api_token
        description: authentication token of user making the request
      responses:
        200:
          description: OK
      tags:
      - List
  /api/v1/users:
    get:
      summary: List
      description: List all users registered.
      operationId: getApiV1Users
      x-api-path-slug: apiv1users-get
      parameters:
      - in: query
        name: api_token
        description: authentication token of user making the request
      responses:
        200:
          description: OK
      tags:
      - List