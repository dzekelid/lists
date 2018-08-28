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
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/apis.md
specificationVersion: "0.14"
apis:
- name: Tasks - Add Lists Task List Clear
  x-api-slug: liststasklistclear-post
  description: Clears all completed tasks from the specified task list. The affected
    tasks will be marked as 'hidden' and no longer be returned by default when retrieving
    all tasks for a task list.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-tasks-icon.png
  humanURL: https://developers.google.com/google-apps/tasks/
  baseURL: ://www.googleapis.com//tasks/v1
  tags: Google APIs, Tasks, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/liststasklistclear-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/liststasklistclear-post-openapi.md
- name: Tasks - Get Lists Task List Tasks
  x-api-slug: liststasklisttasks-get
  description: Returns all tasks in the specified task list.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-tasks-icon.png
  humanURL: https://developers.google.com/google-apps/tasks/
  baseURL: ://www.googleapis.com//tasks/v1
  tags: Google APIs, Tasks, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/liststasklisttasks-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/liststasklisttasks-get-openapi.md
- name: Tasks - Add Lists Task List Tasks
  x-api-slug: liststasklisttasks-post
  description: Creates a new task on the specified task list.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-tasks-icon.png
  humanURL: https://developers.google.com/google-apps/tasks/
  baseURL: ://www.googleapis.com//tasks/v1
  tags: Google APIs, Tasks, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/liststasklisttasks-post-openapi.md
- name: Tasks - Delete Lists Task List Tasks Task
  x-api-slug: liststasklisttaskstask-delete
  description: Deletes the specified task from the task list.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-tasks-icon.png
  humanURL: https://developers.google.com/google-apps/tasks/
  baseURL: ://www.googleapis.com//tasks/v1
  tags: Google APIs, Tasks, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/liststasklisttaskstask-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/liststasklisttaskstask-delete-openapi.md
- name: Tasks - Get Lists Task List Tasks Task
  x-api-slug: liststasklisttaskstask-get
  description: Returns the specified task.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-tasks-icon.png
  humanURL: https://developers.google.com/google-apps/tasks/
  baseURL: ://www.googleapis.com//tasks/v1
  tags: Google APIs, Tasks, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/liststasklisttaskstask-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/liststasklisttaskstask-get-openapi.md
- name: Tasks - Patch Lists Task List Tasks Task
  x-api-slug: liststasklisttaskstask-patch
  description: Updates the specified task. This method supports patch semantics.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-tasks-icon.png
  humanURL: https://developers.google.com/google-apps/tasks/
  baseURL: ://www.googleapis.com//tasks/v1
  tags: Google APIs, Tasks, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/liststasklisttaskstask-patch-openapi.md
- name: Tasks - Put Lists Task List Tasks Task
  x-api-slug: liststasklisttaskstask-put
  description: Updates the specified task.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-tasks-icon.png
  humanURL: https://developers.google.com/google-apps/tasks/
  baseURL: ://www.googleapis.com//tasks/v1
  tags: Google APIs, Tasks, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/liststasklisttaskstask-put-openapi.md
- name: Tasks - Add Lists Task List Tasks Task Move
  x-api-slug: liststasklisttaskstaskmove-post
  description: Moves the specified task to another position in the task list. This
    can include putting it as a child task under a new parent and/or move it to a
    different position among its sibling tasks.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-tasks-icon.png
  humanURL: https://developers.google.com/google-apps/tasks/
  baseURL: ://www.googleapis.com//tasks/v1
  tags: Google APIs, Tasks, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/liststasklisttaskstaskmove-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/liststasklisttaskstaskmove-post-openapi.md
- name: Tasks - Get Users @me Lists
  x-api-slug: usersmelists-get
  description: Returns all the authenticated user's task lists.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-tasks-icon.png
  humanURL: https://developers.google.com/google-apps/tasks/
  baseURL: ://www.googleapis.com//tasks/v1
  tags: Google APIs, Tasks, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/usersmelists-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/usersmelists-get-openapi.md
- name: Tasks - Add Users @me Lists
  x-api-slug: usersmelists-post
  description: Creates a new task list and adds it to the authenticated user's task
    lists.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-tasks-icon.png
  humanURL: https://developers.google.com/google-apps/tasks/
  baseURL: ://www.googleapis.com//tasks/v1
  tags: Google APIs, Tasks, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/usersmelists-post-openapi.md
