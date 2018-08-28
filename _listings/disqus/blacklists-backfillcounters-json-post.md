---
swagger: "2.0"
info:
  title: Disqus Blacklists BackfillCounters
  description: Blacklists BackfillCounters
  termsOfService: https://docs.disqus.com/kb/terms-and-policies/
  version: 1.0.0
host: disqus.com
basePath: api/3.0/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /blacklists/backfillCounters.json:
    post:
      summary: Blacklists BackfillCounters
      description: "\n     Blacklists BackfillCounters "
      operationId: blacklists-backfillcounters
      responses:
        200:
          description: OK
      tags:
      - comments
      - black lists
definitions: []
x-collection-name: Disqus
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