---
name: CallFire
x-slug: callfire
description: Grow your business with virtual phone numbers, IVR, voice broadcasting,
  mass text messaging services and power dialing. Try CallFire for FREE!
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
x-kinRank: "9"
x-alexaRank: "129466"
tags: Lists
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/callfire/apis.md
specificationVersion: "0.14"
apis:
- name: Callfire Find contact lists
  x-api-slug: callfire
  description: Searches for all contact lists which are available for the current
    user. Returns a paged list of contact lists
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//contacts/lists
  tags: Contacts,Lists
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/callfire/contactslists-get-openapi.md
- name: Callfire Create contact lists
  x-api-slug: callfire
  description: Creates a contact list for use with campaigns using 1 of 3 inputs.
    A List of Contact objects, a list of String E.164 numbers, or a list of CallFire
    contactIds can be used as the data source for the created contact list. After
    contact list is added into the CallFire system, contact lists goes through seven
    system safeguards that check the accuracy and consistency of the data. For example,
    our system checks that contact number is formatted correctly, is valid, is not
    duplicated in another contact list, or is not added on a specific DNC list. You
    can configure to keep/merge or remove contacts which do not complies these rules.
    If contacts were not added to a contact list after the validation, this means
    the data needs to be properly formatted and corrected before calling this API
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//contacts/lists
  tags: Contacts,Lists
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/callfire/contactslists-post-openapi.md
- name: Callfire Create contact list from file
  x-api-slug: callfire
  description: Creates a contact list to be used with campaigns through uploading
    a .csv file. Returns the id of created list
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//contacts/lists/upload
  tags: Contacts,Lists,Upload
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/callfire/contactslistsupload-post-openapi.md
- name: Callfire Delete a contact list
  x-api-slug: callfire
  description: Deletes a contact list, included contacts will not be deleted.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//contacts/lists/{id}
  tags: Contacts,Lists
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/callfire/contactslistsid-delete-openapi.md
- name: Callfire Find a specific contact list
  x-api-slug: callfire
  description: Returns a single ContactList instance for a given contact list id
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//contacts/lists/{id}
  tags: Contacts,Lists
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/callfire/contactslistsid-get-openapi.md
- name: Callfire Update a contact list
  x-api-slug: callfire
  description: Updates contact list instance.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//contacts/lists/{id}
  tags: Contacts,Lists
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/callfire/contactslistsid-put-openapi.md
- name: Callfire Delete contacts from a contact list
  x-api-slug: callfire
  description: Deletes contacts from a contact list. List the contact ids in request
    to delete multiple contacts with one request.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//contacts/lists/{id}/items
  tags: Contacts,Lists,Items
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/callfire/contactslistsiditems-delete-openapi.md
- name: Callfire Find contacts in a contact list
  x-api-slug: callfire
  description: Searches for all entries in a contact list with specified id. Returns
    a paged list of contact entries
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//contacts/lists/{id}/items
  tags: Contacts,Lists,Items
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/callfire/contactslistsiditems-get-openapi.md
- name: Callfire Add contacts to a contact list
  x-api-slug: callfire
  description: 'Adds contacts to a contact list. Available contact sources are: list
    of the contact entities, list of ids of existing contacts in user''s account,
    list of phone numbers in E.164 format (11-digits)'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//contacts/lists/{id}/items
  tags: Contacts,Lists,Items
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/callfire/contactslistsiditems-post-openapi.md
- name: Callfire Delete a contact from a contact list
  x-api-slug: callfire
  description: Deletes a single contact from a contact list
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2//contacts/lists/{id}/items/{contactId}
  tags: Contacts,Lists,Items,ContactId
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/callfire/contactslistsiditemscontactid-delete-openapi.md
- name: Callfire
  x-api-slug: callfire
  description: Grow your business with virtual phone numbers, IVR, voice broadcasting,
    mass text messaging services and power dialing. Try CallFire for FREE!
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/11768-callfire.jpg
  humanURL: http://www.callfire.com
  baseURL: https://www.callfire.com//v2
  tags: Lists
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/callfire/openapi.md
x-common:
- type: x--net-sdk
  url: https://github.com/CallFire/CallFire-CSharp-SDK
- type: x-account-billing
  url: https://answers.callfire.com/hc/en-us/sections/200166268-Billing
- type: x-account-settings
  url: https://answers.callfire.com/hc/en-us/sections/200187056-Account-Settings
- type: x-authentication
  url: https://www.callfire.com/api-documentation/how-do-i-enable-api-on-my-account
- type: x-blog
  url: https://www.callfire.com/blog
- type: x-blog-rss
  url: https://www.callfire.com/blog/feed
- type: x-twitter
  url: https://twitter.com/CallFire
- type: x-case-studies
  url: https://www.callfire.com/case-studies
- type: x-compliance
  url: https://www.callfire.com/legal/compliance
- type: x-contact-form
  url: https://www.callfire.com/contact
- type: x-crunchbase
  url: https://www.crunchbase.com/organization/callfire
- type: x-crunchbase
  url: https://crunchbase.com/organization/callfire
- type: x-developer
  url: https://www.callfire.com/api-documentation
- type: x-documentation
  url: https://www.callfire.com/api-documentation/rest/version/1.1
- type: x-drupal-plugin
  url: https://github.com/CallFire/CallFire-Drupal-Integration
- type: x-email
  url: answers@callfire.com
- type: x-email
  url: support@callfire.com
- type: x-facebook
  url: https://www.facebook.com/callfire
- type: x-faq
  url: https://answers.callfire.com/hc/en-us/sections/200193833-FAQs
- type: x-getting-started
  url: https://www.callfire.com/help/docs/getting-started
- type: x-github
  url: https://github.com/callfire
- type: x-glossary
  url: https://www.callfire.com/help/glossary/communications
- type: x-google-plus
  url: https://plus.google.com/100142045997033051154
- type: x-messages
  url: https://www.callfire.com/ui/number/messages?6
- type: x-partners
  url: https://www.callfire.com/partners
- type: x-phone
  url: 1.877.897.3473
- type: x-php-sdk
  url: https://github.com/CallFire/CallFire-PHP-SDK
- type: x-pricing
  url: https://www.callfire.com/pricing
- type: x-privacy
  url: https://www.callfire.com/legal/privacy
- type: x-selfservice-registration
  url: https://www.callfire.com/ui/register?1
- type: x-terms-of-service
  url: https://www.callfire.com/legal/terms
- type: x-tickets
  url: https://answers.callfire.com/hc/en-us/requests/new
- type: x-tour
  url: javascript:;
- type: x-videos
  url: https://answers.callfire.com/hc/en-us/articles/200849247-Videos
- type: x-webinars
  url: https://answers.callfire.com/hc/en-us/articles/202174798-Webinars
- type: x-website
  url: http://www.callfire.com
- type: x-wordpress-plugin
  url: https://github.com/CallFire/CallFire-WordPress-Integration
- type: x-youtube
  url: https://www.youtube.com/user/CallFireTelephony
- type: x-zapier
  url: https://zapier.com/zapbook/callfire/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---