---
swagger: "2.0"
x-collection-name: Mailgun
x-complete: 1
info:
  title: Mailgun API
  description: powerful-apis-that-allow-you-to-send-receive-and-track-email-effortlessly-
  version: v2
host: api.mailgun.net
basePath: v2/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  lists/:
    get:
      summary: Lists
      description: Returns a list of mailing lists under your account.
      operationId: getLists
      x-api-path-slug: lists-get
      parameters:
      - in: query
        name: access_level
        description: 'List access level, one of: readonly (default), members, everyone'
      - in: query
        name: address
        description: Find a mailing list by itu2019s address (optional)
      - in: query
        name: description
        description: Description string
      - in: query
        name: limit
        description: Maximum number of records to return (100 by default)
      - in: query
        name: namespace_id
        description: New name, e
      - in: query
        name: skip
        description: Records to skip (0 by default)
      responses:
        200:
          description: OK
      tags:
      - Lists
---