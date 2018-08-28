---
name: DigitalOcean
x-slug: digitalocean
description: DigitalOcean is a simple and fast cloud hosting service built for developers.
  Customers can create a cloud server in 55 seconds, and pricing plans start at only
  $5 per month for 512MB of RAM, 20GB SSD, 1 CPU, and 1TB Transfer. Featuring a 99.99%
  Uptime SLA, DigitalOcean has servers located in New York, San Francisco, and Amsterdam.
  The DigitalOcean control panel interface is simple and intuitive, which power users
  can replicate on a larger scale with the company&rsquo;s API. DigitalOcean uses
  KVM virtualization and additionally hosts a library of helpful walkthroughs and
  tutorials that cover server configuration and optimization.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/DO_Logo_Horizontal_Black-3500c326.png
x-kinRank: "7"
x-alexaRank: "0"
tags: Lists
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/digitalocean/apis.md
specificationVersion: "0.14"
apis:
- name: DigitalOcean API-V2 - List all certificates
  x-api-slug: certificates-get
  description: "To list all of the certificates available on your account, send a
    GET request to /v2/certificates.\r\n\r\nThe result will be a JSON object with
    a certificates key. This will be set to an array of certificate objects, each
    of which will contain the standard certificate attributes:"
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/DO_Logo_Horizontal_Black-3500c326.png
  humanURL: https://www.digitalocean.com
  baseURL: https://example.com//
  tags: Cloud, Compute, Hosting, API Provider, API Service Provider, Profiles, Service
    API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/digitalocean/certificates-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/digitalocean/certificates-get-openapi.md
- name: DigitalOcean API-V2 - List all certificates
  x-api-slug: certificates-get
  description: "To list all of the certificates available on your account, send a
    GET request to /v2/certificates.\r\n\r\nThe result will be a JSON object with
    a certificates key. This will be set to an array of certificate objects, each
    of which will contain the standard certificate attributes:"
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/DO_Logo_Horizontal_Black-3500c326.png
  humanURL: https://www.digitalocean.com
  baseURL: https://example.com//
  tags: Cloud, Compute, Hosting, API Provider, API Service Provider, Profiles, Service
    API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/digitalocean/certificates-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/digitalocean/certificates-get-openapi.md
- name: DigitalOcean API-V2 - List all Domains
  x-api-slug: domains-get
  description: "To retrieve a list of all of the domains in your account, send a GET
    request to /v2/domains.\r\n\r\nThe response will be a JSON object with a key called
    domains."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/DO_Logo_Horizontal_Black-3500c326.png
  humanURL: https://www.digitalocean.com
  baseURL: https://example.com//
  tags: Cloud, Compute, Hosting, API Provider, API Service Provider, Profiles, Service
    API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/digitalocean/domains-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/digitalocean/domains-get-openapi.md
- name: DigitalOcean API-V2 - List all Domains
  x-api-slug: domains-get
  description: "To retrieve a list of all of the domains in your account, send a GET
    request to /v2/domains.\r\n\r\nThe response will be a JSON object with a key called
    domains."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/DO_Logo_Horizontal_Black-3500c326.png
  humanURL: https://www.digitalocean.com
  baseURL: https://example.com//
  tags: Cloud, Compute, Hosting, API Provider, API Service Provider, Profiles, Service
    API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/digitalocean/domains-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/digitalocean/domains-get-openapi.md
- name: DigitalOcean API-V2 - List all Regions
  x-api-slug: regions-get
  description: "To list all of the regions that are available, send a GET request
    to /v2/regions.\r\n\r\nThe response will be a JSON object with a key called _regions_."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/DO_Logo_Horizontal_Black-3500c326.png
  humanURL: https://www.digitalocean.com
  baseURL: https://example.com//
  tags: Cloud, Compute, Hosting, API Provider, API Service Provider, Profiles, Service
    API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/digitalocean/regions-get-openapi.md
- name: DigitalOcean API-V2 - List all Regions
  x-api-slug: regions-get
  description: "To list all of the regions that are available, send a GET request
    to /v2/regions.\r\n\r\nThe response will be a JSON object with a key called _regions_."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/DO_Logo_Horizontal_Black-3500c326.png
  humanURL: https://www.digitalocean.com
  baseURL: https://example.com//
  tags: Cloud, Compute, Hosting, API Provider, API Service Provider, Profiles, Service
    API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/digitalocean/regions-get-openapi.md
