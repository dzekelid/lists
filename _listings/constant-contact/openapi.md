---
swagger: "2.0"
x-collection-name: Constant Contact
x-complete: 1
info:
  title: Constant Contact
  description: make-constant-contacts-leading-email-and-event-marketing-services-accessible-directly-from-your-app-
  version: 1.0.0
host: api.constantcontact.com
basePath: /ws/customers/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{username}/lists:
    get:
      summary: Get All Mailing Lists
      description: Get All Mailing Lists
      operationId: get-all-mailing-lists
      x-api-path-slug: usernamelists-get
      parameters:
      - in: path
        name: username
      responses:
        200:
          description: OK
      tags:
      - Mailing
      - Lists
---