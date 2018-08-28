---
swagger: "2.0"
x-collection-name: Twitter
x-complete: 0
info:
  title: Twitter Help Terms of Services
  description: Returns the Twitter Terms of Service
  version: "1.1"
host: api.twitter.com
basePath: /1.1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /lists/list:
    get:
      summary: List LIst
      description: Return all lists the authenticating or specified user subscribes
        to, including their own.
      operationId: return-all-lists-the-authenticating-or-specified-user-subscribes-to-including-their-own
      x-api-path-slug: listslist-get
      parameters:
      - in: query
        name: screen_name
        description: The screen name of the user for whom to return results for
      - in: query
        name: user_id
        description: The ID of the user for whom to return results for
      responses:
        200:
          description: OK
      tags:
      - Social
      - Lists
  /lists/statuses.json:
    get:
      summary: List Statuses
      description: Returns a timeline of tweets authored by memebers of the specified
        list
      operationId: returns-a-timeline-of-tweets-authored-by-memebers-of-the-specified-list
      x-api-path-slug: listsstatuses-json-get
      parameters:
      - in: query
        name: count
        description: Specifies the number of results to retrieve per page
      - in: query
        name: include_entities
        description: Entities are ON by default
      - in: query
        name: include_rts
        description: When set to either true, t or 1, the list timeline will contain
          native retweets in addition to the standard stream of tweets
      - in: query
        name: list_id
        description: The numerical id of the list
      - in: query
        name: max_id
        description: Returns results with an ID less than or equal to the specified
          ID
      - in: query
        name: owner_id
        description: The user ID of the user who owns the list being requested by
          a slug
      - in: query
        name: owner_screen_name
        description: The screen name of the user who owns the list being requested
          by a slug
      - in: query
        name: since_id
        description: Returns results with an ID greater than the sepcified ID
      - in: query
        name: slug
        description: You can identify a list by its slug instead of its numerical
          id
      responses:
        200:
          description: OK
      tags:
      - Social
      - Lists
  /lists/members/destroy:
    get:
      summary: Remove User From List
      description: Returns the list of memebers destroy
      operationId: returns-the-list-of-memebers-destroy
      x-api-path-slug: listsmembersdestroy-get
      parameters:
      - in: query
        name: list_id
        description: The numerical id of the list
      - in: query
        name: owner_id
        description: The is of the user who wons the list being requested by a slug
      - in: query
        name: owner_screen_name
        description: The screen name of the user who owns the list being requested
          by a slug
      - in: query
        name: screen_name
        description: The screen name of the user for whom to remove from the list
      - in: query
        name: slug
        description: You can identify a list by its slug instrad of its numerical
          id
      - in: query
        name: user_id
        description: The id of the user for whom to remove from the list
      responses:
        200:
          description: OK
      tags:
      - Social
      - Lists
  /lists/memberships:
    get:
      summary: Get Memberships
      description: Returns the lists of the specified user has been added to
      operationId: returns-the-lists-of-the-specified-user-has-been-added-to
      x-api-path-slug: listsmemberships-get
      parameters:
      - in: query
        name: cursor
        description: Breaks the results into pages
      - in: query
        name: filter_to_owned_lists
        description: When set to true, t or 1, will return just lists the authenticating
          user owns
      - in: query
        name: screen_name
        description: The screen name of the user for whom to return results for
      - in: query
        name: user_id
        description: The id of the user for whom to return results for
      responses:
        200:
          description: OK
      tags:
      - Social
      - Lists
  /lists/subscribers:
    get:
      summary: List Subscribers
      description: Returns the subscribers of the specified list
      operationId: returns-the-subscribers-of-the-specified-list
      x-api-path-slug: listssubscribers-get
      parameters:
      - in: query
        name: cursor
        description: Breaks the results into pages
      - in: query
        name: include_entities
        description: Wehn set to either true, t or 1
      - in: query
        name: list_id
        description: The numerical id of the list
      - in: query
        name: owner_id
        description: The user ID of the user who owns the list being requested by
          a slug
      - in: query
        name: owner_screen_name
        description: the screen name of the user who owns the list being requested
          by a slug
      - in: query
        name: skip_status
        description: When set to either true, t or 1
      - in: query
        name: slug
        description: You can identify a list by its slug insted of its numerical id
      responses:
        200:
          description: OK
      tags:
      - Social
      - Lists
  /lists/subscribers/create:
    post:
      summary: Add List Subscribers
      description: Subscribes the authenticated user to the specified list
      operationId: subscribes-the-authenticated-user-to-the-specified-list
      x-api-path-slug: listssubscriberscreate-post
      parameters:
      - in: query
        name: list_id
        description: The numerical id of the list
      - in: query
        name: owner_id
        description: The user ID of the user who owns the list being requested by
          a slug
      - in: query
        name: owner_screen_name
        description: the screen name of the user who owns the list being requested
          by a slug
      - in: query
        name: slug
        description: You can identify a list being requested by a slug
      responses:
        200:
          description: OK
      tags:
      - Social
      - Lists
  /lists/subscribers/show:
    get:
      summary: Show List Subscribers
      description: Check if the specified user is a subscriber of the specified list
      operationId: check-if-the-specified-user-is-a-subscriber-of-the-specified-list
      x-api-path-slug: listssubscribersshow-get
      parameters:
      - in: query
        name: include_entities
        description: Wehn set to either true, t or 1
      - in: query
        name: list_id
        description: The numerical id of the list
      - in: query
        name: owner_id
        description: The is of the user who wons the list being requested by a slug
      - in: query
        name: owner_screen_name
        description: The screen name of the user who owns the list being requested
          by a slug
      - in: query
        name: screen_name
        description: The screen name of the user for whom to remove from the list
      - in: query
        name: skip_status
        description: When set to either true, t or 1
      - in: query
        name: slug
        description: You can identify a list being requested by a slug
      - in: query
        name: user_id
        description: The id of the user for whom to remove from the list
      responses:
        200:
          description: OK
      tags:
      - Social
      - Lists
  /lists/subscribers/destroy:
    get:
      summary: Remove List Subscribers
      description: Returns list of subscribers destroy
      operationId: returns-list-of-subscribers-destroy
      x-api-path-slug: listssubscribersdestroy-get
      parameters:
      - in: query
        name: list_id
        description: The numerical id of the list
      - in: query
        name: owner_id
        description: The user ID of the user who owns the list being requested by
          a slug
      - in: query
        name: owner_screen_name
        description: the screen name of the user who owns the list being requested
          by a slug
      - in: query
        name: slug
        description: You can identify a list being requested by a slug
      responses:
        200:
          description: OK
      tags:
      - Social
      - Lists
  /lists/members/create_all:
    get:
      summary: Add Users to List
      description: Returns lists of members create_all
      operationId: returns-lists-of-members-create-all
      x-api-path-slug: listsmemberscreate-all-get
      parameters:
      - in: query
        name: list_id
        description: The numerical id of the list
      - in: query
        name: owner_id
        description: The user ID of the user who owns the list being requested by
          a slug
      - in: query
        name: owner_screen_name
        description: the screen name of the user who owns the list being requested
          by a slug
      - in: query
        name: screen_name
        description: The screen name of the user for whom to remove from the list
      - in: query
        name: slug
        description: You can identify a list being requested by a slug
      - in: query
        name: user_id
        description: The id of the user for whom to remove from the list
      responses:
        200:
          description: OK
      tags:
      - Social
      - Lists
  /list/members/show:
    get:
      summary: Show Members
      description: Check if the specified user is a member of the specified list
      operationId: check-if-the-specified-user-is-a-member-of-the-specified-list
      x-api-path-slug: listmembersshow-get
      parameters:
      - in: query
        name: include_entities
        description: Wehn set to either true, t or 1
      - in: query
        name: list_id
        description: The numerical id of the list
      - in: query
        name: owner_id
        description: The user ID of the user who owns the list being requested by
          a slug
      - in: query
        name: owner_screen_name
        description: The screen name of the user who owns the list being requested
          by a slug
      - in: query
        name: screen_name
        description: The screen name of the user for whom to remove from the list
      - in: query
        name: skip_status
        description: When set to either true, t or 1
      - in: query
        name: slug
        description: You can identify a list being requested by a slug
      - in: query
        name: user_id
        description: The id of the user for whom to remove from the list
      responses:
        200:
          description: OK
      tags:
      - Social
      - Lists
  /list/members:
    get:
      summary: Get Members
      description: Returns the members of the specified list
      operationId: returns-the-members-of-the-specified-list
      x-api-path-slug: listmembers-get
      parameters:
      - in: query
        name: cursor
        description: Breaks the results into pages
      - in: query
        name: include_entities
        description: Wehn set to either true, t or 1
      - in: query
        name: list_id
        description: The numerical id of the list
      - in: query
        name: owner_id
        description: The user ID of the user who owns the list being requested by
          a slug
      - in: query
        name: owner_screen_name
        description: The screen name of the user who owns the list being requested
          by a slug
      - in: query
        name: skip_status
        description: When set to either true, t or 1
      - in: query
        name: slug
        description: You can identify a list being requested by a slug
      responses:
        200:
          description: OK
      tags:
      - Social
      - Lists
  /list/members/create:
    post:
      summary: Add Member
      description: Returns list of members create
      operationId: returns-list-of-members-create
      x-api-path-slug: listmemberscreate-post
      parameters:
      - in: query
        name: list_id
        description: The numerical id of the list
      - in: query
        name: owner_id
        description: The user ID of the user who owns the list being requested by
          a slug
      - in: query
        name: owner_screen_name
        description: The screen name of the user who owns the list being requested
          by a slug
      - in: query
        name: screen_name
        description: The screen name of the user for whom to remove from the list
      - in: query
        name: slug
        description: You can identify a list being requested by a slug
      responses:
        200:
          description: OK
      tags:
      - Social
      - Lists
  /lists/destroy:
    post:
      summary: Destroy List
      description: Returns list of destroy
      operationId: returns-list-of-destroy
      x-api-path-slug: listsdestroy-post
      parameters:
      - in: query
        name: list_id
        description: The numerical id of the list
      - in: query
        name: owner_id
        description: The user ID of the user who owns the list being requested by
          a slug
      - in: query
        name: owner_screen_name
        description: The screen name of the user who owns the list being requested
          by a slug
      - in: query
        name: slug
        description: You can identify a list being requested by a slug
      responses:
        200:
          description: OK
      tags:
      - Social
      - Lists
  /lists/update:
    post:
      summary: Update List
      description: Returns lists of updates
      operationId: returns-lists-of-updates
      x-api-path-slug: listsupdate-post
      parameters:
      - in: query
        name: description
        description: The description to give the list
      - in: query
        name: list_id
        description: The numerical id of the list
      - in: query
        name: mode
        description: Whether your list is public or private
      - in: query
        name: name
        description: The name for the list
      - in: query
        name: owner_id
        description: The user ID of the user who owns the list being requested by
          a slug
      - in: query
        name: owner_screen_name
        description: The screen name of the user who owns the list being requested
          by a slug
      - in: query
        name: slug
        description: You can identify a list being requested by a slug
      responses:
        200:
          description: OK
      tags:
      - Social
      - Lists
  /lists/create:
    post:
      summary: Create List
      description: Returns list of create
      operationId: returns-list-of-create
      x-api-path-slug: listscreate-post
      parameters:
      - in: query
        name: description
        description: The description to give the list
      - in: query
        name: mode
        description: Whether your list is public or private
      - in: query
        name: name
        description: The name for the list
      responses:
        200:
          description: OK
      tags:
      - Social
      - Lists
  /lists/show:
    get:
      summary: Show LIsts
      description: Returns list of show
      operationId: returns-list-of-show
      x-api-path-slug: listsshow-get
      parameters:
      - in: query
        name: list_id
        description: The numerical id of the list
      - in: query
        name: owner_id
        description: The user ID of the user who owns the list being requested by
          a slug
      - in: query
        name: owner_screen_name
        description: The screen name of the user who owns the list being requested
          by a slug
      - in: query
        name: slug
        description: You can identify a list being requested by a slug
      responses:
        200:
          description: OK
      tags:
      - Social
      - Lists
  /lists/subscriptions:
    get:
      summary: Show List Subscriptions
      description: Returns list of subscriptions
      operationId: returns-list-of-subscriptions
      x-api-path-slug: listssubscriptions-get
      parameters:
      - in: query
        name: count
        description: The amount of results to return per page
      - in: query
        name: cursor
        description: Breaks the results into pages
      - in: query
        name: screen_name
        description: The screen name of the user
      - in: query
        name: user_id
        description: The id of the user for whom to return results for
      responses:
        200:
          description: OK
      tags:
      - Social
      - Lists
  /list/members/destroy_all:
    get:
      summary: Remove Members
      description: Returns lists of destroy all
      operationId: returns-lists-of-destroy-all
      x-api-path-slug: listmembersdestroy-all-get
      parameters:
      - in: query
        name: list_id
        description: The numerical id of the list
      - in: query
        name: owner_id
        description: The user ID of the user who owns the list being requested by
          a slug
      - in: query
        name: owner_screen_name
        description: The screen name of the user who owns the list being requested
          by a slug
      - in: query
        name: screen_name
        description: The screen name of the user for whom to remove from the list
      - in: query
        name: slug
        description: You can identify a list being requested by a slug
      - in: query
        name: user_id
        description: The id of the user for whom to remove from the list
      responses:
        200:
          description: OK
      tags:
      - Social
      - Lists
  /help/tos:
    get:
      summary: Help Terms of Services
      description: Returns the Twitter Terms of Service
      operationId: returns-the-twitter-terms-of-service
      x-api-path-slug: helptos-get
      responses:
        200:
          description: OK
      tags:
      - Social
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