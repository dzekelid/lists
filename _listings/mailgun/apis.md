---
name: Mailgun
x-slug: mailgun
description: Mailgun provides a web service for integrating email inboxes into apps.
  Providing APIs for sending, receiving, and storing APis, including tools for managing
  delivery, real-time integration, organizing, routing, and tracking on emails. Malign
  provides a free trial to learn about services, and pay as you go, unit based pricing
  to continue from there, including volume pricing for increased usage.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/612-mail_gun.jpg
x-kinRank: "8"
x-alexaRank: "24750"
tags: Lists
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mailgun/apis.md
specificationVersion: "0.14"
apis:
- name: Mailgun API - Lists
  x-api-slug: lists-get
  description: Returns a list of mailing lists under your account.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/612-mail_gun.jpg
  humanURL: http://mailgun.net
  baseURL: https://api.mailgun.net/v2/
  tags: Stack Network, SaaS, Technology, API Provider, API Provider, Emails, Messages,
    Profiles, Emails, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mailgun/lists-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mailgun/lists-get-openapi.md
- name: Mailgun API - Create List
  x-api-slug: lists-post
  description: Creates a new mailing list.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/612-mail_gun.jpg
  humanURL: http://mailgun.net
  baseURL: https://api.mailgun.net/v2/
  tags: Stack Network, SaaS, Technology, API Provider, API Provider, Emails, Messages,
    Profiles, Emails, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mailgun/lists-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mailgun/lists-post-openapi.md
- name: Mailgun API - Delete List
  x-api-slug: listsaddress-delete
  description: Deletes a mailing list.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/612-mail_gun.jpg
  humanURL: http://mailgun.net
  baseURL: https://api.mailgun.net/v2/
  tags: Stack Network, SaaS, Technology, API Provider, API Provider, Emails, Messages,
    Profiles, Emails, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mailgun/listsaddress-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mailgun/listsaddress-delete-openapi.md
- name: Mailgun API - List
  x-api-slug: listsaddress-get
  description: Returns a single mailing list by a given address.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/612-mail_gun.jpg
  humanURL: http://mailgun.net
  baseURL: https://api.mailgun.net/v2/
  tags: Stack Network, SaaS, Technology, API Provider, API Provider, Emails, Messages,
    Profiles, Emails, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mailgun/listsaddress-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mailgun/listsaddress-get-openapi.md
- name: Mailgun API - Update List
  x-api-slug: listsaddress-put
  description: Update mailing list properties, such as address, description or name
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/612-mail_gun.jpg
  humanURL: http://mailgun.net
  baseURL: https://api.mailgun.net/v2/
  tags: Stack Network, SaaS, Technology, API Provider, API Provider, Emails, Messages,
    Profiles, Emails, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mailgun/listsaddress-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mailgun/listsaddress-put-openapi.md
- name: Mailgun API - Add To List
  x-api-slug: listsaddressmembers-get
  description: Adds a member to the mailing list.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/612-mail_gun.jpg
  humanURL: http://mailgun.net
  baseURL: https://api.mailgun.net/v2/
  tags: Stack Network, SaaS, Technology, API Provider, API Provider, Emails, Messages,
    Profiles, Emails, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mailgun/listsaddressmembers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mailgun/listsaddressmembers-get-openapi.md
- name: Mailgun API - List Members
  x-api-slug: listsaddressmembers-get
  description: Fetches the list of mailing list members.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/612-mail_gun.jpg
  humanURL: http://mailgun.net
  baseURL: https://api.mailgun.net/v2/
  tags: Stack Network, SaaS, Technology, API Provider, API Provider, Emails, Messages,
    Profiles, Emails, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mailgun/listsaddressmembers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mailgun/listsaddressmembers-get-openapi.md
- name: Mailgun API - List Member
  x-api-slug: listsaddressmembersmember-address-get
  description: Retrieves a mailing list member.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/612-mail_gun.jpg
  humanURL: http://mailgun.net
  baseURL: https://api.mailgun.net/v2/
  tags: Stack Network, SaaS, Technology, API Provider, API Provider, Emails, Messages,
    Profiles, Emails, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mailgun/listsaddressmembersmember-address-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mailgun/listsaddressmembersmember-address-get-openapi.md
- name: Mailgun API - Add to unsubscribe list.
  x-api-slug: unsubscribes-post
  description: Adds address to unsubscribed table.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/612-mail_gun.jpg
  humanURL: http://mailgun.net
  baseURL: https://api.mailgun.net/v2/
  tags: Stack Network, SaaS, Technology, API Provider, API Provider, Emails, Messages,
    Profiles, Emails, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mailgun/unsubscribes-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mailgun/unsubscribes-post-openapi.md
