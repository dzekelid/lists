---
name: Spotify
x-slug: spotify
description: Spotify is a digital music service that gives you access to millions
  of songs.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1165-spotify.jpg
x-kinRank: "8"
x-alexaRank: "133"
tags: Lists
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/spotify/apis.md
specificationVersion: "0.14"
apis:
- name: Spotify Browse Category
  x-api-slug: spotify
  description: '[Get a Single Browse Category](https://developer.spotify.com/web-api/get-category/)'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1165-spotify.jpg
  humanURL: http://www.spotify.com
  baseURL: https://api.spotify.com//v1//browse/categories/{category_id}
  tags: Music,Categories,Playlists
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/spotify/browsecategoriescategory-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/spotify/browsecategoriescategory-id-get-openapi.md
- name: Spotify Browse Category Playlists
  x-api-slug: spotify
  description: '[Get a Category''s playlists](https://developer.spotify.com/web-api/get-categorys-playlists/)'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1165-spotify.jpg
  humanURL: http://www.spotify.com
  baseURL: https://api.spotify.com//v1//browse/categories/{category_id}/playlists
  tags: Music,Playlists
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/spotify/browsecategoriescategory-idplaylists-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/spotify/browsecategoriescategory-idplaylists-get-openapi.md
- name: Spotify Browse Featured Playlists
  x-api-slug: spotify
  description: '[Get a List of Featured Playlists](https://developer.spotify.com/web-api/get-list-featured-playlists/)'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1165-spotify.jpg
  humanURL: http://www.spotify.com
  baseURL: https://api.spotify.com//v1//browse/featured-playlists
  tags: Music,Playlists
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/spotify/browsefeaturedplaylists-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/spotify/browsefeaturedplaylists-get-openapi.md
- name: Spotify Get User Playlists
  x-api-slug: spotify
  description: '[Get a List of a User''s Playlists](https://developer.spotify.com/web-api/get-list-users-playlists/)'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1165-spotify.jpg
  humanURL: http://www.spotify.com
  baseURL: https://api.spotify.com//v1//users/{user_id}/playlists
  tags: Music,User,Playlists
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/spotify/usersuser-idplaylists-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/spotify/usersuser-idplaylists-get-openapi.md
- name: Spotify Add User Playlists
  x-api-slug: spotify
  description: '[Create a Playlist](https://developer.spotify.com/web-api/create-playlist/)'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1165-spotify.jpg
  humanURL: http://www.spotify.com
  baseURL: https://api.spotify.com//v1//users/{user_id}/playlists
  tags: Music,User,Playlists
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/spotify/usersuser-idplaylists-post-openapi.md
- name: Spotify Get User Playlist
  x-api-slug: spotify
  description: '[Get a Playlist](https://developer.spotify.com/web-api/get-playlist/)'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1165-spotify.jpg
  humanURL: http://www.spotify.com
  baseURL: https://api.spotify.com//v1//users/{user_id}/playlists/{playlist_id}
  tags: Music,User,Playlists
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/spotify/usersuser-idplaylistsplaylist-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/spotify/usersuser-idplaylistsplaylist-id-get-openapi.md
- name: Spotify Update User Playlist
  x-api-slug: spotify
  description: '[Change a Playlist''s Details](https://developer.spotify.com/web-api/change-playlist-details/)'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1165-spotify.jpg
  humanURL: http://www.spotify.com
  baseURL: https://api.spotify.com//v1//users/{user_id}/playlists/{playlist_id}
  tags: Music,User,Playlists
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/spotify/usersuser-idplaylistsplaylist-id-put-openapi.md
- name: Spotify Delete User Playlist Followers
  x-api-slug: spotify
  description: '[Unfollow a Playlist](https://developer.spotify.com/web-api/unfollow-playlist/)'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1165-spotify.jpg
  humanURL: http://www.spotify.com
  baseURL: https://api.spotify.com//v1//users/{user_id}/playlists/{playlist_id}/followers
  tags: Music,User,Playlists,Followers
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/spotify/usersuser-idplaylistsplaylist-idfollowers-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/spotify/usersuser-idplaylistsplaylist-idfollowers-delete-openapi.md
- name: Spotify Update User Playlist Followers
  x-api-slug: spotify
  description: '[Follow a Playlist](https://developer.spotify.com/web-api/follow-playlist/)'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1165-spotify.jpg
  humanURL: http://www.spotify.com
  baseURL: https://api.spotify.com//v1//users/{user_id}/playlists/{playlist_id}/followers
  tags: Music,User,Playlists,Followers
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/spotify/usersuser-idplaylistsplaylist-idfollowers-put-openapi.md
- name: Spotify Get User Playlist Followers Contains
  x-api-slug: spotify
  description: '[Check if Users Follow a Playlist](https://developer.spotify.com/web-api/check-user-following-playlist/)'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1165-spotify.jpg
  humanURL: http://www.spotify.com
  baseURL: https://api.spotify.com//v1//users/{user_id}/playlists/{playlist_id}/followers/contains
  tags: Music,User,Playlists,Followers
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/spotify/usersuser-idplaylistsplaylist-idfollowerscontains-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/spotify/usersuser-idplaylistsplaylist-idfollowerscontains-get-openapi.md
- name: Spotify Delete User Playlist Tracks
  x-api-slug: spotify
  description: '[Remove Tracks from a Playlist](https://developer.spotify.com/web-api/remove-tracks-playlist/)'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1165-spotify.jpg
  humanURL: http://www.spotify.com
  baseURL: https://api.spotify.com//v1//users/{user_id}/playlists/{playlist_id}/tracks
  tags: Music,User,Playlists,Tracks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/spotify/usersuser-idplaylistsplaylist-idtracks-delete-openapi.md
