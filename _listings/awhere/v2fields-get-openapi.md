---
swagger: "2.0"
x-collection-name: aWhere
x-complete: 0
info:
  title: aWhere Get Fields List
  description: "####Request\nThis API call retrieves the list of fields in your account.
    \n\n[Get Fields Documentation](http://developer.awhere.com/api/reference/fields/get-fields)\n\n\n####Security\nThis
    API call uses the security Access Token that is retrieved with the \"Get a Token\"
    request. If you run that request first, it will save a token to Postman and this
    API will use it automatically. You can also see where the token should normally
    go by clicking the \"Headers\" tab below. The Authorization header holds the token,
    replacing the \"{{aWhereAccessToken}}\" part."
  version: 1.0.0
host: api.awhere.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v2/fields:
    get:
      summary: Get Fields List
      description: "####Request\nThis API call retrieves the list of fields in your
        account. \n\n[Get Fields Documentation](http://developer.awhere.com/api/reference/fields/get-fields)\n\n\n####Security\nThis
        API call uses the security Access Token that is retrieved with the \"Get a
        Token\" request. If you run that request first, it will save a token to Postman
        and this API will use it automatically. You can also see where the token should
        normally go by clicking the \"Headers\" tab below. The Authorization header
        holds the token, replacing the \"{{aWhereAccessToken}}\" part."
      operationId: V2FieldsGet
      x-api-path-slug: v2fields-get
      responses:
        200:
          description: OK
      tags:
      - Agriculture
      - Fields
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