---
swagger: "2.0"
x-collection-name: SendGrid
x-complete: 0
info:
  title: SendGrid Get Contactdb Lists
  description: |-
    **This endpoint allows you to retrieve all of your recipient lists. If you don't have any lists, an empty array will be returned.**

    The Contacts API helps you manage your [Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html) recipients.
  version: 1.0.0
host: api.sendgrid.com
basePath: /v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /contactdb/lists:
    delete:
      summary: Delete Contactdb Lists
      description: |-
        **This endpoint allows you to delete multiple recipient lists.**

        The Contacts API helps you manage your [Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html) recipients.
      operationId: contactdb.lists.delete
      x-api-path-slug: contactdblists-delete
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Contactdb
      - Lists
    get:
      summary: Get Contactdb Lists
      description: |-
        **This endpoint allows you to retrieve all of your recipient lists. If you don't have any lists, an empty array will be returned.**

        The Contacts API helps you manage your [Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html) recipients.
      operationId: contactdb.lists.get
      x-api-path-slug: contactdblists-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Contactdb
      - Lists
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