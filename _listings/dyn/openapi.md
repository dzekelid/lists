swagger: "2.0"
x-collection-name: Dyn
x-complete: 1
info:
  title: Dyn
  version: 1.0.0
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