---
swagger: "2.0"
x-collection-name: IBM Financial Crimes Insight for Insurance
x-complete: 0
info:
  title: IBM Financial Crimes Insight for Insurance API Screen a specific attribute
    against a dynamic list
  description: This method is used to screen data against a specific list of values,
    resulting in a JSON object containing a list of matching objects
  version: 1.0.0
host: fcihost.ibm.com:9443
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /ibm/fci/platform/fact/entity/match:
    get:
      summary: Get a list of resolved objects from resolved entities for a given object.
      description: Get a list of resolved objects from resolved entities for a given
        object. Using the provided object ID, produce a list of all objects of the
        same business object type that have been determined to be 'matches'.
      operationId: getMatchedEntity
      x-api-path-slug: ibmfciplatformfactentitymatch-get
      parameters:
      - in: query
        name: count
        description: Number of objects to return; all if not included
      - in: header
        name: IBM-FCI-Role
        description: Userid / password for user with appropriate role
      - in: header
        name: IBM-FCI-Token
        description: Security token obtained for execution
      - in: query
        name: id
        description: Object id of the object
      - in: query
        name: logicalType
        description: Metadata element ID for a business object
      - in: query
        name: returnFlag
        description: Default value == 2
      - in: query
        name: threshold
        description: Minimum matching score to include a resolved entity; defaults
          to system property if not supplied
      - in: query
        name: type
        description: Stereotype for object
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Resolved
      - Objects
      - From
      - Resolved
      - Entitiesa
      - Given
      - Object
  /ibm/fci/platform/fact/screen:
    get:
      summary: Screen a specific attribute against a dynamic list
      description: This method is used to screen data against a specific list of values,
        resulting in a JSON object containing a list of matching objects
      operationId: screen
      x-api-path-slug: ibmfciplatformfactscreen-get
      parameters:
      - in: query
        name: context
        description: Registered context to which to filter / restrict this screen
      - in: query
        name: fieldName
        description: Field of the logical object to be searched
      - in: header
        name: IBM-FCI-Role
        description: Userid / password for user with appropriate role
      - in: header
        name: IBM-FCI-Token
        description: Security token obtained for execution
      - in: query
        name: objectType
        description: Business object name of the objects to search
      - in: query
        name: offset
        description: Used when more then max set of objects meet the criteria; when
          paging is required, this represents the paging offset
      - in: query
        name: style
        description: Searching style, defaults to SMART_MATCH
      - in: query
        name: values
        description: Comma separated list of values to search for in the local database
      responses:
        200:
          description: OK
      tags:
      - Screen
      - Specific
      - Attribute
      - Against
      - Dynamic
      - List
  /ibm/fci/platform/fact/watchlist:
    get:
      summary: Retrieve a list of the registered watchlists
      description: This method is used to retrieve the list of registered watchlists
        from the database
      operationId: getWatchlists
      x-api-path-slug: ibmfciplatformfactwatchlist-get
      parameters:
      - in: header
        name: IBM-FCI-Role
        description: Userid / password for user with appropriate role
      - in: header
        name: IBM-FCI-Token
        description: Security token obtained for execution
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - List
      - Of
      - Registered
      - Watchlists
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