- name: Tasks - Add Lists Task List Clear
  x-api-slug: liststasklistclear-post
  description: Clears all completed tasks from the specified task list. The affected
    tasks will be marked as 'hidden' and no longer be returned by default when retrieving
    all tasks for a task list.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-tasks-icon.png
  humanURL: https://developers.google.com/google-apps/tasks/
  baseURL: ://www.googleapis.com//tasks/v1
  tags: Google APIs, Tasks, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/liststasklistclear-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/liststasklistclear-post-openapi.md
- name: Tasks - Get Lists Task List Tasks
  x-api-slug: liststasklisttasks-get
  description: Returns all tasks in the specified task list.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-tasks-icon.png
  humanURL: https://developers.google.com/google-apps/tasks/
  baseURL: ://www.googleapis.com//tasks/v1
  tags: Google APIs, Tasks, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/liststasklisttasks-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/liststasklisttasks-get-openapi.md
- name: Tasks - Add Lists Task List Tasks
  x-api-slug: liststasklisttasks-post
  description: Creates a new task on the specified task list.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-tasks-icon.png
  humanURL: https://developers.google.com/google-apps/tasks/
  baseURL: ://www.googleapis.com//tasks/v1
  tags: Google APIs, Tasks, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/liststasklisttasks-post-openapi.md
- name: Tasks - Delete Lists Task List Tasks Task
  x-api-slug: liststasklisttaskstask-delete
  description: Deletes the specified task from the task list.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-tasks-icon.png
  humanURL: https://developers.google.com/google-apps/tasks/
  baseURL: ://www.googleapis.com//tasks/v1
  tags: Google APIs, Tasks, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/liststasklisttaskstask-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/liststasklisttaskstask-delete-openapi.md
- name: Tasks - Get Lists Task List Tasks Task
  x-api-slug: liststasklisttaskstask-get
  description: Returns the specified task.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-tasks-icon.png
  humanURL: https://developers.google.com/google-apps/tasks/
  baseURL: ://www.googleapis.com//tasks/v1
  tags: Google APIs, Tasks, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/liststasklisttaskstask-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/liststasklisttaskstask-get-openapi.md
- name: Tasks - Patch Lists Task List Tasks Task
  x-api-slug: liststasklisttaskstask-patch
  description: Updates the specified task. This method supports patch semantics.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-tasks-icon.png
  humanURL: https://developers.google.com/google-apps/tasks/
  baseURL: ://www.googleapis.com//tasks/v1
  tags: Google APIs, Tasks, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/liststasklisttaskstask-patch-openapi.md
- name: Tasks - Put Lists Task List Tasks Task
  x-api-slug: liststasklisttaskstask-put
  description: Updates the specified task.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-tasks-icon.png
  humanURL: https://developers.google.com/google-apps/tasks/
  baseURL: ://www.googleapis.com//tasks/v1
  tags: Google APIs, Tasks, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/liststasklisttaskstask-put-openapi.md
- name: Tasks - Add Lists Task List Tasks Task Move
  x-api-slug: liststasklisttaskstaskmove-post
  description: Moves the specified task to another position in the task list. This
    can include putting it as a child task under a new parent and/or move it to a
    different position among its sibling tasks.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-tasks-icon.png
  humanURL: https://developers.google.com/google-apps/tasks/
  baseURL: ://www.googleapis.com//tasks/v1
  tags: Google APIs, Tasks, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/liststasklisttaskstaskmove-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/liststasklisttaskstaskmove-post-openapi.md
- name: Tasks - Delete Users Task List
  x-api-slug: usersmeliststasklist-delete
  description: Deletes the authenticated user's specified task list.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-tasks-icon.png
  humanURL: https://developers.google.com/google-apps/tasks/
  baseURL: ://www.googleapis.com//tasks/v1
  tags: Google APIs, Tasks, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/usersmeliststasklist-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/usersmeliststasklist-delete-openapi.md
- name: Tasks - Get Users Task List
  x-api-slug: usersmeliststasklist-get
  description: Returns the authenticated user's specified task list.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-tasks-icon.png
  humanURL: https://developers.google.com/google-apps/tasks/
  baseURL: ://www.googleapis.com//tasks/v1
  tags: Google APIs, Tasks, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/usersmeliststasklist-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/usersmeliststasklist-get-openapi.md
