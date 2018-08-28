---
swagger: "2.0"
x-collection-name: Flat
x-complete: 0
info:
  title: Flat List liked scores
  description: ""
  termsOfService: https://flat.io/legal
  contact:
    name: Flat
    url: https://flat.io/support
    email: developers@flat.io
  version: 2.1.0
host: api.flat.io
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /groups/{group}/scores:
    get:
      summary: List group's scores
      description: Get the list of scores shared with a group.
      operationId: getGroupScores
      x-api-path-slug: groupsgroupscores-get
      parameters:
      - in: path
        name: group
        description: Unique identifier of the group
      - in: query
        name: parent
        description: Filter the score forked from the score id `parent`
      responses:
        200:
          description: OK
      tags:
      - List
      - Groups
      - Scores
  /scores/{score}/collaborators:
    get:
      summary: List the collaborators
      description: |-
        This API call will list the different collaborators of a score and their rights on the document. The returned list will at least contain the owner of the document.

        Collaborators can be a single user (the object `user` will be populated) or a group (the object `group` will be populated).
      operationId: getScoreCollaborators
      x-api-path-slug: scoresscorecollaborators-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - List
      - Collaborators
  /scores/{score}/comments:
    get:
      summary: List comments
      description: This method lists the different comments added on a music score
        (documents and inline) sorted by their post dates.
      operationId: getScoreComments
      x-api-path-slug: scoresscorecomments-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - List
      - Comments
  /scores/{score}/revisions:
    get:
      summary: List the revisions
      description: |-
        When creating a score or saving a new version of a score, a revision is created in our storage. This method allows you to list all of them, sorted by last modification.

        Depending the plan of the account, this list can be trunked to the few last revisions.
      operationId: getScoreRevisions
      x-api-path-slug: scoresscorerevisions-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - List
      - Revisions
  /users/{user}/likes:
    get:
      summary: List liked scores
      description: ""
      operationId: gerUserLikes
      x-api-path-slug: usersuserlikes-get
      parameters:
      - in: query
        name: ids
        description: Return only the identifiers of the scores
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - List
      - Liked
      - Scores
  /users/{user}/scores:
    get:
      summary: List user's scores
      description: Get the list of scores owned by the User
      operationId: getUserScores
      x-api-path-slug: usersuserscores-get
      parameters:
      - in: query
        name: No Name
      - in: query
        name: parent
        description: Filter the score forked from the score id `parent`
      responses:
        200:
          description: OK
      tags:
      - List
      - Users
      - Scores
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