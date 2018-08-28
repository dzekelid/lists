---
swagger: "2.0"
x-collection-name: AWS CloudFront
x-complete: 0
info:
  title: AWS CloudFront API List Tags For Resource
  version: 1.0.0
  description: List tags for a CloudFront resource.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ListCloudFrontOriginAccessIdentities:
    get:
      summary: List Cloud Front Origin Access Identities
      description: Lists origin access identities.
      operationId: listCloudFrontOriginAccessIdentities
      x-api-path-slug: actionlistcloudfrontoriginaccessidentities-get
      parameters:
      - in: query
        name: Affinity
        description: The new affinity setting for the instance
        type: string
      - in: query
        name: HostId
        description: The ID of the Dedicated Host that the instance will have affinity
          with
        type: string
      - in: query
        name: InstanceId
        description: The ID of the instance that you are modifying
        type: string
      - in: query
        name: Marker
        description: Use this when paginating results to indicate where to begin in
          your list of origin      access identities
        type: string
      - in: query
        name: MaxItems
        description: The maximum number of origin access identities you want in the
          response body
        type: string
      - in: query
        name: Tenancy
        description: The tenancy of the instance that you are modifying
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Cloud
      - Front
      - Origin
      - Access
      - Identities
  /?Action=ListDistributions:
    get:
      summary: List Distributions
      description: List distributions.
      operationId: listDistributions
      x-api-path-slug: actionlistdistributions-get
      parameters:
      - in: query
        name: ClientToken
        description: Unique, case-sensitive identifier you provide to ensure idempotency
          of the request
        type: string
      - in: query
        name: CurrencyCode
        description: The currency in which the totalUpfrontPrice, LimitPrice,            and
          totalHourlyPrice amounts are specified
        type: string
      - in: query
        name: HostIdSet.N
        description: The ID/s of the Dedicated Host/s that the reservation will be
          associated            with
        type: string
      - in: query
        name: LimitPrice
        description: The specified limit is checked against the total upfront cost
          of the reservation            (calculated as the offerings upfront cost
          multiplied by the host count)
        type: string
      - in: query
        name: Marker
        description: Use this when paginating results to indicate where to begin in
          your list of      distributions
        type: string
      - in: query
        name: MaxItems
        description: The maximum number of distributions you want in the response
          body
        type: string
      - in: query
        name: OfferingId
        description: The ID of the offering
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Distributions
  /?Action=ListDistributionsByWebACLId:
    get:
      summary: List Distributions By Web A C L Id
      description: List the distributions that are associated with a specified AWS
        WAF web ACL.
      operationId: listDistributionsByWebACLId
      x-api-path-slug: actionlistdistributionsbywebaclid-get
      parameters:
      - in: query
        name: HostId.N
        description: The IDs of the Dedicated Hosts you want to release
        type: string
      - in: query
        name: Marker
        description: Use Marker and MaxItems to control pagination of results
        type: string
      - in: query
        name: MaxItems
        description: The maximum number of distributions that you want CloudFront
          to return in the response body
        type: string
      - in: query
        name: WebACLId
        description: The ID of the AWS WAF web ACL that you want to list the associated
          distributions
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Distributions
      - Web
      - C
      - L
      - Id
  /?Action=ListInvalidations:
    get:
      summary: List Invalidations
      description: Lists invalidation batches.
      operationId: listInvalidations
      x-api-path-slug: actionlistinvalidations-get
      parameters:
      - in: query
        name: DhcpOptionsId
        description: The ID of the DHCP options set, or default to associate         no
          DHCP options with the VPC
        type: string
      - in: query
        name: DistributionId
        description: The distributions ID
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: Marker
        description: Use this parameter when paginating results to indicate where
          to begin in your list of      invalidation batches
        type: string
      - in: query
        name: MaxItems
        description: The maximum number of invalidation batches that you want in the
          response      body
        type: string
      - in: query
        name: VpcId
        description: The ID of the VPC
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Invalidations
  /?Action=ListStreamingDistributions:
    get:
      summary: List Streaming Distributions
      description: List streaming distributions.
      operationId: listStreamingDistributions
      x-api-path-slug: actionliststreamingdistributions-get
      parameters:
      - in: query
        name: DhcpConfiguration.N
        description: A DHCP configuration option
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: Marker
        description: The value that you provided for the Marker request parameter
        type: string
      - in: query
        name: MaxItems
        description: The value that you provided for the MaxItems request parameter
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Streaming
      - Distributions
  /?Action=ListTagsForResource:
    get:
      summary: List Tags For Resource
      description: List tags for a CloudFront resource.
      operationId: listTagsForResource
      x-api-path-slug: actionlisttagsforresource-get
      parameters:
      - in: query
        name: DhcpOptionsId
        description: The ID of the DHCP options set
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: Resource
        description: An ARN of a CloudFront resource
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Tags
      - Resource
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