- name: Spotify Get User Playlist Tracks
  x-api-slug: spotify
  description: '[Get a Playlist''s Tracks](https://developer.spotify.com/web-api/get-playlists-tracks/)'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1165-spotify.jpg
  humanURL: http://www.spotify.com
  baseURL: https://api.spotify.com//v1//users/{user_id}/playlists/{playlist_id}/tracks
  tags: Music,User,Playlists,Tracks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/spotify/usersuser-idplaylistsplaylist-idtracks-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/spotify/usersuser-idplaylistsplaylist-idtracks-get-openapi.md
- name: Spotify Add User Playlist Track
  x-api-slug: spotify
  description: '[Add Tracks to a Playlist](https://developer.spotify.com/web-api/add-tracks-to-playlist/)'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1165-spotify.jpg
  humanURL: http://www.spotify.com
  baseURL: https://api.spotify.com//v1//users/{user_id}/playlists/{playlist_id}/tracks
  tags: Music,User,Playlists,Tracks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/spotify/usersuser-idplaylistsplaylist-idtracks-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/spotify/usersuser-idplaylistsplaylist-idtracks-post-openapi.md
- name: Spotify Update User Playlist Track
  x-api-slug: spotify
  description: '[Reorder or replace a Playlist''s Tracks](https://developer.spotify.com/web-api/reorder-playlists-tracks/)'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1165-spotify.jpg
  humanURL: http://www.spotify.com
  baseURL: https://api.spotify.com//v1//users/{user_id}/playlists/{playlist_id}/tracks
  tags: Music,User,Playlists,Tracks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/spotify/usersuser-idplaylistsplaylist-idtracks-put-openapi.md
- name: Spotify
  x-api-slug: spotify
  description: Spotify is a digital music service that gives you access to millions
    of songs.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/1165-spotify.jpg
  humanURL: http://www.spotify.com
  baseURL: https://api.spotify.com//v1
  tags: Lists
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/spotify/openapi.md
x-common:
- type: x-api-json--authoritative
  url: https://developer.spotify.com/wp-content/uploads/apis.json
- type: x-android-sdk
  url: https://developer.spotify.com/technologies/spotify-android-sdk/
- type: x-application-gallery
  url: https://developer.spotify.com/my-applications/
- type: x-application-gallery
  url: https://developer.spotify.com/showcase/
- type: x-base-url
  url: https://api.spotify.com
- type: x-blog
  url: http://www.spotify.com/blog/
- type: x-blog-rss
  url: http://www.spotify.com/blog/feed
- type: x-change-log
  url: https://developer.spotify.com/web-api/change-log/
- type: x-console
  url: https://developer.spotify.com/web-api/console/
- type: x-crunchbase
  url: https://crunchbase.com/organization/spotify
- type: x-crunchbase
  url: http://www.crunchbase.com/company/spotify
- type: x-developer
  url: https://developer.spotify.com/
- type: x-email
  url: office@spotify.com
- type: x-ios-sdk
  url: https://developer.spotify.com/technologies/spotify-ios-sdk/
- type: x-issues
  url: https://github.com/spotify/web-api/issues
- type: x-stack-overflow
  url: http://stackoverflow.com/questions/tagged/spotify
- type: x-terms-of-service
  url: https://developer.spotify.com/developer-terms-of-use/
- type: x-twitter
  url: https://twitter.com/SpotifyPlatform
- type: x-twitter
  url: https://twitter.com/spotify
- type: x-github
  url: https://github.com/spotify
- type: x-website
  url: http://www.spotify.com
- type: x-website
  url: http://spotify.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---