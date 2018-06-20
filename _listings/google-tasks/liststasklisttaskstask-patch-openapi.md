---
swagger: "2.0"
x-collection-name: Google Tasks
x-complete: 0
info:
  title: Google Tasks API Patch Lists Task List Tasks Task
  description: Updates the specified task. This method supports patch semantics.
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
  /lists/{tasklist}/tasks:
    get:
      summary: Get Lists Task List Tasks
      description: Returns all tasks in the specified task list.
      operationId: tasks.tasks.list
      x-api-path-slug: liststasklisttasks-get
      parameters:
      - in: query
        name: completedMax
        description: Upper bound for a tasks completion date (as a RFC 3339 timestamp)
          to filter by
      - in: query
        name: completedMin
        description: Lower bound for a tasks completion date (as a RFC 3339 timestamp)
          to filter by
      - in: query
        name: dueMax
        description: Upper bound for a tasks due date (as a RFC 3339 timestamp) to
          filter by
      - in: query
        name: dueMin
        description: Lower bound for a tasks due date (as a RFC 3339 timestamp) to
          filter by
      - in: query
        name: maxResults
        description: Maximum number of task lists returned on one page
      - in: query
        name: pageToken
        description: Token specifying the result page to return
      - in: query
        name: showCompleted
        description: Flag indicating whether completed tasks are returned in the result
      - in: query
        name: showDeleted
        description: Flag indicating whether deleted tasks are returned in the result
      - in: query
        name: showHidden
        description: Flag indicating whether hidden tasks are returned in the result
      - in: path
        name: tasklist
        description: Task list identifier
      - in: query
        name: updatedMin
        description: Lower bound for a tasks last modification time (as a RFC 3339
          timestamp) to filter by
      responses:
        200:
          description: OK
      tags:
      - Lists
      - Task
      - List
      - Tasks
    post:
      summary: Add Lists Task List Tasks
      description: Creates a new task on the specified task list.
      operationId: tasks.tasks.insert
      x-api-path-slug: liststasklisttasks-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: parent
        description: Parent task identifier
      - in: query
        name: previous
        description: Previous sibling task identifier
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
      - Tasks
  /lists/{tasklist}/tasks/{task}:
    delete:
      summary: Delete Lists Task List Tasks Task
      description: Deletes the specified task from the task list.
      operationId: tasks.tasks.delete
      x-api-path-slug: liststasklisttaskstask-delete
      parameters:
      - in: path
        name: task
        description: Task identifier
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
      - Tasks
      - Task
    get:
      summary: Get Lists Task List Tasks Task
      description: Returns the specified task.
      operationId: tasks.tasks.get
      x-api-path-slug: liststasklisttaskstask-get
      parameters:
      - in: path
        name: task
        description: Task identifier
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
      - Tasks
      - Task
    patch:
      summary: Patch Lists Task List Tasks Task
      description: Updates the specified task. This method supports patch semantics.
      operationId: tasks.tasks.patch
      x-api-path-slug: liststasklisttaskstask-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: task
        description: Task identifier
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
      - Tasks
      - Task
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