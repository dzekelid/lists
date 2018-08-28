swagger: "2.0"
x-collection-name: Browshot
x-complete: 1
info:
  title: Browshot
  description: take-screenshots-of-any-website-in-real-time
  termsOfService: https://browshot.com/terms
  contact:
    name: API Support
    url: https://browshot.com/contact
    email: support@browshot.com
  version: 1.17.0
host: api.browshot.com
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /browser/list:
    get:
      summary: Get all browsers
      description: Get all browsers.
      operationId: GetBrowsersInfo
      x-api-path-slug: browserlist-get
      responses:
        200:
          description: OK
      tags:
      - Browser
      - List
  /instance/list:
    get:
      summary: Get all instances
      description: Get all instances.
      operationId: GetInstancesInfo
      x-api-path-slug: instancelist-get
      responses:
        200:
          description: OK
      tags:
      - Instance
      - List
  /screenshot/list:
    get:
      summary: Get information about screenshots
      description: Get information about the last 100 screenshots requested.
      operationId: GetMultipleScreenshotsInfo
      x-api-path-slug: screenshotlist-get
      parameters:
      - in: query
        name: limit
        description: maximum number of screenshots information to return
      - in: query
        name: status
        description: get list of screenshot in a given status (error, finished, in_process)
      responses:
        200:
          description: OK
      tags:
      - Screenshot
      - List