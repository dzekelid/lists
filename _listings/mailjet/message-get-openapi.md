---
swagger: "2.0"
x-collection-name: Mailjet
x-complete: 0
info:
  title: Mailjet Messages API Message List
  description: Allows you to list messages.
  version: v3
host: api.mailjet.com
basePath: v3/REST/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  message/:
    get:
      summary: Message List
      description: Allows you to list messages.
      operationId: getMessage
      x-api-path-slug: message-get
      parameters:
      - in: query
        name: Campaign
        description: Only retrieve message resources for which Campaign ID equals
          the specified value
      - in: query
        name: Contact
        description: Only retrieve message resources for which Contact ID equals the
          specified value
      - in: query
        name: MessageState
        description: Only show messages with this state
      - in: query
        name: PlanSubscription
        description: Only retrieve message resources for which PlanSubscription ID
          equals the specified value
      - in: query
        name: Sender
        description: Only show messages from this sender
      responses:
        200:
          description: OK
      tags:
      - Message
      - List
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