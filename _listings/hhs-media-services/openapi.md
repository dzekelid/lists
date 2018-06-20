---
swagger: "2.0"
x-collection-name: HHS Media Services
x-complete: 1
info:
  title: HHS Media Services
  description: div-classswaggeruiwrap-extrafooterh3common-features--behaviorsh3----div-classfeatures--------ul------------listrong-sort-paramstrong-supports-multi-column-sorting-through-the-use-of-commas-as-delimiters-and-a-hyphen-to-denote-descending-order-----------------br----------------strongspanexamplesspanstrong----------------ul--------------------lispan-classexamplenamespanspan-classdescriptionsort-results-by-name-ascendingspanli--------------------lispan-classexamplenamespanspan-classdescriptionsort-results-by-name-descendingspanli--------------------lispan-classexamplenameidspanspan-classdescriptionsort-results-by-name-descending-and-then-by-id-ascendingspanli--------------------lispan-classexampleiddatecontentauthoredspanspan-classdescriptionsort-results-by-id-ascending-and-then-date-descendingspanli----------------ul------------li------------listrongdate-formatsstrong-date-input-format-is-expected-to-be-based-on-a-hrefhttpwww-ietf-orgrfcrfc3339-txtrfc-3339a--br----------------spanstrongexamplestrongspan----------------ulli20131118t184301zliul------------li--------ul----divdiv
  termsOfService: http://www.hhs.gov/web/socialmedia/policies/tos.html#ready
  version: "2"
host: api.digitalmedia.hhs.gov
basePath: /api/v2
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /resources/userMediaLists/{id}.json:
    get:
      summary: Get UserMediaList by ID
      description: Get a specific user media list by 'id'.
      operationId: getUserMediaList
      x-api-path-slug: resourcesusermedialistsid-json-get
      parameters:
      - in: query
        name: displayMethod
        description: Method used to render an html request
      - in: path
        name: id
        description: The id of the record to look up
      responses:
        200:
          description: OK
      tags:
      - Resources
      - UserMediaLists
      - Id
---