- name: Mailgun API - Add to unsubscribe list.
  x-api-slug: unsubscribes-post
  description: Adds address to unsubscribed table.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/612-mail_gun.jpg
  humanURL: http://mailgun.net
  baseURL: https://api.mailgun.net/v2/
  tags: Stack Network, SaaS, Technology, API Provider, API Provider, Emails, Messages,
    Profiles, Emails, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mailgun/unsubscribes-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mailgun/unsubscribes-post-openapi.md
- name: Mailgun API - Add to unsubscribe list.
  x-api-slug: unsubscribes-post
  description: Adds address to unsubscribed table.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/612-mail_gun.jpg
  humanURL: http://mailgun.net
  baseURL: https://api.mailgun.net/v2/
  tags: Stack Network, SaaS, Technology, API Provider, API Provider, Emails, Messages,
    Profiles, Emails, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mailgun/unsubscribes-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mailgun/unsubscribes-post-openapi.md
- name: Mailgun API - List Member
  x-api-slug: listsaddressmembersmember-address-get
  description: Retrieves a mailing list member.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/612-mail_gun.jpg
  humanURL: http://mailgun.net
  baseURL: https://api.mailgun.net/v2/
  tags: Stack Network, SaaS, Technology, API Provider, API Provider, Emails, Messages,
    Profiles, Emails, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mailgun/listsaddressmembersmember-address-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mailgun/listsaddressmembersmember-address-get-openapi.md
- name: Mailgun API - List Member
  x-api-slug: listsaddressmembersmember-address-get
  description: Retrieves a mailing list member.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/612-mail_gun.jpg
  humanURL: http://mailgun.net
  baseURL: https://api.mailgun.net/v2/
  tags: Stack Network, SaaS, Technology, API Provider, API Provider, Emails, Messages,
    Profiles, Emails, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mailgun/listsaddressmembersmember-address-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mailgun/listsaddressmembersmember-address-get-openapi.md
- name: Mailgun API - List Members
  x-api-slug: listsaddressmembers-get
  description: Fetches the list of mailing list members.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/612-mail_gun.jpg
  humanURL: http://mailgun.net
  baseURL: https://api.mailgun.net/v2/
  tags: Stack Network, SaaS, Technology, API Provider, API Provider, Emails, Messages,
    Profiles, Emails, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mailgun/listsaddressmembers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mailgun/listsaddressmembers-get-openapi.md
- name: Mailgun API - List Members
  x-api-slug: listsaddressmembers-get
  description: Fetches the list of mailing list members.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/612-mail_gun.jpg
  humanURL: http://mailgun.net
  baseURL: https://api.mailgun.net/v2/
  tags: Stack Network, SaaS, Technology, API Provider, API Provider, Emails, Messages,
    Profiles, Emails, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mailgun/listsaddressmembers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mailgun/listsaddressmembers-get-openapi.md
- name: Mailgun API - Add To List
  x-api-slug: listsaddressmembers-get
  description: Adds a member to the mailing list.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/612-mail_gun.jpg
  humanURL: http://mailgun.net
  baseURL: https://api.mailgun.net/v2/
  tags: Stack Network, SaaS, Technology, API Provider, API Provider, Emails, Messages,
    Profiles, Emails, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mailgun/listsaddressmembers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mailgun/listsaddressmembers-get-openapi.md
- name: Mailgun API - Add To List
  x-api-slug: listsaddressmembers-get
  description: Adds a member to the mailing list.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/612-mail_gun.jpg
  humanURL: http://mailgun.net
  baseURL: https://api.mailgun.net/v2/
  tags: Stack Network, SaaS, Technology, API Provider, API Provider, Emails, Messages,
    Profiles, Emails, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mailgun/listsaddressmembers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mailgun/listsaddressmembers-get-openapi.md
- name: Mailgun API - Update List
  x-api-slug: listsaddress-put
  description: Update mailing list properties, such as address, description or name
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/612-mail_gun.jpg
  humanURL: http://mailgun.net
  baseURL: https://api.mailgun.net/v2/
  tags: Stack Network, SaaS, Technology, API Provider, API Provider, Emails, Messages,
    Profiles, Emails, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mailgun/listsaddress-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mailgun/listsaddress-put-openapi.md
- name: Mailgun API - Update List
  x-api-slug: listsaddress-put
  description: Update mailing list properties, such as address, description or name
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/612-mail_gun.jpg
  humanURL: http://mailgun.net
  baseURL: https://api.mailgun.net/v2/
  tags: Stack Network, SaaS, Technology, API Provider, API Provider, Emails, Messages,
    Profiles, Emails, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mailgun/listsaddress-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mailgun/listsaddress-put-openapi.md
