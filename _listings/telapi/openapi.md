swagger: "2.0"
x-collection-name: TelAPI
x-complete: 1
info:
  title: TelAPI
  description: telapi-is-a-rest-api--what-that-means-for-you-is-that-interacting-with-telapi-to-perform-all-of-your-telephony-needs-is-almost-as-simple-as-visiting-a-website--deeper-knowledge-regarding-rest-is-useful-when-developing-with-telapi-but-definitely-not-required--we-aim-to-provide-all-of-the-information-needed-for-working-with-our-rest-api-throughout-its-documentation-provided-here-so-even-if-you-are-new-to-rest-telapi-will-still-be-a-pleasure-to-use-
  termsOfService: http://www.telapi.com/legal/tos
  version: v2
host: api.telapi.com
basePath: v2/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/hotel/v0/hotels/{hotelId}/room_types:
    get:
      summary: Get a list with the details of all room types for for the specified
        hotel id.
      description: With this call you can load the details about a all available room
        types for the specified hotel.
      operationId: RoomTypes_GetRoomTypes
      x-api-path-slug: apihotelv0hotelshotelidroom-types-get
      parameters:
      - in: header
        name: App-Id
        description: Application identifier
      - in: header
        name: App-Key
        description: Application key
      - in: path
        name: hotelId
        description: The hotel id the room type belongs to
      responses:
        200:
          description: OK
      tags:
      - List
      - Details
      - Of
      - ""
      - Room
      - Typesfor
      - Specified
      - Hotel
      - Id