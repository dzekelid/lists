---
swagger: "2.0"
x-collection-name: 7digital
x-complete: 0
info:
  title: 7digital Playlist API playlists/{playlistId}
  description: Deletes the playlist at {playlistId}. The playlist can only be deleted
    by its owner, i.e. oauth_token representing the user has to be provided.
  version: "1.2"
host: api.7digital.com
basePath: 1.2/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  playlists:
    'get ':
      summary: playlists
      description: Returns a list of all public playlists. If an oauth_token is provided
        then also given users private playlists will be included in the response.
      operationId: playlists
      x-api-path-slug: playlists-get
      parameters:
      - ~
      - in: query
        name: oauth_token
        description: Users OAuth access token - allows user to view Private playlist
          if it belongs to them
      - in: query
        name: page
        description: nttttttPage number of the result set
      - in: query
        name: pageSize
        description: Number of items to be returned per page
      - in: query
        name: user
        description: This allows you to pass the id of a user you wish to view the
          playlists of a specific user
      responses:
        200:
          description: OK
      tags:
      - Playlists
  playlists/{playlistId}:
    'delete ':
      summary: playlists/{playlistId}
      description: Deletes the playlist at {playlistId}. The playlist can only be
        deleted by its owner, i.e. oauth_token representing the user has to be provided.
      operationId: playlistsplaylistid
      x-api-path-slug: playlistsplaylistid-delete
      parameters:
      - ~
      - in: query
        name: oauth_token
        description: Users OAuth access token
      responses:
        200:
          description: OK
      tags:
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