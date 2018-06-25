---
name: Eventbrite
x-slug: eventbrite
description: Eventbrite brings people together through live experiences. Discover
  events that match your passions, or create your own with online ticketing tools.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
x-kinRank: "9"
x-alexaRank: "643"
tags: Lists
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/eventbrite/apis.md
specificationVersion: "0.14"
apis:
- name: Eventbrite Get Users Contact Lists
  x-api-slug: eventbrite
  description: |-
    Returns a list of contact_list that the user owns as the key
    contact_lists.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D///users/{id}/contact_lists/
  tags: Users,Contact,Lists
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/eventbrite/usersidcontact-lists-get-openapi.md
- name: Eventbrite Post Users Contact Lists
  x-api-slug: eventbrite
  description: |-
    Makes a new contact_list for the user and returns it as
    contact_list.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D///users/{id}/contact_lists/
  tags: Users,Contact,Lists
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/eventbrite/usersidcontact-lists-post-openapi.md
- name: Eventbrite Get Users Contact Lists Contact List
  x-api-slug: eventbrite
  description: Gets a user&#8217;s contact_list by ID as contact_list.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D///users/{id}/contact_lists/:contact_list_id/
  tags: Users,Contact,Lists,:contact,List
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/eventbrite/usersidcontact-listscontact-list-id-get-openapi.md
- name: Eventbrite Post Users Contact Lists Contact List
  x-api-slug: eventbrite
  description: Updates the contact_list and returns it as contact_list.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D///users/{id}/contact_lists/:contact_list_id/
  tags: Users,Contact,Lists,:contact,List
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/eventbrite/usersidcontact-listscontact-list-id-post-openapi.md
- name: Eventbrite Delete Users Contact Lists Contact List
  x-api-slug: eventbrite
  description: 'Deletes the contact list. Returns {&quot;deleted&quot;: true}.'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D///users/{id}/contact_lists/:contact_list_id/
  tags: Users,Contact,Lists,:contact,List
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/eventbrite/usersidcontact-listscontact-list-id-delete-openapi.md
- name: Eventbrite Get Users Contact Lists Contact List Contacts
  x-api-slug: eventbrite
  description: |-
    Returns the contacts on the contact list
    as contacts.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D///users/{id}/contact_lists/:contact_list_id/contacts/
  tags: Users,Contact,Lists,:contact,List,Contacts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/eventbrite/usersidcontact-listscontact-list-idcontacts-get-openapi.md
- name: Eventbrite Post Users Contact Lists Contact List Contacts
  x-api-slug: eventbrite
  description: 'Adds a new contact to the contact list. Returns {&quot;created&quot;:
    true}.'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D///users/{id}/contact_lists/:contact_list_id/contacts/
  tags: Users,Contact,Lists,:contact,List,Contacts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/eventbrite/usersidcontact-listscontact-list-idcontacts-post-openapi.md
- name: Eventbrite Delete Users Contact Lists Contact List Contacts
  x-api-slug: eventbrite
  description: |-
    Deletes the specified contact from the contact list.
    Returns {&quot;deleted&quot;: true}.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D///users/{id}/contact_lists/:contact_list_id/contacts/
  tags: Users,Contact,Lists,:contact,List,Contacts
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/eventbrite/usersidcontact-listscontact-list-idcontacts-delete-openapi.md
- name: Eventbrite
  x-api-slug: eventbrite
  description: Eventbrite brings people together through live experiences. Discover
    events that match your passions, or create your own with online ticketing tools.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/193-eventbrite.jpg
  humanURL: http://eventbriteapi.com
  baseURL: https://www.eventbrite.com//%7Bdata-type%7D/
  tags: Lists
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/eventbrite/openapi.md
x-common:
- type: x-apigee-console
  url: https://api.apigee.com/v1/consoles/eventbrite/apidescription?format=internal&ver=1351170233000
- type: x-authentication
  url: https://developer.eventbrite.com/docs/auth/
- type: x-base
  url: https://www.eventbriteapi.com/
- type: x-blog
  url: http://blog.eventbrite.com/
- type: x-blog-rss
  url: http://blog.eventbrite.com/feed/
- type: x-crunchbase
  url: http://www.crunchbase.com/company/eventbrite
- type: x-crunchbase
  url: https://crunchbase.com/organization/eventbrite
- type: x-developer
  url: https://developer.eventbrite.com/
- type: x-github
  url: https://github.com/eventbrite
- type: x-pricing
  url: http://help.eventbrite.com/customer/en_us/portal/articles/428604
- type: x-privacy
  url: http://www.eventbrite.com/privacypolicy
- type: x-sdks-io
  url: https://sdks.io/SDK/View/eventbrite
- type: x-selfservice-registration
  url: https://www.eventbrite.com/signup/?referrer=%2F%3Fshow_onboarding%3D1&user_type=prebuyer&user_type_sig=AH_ElWGNJ_zHaAxwjzt5jiCRmvPvNBsy6w
- type: x-terms-of-service
  url: http://www.eventbrite.com/tos
- type: x-twitter
  url: https://twitter.com/EventbriteAPI
- type: x-twitter
  url: https://twitter.com/eventbrite
- type: x-website
  url: http://eventbriteapi.com
- type: x-website
  url: http://developer.eventbrite.com/
- type: x-website
  url: http://eventbrite.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---