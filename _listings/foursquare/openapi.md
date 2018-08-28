swagger: "2.0"
x-collection-name: Foursquare
x-complete: 1
info:
  title: Foursquare
  version: 1.0.0
host: api.foursquare.com
basePath: /v2/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /lists/add:
    post:
      summary: Post Lists Add
      description: /lists/{LIST_ID}
      operationId: listslist-id
      x-api-path-slug: listsadd-post
      parameters:
      - in: query
        name: collaborative
        description: Indicating if this list can be edited by friends
      - in: query
        name: description
        description: The description of the list
      - in: query
        name: name
        description: The name of the list
      - in: query
        name: photoId
        description: The id of a photo that should be set as the list photo
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Lists
  /lists/{LIST_ID}:
    get:
      summary: Get Lists
      description: /tips/{TIP_ID}/unmark
      operationId: tipstip-idunmark
      x-api-path-slug: listslist-id-get
      parameters:
      - in: query
        name: limit
        description: Number of results to return, up to 200
      - in: query
        name: LIST_ID
        description: id for a user-created (e
      - in: path
        name: LIST_ID
      - in: query
        name: offset
        description: The number of results to skip
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Lists
  /lists/{LIST_ID}/additem:
    post:
      summary: Post Lists Additem
      description: /lists/{LIST_ID}/suggestvenues
      operationId: listslist-idsuggestvenues
      x-api-path-slug: listslist-idadditem-post
      parameters:
      - in: query
        name: itemId
        description: Used in conjuction with listId, the id of an item on that list
          that we wish to copy to this list
      - in: query
        name: listId
        description: Used in conjuction with itemId, the id for a user created or
          followed list as well as one of USER_ID/tips, USER_ID/todos, or USER_ID/dones
      - in: query
        name: LIST_ID
        description: Id for a user-created or followed list as well as one of USER_ID/tips,
          USER_ID/todos, or USER_ID/dones
      - in: path
        name: LIST_ID
      - in: query
        name: text
        description: If the target is a user-created list, this will create a public
          tip on the venue
      - in: query
        name: tipId
        description: Used to add a tip to a list
      - in: query
        name: url
        description: If adding a new tip via text, this can associate a url with the
          tip
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      - in: query
        name: venueId
        description: A venue to add to the list
      responses:
        200:
          description: OK
      tags:
      - Lists
      - Item
  /lists/{LIST_ID}/deleteitem:
    post:
      summary: Post Lists Deleteitem
      description: /lists/{LIST_ID}/additem
      operationId: listslist-idadditem
      x-api-path-slug: listslist-iddeleteitem-post
      parameters:
      - in: query
        name: itemId
        description: Id of the item to delete
      - in: query
        name: LIST_ID
        description: Id for a user-created or followed list or one of USER_ID/tips,
          USER_ID/todos, or USER_ID/dones
      - in: path
        name: LIST_ID
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Lists
      - Item
  /lists/{LIST_ID}/follow:
    post:
      summary: Post Lists Follow
      description: /lists/{LIST_ID}/deleteitem
      operationId: listslist-iddeleteitem
      x-api-path-slug: listslist-idfollow-post
      parameters:
      - in: query
        name: LIST_ID
        description: Id of a user-created list
      - in: path
        name: LIST_ID
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Lists
      - Follow
  /lists/{LIST_ID}/followers:
    get:
      summary: Get Lists Followers
      description: /lists/add
      operationId: listsadd
      x-api-path-slug: listslist-idfollowers-get
      parameters:
      - in: query
        name: LIST_ID
        description: Id for a user-created list
      - in: path
        name: LIST_ID
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Lists
      - Followers
  /lists/{LIST_ID}/moveitem:
    post:
      summary: Post Lists Moveitem
      description: /lists/{LIST_ID}/follow
      operationId: listslist-idfollow
      x-api-path-slug: listslist-idmoveitem-post
      parameters:
      - in: query
        name: afterId
        description: Move itemId after afterId
      - in: query
        name: beforeId
        description: Move itemId before beforeId
      - in: query
        name: itemId
        description: Id of the item on this list to move
      - in: query
        name: LIST_ID
        description: Id for a user-created or followed list or one of USER_ID/tips,
          USER_ID/todos, or USER_ID/dones
      - in: path
        name: LIST_ID
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Lists
      - Moveitem
  /lists/{LIST_ID}/share:
    post:
      summary: Post Lists Share
      description: /lists/{LIST_ID}/moveitem
      operationId: listslist-idmoveitem
      x-api-path-slug: listslist-idshare-post
      parameters:
      - in: query
        name: broadcast
        description: Where to broadcast this list
      - in: query
        name: LIST_ID
        description: Id for a user-created list
      - in: path
        name: LIST_ID
      - in: query
        name: message
        description: A personal note to include with the share
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Lists
      - Share
  /lists/{LIST_ID}/suggestphoto:
    get:
      summary: Get Lists Suggestphoto
      description: /lists/{LIST_ID}/followers
      operationId: listslist-idfollowers
      x-api-path-slug: listslist-idsuggestphoto-get
      parameters:
      - in: query
        name: itemId
        description: Id of item on this list
      - in: query
        name: LIST_ID
        description: Id for a user-created list
      - in: path
        name: LIST_ID
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Lists
      - Suggestphoto
  /lists/{LIST_ID}/suggesttip:
    get:
      summary: Get Lists Suggesttip
      description: /lists/{LIST_ID}/suggestphoto
      operationId: listslist-idsuggestphoto
      x-api-path-slug: listslist-idsuggesttip-get
      parameters:
      - in: query
        name: itemId
        description: Id of item on this list
      - in: query
        name: LIST_ID
        description: Id for a user-created list
      - in: path
        name: LIST_ID
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Lists
      - Suggesttip
  /lists/{LIST_ID}/suggestvenues:
    get:
      summary: Get Lists Suggestvenues
      description: /lists/{LIST_ID}/suggesttip
      operationId: listslist-idsuggesttip
      x-api-path-slug: listslist-idsuggestvenues-get
      parameters:
      - in: query
        name: LIST_ID
        description: Id for a user-created list
      - in: path
        name: LIST_ID
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Lists
      - Suggestvenues
  /lists/{LIST_ID}/unfollow:
    post:
      summary: Post Lists Unfollow
      description: /lists/{LIST_ID}/share
      operationId: listslist-idshare
      x-api-path-slug: listslist-idunfollow-post
      parameters:
      - in: query
        name: LIST_ID
        description: Id of a user-created list
      - in: path
        name: LIST_ID
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Lists
      - Unfollow
  /lists/{LIST_ID}/update:
    post:
      summary: Post Lists Update
      description: /lists/{LIST_ID}/unfollow
      operationId: listslist-idunfollow
      x-api-path-slug: listslist-idupdate-post
      parameters:
      - in: query
        name: collaborative
        description: Indicating if this list can be edited by friends
      - in: query
        name: description
        description: If present and a non-empty value, updates the List description
      - in: query
        name: LIST_ID
        description: Id for a user-created list
      - in: path
        name: LIST_ID
      - in: query
        name: name
        description: If present and a non-empty value, updates the List name
      - in: query
        name: photoId
        description: If present and a non-empty value, updates the List photo
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Lists
  /lists/{LIST_ID}/updateitem:
    post:
      summary: Post Lists Updateitem
      description: /lists/{LIST_ID}/update
      operationId: listslist-idupdate
      x-api-path-slug: listslist-idupdateitem-post
      parameters:
      - in: query
        name: itemId
        description: The id of an item on this list
      - in: query
        name: LIST_ID
        description: Id for a user-created list
      - in: path
        name: LIST_ID
      - in: query
        name: photoId
        description: If present and a non-empty value, adds a photo to this item
      - in: query
        name: text
        description: If present creates a public tip on the venue and replaces any
          existing tip on the item
      - in: query
        name: tipId
        description: If present and a non-empty value, adds or replaces a tip on this
          item
      - in: query
        name: url
        description: If adding a new tip via text, this can associate a url with the
          tip
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Lists
      - Item
  /users/{USER_ID}/lists:
    get:
      summary: Get Users Lists
      description: /users/{USER_ID}/friends
      operationId: usersuser-idfriends
      x-api-path-slug: usersuser-idlists-get
      parameters:
      - in: query
        name: group
        description: Can be created (lists created by this user), edited (other peoples
          lists this user has edited), followed (lists this user follows), friends
          (lists from this users friends), and suggested (lists relevant to the users
          current location)
      - in: query
        name: ll
        description: Location of the user, required in order to receive the suggested
          group
      - in: query
        name: USER_ID
        description: Identity of the user to get lists for
      - in: path
        name: USER_ID
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Users
      - Lists
  /campaigns/list:
    get:
      summary: Get Campaigns List
      description: /campaigns/add
      operationId: campaignsadd
      x-api-path-slug: campaignslist-get
      parameters:
      - in: query
        name: groupId
        description: If specified, limits response to campaigns involving the given
          group
      - in: query
        name: specialId
        description: If specified, limits response to campaigns involving the given
          special
      - in: query
        name: status
        description: 'Which campaigns to return: pending, active, expired, all (default=all)'
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Campaigns
      - List
  /specials/list:
    get:
      summary: Get Specials List
      description: /specials/add
      operationId: specialsadd
      x-api-path-slug: specialslist-get
      parameters:
      - in: query
        name: status
        description: 'Which specials to return: pending, active, expired, all'
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      - in: query
        name: venueId
        description: Comma-separated list of venue IDs; filters results to the specials
          assigned to the venue(s)
      responses:
        200:
          description: OK
      tags:
      - Specials
      - List
  /venuegroups/list:
    get:
      summary: Get Venuegroups List
      description: /venuegroups/{GROUP_ID}/delete
      operationId: venuegroupsgroup-iddelete
      x-api-path-slug: venuegroupslist-get
      parameters:
      - in: query
        name: v
        description: All requests now accept a v=YYYYMMDD param, which indicates that
          the client is up to date as of the specified date
      responses:
        200:
          description: OK
      tags:
      - Venuegroups
      - List