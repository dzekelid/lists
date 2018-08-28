---
name: Mattermost
x-slug: mattermost
description: Open source, private cloud Slack-alternative, Workplace messaging for
  web, PCs and phones. MIT-licensed. Hundreds of contributors. 14 languages. Secure,
  configurable, and scalable from teams to the enterprise.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
x-kinRank: "8"
x-alexaRank: "95684"
tags: Lists
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mattermost/apis.md
specificationVersion: "0.14"
apis:
- name: Mattermost API Reference - Get a list of channels by ids
  x-api-slug: teamsteam-idchannelsids-post
  description: |-
    Get a list of public channels on a team by id.
    ##### Permissions
    `view_team` for the team the channels are on.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mattermost/teamsteam-idchannelsids-post-openapi.md
- name: Mattermost API Reference - Get a list of flagged posts
  x-api-slug: usersuser-idpostsflagged-get
  description: |-
    Get a page of flagged posts of a user provided user id string. Selects from a channel, team or all flagged posts by a user.
    ##### Permissions
    Must be user or have `manage_system` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mattermost/usersuser-idpostsflagged-get-openapi.md
- name: Mattermost API Reference - List a user's preferences by category
  x-api-slug: usersuser-idpreferencescategory-get
  description: |-
    Lists the current user's stored preferences in the given category.
    ##### Permissions
    Must be logged in as the user being updated or have the `edit_other_users` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mattermost/usersuser-idpreferencescategory-get-openapi.md
- name: Mattermost API Reference - Get a list of custom emoji
  x-api-slug: emoji-get
  description: |-
    Get a page of metadata for custom emoji on the system. Since server version 4.7, sort using the `sort` query parameter.
    ##### Permissions
    Must be authenticated.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mattermost/emoji-get-openapi.md
- name: Mattermost API Reference - List incoming webhooks
  x-api-slug: hooksincoming-get
  description: |-
    Get a page of a list of incoming webhooks. Optionally filter for a specific team using query parameters.
    ##### Permissions
    `manage_webhooks` for the system or `manage_webhooks` for the specific team.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mattermost/hooksincoming-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mattermost/hooksincoming-get-openapi.md
- name: Mattermost API Reference - List outgoing webhooks
  x-api-slug: hooksoutgoing-get
  description: |-
    Get a page of a list of outgoing webhooks. Optionally filter for a specific team or channel using query parameters.
    ##### Permissions
    `manage_webhooks` for the system or `manage_webhooks` for the specific team/channel.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mattermost/hooksoutgoing-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mattermost/hooksoutgoing-get-openapi.md
- name: Mattermost API Reference - List commands for a team
  x-api-slug: commands-get
  description: |-
    List commands for a team.
    ##### Permissions
    `manage_slash_commands` if need list custom commands.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mattermost/commands-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mattermost/commands-get-openapi.md
- name: Mattermost API Reference - List autocomplete commands
  x-api-slug: teamsteam-idcommandsautocomplete-get
  description: |-
    List autocomplete commands in the team.
    ##### Permissions
    `view_team` for the team.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mattermost/teamsteam-idcommandsautocomplete-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mattermost/teamsteam-idcommandsautocomplete-get-openapi.md
- name: Mattermost API Reference - Get a list of roles by name
  x-api-slug: rolesnames-post
  description: |-
    Get a list of roles from their names.

    ##### Permissions
    Requires an active session but no other permissions.

    __Minimum server version__: 4.9
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mattermost/rolesnames-post-openapi.md
- name: Mattermost API Reference - Get a list of roles by name
  x-api-slug: rolesnames-post
  description: |-
    Get a list of roles from their names.

    ##### Permissions
    Requires an active session but no other permissions.

    __Minimum server version__: 4.9
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mattermost/rolesnames-post-openapi.md
- name: Mattermost API Reference - Get a list of roles by name
  x-api-slug: rolesnames-post
  description: |-
    Get a list of roles from their names.

    ##### Permissions
    Requires an active session but no other permissions.

    __Minimum server version__: 4.9
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mattermost/rolesnames-post-openapi.md
- name: Mattermost API Reference - List autocomplete commands
  x-api-slug: teamsteam-idcommandsautocomplete-get
  description: |-
    List autocomplete commands in the team.
    ##### Permissions
    `view_team` for the team.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mattermost/teamsteam-idcommandsautocomplete-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mattermost/teamsteam-idcommandsautocomplete-get-openapi.md
