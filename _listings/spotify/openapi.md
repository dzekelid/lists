---
swagger: "2.0"
x-collection-name: Spotify
x-complete: 1
info:
  title: Spotify
  description: our-web-api-lets-your-applications-fetch-data-from-the-spotify-music-catalog-and-manage-users-playlists-and-saved-music--based-on-simple-rest-principles-our-web-api-endpoints-return-metadata-in-json-format-about-artists-albums-and-tracks-directly-from-the-spotify-catalogue--the-api-also-provides-access-to-userrelated-data-such-as-playlists-and-music-saved-in-a-your-music-library-subject-to-users-authorization-
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
  /users/{user_id}/playlists/{playlist_id}/followers/contains:
    get:
      summary: Get User Playlist Followers Contains
      description: '[Check if Users Follow a Playlist](https://developer.spotify.com/web-api/check-user-following-playlist/)'
      operationId: check-if-users-follow-a-playlisthttpsdeveloperspotifycomwebapicheckuserfollowingplaylist
      x-api-path-slug: usersuser-idplaylistsplaylist-idfollowerscontains-get
      parameters:
      - in: query
        name: ids
        description: A comma-separated list of users ids
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
  /users/{user_id}/playlists/{playlist_id}/tracks:
    delete:
      summary: Delete User Playlist Tracks
      description: '[Remove Tracks from a Playlist](https://developer.spotify.com/web-api/remove-tracks-playlist/)'
      operationId: remove-tracks-from-a-playlisthttpsdeveloperspotifycomwebapiremovetracksplaylist
      x-api-path-slug: usersuser-idplaylistsplaylist-idtracks-delete
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
      - Tracks
    get:
      summary: Get User Playlist Tracks
      description: '[Get a Playlist''s Tracks](https://developer.spotify.com/web-api/get-playlists-tracks/)'
      operationId: get-a-playlists-trackshttpsdeveloperspotifycomwebapigetplayliststracks
      x-api-path-slug: usersuser-idplaylistsplaylist-idtracks-get
      parameters:
      - in: header
        name: Accept
        description: It is used to set specified media type
      - in: query
        name: fields
        description: A comma-separated list of fields to filter query
      - in: query
        name: limit
        description: The maximum number of items to return
      - in: query
        name: market
        description: The market (an ISO 3166-1 alpha-2 country code)
      - in: query
        name: offset
        description: The index of the first item to return
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
      - Tracks
    post:
      summary: Add User Playlist Track
      description: '[Add Tracks to a Playlist](https://developer.spotify.com/web-api/add-tracks-to-playlist/)'
      operationId: add-tracks-to-a-playlisthttpsdeveloperspotifycomwebapiaddtrackstoplaylist
      x-api-path-slug: usersuser-idplaylistsplaylist-idtracks-post
      parameters:
      - in: header
        name: Accept
        description: It is used to set specified media type
      - in: path
        name: playlist_id
        description: The Spotify playlist ID
      - in: query
        name: position
        description: The position to insert the tracks, a zero-based index
      - in: query
        name: uris
        description: A comma-separated list of Spotify track URIs to add
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
      - Tracks
    put:
      summary: Update User Playlist Track
      description: '[Reorder or replace a Playlist''s Tracks](https://developer.spotify.com/web-api/reorder-playlists-tracks/)'
      operationId: reorder-or-replace-a-playlists-trackshttpsdeveloperspotifycomwebapireorderplayliststracks
      x-api-path-slug: usersuser-idplaylistsplaylist-idtracks-put
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
      - Tracks
---