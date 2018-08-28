---
swagger: "2.0"
x-collection-name: SoundCloud
x-complete: 1
info:
  title: Sound Cloud
  description: access-host-upload-and-comment-on-audio-
  version: 1.0.0
host: api.soundcloud.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /users/{user_id}/playlists.json:
    get:
      summary: Get Users Playlists
      description: Returns a collection of playlists created by user with user id
      operationId: getUsersUserPlaylists.json
      x-api-path-slug: usersuser-idplaylists-json-get
      parameters:
      - in: query
        name: consumer_key
      responses:
        200:
          description: OK
      tags:
      - Users
      - Playlists
  /me/playlists.json:
    get:
      summary: Get Me Playlists
      description: Returns a collection of playlists created by the logged-in user
      operationId: getMePlaylists.json
      x-api-path-slug: meplaylists-json-get
      responses:
        200:
          description: OK
      tags:
      - Me
      - Playlists
  /playlists.json:
    get:
      summary: Get Playlists
      description: Returns a collection of playlists
      operationId: getPlaylists.json
      x-api-path-slug: playlists-json-get
      parameters:
      - in: query
        name: consumer_key
      responses:
        200:
          description: OK
      tags:
      - Playlists
  /playlists/{playlist_id}.json:
    get:
      summary: Get Playlists Playlist
      description: Returns a playlist by playlist id
      operationId: getPlaylistsPlaylist.json
      x-api-path-slug: playlistsplaylist-id-json-get
      parameters:
      - in: query
        name: consumer_key
      responses:
        200:
          description: OK
      tags:
      - Playlists
      - Playlist
  /users/{user_id}/playlists.{format}:
    get:
      summary: Get Users Playlists. Format
      description: Returns a collection of playlists created by user with user id
      operationId: getUsersUserPlaylists.Format
      x-api-path-slug: usersuser-idplaylists-format-get
      parameters:
      - in: query
        name: consumer_key
        description: Access, host, upload, and comment on audio
      - in: path
        name: user_id
        description: Access, host, upload, and comment on audio
      responses:
        200:
          description: OK
      tags:
      - Users
      - Playlists
      - ""
      - Format
  /me/playlists.{format}:
    get:
      summary: Get Me Playlists. Format
      description: Returns a collection of playlists created by the logged-in user
      operationId: getMePlaylists.Format
      x-api-path-slug: meplaylists-format-get
      responses:
        200:
          description: OK
      tags:
      - Me
      - Playlists
      - ""
      - Format
  /playlists.{format}:
    get:
      summary: Get Playlists. Format
      description: Returns a collection of playlists
      operationId: getPlaylists.Format
      x-api-path-slug: playlists-format-get
      parameters:
      - in: query
        name: consumer_key
        description: Access, host, upload, and comment on audio
      - in: query
        name: filter
        description: Access, host, upload, and comment on audio
      - in: query
        name: q
        description: Access, host, upload, and comment on audio
      responses:
        200:
          description: OK
      tags:
      - Playlists
      - ""
      - Format
  /playlists/{playlist_id}.{format}:
    get:
      summary: Get Playlists Playlist . Format
      description: Returns a playlist by playlist id
      operationId: getPlaylistsPlaylist.Format
      x-api-path-slug: playlistsplaylist-id-format-get
      parameters:
      - in: query
        name: consumer_key
        description: Access, host, upload, and comment on audio
      - in: path
        name: playlist_id
        description: Access, host, upload, and comment on audio
      responses:
        200:
          description: OK
      tags:
      - Playlists
      - Playlist
      - ""
      - ""
      - Format
---