- name: Tasks - Patch Users Task List
  x-api-slug: usersmeliststasklist-patch
  description: Updates the authenticated user's specified task list. This method supports
    patch semantics.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-tasks-icon.png
  humanURL: https://developers.google.com/google-apps/tasks/
  baseURL: ://www.googleapis.com//tasks/v1
  tags: Google APIs, Tasks, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/usersmeliststasklist-patch-openapi.md
- name: Tasks - Put Users Task List
  x-api-slug: usersmeliststasklist-put
  description: Updates the authenticated user's specified task list.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-tasks-icon.png
  humanURL: https://developers.google.com/google-apps/tasks/
  baseURL: ://www.googleapis.com//tasks/v1
  tags: Google APIs, Tasks, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/usersmeliststasklist-put-openapi.md
- name: Tasks - Put Users Task List
  x-api-slug: usersmeliststasklist-put
  description: Updates the authenticated user's specified task list.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-tasks-icon.png
  humanURL: https://developers.google.com/google-apps/tasks/
  baseURL: ://www.googleapis.com//tasks/v1
  tags: Google APIs, Tasks, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/usersmeliststasklist-put-openapi.md
- name: Tasks - Put Users Task List
  x-api-slug: usersmeliststasklist-put
  description: Updates the authenticated user's specified task list.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-tasks-icon.png
  humanURL: https://developers.google.com/google-apps/tasks/
  baseURL: ://www.googleapis.com//tasks/v1
  tags: Google APIs, Tasks, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/usersmeliststasklist-put-openapi.md
- name: Tasks - Put Users Task List
  x-api-slug: usersmeliststasklist-put
  description: Updates the authenticated user's specified task list.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-tasks-icon.png
  humanURL: https://developers.google.com/google-apps/tasks/
  baseURL: ://www.googleapis.com//tasks/v1
  tags: Google APIs, Tasks, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/usersmeliststasklist-put-openapi.md
- name: Tasks - Patch Users Task List
  x-api-slug: usersmeliststasklist-patch
  description: Updates the authenticated user's specified task list. This method supports
    patch semantics.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-tasks-icon.png
  humanURL: https://developers.google.com/google-apps/tasks/
  baseURL: ://www.googleapis.com//tasks/v1
  tags: Google APIs, Tasks, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/usersmeliststasklist-patch-openapi.md
- name: Tasks - Put Users Task List
  x-api-slug: usersmeliststasklist-put
  description: Updates the authenticated user's specified task list.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-tasks-icon.png
  humanURL: https://developers.google.com/google-apps/tasks/
  baseURL: ://www.googleapis.com//tasks/v1
  tags: Google APIs, Tasks, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/usersmeliststasklist-put-openapi.md
- name: Tasks - Patch Users Task List
  x-api-slug: usersmeliststasklist-patch
  description: Updates the authenticated user's specified task list. This method supports
    patch semantics.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-tasks-icon.png
  humanURL: https://developers.google.com/google-apps/tasks/
  baseURL: ://www.googleapis.com//tasks/v1
  tags: Google APIs, Tasks, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/usersmeliststasklist-patch-openapi.md
- name: Tasks - Patch Users Task List
  x-api-slug: usersmeliststasklist-patch
  description: Updates the authenticated user's specified task list. This method supports
    patch semantics.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-tasks-icon.png
  humanURL: https://developers.google.com/google-apps/tasks/
  baseURL: ://www.googleapis.com//tasks/v1
  tags: Google APIs, Tasks, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/usersmeliststasklist-patch-openapi.md
- name: Tasks - Get Users Task List
  x-api-slug: usersmeliststasklist-get
  description: Returns the authenticated user's specified task list.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-tasks-icon.png
  humanURL: https://developers.google.com/google-apps/tasks/
  baseURL: ://www.googleapis.com//tasks/v1
  tags: Google APIs, Tasks, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/usersmeliststasklist-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/usersmeliststasklist-get-openapi.md
- name: Tasks - Patch Users Task List
  x-api-slug: usersmeliststasklist-patch
  description: Updates the authenticated user's specified task list. This method supports
    patch semantics.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-tasks-icon.png
  humanURL: https://developers.google.com/google-apps/tasks/
  baseURL: ://www.googleapis.com//tasks/v1
  tags: Google APIs, Tasks, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/usersmeliststasklist-patch-openapi.md
