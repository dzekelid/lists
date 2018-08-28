swagger: "2.0"
x-collection-name: Yapily
x-complete: 1
info:
  title: Yapily API
  description: to-access-endpoints-that-require-authentication-use-your-application-key-and-secret-created-in-the-dashboard-httpsdashboard-yapily-com
  version: 1.0.0
host: api.yapily.com:443
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /institutions:
    get:
      summary: Retrieves the list of institutions available in Yapily
      description: Retrieves the list of institutions available in yapily.
      operationId: getInstitutionsUsingGET
      x-api-path-slug: institutions-get
      responses:
        200:
          description: OK
      tags:
      - Retrieves
      - List
      - Institutions
      - Available
      - In
      - Yapily