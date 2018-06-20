---
name: 7digital
x-slug: 7digital
description: Welcome to 7digital!    Choose from over 30 million high quality tracks
  in our store; download, sync and play your music on the go.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/294-7digital.jpg
x-kinRank: "7"
x-alexaRank: "55455"
tags: Lists
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/7digital/apis.md
specificationVersion: "0.14"
apis:
- name: 7digital Playlist API playlists
  x-api-slug: 7digital-playlist-api
  description: Returns a list of all public playlists. If an oauth_token is provided
    then also given users private playlists will be included in the response.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/294-7digital.jpg
  humanURL: http://7digital.com
  baseURL: https://api.7digital.com/1.2//playlists
  tags: Playlists
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/7digital/playlists-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/7digital/playlists-get-openapi.md
- name: 7digital Playlist API playlists/{playlistId}
  x-api-slug: 7digital-playlist-api
  description: Deletes the playlist at {playlistId}. The playlist can only be deleted
    by its owner, i.e. oauth_token representing the user has to be provided.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/294-7digital.jpg
  humanURL: http://7digital.com
  baseURL: https://api.7digital.com/1.2//playlists/{playlistId}
  tags: Playlists
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/7digital/playlistsplaylistid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/7digital/playlistsplaylistid-delete-openapi.md
- name: 7digital Playlist API playlists/{playlistId}
  x-api-slug: 7digital-playlist-api
  description: Returns playlist details and track listing. Access to private playlists
    is only allowed when an oauth_token of the playlist owner is provided.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/294-7digital.jpg
  humanURL: http://7digital.com
  baseURL: https://api.7digital.com/1.2//playlists/{playlistId}
  tags: Playlists
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/7digital/playlistsplaylistid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/7digital/playlistsplaylistid-get-openapi.md
- name: 7digital Playlist API playlists/{playlistId}/details
  x-api-slug: 7digital-playlist-api
  description: Updates playlist details at {playlistId} with the supplied playlist
    details. It does not affect playlist tracks. Use this method e.g. for changing
    visibility of the playlist from private to public. The playlist details can only
    be updated by the playlist owner, i.e. oauth_token representing the user has to
    be provided.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/294-7digital.jpg
  humanURL: http://7digital.com
  baseURL: https://api.7digital.com/1.2//playlists/{playlistId}/details
  tags: Playlists,Details
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/7digital/playlistsplaylistiddetails-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/7digital/playlistsplaylistiddetails-post-openapi.md
- name: 7digital Playlist API playlists/{playlistId}/tracks/{playlisttrackid}
  x-api-slug: 7digital-playlist-api
  description: Removes the specified track {playlisttrackid} from the specified playlist
    at {playlistId}.  Tracks can only be removed by the playlist owner, i.e. oauth_token
    representing the user has to be provided.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/294-7digital.jpg
  humanURL: http://7digital.com
  baseURL: https://api.7digital.com/1.2//playlists/{playlistId}/tracks/{playlisttrackid}
  tags: Playlists,Tracks,Playlisttrackid
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/7digital/playlistsplaylistidtracksplaylisttrackid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/7digital/playlistsplaylistidtracksplaylisttrackid-delete-openapi.md
- name: 7digital Playlist API
  x-api-slug: 7digital-playlist-api
  description: Welcome to 7digital!    Choose from over 30 million high quality tracks
    in our store; download, sync and play your music on the go.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/294-7digital.jpg
  humanURL: http://7digital.com
  baseURL: https://api.7digital.com/1.2/
  tags: Lists
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/7digital/openapi.md
- name: 7digital Purchasing API playlists
  x-api-slug: 7digital-purchasing-api
  description: Returns a list of all public playlists. If an oauth_token is provided
    then also given users private playlists will be included in the response.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/294-7digital.jpg
  humanURL: http://7digital.com
  baseURL: https://api.7digital.com/1.2//playlists
  tags: Playlists
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/7digital/playlists-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/7digital/playlists-get-openapi.md
- name: 7digital Purchasing API playlists/{playlistId}
  x-api-slug: 7digital-purchasing-api
  description: Returns playlist details and track listing. Access to private playlists
    is only allowed when an oauth_token of the playlist owner is provided.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/294-7digital.jpg
  humanURL: http://7digital.com
  baseURL: https://api.7digital.com/1.2//playlists/{playlistId}
  tags: Playlists
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/7digital/playlistsplaylistid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/7digital/playlistsplaylistid-get-openapi.md
- name: 7digital Purchasing API playlists/{playlistId}/details
  x-api-slug: 7digital-purchasing-api
  description: Updates playlist details at {playlistId} with the supplied playlist
    details. It does not affect playlist tracks. Use this method e.g. for changing
    visibility of the playlist from private to public. The playlist details can only
    be updated by the playlist owner, i.e. oauth_token representing the user has to
    be provided.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/294-7digital.jpg
  humanURL: http://7digital.com
  baseURL: https://api.7digital.com/1.2//playlists/{playlistId}/details
  tags: Playlists,Details
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/7digital/playlistsplaylistiddetails-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/7digital/playlistsplaylistiddetails-post-openapi.md
- name: 7digital Purchasing API playlists/{playlistId}/tracks/{playlisttrackid}
  x-api-slug: 7digital-purchasing-api
  description: Removes the specified track {playlisttrackid} from the specified playlist
    at {playlistId}.  Tracks can only be removed by the playlist owner, i.e. oauth_token
    representing the user has to be provided.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/294-7digital.jpg
  humanURL: http://7digital.com
  baseURL: https://api.7digital.com/1.2//playlists/{playlistId}/tracks/{playlisttrackid}
  tags: Playlists,Tracks,Playlisttrackid
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/7digital/playlistsplaylistidtracksplaylisttrackid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/7digital/playlistsplaylistidtracksplaylisttrackid-delete-openapi.md
- name: 7digital Purchasing API
  x-api-slug: 7digital-purchasing-api
  description: The Purchasing API allows 3rd parties to deliver digital content to
    individual users.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/294-7digital.jpg
  humanURL: http://7digital.com
  baseURL: https://api.7digital.com/1.2/
  tags: Lists
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/7digital/openapi.md
x-common:
- type: x--net-sdk
  url: https://github.com/7digital/SevenDigital.Api.Wrapper