- name: Tasks - Get Users Task List
  x-api-slug: usersmeliststasklist-get
  description: Returns the authenticated user's specified task list.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-tasks-icon.png
  humanURL: https://developers.google.com/google-apps/tasks/
  baseURL: ://www.googleapis.com//tasks/v1
  tags: Google APIs, Tasks, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/usersmeliststasklist-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/usersmeliststasklist-get-openapi.md
- name: Tasks - Get Users Task List
  x-api-slug: usersmeliststasklist-get
  description: Returns the authenticated user's specified task list.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-tasks-icon.png
  humanURL: https://developers.google.com/google-apps/tasks/
  baseURL: ://www.googleapis.com//tasks/v1
  tags: Google APIs, Tasks, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/usersmeliststasklist-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/usersmeliststasklist-get-openapi.md
- name: Tasks - Delete Users Task List
  x-api-slug: usersmeliststasklist-delete
  description: Deletes the authenticated user's specified task list.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-tasks-icon.png
  humanURL: https://developers.google.com/google-apps/tasks/
  baseURL: ://www.googleapis.com//tasks/v1
  tags: Google APIs, Tasks, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/usersmeliststasklist-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/usersmeliststasklist-delete-openapi.md
- name: Tasks - Get Users Task List
  x-api-slug: usersmeliststasklist-get
  description: Returns the authenticated user's specified task list.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-tasks-icon.png
  humanURL: https://developers.google.com/google-apps/tasks/
  baseURL: ://www.googleapis.com//tasks/v1
  tags: Google APIs, Tasks, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/usersmeliststasklist-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/usersmeliststasklist-get-openapi.md
- name: Tasks - Delete Users Task List
  x-api-slug: usersmeliststasklist-delete
  description: Deletes the authenticated user's specified task list.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-tasks-icon.png
  humanURL: https://developers.google.com/google-apps/tasks/
  baseURL: ://www.googleapis.com//tasks/v1
  tags: Google APIs, Tasks, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/usersmeliststasklist-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/usersmeliststasklist-delete-openapi.md
- name: Tasks - Delete Users Task List
  x-api-slug: usersmeliststasklist-delete
  description: Deletes the authenticated user's specified task list.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-tasks-icon.png
  humanURL: https://developers.google.com/google-apps/tasks/
  baseURL: ://www.googleapis.com//tasks/v1
  tags: Google APIs, Tasks, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/usersmeliststasklist-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/usersmeliststasklist-delete-openapi.md
- name: Tasks - Add Lists Task List Tasks Task Move
  x-api-slug: liststasklisttaskstaskmove-post
  description: Moves the specified task to another position in the task list. This
    can include putting it as a child task under a new parent and/or move it to a
    different position among its sibling tasks.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-tasks-icon.png
  humanURL: https://developers.google.com/google-apps/tasks/
  baseURL: ://www.googleapis.com//tasks/v1
  tags: Google APIs, Tasks, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/liststasklisttaskstaskmove-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/liststasklisttaskstaskmove-post-openapi.md
- name: Tasks - Delete Users Task List
  x-api-slug: usersmeliststasklist-delete
  description: Deletes the authenticated user's specified task list.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-tasks-icon.png
  humanURL: https://developers.google.com/google-apps/tasks/
  baseURL: ://www.googleapis.com//tasks/v1
  tags: Google APIs, Tasks, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/usersmeliststasklist-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/usersmeliststasklist-delete-openapi.md
- name: Tasks - Add Lists Task List Tasks Task Move
  x-api-slug: liststasklisttaskstaskmove-post
  description: Moves the specified task to another position in the task list. This
    can include putting it as a child task under a new parent and/or move it to a
    different position among its sibling tasks.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-tasks-icon.png
  humanURL: https://developers.google.com/google-apps/tasks/
  baseURL: ://www.googleapis.com//tasks/v1
  tags: Google APIs, Tasks, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/liststasklisttaskstaskmove-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/liststasklisttaskstaskmove-post-openapi.md
