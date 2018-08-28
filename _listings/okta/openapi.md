swagger: "2.0"
x-collection-name: Okta
x-complete: 1
info:
  title: Users (Okta API)
  description: the-okta-user-apidocsapirestusers-html-provides-operations-to-manage-users-in-your-organization-
  version: 1.0.0
host: example.com
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /users:
    get:
      summary: List Password Expired Users
      description: List password expired users.
      operationId: getUsers
      x-api-path-slug: users-get
      parameters:
      - in: header
        name: Accept
      - in: header
        name: Content-Type
      - in: query
        name: filter
      - in: query
        name: limit
      responses:
        200:
          description: OK
      tags:
      - List
      - Password
      - Expired
      - Users