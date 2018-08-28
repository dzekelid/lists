---
swagger: "2.0"
x-collection-name: Cisco WebEx
x-complete: 0
info:
  title: WebEx Teams API List messages
  description: "Lists all messages in a room. If present, includes the associated
    media content attachment for each message.\r\n\r\nThe list sorts the messages
    in descending order by creation date.\r\n\r\nhttps://developer.webex.com/endpoint-messages-get.html"
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
      summary: List people (whose name starts with)
      description: |-
        List people in your organization.

        https://developer.webex.com/endpoint-people-get.html
      operationId: PeopleGet2
      x-api-path-slug: people-get
      parameters:
      - in: query
        name: displayName
      responses:
        200:
          description: OK
      tags:
      - Video Conferencing
      - List
      - People
      - (whose
      - Name
      - Starts
      - With)
  /webhooks:
    get:
      summary: List webhooks
      description: |-
        Lists all of your webhooks.

        https://developer.webex.com/endpoint-webhooks-get.html
      operationId: WebhooksGet
      x-api-path-slug: webhooks-get
      responses:
        200:
          description: OK
      tags:
      - Video Conferencing
      - List
      - Webhooks
  /rooms:
    get:
      summary: List rooms
      description: "List rooms.\r\n\r\nBy default, lists rooms to which the authenticated
        user belongs.\r\n\r\nhttps://developer.webex.com/endpoint-rooms-get.html"
      operationId: RoomsGet3
      x-api-path-slug: rooms-get
      responses:
        200:
          description: OK
      tags:
      - Video Conferencing
      - List
      - Rooms
  /messages:
    get:
      summary: List messages
      description: "Lists all messages in a room. If present, includes the associated
        media content attachment for each message.\r\n\r\nThe list sorts the messages
        in descending order by creation date.\r\n\r\nhttps://developer.webex.com/endpoint-messages-get.html"
      operationId: MessagesGet
      x-api-path-slug: messages-get
      parameters:
      - in: query
        name: roomId
      responses:
        200:
          description: OK
      tags:
      - Video Conferencing
      - List
      - Messages
  /teams:
    get:
      summary: List teams
      description: |-
        List teams.

        https://developer.webex.com/endpoint-teams-get.html
      operationId: TeamsGet
      x-api-path-slug: teams-get
      responses:
        200:
          description: OK
      tags:
      - Video Conferencing
      - List
      - Teams
  /memberships:
    get:
      summary: List memberships (for all rooms)
      description: |-
        Lists all room memberships. By default, lists memberships for rooms to which the authenticated user belongs.

        Use query parameters to filter the response.

        Use roomId to list memberships for a room, by ID.

        Use either personId or personEmail to filter the results.

        https://developer.webex.com/endpoint-memberships-get.html
      operationId: MembershipsGet2
      x-api-path-slug: memberships-get
      responses:
        200:
          description: OK
      tags:
      - Video Conferencing
      - List
      - Memberships
      - (for
      - ""
      - Rooms)
  /team/memberships:
    get:
      summary: List team memberships
      description: "Lists all team memberships. By default, lists memberships for
        teams to which the authenticated user belongs.\r\n\r\nUse query parameters
        to filter the response.\r\n\r\nUse teamId to list memberships for a team,
        by ID.\r\n\r\nUse either personId or personEmail to filter the results.\r\n\r\nhttps://developer.webex.com/endpoint-teammemberships-get.html"
      operationId: TeamMembershipsGet
      x-api-path-slug: teammemberships-get
      parameters:
      - in: query
        name: teamId
      responses:
        200:
          description: OK
      tags:
      - Video Conferencing
      - List
      - Team
      - Memberships
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