- name: Mattermost API Reference - Get a list of roles by name
  x-api-slug: rolesnames-post
  description: |-
    Get a list of roles from their names.

    ##### Permissions
    Requires an active session but no other permissions.

    __Minimum server version__: 4.9
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mattermost/rolesnames-post-openapi.md
- name: Mattermost API Reference - List autocomplete commands
  x-api-slug: teamsteam-idcommandsautocomplete-get
  description: |-
    List autocomplete commands in the team.
    ##### Permissions
    `view_team` for the team.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mattermost/teamsteam-idcommandsautocomplete-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mattermost/teamsteam-idcommandsautocomplete-get-openapi.md
- name: Mattermost API Reference - List commands for a team
  x-api-slug: commands-get
  description: |-
    List commands for a team.
    ##### Permissions
    `manage_slash_commands` if need list custom commands.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mattermost/commands-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mattermost/commands-get-openapi.md
- name: Mattermost API Reference - List autocomplete commands
  x-api-slug: teamsteam-idcommandsautocomplete-get
  description: |-
    List autocomplete commands in the team.
    ##### Permissions
    `view_team` for the team.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mattermost/teamsteam-idcommandsautocomplete-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mattermost/teamsteam-idcommandsautocomplete-get-openapi.md
- name: Mattermost API Reference - List commands for a team
  x-api-slug: commands-get
  description: |-
    List commands for a team.
    ##### Permissions
    `manage_slash_commands` if need list custom commands.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mattermost/commands-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mattermost/commands-get-openapi.md
- name: Mattermost API Reference - List outgoing webhooks
  x-api-slug: hooksoutgoing-get
  description: |-
    Get a page of a list of outgoing webhooks. Optionally filter for a specific team or channel using query parameters.
    ##### Permissions
    `manage_webhooks` for the system or `manage_webhooks` for the specific team/channel.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mattermost/hooksoutgoing-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mattermost/hooksoutgoing-get-openapi.md
- name: Mattermost API Reference - List commands for a team
  x-api-slug: commands-get
  description: |-
    List commands for a team.
    ##### Permissions
    `manage_slash_commands` if need list custom commands.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mattermost/commands-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mattermost/commands-get-openapi.md
- name: Mattermost API Reference - List outgoing webhooks
  x-api-slug: hooksoutgoing-get
  description: |-
    Get a page of a list of outgoing webhooks. Optionally filter for a specific team or channel using query parameters.
    ##### Permissions
    `manage_webhooks` for the system or `manage_webhooks` for the specific team/channel.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mattermost/hooksoutgoing-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mattermost/hooksoutgoing-get-openapi.md
- name: Mattermost API Reference - List incoming webhooks
  x-api-slug: hooksincoming-get
  description: |-
    Get a page of a list of incoming webhooks. Optionally filter for a specific team using query parameters.
    ##### Permissions
    `manage_webhooks` for the system or `manage_webhooks` for the specific team.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mattermost/hooksincoming-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mattermost/hooksincoming-get-openapi.md
- name: Mattermost API Reference - List outgoing webhooks
  x-api-slug: hooksoutgoing-get
  description: |-
    Get a page of a list of outgoing webhooks. Optionally filter for a specific team or channel using query parameters.
    ##### Permissions
    `manage_webhooks` for the system or `manage_webhooks` for the specific team/channel.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mattermost/hooksoutgoing-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mattermost/hooksoutgoing-get-openapi.md
- name: Mattermost API Reference - List incoming webhooks
  x-api-slug: hooksincoming-get
  description: |-
    Get a page of a list of incoming webhooks. Optionally filter for a specific team using query parameters.
    ##### Permissions
    `manage_webhooks` for the system or `manage_webhooks` for the specific team.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mattermost/hooksincoming-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mattermost/hooksincoming-get-openapi.md
- name: Mattermost API Reference - Get a list of custom emoji
  x-api-slug: emoji-get
  description: |-
    Get a page of metadata for custom emoji on the system. Since server version 4.7, sort using the `sort` query parameter.
    ##### Permissions
    Must be authenticated.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mattermost/emoji-get-openapi.md
- name: Mattermost API Reference - List incoming webhooks
  x-api-slug: hooksincoming-get
  description: |-
    Get a page of a list of incoming webhooks. Optionally filter for a specific team using query parameters.
    ##### Permissions
    `manage_webhooks` for the system or `manage_webhooks` for the specific team.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mattermost/hooksincoming-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mattermost/hooksincoming-get-openapi.md
