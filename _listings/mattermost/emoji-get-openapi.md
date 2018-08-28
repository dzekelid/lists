---
swagger: "2.0"
x-collection-name: Mattermost
x-complete: 0
info:
  title: Mattermost API Get a list of custom emoji
  description: |-
    Get a page of metadata for custom emoji on the system. Since server version 4.7, sort using the `sort` query parameter.
    ##### Permissions
    Must be authenticated.
  termsOfService: https://about.mattermost.com/default-terms/
  version: 4.0.0
host: your-mattermost-url.com
basePath: /api/v4
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /teams/{team_id}/channels/ids:
    post:
      summary: Get a list of channels by ids
      description: |-
        Get a list of public channels on a team by id.
        ##### Permissions
        `view_team` for the team the channels are on.
      operationId: get-a-list-of-public-channels-on-a-team-by-id-permissionsview-team-for-the-team-the-channels-are-on
      x-api-path-slug: teamsteam-idchannelsids-post
      parameters:
      - in: body
        name: body
        description: List of channel ids
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: team_id
        description: Team GUID
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Channels
      - By
      - Ids
  /users/{user_id}/posts/flagged:
    get:
      summary: Get a list of flagged posts
      description: |-
        Get a page of flagged posts of a user provided user id string. Selects from a channel, team or all flagged posts by a user.
        ##### Permissions
        Must be user or have `manage_system` permission.
      operationId: get-a-page-of-flagged-posts-of-a-user-provided-user-id-string-selects-from-a-channel-team-or-all-fla
      x-api-path-slug: usersuser-idpostsflagged-get
      parameters:
      - in: query
        name: channel_id
        description: Channel ID
      - in: query
        name: page
        description: The page to select
      - in: query
        name: per_page
        description: The number of posts per page
      - in: query
        name: team_id
        description: Team ID
      - in: path
        name: user_id
        description: ID of the user
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Flagged
      - Posts
  /users/{user_id}/preferences/{category}:
    get:
      summary: List a user's preferences by category
      description: |-
        Lists the current user's stored preferences in the given category.
        ##### Permissions
        Must be logged in as the user being updated or have the `edit_other_users` permission.
      operationId: lists-the-current-users-stored-preferences-in-the-given-category-permissionsmust-be-logged-in-as-the
      x-api-path-slug: usersuser-idpreferencescategory-get
      parameters:
      - in: path
        name: category
        description: The category of a group of preferences
      - in: path
        name: user_id
        description: User GUID
      responses:
        200:
          description: OK
      tags:
      - List
      - Users
      - Preferences
      - By
      - Category
  /emoji:
    get:
      summary: Get a list of custom emoji
      description: |-
        Get a page of metadata for custom emoji on the system. Since server version 4.7, sort using the `sort` query parameter.
        ##### Permissions
        Must be authenticated.
      operationId: get-a-page-of-metadata-for-custom-emoji-on-the-system-since-server-version-47-sort-using-the-sort-qu
      x-api-path-slug: emoji-get
      parameters:
      - in: query
        name: page
        description: The page to select
      - in: query
        name: per_page
        description: The number of users per page
      - in: query
        name: sort
        description: Either blank for no sorting or name to sort by emoji names
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Custom
      - Emoji
  /hooks/incoming:
    get:
      summary: List incoming webhooks
      description: |-
        Get a page of a list of incoming webhooks. Optionally filter for a specific team using query parameters.
        ##### Permissions
        `manage_webhooks` for the system or `manage_webhooks` for the specific team.
      operationId: get-a-page-of-a-list-of-incoming-webhooks-optionally-filter-for-a-specific-team-using-query-paramete
      x-api-path-slug: hooksincoming-get
      parameters:
      - in: query
        name: page
        description: The page to select
      - in: query
        name: per_page
        description: The number of hooks per page
      - in: query
        name: team_id
        description: The ID of the team to get hooks for
      responses:
        200:
          description: OK
      tags:
      - List
      - Incoming
      - Webhooks
  /hooks/outgoing:
    get:
      summary: List outgoing webhooks
      description: |-
        Get a page of a list of outgoing webhooks. Optionally filter for a specific team or channel using query parameters.
        ##### Permissions
        `manage_webhooks` for the system or `manage_webhooks` for the specific team/channel.
      operationId: get-a-page-of-a-list-of-outgoing-webhooks-optionally-filter-for-a-specific-team-or-channel-using-que
      x-api-path-slug: hooksoutgoing-get
      parameters:
      - in: query
        name: channel_id
        description: The ID of the channel to get hooks for
      - in: query
        name: page
        description: The page to select
      - in: query
        name: per_page
        description: The number of hooks per page
      - in: query
        name: team_id
        description: The ID of the team to get hooks for
      responses:
        200:
          description: OK
      tags:
      - List
      - Outgoing
      - Webhooks
  /commands:
    get:
      summary: List commands for a team
      description: |-
        List commands for a team.
        ##### Permissions
        `manage_slash_commands` if need list custom commands.
      operationId: list-commands-for-a-team-permissionsmanage-slash-commands-if-need-list-custom-commands
      x-api-path-slug: commands-get
      parameters:
      - in: query
        name: custom_only
        description: To get only the custom commands
      - in: query
        name: team_id
        description: The team id
      responses:
        200:
          description: OK
      tags:
      - List
      - Commandsa
      - Team
  /teams/{team_id}/commands/autocomplete:
    get:
      summary: List autocomplete commands
      description: |-
        List autocomplete commands in the team.
        ##### Permissions
        `view_team` for the team.
      operationId: list-autocomplete-commands-in-the-team-permissionsview-team-for-the-team
      x-api-path-slug: teamsteam-idcommandsautocomplete-get
      parameters:
      - in: path
        name: team_id
        description: Team GUID
      responses:
        200:
          description: OK
      tags:
      - List
      - Autocomplete
      - Commands
  /roles/names:
    post:
      summary: Get a list of roles by name
      description: |-
        Get a list of roles from their names.

        ##### Permissions
        Requires an active session but no other permissions.

        __Minimum server version__: 4.9
      operationId: get-a-list-of-roles-from-their-names-permissionsrequires-an-active-session-but-no-other-permissions-
      x-api-path-slug: rolesnames-post
      parameters:
      - in: body
        name: body
        description: List of role names
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Roles
      - By
      - Name
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