- name: Mailgun API - List
  x-api-slug: listsaddress-get
  description: Returns a single mailing list by a given address.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/612-mail_gun.jpg
  humanURL: http://mailgun.net
  baseURL: https://api.mailgun.net/v2/
  tags: Stack Network, SaaS, Technology, API Provider, API Provider, Emails, Messages,
    Profiles, Emails, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mailgun/listsaddress-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mailgun/listsaddress-get-openapi.md
- name: Mailgun API - List
  x-api-slug: listsaddress-get
  description: Returns a single mailing list by a given address.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/612-mail_gun.jpg
  humanURL: http://mailgun.net
  baseURL: https://api.mailgun.net/v2/
  tags: Stack Network, SaaS, Technology, API Provider, API Provider, Emails, Messages,
    Profiles, Emails, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mailgun/listsaddress-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mailgun/listsaddress-get-openapi.md
- name: Mailgun API - Delete List
  x-api-slug: listsaddress-delete
  description: Deletes a mailing list.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/612-mail_gun.jpg
  humanURL: http://mailgun.net
  baseURL: https://api.mailgun.net/v2/
  tags: Stack Network, SaaS, Technology, API Provider, API Provider, Emails, Messages,
    Profiles, Emails, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mailgun/listsaddress-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mailgun/listsaddress-delete-openapi.md
- name: Mailgun API - Delete List
  x-api-slug: listsaddress-delete
  description: Deletes a mailing list.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/612-mail_gun.jpg
  humanURL: http://mailgun.net
  baseURL: https://api.mailgun.net/v2/
  tags: Stack Network, SaaS, Technology, API Provider, API Provider, Emails, Messages,
    Profiles, Emails, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mailgun/listsaddress-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mailgun/listsaddress-delete-openapi.md
- name: Mailgun API - Create List
  x-api-slug: lists-post
  description: Creates a new mailing list.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/612-mail_gun.jpg
  humanURL: http://mailgun.net
  baseURL: https://api.mailgun.net/v2/
  tags: Stack Network, SaaS, Technology, API Provider, API Provider, Emails, Messages,
    Profiles, Emails, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mailgun/lists-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mailgun/lists-post-openapi.md
- name: Mailgun API - Create List
  x-api-slug: lists-post
  description: Creates a new mailing list.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/612-mail_gun.jpg
  humanURL: http://mailgun.net
  baseURL: https://api.mailgun.net/v2/
  tags: Stack Network, SaaS, Technology, API Provider, API Provider, Emails, Messages,
    Profiles, Emails, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mailgun/lists-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/mailgun/lists-post-openapi.md
x-common:
- type: x--net-library
  url: http://documentation.mailgun.com/libraries.html#c
- type: x-api-gallery
  url: http://lykke.api.gallery.streamdata.io
- type: x-api-stack
  url: http://mailgun.stack.network
- type: x-base
  url: https://api.mailgun.net
- type: x-blog
  url: http://blog.mailgun.net
- type: x-blog-rss
  url: https://twitter.com/unbounce
- type: x-crunchbase
  url: http://www.crunchbase.com/company/mailgun
- type: x-crunchbase
  url: https://crunchbase.com/organization/mailgun
- type: x-developer
  url: http://documentation.mailgun.com/
- type: x-email
  url: privacy@mailgun.com
- type: x-faq
  url: http://documentation.mailgun.com/faqs.html
- type: x-github
  url: https://github.com/mailgun
- type: x-heroku-addon
  url: https://addons.heroku.com/mailgun
- type: x-java-library
  url: http://documentation.mailgun.com/libraries.html#java
- type: x-node-js-library
  url: http://documentation.mailgun.com/libraries.html#node-js
- type: x-php-library
  url: http://documentation.mailgun.com/libraries.html#php
- type: x-pricing
  url: http://www.mailgun.com/pricing
- type: x-privacy
  url: http://www.mailgun.com/privacy
- type: x-python-library
  url: http://documentation.mailgun.com/libraries.html#python
- type: x-ruby-library
  url: http://documentation.mailgun.com/libraries.html#ruby
- type: x-selfservice-registration
  url: https://www.mailgun.com/signup
- type: x-stack-overflow
  url: https://stackoverflow.com/questions/tagged/mailgun
- type: x-terms-of-service
  url: http://www.mailgun.com/terms
- type: x-twitter
  url: https://twitter.com/#!/mail_gun
- type: x-website
  url: http://mailgun.net
- type: x-wordpress-plugin
  url: https://wordpress.org/plugins/mailgun/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---