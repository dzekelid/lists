---
name: Twitter
x-slug: twitter
description: From breaking news and entertainment to sports and politics, get the
  full story with all the live commentary.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/266-twitter.jpg
x-kinRank: "9"
x-alexaRank: "12"
tags: Lists
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/twitter/apis.md
specificationVersion: "0.14"
apis:
- name: Twitter List LIst
  x-api-slug: twitter
  description: Return all lists the authenticating or specified user subscribes to,
    including their own.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/266-twitter.jpg
  humanURL: https://twitter.com/
  baseURL: https://api.twitter.com//1.1//lists/list
  tags: Social,Lists
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/twitter/listslist-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/twitter/listslist-get-openapi.md
- name: Twitter List Statuses
  x-api-slug: twitter
  description: Returns a timeline of tweets authored by memebers of the specified
    list
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/266-twitter.jpg
  humanURL: https://twitter.com/
  baseURL: https://api.twitter.com//1.1//lists/statuses.json
  tags: Social,Lists
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/twitter/listsstatuses-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/twitter/listsstatuses-json-get-openapi.md
- name: Twitter Remove User From List
  x-api-slug: twitter
  description: Returns the list of memebers destroy
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/266-twitter.jpg
  humanURL: https://twitter.com/
  baseURL: https://api.twitter.com//1.1//lists/members/destroy
  tags: Social,Lists
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/twitter/listsmembersdestroy-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/twitter/listsmembersdestroy-get-openapi.md
- name: Twitter Get Memberships
  x-api-slug: twitter
  description: Returns the lists of the specified user has been added to
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/266-twitter.jpg
  humanURL: https://twitter.com/
  baseURL: https://api.twitter.com//1.1//lists/memberships
  tags: Social,Lists
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/twitter/listsmemberships-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/twitter/listsmemberships-get-openapi.md
- name: Twitter List Subscribers
  x-api-slug: twitter
  description: Returns the subscribers of the specified list
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/266-twitter.jpg
  humanURL: https://twitter.com/
  baseURL: https://api.twitter.com//1.1//lists/subscribers
  tags: Social,Lists
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/twitter/listssubscribers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/twitter/listssubscribers-get-openapi.md
- name: Twitter Add List Subscribers
  x-api-slug: twitter
  description: Subscribes the authenticated user to the specified list
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/266-twitter.jpg
  humanURL: https://twitter.com/
  baseURL: https://api.twitter.com//1.1//lists/subscribers/create
  tags: Social,Lists
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/twitter/listssubscriberscreate-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/twitter/listssubscriberscreate-post-openapi.md
- name: Twitter Show List Subscribers
  x-api-slug: twitter
  description: Check if the specified user is a subscriber of the specified list
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/266-twitter.jpg
  humanURL: https://twitter.com/
  baseURL: https://api.twitter.com//1.1//lists/subscribers/show
  tags: Social,Lists
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/twitter/listssubscribersshow-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/twitter/listssubscribersshow-get-openapi.md
- name: Twitter Remove List Subscribers
  x-api-slug: twitter
  description: Returns list of subscribers destroy
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/266-twitter.jpg
  humanURL: https://twitter.com/
  baseURL: https://api.twitter.com//1.1//lists/subscribers/destroy
  tags: Social,Lists
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/twitter/listssubscribersdestroy-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/twitter/listssubscribersdestroy-get-openapi.md
- name: Twitter Add Users to List
  x-api-slug: twitter
  description: Returns lists of members create_all
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/266-twitter.jpg
  humanURL: https://twitter.com/
  baseURL: https://api.twitter.com//1.1//lists/members/create_all
  tags: Social,Lists
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/twitter/listsmemberscreate-all-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/twitter/listsmemberscreate-all-get-openapi.md
- name: Twitter Show Members
  x-api-slug: twitter
  description: Check if the specified user is a member of the specified list
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/266-twitter.jpg
  humanURL: https://twitter.com/
  baseURL: https://api.twitter.com//1.1//list/members/show
  tags: Social,Lists
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/twitter/listmembersshow-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/twitter/listmembersshow-get-openapi.md
- name: Twitter Get Members
  x-api-slug: twitter
  description: Returns the members of the specified list
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/266-twitter.jpg
  humanURL: https://twitter.com/
  baseURL: https://api.twitter.com//1.1//list/members
  tags: Social,Lists
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/twitter/listmembers-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/twitter/listmembers-get-openapi.md
- name: Twitter Add Member
  x-api-slug: twitter
  description: Returns list of members create
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/266-twitter.jpg
  humanURL: https://twitter.com/
  baseURL: https://api.twitter.com//1.1//list/members/create
  tags: Social,Lists
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/twitter/listmemberscreate-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/twitter/listmemberscreate-post-openapi.md
- name: Twitter Destroy List
  x-api-slug: twitter
  description: Returns list of destroy
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/266-twitter.jpg
  humanURL: https://twitter.com/
  baseURL: https://api.twitter.com//1.1//lists/destroy
  tags: Social,Lists
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/twitter/listsdestroy-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/twitter/listsdestroy-post-openapi.md
- name: Twitter Update List
  x-api-slug: twitter
  description: Returns lists of updates
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/266-twitter.jpg
  humanURL: https://twitter.com/
  baseURL: https://api.twitter.com//1.1//lists/update
  tags: Social,Lists
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/twitter/listsupdate-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/twitter/listsupdate-post-openapi.md
- name: Twitter Create List
  x-api-slug: twitter
  description: Returns list of create
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/266-twitter.jpg
  humanURL: https://twitter.com/
  baseURL: https://api.twitter.com//1.1//lists/create
  tags: Social,Lists
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/twitter/listscreate-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/twitter/listscreate-post-openapi.md
- name: Twitter Show LIsts
  x-api-slug: twitter
  description: Returns list of show
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/266-twitter.jpg
  humanURL: https://twitter.com/
  baseURL: https://api.twitter.com//1.1//lists/show
  tags: Social,Lists
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/twitter/listsshow-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/twitter/listsshow-get-openapi.md
- name: Twitter Show List Subscriptions
  x-api-slug: twitter
  description: Returns list of subscriptions
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/266-twitter.jpg
  humanURL: https://twitter.com/
  baseURL: https://api.twitter.com//1.1//lists/subscriptions
  tags: Social,Lists
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/twitter/listssubscriptions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/twitter/listssubscriptions-get-openapi.md
- name: Twitter Remove Members
  x-api-slug: twitter
  description: Returns lists of destroy all
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/266-twitter.jpg
  humanURL: https://twitter.com/
  baseURL: https://api.twitter.com//1.1//list/members/destroy_all
  tags: Social,Lists
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/twitter/listmembersdestroy-all-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/twitter/listmembersdestroy-all-get-openapi.md
- name: Twitter Help Terms of Services
  x-api-slug: twitter
  description: Returns the Twitter Terms of Service
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/266-twitter.jpg
  humanURL: https://twitter.com/
  baseURL: https://api.twitter.com//1.1//help/tos
  tags: Social,Lists
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/twitter/helptos-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/twitter/helptos-get-openapi.md
- name: Twitter
  x-api-slug: twitter
  description: From breaking news and entertainment to sports and politics, get the
    full story with all the live commentary.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/266-twitter.jpg
  humanURL: https://twitter.com/
  baseURL: https://api.twitter.com//1.1
  tags: Lists
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/twitter/openapi.md
x-common:
- type: x--net-library
  url: https://tweetinvi.codeplex.com/