- name: Tasks - Add Lists Task List Tasks Task Move
  x-api-slug: liststasklisttaskstaskmove-post
  description: Moves the specified task to another position in the task list. This
    can include putting it as a child task under a new parent and/or move it to a
    different position among its sibling tasks.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-tasks-icon.png
  humanURL: https://developers.google.com/google-apps/tasks/
  baseURL: ://www.googleapis.com//tasks/v1
  tags: Google APIs, Tasks, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/liststasklisttaskstaskmove-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/liststasklisttaskstaskmove-post-openapi.md
- name: Tasks - Put Lists Task List Tasks Task
  x-api-slug: liststasklisttaskstask-put
  description: Updates the specified task.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-tasks-icon.png
  humanURL: https://developers.google.com/google-apps/tasks/
  baseURL: ://www.googleapis.com//tasks/v1
  tags: Google APIs, Tasks, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/liststasklisttaskstask-put-openapi.md
- name: Tasks - Add Lists Task List Tasks Task Move
  x-api-slug: liststasklisttaskstaskmove-post
  description: Moves the specified task to another position in the task list. This
    can include putting it as a child task under a new parent and/or move it to a
    different position among its sibling tasks.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-tasks-icon.png
  humanURL: https://developers.google.com/google-apps/tasks/
  baseURL: ://www.googleapis.com//tasks/v1
  tags: Google APIs, Tasks, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/liststasklisttaskstaskmove-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/liststasklisttaskstaskmove-post-openapi.md
- name: Tasks - Put Lists Task List Tasks Task
  x-api-slug: liststasklisttaskstask-put
  description: Updates the specified task.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-tasks-icon.png
  humanURL: https://developers.google.com/google-apps/tasks/
  baseURL: ://www.googleapis.com//tasks/v1
  tags: Google APIs, Tasks, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/liststasklisttaskstask-put-openapi.md
- name: Tasks - Put Lists Task List Tasks Task
  x-api-slug: liststasklisttaskstask-put
  description: Updates the specified task.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-tasks-icon.png
  humanURL: https://developers.google.com/google-apps/tasks/
  baseURL: ://www.googleapis.com//tasks/v1
  tags: Google APIs, Tasks, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/liststasklisttaskstask-put-openapi.md
- name: Tasks - Patch Lists Task List Tasks Task
  x-api-slug: liststasklisttaskstask-patch
  description: Updates the specified task. This method supports patch semantics.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-tasks-icon.png
  humanURL: https://developers.google.com/google-apps/tasks/
  baseURL: ://www.googleapis.com//tasks/v1
  tags: Google APIs, Tasks, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/liststasklisttaskstask-patch-openapi.md
- name: Tasks - Put Lists Task List Tasks Task
  x-api-slug: liststasklisttaskstask-put
  description: Updates the specified task.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-tasks-icon.png
  humanURL: https://developers.google.com/google-apps/tasks/
  baseURL: ://www.googleapis.com//tasks/v1
  tags: Google APIs, Tasks, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/liststasklisttaskstask-put-openapi.md
- name: Tasks - Patch Lists Task List Tasks Task
  x-api-slug: liststasklisttaskstask-patch
  description: Updates the specified task. This method supports patch semantics.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-tasks-icon.png
  humanURL: https://developers.google.com/google-apps/tasks/
  baseURL: ://www.googleapis.com//tasks/v1
  tags: Google APIs, Tasks, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/liststasklisttaskstask-patch-openapi.md
- name: Tasks - Patch Lists Task List Tasks Task
  x-api-slug: liststasklisttaskstask-patch
  description: Updates the specified task. This method supports patch semantics.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-tasks-icon.png
  humanURL: https://developers.google.com/google-apps/tasks/
  baseURL: ://www.googleapis.com//tasks/v1
  tags: Google APIs, Tasks, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/liststasklisttaskstask-patch-openapi.md
- name: Tasks - Get Lists Task List Tasks Task
  x-api-slug: liststasklisttaskstask-get
  description: Returns the specified task.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-tasks-icon.png
  humanURL: https://developers.google.com/google-apps/tasks/
  baseURL: ://www.googleapis.com//tasks/v1
  tags: Google APIs, Tasks, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/liststasklisttaskstask-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/liststasklisttaskstask-get-openapi.md
- name: Tasks - Patch Lists Task List Tasks Task
  x-api-slug: liststasklisttaskstask-patch
  description: Updates the specified task. This method supports patch semantics.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-tasks-icon.png
  humanURL: https://developers.google.com/google-apps/tasks/
  baseURL: ://www.googleapis.com//tasks/v1
  tags: Google APIs, Tasks, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/liststasklisttaskstask-patch-openapi.md
