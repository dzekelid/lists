---
swagger: "2.0"
x-collection-name: AWS S3
x-complete: 0
info:
  title: AWS S3 List Bucket Metrics
  version: 1.0.0
  description: Lists the metrics configurations for the CloudWatch request metrics
    of the bucket
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?analytics:
    get:
      summary: List Bucket Analytics Configurations
      description: This implementation of the GET operation returns a list of analyticsconfigurations
        for the bucket
      operationId: list-bucket-analytics-configurations
      x-api-path-slug: analytics-get
      parameters:
      - in: query
        name: ContinuationToken
        description: The marker that is used to continue an analytics configuration
          listing that has beenttttttttttruncated
      responses:
        200:
          description: OK
      tags:
      - List
      - Bucket
      - Analytics
      - Configurations
  /?inventory:
    get:
      summary: List Bucket Inventory Configurations
      description: This implementation of the GET operation returns a list of inventoryconfigurations
        for the bucket
      operationId: list-bucket-inventory-configurations
      x-api-path-slug: inventory-get
      parameters:
      - in: query
        name: ContinuationToken
        description: The marker that is used to continue an inventory configuration
          listing that has beenttttttttttruncated
      responses:
        200:
          description: OK
      tags:
      - List
      - Bucket
      - Inventory
      - Configurations
  /?metrics:
    get:
      summary: List Bucket Metrics
      description: Lists the metrics configurations for the CloudWatch request metrics
        of the bucket
      operationId: list-bucket-metrics
      x-api-path-slug: metrics-get
      parameters:
      - in: query
        name: BucketName
        description: The name of the bucket containing the metrics configurationstttttttttto
          retrieve
      - in: query
        name: ContinuationToken
        description: The marker that is used to continue a metrics configurationtttttttttlisting
          that has been truncated
      responses:
        200:
          description: OK
      tags:
      - List
      - Bucket
      - Metrics
  /?uploads:
    get:
      summary: List Multipart Uploads
      description: This operation lists in-progress multipart uploads
      operationId: list-multipart-uploads
      x-api-path-slug: uploads-get
      parameters:
      - in: query
        name: delimiter
        description: Character you use to group keys
      - in: query
        name: encoding-type
        description: Requests Amazon S3 to encode the response and specifies the encoding
          method totttttttttuse
      - in: query
        name: key-marker
        description: Together with upload-id-marker, this parameter specifies the
          multiparttttttttttupload after which listing should begin
      - in: query
        name: max-uploads
        description: Sets the maximum number of multipart uploads, from 1 to 1,000,
          to return in thetttttttttresponse body
      - in: query
        name: prefix
        description: Lists in-progress uploads only for those keys that begin with
          the specified prefix
      - in: query
        name: upload-id-&#8203;marker
        description: Together with key-marker, specifies the multipart upload after
          whichtttttttttlisting should begin
      responses:
        200:
          description: OK
      tags:
      - List
      - Multipart
      - Uploads
  /ObjectName?uploadId=UploadId:
    get:
      summary: List Parts
      description: This operation lists the parts that have been uploaded for a specific
        multipart upload
      operationId: list-parts
      x-api-path-slug: objectnameuploadiduploadid-get
      parameters:
      - in: query
        name: encoding-type
        description: Requests Amazon S3 to encode the response and specifies the encoding
          method totttttttttuse
      - in: query
        name: max-parts
        description: Sets the maximum number of parts to return in the response body
      - in: query
        name: part-number&#8203;-marker
        description: Specifies the part after which listing should begin
      - in: query
        name: uploadId
        description: Upload ID identifying the multipart upload whose parts are being
          listed
      responses:
        200:
          description: OK
      tags:
      - List
      - Parts
  /?list-type=2:
    get:
      summary: GET Bucket (List Objects) Version 2
      description: This implementation of the GET operation returns some or all (up
        to 1,000) ofthe objects in a bucket
      operationId: get-bucket-list-objects-version-2
      x-api-path-slug: listtype2-get
      parameters:
      - in: query
        name: continuation-token
        description: When the Amazon S3 response to this API call is truncated (that
          is, IsTruncated responsetttttttttelement value is true), the response also
          includes thettttttttttNextContinuationToken element, the value of whichtttttttttyou
          can use in the next request as thettttttttttcontinuation-token to list the
          next settttttttttof objects
      - in: query
        name: delimiter
        description: A delimiter is a character you use to group keys
      - in: query
        name: encoding-type
        description: Requests Amazon S3 to encode the response and specifies the encoding
          method totttttttttuse
      - in: query
        name: fetch-owner
        description: By default, the API does not return the Owner information in
          the response
      - in: query
        name: list-type
        description: Version 2 of the API requires this parameter and you must set
          its value to 2
      - in: query
        name: max-keys
        description: Sets the maximum number of keys returned in the response body
      - in: query
        name: prefix
        description: Limits the response to keys that begin with the specifiedtttttttttprefix
      - in: query
        name: start-after
        description: If you want the API to return key names after a specifictttttttttobject
          key in your key space, you can add this parameter
      responses:
        200:
          description: OK
      tags:
      - Bucket
      - (List
      - Objects)
      - Version
      - "2"
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