- type: x-advertising-development-kit
  url: https://docs.fabric.io/unity/mopub/overview.html
- type: x-android-sdk
  url: https://docs.fabric.io/android/fabric/overview.html
- type: x-apple-sdk
  url: https://docs.fabric.io/apple/fabric/overview.html
- type: x-application-management
  url: https://apps.twitter.com/
- type: x-application-only-authentication
  url: https://dev.twitter.com/oauth/application-only
- type: x-authentication
  url: https://dev.twitter.com/oauth
- type: x-authentication-overview
  url: https://dev.twitter.com/oauth/overview
- type: x-base
  url: https://api.twitter.com
- type: x-best-practices
  url: https://dev.twitter.com/overview/general
- type: x-beta
  url: https://docs.fabric.io/unity/beta/overview.html
- type: x-branding
  url: https://brand.twitter.com/
- type: x-branding
  url: https://dev.twitter.com/overview/terms/display-requirements
- type: x-branding
  url: https://about.twitter.com/company/brand-assets
- type: x-case-studies
  url: https://dev.twitter.com/overview/case-studies
- type: x-change-log
  url: https://dev.twitter.com/ads/overview/recent-changes
- type: x-code-libraries
  url: https://dev.twitter.com/overview/api/twitter-libraries
- type: x-coldfusion-library
  url: http://monkehtweet.riaforge.org/
