---
name: Google Tasks
x-slug: google-tasks
description: The Google Tasks API lets you search, read, and update Google Tasks content
  and metadata. This document describes how to use a RESTful calling style and client
  libraries for various programming languages (currently Java, Python, and PHP) to
  access and edit Google Tasks data.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-tasks-icon.png
x-kinRank: "9"
x-alexaRank: "0"
tags: Lists
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/apis.md
specificationVersion: "0.14"
apis:
- name: Google Tasks API Add Lists Task List Clear
  x-api-slug: google-tasks-api
  description: Clears all completed tasks from the specified task list. The affected
    tasks will be marked as 'hidden' and no longer be returned by default when retrieving
    all tasks for a task list.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-tasks-icon.png
  humanURL: https://developers.google.com/google-apps/tasks/
  baseURL: ://www.googleapis.com//tasks/v1//lists/{tasklist}/clear
  tags: Lists, Task, List, Clear
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/liststasklistclear-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/liststasklistclear-post-openapi.md
- name: Google Tasks API Get Lists Task List Tasks
  x-api-slug: google-tasks-api
  description: Returns all tasks in the specified task list.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-tasks-icon.png
  humanURL: https://developers.google.com/google-apps/tasks/
  baseURL: ://www.googleapis.com//tasks/v1//lists/{tasklist}/tasks
  tags: Lists, Task, List, Tasks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/liststasklisttasks-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/liststasklisttasks-get-openapi.md
- name: Google Tasks API Add Lists Task List Tasks
  x-api-slug: google-tasks-api
  description: Creates a new task on the specified task list.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-tasks-icon.png
  humanURL: https://developers.google.com/google-apps/tasks/
  baseURL: ://www.googleapis.com//tasks/v1//lists/{tasklist}/tasks
  tags: Lists, Task, List, Tasks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/liststasklisttasks-post-openapi.md
- name: Google Tasks API Delete Lists Task List Tasks Task
  x-api-slug: google-tasks-api
  description: Deletes the specified task from the task list.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-tasks-icon.png
  humanURL: https://developers.google.com/google-apps/tasks/
  baseURL: ://www.googleapis.com//tasks/v1//lists/{tasklist}/tasks/{task}
  tags: Lists, Task, List, Tasks, Task
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/liststasklisttaskstask-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/liststasklisttaskstask-delete-openapi.md
- name: Google Tasks API Get Lists Task List Tasks Task
  x-api-slug: google-tasks-api
  description: Returns the specified task.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-tasks-icon.png
  humanURL: https://developers.google.com/google-apps/tasks/
  baseURL: ://www.googleapis.com//tasks/v1//lists/{tasklist}/tasks/{task}
  tags: Lists, Task, List, Tasks, Task
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/liststasklisttaskstask-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/liststasklisttaskstask-get-openapi.md
- name: Google Tasks API Patch Lists Task List Tasks Task
  x-api-slug: google-tasks-api
  description: Updates the specified task. This method supports patch semantics.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-tasks-icon.png
  humanURL: https://developers.google.com/google-apps/tasks/
  baseURL: ://www.googleapis.com//tasks/v1//lists/{tasklist}/tasks/{task}
  tags: Lists, Task, List, Tasks, Task
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/liststasklisttaskstask-patch-openapi.md
- name: Google Tasks API Put Lists Task List Tasks Task
  x-api-slug: google-tasks-api
  description: Updates the specified task.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-tasks-icon.png
  humanURL: https://developers.google.com/google-apps/tasks/
  baseURL: ://www.googleapis.com//tasks/v1//lists/{tasklist}/tasks/{task}
  tags: Lists, Task, List, Tasks, Task
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/liststasklisttaskstask-put-openapi.md
- name: Google Tasks API Add Lists Task List Tasks Task Move
  x-api-slug: google-tasks-api
  description: Moves the specified task to another position in the task list. This
    can include putting it as a child task under a new parent and/or move it to a
    different position among its sibling tasks.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-tasks-icon.png
  humanURL: https://developers.google.com/google-apps/tasks/
  baseURL: ://www.googleapis.com//tasks/v1//lists/{tasklist}/tasks/{task}/move
  tags: Lists, Task, List, Tasks, Task, Move
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/liststasklisttaskstaskmove-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/liststasklisttaskstaskmove-post-openapi.md
- name: Google Tasks API Get Users @me Lists
  x-api-slug: google-tasks-api
  description: Returns all the authenticated user's task lists.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-tasks-icon.png
  humanURL: https://developers.google.com/google-apps/tasks/
  baseURL: ://www.googleapis.com//tasks/v1//users/@me/lists
  tags: Users, @me, Lists
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/usersmelists-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/usersmelists-get-openapi.md
- name: Google Tasks API Add Users @me Lists
  x-api-slug: google-tasks-api
  description: Creates a new task list and adds it to the authenticated user's task
    lists.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-tasks-icon.png
  humanURL: https://developers.google.com/google-apps/tasks/
  baseURL: ://www.googleapis.com//tasks/v1//users/@me/lists
  tags: Users, @me, Lists
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/usersmelists-post-openapi.md
- name: Google Tasks API
  x-api-slug: google-tasks-api
  description: The Google Tasks API lets you search, read, and update Google Tasks
    content and metadata. This document describes how to use a RESTful calling style
    and client libraries for various programming languages (currently Java, Python,
    and PHP) to access and edit Google Tasks data.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-tasks-icon.png
  humanURL: https://developers.google.com/google-apps/tasks/
  baseURL: ://www.googleapis.com//tasks/v1
  tags: Lists
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/openapi.md
x-common:
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