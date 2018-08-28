---
swagger: "2.0"
x-collection-name: IDX Broker
x-complete: 0
info:
  title: IDX Broker Get List Methods
  description: A simple method for listing all available methods in the current API
    component.
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /mls/listcomponents:
    get:
      summary: Get Mls List Components
      description: This is a simple, access anywhere, method for getting a list of
        all API components available.
      operationId: MlsListcomponentsGet
      x-api-path-slug: mlslistcomponents-get
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: ancillarykey
      - in: header
        name: apiversion
      - in: header
        name: Content-Type
      - in: header
        name: outputtype
      responses:
        200:
          description: OK
      tags:
      - Mls
      - List
      - Components
  /clients/citieslistname:
    get:
      summary: Get Cities List Name
      description: Returns the IDs and names for each of a client's city lists including
        MLS city lists.
      operationId: ClientsCitieslistnameGet
      x-api-path-slug: clientscitieslistname-get
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: ancillarykey
      - in: header
        name: apiversion
      - in: header
        name: Content-Type
      - in: header
        name: outputtype
      responses:
        200:
          description: OK
      tags:
      - Cities
      - List
      - Name
  /clients/listallowedfields/{approvedMLS}/{featuredId}:
    get:
      summary: Get List Allowed Fields Approved MLS Featured
      description: Returns the allowed returnable fields for a given listingID.
      operationId: ClientsListallowedfieldsByApprovedMLSAndFeaturedIdGet
      x-api-path-slug: clientslistallowedfieldsapprovedmlsfeaturedid-get
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: ancillarykey
      - in: header
        name: apiversion
      - in: path
        name: approvedMLS
      - in: header
        name: Content-Type
      - in: path
        name: featuredId
      - in: header
        name: outputtype
      responses:
        200:
          description: OK
      tags:
      - List
      - Owed
      - Fields
      - Approved
      - MLS
      - Featured
  /clients/listmethods:
    get:
      summary: Get List Methods
      description: A simple method for listing all available methods in the current
        API component.
      operationId: ClientsListmethodsGet
      x-api-path-slug: clientslistmethods-get
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: ancillarykey
      - in: header
        name: apiversion
      - in: header
        name: Content-Type
      - in: header
        name: outputtype
      responses:
        200:
          description: OK
      tags:
      - List
      - Methods
  /leads/listcomponents:
    get:
      summary: Get Leads List Components
      description: This is a simple, access anywhere, method for getting a list of
        all API components available.
      operationId: LeadsListcomponentsGet
      x-api-path-slug: leadslistcomponents-get
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: ancillarykey
      - in: header
        name: apiversion
      - in: header
        name: Content-Type
      - in: header
        name: outputtype
      responses:
        200:
          description: OK
      tags:
      - Leads
      - List
      - Components
  /leads/listmethods:
    get:
      summary: Get Leads List Methods
      description: A simple method for listing all available methods in the current
        API component.
      operationId: LeadsListmethodsGet
      x-api-path-slug: leadslistmethods-get
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: ancillarykey
      - in: header
        name: apiversion
      - in: header
        name: Content-Type
      - in: header
        name: outputtype
      responses:
        200:
          description: OK
      tags:
      - Leads
      - List
      - Methods
  /partners/listcomponents:
    get:
      summary: Get Partners List Components
      description: This is a simple, access anywhere, method for getting a list of
        all API components available.
      operationId: PartnersListcomponentsGet
      x-api-path-slug: partnerslistcomponents-get
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: apiversion
      - in: header
        name: Content-Type
      - in: header
        name: outputtype
      responses:
        200:
          description: OK
      tags:
      - Partners
      - List
      - Components
  /partners/listmethods:
    get:
      summary: Get Partners List Methods
      description: A simple method for listing all available methods in the current
        API component.
      operationId: PartnersListmethodsGet
      x-api-path-slug: partnerslistmethods-get
      parameters:
      - in: header
        name: accesskey
      - in: header
        name: apiversion
      - in: header
        name: Content-Type
      - in: header
        name: outputtype
      responses:
        200:
          description: OK
      tags:
      - Partners
      - List
      - Methods
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