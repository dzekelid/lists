---
name: GoToMeeting
x-slug: gotomeeting
description: Citrix enables business mobility through the secure delivery of apps
  and data to any device on any network.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
x-kinRank: "7"
x-alexaRank: "7422"
tags: Lists
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/gotomeeting/apis.md
specificationVersion: "0.14"
apis:
- name: Go To Webinar Get webinar panelists
  x-api-slug: go-to-webinar
  description: Retrieves all the panelists for a specific webinar.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2W/rest//organizers/{organizerKey}/webinars/{webinarKey}/panelists
  tags: Organizers,OrganizerKey,Webinars,WebinarKey,Panelists
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/gotomeeting/organizersorganizerkeywebinarswebinarkeypanelists-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/gotomeeting/organizersorganizerkeywebinarswebinarkeypanelists-get-openapi.md
- name: Go To Webinar Create Panelists
  x-api-slug: go-to-webinar
  description: Create panelists for a specified webinar
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2W/rest//organizers/{organizerKey}/webinars/{webinarKey}/panelists
  tags: Organizers,OrganizerKey,Webinars,WebinarKey,Panelists
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/gotomeeting/organizersorganizerkeywebinarswebinarkeypanelists-post-openapi.md
- name: Go To Webinar Delete webinar panelist
  x-api-slug: go-to-webinar
  description: Removes a webinar panelist.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2W/rest//organizers/{organizerKey}/webinars/{webinarKey}/panelists/{panelistKey}
  tags: Organizers,OrganizerKey,Webinars,WebinarKey,Panelists,PanelistKey
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/gotomeeting/organizersorganizerkeywebinarswebinarkeypanelistspanelistkey-delete-openapi.md
- name: Go To Webinar Resend panelist invitation
  x-api-slug: go-to-webinar
  description: Resend the panelist invitation email.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2W/rest//organizers/{organizerKey}/webinars/{webinarKey}/panelists/{panelistKey}/resendInvitation
  tags: Organizers,OrganizerKey,Webinars,WebinarKey,Panelists,PanelistKey,ResendInvitation
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/gotomeeting/organizersorganizerkeywebinarswebinarkeypanelistspanelistkeyresendinvitation-post-openapi.md
- name: Go To Webinar
  x-api-slug: go-to-webinar
  description: Citrix enables business mobility through the secure delivery of apps
    and data to any device on any network.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/731-gotomeeting.jpg
  humanURL: https://citrixonline.com
  baseURL: https://api.citrixonline.com//G2W/rest
  tags: Lists
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/gotomeeting/openapi.md
x-common:
- type: x-base
  url: https://api.citrixonline.com
- type: x-blog
  url: http://blogs.citrix.com/
- type: x-crunchbase
  url: https://crunchbase.com/organization/citrix-systems
- type: x-crunchbase
  url: http://www.crunchbase.com/company/citrix-systems
- type: x-developer
  url: https://developer.citrixonline.com/
- type: x-email
  url: secure@citrix.com
- type: x-email
  url: americasconsulting@citrix.com
- type: x-email
  url: poland@citrix.com
- type: x-email
  url: citrix_ru@citrix.com
- type: x-email
  url: Licensing-emea@eu.citrix.com
- type: x-email
  url: eduardo.fleites@citrix.com
- type: x-email
  url: CitrixReady@citrix.com
- type: x-email
  url: CSP@citrix.com
- type: x-email
  url: partneroperationsEMEA@eu.citrix.com
- type: x-github
  url: https://github.com/citrix
- type: x-twitter
  url: https://twitter.com/gotomeeting
- type: x-twitter
  url: https://twitter.com/citrix
- type: x-website
  url: https://citrixonline.com
- type: x-website
  url: http://citrixonline.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---