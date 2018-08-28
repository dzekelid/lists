---
swagger: "2.0"
x-collection-name: Flowroute
x-complete: 0
info:
  title: FlowRoute API List Available Area Codes
  description: Returns a list of all Numbering Plan Area (NPA) codes containing purchasable
    phone numbers.
  version: 1.0.0
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v2/routes:
    get:
      summary: List Inbound Routes
      description: Returns a list of your inbound routes. From the list, you can then
        select routes to use as the primary and failover routes for a phone number,
        which you can do via "Update Primary Voice Route for a Phone Number" and "Update
        Failover Voice Route for a Phone Number".
      operationId: returns-a-list-of-your-inbound-routes-from-the-list-you-can-then-select-routes-to-use-as-the-primary
      x-api-path-slug: v2routes-get
      parameters:
      - in: query
        name: limit
        description: Limits the number of routes to retrieve
      - in: query
        name: offset
        description: Offsets the list of routes by your specified value
      - in: query
        name: route_type
        description: Restricts the results to inbound routes with your specified route
          type
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - List
      - Inbound
      - Routes
  /v2/numbers/available/exchanges:
    get:
      summary: List Available Exchange Codes
      description: Returns a list of all Central Office (exchange) codes containing
        purchasable phone numbers.
      operationId: returns-a-list-of-all-central-office-exchange-codes-containing-purchasable-phone-numbers
      x-api-path-slug: v2numbersavailableexchanges-get
      parameters:
      - in: query
        name: areacode
        description: Restricts the results to the specified area code
      - in: query
        name: limit
        description: Limits the number of items to retrieve
      - in: query
        name: max_setup_cost
        description: Restricts the results to exchanges that include at least one
          telephone number with a setup fee below or equal to the specified max_setup_cost
      - in: query
        name: offset
        description: Offsets the list of phone numbers by your specified value
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - List
      - Available
      - Exchange
      - Codes
  /v2/numbers/available/areacodes:
    get:
      summary: List Available Area Codes
      description: Returns a list of all Numbering Plan Area (NPA) codes containing
        purchasable phone numbers.
      operationId: returns-a-list-of-all-numbering-plan-area-npa-codes-containing-purchasable-phone-numbers
      x-api-path-slug: v2numbersavailableareacodes-get
      parameters:
      - in: query
        name: limit
        description: Limits the number of items to retrieve
      - in: query
        name: max_setup_cost
        description: Restricts the results to area codes that include at least one
          telephone number with a setup fee below or equal to the specified max_setup_cost
      - in: query
        name: offset
        description: Offsets the list of phone numbers by your specified value
      responses:
        200:
          description: OK
      tags:
      - Messaging
      - List
      - Available
      - Area
      - Codes
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