---
swagger: "2.0"
x-collection-name: AWS Code Pipeline
x-complete: 0
info:
  title: AWS Code Pipeline API List Pipelines
  version: 1.0.0
  description: Gets a summary of all of the pipelines associated with your account.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ListActionTypes:
    get:
      summary: List Action Types
      description: |-
        Gets a summary of all AWS CodePipeline action types associated with your
                    account.
      operationId: listActionTypes
      x-api-path-slug: actionlistactiontypes-get
      parameters:
      - in: query
        name: actionOwnerFilter
        description: Filters the list of action types to those created by a specified
          entity
        type: string
      - in: query
        name: AllocationId
        description: '[EC2-VPC] The allocation ID'
        type: string
      - in: query
        name: AllowReassociation
        description: '[EC2-VPC] For a VPC in an EC2-Classic account, specify true
          to allow an Elastic IP address that is already associated with an instance
          or network interface to be reassociated with the specified instance or network
          interface'
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: InstanceId
        description: The ID of the instance
        type: string
      - in: query
        name: NetworkInterfaceId
        description: '[EC2-VPC] The ID of the network interface'
        type: string
      - in: query
        name: nextToken
        description: An identifier that was returned from the previous list action
          types call, which can            be used to return the next set of action
          types in the list
        type: string
      - in: query
        name: PrivateIpAddress
        description: '[EC2-VPC] The primary or secondary private IP address to associate
          with the Elastic IP address'
        type: string
      - in: query
        name: PublicIp
        description: The Elastic IP address
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Action
      - Types
  /?Action=ListPipelines:
    get:
      summary: List Pipelines
      description: Gets a summary of all of the pipelines associated with your account.
      operationId: listPipelines
      x-api-path-slug: actionlistpipelines-get
      parameters:
      - in: query
        name: AllocationId.N
        description: '[EC2-VPC] One or more allocation IDs'
        type: string
      - in: query
        name: DryRun
        description: Checks whether you have the required permissions for the action,
          without actually making the request,        and provides an error response
        type: string
      - in: query
        name: Filter.N
        description: One or more filters
        type: string
      - in: query
        name: nextToken
        description: An identifier that was returned from the previous list pipelines
          call, which can be            used to return the next set of pipelines in
          the list
        type: string
      - in: query
        name: PublicIp.N
        description: '[EC2-Classic] One or more Elastic IP addresses'
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Pipelines
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