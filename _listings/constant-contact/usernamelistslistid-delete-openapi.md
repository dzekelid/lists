---
swagger: "2.0"
x-collection-name: Constant Contact
x-complete: 0
info:
  title: Constant Contact Delete Mailing List
  description: Delete Mailing List
  version: 1.0.0
host: api.constantcontact.com
basePath: /ws/customers/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /{username}/lists:
    get:
      summary: Get All Mailing Lists
      description: Get All Mailing Lists
      operationId: get-all-mailing-lists
      x-api-path-slug: usernamelists-get
      parameters:
      - in: path
        name: username
      responses:
        200:
          description: OK
      tags:
      - Mailing
      - Lists
    post:
      summary: Add Mailing List
      description: Add Mailing List
      operationId: add-mailing-list
      x-api-path-slug: usernamelists-post
      parameters:
      - in: query
        name: Content-Type
        description: Specifies Content Type
      - in: path
        name: username
      responses:
        200:
          description: OK
      tags:
      - Mailing
      - List
  /{username}/activities:
    get:
      summary: List Activities
      description: List Activities
      operationId: list-activities
      x-api-path-slug: usernameactivities-get
      parameters:
      - in: path
        name: username
      responses:
        200:
          description: OK
      tags:
      - List
      - Activities
  /{username}/campaigns:
    get:
      summary: List Campaigns
      description: List Campaigns
      operationId: list-campaigns
      x-api-path-slug: usernamecampaigns-get
      parameters:
      - in: query
        name: refresh
        description: To initiate re-calculation of campaign results, you must use
          refresh= true
      - in: path
        name: username
      responses:
        200:
          description: OK
      tags:
      - List
      - Campaigns
  /{username}/contacts:
    get:
      summary: List Contacts
      description: List Contacts
      operationId: list-contacts
      x-api-path-slug: usernamecontacts-get
      parameters:
      - in: query
        name: listid
        description: Specific list
      - in: query
        name: updatedsince
        description: Specified date
      - in: path
        name: username
      responses:
        200:
          description: OK
      tags:
      - List
      - Contacts
  /{username}/events:
    get:
      summary: List Events
      description: List Events
      operationId: list-events
      x-api-path-slug: usernameevents-get
      parameters:
      - in: path
        name: username
      responses:
        200:
          description: OK
      tags:
      - List
      - Events
  /{username}/events/{event-id}/registrants:
    get:
      summary: List Registrants
      description: List Registrants
      operationId: list-registrants
      x-api-path-slug: usernameeventseventidregistrants-get
      parameters:
      - in: path
        name: event-id
      - in: path
        name: username
      responses:
        200:
          description: OK
      tags:
      - List
      - Registrants
  /{username}/events/{event-id}/registrants/{registrant-id}/guests:
    get:
      summary: Get List of Guests
      description: Get List of Guests
      operationId: get-list-of-guests
      x-api-path-slug: usernameeventseventidregistrantsregistrantidguests-get
      parameters:
      - in: path
        name: event-id
      - in: path
        name: registrant-id
      - in: path
        name: username
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Guests
  /{username}/library/folders:
    get:
      summary: List Folders
      description: List Folders
      operationId: list-folders
      x-api-path-slug: usernamelibraryfolders-get
      parameters:
      - in: query
        name: Accept
        description: Specifies Accept
      - in: query
        name: Content-Type
        description: Specifies Content Type
      - in: path
        name: username
      responses:
        200:
          description: OK
      tags:
      - List
      - Folders
  /{username}/library/folders/{folder-id}/images:
    get:
      summary: List Images
      description: List Images
      operationId: list-images
      x-api-path-slug: usernamelibraryfoldersfolderidimages-get
      parameters:
      - in: query
        name: Accept
        description: Specifies Accept
      - in: query
        name: Content-Type
        description: Specifies Content Type
      - in: path
        name: folder-id
      - in: path
        name: username
      responses:
        200:
          description: OK
      tags:
      - List
      - Images
  /{username}/lists/{list-id}:
    delete:
      summary: Delete Mailing List
      description: Delete Mailing List
      operationId: delete-mailing-list
      x-api-path-slug: usernamelistslistid-delete
      parameters:
      - in: path
        name: list-id
      - in: path
        name: username
      responses:
        200:
          description: OK
      tags:
      - Mailing
      - List
    get:
      summary: Get Mailing List
      description: Get Mailing List
      operationId: get-mailing-list
      x-api-path-slug: usernamelistslistid-get
      parameters:
      - in: path
        name: list-id
      - in: path
        name: username
      responses:
        200:
          description: OK
      tags:
      - Mailing
      - List
    put:
      summary: Update Mailing List
      description: Update Mailing List
      operationId: update-mailing-list
      x-api-path-slug: usernamelistslistid-put
      parameters:
      - in: query
        name: Content-Type
        description: Specifies Content Type
      - in: path
        name: list-id
      - in: path
        name: username
      responses:
        200:
          description: OK
      tags:
      - Mailing
      - List
  /{username}/lists/{list-id}/members:
    get:
      summary: Get Contacts Collection from a List
      description: Get Contacts Collection from a List
      operationId: get-contacts-collection-from-a-list
      x-api-path-slug: usernamelistslistidmembers-get
      parameters:
      - in: path
        name: list-id
      - in: path
        name: username
      responses:
        200:
          description: OK
      tags:
      - Contacts
      - Collection
      - From
      - List
  /{username}/settings/emailaddresses:
    get:
      summary: List Account Email Addresses
      description: List Account Email Addresses
      operationId: list-account-email-addresses
      x-api-path-slug: usernamesettingsemailaddresses-get
      parameters:
      - in: path
        name: username
      responses:
        200:
          description: OK
      tags:
      - List
      - Account
      - Email
      - Resses
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