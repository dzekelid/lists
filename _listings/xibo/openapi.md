swagger: "2.0"
x-collection-name: Xibo
x-complete: 1
info:
  title: Xibo API
  description: xibo-cms-api
  termsOfService: http://xibo.org.uk/legal
  version: 1.0.0
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /schedule/{displayGroupId}/events:
    get:
      summary: Event List
      description: ""
      operationId: scheduleCalendarData
      x-api-path-slug: scheduledisplaygroupidevents-get
      parameters:
      - in: formData
        name: date
        description: Date in Y-m-d H:i:s
      - in: path
        name: displayGroupId
        description: The DisplayGroupId to return the event list for
      responses:
        200:
          description: OK
      tags:
      - Event
      - List