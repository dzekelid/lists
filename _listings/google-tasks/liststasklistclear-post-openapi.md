---
swagger: "2.0"
x-collection-name: Google Tasks
x-complete: 0
info:
  title: Google Tasks API Add Lists Task List Clear
  description: Clears all completed tasks from the specified task list. The affected
    tasks will be marked as 'hidden' and no longer be returned by default when retrieving
    all tasks for a task list.
  contact:
    name: Google
    url: https://google.com
  version: v1
host: www.googleapis.com
basePath: /tasks/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /lists/{tasklist}/clear:
    post:
      summary: Add Lists Task List Clear
      description: Clears all completed tasks from the specified task list. The affected
        tasks will be marked as 'hidden' and no longer be returned by default when
        retrieving all tasks for a task list.
      operationId: tasks.tasks.clear
      x-api-path-slug: liststasklistclear-post
      parameters:
      - in: path
        name: tasklist
        description: Task list identifier
      responses:
        200:
          description: OK
      tags:
      - Lists
      - Task
      - List
      - Clear
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