- name: DigitalOcean API-V2 - List all Volume snapshots
  x-api-slug: snapshots-get
  description: To retrieve only snapshots based on volumes, include the resource_type
    query paramter set to volume, /v2/snapshots?resource_type=volume.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/DO_Logo_Horizontal_Black-3500c326.png
  humanURL: https://www.digitalocean.com
  baseURL: https://example.com//
  tags: Cloud, Compute, Hosting, API Provider, API Service Provider, Profiles, Service
    API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/digitalocean/snapshots-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/digitalocean/snapshots-get-openapi.md
- name: DigitalOcean API-V2 - List all Volume snapshots
  x-api-slug: snapshots-get
  description: To retrieve only snapshots based on volumes, include the resource_type
    query paramter set to volume, /v2/snapshots?resource_type=volume.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/DO_Logo_Horizontal_Black-3500c326.png
  humanURL: https://www.digitalocean.com
  baseURL: https://example.com//
  tags: Cloud, Compute, Hosting, API Provider, API Service Provider, Profiles, Service
    API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/digitalocean/snapshots-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/digitalocean/snapshots-get-openapi.md
- name: DigitalOcean API-V2 - List all Sizes
  x-api-slug: sizes-get
  description: "To list all of the sizes, send a GET request to /v2/sizes.\r\n\r\nThe
    response will be a JSON object with a key called _sizes_."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/DO_Logo_Horizontal_Black-3500c326.png
  humanURL: https://www.digitalocean.com
  baseURL: https://example.com//
  tags: Cloud, Compute, Hosting, API Provider, API Service Provider, Profiles, Service
    API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/digitalocean/sizes-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/digitalocean/sizes-get-openapi.md
- name: DigitalOcean API-V2 - List all Sizes
  x-api-slug: sizes-get
  description: "To list all of the sizes, send a GET request to /v2/sizes.\r\n\r\nThe
    response will be a JSON object with a key called _sizes_."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/DO_Logo_Horizontal_Black-3500c326.png
  humanURL: https://www.digitalocean.com
  baseURL: https://example.com//
  tags: Cloud, Compute, Hosting, API Provider, API Service Provider, Profiles, Service
    API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/digitalocean/sizes-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/digitalocean/sizes-get-openapi.md
- name: DigitalOcean API-V2 - List all Keys
  x-api-slug: accountkeys-get
  description: "To list all of the keys in your account, send a GET request to /v2/account/keys.\r\n\r\nThe
    response will be a JSON object with a key set to _ssh_keys_."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/DO_Logo_Horizontal_Black-3500c326.png
  humanURL: https://www.digitalocean.com
  baseURL: https://example.com//
  tags: Cloud, Compute, Hosting, API Provider, API Service Provider, Profiles, Service
    API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/digitalocean/accountkeys-get-openapi.md
- name: DigitalOcean API-V2 - List all Keys
  x-api-slug: accountkeys-get
  description: "To list all of the keys in your account, send a GET request to /v2/account/keys.\r\n\r\nThe
    response will be a JSON object with a key set to _ssh_keys_."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/DO_Logo_Horizontal_Black-3500c326.png
  humanURL: https://www.digitalocean.com
  baseURL: https://example.com//
  tags: Cloud, Compute, Hosting, API Provider, API Service Provider, Profiles, Service
    API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/digitalocean/accountkeys-get-openapi.md
- name: DigitalOcean API-V2 - List all Tags
  x-api-slug: tags-get
  description: "To list all of your tags, you can send a GET request to /v2/tags.\r\n\r\nThe
    response will be a JSON object with a key called _tags_."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/DO_Logo_Horizontal_Black-3500c326.png
  humanURL: https://www.digitalocean.com
  baseURL: https://example.com//
  tags: Cloud, Compute, Hosting, API Provider, API Service Provider, Profiles, Service
    API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/digitalocean/tags-get-openapi.md
- name: DigitalOcean API-V2 - List all Tags
  x-api-slug: tags-get
  description: "To list all of your tags, you can send a GET request to /v2/tags.\r\n\r\nThe
    response will be a JSON object with a key called _tags_."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/DO_Logo_Horizontal_Black-3500c326.png
  humanURL: https://www.digitalocean.com
  baseURL: https://example.com//
  tags: Cloud, Compute, Hosting, API Provider, API Service Provider, Profiles, Service
    API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/digitalocean/tags-get-openapi.md
