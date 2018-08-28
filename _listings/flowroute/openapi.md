swagger: "2.0"
x-collection-name: Flowroute
x-complete: 1
info:
  title: Flowroute APIs
  description: the-flowroute-apis-are-organized-around-rest--our-apis-have-resourceoriented-urls-support-http-verbs-and-respond-with-http-status-codes--all-api-requests-and-responses-including-errors-will-be-represented-as-json-objects--you-can-use-the-flowroute-apis-to-manage-your-flowroute-phone-numbers-including-setting-primary-and-failover-routes-for-inbound-calls-and-sending-text-messages-sms-and-mms-using-longcode-or-tollfree-numbers-in-your-account-
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