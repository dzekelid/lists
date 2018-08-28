---
swagger: "2.0"
x-collection-name: Microsoft Graph
x-complete: 0
info:
  title: Microsoft Graph List Rows
  description: List rows Retrieve a list of tablerow objects.
  version: 1.0.0
host: graph.microsoft.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /me/mailFolders/{id}/childFolders/{id}/.../messages/{id}/attachments/{id}:
    get:
      summary: List Attachments
      description: List attachments Retrieve a list of attachment objects attached
        to a message.
      operationId: ListAttachments
      x-api-path-slug: memailfoldersidchildfoldersid---messagesidattachmentsid-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Attachments
  /users/{id | userPrincipalName}/mailFolders/{id}/childFolders/{id}/messages/{id}/attachments/{id}:
    get:
      summary: List Attachments
      description: List attachments Retrieve a list of attachment objects attached
        to a message.
      operationId: ListAttachments
      x-api-path-slug: usersid--userprincipalnamemailfoldersidchildfoldersidmessagesidattachmentsid-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      - in: path
        name: id | userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Attachments
  /me/calendar/calendarView:
    get:
      summary: List Calendar View
      description: |-
        List calendarView
        Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range,
        from the default calendar (../me/calendarview) of a user or group, or some other calendar of the user's.
      operationId: ListCalendarView
      x-api-path-slug: mecalendarcalendarview-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: header
        name: Content-Type
        description: application/json
        type: string
      - in: query
        name: endDateTime
        type: string
      - in: header
        name: Prefer
        type: string
      - in: query
        name: startDateTime
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Calendar
      - View
  /users/{id | userPrincipalName}/calendar/calendarView:
    get:
      summary: List Calendar View
      description: |-
        List calendarView
        Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range,
        from the default calendar (../me/calendarview) of a user or group, or some other calendar of the user's.
      operationId: ListCalendarView
      x-api-path-slug: usersid--userprincipalnamecalendarcalendarview-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: query
        name: endDateTime
        type: string
      - in: path
        name: id | userPrincipalName
        type: string
      - in: header
        name: Prefer
        description: outlook
      - in: query
        name: startDateTime
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Calendar
      - View
  /groups/{id}/calendar/calendarView:
    get:
      summary: List Calendar View
      description: |-
        List calendarView
        Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range,
        from the default calendar (../me/calendarview) of a user or group, or some other calendar of the user's.
      operationId: ListCalendarView
      x-api-path-slug: groupsidcalendarcalendarview-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: query
        name: endDateTime
        type: string
      - in: path
        name: id
        type: string
      - in: header
        name: Prefer
        description: outlook
      - in: query
        name: startDateTime
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Calendar
      - View
  /me/calendars/{id}/calendarView:
    get:
      summary: List Calendar View
      description: |-
        List calendarView
        Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range,
        from the default calendar (../me/calendarview) of a user or group, or some other calendar of the user's.
      operationId: ListCalendarView
      x-api-path-slug: mecalendarsidcalendarview-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: header
        name: Content-Type
        description: application/json
        type: string
      - in: query
        name: endDateTime
        type: string
      - in: path
        name: id
        type: string
      - in: header
        name: Prefer
        type: string
      - in: query
        name: startDateTime
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Calendar
      - View
  /users/{id | userPrincipalName}/calendars/{id}/calendarView:
    get:
      summary: List Calendar View
      description: |-
        List calendarView
        Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range,
        from the default calendar (../me/calendarview) of a user or group, or some other calendar of the user's.
      operationId: ListCalendarView
      x-api-path-slug: usersid--userprincipalnamecalendarsidcalendarview-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: header
        name: Content-Type
        description: application/json
        type: string
      - in: query
        name: endDateTime
        type: string
      - in: path
        name: id
        type: string
      - in: path
        name: id | userPrincipalName
        type: string
      - in: header
        name: Prefer
        type: string
      - in: query
        name: startDateTime
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Calendar
      - View
  /me/calendarGroup/calendars/{id}/calendarView:
    get:
      summary: List Calendar View
      description: |-
        List calendarView
        Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range,
        from the default calendar (../me/calendarview) of a user or group, or some other calendar of the user's.
      operationId: ListCalendarView
      x-api-path-slug: mecalendargroupcalendarsidcalendarview-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: header
        name: Content-Type
        description: application/json
        type: string
      - in: query
        name: endDateTime
        type: string
      - in: path
        name: id
        type: string
      - in: header
        name: Prefer
        type: string
      - in: query
        name: startDateTime
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Calendar
      - View
  /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/calendarView:
    get:
      summary: List Calendar View
      description: |-
        List calendarView
        Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range,
        from the default calendar (../me/calendarview) of a user or group, or some other calendar of the user's.
      operationId: ListCalendarView
      x-api-path-slug: usersid--userprincipalnamecalendargroupcalendarsidcalendarview-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: header
        name: Content-Type
        description: application/json
        type: string
      - in: query
        name: endDateTime
        type: string
      - in: path
        name: id
        type: string
      - in: path
        name: id | userPrincipalName
        type: string
      - in: header
        name: Prefer
        type: string
      - in: query
        name: startDateTime
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Calendar
      - View
  /me/calendarGroups/{id}/calendars/{id}/calendarView:
    get:
      summary: List Calendar View
      description: |-
        List calendarView
        Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range,
        from the default calendar (../me/calendarview) of a user or group, or some other calendar of the user's.
      operationId: ListCalendarView
      x-api-path-slug: mecalendargroupsidcalendarsidcalendarview-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: header
        name: Content-Type
        description: application/json
        type: string
      - in: query
        name: endDateTime
        type: string
      - in: path
        name: id
        type: string
      - in: header
        name: Prefer
        type: string
      - in: query
        name: startDateTime
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Calendar
      - View
  /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/calendarView:
    get:
      summary: List Calendar View
      description: |-
        List calendarView
        Get the occurrences, exceptions, and single instances of events in a calendar view defined by a time range,
        from the default calendar (../me/calendarview) of a user or group, or some other calendar of the user's.
      operationId: ListCalendarView
      x-api-path-slug: usersid--userprincipalnamecalendargroupsidcalendarsidcalendarview-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: header
        name: Content-Type
        description: application/json
        type: string
      - in: query
        name: endDateTime
        type: string
      - in: path
        name: id
        type: string
      - in: path
        name: id | userPrincipalName
        type: string
      - in: header
        name: Prefer
        type: string
      - in: query
        name: startDateTime
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Calendar
      - View
  /me/calendar/events:
    get:
      summary: List Events
      description: List events Retrieve a list of events in a calendar.  The list
        contains single instance meetings and series masters.
      operationId: ListEvents
      x-api-path-slug: mecalendarevents-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: header
        name: Prefer
        description: outlook
      - in: header
        name: 'Prefer: outlook.timezone'
        description: The default time zone for events in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Events
  /users/{id | userPrincipalName}/calendar/events:
    get:
      summary: List Events
      description: List events Retrieve a list of events in a calendar.  The list
        contains single instance meetings and series masters.
      operationId: ListEvents
      x-api-path-slug: usersid--userprincipalnamecalendarevents-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id | userPrincipalName
        type: string
      - in: header
        name: Prefer
        description: outlook
      - in: header
        name: 'Prefer: outlook.timezone'
        description: The default time zone for events in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Events
  /groups/{id}/calendar/events:
    get:
      summary: List Events
      description: List events Retrieve a list of event objects.
      operationId: ListEvents
      x-api-path-slug: groupsidcalendarevents-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: path
        name: id
        type: string
      - in: header
        name: Prefer
        description: outlook
      responses:
        200:
          description: OK
      tags:
      - List
      - Events
  /me/calendars/{id}/events:
    get:
      summary: List Events
      description: List events Retrieve a list of events in a calendar.  The list
        contains single instance meetings and series masters.
      operationId: ListEvents
      x-api-path-slug: mecalendarsidevents-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      - in: header
        name: Prefer
        description: outlook
      - in: header
        name: 'Prefer: outlook.timezone'
        description: The default time zone for events in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Events
  /users/{id | userPrincipalName}/calendars/{id}/events:
    get:
      summary: List Events
      description: List events Retrieve a list of events in a calendar.  The list
        contains single instance meetings and series masters.
      operationId: ListEvents
      x-api-path-slug: usersid--userprincipalnamecalendarsidevents-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      - in: path
        name: id | userPrincipalName
        type: string
      - in: header
        name: Prefer
        description: outlook
      - in: header
        name: 'Prefer: outlook.timezone'
        description: The default time zone for events in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Events
  /me/calendarGroup/calendars/{id}/events:
    get:
      summary: List Events
      description: List events Retrieve a list of events in a calendar.  The list
        contains single instance meetings and series masters.
      operationId: ListEvents
      x-api-path-slug: mecalendargroupcalendarsidevents-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      - in: header
        name: Prefer
        description: outlook
      - in: header
        name: 'Prefer: outlook.timezone'
        description: The default time zone for events in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Events
  /users/{id | userPrincipalName}/calendarGroup/calendars/{id}/events:
    get:
      summary: List Events
      description: List events Retrieve a list of events in a calendar.  The list
        contains single instance meetings and series masters.
      operationId: ListEvents
      x-api-path-slug: usersid--userprincipalnamecalendargroupcalendarsidevents-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      - in: path
        name: id | userPrincipalName
        type: string
      - in: header
        name: Prefer
        description: outlook
      - in: header
        name: 'Prefer: outlook.timezone'
        description: The default time zone for events in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Events
  /me/calendarGroups/{id}/calendars/{id}/events:
    get:
      summary: List Events
      description: List events Retrieve a list of events in a calendar.  The list
        contains single instance meetings and series masters.
      operationId: ListEvents
      x-api-path-slug: mecalendargroupsidcalendarsidevents-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      - in: header
        name: Prefer
        description: outlook
      - in: header
        name: 'Prefer: outlook.timezone'
        description: The default time zone for events in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Events
  /users/{id | userPrincipalName}/calendarGroups/{id}/calendars/{id}/events:
    get:
      summary: List Events
      description: List events Retrieve a list of events in a calendar.  The list
        contains single instance meetings and series masters.
      operationId: ListEvents
      x-api-path-slug: usersid--userprincipalnamecalendargroupsidcalendarsidevents-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      - in: path
        name: id | userPrincipalName
        type: string
      - in: header
        name: Prefer
        description: outlook
      - in: header
        name: 'Prefer: outlook.timezone'
        description: The default time zone for events in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Events
  /me/calendarGroup/calendars:
    get:
      summary: List Calendars
      description: List calendars Retrieve a list of calendars belonging to a calendar
        group.
      operationId: ListCalendars
      x-api-path-slug: mecalendargroupcalendars-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Calendars
  /users/{id | userPrincipalName}/calendarGroup/calendars:
    get:
      summary: List Calendars
      description: List calendars Retrieve a list of calendars belonging to a calendar
        group.
      operationId: ListCalendars
      x-api-path-slug: usersid--userprincipalnamecalendargroupcalendars-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: header
        name: Content-Type
        description: application/json
      - in: path
        name: id | userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Calendars
  /me/calendarGroups/{id}/calendars:
    get:
      summary: List Calendars
      description: List calendars Retrieve a list of calendars belonging to a calendar
        group.
      operationId: ListCalendars
      x-api-path-slug: mecalendargroupsidcalendars-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Calendars
  /users/{id | userPrincipalName}/calendarGroups/{id}/calendars:
    get:
      summary: List Calendars
      description: List calendars Retrieve a list of calendars belonging to a calendar
        group.
      operationId: ListCalendars
      x-api-path-slug: usersid--userprincipalnamecalendargroupsidcalendars-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      - in: path
        name: id | userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Calendars
  /workbook/worksheets(&lt;id|name&gt;)/charts(&lt;name&gt;)/series(&lt;undefined&gt;)/points:
    get:
      summary: List Points
      description: List points Retrieve a list of chartpoints objects.
      operationId: ListPoints
      x-api-path-slug: workbookworksheetsltidnamegtchartsltnamegtseriesltundefinedgtpoints-get
      parameters:
      - in: header
        name: Authorization
        description: Bearer
      responses:
        200:
          description: OK
      tags:
      - List
      - Points
  /me/contactFolders/{id}/childFolders:
    get:
      summary: List Child Folders
      description: List childFolders Get a collection of child folders under the specified
        contact folder.
      operationId: ListChildFolders
      x-api-path-slug: mecontactfoldersidchildfolders-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Child
      - Folders
  /users/{id | userPrincipalName}/contactFolders/{id}/childFolders:
    get:
      summary: List Child Folders
      description: List childFolders Get a collection of child folders under the specified
        contact folder.
      operationId: ListChildFolders
      x-api-path-slug: usersid--userprincipalnamecontactfoldersidchildfolders-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      - in: path
        name: id | userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Child
      - Folders
  /me/contacts:
    get:
      summary: List Contacts
      description: List contacts Get a contact collection from the default Contacts
        folder of the signed-in user (.../me/contacts), or from the specified contact
        folder.
      operationId: ListContacts
      x-api-path-slug: mecontacts-get
      parameters:
      - in: query
        name: $filter
        type: string
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: header
        name: Content-Type
        description: application/json
      responses:
        200:
          description: OK
      tags:
      - List
      - Contacts
  /users/{id | userPrincipalName}/contacts:
    get:
      summary: List Contacts
      description: List contacts Get a contact collection from the default Contacts
        folder of the signed-in user (.../me/contacts), or from the specified contact
        folder.
      operationId: ListContacts
      x-api-path-slug: usersid--userprincipalnamecontacts-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: header
        name: Content-Type
        description: application/json
      - in: path
        name: id | userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Contacts
  /me/contactFolders/{id}/contacts:
    get:
      summary: List Contacts
      description: List contacts Get a contact collection from the default Contacts
        folder of the signed-in user (.../me/contacts), or from the specified contact
        folder.
      operationId: ListContacts
      x-api-path-slug: mecontactfoldersidcontacts-get
      parameters:
      - in: query
        name: $filter
        type: string
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: header
        name: Content-Type
        description: application/json
      - in: path
        name: Id
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Contacts
  /users/{id | userPrincipalName}/contactFolders/{id}/contacts:
    get:
      summary: List Contacts
      description: List contacts Get a contact collection from the default Contacts
        folder of the signed-in user (.../me/contacts), or from the specified contact
        folder.
      operationId: ListContacts
      x-api-path-slug: usersid--userprincipalnamecontactfoldersidcontacts-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: header
        name: Content-Type
        description: application/json
      - in: path
        name: id
        type: string
      - in: path
        name: id | userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Contacts
  /devices:
    get:
      summary: List Devices
      description: List devices Retrieve a list of device objects registered in the
        organization.
      operationId: ListDevices
      x-api-path-slug: devices-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Devices
  /devices/{id}/registeredOwners:
    get:
      summary: List Registered Owners
      description: List registeredOwners Retrieve a list of users that are registered
        owners of the device.
      operationId: ListRegisteredOwners
      x-api-path-slug: devicesidregisteredowners-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Registered
      - Owners
  /devices/{id}/registeredUsers:
    get:
      summary: List Registered Users
      description: List registeredUsers Retrieve a list of users that are registered
        users of the device.
      operationId: ListRegisteredUsers
      x-api-path-slug: devicesidregisteredusers-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Registered
      - Users
  /directoryRoles:
    get:
      summary: List Directory Roles
      description: List directoryRoles List the directory roles that are activated
        in the tenant.
      operationId: ListDirectoryRoles
      x-api-path-slug: directoryroles-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Directory
      - Roles
  /directoryRoles/{id}/members:
    get:
      summary: List Members
      description: List members Retrieve a list of the users that are assigned to
        the directory role.  Only users can be assigned to a directory role.
      operationId: ListMembers
      x-api-path-slug: directoryrolesidmembers-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Members
  /directoryRoleTemplates:
    get:
      summary: List Directory Role Templates
      description: List directoryRoleTemplates Retrieve a list of directoryRoleTemplate
        objects.
      operationId: ListDirectoryRoleTemplates
      x-api-path-slug: directoryroletemplates-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Directory
      - Role
      - Templates
  /drives:
    get:
      summary: List Available Drives
      description: List available drives Retrieve the list of Drive resources available
        for a target User or Group. Your app can also request the set of document
        libraries on the SharePoint root site.
      operationId: ListAvailableDrives
      x-api-path-slug: drives-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Available
      - Drives
  /me/drives:
    get:
      summary: List Available Drives
      description: List available drives Retrieve the list of Drive resources available
        for a target User or Group. Your app can also request the set of document
        libraries on the SharePoint root site.
      operationId: ListAvailableDrives
      x-api-path-slug: medrives-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Available
      - Drives
  /groups/{id}/drives:
    get:
      summary: List Available Drives
      description: List available drives Retrieve the list of Drive resources available
        for a target User or Group. Your app can also request the set of document
        libraries on the SharePoint root site.
      operationId: ListAvailableDrives
      x-api-path-slug: groupsiddrives-get
      parameters:
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Available
      - Drives
  /me/events/{id}/attachments:
    get:
      summary: List Attachments
      description: List attachments Retrieve a list of attachment objects attached
        to an event.
      operationId: ListAttachments
      x-api-path-slug: meeventsidattachments-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Attachments
  /users/{id | userPrincipalName}/events/{id}/attachments:
    get:
      summary: List Attachments
      description: List attachments Retrieve a list of attachment objects attached
        to an event.
      operationId: ListAttachments
      x-api-path-slug: usersid--userprincipalnameeventsidattachments-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      - in: path
        name: id | userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Attachments
  /groups/{id}/events/{id}/attachments:
    get:
      summary: List Attachments
      description: List attachments Retrieve a list of attachment objects attached
        to an event.
      operationId: ListAttachments
      x-api-path-slug: groupsideventsidattachments-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Attachments
  /me/calendar/events/{id}/attachments:
    get:
      summary: List Attachments
      description: List attachments Retrieve a list of attachment objects attached
        to an event.
      operationId: ListAttachments
      x-api-path-slug: mecalendareventsidattachments-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Attachments
  /users/{id | userPrincipalName}/calendar/events/{id}/attachments:
    get:
      summary: List Attachments
      description: List attachments Retrieve a list of attachment objects attached
        to an event.
      operationId: ListAttachments
      x-api-path-slug: usersid--userprincipalnamecalendareventsidattachments-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      - in: path
        name: id | userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Attachments
  /groups/{id}/calendar/events/{id}/attachments:
    get:
      summary: List Attachments
      description: List attachments Retrieve a list of attachment objects attached
        to an event.
      operationId: ListAttachments
      x-api-path-slug: groupsidcalendareventsidattachments-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Attachments
  /me/calendars/{id}/events/{id}/attachments:
    get:
      summary: List Attachments
      description: List attachments Retrieve a list of attachment objects attached
        to an event.
      operationId: ListAttachments
      x-api-path-slug: mecalendarsideventsidattachments-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Attachments
  /users/{id | userPrincipalName}/calendars/{id}/events/{id}/attachments:
    get:
      summary: List Attachments
      description: List attachments Retrieve a list of attachment objects attached
        to an event.
      operationId: ListAttachments
      x-api-path-slug: usersid--userprincipalnamecalendarsideventsidattachments-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      - in: path
        name: id | userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Attachments
  /me/calendargroup/calendars/{id}/events/{id}/attachments:
    get:
      summary: List Attachments
      description: List attachments Retrieve a list of attachment objects attached
        to an event.
      operationId: ListAttachments
      x-api-path-slug: mecalendargroupcalendarsideventsidattachments-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Attachments
  /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/attachments:
    get:
      summary: List Attachments
      description: List attachments Retrieve a list of attachment objects attached
        to an event.
      operationId: ListAttachments
      x-api-path-slug: usersid--userprincipalnamecalendargroupcalendarsideventsidattachments-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      - in: path
        name: id | userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Attachments
  /me/calendargroups/{id}/calendars/{id}/events/{id}/attachments:
    get:
      summary: List Attachments
      description: List attachments Retrieve a list of attachment objects attached
        to an event.
      operationId: ListAttachments
      x-api-path-slug: mecalendargroupsidcalendarsideventsidattachments-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Attachments
  /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/attachments:
    get:
      summary: List Attachments
      description: List attachments Retrieve a list of attachment objects attached
        to an event.
      operationId: ListAttachments
      x-api-path-slug: usersid--userprincipalnamecalendargroupsidcalendarsideventsidattachments-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      - in: path
        name: id | userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Attachments
  /me/events/{id}/instances:
    get:
      summary: List Instances
      description: List instances Get the instances (occurrences) of an event for
        a specified time range. If the event is a SeriesMaster type, this returns
        the occurrences and exceptions of the event in the specified time range.
      operationId: ListInstances
      x-api-path-slug: meeventsidinstances-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: query
        name: endDateTime
        type: string
      - in: path
        name: id
        type: string
      - in: header
        name: Prefer
        type: string
      - in: query
        name: startDateTime
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Instances
  /users/{id | userPrincipalName}/events/{id}/instances:
    get:
      summary: List Instances
      description: List instances Get the instances (occurrences) of an event for
        a specified time range. If the event is a SeriesMaster type, this returns
        the occurrences and exceptions of the event in the specified time range.
      operationId: ListInstances
      x-api-path-slug: usersid--userprincipalnameeventsidinstances-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: query
        name: endDateTime
        type: string
      - in: path
        name: id
        type: string
      - in: path
        name: id | userPrincipalName
        type: string
      - in: header
        name: Prefer
        type: string
      - in: query
        name: startDateTime
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Instances
  /groups/{id}/events/{id}/instances:
    get:
      summary: List Instances
      description: List instances Get the instances (occurrences) of an event for
        a specified time range. If the event is a SeriesMaster type, this returns
        the occurrences and exceptions of the event in the specified time range.
      operationId: ListInstances
      x-api-path-slug: groupsideventsidinstances-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: query
        name: endDateTime
        type: string
      - in: path
        name: id
        type: string
      - in: header
        name: Prefer
        type: string
      - in: query
        name: startDateTime
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Instances
  /me/calendar/events/{id}/instances:
    get:
      summary: List Instances
      description: List instances Get the instances (occurrences) of an event for
        a specified time range. If the event is a SeriesMaster type, this returns
        the occurrences and exceptions of the event in the specified time range.
      operationId: ListInstances
      x-api-path-slug: mecalendareventsidinstances-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: query
        name: endDateTime
        type: string
      - in: path
        name: id
        type: string
      - in: header
        name: Prefer
        type: string
      - in: query
        name: startDateTime
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Instances
  /users/{id | userPrincipalName}/calendar/events/{id}/instances:
    get:
      summary: List Instances
      description: List instances Get the instances (occurrences) of an event for
        a specified time range. If the event is a SeriesMaster type, this returns
        the occurrences and exceptions of the event in the specified time range.
      operationId: ListInstances
      x-api-path-slug: usersid--userprincipalnamecalendareventsidinstances-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: query
        name: endDateTime
        type: string
      - in: path
        name: id
        type: string
      - in: path
        name: id | userPrincipalName
        type: string
      - in: header
        name: Prefer
        type: string
      - in: query
        name: startDateTime
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Instances
  /groups/{id}/calendar/events/{id}/instances:
    get:
      summary: List Instances
      description: List instances Get the instances (occurrences) of an event for
        a specified time range. If the event is a SeriesMaster type, this returns
        the occurrences and exceptions of the event in the specified time range.
      operationId: ListInstances
      x-api-path-slug: groupsidcalendareventsidinstances-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: query
        name: endDateTime
        type: string
      - in: path
        name: id
        type: string
      - in: header
        name: Prefer
        type: string
      - in: query
        name: startDateTime
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Instances
  /me/calendars/{id}/events/{id}/instances:
    get:
      summary: List Instances
      description: List instances Get the instances (occurrences) of an event for
        a specified time range. If the event is a SeriesMaster type, this returns
        the occurrences and exceptions of the event in the specified time range.
      operationId: ListInstances
      x-api-path-slug: mecalendarsideventsidinstances-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: query
        name: endDateTime
        type: string
      - in: path
        name: id
        type: string
      - in: header
        name: Prefer
        type: string
      - in: query
        name: startDateTime
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Instances
  /users/{id | userPrincipalName}/calendars/{id}/events/{id}/instances:
    get:
      summary: List Instances
      description: List instances Get the instances (occurrences) of an event for
        a specified time range. If the event is a SeriesMaster type, this returns
        the occurrences and exceptions of the event in the specified time range.
      operationId: ListInstances
      x-api-path-slug: usersid--userprincipalnamecalendarsideventsidinstances-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: query
        name: endDateTime
        type: string
      - in: path
        name: id
        type: string
      - in: path
        name: id | userPrincipalName
        type: string
      - in: header
        name: Prefer
        type: string
      - in: query
        name: startDateTime
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Instances
  /me/calendargroup/calendars/{id}/events/{id}/instances:
    get:
      summary: List Instances
      description: List instances Get the instances (occurrences) of an event for
        a specified time range. If the event is a SeriesMaster type, this returns
        the occurrences and exceptions of the event in the specified time range.
      operationId: ListInstances
      x-api-path-slug: mecalendargroupcalendarsideventsidinstances-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: query
        name: endDateTime
        type: string
      - in: path
        name: id
        type: string
      - in: header
        name: Prefer
        type: string
      - in: query
        name: startDateTime
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Instances
  /users/{id | userPrincipalName}/calendargroup/calendars/{id}/events/{id}/instances:
    get:
      summary: List Instances
      description: List instances Get the instances (occurrences) of an event for
        a specified time range. If the event is a SeriesMaster type, this returns
        the occurrences and exceptions of the event in the specified time range.
      operationId: ListInstances
      x-api-path-slug: usersid--userprincipalnamecalendargroupcalendarsideventsidinstances-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: query
        name: endDateTime
        type: string
      - in: path
        name: id
        type: string
      - in: path
        name: id | userPrincipalName
        type: string
      - in: header
        name: Prefer
        type: string
      - in: query
        name: startDateTime
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Instances
  /me/calendargroups/{id}/calendars/{id}/events/{id}/instances:
    get:
      summary: List Instances
      description: List instances Get the instances (occurrences) of an event for
        a specified time range. If the event is a SeriesMaster type, this returns
        the occurrences and exceptions of the event in the specified time range.
      operationId: ListInstances
      x-api-path-slug: mecalendargroupsidcalendarsideventsidinstances-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: query
        name: endDateTime
        type: string
      - in: path
        name: id
        type: string
      - in: header
        name: Prefer
        type: string
      - in: query
        name: startDateTime
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Instances
  /users/{id | userPrincipalName}/calendargroups/{id}/calendars/{id}/events/{id}/instances:
    get:
      summary: List Instances
      description: List instances Get the instances (occurrences) of an event for
        a specified time range. If the event is a SeriesMaster type, this returns
        the occurrences and exceptions of the event in the specified time range.
      operationId: ListInstances
      x-api-path-slug: usersid--userprincipalnamecalendargroupsidcalendarsideventsidinstances-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: query
        name: endDateTime
        type: string
      - in: path
        name: id
        type: string
      - in: path
        name: id | userPrincipalName
        type: string
      - in: header
        name: Prefer
        type: string
      - in: query
        name: startDateTime
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Instances
  /me/messages/{id}/attachments:
    get:
      summary: List Attachments
      description: List attachments Retrieve a list of attachment objects attached
        to a message.
      operationId: ListAttachments
      x-api-path-slug: memessagesidattachments-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Attachments
  /users/{id | userPrincipalName}/messages/{id}/attachments:
    get:
      summary: List Attachments
      description: List attachments Retrieve a list of attachment objects attached
        to a message.
      operationId: ListAttachments
      x-api-path-slug: usersid--userprincipalnamemessagesidattachments-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      - in: path
        name: id | userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Attachments
  /groups:
    get:
      summary: List Groups
      description: List groups List all the groups available in an organization, including
        but not limited to Office 365 Groups. The default properties of each group
        are returned.
      operationId: ListGroups
      x-api-path-slug: groups-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Groups
  /groups/{id}/acceptedSenders:
    get:
      summary: List Accepted Senders
      description: List acceptedSenders Get a list of users or groups that are in
        the acceptedSenders list for this group.
      operationId: ListAcceptedSenders
      x-api-path-slug: groupsidacceptedsenders-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Accepted
      - Senders
  /groups/{id}/calendarView:
    get:
      summary: List Calendar View
      description: List calendarView Get the occurrences, exceptions, and single instances
        of events in a calendar view defined by a time range, from the default calendar
        of a group.
      operationId: ListCalendarView
      x-api-path-slug: groupsidcalendarview-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: query
        name: endDateTime
        type: string
      - in: path
        name: id
        type: string
      - in: header
        name: Prefer
        description: string
      - in: query
        name: startDateTime
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Calendar
      - View
  /groups/{id}/conversations:
    get:
      summary: List Conversations
      description: List conversations Retrieve the list of conversations in this group.
      operationId: ListConversations
      x-api-path-slug: groupsidconversations-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Conversations
  /groups/{id}/events:
    get:
      summary: List Events
      description: List events Retrieve a list of event objects.
      operationId: ListEvents
      x-api-path-slug: groupsidevents-get
      parameters:
      - in: query
        name: $expand
        type: string
      - in: query
        name: $filter
        type: string
      - in: header
        name: Authorization
        description: Bearer
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Events
  /groups/{id}/memberOf:
    get:
      summary: List Member Of
      description: List memberOf Get groups that the group is a direct member of.
      operationId: ListMemberOf
      x-api-path-slug: groupsidmemberof-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Member
      - Of
  /groups/{id}/members:
    get:
      summary: List Members
      description: List members Get a list of the group's direct members. A group
        can have users, contacts, and other groups as members. This operation is not
        transitive.
      operationId: ListMembers
      x-api-path-slug: groupsidmembers-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Members
  /groups/{id}/owners:
    get:
      summary: List Owners
      description: List owners Retrieve a list of the group's owners. The owners are
        a set of non-admin users who are allowed to modify the group object.
      operationId: ListOwners
      x-api-path-slug: groupsidowners-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Owners
  /groups/{id}/rejectedSenders:
    get:
      summary: List Rejected Senders
      description: List rejectedSenders Get a list of users or groups that are in
        the rejectedSenders list for this group.
      operationId: ListRejectedSenders
      x-api-path-slug: groupsidrejectedsenders-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Rejected
      - Senders
  /groups/{id}/threads:
    get:
      summary: List Threads
      description: List threads Get all the threads of a group.
      operationId: ListThreads
      x-api-path-slug: groupsidthreads-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Threads
  /me/inferenceClassification/overrides:
    get:
      summary: List Overrides
      description: List overrides Get the overrides that a user has set up to always
        classify messages from certain senders in specific ways.
      operationId: ListOverrides
      x-api-path-slug: meinferenceclassificationoverrides-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Overrides
  /users/{id}/inferenceClassification/overrides:
    get:
      summary: List Overrides
      description: List overrides Get the overrides that a user has set up to always
        classify messages from certain senders in specific ways.
      operationId: ListOverrides
      x-api-path-slug: usersidinferenceclassificationoverrides-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Overrides
  /groups/{group-id}/drive/items/{item-id}:
    get:
      summary: List Children Of A Drive Item
      description: List children of a driveItem Return a collection of DriveItems
        in the children relationship of a DriveItem.
      operationId: ListChildrenOfADriveItem
      x-api-path-slug: groupsgroupiddriveitemsitemid-get
      parameters:
      - in: path
        name: group-id
        type: string
      - in: header
        name: if-none-match
        description: If this request header is included and the eTag (or cTag) provided
          matches the current tag on the file, an HTTP 304 Not Modified response is
          returned
        type: string
      - in: path
        name: item-id
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Children
      - OfDrive
      - Item
  /me/drive/root/children:
    get:
      summary: List Children Of A Drive Item
      description: List children of a driveItem Return a collection of DriveItems
        in the children relationship of a DriveItem.
      operationId: ListChildrenOfADriveItem
      x-api-path-slug: medriverootchildren-get
      parameters:
      - in: header
        name: if-none-match
        description: If this request header is included and the eTag (or cTag) provided
          matches the current tag on the file, an HTTP 304 Not Modified response is
          returned
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Children
      - OfDrive
      - Item
  /me/drive/items/{item-id}/children:
    get:
      summary: List Children Of A Drive Item
      description: List children of a driveItem Return a collection of DriveItems
        in the children relationship of a DriveItem.
      operationId: ListChildrenOfADriveItem
      x-api-path-slug: medriveitemsitemidchildren-get
      parameters:
      - in: header
        name: if-none-match
        description: If this request header is included and the eTag (or cTag) provided
          matches the current tag on the file, an HTTP 304 Not Modified response is
          returned
        type: string
      - in: path
        name: item-id
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Children
      - OfDrive
      - Item
  /me/drive/root:/{item-path}:/children:
    get:
      summary: List Children Of A Drive Item
      description: List children of a driveItem Return a collection of DriveItems
        in the children relationship of a DriveItem.
      operationId: ListChildrenOfADriveItem
      x-api-path-slug: medriverootitempathchildren-get
      parameters:
      - in: header
        name: if-none-match
        description: If this request header is included and the eTag (or cTag) provided
          matches the current tag on the file, an HTTP 304 Not Modified response is
          returned
        type: string
      - in: path
        name: item-path
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Children
      - OfDrive
      - Item
  /drives/{drive-id}/items/{item-id}/children:
    get:
      summary: List Children Of A Drive Item
      description: List children of a driveItem Return a collection of DriveItems
        in the children relationship of a DriveItem.
      operationId: ListChildrenOfADriveItem
      x-api-path-slug: drivesdriveiditemsitemidchildren-get
      parameters:
      - in: path
        name: drive-id
        type: string
      - in: header
        name: if-none-match
        description: If this request header is included and the eTag (or cTag) provided
          matches the current tag on the file, an HTTP 304 Not Modified response is
          returned
        type: string
      - in: path
        name: item-id
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Children
      - OfDrive
      - Item
  /me/drive/items/{item-id}/permissions:
    get:
      summary: List Permissions On A Drive Item
      description: List permissions on a DriveItem List the effective permissions
        of on a DriveItem.
      operationId: ListPermissionsOnADriveItem
      x-api-path-slug: medriveitemsitemidpermissions-get
      parameters:
      - in: header
        name: if-none-match
        description: If this request header is included and the etag provided matches
          the current etag on the item, an HTTP 304 Not Modified response is returned
        type: string
      - in: path
        name: item-id
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Permissions
      - OnDrive
      - Item
  /me/drive/root:/{path}:/permissions:
    get:
      summary: List Permissions On A Drive Item
      description: List permissions on a DriveItem List the effective permissions
        of on a DriveItem.
      operationId: ListPermissionsOnADriveItem
      x-api-path-slug: medriverootpathpermissions-get
      parameters:
      - in: header
        name: if-none-match
        description: If this request header is included and the etag provided matches
          the current etag on the item, an HTTP 304 Not Modified response is returned
        type: string
      - in: path
        name: path
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Permissions
      - OnDrive
      - Item
  /drives/{drive-id}/items/{item-id}/permissions:
    get:
      summary: List Permissions On A Drive Item
      description: List permissions on a DriveItem List the effective permissions
        of on a DriveItem.
      operationId: ListPermissionsOnADriveItem
      x-api-path-slug: drivesdriveiditemsitemidpermissions-get
      parameters:
      - in: path
        name: drive-id
        type: string
      - in: header
        name: if-none-match
        description: If this request header is included and the etag provided matches
          the current etag on the item, an HTTP 304 Not Modified response is returned
        type: string
      - in: path
        name: item-id
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Permissions
      - OnDrive
      - Item
  /groups/{group-id}/drive/items/{item-id}/permissions:
    get:
      summary: List Permissions On A Drive Item
      description: List permissions on a DriveItem List the effective permissions
        of on a DriveItem.
      operationId: ListPermissionsOnADriveItem
      x-api-path-slug: groupsgroupiddriveitemsitemidpermissions-get
      parameters:
      - in: path
        name: group-id
        type: string
      - in: header
        name: if-none-match
        description: If this request header is included and the etag provided matches
          the current etag on the item, an HTTP 304 Not Modified response is returned
        type: string
      - in: path
        name: item-id
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Permissions
      - OnDrive
      - Item
  /me/drive/root:/{item-path}:/thumbnails:
    get:
      summary: List Thumbnails For A Drive Item
      description: List thumbnails for a DriveItem Retrieve a collection of ThumbnailSet
        resources for a DriveItem resource.
      operationId: ListThumbnailsForADriveItem
      x-api-path-slug: medriverootitempaththumbnails-get
      parameters:
      - in: path
        name: item-path
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - ThumbnailsA
      - Drive
      - Item
  /me/drive/items/{item-id}/thumbnails:
    get:
      summary: List Thumbnails For A Drive Item
      description: List thumbnails for a DriveItem Retrieve a collection of ThumbnailSet
        resources for a DriveItem resource.
      operationId: ListThumbnailsForADriveItem
      x-api-path-slug: medriveitemsitemidthumbnails-get
      parameters:
      - in: path
        name: item-id
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - ThumbnailsA
      - Drive
      - Item
  /groups/{group-id}/drive/items/{item-id}/thumbnails:
    get:
      summary: List Thumbnails For A Drive Item
      description: List thumbnails for a DriveItem Retrieve a collection of ThumbnailSet
        resources for a DriveItem resource.
      operationId: ListThumbnailsForADriveItem
      x-api-path-slug: groupsgroupiddriveitemsitemidthumbnails-get
      parameters:
      - in: path
        name: group-id
        type: string
      - in: path
        name: item-id
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - ThumbnailsA
      - Drive
      - Item
  /me/mailFolders/{id}/childFolders:
    get:
      summary: List Child Folders
      description: List childFolders Get the folder collection under the specified
        folder. You can use the .../me/MailFolders shortcut to get the top-level folder
        collection and navigate to another folder.
      operationId: ListChildFolders
      x-api-path-slug: memailfoldersidchildfolders-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Child
      - Folders
  /users/{id | userPrincipalName}/mailFolders/{id}/childFolders:
    get:
      summary: List Child Folders
      description: List childFolders Get the folder collection under the specified
        folder. You can use the .../me/MailFolders shortcut to get the top-level folder
        collection and navigate to another folder.
      operationId: ListChildFolders
      x-api-path-slug: usersid--userprincipalnamemailfoldersidchildfolders-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      - in: path
        name: id | userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Child
      - Folders
  /me/mailFolders/{id}/messages:
    get:
      summary: List Messages
      description: List messages Get all the messages in the signed-in user's mailbox,
        or those messages in a specified folder in the mailbox.
      operationId: ListMessages
      x-api-path-slug: memailfoldersidmessages-get
      parameters:
      - in: query
        name: $filter
        type: string
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Messages
  /users/{id | userPrincipalName}/mailFolders/{id}/messages:
    get:
      summary: List Messages
      description: List messages Get all the messages in the signed-in user's mailbox,
        or those messages in a specified folder in the mailbox.
      operationId: ListMessages
      x-api-path-slug: usersid--userprincipalnamemailfoldersidmessages-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: path
        name: id
        type: string
      - in: path
        name: id | userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Messages
  /me/mailFolders/{id}/messages/{id}/attachments:
    get:
      summary: List Attachments
      description: List attachments Retrieve a list of attachment objects attached
        to a message.
      operationId: ListAttachments
      x-api-path-slug: memailfoldersidmessagesidattachments-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Attachments
  /users/{id | userPrincipalName}/mailFolders/{id}/messages/{id}/attachments:
    get:
      summary: List Attachments
      description: List attachments Retrieve a list of attachment objects attached
        to a message.
      operationId: ListAttachments
      x-api-path-slug: usersid--userprincipalnamemailfoldersidmessagesidattachments-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id
        type: string
      - in: path
        name: id | userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Attachments
  /workbook/names:
    get:
      summary: List Named Item Collection
      description: List NamedItemCollection Retrieve a list of nameditem objects.
      operationId: ListNamedItemCollection
      x-api-path-slug: workbooknames-get
      parameters:
      - in: header
        name: Authorization
        description: Bearer
      responses:
        200:
          description: OK
      tags:
      - List
      - Named
      - Item
      - Collection
  /groups/{id}/threads/{id}/posts/{id}/attachments:
    get:
      summary: List Attachments
      description: List attachments Retrieve a list of attachment objects attached
        to a post.
      operationId: ListAttachments
      x-api-path-slug: groupsidthreadsidpostsidattachments-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Attachments
  /groups/{id}/conversations/{id}/threads/{id}/posts/{id}/attachments:
    get:
      summary: List Attachments
      description: List attachments Retrieve a list of attachment objects attached
        to a post.
      operationId: ListAttachments
      x-api-path-slug: groupsidconversationsidthreadsidpostsidattachments-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Attachments
  /workbook/names(&lt;name&gt;)/range/format/borders:
    get:
      summary: List Range Border Collection
      description: List RangeBorderCollection Retrieve a list of rangeborder objects.
      operationId: ListRangeBorderCollection
      x-api-path-slug: workbooknamesltnamegtrangeformatborders-get
      parameters:
      - in: header
        name: Authorization
        description: Bearer
      responses:
        200:
          description: OK
      tags:
      - List
      - Range
      - Border
      - Collection
  /workbook/worksheets(&lt;id|name&gt;)/range(&lt;address&gt;)/format/borders:
    get:
      summary: List Range Border Collection
      description: List RangeBorderCollection Retrieve a list of rangeborder objects.
      operationId: ListRangeBorderCollection
      x-api-path-slug: workbookworksheetsltidnamegtrangeltaddressgtformatborders-get
      parameters:
      - in: header
        name: Authorization
        description: Bearer
      responses:
        200:
          description: OK
      tags:
      - List
      - Range
      - Border
      - Collection
  /workbook/tables(&lt;id|name&gt;)/columns(&lt;id|name&gt;)/range/format/borders:
    get:
      summary: List Range Border Collection
      description: List RangeBorderCollection Retrieve a list of rangeborder objects.
      operationId: ListRangeBorderCollection
      x-api-path-slug: workbooktablesltidnamegtcolumnsltidnamegtrangeformatborders-get
      parameters:
      - in: header
        name: Authorization
        description: Bearer
      responses:
        200:
          description: OK
      tags:
      - List
      - Range
      - Border
      - Collection
  /subscribedSkus:
    get:
      summary: List Subscribed Skus
      description: List subscribedSkus Retrieve the list of commercial subscriptions
        that an organization has acquired.
      operationId: ListSubscribedSkus
      x-api-path-slug: subscribedskus-get
      parameters:
      - in: header
        name: Authorization
        description: Bearer token
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Subscribed
      - Skus
  /workbook/tables:
    get:
      summary: List Table Collection
      description: List TableCollection Retrieve a list of table objects.
      operationId: ListTableCollection
      x-api-path-slug: workbooktables-get
      parameters:
      - in: header
        name: Authorization
        description: Bearer
      responses:
        200:
          description: OK
      tags:
      - List
      - Table
      - Collection
  /workbook/worksheets(&lt;id|name&gt;)/tables:
    get:
      summary: List Table Collection
      description: List TableCollection Retrieve a list of table objects.
      operationId: ListTableCollection
      x-api-path-slug: workbookworksheetsltidnamegttables-get
      parameters:
      - in: header
        name: Authorization
        description: Bearer
      responses:
        200:
          description: OK
      tags:
      - List
      - Table
      - Collection
  /workbook/tables(&lt;id|name&gt;)/columns:
    get:
      summary: List Columns
      description: List columns Retrieve a list of tablecolumn objects.
      operationId: ListColumns
      x-api-path-slug: workbooktablesltidnamegtcolumns-get
      parameters:
      - in: header
        name: Authorization
        description: Bearer
      responses:
        200:
          description: OK
      tags:
      - List
      - Columns
  /workbook/worksheets(&lt;id|name&gt;)/tables(&lt;id|name&gt;)/columns:
    get:
      summary: List Columns
      description: List columns Retrieve a list of tablecolumn objects.
      operationId: ListColumns
      x-api-path-slug: workbookworksheetsltidnamegttablesltidnamegtcolumns-get
      parameters:
      - in: header
        name: Authorization
        description: Bearer
      responses:
        200:
          description: OK
      tags:
      - List
      - Columns
  /workbook/tables(&lt;id|name&gt;)/rows:
    get:
      summary: List Rows
      description: List rows Retrieve a list of tablerow objects.
      operationId: ListRows
      x-api-path-slug: workbooktablesltidnamegtrows-get
      parameters:
      - in: header
        name: Authorization
        description: Bearer
      responses:
        200:
          description: OK
      tags:
      - List
      - Rows
  /workbook/worksheets(&lt;id|name&gt;)/tables(&lt;id|name&gt;)/rows:
    get:
      summary: List Rows
      description: List rows Retrieve a list of tablerow objects.
      operationId: ListRows
      x-api-path-slug: workbookworksheetsltidnamegttablesltidnamegtrows-get
      parameters:
      - in: header
        name: Authorization
        description: Bearer
      responses:
        200:
          description: OK
      tags:
      - List
      - Rows
  /users:
    get:
      summary: List Users
      description: List users Retrieve a list of user objects.
      operationId: ListUsers
      x-api-path-slug: users-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: header
        name: Content-Type
        description: application/json
      responses:
        200:
          description: OK
      tags:
      - List
      - Users
  /users/{id | userPrincipalName}/calendarGroups:
    get:
      summary: List Calendar Groups
      description: List calendarGroups Get the user's calendar groups.
      operationId: ListCalendarGroups
      x-api-path-slug: usersid--userprincipalnamecalendargroups-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: header
        name: Content-Type
        description: application/json
      - in: path
        name: id | userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Calendar
      - Groups
  /users/{id | userPrincipalName}/calendars:
    get:
      summary: List Calendars
      description: List calendars Get all the user's calendars (/calendars navigation
        property), get the calendars from the default calendar group or from a specific
        calendar group.
      operationId: ListCalendars
      x-api-path-slug: usersid--userprincipalnamecalendars-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: header
        name: Content-Type
        description: application/json
      - in: path
        name: id | userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Calendars
  /me/calendargroups/{calendar_group_id}/calendars:
    get:
      summary: List Calendars
      description: List calendars Get all the user's calendars (/calendars navigation
        property), get the calendars from the default calendar group or from a specific
        calendar group.
      operationId: ListCalendars
      x-api-path-slug: mecalendargroupscalendar-group-idcalendars-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: path
        name: calendar_group_id
        type: string
      - in: header
        name: Content-Type
        description: application/json
      responses:
        200:
          description: OK
      tags:
      - List
      - Calendars
  /users/{id | userPrincipalName}/calendarGroups/{calendar_group_id}/calendars:
    get:
      summary: List Calendars
      description: List calendars Get all the user's calendars (/calendars navigation
        property), get the calendars from the default calendar group or from a specific
        calendar group.
      operationId: ListCalendars
      x-api-path-slug: usersid--userprincipalnamecalendargroupscalendar-group-idcalendars-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: path
        name: calendar_group_id
        type: string
      - in: header
        name: Content-Type
        description: application/json
      - in: path
        name: id | userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Calendars
  /users/{id | userPrincipalName}/calendarView:
    get:
      summary: List Calendar View
      description: List calendarView Get the occurrences, exceptions, and single instances
        of events in a calendar view defined by a time range, from the user's default
        calendar, or from some other calendar of the user's.
      operationId: ListCalendarView
      x-api-path-slug: usersid--userprincipalnamecalendarview-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: header
        name: Content-Type
        description: application/json
        type: string
      - in: query
        name: endDateTime
        type: string
      - in: path
        name: id | userPrincipalName
        type: string
      - in: header
        name: Prefer
        type: string
      - in: query
        name: startDateTime
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Calendar
      - View
  /users/{id | userPrincipalName}/contactFolders:
    get:
      summary: List Contact Folders
      description: List contactFolders Get the contact folder collection in the default
        Contacts folder of the signed-in user.
      operationId: ListContactFolders
      x-api-path-slug: usersid--userprincipalnamecontactfolders-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: header
        name: Content-Type
        description: application/json
      - in: path
        name: id | userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Contact
      - Folders
  /me/contactFolder/{id}/childFolders/{id}/.../contacts:
    get:
      summary: List Contacts
      description: List contacts Get a contact collection from the default Contacts
        folder of the signed-in user.
      operationId: ListContacts
      x-api-path-slug: mecontactfolderidchildfoldersid---contacts-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: header
        name: Content-Type
        description: application/json
      - in: path
        name: id
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Contacts
  /users/{id | userPrincipalName}/contactFolders/{id}/childFolders/{id}/contacts:
    get:
      summary: List Contacts
      description: List contacts Get a contact collection from the default Contacts
        folder of the signed-in user.
      operationId: ListContacts
      x-api-path-slug: usersid--userprincipalnamecontactfoldersidchildfoldersidcontacts-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: header
        name: Content-Type
        description: application/json
      - in: path
        name: id
        type: string
      - in: path
        name: id | userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Contacts
  /users/{id | userPrincipalName}/createdObjects:
    get:
      summary: List Created Objects
      description: List createdObjects Get a list of directory objects that were created
        by the user.
      operationId: ListCreatedObjects
      x-api-path-slug: usersid--userprincipalnamecreatedobjects-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: header
        name: Content-Type
        description: application/json
      - in: path
        name: id | userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Created
      - Objects
  /users/{id | userPrincipalName}/directReports:
    get:
      summary: List Direct Reports
      description: List directReports Get user's direct reports. Returns the users
        and contacts for whom this user is assigned as manager.
      operationId: ListDirectReports
      x-api-path-slug: usersid--userprincipalnamedirectreports-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: header
        name: Content-Type
        description: application/json
      - in: path
        name: id | userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Direct
      - Reports
  /users/{id | userPrincipalName}/events:
    get:
      summary: List Events
      description: List events Get a list of event objects in the user's mailbox.
        The list contains single instance meetings and series masters.
      operationId: ListEvents
      x-api-path-slug: usersid--userprincipalnameevents-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
        type: string
      - in: path
        name: id | userPrincipalName
        type: string
      - in: header
        name: 'Prefer: outlook.timezone'
        description: The default time zone for events in the response
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Events
  /users/{id | userPrincipalName}/mailFolders:
    get:
      summary: List Mail Folders
      description: List mailFolders Get the mail folder collection under the root
        folder of the signed-in user.
      operationId: ListMailFolders
      x-api-path-slug: usersid--userprincipalnamemailfolders-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: header
        name: Content-Type
        description: application/json
      - in: path
        name: id | userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Mail
      - Folders
  /users/{id | userPrincipalName}/manager:
    get:
      summary: List Manager
      description: List manager Get user's manager. Returns the user or contact assigned
        as the user's manager.
      operationId: ListManager
      x-api-path-slug: usersid--userprincipalnamemanager-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: header
        name: Content-Type
        description: application/json
      - in: path
        name: id | userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Manager
  /users/{id | userPrincipalName}/memberOf:
    get:
      summary: List Member Of
      description: List memberOf Get groups and directory roles that the user is a
        direct member of.
      operationId: ListMemberOf
      x-api-path-slug: usersid--userprincipalnamememberof-get
      parameters:
      - in: header
        name: Accept
        description: application/json
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: path
        name: id | userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Member
      - Of
  /users/{id | userPrincipalName}/messages:
    get:
      summary: List Messages
      description: List messages Get the messages in the signed-in user's mailbox
        (including the Deleted Items and Clutter folders).
      operationId: ListMessages
      x-api-path-slug: usersid--userprincipalnamemessages-get
      parameters:
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: path
        name: id | userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Messages
  /users/{id | userPrincipalName}/ownedDevices:
    get:
      summary: List Owned Devices
      description: List ownedDevices Get the list of devices that are owned by the
        user.
      operationId: ListOwnedDevices
      x-api-path-slug: usersid--userprincipalnameowneddevices-get
      parameters:
      - in: header
        name: Accept
        description: application/json
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: path
        name: id | userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Owned
      - Devices
  /users/{id | userPrincipalName}/ownedObjects:
    get:
      summary: List Owned Objects
      description: List ownedObjects Get the list of directory objects that are owned
        by the user.
      operationId: ListOwnedObjects
      x-api-path-slug: usersid--userprincipalnameownedobjects-get
      parameters:
      - in: header
        name: Accept
        description: application/json
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: path
        name: id | userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Owned
      - Objects
  /users/{id | userPrincipalName}/registeredDevices:
    get:
      summary: List Registered Devices
      description: List registeredDevices Get the list of user's registered devices.
      operationId: ListRegisteredDevices
      x-api-path-slug: usersid--userprincipalnameregistereddevices-get
      parameters:
      - in: header
        name: Accept
        description: application/json
      - in: header
        name: Authorization
        description: 'Bearer '
      - in: path
        name: id | userPrincipalName
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Registered
      - Devices
  /workbook/worksheets:
    get:
      summary: List Worksheets
      description: List worksheets Retrieve a list of worksheet objects.
      operationId: ListWorksheets
      x-api-path-slug: workbookworksheets-get
      parameters:
      - in: header
        name: Authorization
        description: Bearer
      responses:
        200:
          description: OK
      tags:
      - List
      - Worksheets
  /workbook/worksheets({id|name})/names:
    get:
      summary: List Names
      description: List names Retrieve a list of named item associated with the worksheet.
      operationId: ListNames
      x-api-path-slug: workbookworksheetsidnamenames-get
      parameters:
      - in: header
        name: Authorization
        description: Bearer {code}
      - in: path
        name: id|name
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Names
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