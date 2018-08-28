---
swagger: "2.0"
x-collection-name: CollabNet
x-complete: 0
info:
  title: CollabNet TeamForge API Documentation Adds current user to specified project's
    member list
  version: 1.0.0
  description: Adds current user to specified project's member list.
basePath: /ctfrest/foundation/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /users/{userid}/projects/{projectid}:
    put:
      summary: Adds a user to specified project's member list by user id
      description: Adds a user to specified project's member list by user id.
      operationId: addUserById
      x-api-path-slug: usersuseridprojectsprojectid-put
      parameters:
      - in: path
        name: projectid
        description: Project id
      - in: path
        name: userid
        description: User id
      responses:
        200:
          description: OK
      tags:
      - User
      - To
      - Specified
      - Projects
      - Member
      - List
      - By
      - User
  /users/{userid}/projects:
    get:
      summary: Gets a user's project list by user id
      description: Gets a user's project list by user id.
      operationId: getProjectsByUserid
      x-api-path-slug: usersuseridprojects-get
      parameters:
      - in: query
        name: fetchHierarchyPath
      - in: query
        name: sortby
        description: Sort by column name
      - in: path
        name: userid
        description: User id
      responses:
        200:
          description: OK
      tags:
      - Users
      - Project
      - List
      - By
      - User
  /users/{userid}/groups:
    get:
      summary: Gets a user's group list by user id
      description: Gets a user's group list by user id.
      operationId: getUserGroupsByUserid
      x-api-path-slug: usersuseridgroups-get
      parameters:
      - in: path
        name: userid
        description: User id
      responses:
        200:
          description: OK
      tags:
      - Users
      - Group
      - List
      - By
      - User
  /users/myself/projects/{projectid}:
    put:
      summary: Adds current user to specified project's member list
      description: Adds current user to specified project's member list.
      operationId: addMyself
      x-api-path-slug: usersmyselfprojectsprojectid-put
      parameters:
      - in: path
        name: projectid
        description: Project id
      responses:
        200:
          description: OK
      tags:
      - Current
      - User
      - To
      - Specified
      - Projects
      - Member
      - List
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