swagger: "2.0"
x-collection-name: 123FormBuilder
x-complete: 1
info:
  title: ""
  version: 1.0.0
host: api.123contactform.com
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /forms:
    get:
      summary: List forms
      description: The forms endpoint returns information about the forms. The response
        includes submissions and other details about each form.
      operationId: the-forms-endpoint-returns-information-about-the-forms-the-response-includes-submissions-and-other-d
      x-api-path-slug: forms-get
      parameters:
      - in: query
        name: JWT
        description: JWT authentication token
      - in: query
        name: page
        description: Page number
      - in: query
        name: per_page
        description: The number of forms to get per page in a request
      - in: query
        name: search
        description: Filter form name
      responses:
        200:
          description: OK
      tags:
      - List
      - Forms