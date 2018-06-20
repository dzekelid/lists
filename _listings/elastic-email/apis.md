---
name: Elastic Email
x-slug: elastic-email
description: Elastic Email is an all-in-one email delivery platform. Send beautiful
  newsletters or transactional emails in a better way.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/586-elastic-email.jpg
x-kinRank: "8"
x-alexaRank: "50338"
tags: Lists
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/elastic-email/apis.md
specificationVersion: "0.14"
apis:
- name: Elastic Email SMTP API Add Existing Subscriber To List
  x-api-slug: elastic-email-smtp-api
  description: Add Existing Subscriber To List
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/586-elastic-email.jpg
  humanURL: http://elasticemail.com
  baseURL: http://api.elasticemail.com///lists/add-contact
  tags: Lists,Add,Contact
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/elastic-email/listsaddcontact-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/elastic-email/listsaddcontact-get-openapi.md
- name: Elastic Email SMTP API Create New Subscriber
  x-api-slug: elastic-email-smtp-api
  description: Create New Subscriber
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/586-elastic-email.jpg
  humanURL: http://elasticemail.com
  baseURL: http://api.elasticemail.com///lists/create-contact
  tags: Lists,Create,Contact
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/elastic-email/listscreatecontact-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/elastic-email/listscreatecontact-get-openapi.md
- name: Elastic Email SMTP API Create New List
  x-api-slug: elastic-email-smtp-api
  description: Create New List
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/586-elastic-email.jpg
  humanURL: http://elasticemail.com
  baseURL: http://api.elasticemail.com///lists/create-lists
  tags: Lists,Create,Lists
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/elastic-email/listscreatelists-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/elastic-email/listscreatelists-get-openapi.md
- name: Elastic Email SMTP API Delete Existing List
  x-api-slug: elastic-email-smtp-api
  description: Delete Existing List
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/586-elastic-email.jpg
  humanURL: http://elasticemail.com
  baseURL: http://api.elasticemail.com///lists/delete
  tags: Lists,Delete
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/elastic-email/listsdelete-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/elastic-email/listsdelete-get-openapi.md
- name: Elastic Email SMTP API Delete Existing Subscriber
  x-api-slug: elastic-email-smtp-api
  description: Delete Existing Subscriber
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/586-elastic-email.jpg
  humanURL: http://elasticemail.com
  baseURL: http://api.elasticemail.com///lists/delete-contact
  tags: Lists,Delete,Contact
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/elastic-email/listsdeletecontact-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/elastic-email/listsdeletecontact-get-openapi.md
- name: Elastic Email SMTP API Remove Existing Subscriber From List
  x-api-slug: elastic-email-smtp-api
  description: Remove Existing Subscriber From List
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/586-elastic-email.jpg
  humanURL: http://elasticemail.com
  baseURL: http://api.elasticemail.com///lists/remove-contact
  tags: Lists,Remove,Contact
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/elastic-email/listsremovecontact-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/elastic-email/listsremovecontact-get-openapi.md
- name: Elastic Email SMTP API Create Multiple Subscriber From CSV File
  x-api-slug: elastic-email-smtp-api
  description: Create Multiple Subscriber From CSV File
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/586-elastic-email.jpg
  humanURL: http://elasticemail.com
  baseURL: http://api.elasticemail.com///lists/upload-contacts
  tags: Lists,Upload,Contacts
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/elastic-email/listsuploadcontacts-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/elastic-email/listsuploadcontacts-get-openapi.md
- name: Elastic Email SMTP API Unsubscribed
  x-api-slug: elastic-email-smtp-api
  description: This api will return you the list of email addresses which are currently
    in your block list.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/586-elastic-email.jpg
  humanURL: http://elasticemail.com
  baseURL: http://api.elasticemail.com///mailer/lists/unsubscribed
  tags: Mailer,Lists,Unsubscribed
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/elastic-email/mailerlistsunsubscribed-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/elastic-email/mailerlistsunsubscribed-get-openapi.md
- name: Elastic Email SMTP API
  x-api-slug: elastic-email-smtp-api
  description: Elastic Email is a simple, fast email delivery service for your cloud
    application or marketing needs.  Elastic Email is designed as an SMTP relay for
    reliable delivery of bulk email marketing or single recipient transactional emails
    with detailed delivery statistics.  No monthly committments, no minimums, no limits.  Just
    pay for what you use for as low as  $0.08 / 1000 emails.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/586-elastic-email.jpg
  humanURL: http://elasticemail.com
  baseURL: http://api.elasticemail.com//
  tags: Lists
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/elastic-email/openapi.md
x-common:
- type: x-base
  url: http://api.elasticemail.com
- type: x-blog
  url: http://elasticemail.com/blog
- type: x-blog-rss
  url: http://elasticemail.com/posts/rss/xml
- type: x-crunchbase
  url: https://crunchbase.com/organization/elastic-email
- type: x-crunchbase
  url: http://www.crunchbase.com/company/elastic-email
- type: x-documentation
  url: https://elasticemail.com/api-documentation
- type: x-email
  url: support@elasticemail.com
- type: x-pricing
  url: https://elasticemail.com/pricing
- type: x-privacy
  url: https://elasticemail.com/privacy-policy
- type: x-selfservice-registration
  url: https://elasticemail.com/account#/create-account
- type: x-terms-of-service
  url: https://elasticemail.com/terms
- type: x-twitter
  url: https://twitter.com/elastic_email
- type: x-website
  url: http://elasticemail.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---