- type: x-console
  url: http://dev.twitter.com/rest/tools/console
- type: x-crunchbase
  url: http://www.crunchbase.com/company/twitter
- type: x-crunchbase
  url: https://crunchbase.com/organization/twitter
- type: x-css-control
  url: https://dev.twitter.com/web/overview/css
- type: x-developer
  url: https://developer.twitter.com/
- type: x-blog
  url: https://dev.twitter.com/blog/
- type: x-blog-rss
  url: https://blog.twitter.com/api/blog.rss?name=developer
- type: x-documentation
  url: https://dev.twitter.com/overview/documentation
- type: x-email
  url: copyright@twitter.com
- type: x-embeddable
  url: https://dev.twitter.com/web/overview
- type: x-encryption
  url: https://dev.twitter.com/overview/api/tls
- type: x-blog
  url: https://blog.twitter.com/engineering
- type: x-blog-rss
  url: https://blog.twitter.com/api/blog.rss?name=engineering
- type: x-error-codes
  url: https://dev.twitter.com/overview/api/response-codes
- type: x-events
  url: https://dev.twitter.com/overview/events
- type: x-forum
  url: https://twittercommunity.com/
- type: x-forum
  url: https://twittercommunity.com/c/fabric
- type: x-geo-guidelines
  url: https://dev.twitter.com/overview/terms/geo-developer-guidelines
- type: x-github
  url: https://github.com/twitter
- type: x-go-library
  url: https://github.com/kurrik/twittergo
- type: x-internationalization
  url: https://dev.twitter.com/overview/general/adding-international-support-to-your-apps
- type: x-java-library
  url: https://www.github.com/twitter/hbc
- type: x-node-js-library
  url: https://github.com/BoyCook/TwitterJSClient
- type: x-oembed
  url: https://dev.twitter.com/web/embedded-timelines/oembed
- type: x-partners
  url: https://dev.twitter.com/overview/general/official-partner-program
- type: x-php-library
  url: https://github.com/abraham/twitteroauth
- type: x-pin-based-authorization
  url: https://dev.twitter.com/oauth/pin-based
- type: x-blog
  url: https://blog.twitter.com/
- type: x-blog-rss
  url: https://blog.twitter.com/api/blog.rss?name=company
- type: x-privacy
  url: https://twitter.com/privacy?lang=en
- type: x-python-library
  url: https://github.com/bear/python-twitter
- type: x-rate-limits
  url: https://dev.twitter.com/rest/public/rate-limiting
- type: x-rate-limits-chart
  url: https://dev.twitter.com/rest/public/rate-limits
- type: x-road-map
  url: https://dev.twitter.com/ads/overview/upcoming-changes
- type: x-ruby-library
  url: https://github.com/sferik/twitter
- type: x-schema
  url: https://dev.twitter.com/overview/api/entities-in-twitter-objects
- type: x-security
  url: https://dev.twitter.com/overview/general/security-best-practices
- type: x-statistics
  url: https://docs.fabric.io/unity/answers/overview.html
- type: x-status
  url: https://dev.twitter.com/overview/status
- type: x-streaming
  url: https://dev.twitter.com/streaming/overview
- type: x-support
  url: https://support.twitter.com/
- type: x-terms-of-service
  url: https://dev.twitter.com/overview/terms
- type: x-transparency-report
  url: https://transparency.twitter.com/
- type: x-twitter
  url: https://twitter.com/Twitter
- type: x-twitter
  url: https://twitter.com/twitterapi/
- type: x-twitter
  url: https://twitter.com/twittereng/
- type: x-website
  url: https://twitter.com/
- type: x-wordpress
  url: https://dev.twitter.com/web/wordpress
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---