- name: Tasks - Get Lists Task List Tasks Task
  x-api-slug: liststasklisttaskstask-get
  description: Returns the specified task.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-tasks-icon.png
  humanURL: https://developers.google.com/google-apps/tasks/
  baseURL: ://www.googleapis.com//tasks/v1
  tags: Google APIs, Tasks, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/liststasklisttaskstask-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/liststasklisttaskstask-get-openapi.md
- name: Tasks - Get Lists Task List Tasks Task
  x-api-slug: liststasklisttaskstask-get
  description: Returns the specified task.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-tasks-icon.png
  humanURL: https://developers.google.com/google-apps/tasks/
  baseURL: ://www.googleapis.com//tasks/v1
  tags: Google APIs, Tasks, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/liststasklisttaskstask-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/liststasklisttaskstask-get-openapi.md
- name: Tasks - Delete Lists Task List Tasks Task
  x-api-slug: liststasklisttaskstask-delete
  description: Deletes the specified task from the task list.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-tasks-icon.png
  humanURL: https://developers.google.com/google-apps/tasks/
  baseURL: ://www.googleapis.com//tasks/v1
  tags: Google APIs, Tasks, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/liststasklisttaskstask-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/liststasklisttaskstask-delete-openapi.md
- name: Tasks - Get Lists Task List Tasks Task
  x-api-slug: liststasklisttaskstask-get
  description: Returns the specified task.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-tasks-icon.png
  humanURL: https://developers.google.com/google-apps/tasks/
  baseURL: ://www.googleapis.com//tasks/v1
  tags: Google APIs, Tasks, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/liststasklisttaskstask-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/liststasklisttaskstask-get-openapi.md
- name: Tasks - Delete Lists Task List Tasks Task
  x-api-slug: liststasklisttaskstask-delete
  description: Deletes the specified task from the task list.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-tasks-icon.png
  humanURL: https://developers.google.com/google-apps/tasks/
  baseURL: ://www.googleapis.com//tasks/v1
  tags: Google APIs, Tasks, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/liststasklisttaskstask-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/liststasklisttaskstask-delete-openapi.md
- name: Tasks - Delete Lists Task List Tasks Task
  x-api-slug: liststasklisttaskstask-delete
  description: Deletes the specified task from the task list.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-tasks-icon.png
  humanURL: https://developers.google.com/google-apps/tasks/
  baseURL: ://www.googleapis.com//tasks/v1
  tags: Google APIs, Tasks, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/liststasklisttaskstask-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/liststasklisttaskstask-delete-openapi.md
- name: Tasks - Add Lists Task List Tasks
  x-api-slug: liststasklisttasks-post
  description: Creates a new task on the specified task list.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-tasks-icon.png
  humanURL: https://developers.google.com/google-apps/tasks/
  baseURL: ://www.googleapis.com//tasks/v1
  tags: Google APIs, Tasks, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/liststasklisttasks-post-openapi.md
- name: Tasks - Delete Lists Task List Tasks Task
  x-api-slug: liststasklisttaskstask-delete
  description: Deletes the specified task from the task list.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-tasks-icon.png
  humanURL: https://developers.google.com/google-apps/tasks/
  baseURL: ://www.googleapis.com//tasks/v1
  tags: Google APIs, Tasks, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/liststasklisttaskstask-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/liststasklisttaskstask-delete-openapi.md
- name: Tasks - Add Lists Task List Tasks
  x-api-slug: liststasklisttasks-post
  description: Creates a new task on the specified task list.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-tasks-icon.png
  humanURL: https://developers.google.com/google-apps/tasks/
  baseURL: ://www.googleapis.com//tasks/v1
  tags: Google APIs, Tasks, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/liststasklisttasks-post-openapi.md
- name: Tasks - Add Lists Task List Tasks
  x-api-slug: liststasklisttasks-post
  description: Creates a new task on the specified task list.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-tasks-icon.png
  humanURL: https://developers.google.com/google-apps/tasks/
  baseURL: ://www.googleapis.com//tasks/v1
  tags: Google APIs, Tasks, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/liststasklisttasks-post-openapi.md
