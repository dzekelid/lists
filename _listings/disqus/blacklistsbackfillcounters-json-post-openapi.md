---
swagger: "2.0"
x-collection-name: Disqus
x-complete: 0
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
      description: Blacklists BackfillCounters
      operationId: blacklists-backfillcounters
      x-api-path-slug: blacklistsbackfillcounters-json-post
      responses:
        200:
          description: OK
      tags:
      - Comments
      - Black Lists
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