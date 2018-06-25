---
swagger: "2.0"
x-collection-name: The New York Times
x-complete: 0
info:
  title: New York Times Best Seller List
  description: The Books API has services for getting information about The New York
    Times Best Sellers Lists and Book Reviews.
  termsOfService: https://developer.nytimes.com/tou
  version: 2.0.0
host: api.nytimes.com
basePath: /svc
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /books/v2/lists.{format}:
    get:
      summary: Best Seller List
      description: The Books API has services for getting information about The New
        York Times Best Sellers Lists and Book Reviews.
      operationId: GET_lists-format
      x-api-path-slug: booksv2lists-format-get
      parameters:
      - in: query
        name: bestsellers-date
        description: YYYY-MM-DDThe week-ending date for the sales reflected on list-name
      - in: query
        name: date
        description: YYYY-MM-DD  The date the best-seller list was published on NYTimes
      - in: path
        name: format
        description: The format
        type: string
        format: string
      - in: query
        name: isbn
        description: International Standard Book Number, 10 or 13 digits
      - in: query
        name: list
        description: The name of the Times best-seller list
      - in: query
        name: offset
        description: Sets the starting point of the result set
      - in: query
        name: published-date
        description: YYYY-MM-DDThe date the best-seller list was published on NYTimes
      - in: query
        name: rank
        description: The rank of the best seller on list-name as of bestsellers-date
      - in: query
        name: rank-last-week
        description: The rank of the best seller on list-name one week prior to bestsellers-date
      - in: query
        name: sort-order
        description: Sets the sort order of the result set
      - in: query
        name: weeks-on-list
        description: The number of weeks that the best seller has been on list-name,
          as of bestsellers-date
      responses:
        200:
          description: OK
      tags:
      - News
      - Lists
x-streamrank:
  polling_total_time_average: "0.12"
  polling_size_download_average: "14702.92"
  streaming_total_time_average: "0.07"
  streaming_size_download_average: "7358.57"
  change_yes: "4"
  change_no: "2148"
  time_percentage: "40"
  size_percentage: "50"
  change_percentage: "0"
  last_run: "2018-05-12"
  days_run: "7"
  minute_run: "0"
---