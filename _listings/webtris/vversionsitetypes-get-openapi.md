---
swagger: "2.0"
x-collection-name: WebTRIS
x-complete: 0
info:
  title: WebTRIS Traffic Flow API Return list of site types
  version: 1.0.0
  description: Return list of site types.
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