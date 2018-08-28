---
swagger: "2.0"
x-collection-name: Spotify
x-complete: 0
info:
  title: Spotify Update User Playlist Followers
  description: '[Follow a Playlist](https://developer.spotify.com/web-api/follow-playlist/)'
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
  /browse/featured-playlists:
    get:
      summary: Browse Featured Playlists
      description: '[Get a List of Featured Playlists](https://developer.spotify.com/web-api/get-list-featured-playlists/)'
      operationId: get-a-list-of-featured-playlistshttpsdeveloperspotifycomwebapigetlistfeaturedplaylists
      x-api-path-slug: browsefeaturedplaylists-get
      parameters:
      - in: header
        name: Accept
        description: It is used to set specified media type
      - in: query
        name: country
        description: The country (an ISO 3166-1 alpha-2 country code)
      - in: query
        name: limit
        description: The maximum number of items to return
      - in: query
        name: locale
        description: The desired language, consisting of an ISO 639 language code
          and an ISO 3166-1 alpha-2 country code, joined by an underscore
      - in: query
        name: offset
        description: The index of the first item to return
      - in: query
        name: timestamp
        description: A timestamp in ISO 8601 format (yyyy-MM-ddTHH:mm:ss) with the
          users local time to get results tailored to a specific date and time in
          the day
      responses:
        200:
          description: OK
      tags:
      - Music
      - Playlists
  /users/{user_id}/playlists:
    get:
      summary: Get User Playlists
      description: '[Get a List of a User''s Playlists](https://developer.spotify.com/web-api/get-list-users-playlists/)'
      operationId: get-a-list-of-a-users-playlistshttpsdeveloperspotifycomwebapigetlistusersplaylists
      x-api-path-slug: usersuser-idplaylists-get
      parameters:
      - in: header
        name: Accept
        description: It is used to set specified media type
      - in: query
        name: limit
        description: The maximum number of items to return
      - in: query
        name: offset
        description: The index of the first item to return
      - in: path
        name: user_id
        description: The users Spotify user ID
      responses:
        200:
          description: OK
      tags:
      - Music
      - User
      - Playlists
    post:
      summary: Add User Playlists
      description: '[Create a Playlist](https://developer.spotify.com/web-api/create-playlist/)'
      operationId: create-a-playlisthttpsdeveloperspotifycomwebapicreateplaylist
      x-api-path-slug: usersuser-idplaylists-post
      parameters:
      - in: header
        name: Accept
        description: It is used to set specified media type
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: user_id
        description: The users Spotify user ID
      responses:
        200:
          description: OK
      tags:
      - Music
      - User
      - Playlists
  /users/{user_id}/playlists/{playlist_id}:
    get:
      summary: Get User Playlist
      description: '[Get a Playlist](https://developer.spotify.com/web-api/get-playlist/)'
      operationId: get-a-playlisthttpsdeveloperspotifycomwebapigetplaylist
      x-api-path-slug: usersuser-idplaylistsplaylist-id-get
      parameters:
      - in: header
        name: Accept
        description: It is used to set specified media type
      - in: query
        name: fields
        description: A comma-separated list of fields to filter query
      - in: query
        name: market
        description: The market (an ISO 3166-1 alpha-2 country code)
      - in: path
        name: playlist_id
        description: The Spotify playlist ID
      - in: path
        name: user_id
        description: The users Spotify user ID
      responses:
        200:
          description: OK
      tags:
      - Music
      - User
      - Playlists
    put:
      summary: Update User Playlist
      description: '[Change a Playlist''s Details](https://developer.spotify.com/web-api/change-playlist-details/)'
      operationId: change-a-playlists-detailshttpsdeveloperspotifycomwebapichangeplaylistdetails
      x-api-path-slug: usersuser-idplaylistsplaylist-id-put
      parameters:
      - in: header
        name: Accept
        description: It is used to set specified media type
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: playlist_id
        description: The Spotify playlist ID
      - in: path
        name: user_id
        description: The users Spotify user ID
      responses:
        200:
          description: OK
      tags:
      - Music
      - User
      - Playlists
  /users/{user_id}/playlists/{playlist_id}/followers:
    delete:
      summary: Delete User Playlist Followers
      description: '[Unfollow a Playlist](https://developer.spotify.com/web-api/unfollow-playlist/)'
      operationId: unfollow-a-playlisthttpsdeveloperspotifycomwebapiunfollowplaylist
      x-api-path-slug: usersuser-idplaylistsplaylist-idfollowers-delete
      parameters:
      - in: path
        name: playlist_id
        description: The Spotify playlist ID
      - in: path
        name: user_id
        description: The users Spotify user ID
      responses:
        200:
          description: OK
      tags:
      - Music
      - User
      - Playlists
      - Followers
    put:
      summary: Update User Playlist Followers
      description: '[Follow a Playlist](https://developer.spotify.com/web-api/follow-playlist/)'
      operationId: follow-a-playlisthttpsdeveloperspotifycomwebapifollowplaylist
      x-api-path-slug: usersuser-idplaylistsplaylist-idfollowers-put
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: playlist_id
        description: The Spotify playlist ID
      - in: path
        name: user_id
        description: The users Spotify user ID
      responses:
        200:
          description: OK
      tags:
      - Music
      - User
      - Playlists
      - Followers
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