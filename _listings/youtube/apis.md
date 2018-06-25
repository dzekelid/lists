---
name: YouTube
x-slug: youtube
description: Enjoy the videos and music you love, upload original content, and share
  it all with friends, family, and the world on YouTube.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11515-youtube.jpg
x-kinRank: "9"
x-alexaRank: "2"
tags: Lists
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/youtube/apis.md
specificationVersion: "0.14"
apis:
- name: Youtube Delete Playlists
  x-api-slug: youtube
  description: Deletes a playlist.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11515-youtube.jpg
  humanURL: https://www.youtube.com/
  baseURL: https://www.googleapis.com//youtube/v1//playlists
  tags: Playlists
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/youtube/playlists-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/youtube/playlists-delete-openapi.md
- name: Youtube Get Playlists
  x-api-slug: youtube
  description: Returns a collection of playlists that match the API request parameters.
    For example, you can retrieve all playlists that the authenticated user owns,
    or you can retrieve one or more playlists by their unique IDs.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11515-youtube.jpg
  humanURL: https://www.youtube.com/
  baseURL: https://www.googleapis.com//youtube/v1//playlists
  tags: Playlists
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/youtube/playlists-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/youtube/playlists-get-openapi.md
- name: Youtube Add Playlists
  x-api-slug: youtube
  description: Creates a playlist.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11515-youtube.jpg
  humanURL: https://www.youtube.com/
  baseURL: https://www.googleapis.com//youtube/v1//playlists
  tags: Playlists
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/youtube/playlists-post-openapi.md
- name: Youtube Put Playlists
  x-api-slug: youtube
  description: Modifies a playlist. For example, you could change a playlist's title,
    description, or privacy status.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11515-youtube.jpg
  humanURL: https://www.youtube.com/
  baseURL: https://www.googleapis.com//youtube/v1//playlists
  tags: Playlists
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/youtube/playlists-put-openapi.md
- name: Youtube
  x-api-slug: youtube
  description: Enjoy the videos and music you love, upload original content, and share
    it all with friends, family, and the world on YouTube.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11515-youtube.jpg
  humanURL: https://www.youtube.com/
  baseURL: https://www.googleapis.com//youtube/v1
  tags: Lists
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/youtube/openapi.md
x-common:
- type: x-articles
  url: https://developers.google.com/youtube/articles/
- type: x-authentication
  url: https://developers.google.com/youtube/v3/guides/authentication
- type: x-blog
  url: https://youtube-eng.googleblog.com/
- type: x-blog-rss
  url: https://youtube-eng.googleblog.com/feeds/posts/default?alt=rss
- type: x-branding
  url: https://developers.google.com/youtube/branding_guidelines
- type: x-bug-report
  url: https://code.google.com/p/gdata-issues/issues/entry
- type: x-bug-report
  url: https://code.google.com/p/gdata-issues/issues/list?q=label:API-YouTube
- type: x-buttons
  url: https://developers.google.com/youtube/youtube_subscribe_button
- type: x-crunchbase
  url: https://crunchbase.com/organization/youtube
- type: x-deprecation-policy
  url: https://developers.google.com/youtube/youtube-api-list
- type: x-developer
  url: https://developers.google.com/youtube/
- type: x-email
  url: copyright@youtube.com
- type: x-getting-started
  url: https://developers.google.com/youtube/v3/getting-started
- type: x-github
  url: https://github.com/youtube
- type: x-github
  url: https://github.com/youtube/
- type: x-terms-of-service
  url: https://developers.google.com/youtube/terms
- type: x-training
  url: https://developers.google.com/youtube/training/
- type: x-twitter
  url: https://twitter.com/YouTubeDev
- type: x-twitter
  url: https://twitter.com/YouTube
- type: x-website
  url: https://www.youtube.com/
- type: x-widgets
  url: https://developers.google.com/youtube/youtube_upload_widget
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---