- name: DigitalOcean API-V2 - List all Tags
  x-api-slug: tags-get
  description: "To list all of your tags, you can send a GET request to /v2/tags.\r\n\r\nThe
    response will be a JSON object with a key called _tags_."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/DO_Logo_Horizontal_Black-3500c326.png
  humanURL: https://www.digitalocean.com
  baseURL: https://example.com//
  tags: Cloud, Compute, Hosting, API Provider, API Service Provider, Profiles, Service
    API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/digitalocean/tags-get-openapi.md
- name: DigitalOcean API-V2 - List all Keys
  x-api-slug: accountkeys-get
  description: "To list all of the keys in your account, send a GET request to /v2/account/keys.\r\n\r\nThe
    response will be a JSON object with a key set to _ssh_keys_."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/DO_Logo_Horizontal_Black-3500c326.png
  humanURL: https://www.digitalocean.com
  baseURL: https://example.com//
  tags: Cloud, Compute, Hosting, API Provider, API Service Provider, Profiles, Service
    API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/digitalocean/accountkeys-get-openapi.md
- name: DigitalOcean API-V2 - List all Keys
  x-api-slug: accountkeys-get
  description: "To list all of the keys in your account, send a GET request to /v2/account/keys.\r\n\r\nThe
    response will be a JSON object with a key set to _ssh_keys_."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/DO_Logo_Horizontal_Black-3500c326.png
  humanURL: https://www.digitalocean.com
  baseURL: https://example.com//
  tags: Cloud, Compute, Hosting, API Provider, API Service Provider, Profiles, Service
    API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/digitalocean/accountkeys-get-openapi.md
- name: DigitalOcean API-V2 - List all Sizes
  x-api-slug: sizes-get
  description: "To list all of the sizes, send a GET request to /v2/sizes.\r\n\r\nThe
    response will be a JSON object with a key called _sizes_."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/DO_Logo_Horizontal_Black-3500c326.png
  humanURL: https://www.digitalocean.com
  baseURL: https://example.com//
  tags: Cloud, Compute, Hosting, API Provider, API Service Provider, Profiles, Service
    API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/digitalocean/sizes-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/digitalocean/sizes-get-openapi.md
- name: DigitalOcean API-V2 - List all Sizes
  x-api-slug: sizes-get
  description: "To list all of the sizes, send a GET request to /v2/sizes.\r\n\r\nThe
    response will be a JSON object with a key called _sizes_."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/DO_Logo_Horizontal_Black-3500c326.png
  humanURL: https://www.digitalocean.com
  baseURL: https://example.com//
  tags: Cloud, Compute, Hosting, API Provider, API Service Provider, Profiles, Service
    API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/digitalocean/sizes-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/digitalocean/sizes-get-openapi.md
- name: DigitalOcean API-V2 - List all Volume snapshots
  x-api-slug: snapshots-get
  description: To retrieve only snapshots based on volumes, include the resource_type
    query paramter set to volume, /v2/snapshots?resource_type=volume.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/DO_Logo_Horizontal_Black-3500c326.png
  humanURL: https://www.digitalocean.com
  baseURL: https://example.com//
  tags: Cloud, Compute, Hosting, API Provider, API Service Provider, Profiles, Service
    API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/digitalocean/snapshots-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/digitalocean/snapshots-get-openapi.md
- name: DigitalOcean API-V2 - List all Volume snapshots
  x-api-slug: snapshots-get
  description: To retrieve only snapshots based on volumes, include the resource_type
    query paramter set to volume, /v2/snapshots?resource_type=volume.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/DO_Logo_Horizontal_Black-3500c326.png
  humanURL: https://www.digitalocean.com
  baseURL: https://example.com//
  tags: Cloud, Compute, Hosting, API Provider, API Service Provider, Profiles, Service
    API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/digitalocean/snapshots-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/digitalocean/snapshots-get-openapi.md
- name: DigitalOcean API-V2 - List all Regions
  x-api-slug: regions-get
  description: "To list all of the regions that are available, send a GET request
    to /v2/regions.\r\n\r\nThe response will be a JSON object with a key called _regions_."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/DO_Logo_Horizontal_Black-3500c326.png
  humanURL: https://www.digitalocean.com
  baseURL: https://example.com//
  tags: Cloud, Compute, Hosting, API Provider, API Service Provider, Profiles, Service
    API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/digitalocean/regions-get-openapi.md
