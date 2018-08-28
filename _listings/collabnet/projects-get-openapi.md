---
swagger: "2.0"
x-collection-name: CollabNet
x-complete: 0
info:
  title: CollabNet TeamForge API Documentation Gets paginated project list.
  version: 1.0.0
  description: Gets paginated project list..
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
  /users/myself/projects:
    get:
      summary: Gets current user's project list
      description: Gets current user's project list.
      operationId: getMyProjects
      x-api-path-slug: usersmyselfprojects-get
      parameters:
      - in: query
        name: fetchHierarchyPath
      - in: query
        name: sortby
        description: Sort by column name
      responses:
        200:
          description: OK
      tags:
      - Current
      - Users
      - Project
      - List
  /users/myself/groups:
    get:
      summary: Gets current user's group list
      description: Gets current user's group list.
      operationId: getMyUserGroups
      x-api-path-slug: usersmyselfgroups-get
      responses:
        200:
          description: OK
      tags:
      - Current
      - Users
      - Group
      - List
  /users/by-username/{username}/projects/{projectid}:
    put:
      summary: Adds a user to specified project's member list by username
      description: Adds a user to specified project's member list by username.
      operationId: addUserByUsername
      x-api-path-slug: usersbyusernameusernameprojectsprojectid-put
      parameters:
      - in: path
        name: projectid
        description: Project id
      - in: path
        name: username
        description: Username
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
      - Username
  /users/by-username/{username}/projects:
    get:
      summary: Gets a user's project list by username
      description: Gets a user's project list by username.
      operationId: getProjectsByUsername
      x-api-path-slug: usersbyusernameusernameprojects-get
      parameters:
      - in: query
        name: fetchHierarchyPath
      - in: query
        name: sortby
        description: Sort by column name
      - in: path
        name: username
        description: Username
      responses:
        200:
          description: OK
      tags:
      - Users
      - Project
      - List
      - By
      - Username
  /users/by-username/{username}/groups:
    get:
      summary: Gets a user's group list by username
      description: Gets a user's group list by username.
      operationId: getUserGroupsByUsername
      x-api-path-slug: usersbyusernameusernamegroups-get
      parameters:
      - in: path
        name: username
        description: Username
      responses:
        200:
          description: OK
      tags:
      - Users
      - Group
      - List
      - By
      - Username
  /users:
    get:
      summary: Gets paginated user list
      description: Gets paginated user list.
      operationId: getUsers
      x-api-path-slug: users-get
      parameters:
      - in: query
        name: count
        description: Max
      - in: query
        name: ids
        description: List of user ids (separated by comma)
      - in: query
        name: names
        description: List of usernames (separated by comma)
      - in: query
        name: offset
        description: Offset
      - in: query
        name: search
        description: Comma separated terms to search in username, fullname fields
      - in: query
        name: sortby
        description: Sort by column name
      - in: query
        name: status
        description: User status
      responses:
        200:
          description: OK
      tags:
      - Paginated
      - User
      - List
  /roles:
    get:
      summary: Gets global/site role list
      description: Gets global/site role list.
      operationId: getRoles
      x-api-path-slug: roles-get
      parameters:
      - in: query
        name: projectId
        description: Context project id (to verify access permissions)
      - in: query
        name: type
        description: Role type
      responses:
        200:
          description: OK
      tags:
      - Global
      - Site
      - Role
      - List
  /projecttemplates:
    get:
      summary: Gets paginated project template list.
      description: Gets paginated project template list..
      operationId: getProjectTemplates
      x-api-path-slug: projecttemplates-get
      parameters:
      - in: query
        name: count
        description: Max
      - in: query
        name: offset
        description: Offset
      - in: query
        name: sortby
        description: Sort by column name
      responses:
        200:
          description: OK
      tags:
      - Paginated
      - Project
      - Template
      - List
  /projects/{projectid}/subprojects:
    get:
      summary: Gets subproject list.
      description: Gets subproject list..
      operationId: getSubprojects
      x-api-path-slug: projectsprojectidsubprojects-get
      parameters:
      - in: query
        name: fetchHierarchyPath
      - in: path
        name: projectid
        description: Project identifier
      - in: query
        name: sortby
        description: Sort by column name
      responses:
        200:
          description: OK
      tags:
      - Subproject
      - List
  /projects/{projectid}/roles/inherited-roles:
    get:
      summary: Gets inherited project role list
      description: Gets inherited project role list.
      operationId: getInheritedProjectRoles
      x-api-path-slug: projectsprojectidrolesinheritedroles-get
      parameters:
      - in: path
        name: projectid
        description: Project identifier
      responses:
        200:
          description: OK
      tags:
      - Inherited
      - Project
      - Role
      - List
  /projects/{projectid}/roles:
    get:
      summary: Gets project role list
      description: Gets project role list.
      operationId: getProjectRoles
      x-api-path-slug: projectsprojectidroles-get
      parameters:
      - in: query
        name: includeInherited
        description: Include inherited roles? This parameter is relevant for Project
          type only
      - in: path
        name: projectid
        description: Project or project group identifier
      responses:
        200:
          description: OK
      tags:
      - Project
      - Role
      - List
  /projects/requests:
    get:
      summary: Gets paginated project request list
      description: Gets paginated project request list.
      operationId: getProjectRequests
      x-api-path-slug: projectsrequests-get
      parameters:
      - in: query
        name: count
        description: Max
      - in: query
        name: offset
        description: Offset
      responses:
        200:
          description: OK
      tags:
      - Paginated
      - Project
      - Request
      - List
  /projects:
    get:
      summary: Gets paginated project list.
      description: Gets paginated project list..
      operationId: getProjects
      x-api-path-slug: projects-get
      parameters:
      - in: query
        name: count
        description: Max
      - in: query
        name: fetchHierarchyPath
      - in: query
        name: offset
        description: Offset
      - in: query
        name: searchvalue
      - in: query
        name: sortby
        description: Sort by column name
      responses:
        200:
          description: OK
      tags:
      - Paginated
      - Project
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