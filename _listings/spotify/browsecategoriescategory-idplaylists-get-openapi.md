---
swagger: "2.0"
x-collection-name: Spotify
x-complete: 0
info:
  title: Spotify Browse Category Playlists
  description: '[Get a Category''s playlists](https://developer.spotify.com/web-api/get-categorys-playlists/)'
  version: v1
host: api.spotify.com
basePath: /v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /browse/categories/{category_id}:
    get:
      summary: Browse Category
      description: '[Get a Single Browse Category](https://developer.spotify.com/web-api/get-category/)'
      operationId: get-a-single-browse-categoryhttpsdeveloperspotifycomwebapigetcategory
      x-api-path-slug: browsecategoriescategory-id-get
      parameters:
      - in: header
        name: Accept
        description: It is used to set specified media type
      - in: path
        name: category_id
        description: The Spotify ID of the category you wish to fetch
      - in: query
        name: country
        description: The country (an ISO 3166-1 alpha-2 country code)
      - in: query
        name: locale
        description: The desired language, consisting of an ISO 639 language code
          and an ISO 3166-1 alpha-2 country code, joined by an underscore
      responses:
        200:
          description: OK
      tags:
      - Music
      - Categories
      - Playlists
  /browse/categories/{category_id}/playlists:
    get:
      summary: Browse Category Playlists
      description: '[Get a Category''s playlists](https://developer.spotify.com/web-api/get-categorys-playlists/)'
      operationId: get-a-categorys-playlistshttpsdeveloperspotifycomwebapigetcategorysplaylists
      x-api-path-slug: browsecategoriescategory-idplaylists-get
      parameters:
      - in: header
        name: Accept
        description: It is used to set specified media type
      - in: path
        name: category_id
        description: The Spotify ID of the category you wish to fetch
      - in: query
        name: country
        description: The country (an ISO 3166-1 alpha-2 country code)
      - in: query
        name: limit
        description: The maximum number of items to return
      - in: query
        name: offset
        description: The index of the first item to return
      responses:
        200:
          description: OK
      tags:
      - Music
      - Playlists
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