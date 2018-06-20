---
swagger: "2.0"
x-collection-name: Reverb
x-complete: 1
info:
  title: reverb
  description: reverb
  termsOfService: https://reverb.com/page/terms
  contact:
    name: Reverb API
    url: https://dev.reverb.com
    email: integrations@reverb.com
  version: "3.0"
host: api.reverb.com
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /my/lists:
    get:
      summary: Get My Lists
      description: Get a list of your lists (wishlist, watch list, etc)
      operationId: getMyLists
      x-api-path-slug: mylists-get
      responses:
        200:
          description: OK
      tags:
      - My
      - Lists
---