swagger: "2.0"
x-collection-name: Charity Navigator
x-complete: 1
info:
  title: CharityNavigatorDataAPI
  description: the-charity-navigator-data-api-provides-access-to-charity-navigatorsratings-research-content-and-charitable-organization-profiles-
  version: 1.0.0
host: api.data.charitynavigator.org
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /Lists:
    get:
      summary: Get Lists
      description: |-
        Retrieve a set of Lists defined in Charity Navigator. Each entry in this
        collection is a curated or generated list of organizations, published by Charity
        Navigator. <br/> ![Content
        Subscription](https://cdn2.hubspot.net/hubfs/597611/CharityNavigator/FA-Data-Table-16.png
        "Included with the paid Content Subscription.")
      operationId: getLists
      x-api-path-slug: lists-get
      parameters:
      - in: query
        name: app_id
        description: '3Scale App ID: unique identifier for an application registered
          in theCharity Navigator  developer portal'
      - in: query
        name: app_key
        description: '3Scale App Key: a secret key to authenticate the assigned App
          ID'
      - in: query
        name: pageNum
        description: Page number to return, in case the number of available objects
          in the resultset is greater than the specified or default `pageSize`
      - in: query
        name: pageSize
        description: Number of objects to return in a single response message
      responses:
        200:
          description: OK
      tags:
      - Lists
  /Lists/{ListID}:
    get:
      summary: Get Lists List
      description: |-
        Retrieve a curated or generated list of organizations, published by Charity
        Navigator. <br/> ![Content
        Subscription](https://cdn2.hubspot.net/hubfs/597611/CharityNavigator/FA-Data-Table-16.png
        "Included with the paid Content Subscription.")
      operationId: getList
      x-api-path-slug: listslistid-get
      parameters:
      - in: query
        name: app_id
        description: '3Scale App ID: unique identifier for an application registered
          in theCharity Navigator  developer portal'
      - in: query
        name: app_key
        description: '3Scale App Key: a secret key to authenticate the assigned App
          ID'
      - in: path
        name: ListID
      responses:
        200:
          description: OK
      tags:
      - Lists
      - List