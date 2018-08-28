---
swagger: "2.0"
info:
  title: Akamai API Modify a Network List
  description: Modify a Network List
  version: 1.0.0
host: developer.akamai.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /network-list/v1/network_lists/{networkListId}:
    put:
      summary: Modify a Network List
      description: Modify a Network List
      operationId: networklistv1network-listsnetworklistidextended
      parameters:
      - in: query
        name: extended
        description: If enabled, returns more verbose data such as creation date and
          activation status
        type: string
      - in: query
        name: networkListId
        description: Unique identifier for the network list, corresponding to the
          unique-id within the data
        type: string
      responses:
        200:
          description: OK
      tags:
      - network
      - list
      - network
      - lists
      - networklist
      - extended
definitions: []
x-collection-name: Akamai
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