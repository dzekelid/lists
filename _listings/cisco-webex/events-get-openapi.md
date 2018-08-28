---
swagger: "2.0"
x-collection-name: Cisco WebEx
x-complete: 0
info:
  title: Webex Teams Admin API List Events (new messages)
  description: |-
    List events in your organization. Several query parameters are available to filter the response.
    Long result sets will be split into pages.

    https://developer.webex.com/endpoint-events-get.html
  version: 1.0.0
host: api.ciscospark.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /events:
    get:
      summary: List Events (new messages)
      description: |-
        List events in your organization. Several query parameters are available to filter the response.
        Long result sets will be split into pages.

        https://developer.webex.com/endpoint-events-get.html
      operationId: EventsGet4
      x-api-path-slug: events-get
      parameters:
      - in: query
        name: resource
      - in: query
        name: type
      responses:
        200:
          description: OK
      tags:
      - Video Conferencing
      - List
      - Events
      - (new
      - Messages)
  /licenses:
    get:
      summary: List Licenses
      description: |-
        List all licenses for a given organization. If no orgId is specified, the default is the organization of the authenticated user.

        https://developer.webex.com/endpoint-licenses-get.html

        Example of a response:
        ``` json
        {
          'items' : [ {
            'id' : 'OTZhYmMyYWEtM2RjYy0xMWU1LWExNTItZmUzNDgxOWNkYzlh',
            'displayName' : 'Spark Calling',
            'totalUnits' : '42',
            'consumedUnits' : '8'
          } ]
        }
        ```
      operationId: LicensesGet
      x-api-path-slug: licenses-get
      responses:
        200:
          description: OK
      tags:
      - Video Conferencing
      - List
      - Licenses
  /organizations:
    get:
      summary: List Organizations
      description: |-
        List all organizations visible by your account.

        https://developer.webex.com/endpoint-organizations-get.html

        Example Response:
        ``` json
        {
          'items' : [ {
            'id' : 'OTZhYmMyYWEtM2RjYy0xMWU1LWExNTItZmUzNDgxOWNkYzlh',
            'displayName' : 'Acme, Inc.',
            'created' : '2015-10-18T14:26:16+00:00'
          } ]
        }
        ```
      operationId: OrganizationsGet
      x-api-path-slug: organizations-get
      responses:
        200:
          description: OK
      tags:
      - Video Conferencing
      - List
      - Organizations
  /people:
    get:
      summary: List people (with exact email)
      description: |-
        List people in your organization.

        https://developer.webex.com/endpoint-people-get.html
      operationId: PeopleGet
      x-api-path-slug: people-get
      parameters:
      - in: query
        name: email
      responses:
        200:
          description: OK
      tags:
      - Video Conferencing
      - List
      - People
      - (with
      - Exact
      - Email)
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