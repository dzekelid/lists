---
swagger: "2.0"
x-collection-name: Eventbrite
x-complete: 0
info:
  title: Eventbrite Delete Users Contact Lists Contact List
  description: 'Deletes the contact list. Returns {&quot;deleted&quot;: true}.'
  version: 1.0.0
host: www.eventbrite.com
basePath: /%7Bdata-type%7D/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /users/{id}/contact_lists/:
    get:
      summary: Get Users Contact Lists
      description: |-
        Returns a list of contact_list that the user owns as the key
        contact_lists.
      operationId: getUsersContactLists
      x-api-path-slug: usersidcontact-lists-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Contact
      - Lists
    post:
      summary: Post Users Contact Lists
      description: |-
        Makes a new contact_list for the user and returns it as
        contact_list.
      operationId: postUsersContactLists
      x-api-path-slug: usersidcontact-lists-post
      parameters:
      - in: query
        name: contact_list.name
        description: Name of the new contact list
        type: query
      responses:
        200:
          description: OK
      tags:
      - Users
      - Contact
      - Lists
  /users/{id}/contact_lists/:contact_list_id/:
    get:
      summary: Get Users Contact Lists Contact List
      description: Gets a user&#8217;s contact_list by ID as contact_list.
      operationId: getUsersContactListsContactList
      x-api-path-slug: usersidcontact-listscontact-list-id-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Contact
      - Lists
      - :contact
      - List
    post:
      summary: Post Users Contact Lists Contact List
      description: Updates the contact_list and returns it as contact_list.
      operationId: postUsersContactListsContactList
      x-api-path-slug: usersidcontact-listscontact-list-id-post
      parameters:
      - in: query
        name: contact_list.name
        description: New name of the contact list
        type: query
      responses:
        200:
          description: OK
      tags:
      - Users
      - Contact
      - Lists
      - :contact
      - List
    delete:
      summary: Delete Users Contact Lists Contact List
      description: 'Deletes the contact list. Returns {&quot;deleted&quot;: true}.'
      operationId: deleteUsersContactListsContactList
      x-api-path-slug: usersidcontact-listscontact-list-id-delete
      responses:
        200:
          description: OK
      tags:
      - Users
      - Contact
      - Lists
      - :contact
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