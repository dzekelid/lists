---
swagger: "2.0"
x-collection-name: DigitalOcean
x-complete: 0
info:
  title: Digital Ocean List all Sizes
  description: "To list all of the sizes, send a GET request to /v2/sizes.\r\n\r\nThe
    response will be a JSON object with a key called _sizes_."
  version: 1.0.0
host: example.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /certificates:
    get:
      summary: List all certificates
      description: "To list all of the certificates available on your account, send
        a GET request to /v2/certificates.\r\n\r\nThe result will be a JSON object
        with a certificates key. This will be set to an array of certificate objects,
        each of which will contain the standard certificate attributes:"
      operationId: CertificatesGet
      x-api-path-slug: certificates-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - List
      - ""
      - Certificates
  /domains:
    get:
      summary: List all Domains
      description: "To retrieve a list of all of the domains in your account, send
        a GET request to /v2/domains.\r\n\r\nThe response will be a JSON object with
        a key called domains."
      operationId: DomainsGet
      x-api-path-slug: domains-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - List
      - ""
      - Domains
  /regions:
    get:
      summary: List all Regions
      description: "To list all of the regions that are available, send a GET request
        to /v2/regions.\r\n\r\nThe response will be a JSON object with a key called
        _regions_."
      operationId: RegionsGet
      x-api-path-slug: regions-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - List
      - ""
      - Regions
  /snapshots:
    get:
      summary: List all Volume snapshots
      description: To retrieve only snapshots based on volumes, include the resource_type
        query paramter set to volume, /v2/snapshots?resource_type=volume.
      operationId: SnapshotsGet3
      x-api-path-slug: snapshots-get
      parameters:
      - in: header
        name: Content-Type
      - in: query
        name: page
      - in: query
        name: per_page
      - in: query
        name: resource_type
      responses:
        200:
          description: OK
      tags:
      - List
      - ""
      - Volume
      - Snapshots
  /sizes:
    get:
      summary: List all Sizes
      description: "To list all of the sizes, send a GET request to /v2/sizes.\r\n\r\nThe
        response will be a JSON object with a key called _sizes_."
      operationId: SizesGet
      x-api-path-slug: sizes-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - List
      - ""
      - Sizes
  /account/keys:
    get:
      summary: List all Keys
      description: "To list all of the keys in your account, send a GET request to
        /v2/account/keys.\r\n\r\nThe response will be a JSON object with a key set
        to _ssh_keys_."
      operationId: AccountKeysGet
      x-api-path-slug: accountkeys-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - List
      - ""
      - Keys
  /tags:
    get:
      summary: List all Tags
      description: "To list all of your tags, you can send a GET request to /v2/tags.\r\n\r\nThe
        response will be a JSON object with a key called _tags_."
      operationId: TagsGet
      x-api-path-slug: tags-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - List
      - ""
      - Tags
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---