---
swagger: "2.0"
x-collection-name: Elastic Email
x-complete: 1
info:
  title: Elastic Email SMTP API
  description: api-for-sending-and-management-email-
  version: v1
host: api.elasticemail.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  lists/add-contact:
    get:
      summary: Add Existing Subscriber To List
      description: Add Existing Subscriber To List
      operationId: getListsAddContact
      x-api-path-slug: listsaddcontact-get
      parameters:
      - in: query
        name: api_key
        description: Your API Key
      - in: query
        name: listname
        description: name of list you wish to add subscriber to (separate by semi-colon
          to add to multiple lists)
      - in: query
        name: username
        description: Your user name
      responses:
        200:
          description: OK
      tags:
      - Lists
      - Add
      - Contact
  lists/create-contact:
    get:
      summary: Create New Subscriber
      description: Create New Subscriber
      operationId: getListsCreateContact
      x-api-path-slug: listscreatecontact-get
      parameters:
      - in: query
        name: api_key
        description: your api key found on the Account screen
      - in: query
        name: birthdate
        description: date of birth of the subscriber
      - in: query
        name: city
        description: city of the subscriber
      - in: query
        name: country
        description: country of the subscriber
      - in: query
        name: email
        description: email address of subscriber/recipient
      - in: query
        name: firstname
        description: first name of the subscriber
      - in: query
        name: gender
        description: male or female
      - in: query
        name: lastname
        description: last name of the subscriber
      - in: query
        name: listname
        description: the name of the list or lists (separated by semi-colon) the subscriber
          will be added to - if blank, it will just create the subscriber
      - in: query
        name: organizationname
        description: organization name the subscriber works for
      - in: query
        name: phone
        description: phone number for the subscriber
      - in: query
        name: postalcode
        description: the zip or postal code of the subscriber
      - in: query
        name: state
        description: the state or province for the subscriber
      - in: query
        name: the zip or postal code of the subscriber
        description: Your user name
      - in: query
        name: title
        description: the title for the subscriber (Mr
      responses:
        200:
          description: OK
      tags:
      - Lists
      - Create
      - Contact
  lists/create-lists:
    get:
      summary: Create New List
      description: Create New List
      operationId: getListsCreateLists
      x-api-path-slug: listscreatelists-get
      parameters:
      - in: query
        name: api_key
        description: Your API Key
      - in: query
        name: listname
        description: name of list you wish to create
      - in: query
        name: username
        description: Your user name
      responses:
        200:
          description: OK
      tags:
      - Lists
      - Create
      - Lists
  lists/delete:
    get:
      summary: Delete Existing List
      description: Delete Existing List
      operationId: getListsDelete
      x-api-path-slug: listsdelete-get
      parameters:
      - in: query
        name: api_key
        description: Your API Key
      - in: query
        name: listname
        description: name of list you wish to delete
      - in: query
        name: username
        description: Your user name
      responses:
        200:
          description: OK
      tags:
      - Lists
      - Delete
  lists/delete-contact:
    get:
      summary: Delete Existing Subscriber
      description: Delete Existing Subscriber
      operationId: getListsDeleteContact
      x-api-path-slug: listsdeletecontact-get
      parameters:
      - in: query
        name: api_key
        description: Your API Key
      - in: query
        name: email
        description: email address of subscriber/recipient (separate by semi-colon
          to remove multiple)
      - in: query
        name: username
        description: Your user name
      responses:
        200:
          description: OK
      tags:
      - Lists
      - Delete
      - Contact
  lists/remove-contact:
    get:
      summary: Remove Existing Subscriber From List
      description: Remove Existing Subscriber From List
      operationId: getListsRemoveContact
      x-api-path-slug: listsremovecontact-get
      parameters:
      - in: query
        name: api_key
        description: Your API Key
      - in: query
        name: listname
        description: name of list you wish to remove subscriber from (separate by
          semi-colon to remove from multiple lists)
      - in: query
        name: username
        description: Your user name
      responses:
        200:
          description: OK
      tags:
      - Lists
      - Remove
      - Contact
  lists/upload-contacts:
    get:
      summary: Create Multiple Subscriber From CSV File
      description: Create Multiple Subscriber From CSV File
      operationId: getListsUploadContacts
      x-api-path-slug: listsuploadcontacts-get
      parameters:
      - in: query
        name: api_key
        description: Your API Key
      - in: query
        name: birthdate
        description: date of birth of the subscriber
      - in: query
        name: city
        description: city of the subscriber
      - in: query
        name: country
        description: country of the subscriber
      - in: query
        name: email
        description: email address of subscriber/recipient
      - in: query
        name: firstname
        description: first name of the subscriber
      - in: query
        name: gender
        description: male or female
      - in: query
        name: lastname
        description: last name of the subscriber
      - in: query
        name: listname
        description: the name of the list or lists (separated by semi-colon) the subscriber
          will be added to - if blank, it will just create the subscriber
      - in: query
        name: organizationname
        description: organization name the subscriber works for
      - in: query
        name: phone
        description: phone number for the subscriber
      - in: query
        name: postalcode
        description: the zip or postal code of the subscriber
      - in: query
        name: state
        description: the state or province for the subscriber
      - in: query
        name: title
        description: the title for the subscriber (Mr
      - in: query
        name: username
        description: Your user name
      responses:
        200:
          description: OK
      tags:
      - Lists
      - Upload
      - Contacts
  mailer/lists/unsubscribed:
    get:
      summary: Unsubscribed
      description: This api will return you the list of email addresses which are
        currently in your block list.
      operationId: getMailerListsUnsubscribed
      x-api-path-slug: mailerlistsunsubscribed-get
      parameters:
      - in: query
        name: api_key
        description: Your API Key
      - in: query
        name: username
        description: Your user name
      responses:
        200:
          description: OK
      tags:
      - Mailer
      - Lists
      - Unsubscribed
---