- type: x-android-sdk
  url: http://developer.7digital.com/7digital-android-sdk
- type: x-application-gallery
  url: http://developer.7digital.com/CaseStudies
- type: x-base
  url: http://api.7digital.com/
- type: x-blog
  url: http://developer.7digital.com/blog
- type: x-blog-rss
  url: http://blogs.7digital.com/dev/feed/
- type: x-crunchbase
  url: http://www.crunchbase.com/company/7digital
- type: x-crunchbase
  url: https://crunchbase.com/organization/7digital
- type: x-developer
  url: http://developer.7digital.net/
- type: x-email
  url: api@7digital.com
- type: x-email
  url: help@7digital.com
- type: x-email
  url: sales@7digital.com
- type: x-email
  url: legal@7digital.com
- type: x-email
  url: contention-queries@7digital.com
- type: x-github
  url: https://github.com/7digital
- type: x-ios-sdk
  url: https://github.com/7digital/7digital-iOS-SDK
- type: x-node-js-sdk
  url: https://github.com/raoulmillais/node-7digital-api
- type: x-php-sdk
  url: https://github.com/gquemener/7digital-client
- type: x-python-sdk
  url: https://github.com/jasonrubenstein/python-7Digital
- type: x-ruby-sdk
  url: http://github.com/filip7d/7digital
- type: x-selfservice-registration
  url: https://api-signup.7digital.com/
- type: x-twitter
  url: https://twitter.com/7digital
- type: x-website
  url: http://7digital.com
- type: x-website
  url: http://7digital.net/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---