---
swagger: "2.0"
x-collection-name: Mailgun
x-complete: 0
info:
  title: Mailgun API List
  description: Returns a single mailing list by a given address.
  version: v2
host: api.mailgun.net
basePath: v2/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  lists/:
    get:
      summary: Lists
      description: Returns a list of mailing lists under your account.
      operationId: getLists
      x-api-path-slug: lists-get
      parameters:
      - in: query
        name: access_level
        description: 'List access level, one of: readonly (default), members, everyone'
      - in: query
        name: address
        description: Find a mailing list by itu2019s address (optional)
      - in: query
        name: description
        description: Description string
      - in: query
        name: limit
        description: Maximum number of records to return (100 by default)
      - in: query
        name: namespace_id
        description: New name, e
      - in: query
        name: skip
        description: Records to skip (0 by default)
      responses:
        200:
          description: OK
      tags:
      - Lists
  lists:
    post:
      summary: Create List
      description: Creates a new mailing list.
      operationId: postLists
      x-api-path-slug: lists-post
      parameters:
      - in: query
        name: access_level
        description: 'List access level, one of: readonly (default), members, everyone'
      - in: query
        name: address
        description: A valid email address for the mailing list, e
      - in: query
        name: description
        description: A description
      - in: query
        name: name
        description: Mailing list name, e
      responses:
        200:
          description: OK
      tags:
      - List
  lists/{address}:
    delete:
      summary: Delete List
      description: Deletes a mailing list.
      operationId: deleteListsAddress
      x-api-path-slug: listsaddress-delete
      parameters:
      - in: query
        name: address
        description: Address to remove
      responses:
        200:
          description: OK
      tags:
      - List
    get:
      summary: List
      description: Returns a single mailing list by a given address.
      operationId: getListsAddress
      x-api-path-slug: listsaddress-get
      parameters:
      - in: query
        name: address
        description: Address to return for a single list
      responses:
        200:
          description: OK
      tags:
      - List
    put:
      summary: Update List
      description: Update mailing list properties, such as address, description or
        name
      operationId: putListsAddress
      x-api-path-slug: listsaddress-put
      responses:
        200:
          description: OK
      tags:
      - List
  lists/{address}/members:
    get:
      summary: Add To List
      description: Adds a member to the mailing list.
      operationId: getListsAddressMembers
      x-api-path-slug: listsaddressmembers-get
      parameters:
      - in: query
        name: address
        description: Valid email address specification, e
      - in: query
        name: Name
        description: Optional member name
      - in: query
        name: subscribed
        description: yes to add as subscribed (default), no as unsubscribed
      - in: query
        name: upsert
        description: yes to update member if present, no to raise error in case of
          a duplicate member (default)
      - in: query
        name: vars
        description: JSON-encoded dictionary string with arbitrary parameters, e
      responses:
        200:
          description: OK
      tags:
      - List
  lists/{address}/members/:
    get:
      summary: List Members
      description: Fetches the list of mailing list members.
      operationId: getListsAddressMembers
      x-api-path-slug: listsaddressmembers-get
      parameters:
      - in: query
        name: limit
        description: Maximum number of records to return (100 by default)
      - in: query
        name: skip
        description: Records to skip (0 by default)
      - in: query
        name: subscribed
        description: yes to list subscribed, no for unsubscribed, list all if not
          set
      responses:
        200:
          description: OK
      tags:
      - List
      - Members
  lists/{address}/members/{member_address}:
    get:
      summary: List Member
      description: Retrieves a mailing list member.
      operationId: getListsAddressMembersMemberAddress
      x-api-path-slug: listsaddressmembersmember-address-get
      parameters:
      - in: query
        name: address
        description: Email address of commenter
      - in: query
        name: member_address
        description: Email address on the list
      responses:
        200:
          description: OK
      tags:
      - List
      - Member
  unsubscribes/:
    post:
      summary: Add to unsubscribe list.
      description: Adds address to unsubscribed table.
      operationId: postUnsubscribes
      x-api-path-slug: unsubscribes-post
      parameters:
      - in: query
        name: address
        description: The address to add to unsubscribe list
      - in: query
        name: tag
        description: Tag to unsubscribe from, use * to unsubscribe address from domain
      responses:
        200:
          description: OK
      tags:
      - To
      - Unsubscribe
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