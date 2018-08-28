swagger: "2.0"
x-collection-name: WebTRIS
x-complete: 1
info:
  title: ""
  version: 1.0.0
host: webtris.highwaysengland.co.uk
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v{version}/areas:
    get:
      summary: Returns list of areas
      description: Returns list of areas.
      operationId: Areas_Get
      x-api-path-slug: vversionareas-get
      parameters:
      - in: path
        name: version
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - Areas
  /v{version}/sites:
    get:
      summary: Get a list of sites
      description: Get a list of sites.
      operationId: Sites_Index
      x-api-path-slug: vversionsites-get
      parameters:
      - in: path
        name: version
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Sites
  /v{version}/sitetypes:
    get:
      summary: Return list of site types
      description: Return list of site types.
      operationId: SiteTypes_Index
      x-api-path-slug: vversionsitetypes-get
      parameters:
      - in: path
        name: version
      responses:
        200:
          description: OK
      tags:
      - Return
      - List
      - Of
      - Site
      - Types