- name: Mattermost API Reference - Get a list of custom emoji
  x-api-slug: emoji-get
  description: |-
    Get a page of metadata for custom emoji on the system. Since server version 4.7, sort using the `sort` query parameter.
    ##### Permissions
    Must be authenticated.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mattermost/emoji-get-openapi.md
- name: Mattermost API Reference - List a user's preferences by category
  x-api-slug: usersuser-idpreferencescategory-get
  description: |-
    Lists the current user's stored preferences in the given category.
    ##### Permissions
    Must be logged in as the user being updated or have the `edit_other_users` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mattermost/usersuser-idpreferencescategory-get-openapi.md
- name: Mattermost API Reference - Get a list of custom emoji
  x-api-slug: emoji-get
  description: |-
    Get a page of metadata for custom emoji on the system. Since server version 4.7, sort using the `sort` query parameter.
    ##### Permissions
    Must be authenticated.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mattermost/emoji-get-openapi.md
- name: Mattermost API Reference - List a user's preferences by category
  x-api-slug: usersuser-idpreferencescategory-get
  description: |-
    Lists the current user's stored preferences in the given category.
    ##### Permissions
    Must be logged in as the user being updated or have the `edit_other_users` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mattermost/usersuser-idpreferencescategory-get-openapi.md
- name: Mattermost API Reference - Get a list of flagged posts
  x-api-slug: usersuser-idpostsflagged-get
  description: |-
    Get a page of flagged posts of a user provided user id string. Selects from a channel, team or all flagged posts by a user.
    ##### Permissions
    Must be user or have `manage_system` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mattermost/usersuser-idpostsflagged-get-openapi.md
- name: Mattermost API Reference - List a user's preferences by category
  x-api-slug: usersuser-idpreferencescategory-get
  description: |-
    Lists the current user's stored preferences in the given category.
    ##### Permissions
    Must be logged in as the user being updated or have the `edit_other_users` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mattermost/usersuser-idpreferencescategory-get-openapi.md
- name: Mattermost API Reference - Get a list of flagged posts
  x-api-slug: usersuser-idpostsflagged-get
  description: |-
    Get a page of flagged posts of a user provided user id string. Selects from a channel, team or all flagged posts by a user.
    ##### Permissions
    Must be user or have `manage_system` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mattermost/usersuser-idpostsflagged-get-openapi.md
- name: Mattermost API Reference - Get a list of channels by ids
  x-api-slug: teamsteam-idchannelsids-post
  description: |-
    Get a list of public channels on a team by id.
    ##### Permissions
    `view_team` for the team the channels are on.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mattermost/teamsteam-idchannelsids-post-openapi.md
- name: Mattermost API Reference - Get a list of flagged posts
  x-api-slug: usersuser-idpostsflagged-get
  description: |-
    Get a page of flagged posts of a user provided user id string. Selects from a channel, team or all flagged posts by a user.
    ##### Permissions
    Must be user or have `manage_system` permission.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mattermost/usersuser-idpostsflagged-get-openapi.md
- name: Mattermost API Reference - Get a list of channels by ids
  x-api-slug: teamsteam-idchannelsids-post
  description: |-
    Get a list of public channels on a team by id.
    ##### Permissions
    `view_team` for the team the channels are on.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mattermost/teamsteam-idchannelsids-post-openapi.md
- name: Mattermost API Reference - Get a list of channels by ids
  x-api-slug: teamsteam-idchannelsids-post
  description: |-
    Get a list of public channels on a team by id.
    ##### Permissions
    `view_team` for the team the channels are on.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/mattermost-logo.png
  humanURL: https://mattermost.com
  baseURL: https://your-mattermost-url.com//api/v4
  tags: Enterprise, SaaS, Technology, Cloud, API Provider, API Service Provider, Profiles,
    Relative Data, Service API, Networks
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mattermost/teamsteam-idchannelsids-post-openapi.md
x-common:
- type: x-api-gallery
  url: http://matrix.api.gallery.streamdata.io
- type: x-api-stack
  url: http://mattermost.stack.network
- type: x-blog
  url: https://about.mattermost.com/blog/
- type: x-blog-rss
  url: https://about.mattermost.com/feed/
- type: x-crunchbase
  url: https://crunchbase.com/organization/mattermost
- type: x-developer
  url: https://api.mattermost.com/
- type: x-github
  url: https://github.com/mattermost
- type: x-pricing
  url: https://about.mattermost.com/pricing/
- type: x-security
  url: https://docs.mattermost.com/overview/security.html
- type: x-twitter
  url: https://twitter.com/mattermosthq
- type: x-website
  url: https://mattermost.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---