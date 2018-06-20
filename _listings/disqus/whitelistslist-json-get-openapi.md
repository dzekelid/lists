---
swagger: "2.0"
x-collection-name: Disqus
x-complete: 0
info:
  title: Disqus Whitelists List
  description: Whitelists List
  termsOfService: https://docs.disqus.com/kb/terms-and-policies/
  version: 1.0.0
host: disqus.com
basePath: api/3.0/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /blacklists/backfillCounters.json:
    post:
      summary: Blacklists BackfillCounters
      description: Blacklists BackfillCounters
      operationId: blacklists-backfillcounters
      x-api-path-slug: blacklistsbackfillcounters-json-post
      responses:
        200:
          description: OK
      tags:
      - Comments
      - Black Lists
  /blacklists/list.json:
    get:
      summary: Blacklists List
      description: Blacklists List
      operationId: blacklists-list
      x-api-path-slug: blacklistslist-json-get
      parameters:
      - in: query
        name: cursor
        description: Defaults to null
        type: string
      - in: query
        name: forum
        description: Looks up a forum by ID (aka short name)
        type: string
      - in: query
        name: limit
        description: Defaults to 25                         Maximum value of 100
        type: string
      - in: query
        name: order
        description: 'Defaults to asc                         Choices: asc, desc'
        type: string
      - in: query
        name: query
        description: Defaults to null
        type: string
      - in: query
        name: related
        description: Defaults to []                         You may specify relations
          to include with your response
        type: string
      - in: query
        name: since
        description: Defaults to null                         Unix timestamp (or ISO
          datetime standard)
        type: string
      - in: query
        name: since_id
        description: Defaults to null
        type: string
      - in: query
        name: type
        description: 'Defaults to null                         Choices: domain, word,
          ip, user, thread_slug, email'
        type: string
      responses:
        200:
          description: OK
      tags:
      - Comments
      - Black Lists
  /blacklists/remove.json:
    post:
      summary: Blacklists Remove
      description: Blacklists Remove
      operationId: blacklists-remove
      x-api-path-slug: blacklistsremove-json-post
      parameters:
      - in: query
        name: domain
        description: Defaults to []                         Domain Name
        type: string
      - in: query
        name: email
        description: Defaults to []                         Email address (defined
          by RFC 5322)
        type: string
      - in: query
        name: forum
        description: Looks up a forum by ID (aka short name)
        type: string
      - in: query
        name: ip
        description: Defaults to []                         IP address in CIDR notation
        type: string
      - in: query
        name: user
        description: Defaults to []                         Looks up a user by ID
          You may look up a user by username using the &#39;username&#39; query type
        type: string
      - in: query
        name: word
        description: Defaults to []                         Maximum length of 200
        type: string
      responses:
        200:
          description: OK
      tags:
      - Comments
      - Black Lists
  /forums/listCategories.json:
    get:
      summary: Forums ListCategories
      description: Forums ListCategories
      operationId: forums-listcategories
      x-api-path-slug: forumslistcategories-json-get
      parameters:
      - in: query
        name: cursor
        description: Defaults to null
        type: string
      - in: query
        name: forum
        description: Looks up a forum by ID (aka short name)
        type: string
      - in: query
        name: limit
        description: Defaults to 25                         Maximum value of 100
        type: string
      - in: query
        name: order
        description: 'Defaults to asc                         Choices: asc, desc'
        type: string
      - in: query
        name: since_id
        description: Defaults to null
        type: string
      responses:
        200:
          description: OK
      tags:
      - Comments
      - Lists
      - Categories
  /forums/listFollowers.json:
    get:
      summary: Forums ListFollowers
      description: Forums ListFollowers
      operationId: forums-listfollowers
      x-api-path-slug: forumslistfollowers-json-get
      parameters:
      - in: query
        name: cursor
        description: Defaults to null
        type: string
      - in: query
        name: forum
        description: Looks up a forum by ID (aka short name)
        type: string
      - in: query
        name: limit
        description: Defaults to 25                         Maximum value of 100
        type: string
      - in: query
        name: order
        description: 'Defaults to asc                         Choices: asc, desc'
        type: string
      - in: query
        name: since_id
        description: Defaults to null
        type: string
      responses:
        200:
          description: OK
      tags:
      - Comments
      - Lists
  /forums/listModerators.json:
    get:
      summary: Forums ListModerators
      description: Forums ListModerators
      operationId: forums-listmoderators
      x-api-path-slug: forumslistmoderators-json-get
      parameters:
      - in: query
        name: forum
        description: Looks up a forum by ID (aka short name)
        type: string
      responses:
        200:
          description: OK
      tags:
      - Comments
      - Lists
  /forums/listMostActiveUsers.json:
    get:
      summary: Forums ListMostActiveUsers
      description: Forums ListMostActiveUsers
      operationId: forums-listmostactiveusers
      x-api-path-slug: forumslistmostactiveusers-json-get
      parameters:
      - in: query
        name: cursor
        description: Defaults to null
        type: string
      - in: query
        name: forum
        description: Looks up a forum by ID (aka short name)
        type: string
      - in: query
        name: limit
        description: Defaults to 25                         Maximum value of 100
        type: string
      - in: query
        name: order
        description: 'Defaults to asc                         Choices: desc'
        type: string
      responses:
        200:
          description: OK
      tags:
      - Comments
      - Lists
  /forums/listMostLikedUsers.json:
    get:
      summary: Forums ListMostLikedUsers
      description: Forums ListMostLikedUsers
      operationId: forums-listmostlikedusers
      x-api-path-slug: forumslistmostlikedusers-json-get
      parameters:
      - in: query
        name: cursor
        description: Defaults to null
        type: string
      - in: query
        name: forum
        description: Looks up a forum by ID (aka short name)
        type: string
      - in: query
        name: limit
        description: Defaults to 25                         Maximum value of 100
        type: string
      - in: query
        name: order
        description: 'Defaults to asc                         Choices: desc'
        type: string
      responses:
        200:
          description: OK
      tags:
      - Comments
      - Lists
  /forums/listPosts.json:
    get:
      summary: Forums ListPosts
      description: Forums ListPosts
      operationId: forums-listposts
      x-api-path-slug: forumslistposts-json-get
      parameters:
      - in: query
        name: cursor
        description: Defaults to null
        type: string
      - in: query
        name: filters
        description: 'Defaults to []                         Valid values are: 1:
          Is_Anonymous 2: Has_Link 3: Has_Low_Rep_Author 4: Has_Bad_Word 5: Is_Flagged
          6: No_Issue 7: Is_Toxic'
        type: string
      - in: query
        name: forum
        description: Looks up a forum by ID (aka short name)
        type: string
      - in: query
        name: include
        description: 'Defaults to [  approved]                         Choices: unapproved,
          approved, spam, deleted, flagged, highlighted'
        type: string
      - in: query
        name: limit
        description: Defaults to 25                         Maximum number of posts
          to return
        type: string
      - in: query
        name: order
        description: 'Defaults to desc                         Choices: asc, desc'
        type: string
      - in: query
        name: query
        description: Defaults to null
        type: string
      - in: query
        name: related
        description: Defaults to []                         You may specify relations
          to include with your response
        type: string
      - in: query
        name: since
        description: Defaults to null                         Unix timestamp (or ISO
          datetime standard)
        type: string
      responses:
        200:
          description: OK
      tags:
      - Comments
      - Lists
  /forums/listThreads.json:
    get:
      summary: Forums ListThreads
      description: Forums ListThreads
      operationId: forums-listthreads
      x-api-path-slug: forumslistthreads-json-get
      parameters:
      - in: query
        name: cursor
        description: Defaults to null
        type: string
      - in: query
        name: forum
        description: Looks up a forum by ID (aka short name)
        type: string
      - in: query
        name: include
        description: 'Defaults to [  open,  closed]                         Choices:
          open, closed, killed'
        type: string
      - in: query
        name: limit
        description: Defaults to 25                         Maximum value of 100
        type: string
      - in: query
        name: order
        description: 'Defaults to desc                         Choices: asc, desc'
        type: string
      - in: query
        name: related
        description: Defaults to []                         You may specify relations
          to include with your response
        type: string
      - in: query
        name: since
        description: Defaults to null                         Unix timestamp (or ISO
          datetime standard)
        type: string
      - in: query
        name: thread
        description: Defaults to null                         Looks up a thread by
          ID You may pass us the &#39;ident&#39; query type instead of an ID by including
          &#39;forum&#39;
        type: string
      responses:
        200:
          description: OK
      tags:
      - Comments
      - Forums
      - Lists
  /forums/listUserModerationHistory.json:
    get:
      summary: Forums ListUserModerationHistory
      description: Forums ListUserModerationHistory
      operationId: forums-listusermoderationhistory
      x-api-path-slug: forumslistusermoderationhistory-json-get
      parameters:
      - in: query
        name: cursor
        description: Defaults to null
        type: string
      - in: query
        name: forum
        description: Looks up a forum by ID (aka short name)
        type: string
      - in: query
        name: limit
        description: Defaults to 20
        type: string
      - in: query
        name: user
        description: Looks up a user by ID You may look up a user by username using
          the &#39;username&#39; query type
        type: string
      responses:
        200:
          description: OK
      tags:
      - Comments
      - Forums
      - Lists
  /forums/listUsers.json:
    get:
      summary: Forums ListUsers
      description: Forums ListUsers
      operationId: forums-listusers
      x-api-path-slug: forumslistusers-json-get
      parameters:
      - in: query
        name: cursor
        description: Defaults to null
        type: string
      - in: query
        name: forum
        description: Looks up a forum by ID (aka short name)
        type: string
      - in: query
        name: limit
        description: Defaults to 25                         Maximum value of 100
        type: string
      - in: query
        name: order
        description: 'Defaults to asc                         Choices: asc, desc'
        type: string
      - in: query
        name: since_id
        description: Defaults to null
        type: string
      responses:
        200:
          description: OK
      tags:
      - Comments
      - Forums
      - Lists
      - Users
  /imports/list.json:
    get:
      summary: Imports List
      description: Imports List
      operationId: imports-list
      x-api-path-slug: importslist-json-get
      parameters:
      - in: query
        name: cursor
        description: Defaults to null
        type: string
      - in: query
        name: forum
        description: Looks up a forum by ID (aka short name)
        type: string
      responses:
        200:
          description: OK
      tags:
      - Comments
      - Import
      - Lists
  /whitelists/list.json:
    get:
      summary: Whitelists List
      description: Whitelists List
      operationId: whitelists-list
      x-api-path-slug: whitelistslist-json-get
      parameters:
      - in: query
        name: cursor
        description: Defaults to null
        type: string
      - in: query
        name: forum
        description: Looks up a forum by ID (aka short name)
        type: string
      - in: query
        name: limit
        description: Defaults to 25                         Maximum value of 100
        type: string
      - in: query
        name: order
        description: 'Defaults to asc                         Choices: asc, desc'
        type: string
      - in: query
        name: query
        description: Defaults to null
        type: string
      - in: query
        name: related
        description: Defaults to []                         You may specify relations
          to include with your response
        type: string
      - in: query
        name: since
        description: Defaults to null                         Unix timestamp (or ISO
          datetime standard)
        type: string
      - in: query
        name: since_id
        description: Defaults to null
        type: string
      - in: query
        name: type
        description: 'Defaults to null                         Choices: email, user'
        type: string
      responses:
        200:
          description: OK
      tags:
      - Comments
      - White Lists
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