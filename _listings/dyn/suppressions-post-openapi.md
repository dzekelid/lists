---
swagger: "2.0"
x-collection-name: Dyn
x-complete: 0
info:
  title: Dyn Add Email Address to Suppression List
  version: 1.0.0
  description: Adding one or more recipients to the suppression list
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  suppressions:
    post:
      summary: Add Email Address to Suppression List
      description: Adding one or more recipients to the suppression list
      operationId: postSuppressions
      x-api-path-slug: suppressions-post
      parameters:
      - in: query
        name: apikey
        description: Required
      - in: query
        name: emailaddress
        description: Required
      responses:
        200:
          description: OK
      tags:
      - .Email
      - ress
      - to
      - Suppression
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