---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Lists instances of a given workflow
  version: 1.0.0
  description: Lists instances of a given workflow.
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/admin/businessworkflow/{workflowName}:
    get:
      summary: Lists instances of a given workflow
      description: Lists instances of a given workflow.
      operationId: BusinessWorkflow_ListWorkflowInstancesByworkflowNameByskipBytake
      x-api-path-slug: apiadminbusinessworkflowworkflowname-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: skip
      - in: query
        name: take
      - in: path
        name: workflowName
      responses:
        200:
          description: OK
      tags:
      - Lists
      - Instances
      - Of
      - Given
      - Workflow
  /api/negotiator/my/properties/favourite:
    get:
      summary: Lists favourited properties
      description: Lists favourited properties.
      operationId: Negotiator_FavouritePropertiesBypageSizeBypageNumber
      x-api-path-slug: apinegotiatormypropertiesfavourite-get
      parameters:
      - in: query
        name: pageNumber
        description: Page number
      - in: query
        name: pageSize
        description: Page Size
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Lists
      - Favourited
      - Properties
  /api/admin/system/ListAgencies:
    get:
      summary: Lists the name and ID of all agencies in the system.
      description: Lists the name and id of all agencies in the system..
      operationId: System_ListAgenciesByincludeSuspended
      x-api-path-slug: apiadminsystemlistagencies-get
      parameters:
      - in: query
        name: includeSuspended
        description: if set to true [include suspended]
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Lists
      - Name
      - ID
      - Of
      - ""
      - Agencies
      - In
      - System
  /api/webhook/list:
    get:
      summary: Lists all of the webhooks currently set up.
      description: Lists all of the webhooks currently set up..
      operationId: Webhook_ListWebhooksBytriggerFilterName
      x-api-path-slug: apiwebhooklist-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: triggerFilterName
        description: Optionally, filter results that match this trigger
      responses:
        200:
          description: OK
      tags:
      - Lists
      - ""
      - Of
      - Webhooks
      - Currently
      - Set
      - Up
  /api/workflow/triggers:
    get:
      summary: Lists the available triggers that are able to start workflows.
      description: Lists the available triggers that are able to start workflows..
      operationId: Workflow_GetTriggerTypes
      x-api-path-slug: apiworkflowtriggers-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Lists
      - Available
      - Triggers
      - That
      - Are
      - Able
      - To
      - Start
      - Workflows
  /api/workflow/listWorkflows:
    get:
      summary: Lists available workflows
      description: Lists available workflows.
      operationId: Workflow_ListWorkflowsByskipBytake
      x-api-path-slug: apiworkflowlistworkflows-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: skip
        description: Used for paging results
      - in: query
        name: take
        description: Used for paging results
      responses:
        200:
          description: OK
      tags:
      - Lists
      - Available
      - Workflows
  /api/workflow/{workflowName}:
    get:
      summary: Lists instances of a given workflow
      description: Lists instances of a given workflow.
      operationId: Workflow_ListWorkflowInstancesByworkflowNameByskipBytake
      x-api-path-slug: apiworkflowworkflowname-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: skip
      - in: query
        name: take
      - in: path
        name: workflowName
      responses:
        200:
          description: OK
      tags:
      - Lists
      - Instances
      - Of
      - Given
      - Workflow
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