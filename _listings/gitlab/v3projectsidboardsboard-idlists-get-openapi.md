---
swagger: "2.0"
x-collection-name: GitLab
x-complete: 0
info:
  title: GitLab Get Projects Boards Board Lists
  version: 1.0.0
  description: Does not include `backlog` and `done` lists. This feature was introduced
    in 8.13
host: localhost:3000
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/projects/{id}/boards/{board_id}/lists:
    get:
      summary: Get Projects Boards Board Lists
      description: Does not include `backlog` and `done` lists. This feature was introduced
        in 8.13
      operationId: getV3ProjectsIdBoardsBoardIdLists
      x-api-path-slug: v3projectsidboardsboard-idlists-get
      parameters:
      - in: path
        name: board_id
        description: The ID of a board
      - in: path
        name: id
        description: The ID of a project
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Boards
      - Board
      - Lists
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