---
swagger: "2.0"
x-collection-name: Logicbroker
x-complete: 0
info:
  title: Logic Broker CommerceAPI Get a list of all attachments matching a given filter.
  version: 1.0.0
  description: Request rate limited to 10 requests per second with bursts up to 100
    requests.
host: stage.commerceapi.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/Webhooks:
    get:
      summary: Get list of webhooks
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Webhook_GetWebHooks
      x-api-path-slug: apiv1webhooks-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Webhooks
  /api/v1/Partners:
    get:
      summary: Retrieve a list of trading partners.
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Partner_GetPartners
      x-api-path-slug: apiv1partners-get
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - List
      - Of
      - Trading
      - Partners
  /api/v1/Orders/{LogicbrokerKey}/Returns:
    get:
      summary: Retrieve a list of returns for an order
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Order_GetReturns
      x-api-path-slug: apiv1orderslogicbrokerkeyreturns-get
      parameters:
      - in: path
        name: LogicbrokerKey
        description: The Logicbroker key
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - List
      - Of
      - Returnsan
      - Order
  /api/v1/Orders/{LogicbrokerKey}/Shipments:
    get:
      summary: Retrieve a list of shipments for an order
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Order_GetASN
      x-api-path-slug: apiv1orderslogicbrokerkeyshipments-get
      parameters:
      - in: path
        name: LogicbrokerKey
        description: The Logicbroker key
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - List
      - Of
      - Shipmentsan
      - Order
  /api/v1/Orders/{LogicbrokerKey}/Invoices:
    get:
      summary: Retrieve a list of invoices for an order
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Order_GetInvoice
      x-api-path-slug: apiv1orderslogicbrokerkeyinvoices-get
      parameters:
      - in: path
        name: LogicbrokerKey
        description: The Logicbroker key
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - List
      - Of
      - Invoicesan
      - Order
  /api/v1/Attachments:
    get:
      summary: Get a list of all attachments matching a given filter.
      description: Request rate limited to 10 requests per second with bursts up to
        100 requests.
      operationId: Attachment_GetList
      x-api-path-slug: apiv1attachments-get
      parameters:
      - in: query
        name: acknowledged
        description: Acknowledged flag
      - in: query
        name: logicbrokerKey
        description: Logicbroker key
      - in: query
        name: page
        description: Page number
      - in: query
        name: receiverId
        description: Receiver account number
      - in: query
        name: type
        description: Attachment type
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - ""
      - Attachments
      - Matching
      - Given
      - Filter
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