---
swagger: "2.0"
x-collection-name: SendGrid
x-complete: 1
info:
  title: SendGrid
  description: the-sendgrid-web-api-v3-documentation--this-is-the-entirety-of-the-documented-v3-endpoints--we-have-updated-all-the-descriptions-parameters-requests-and-responses--authentication-every-endpoint-requires-authentication-in-the-form-of-an-authorization-header-authorization-bearer-api-key
  version: 1.0.0
host: api.sendgrid.com
basePath: /v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /contactdb/lists:
    delete:
      summary: Delete Contactdb Lists
      description: |-
        **This endpoint allows you to delete multiple recipient lists.**

        The Contacts API helps you manage your [Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html) recipients.
      operationId: contactdb.lists.delete
      x-api-path-slug: contactdblists-delete
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Contactdb
      - Lists
    get:
      summary: Get Contactdb Lists
      description: |-
        **This endpoint allows you to retrieve all of your recipient lists. If you don't have any lists, an empty array will be returned.**

        The Contacts API helps you manage your [Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html) recipients.
      operationId: contactdb.lists.get
      x-api-path-slug: contactdblists-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Contactdb
      - Lists
    post:
      summary: Add Contactdb Lists
      description: |-
        **This endpoint allows you to create a list for your recipients.**

        The Contacts API helps you manage your [Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html) recipients.
      operationId: contactdb.lists.post
      x-api-path-slug: contactdblists-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Contactdb
      - Lists
  /contactdb/lists/{list_id}:
    delete:
      summary: Delete Contactdb Lists List
      description: |-
        **This endpoint allows you to delete a specific recipient list with the given ID.**

        The Contacts API helps you manage your [Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html) recipients.
      operationId: contactdb.lists.list_id.delete
      x-api-path-slug: contactdblistslist-id-delete
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: delete_contacts
        description: Adds the ability to delete all contacts on the list in addition
          to deleting the list
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Contactdb
      - Lists
      - List
    get:
      summary: Get Contactdb Lists List
      description: |-
        This endpoint allows you to retrieve a single recipient list.

        The Contacts API helps you manage your [Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html) recipients.
      operationId: contactdb.lists.list_id.get
      x-api-path-slug: contactdblistslist-id-get
      parameters:
      - in: query
        name: list_id
        description: The ID of the list to retrieve
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Contactdb
      - Lists
      - List
    patch:
      summary: Patch Contactdb Lists List
      description: |-
        **This endpoint allows you to update the name of one of your recipient lists.**


        The Contacts API helps you manage your [Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html) recipients.
      operationId: contactdb.lists.list_id.patch
      x-api-path-slug: contactdblistslist-id-patch
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: list_id
        description: The ID of the list you are updating
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Contactdb
      - Lists
      - List
  /contactdb/lists/{list_id}/recipients:
    get:
      summary: Get Contactdb Lists List  Recipients
      description: "**This endpoint allows you to retrieve all recipients on the list
        with the given ID.** \n\nThe Contacts API helps you manage your [Marketing
        Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html)
        recipients."
      operationId: contactdb.lists.list_id.recipients.get
      x-api-path-slug: contactdblistslist-idrecipients-get
      parameters:
      - in: query
        name: list_id
        description: The ID of the list whose recipients you are requesting
      - in: query
        name: No Name
      - in: query
        name: page
        description: Page index of first recipient to return (must be a positive integer)
      - in: query
        name: page_size
        description: Number of recipients to return at a time (must be a positive
          integer between 1 and 1000)
      responses:
        200:
          description: OK
      tags:
      - Email
      - Contactdb
      - Lists
      - List
      - ""
      - Recipients
    post:
      summary: Add Contactdb Lists List  Recipients
      description: |-
        **This endpoint allows you to add multiple recipients to a list.**

        Adds existing recipients to a list, passing in the recipient IDs to add. Recipient IDs should be passed exactly as they are returned from recipient endpoints.

        The Contacts API helps you manage your [Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html) recipients.
      operationId: contactdb.lists.list_id.recipients.post
      x-api-path-slug: contactdblistslist-idrecipients-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Contactdb
      - Lists
      - List
      - ""
      - Recipients
  /contactdb/lists/{list_id}/recipients/{recipient_id}:
    delete:
      summary: Delete Contactdb Lists List  Recipients Recipient
      description: |-
        **This endpoint allows you to delete a single recipient from a list.**

        The Contacts API helps you manage your [Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html) recipients.
      operationId: contactdb.lists.list_id.recipients.recipient_id.delete
      x-api-path-slug: contactdblistslist-idrecipientsrecipient-id-delete
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: list_id
        description: The ID of the list you are taking this recipient away from
      - in: query
        name: No Name
      - in: query
        name: recipient_id
        description: The ID of the recipient to take off the list
      responses:
        200:
          description: OK
      tags:
      - Email
      - Contactdb
      - Lists
      - List
      - ""
      - Recipients
      - Recipient
    post:
      summary: Add Contactdb Lists List  Recipients Recipient
      description: |-
        **This endpoint allows you to add a single recipient to a list.**

        The Contacts API helps you manage your [Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html) recipients.
      operationId: contactdb.lists.list_id.recipients.recipient_id.post
      x-api-path-slug: contactdblistslist-idrecipientsrecipient-id-post
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Contactdb
      - Lists
      - List
      - ""
      - Recipients
      - Recipient
  /contactdb/recipients/{recipient_id}/lists:
    get:
      summary: Get Contactdb Recipients Recipient  Lists
      description: |-
        **This endpoint allows you to retrieve the lists that a given recipient belongs to.**

        Each recipient can be on many lists. This endpoint gives you all of the lists that any one recipient has been added to.

        The Contacts API helps you manage your [Marketing Campaigns](https://sendgrid.com/docs/User_Guide/Marketing_Campaigns/index.html) recipients.
      operationId: contactdb.recipients.recipient_id.lists.get
      x-api-path-slug: contactdbrecipientsrecipient-idlists-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Contactdb
      - Recipients
      - Recipient
      - ""
      - Lists
---