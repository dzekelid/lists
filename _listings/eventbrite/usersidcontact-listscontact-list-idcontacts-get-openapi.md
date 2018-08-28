---
swagger: "2.0"
x-collection-name: Eventbrite
x-complete: 0
info:
  title: Eventbrite Get Users Contact Lists Contact List Contacts
  description: |-
    Returns the contacts on the contact list
    as contacts.
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
  /users/{id}/contact_lists/:contact_list_id/contacts/:
    get:
      summary: Get Users Contact Lists Contact List Contacts
      description: |-
        Returns the contacts on the contact list
        as contacts.
      operationId: getUsersContactListsContactListContacts
      x-api-path-slug: usersidcontact-listscontact-list-idcontacts-get
      responses:
        200:
          description: OK
      tags:
      - Users
      - Contact
      - Lists
      - :contact
      - List
      - Contacts
    post:
      summary: Post Users Contact Lists Contact List Contacts
      description: 'Adds a new contact to the contact list. Returns {&quot;created&quot;:
        true}.'
      operationId: postUsersContactListsContactListContacts
      x-api-path-slug: usersidcontact-listscontact-list-idcontacts-post
      parameters:
      - in: query
        name: contact.email
        description: Contact&#8217;s email address
        type: query
      - in: query
        name: contact.first_name
        description: Contact&#8217;s first name (or full name)
        type: query
      - in: query
        name: contact.last_name
        description: Contact&#8217;s last name
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
      - Contacts
    delete:
      summary: Delete Users Contact Lists Contact List Contacts
      description: |-
        Deletes the specified contact from the contact list.
        Returns {&quot;deleted&quot;: true}.
      operationId: deleteUsersContactListsContactListContacts
      x-api-path-slug: usersidcontact-listscontact-list-idcontacts-delete
      parameters:
      - in: query
        name: email
        description: Email address to remove
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
      - Contacts
  /user_list_events:
    get:
      summary: Get User List Events
      description: This method lists the events created by this user. Only public
        events are returned if no authentication is passed.
      operationId: Get_user_list_events_
      x-api-path-slug: user-list-events-get
      parameters:
      - in: query
        name: asc_or_desc
        description: Valid options include ???asc??? or results in ascending order
          or ???desc??? or descending order based on event start_date
      - in: query
        name: data-type
        description: xml or json data-types are supported
      - in: query
        name: do_not_display
        description: Comma separated list without spaces
      - in: query
        name: email
        description: The user email
      - in: query
        name: event_statuses
        description: Comma separated list without spaces
      responses:
        200:
          description: OK
      tags:
      - User
      - List
      - Events
  /event_list_attendees:
    get:
      summary: Get Event List Attendees
      description: This method returns a list of attendees for a given event. If no
        authentication is passed, only publicly available attendee records will be
        returned.
      operationId: Get_event_list_attendees_
      x-api-path-slug: event-list-attendees-get
      parameters:
      - in: query
        name: count
        description: Limit the number of attendees returned
      - in: query
        name: data-type
        description: xml or json data-types are supported
      - in: query
        name: do_not_display
        description: Comma separated list without spaces that leaves out certain data
          returned
      - in: query
        name: event_id
        description: The ID of the event
      - in: query
        name: page
        description: Allows for paging through the results of a query
      - in: query
        name: show_full_barcodes
        description: If set to ???true???, it will return all barcodes associates
          with the attendee, plus the barcode status, device used, attendee_id, and
          barcode number
      responses:
        200:
          description: OK
      tags:
      - Event
      - List
      - Attendees
  /user_list_venues:
    get:
      summary: Get User List Venues
      description: This method lists the venues created by this user. Requires authentication.
      operationId: Get_user_list_venues_
      x-api-path-slug: user-list-venues-get
      parameters:
      - in: query
        name: data-type
        description: xml or json data-types are supported
      responses:
        200:
          description: OK
      tags:
      - User
      - List
      - Venues
  /organizer_list_events:
    get:
      summary: Get Organizer List Events
      description: This method returns a list of events for a given organizer.
      operationId: Get_organizer_list_events_
      x-api-path-slug: organizer-list-events-get
      parameters:
      - in: query
        name: data-type
        description: xml or json data-types are supported
      - in: query
        name: id
        description: The organizer id
      responses:
        200:
          description: OK
      tags:
      - Organizer
      - List
      - Events
  /user_list_organizers:
    get:
      summary: Get User List Organizers
      description: This method lists the organizers created by this user. Requires
        authentication.
      operationId: Get_user_list_organizers_
      x-api-path-slug: user-list-organizers-get
      parameters:
      - in: query
        name: data-type
        description: xml or json data-types are supported
      responses:
        200:
          description: OK
      tags:
      - User
      - List
      - Organizers
  /user_list_tickets:
    get:
      summary: Get User List Tickets
      description: This method lists the tickets purchased by the authenticated user.
        Each transaction is an order in our system and an order may contain one or
        more tickets. Tickets to free events are included.
      operationId: Get_user_list_tickets_
      x-api-path-slug: user-list-tickets-get
      parameters:
      - in: query
        name: data-type
        description: xml or json data-types are supported
      responses:
        200:
          description: OK
      tags:
      - User
      - List
      - Tickets
  /event_list_discounts:
    get:
      summary: Get Event List Discounts
      description: This method returns a list of discounts for a given event.
      operationId: Get_event_list_discounts_
      x-api-path-slug: event-list-discounts-get
      parameters:
      - in: query
        name: data-type
        description: xml or json data-types are supported
      - in: query
        name: id
        description: The ID of the event
      responses:
        200:
          description: OK
      tags:
      - Event
      - List
      - Discounts
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