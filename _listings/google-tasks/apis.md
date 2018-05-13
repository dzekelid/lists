---
name: Google Tasks
description: The Google Tasks API lets you search, read, and update Google Tasks content
  and metadata. This document describes how to use a RESTful calling style and client
  libraries for various programming languages (currently Java, Python, and PHP) to
  access and edit Google Tasks data.
image: ""
x-kinRank: "9"
x-alexaRank: ""
tags:
- Tasks
- Stack Network
- Google APIs
created: "2018-03-23"
modified: "2018-03-23"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/apis.yaml
specificationVersion: "0.14"
apis:
- name: Google Tasks API
  description: The Google Tasks API lets you search, read, and update Google Tasks
    content and metadata
  image: ""
  humanURL: ""
  baseURL: ://www.googleapis.com//tasks/v1
  tags: Lists
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/users-me-lists-post.md
- name: Google Tasks API Add Lists Task List Tasks Task Move
  description: Moves the specified task to another position in the task list. This
    can include putting it as a child task under a new parent and/or move it to a
    different position among its sibling tasks.
  image: ""
  humanURL: https://developers.google.com/google-apps/tasks/
  baseURL: http:://www.googleapis.com//tasks/v1
  tags: Lists
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/lists-tasklist-tasks-task-move-post.md
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/lists-tasklist-tasks-task-move-post-postman.md
x-common:
- type: x-code
  url: https://developers.google.com/google-apps/tasks/setup
- type: x-concepts
  url: https://developers.google.com/google-apps/tasks/concepts
- type: x-documentation
  url: https://developers.google.com/google-apps/tasks/v1/reference/
- type: x-website
  url: https://developers.google.com/google-apps/tasks/
- type: x-code
  url: https://developers.google.com/google-apps/tasks/setup
- type: x-concepts
  url: https://developers.google.com/google-apps/tasks/concepts
- type: x-documentation
  url: https://developers.google.com/google-apps/tasks/v1/reference/
- type: x-website
  url: https://developers.google.com/google-apps/tasks/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---