- name: DigitalOcean API-V2 - List all Regions
  x-api-slug: regions-get
  description: "To list all of the regions that are available, send a GET request
    to /v2/regions.\r\n\r\nThe response will be a JSON object with a key called _regions_."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/DO_Logo_Horizontal_Black-3500c326.png
  humanURL: https://www.digitalocean.com
  baseURL: https://example.com//
  tags: Cloud, Compute, Hosting, API Provider, API Service Provider, Profiles, Service
    API, Relative Data
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/digitalocean/regions-get-openapi.md
- name: DigitalOcean API-V2 - List all Domains
  x-api-slug: domains-get
  description: "To retrieve a list of all of the domains in your account, send a GET
    request to /v2/domains.\r\n\r\nThe response will be a JSON object with a key called
    domains."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/DO_Logo_Horizontal_Black-3500c326.png
  humanURL: https://www.digitalocean.com
  baseURL: https://example.com//
  tags: Cloud, Compute, Hosting, API Provider, API Service Provider, Profiles, Service
    API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/digitalocean/domains-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/digitalocean/domains-get-openapi.md
- name: DigitalOcean API-V2 - List all Domains
  x-api-slug: domains-get
  description: "To retrieve a list of all of the domains in your account, send a GET
    request to /v2/domains.\r\n\r\nThe response will be a JSON object with a key called
    domains."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/DO_Logo_Horizontal_Black-3500c326.png
  humanURL: https://www.digitalocean.com
  baseURL: https://example.com//
  tags: Cloud, Compute, Hosting, API Provider, API Service Provider, Profiles, Service
    API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/digitalocean/domains-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/digitalocean/domains-get-openapi.md
- name: DigitalOcean API-V2 - List all Domains
  x-api-slug: domains-get
  description: "To retrieve a list of all of the domains in your account, send a GET
    request to /v2/domains.\r\n\r\nThe response will be a JSON object with a key called
    domains."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/DO_Logo_Horizontal_Black-3500c326.png
  humanURL: https://www.digitalocean.com
  baseURL: https://example.com//
  tags: Cloud, Compute, Hosting, API Provider, API Service Provider, Profiles, Service
    API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/digitalocean/domains-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/digitalocean/domains-get-openapi.md
- name: DigitalOcean API-V2 - List all certificates
  x-api-slug: certificates-get
  description: "To list all of the certificates available on your account, send a
    GET request to /v2/certificates.\r\n\r\nThe result will be a JSON object with
    a certificates key. This will be set to an array of certificate objects, each
    of which will contain the standard certificate attributes:"
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/DO_Logo_Horizontal_Black-3500c326.png
  humanURL: https://www.digitalocean.com
  baseURL: https://example.com//
  tags: Cloud, Compute, Hosting, API Provider, API Service Provider, Profiles, Service
    API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/digitalocean/certificates-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/digitalocean/certificates-get-openapi.md
- name: DigitalOcean API-V2 - List all certificates
  x-api-slug: certificates-get
  description: "To list all of the certificates available on your account, send a
    GET request to /v2/certificates.\r\n\r\nThe result will be a JSON object with
    a certificates key. This will be set to an array of certificate objects, each
    of which will contain the standard certificate attributes:"
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/DO_Logo_Horizontal_Black-3500c326.png
  humanURL: https://www.digitalocean.com
  baseURL: https://example.com//
  tags: Cloud, Compute, Hosting, API Provider, API Service Provider, Profiles, Service
    API, Relative Data
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/digitalocean/certificates-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/digitalocean/certificates-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://digital.river.api.gallery.streamdata.io
- type: x-api-stack
  url: http://digitalocean.stack.network
- type: x-base
  url: https://api.digitalocean.com/
- type: x-blog
  url: https://www.digitalocean.com/company/blog/
- type: x-blog-rss
  url: https://www.digitalocean.com/company/blog/feed.xml
- type: x-command-line-interface
  url: https://github.com/digitalocean/doctl
- type: x-developer
  url: https://developers.digitalocean.com/
- type: x-github
  url: https://github.com/digitalocean
- type: x-twitter
  url: https://twitter.com/digitalocean
- type: x-website
  url: https://www.digitalocean.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---