---
swagger: "2.0"
x-collection-name: AWS EC2 Systems Manager
x-complete: 0
info:
  title: Amazon EC2 Systems Manager API List Tags For Resource
  version: 1.0.0
  description: Returns a list of the tags assigned to the specified resource.
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /?Action=ListAssociations:
    get:
      summary: List Associations
      description: Lists the associations for the specified SSM document or instance.
      operationId: listAssociations
      x-api-path-slug: actionlistassociations-get
      parameters:
      - in: query
        name: AssociationFilterList
        description: One or more filters
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of items to return for this call
        type: string
      - in: query
        name: NextToken
        description: The token for the next set of items to return
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Associations
  /?Action=ListCommandInvocations:
    get:
      summary: List Command Invocations
      description: An invocation is copy of a command sent to a specific instance.
      operationId: listCommandInvocations
      x-api-path-slug: actionlistcommandinvocations-get
      parameters:
      - in: query
        name: CommandId
        description: (Optional) The invocations for a specific command ID
        type: string
      - in: query
        name: Details
        description: (Optional) If set this returns the response of the command executions
          and any command   output
        type: string
      - in: query
        name: Filters
        description: (Optional) One or more filters
        type: string
      - in: query
        name: InstanceId
        description: (Optional) The command execution details for a specific instance
          ID
        type: string
      - in: query
        name: MaxResults
        description: (Optional) The maximum number of items to return for this call
        type: string
      - in: query
        name: NextToken
        description: (Optional) The token for the next set of items to return
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Command
      - Invocations
  /?Action=ListCommands:
    get:
      summary: List Commands
      description: Lists the commands requested by users of the AWS account.
      operationId: listCommands
      x-api-path-slug: actionlistcommands-get
      parameters:
      - in: query
        name: CommandId
        description: (Optional) If provided, lists only the specified command
        type: string
      - in: query
        name: Filters
        description: (Optional) One or more filters
        type: string
      - in: query
        name: InstanceId
        description: (Optional) Lists commands issued against this instance ID
        type: string
      - in: query
        name: MaxResults
        description: (Optional) The maximum number of items to return for this call
        type: string
      - in: query
        name: NextToken
        description: (Optional) The token for the next set of items to return
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Commands
  /?Action=ListDocuments:
    get:
      summary: List Documents
      description: Describes one or more of your SSM documents.
      operationId: listDocuments
      x-api-path-slug: actionlistdocuments-get
      parameters:
      - in: query
        name: DocumentFilterList
        description: One or more filters
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of items to return for this call
        type: string
      - in: query
        name: NextToken
        description: The token for the next set of items to return
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Documents
  /?Action=ListDocumentVersions:
    get:
      summary: List Document Versions
      description: List all versions for a document.
      operationId: listDocumentVersions
      x-api-path-slug: actionlistdocumentversions-get
      parameters:
      - in: query
        name: MaxResults
        description: The maximum number of items to return for this call
        type: string
      - in: query
        name: Name
        description: The name of the document about which you want version information
        type: string
      - in: query
        name: NextToken
        description: The token for the next set of items to return
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Document
      - Versions
  /?Action=ListInventoryEntries:
    get:
      summary: List Inventory Entries
      description: A list of inventory items returned by the request.
      operationId: listInventoryEntries
      x-api-path-slug: actionlistinventoryentries-get
      parameters:
      - in: query
        name: Filters
        description: One or more filters
        type: string
      - in: query
        name: InstanceId
        description: The instance ID for which you want inventory information
        type: string
      - in: query
        name: MaxResults
        description: The maximum number of items to return for this call
        type: string
      - in: query
        name: NextToken
        description: The token for the next set of items to return
        type: string
      - in: query
        name: TypeName
        description: The type of inventory item for which you want information
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - Inventory
      - Entries
  /?Action=ListTagsForResource:
    get:
      summary: List Tags For Resource
      description: Returns a list of the tags assigned to the specified resource.
      operationId: listTagsForResource
      x-api-path-slug: actionlisttagsforresource-get
      parameters:
      - in: query
        name: ResourceId
        description: The resource ID for which you want to see a list of tags
        type: string
      - in: query
        name: ResourceType
        description: Returns a list of tags for a specific resource type
        type: string
      responses:
        200:
          description: OK
      tags:
      - List
      - TagsResource
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