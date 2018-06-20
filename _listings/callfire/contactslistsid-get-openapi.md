---
swagger: "2.0"
x-collection-name: CallFire
x-complete: 0
info:
  title: Callfire Find a specific contact list
  description: Returns a single ContactList instance for a given contact list id
  termsOfService: https://www.callfire.com/legal/terms
  contact:
    name: CallFire
    url: https://www.callfire.com
    email: support@callfire.com
  version: 1.0.0
host: www.callfire.com
basePath: /v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /contacts/lists:
    get:
      summary: Find contact lists
      description: Searches for all contact lists which are available for the current
        user. Returns a paged list of contact lists
      operationId: findContactLists
      x-api-path-slug: contactslists-get
      parameters:
      - in: query
        name: fields
        description: Limit fields received in response
      - in: query
        name: limit
        description: To set the maximum number of records to return in a paged list
          response
      - in: query
        name: name
        description: A name or a partial name of a contact list
      - in: query
        name: offset
        description: Offset to the start of a given page
      responses:
        200:
          description: OK
      tags:
      - Contacts
      - Lists
    post:
      summary: Create contact lists
      description: Creates a contact list for use with campaigns using 1 of 3 inputs.
        A List of Contact objects, a list of String E.164 numbers, or a list of CallFire
        contactIds can be used as the data source for the created contact list. After
        contact list is added into the CallFire system, contact lists goes through
        seven system safeguards that check the accuracy and consistency of the data.
        For example, our system checks that contact number is formatted correctly,
        is valid, is not duplicated in another contact list, or is not added on a
        specific DNC list. You can configure to keep/merge or remove contacts which
        do not complies these rules. If contacts were not added to a contact list
        after the validation, this means the data needs to be properly formatted and
        corrected before calling this API
      operationId: createContactList
      x-api-path-slug: contactslists-post
      parameters:
      - in: body
        name: body
        description: A request object
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Contacts
      - Lists
  /contacts/lists/upload:
    post:
      summary: Create contact list from file
      description: Creates a contact list to be used with campaigns through uploading
        a .csv file. Returns the id of created list
      operationId: createContactListFromFile
      x-api-path-slug: contactslistsupload-post
      parameters:
      - in: formData
        name: file
        description: CSV file to be uploaded
      - in: formData
        name: name
        description: A name of a contact list
      - in: formData
        name: useCustomFields
        description: A flag to indicate how to define property names for contacts
      responses:
        200:
          description: OK
      tags:
      - Contacts
      - Lists
      - Upload
  /contacts/lists/{id}:
    delete:
      summary: Delete a contact list
      description: Deletes a contact list, included contacts will not be deleted.
      operationId: deleteContactList
      x-api-path-slug: contactslistsid-delete
      parameters:
      - in: path
        name: id
        description: An id of the contact list to be deleted
      responses:
        200:
          description: OK
      tags:
      - Contacts
      - Lists
    get:
      summary: Find a specific contact list
      description: Returns a single ContactList instance for a given contact list
        id
      operationId: getContactList
      x-api-path-slug: contactslistsid-get
      parameters:
      - in: query
        name: fields
        description: Limit fields received in response
      - in: path
        name: id
        description: An id of a contact list to return
      responses:
        200:
          description: OK
      tags:
      - Contacts
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