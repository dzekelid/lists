swagger: "2.0"
x-collection-name: ATTOM
x-complete: 1
info:
  title: Attom Data Solutions API
  description: attom-empowers-customers-with-better-property-data--we-warehouse-property-data-nationwide-with-myriad-data-points-on-each-parcel-including-ownership-information-latlong-square-footage-loan-types-sales-history-sales-comps-crime-schools-and-more-
  version: 1.0.0
host: search.onboard-apis.com
basePath: /communityapi/v2.0.0
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /property/id:
    get:
      summary: Returns a list of properties that fit a criteria.
      description: Get a list of property IDs within a specific geography that have
        a specific number of beds. Use orderby to choose how you want your results
        sorted.
      operationId: getPropertyIdList
      x-api-path-slug: propertyid-get
      parameters:
      - in: header
        name: accept
        description: application/xml or application/json (default)
      - in: header
        name: apikey
        description: Application Key
      - in: query
        name: geoid
        description: A list of geographies that this property belongs to
      - in: query
        name: maxBeds
        description: The max Bed size to search from
      - in: query
        name: minBeds
        description: The min Bed size to search from
      - in: query
        name: orderby
        description: Sort Options
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - Properties
      - That
      - Fit
      - Criteria