---
name: Foursquare
x-slug: foursquare
description: Foursquare helps you find the perfect places to go with friends. Discover
  the best food, nightlife, and entertainment in your area.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
x-kinRank: "9"
x-alexaRank: "2544"
tags: Lists
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/foursquare/apis.md
specificationVersion: "0.14"
apis:
- name: Foursquare Post Lists Add
  x-api-slug: foursquare
  description: /lists/{LIST_ID}
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///lists/add
  tags: Lists
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/foursquare/listsadd-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/foursquare/listsadd-post-openapi.md
- name: Foursquare Get Lists
  x-api-slug: foursquare
  description: /tips/{TIP_ID}/unmark
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///lists/{LIST_ID}
  tags: Lists
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/foursquare/listslist-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/foursquare/listslist-id-get-openapi.md
- name: Foursquare Post Lists Additem
  x-api-slug: foursquare
  description: /lists/{LIST_ID}/suggestvenues
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///lists/{LIST_ID}/additem
  tags: Lists,Item
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/foursquare/listslist-idadditem-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/foursquare/listslist-idadditem-post-openapi.md
- name: Foursquare Post Lists Deleteitem
  x-api-slug: foursquare
  description: /lists/{LIST_ID}/additem
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///lists/{LIST_ID}/deleteitem
  tags: Lists,Item
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/foursquare/listslist-iddeleteitem-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/foursquare/listslist-iddeleteitem-post-openapi.md
- name: Foursquare Post Lists Follow
  x-api-slug: foursquare
  description: /lists/{LIST_ID}/deleteitem
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///lists/{LIST_ID}/follow
  tags: Lists,Follow
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/foursquare/listslist-idfollow-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/foursquare/listslist-idfollow-post-openapi.md
- name: Foursquare Get Lists Followers
  x-api-slug: foursquare
  description: /lists/add
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///lists/{LIST_ID}/followers
  tags: Lists,Followers
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/foursquare/listslist-idfollowers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/foursquare/listslist-idfollowers-get-openapi.md
- name: Foursquare Post Lists Moveitem
  x-api-slug: foursquare
  description: /lists/{LIST_ID}/follow
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///lists/{LIST_ID}/moveitem
  tags: Lists,Moveitem
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/foursquare/listslist-idmoveitem-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/foursquare/listslist-idmoveitem-post-openapi.md
- name: Foursquare Post Lists Share
  x-api-slug: foursquare
  description: /lists/{LIST_ID}/moveitem
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///lists/{LIST_ID}/share
  tags: Lists,Share
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/foursquare/listslist-idshare-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/foursquare/listslist-idshare-post-openapi.md
- name: Foursquare Get Lists Suggestphoto
  x-api-slug: foursquare
  description: /lists/{LIST_ID}/followers
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///lists/{LIST_ID}/suggestphoto
  tags: Lists,Suggestphoto
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/foursquare/listslist-idsuggestphoto-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/foursquare/listslist-idsuggestphoto-get-openapi.md
- name: Foursquare Get Lists Suggesttip
  x-api-slug: foursquare
  description: /lists/{LIST_ID}/suggestphoto
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///lists/{LIST_ID}/suggesttip
  tags: Lists,Suggesttip
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/foursquare/listslist-idsuggesttip-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/foursquare/listslist-idsuggesttip-get-openapi.md
- name: Foursquare Get Lists Suggestvenues
  x-api-slug: foursquare
  description: /lists/{LIST_ID}/suggesttip
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///lists/{LIST_ID}/suggestvenues
  tags: Lists,Suggestvenues
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/foursquare/listslist-idsuggestvenues-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/foursquare/listslist-idsuggestvenues-get-openapi.md
- name: Foursquare Post Lists Unfollow
  x-api-slug: foursquare
  description: /lists/{LIST_ID}/share
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///lists/{LIST_ID}/unfollow
  tags: Lists,Unfollow
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/foursquare/listslist-idunfollow-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/foursquare/listslist-idunfollow-post-openapi.md
- name: Foursquare Post Lists Update
  x-api-slug: foursquare
  description: /lists/{LIST_ID}/unfollow
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///lists/{LIST_ID}/update
  tags: Lists
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/foursquare/listslist-idupdate-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/foursquare/listslist-idupdate-post-openapi.md
- name: Foursquare Post Lists Updateitem
  x-api-slug: foursquare
  description: /lists/{LIST_ID}/update
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///lists/{LIST_ID}/updateitem
  tags: Lists,Item
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/foursquare/listslist-idupdateitem-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/foursquare/listslist-idupdateitem-post-openapi.md
- name: Foursquare Get Users Lists
  x-api-slug: foursquare
  description: /users/{USER_ID}/friends
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2///users/{USER_ID}/lists
  tags: Users,Lists
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/foursquare/usersuser-idlists-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/foursquare/usersuser-idlists-get-openapi.md
- name: Foursquare
  x-api-slug: foursquare
  description: foursquare makes the real world easier to use. We build tools that
    help you keep up with friends, discover whats nearby, save money and unlock deals.
    Whether youre setting off on a trip around the world, coordinating a night out
    with friends, or trying to pick out the best dish at your local restaurant, foursquare
    is the perfect companion. The foursquare API gives you access to all of the data
    used by the foursquare mobile applications, and, in some cases, even more.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/203-foursquare.jpg
  humanURL: http://blog.foursquare.com
  baseURL: https://api.foursquare.com//v2/
  tags: Lists
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/foursquare/openapi.md
x-common:
- type: x-api-json--authoritative
  url: http://apis.io/apisdef/legacy/foursquare.json
- type: x-apigee-console
  url: https://api.apigee.com/v1/consoles/foursquare/apidescription?format=internal&ver=1393644831000
- type: x-application-management
  url: https://foursquare.com/developers/apps
- type: x-blog
  url: http://engineering.foursquare.com/
- type: x-blog-rss
  url: http://engineering.foursquare.com/feed/
- type: x-curated-source
  url: http://blog.foursquare.com/2013/09/17/we-put-a-fresh-coat-of-paint-on-foursquare-for-ios-7/
- type: x-website
  url: http://blog.foursquare.com
- type: x-crunchbase
  url: http://www.crunchbase.com/company/foursquare
- type: x-crunchbase
  url: https://crunchbase.com/organization/foursquare
- type: x-email
  url: support@foursquare.com
- type: x-email
  url: ads@foursquare.com
- type: x-email
  url: press@foursquare.com
- type: x-email
  url: security@foursquare.com
- type: x-email
  url: feedback@foursquare.com
- type: x-email
  url: privacy@foursquare.com
- type: x-error-codes
  url: https://developer.foursquare.com/overview/responses
- type: x-foursquare
  url: http://foursquare.com/nasa
- type: x-foursquare
  url: http://foursquare.com/yourcommissary
- type: x-getting-started
  url: https://developer.foursquare.com/start
- type: x-github
  url: https://github.com/foursquare
- type: x-privacy
  url: https://foursquare.com/legal/privacy
- type: x-rate-limits
  url: https://developer.foursquare.com/overview/ratelimits
- type: x-stack-overflow
  url: http://stackoverflow.com/questions/tagged/foursquare
- type: x-terms-of-service
  url: https://developer.foursquare.com/overview/community
- type: x-twitter
  url: https://twitter.com/foursquare
- type: x-twitter
  url: https://twitter.com/foursquareapi
- type: x-website
  url: http://foursquare.com
- type: x-website
  url: https://developer.foursquare.com/
- type: x-website
  url: https://foursquare.com/apps/slack
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---