- name: Tasks - Get Lists Task List Tasks
  x-api-slug: liststasklisttasks-get
  description: Returns all tasks in the specified task list.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-tasks-icon.png
  humanURL: https://developers.google.com/google-apps/tasks/
  baseURL: ://www.googleapis.com//tasks/v1
  tags: Google APIs, Tasks, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/liststasklisttasks-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/liststasklisttasks-get-openapi.md
- name: Tasks - Add Lists Task List Tasks
  x-api-slug: liststasklisttasks-post
  description: Creates a new task on the specified task list.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-tasks-icon.png
  humanURL: https://developers.google.com/google-apps/tasks/
  baseURL: ://www.googleapis.com//tasks/v1
  tags: Google APIs, Tasks, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/liststasklisttasks-post-openapi.md
- name: Tasks - Get Lists Task List Tasks
  x-api-slug: liststasklisttasks-get
  description: Returns all tasks in the specified task list.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-tasks-icon.png
  humanURL: https://developers.google.com/google-apps/tasks/
  baseURL: ://www.googleapis.com//tasks/v1
  tags: Google APIs, Tasks, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/liststasklisttasks-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/liststasklisttasks-get-openapi.md
- name: Tasks - Get Lists Task List Tasks
  x-api-slug: liststasklisttasks-get
  description: Returns all tasks in the specified task list.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-tasks-icon.png
  humanURL: https://developers.google.com/google-apps/tasks/
  baseURL: ://www.googleapis.com//tasks/v1
  tags: Google APIs, Tasks, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/liststasklisttasks-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/liststasklisttasks-get-openapi.md
- name: Tasks - Add Lists Task List Clear
  x-api-slug: liststasklistclear-post
  description: Clears all completed tasks from the specified task list. The affected
    tasks will be marked as 'hidden' and no longer be returned by default when retrieving
    all tasks for a task list.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-tasks-icon.png
  humanURL: https://developers.google.com/google-apps/tasks/
  baseURL: ://www.googleapis.com//tasks/v1
  tags: Google APIs, Tasks, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/liststasklistclear-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/liststasklistclear-post-openapi.md
- name: Tasks - Get Lists Task List Tasks
  x-api-slug: liststasklisttasks-get
  description: Returns all tasks in the specified task list.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-tasks-icon.png
  humanURL: https://developers.google.com/google-apps/tasks/
  baseURL: ://www.googleapis.com//tasks/v1
  tags: Google APIs, Tasks, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/liststasklisttasks-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/liststasklisttasks-get-openapi.md
- name: Tasks - Add Lists Task List Clear
  x-api-slug: liststasklistclear-post
  description: Clears all completed tasks from the specified task list. The affected
    tasks will be marked as 'hidden' and no longer be returned by default when retrieving
    all tasks for a task list.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-tasks-icon.png
  humanURL: https://developers.google.com/google-apps/tasks/
  baseURL: ://www.googleapis.com//tasks/v1
  tags: Google APIs, Tasks, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/liststasklistclear-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/liststasklistclear-post-openapi.md
- name: Tasks - Add Lists Task List Clear
  x-api-slug: liststasklistclear-post
  description: Clears all completed tasks from the specified task list. The affected
    tasks will be marked as 'hidden' and no longer be returned by default when retrieving
    all tasks for a task list.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-tasks-icon.png
  humanURL: https://developers.google.com/google-apps/tasks/
  baseURL: ://www.googleapis.com//tasks/v1
  tags: Google APIs, Tasks, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/liststasklistclear-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/liststasklistclear-post-openapi.md
- name: Tasks - Add Lists Task List Clear
  x-api-slug: liststasklistclear-post
  description: Clears all completed tasks from the specified task list. The affected
    tasks will be marked as 'hidden' and no longer be returned by default when retrieving
    all tasks for a task list.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/google-tasks-icon.png
  humanURL: https://developers.google.com/google-apps/tasks/
  baseURL: ://www.googleapis.com//tasks/v1
  tags: Google APIs, Tasks, Stack Network, API Service Provider, API Provider, Profiles,
    Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/liststasklistclear-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/google-tasks/liststasklistclear-post-openapi.md
x-common:
- type: x-api-gallery
  url: http://google.task.queue.api.gallery.streamdata.io
- type: x-api-stack
  url: http://google.tasks.stack.network
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