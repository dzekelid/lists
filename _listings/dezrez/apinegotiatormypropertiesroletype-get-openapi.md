---
swagger: "2.0"
x-collection-name: Dezrez
x-complete: 0
info:
  title: Dezrez Used for the Property Sales Dashboard to return a list of the negotiator's
    properties.
  version: 1.0.0
  description: Used for the property sales dashboard to return a list of the negotiator's
    properties..
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/admin/businessworkflow/{workflowName}:
    get:
      summary: Lists instances of a given workflow
      description: Lists instances of a given workflow.
      operationId: BusinessWorkflow_ListWorkflowInstancesByworkflowNameByskipBytake
      x-api-path-slug: apiadminbusinessworkflowworkflowname-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: skip
      - in: query
        name: take
      - in: path
        name: workflowName
      responses:
        200:
          description: OK
      tags:
      - Lists
      - Instances
      - Of
      - Given
      - Workflow
  /api/negotiator/my/properties/favourite:
    get:
      summary: Lists favourited properties
      description: Lists favourited properties.
      operationId: Negotiator_FavouritePropertiesBypageSizeBypageNumber
      x-api-path-slug: apinegotiatormypropertiesfavourite-get
      parameters:
      - in: query
        name: pageNumber
        description: Page number
      - in: query
        name: pageSize
        description: Page Size
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Lists
      - Favourited
      - Properties
  /api/admin/system/ListAgencies:
    get:
      summary: Lists the name and ID of all agencies in the system.
      description: Lists the name and id of all agencies in the system..
      operationId: System_ListAgenciesByincludeSuspended
      x-api-path-slug: apiadminsystemlistagencies-get
      parameters:
      - in: query
        name: includeSuspended
        description: if set to true [include suspended]
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Lists
      - Name
      - ID
      - Of
      - ""
      - Agencies
      - In
      - System
  /api/webhook/list:
    get:
      summary: Lists all of the webhooks currently set up.
      description: Lists all of the webhooks currently set up..
      operationId: Webhook_ListWebhooksBytriggerFilterName
      x-api-path-slug: apiwebhooklist-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: triggerFilterName
        description: Optionally, filter results that match this trigger
      responses:
        200:
          description: OK
      tags:
      - Lists
      - ""
      - Of
      - Webhooks
      - Currently
      - Set
      - Up
  /api/workflow/triggers:
    get:
      summary: Lists the available triggers that are able to start workflows.
      description: Lists the available triggers that are able to start workflows..
      operationId: Workflow_GetTriggerTypes
      x-api-path-slug: apiworkflowtriggers-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Lists
      - Available
      - Triggers
      - That
      - Are
      - Able
      - To
      - Start
      - Workflows
  /api/workflow/listWorkflows:
    get:
      summary: Lists available workflows
      description: Lists available workflows.
      operationId: Workflow_ListWorkflowsByskipBytake
      x-api-path-slug: apiworkflowlistworkflows-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: skip
        description: Used for paging results
      - in: query
        name: take
        description: Used for paging results
      responses:
        200:
          description: OK
      tags:
      - Lists
      - Available
      - Workflows
  /api/workflow/{workflowName}:
    get:
      summary: Lists instances of a given workflow
      description: Lists instances of a given workflow.
      operationId: Workflow_ListWorkflowInstancesByworkflowNameByskipBytake
      x-api-path-slug: apiworkflowworkflowname-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: skip
      - in: query
        name: take
      - in: path
        name: workflowName
      responses:
        200:
          description: OK
      tags:
      - Lists
      - Instances
      - Of
      - Given
      - Workflow
  /api/account/systemaccounts:
    get:
      summary: Get list of all system accounts
      description: Get list of all system accounts.
      operationId: Account_GetSystemAccounts
      x-api-path-slug: apiaccountsystemaccounts-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - ""
      - System
      - Accounts
  /api/account/pm/list:
    post:
      summary: Get list of accounts with sorting and searching and by type of group
        for the accounts
      description: Get list of accounts with sorting and searching and by type of
        group for the accounts.
      operationId: Account_GetPMAccountsBydataContractBypageSizeBypageNumber
      x-api-path-slug: apiaccountpmlist-post
      parameters:
      - in: body
        name: dataContract
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: pageNumber
      - in: query
        name: pageSize
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Accounts
      - Sorting
      - Searching
      - By
      - Type
      - Of
      - Groupthe
      - Accounts
  /api/accounting/exports/list/batches:
    get:
      summary: Get list of batch exports
      description: Get list of batch exports.
      operationId: AccountingExport_GetBatchPaymentsBybankAccountIdByincludeProcessed
      x-api-path-slug: apiaccountingexportslistbatches-get
      parameters:
      - in: query
        name: bankAccountId
      - in: query
        name: includeProcessed
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Batch
      - Exports
  /api/accountingsystem/officeaccounts:
    get:
      summary: Get list of office accounts associated with the accounting system
      description: Get list of office accounts associated with the accounting system.
      operationId: AccountingSystem_GetOfficeAccounts
      x-api-path-slug: apiaccountingsystemofficeaccounts-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Office
      - Accounts
      - Associated
      - Accounting
      - System
  /api/agency/teams:
    get:
      summary: Returns a list of team groups for the agency.
      description: Returns a list of team groups for the agency..
      operationId: Agency_TeamsBypageSizeBypageNumberByteamType
      x-api-path-slug: apiagencyteams-get
      parameters:
      - in: query
        name: pageNumber
      - in: query
        name: pageSize
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: teamType
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - Team
      - Groupsthe
      - Agency
  /api/agency/portalconfigurations:
    get:
      summary: Get a list of portal configurations for the brand within a branch.
      description: Get a list of portal configurations for the brand within a branch..
      operationId: Agency_PortalConfigurationsBypageSizeBypageNumber
      x-api-path-slug: apiagencyportalconfigurations-get
      parameters:
      - in: query
        name: pageNumber
      - in: query
        name: pageSize
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Portal
      - Configurationsthe
      - Brand
      - Within
      - Branch
  /api/analytics/campaigns:
    get:
      summary: returns a list of all of the campaigns for an agency
      description: Returns a list of all of the campaigns for an agency.
      operationId: Analytics_GetCampaigns
      x-api-path-slug: apianalyticscampaigns-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - ""
      - Of
      - Campaignsan
      - Agency
  /api/auction/{id}/confirmlots:
    post:
      summary: To confirm or unconfirm a list of lots for the auction
      description: To confirm or unconfirm a list of lots for the auction.
      operationId: Auction_ConfirmLotsByidByconfirmLotsDataContract
      x-api-path-slug: apiauctionidconfirmlots-post
      parameters:
      - in: body
        name: confirmLotsDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - To
      - Confirm
      - Unconfirm
      - List
      - Of
      - Lotsthe
      - Auction
  /api/auction/{id}/withdrawlots:
    post:
      summary: To withdraw a list of properties from the auction
      description: To withdraw a list of properties from the auction.
      operationId: Auction_WithdrawLotsByidBywithdrawLotsDataContract
      x-api-path-slug: apiauctionidwithdrawlots-post
      parameters:
      - in: path
        name: id
        description: The auction ID
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: withdrawLotsDataContract
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - To
      - Withdraw
      - List
      - Of
      - Properties
      - From
      - Auction
  /api/auction/{id}/postponelots:
    post:
      summary: To postpone a list of lots for the auction
      description: To postpone a list of lots for the auction.
      operationId: Auction_PostponeLotsByidBypostponeLotsDataContract
      x-api-path-slug: apiauctionidpostponelots-post
      parameters:
      - in: path
        name: id
        description: The auction ID
      - in: body
        name: postponeLotsDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - To
      - Postpone
      - List
      - Of
      - Lotsthe
      - Auction
  /api/cache/List/{listKey}:
    get:
      summary: Retrieves a list of objects stored in the cache system by its {listKey}
      description: Retrieves a list of objects stored in the cache system by its {listkey}.
      operationId: Cache_GetListBylistKey
      x-api-path-slug: apicachelistlistkey-get
      parameters:
      - in: path
        name: listKey
        description: The list key
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Retrieves
      - List
      - Of
      - Objects
      - Stored
      - In
      - Cache
      - System
      - By
      - Its
      - ListKey
  /api/cache/List/{listKey}/Append:
    put:
      summary: Adds {itemToAppend} to the tail of an existing list, or creates a new
        list with the object in it.
      description: Adds {itemtoappend} to the tail of an existing list, or creates
        a new list with the object in it..
      operationId: Cache_AppendToListByitemToAppendBylistKeyBytimeToLive
      x-api-path-slug: apicachelistlistkeyappend-put
      parameters:
      - in: body
        name: itemToAppend
        description: The item to append
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: listKey
        description: The list key
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: timeToLive
        description: The time to live
      responses:
        200:
          description: OK
      tags:
      - S
      - ItemToAppend
      - To
      - Tail
      - Of
      - Existing
      - List
      - ""
      - Creates
      - New
      - List
      - Object
      - In
      - It
  /api/cache/List/{listKey}/Prepend:
    put:
      summary: Adds {itemToPrepend} to the head of an existing list, or creates a
        new list with the object in it.
      description: Adds {itemtoprepend} to the head of an existing list, or creates
        a new list with the object in it..
      operationId: Cache_PrependToListByitemToPrependBylistKeyBytimeToLive
      x-api-path-slug: apicachelistlistkeyprepend-put
      parameters:
      - in: body
        name: itemToPrepend
        description: The item to prepend
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: listKey
        description: The list key
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: timeToLive
        description: The time to live
      responses:
        200:
          description: OK
      tags:
      - S
      - ItemToPrepend
      - To
      - Head
      - Of
      - Existing
      - List
      - ""
      - Creates
      - New
      - List
      - Object
      - In
      - It
  /api/cache/List/{listKey}/Item:
    delete:
      summary: Removes a given item from the list.
      description: Removes a given item from the list..
      operationId: Cache_RemoveItemFromListByitemToRemoveBylistKey
      x-api-path-slug: apicachelistlistkeyitem-delete
      parameters:
      - in: body
        name: itemToRemove
        description: The item to remove
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: listKey
        description: The list key
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Removes
      - Given
      - Item
      - From
      - List
  /api/cache/List/{listKey}/Pop:
    get:
      summary: Pops an items from the list head.
      description: Pops an items from the list head..
      operationId: Cache_PopFromListHeadBylistKey
      x-api-path-slug: apicachelistlistkeypop-get
      parameters:
      - in: path
        name: listKey
        description: The list key
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Pops
      - Items
      - From
      - List
      - Head
  /api/chat/unreadsummary:
    get:
      summary: Get a count of unread chat messages for the negotiator plus a list
        of corresponding message id's which are unread.
      description: Get a count of unread chat messages for the negotiator plus a list
        of corresponding message id's which are unread..
      operationId: Chat_UnreadSummary
      x-api-path-slug: apichatunreadsummary-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Count
      - Of
      - Unread
      - Chat
      - Messagesthe
      - Negotiator
      - Plus
      - List
      - Of
      - Corresponding
      - Message
      - Ids
      - Which
      - Are
      - Unread
  /api/customfieldgroup/{typeName}:
    get:
      summary: Get a list of custom field groups for a type and optional group name
        specified.
      description: Get a list of custom field groups for a type and optional group
        name specified..
      operationId: CustomFieldGroup_GetBytypeNameBygroupName
      x-api-path-slug: apicustomfieldgrouptypename-get
      parameters:
      - in: query
        name: groupName
        description: An optional parameter to filter by group name
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: path
        name: typeName
        description: The name of the type to get the custom field groups for
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Custom
      - Field
      - Groupsa
      - Type
      - Optional
      - Group
      - Name
      - Specified
  /api/customtextdescription/distinctcustompropertydescriptions:
    get:
      summary: Returns a list of the distinct defined custom descriptions for a property
      description: Returns a list of the distinct defined custom descriptions for
        a property.
      operationId: CustomTextDescription_DistinctCustomPropertyDescriptions
      x-api-path-slug: apicustomtextdescriptiondistinctcustompropertydescriptions-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - Distinct
      - Defined
      - Custom
      - Descriptionsa
      - Property
  /api/todo/getall:
    get:
      summary: "Get the list of all ToDo's if no parameter is sent;\r\n<param name=\"filterToDo\">if
        provided will filter by ToDo type</param><param name=\"pageSize\"></param><param
        name=\"pageNumber\"></param>"
      description: "Get the list of all todo's if no parameter is sent;\r\n<param
        name=\"filtertodo\">if provided will filter by todo type</param><param name=\"pagesize\"></param><param
        name=\"pagenumber\"></param>."
      operationId: DefaultToDo_GetAllBypageSizeBypageNumberByfilterToDo.filterCategoryByfilterToDo.toDoTypeByfilterToDo
      x-api-path-slug: apitodogetall-get
      parameters:
      - in: query
        name: filterToDo.branchId
      - in: query
        name: filterToDo.filterCategory
      - in: query
        name: filterToDo.negotiatorIds
      - in: query
        name: filterToDo.toDoType
      - in: query
        name: pageNumber
      - in: query
        name: pageSize
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - ""
      - ToDos
      - If
      - "No"
      - Parameter
      - Is
      - "Sent;\r\n<param"
      - Name=filterToDo>if
      - Provided
      - Will
      - Filter
      - By
      - ToDo
      - Type<
      - Param><param
      - Name=pageSize><
      - Param><param
      - Name=pageNumber><
      - Param>
  /api/todo/activetasks:
    get:
      summary: Get the list of active tasks of a Todo
      description: Get the list of active tasks of a todo.
      operationId: DefaultToDo_ActiveTasksBytoDoIdByignoreDueDateBypageSizeBypageNumber
      x-api-path-slug: apitodoactivetasks-get
      parameters:
      - in: query
        name: ignoreDueDate
      - in: query
        name: pageNumber
      - in: query
        name: pageSize
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: toDoId
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Active
      - Tasks
      - Of
      - Todo
  /api/todo/completedtasks:
    get:
      summary: Get the list of completed tasks of a Todo
      description: Get the list of completed tasks of a todo.
      operationId: DefaultToDo_CompletedTasksBytoDoId
      x-api-path-slug: apitodocompletedtasks-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: toDoId
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Completed
      - Tasks
      - Of
      - Todo
  /api/todo/teamtodos:
    get:
      summary: Get the list of completed tasks of a Todo
      description: Get the list of completed tasks of a todo.
      operationId: DefaultToDo_TeamTodosBybranchId
      x-api-path-slug: apitodoteamtodos-get
      parameters:
      - in: query
        name: branchId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Completed
      - Tasks
      - Of
      - Todo
  /api/todo/canceltodo:
    put:
      summary: Cancel a to-do list from the tile overview of to-dos
      description: Cancel a to-do list from the tile overview of to-dos.
      operationId: DefaultToDo_CancelTodoBycancelTodoCommandData
      x-api-path-slug: apitodocanceltodo-put
      parameters:
      - in: body
        name: cancelTodoCommandData
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Cancel
      - To-do
      - List
      - From
      - Tile
      - Overview
      - Of
      - To-dos
  /api/todo/reassigntodotasks:
    put:
      summary: Reassign a list of tasks to different negotiator(s)
      description: Reassign a list of tasks to different negotiator(s).
      operationId: DefaultToDo_ReassignTodoTasksByreassignTasksCommandData
      x-api-path-slug: apitodoreassigntodotasks-put
      parameters:
      - in: body
        name: reassignTasksCommandData
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Reassign
      - List
      - Of
      - Tasks
      - To
      - Different
      - Negotiator(s)
  /api/todo/getleads:
    get:
      summary: Get the list of all InboundLead ToDo's
      description: Get the list of all inboundlead todo's.
      operationId: DefaultToDo_GetLeadsBybranchIdByexcludeTasks
      x-api-path-slug: apitodogetleads-get
      parameters:
      - in: query
        name: branchId
      - in: query
        name: excludeTasks
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - ""
      - InboundLead
      - ToDos
  /api/todo/gettodosbyid:
    get:
      summary: Return list of tasks, corresponding to task ids passed in.
      description: Return list of tasks, corresponding to task ids passed in..
      operationId: DefaultToDo_GetTodosByIdByids
      x-api-path-slug: apitodogettodosbyid-get
      parameters:
      - in: query
        name: ids
        description: List of task ids
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Return
      - List
      - Of
      - Tasks
      - ""
      - Corresponding
      - To
      - Task
      - Ids
      - Passed
      - In
  /api/documentgeneration/printablepropertylist:
    post:
      summary: Generates a printable property list, it is targetless so there is no
        reference to applicants or owners
      description: Generates a printable property list, it is targetless so there
        is no reference to applicants or owners.
      operationId: DocumentGeneration_PrintablePropertyListBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationprintablepropertylist-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Printable
      - Property
      - List
      - ""
      - It
      - Is
      - Targetless
      - So
      - There
      - Is
      - "No"
      - Reference
      - To
      - Applicants
      - Owners
  /api/documentgeneration/bulkgrouplistcommunication:
    post:
      summary: Generates a bulk communication pack out to multiple clients in a list.
      description: Generates a bulk communication pack out to multiple clients in
        a list..
      operationId: DocumentGeneration_BulkGroupListCommunicationBygeneratePackDetails
      x-api-path-slug: apidocumentgenerationbulkgrouplistcommunication-post
      parameters:
      - in: body
        name: generatePackDetails
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Bulk
      - Communication
      - Pack
      - Out
      - To
      - Multiple
      - Clients
      - In
      - List
  /api/documentgeneration/lettertemplate/{letterTemplateId}:
    get:
      summary: Returns a list of lettertemplates associated to this agency
      description: Returns a list of lettertemplates associated to this agency.
      operationId: DocumentGeneration_GetLetterTemplateByletterTemplateId
      x-api-path-slug: apidocumentgenerationlettertemplatelettertemplateid-get
      parameters:
      - in: path
        name: letterTemplateId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - Lettertemplates
      - Associated
      - To
      - This
      - Agency
  /api/documentgeneration/mergetemplates:
    get:
      summary: Returns a list of lettertemplates associated to this agency
      description: Returns a list of lettertemplates associated to this agency.
      operationId: DocumentGeneration_GetPrintableMergeTemplates
      x-api-path-slug: apidocumentgenerationmergetemplates-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - Lettertemplates
      - Associated
      - To
      - This
      - Agency
  /api/documentgeneration/unusedmergetemplates:
    get:
      summary: Returns a list of lettertemplates associated to this agency that are
        not currently used in any envelope templates
      description: Returns a list of lettertemplates associated to this agency that
        are not currently used in any envelope templates.
      operationId: DocumentGeneration_GetUnusedMergeTemplates
      x-api-path-slug: apidocumentgenerationunusedmergetemplates-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - Lettertemplates
      - Associated
      - To
      - This
      - Agency
      - That
      - Are
      - Not
      - Currently
      - Used
      - In
      - Any
      - Envelope
      - Templates
  /api/documentgeneration/templatesusinganalytics/{analyticsId}:
    get:
      summary: Returns a list of lettertemplates associated to this agency and to
        a particular google analyitics campaign
      description: Returns a list of lettertemplates associated to this agency and
        to a particular google analyitics campaign.
      operationId: DocumentGeneration_GetTemplatesUsingAnalyticsByanalyticsId
      x-api-path-slug: apidocumentgenerationtemplatesusinganalyticsanalyticsid-get
      parameters:
      - in: path
        name: analyticsId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - Lettertemplates
      - Associated
      - To
      - This
      - Agency
      - To
      - Particular
      - Google
      - Analyitics
      - Campaign
  /api/documentgeneration/insertabletemplates:
    get:
      summary: Returns a list of insertable templates associated to this agency
      description: Returns a list of insertable templates associated to this agency.
      operationId: DocumentGeneration_GetPrintableInsertableTemplates
      x-api-path-slug: apidocumentgenerationinsertabletemplates-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - Insertable
      - Templates
      - Associated
      - To
      - This
      - Agency
  /api/documentgeneration/headertemplates:
    get:
      summary: Returns a list of header templates associated to this agency with their
        associated brand info
      description: Returns a list of header templates associated to this agency with
        their associated brand info.
      operationId: DocumentGeneration_GetPrintableHeaderTemplates
      x-api-path-slug: apidocumentgenerationheadertemplates-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - Header
      - Templates
      - Associated
      - To
      - This
      - Agency
      - Their
      - Associated
      - Brand
      - Info
  /api/documentgeneration/envelopetemplates:
    get:
      summary: Returns a list of envelope templates associated to this agency
      description: Returns a list of envelope templates associated to this agency.
      operationId: DocumentGeneration_GetEnvelopeTemplates
      x-api-path-slug: apidocumentgenerationenvelopetemplates-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - Envelope
      - Templates
      - Associated
      - To
      - This
      - Agency
  /api/documentgeneration/envelopetemplatepacks:
    get:
      summary: Returns a list of envelope template packs associated to this agency
      description: Returns a list of envelope template packs associated to this agency.
      operationId: DocumentGeneration_GetEnvelopeTemplatePacks
      x-api-path-slug: apidocumentgenerationenvelopetemplatepacks-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - Envelope
      - Template
      - Packs
      - Associated
      - To
      - This
      - Agency
  /api/documentgeneration/envelopetemplatepacktypes:
    get:
      summary: Returns a list of envelope template packs associated to this agency
      description: Returns a list of envelope template packs associated to this agency.
      operationId: DocumentGeneration_GetEnvelopeTemplatePackTypesByinUseOnly
      x-api-path-slug: apidocumentgenerationenvelopetemplatepacktypes-get
      parameters:
      - in: query
        name: inUseOnly
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - Envelope
      - Template
      - Packs
      - Associated
      - To
      - This
      - Agency
  /api/documentgeneration/envelopetemplatepacks/{systemName}:
    get:
      summary: Gets a list of the packs for a particular packtype
      description: Gets a list of the packs for a particular packtype.
      operationId: DocumentGeneration_GetEnvelopeTemplatePackForTypeBysystemName
      x-api-path-slug: apidocumentgenerationenvelopetemplatepackssystemname-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: path
        name: systemName
      responses:
        200:
          description: OK
      tags:
      - S
      - List
      - Of
      - Packsa
      - Particular
      - Packtype
  /api/documentgeneration/envelopetemplatepacksummarys/{systemName}:
    get:
      summary: Gets a list of the packs for a particular packtype
      description: Gets a list of the packs for a particular packtype.
      operationId: DocumentGeneration_GetEnvelopeTemplatePackSummarysForTypeBysystemName
      x-api-path-slug: apidocumentgenerationenvelopetemplatepacksummaryssystemname-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: path
        name: systemName
      responses:
        200:
          description: OK
      tags:
      - S
      - List
      - Of
      - Packsa
      - Particular
      - Packtype
  /api/documentgeneration/envelopetemplatepacksummary/{envelopeTemplatePackId}:
    get:
      summary: Gets a list of the packs for a particular packtype
      description: Gets a list of the packs for a particular packtype.
      operationId: DocumentGeneration_GetEnvelopeTemplatePackSummaryByenvelopeTemplatePackId
      x-api-path-slug: apidocumentgenerationenvelopetemplatepacksummaryenvelopetemplatepackid-get
      parameters:
      - in: path
        name: envelopeTemplatePackId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - S
      - List
      - Of
      - Packsa
      - Particular
      - Packtype
  /api/documentgeneration/emailtemplates:
    get:
      summary: Returns a list of email templates associated to this agency
      description: Returns a list of email templates associated to this agency.
      operationId: DocumentGeneration_GetEmailTemplates
      x-api-path-slug: apidocumentgenerationemailtemplates-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - Email
      - Templates
      - Associated
      - To
      - This
      - Agency
  /api/documentgeneration/templates/{templateType}:
    get:
      summary: Returns a list of mergable templates for any type associated to this
        agency
      description: Returns a list of mergable templates for any type associated to
        this agency.
      operationId: DocumentGeneration_GetTemplatesBytemplateType
      x-api-path-slug: apidocumentgenerationtemplatestemplatetype-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: path
        name: templateType
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - Mergable
      - Templatesany
      - Type
      - Associated
      - To
      - This
      - Agency
  /api/documentgeneration/smstemplates:
    get:
      summary: Returns a list of sms templates associated to this agency
      description: Returns a list of sms templates associated to this agency.
      operationId: DocumentGeneration_GetSmsTemplates
      x-api-path-slug: apidocumentgenerationsmstemplates-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - Sms
      - Templates
      - Associated
      - To
      - This
      - Agency
  /api/documentgeneration/packrequiredtypes/{packid}:
    get:
      summary: Get a list of the packs required types (ie all of the types required
        by each document in each envelope)
      description: Get a list of the packs required types (ie all of the types required
        by each document in each envelope).
      operationId: DocumentGeneration_PackRequiredTypesBypackid
      x-api-path-slug: apidocumentgenerationpackrequiredtypespackid-get
      parameters:
      - in: path
        name: packid
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Packs
      - Required
      - Types
      - (ie
      - ""
      - Of
      - Types
      - Required
      - By
      - Each
      - Document
      - In
      - Each
      - Envelope)
  /api/documentgeneration/packsupportedsendmethods/{packid}:
    get:
      summary: Get a list of the supported sending methods for a correspondence (ie
        all of the types required by each document in each envelope)
      description: Get a list of the supported sending methods for a correspondence
        (ie all of the types required by each document in each envelope).
      operationId: DocumentGeneration_PackSupportedSendMethodsBypackid
      x-api-path-slug: apidocumentgenerationpacksupportedsendmethodspackid-get
      parameters:
      - in: path
        name: packid
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Supported
      - Sending
      - Methodsa
      - Correspondence
      - (ie
      - ""
      - Of
      - Types
      - Required
      - By
      - Each
      - Document
      - In
      - Each
      - Envelope)
  /api/enum:
    get:
      summary: "Returns a list of possible values for an enum if you just specify
        {typeName}.\r\nReturns a an enum if you specify {typeName} and {systemName}."
      description: "Returns a list of possible values for an enum if you just specify
        {typename}.\r\nreturns a an enum if you specify {typename} and {systemname}.."
      operationId: Enum_GetBytypeNameBysystemNameByeventCategoryType
      x-api-path-slug: apienum-get
      parameters:
      - in: query
        name: eventCategoryType
        description: Where the enum has values which are categorised, this filters
          on that category
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: systemName
        description: The system name of the enum to get
      - in: query
        name: typeName
        description: The type of enum to get
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - Possible
      - Valuesan
      - Enum
      - If
      - You
      - Just
      - Specify
      - TypeName
      - Returns
      - Enum
      - If
      - You
      - Specify
      - TypeName
      - SystemName
  /api/feature/list:
    get:
      summary: Get  a list of features by a list of ids
      description: Get  a list of features by a list of ids.
      operationId: Feature_GetByfeatureid
      x-api-path-slug: apifeaturelist-get
      parameters:
      - in: query
        name: featureid
        description: the list of ids
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Features
      - By
      - List
      - Of
      - Ids
  /api/fee/getall:
    get:
      summary: Get list of all fees stored
      description: Get list of all fees stored.
      operationId: Fee_GetFeesBypageSizeBypageNumber
      x-api-path-slug: apifeegetall-get
      parameters:
      - in: query
        name: pageNumber
      - in: query
        name: pageSize
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - ""
      - Fees
      - Stored
  /api/group/{id}/getpropertyroleidsalreadysent:
    get:
      summary: returns a list of the property role ids that should be excluded from
        mailouts to this role id because the have been sent before
      description: Returns a list of the property role ids that should be excluded
        from mailouts to this role id because the have been sent before.
      operationId: Group_GetPropertyMarketingRoleIdsSentByidBywithinDaysByresendPriceChangedProperties
      x-api-path-slug: apigroupidgetpropertyroleidsalreadysent-get
      parameters:
      - in: path
        name: id
        description: The id of the group
      - in: query
        name: resendPriceChangedProperties
        description: include the properties that have had to a price change or withdrawn
          event since it was last sent to them
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: withinDays
        description: number of days since the last time it was sent, send 0 for all
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - Property
      - Role
      - Ids
      - That
      - Should
      - Be
      - Excluded
      - From
      - Mailouts
      - To
      - This
      - Role
      - Id
      - Because
      - Have
      - Been
      - Sent
      - Before
  /api/group/{id}/documents:
    get:
      summary: Get a list of documents belonging to a group
      description: Get a list of documents belonging to a group.
      operationId: Group_DocumentsByidBysubTypesBypageSizeBypageNumberBytypeByorderDesc
      x-api-path-slug: apigroupiddocuments-get
      parameters:
      - in: path
        name: id
        description: The id of the group to get the documents for
      - in: query
        name: orderDesc
        description: Order by created date descending (true by default)
      - in: query
        name: pageNumber
      - in: query
        name: pageSize
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: subTypes
      - in: query
        name: type
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Documents
      - Belonging
      - To
      - Group
  /api/group/{id}/offers/made:
    get:
      summary: Get a list of documents belonging to a group
      description: Get a list of documents belonging to a group.
      operationId: Group_OffersMadeByidBypageSizeBypageNumber
      x-api-path-slug: apigroupidoffersmade-get
      parameters:
      - in: path
        name: id
        description: The id of the group to get the documents for
      - in: query
        name: pageNumber
      - in: query
        name: pageSize
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Documents
      - Belonging
      - To
      - Group
  /api/group/{id}/offers/received:
    get:
      summary: Get a list of documents belonging to a group
      description: Get a list of documents belonging to a group.
      operationId: Group_OffersReceivedByidBypageSizeBypageNumber
      x-api-path-slug: apigroupidoffersreceived-get
      parameters:
      - in: path
        name: id
        description: The id of the group to get the documents for
      - in: query
        name: pageNumber
      - in: query
        name: pageSize
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Documents
      - Belonging
      - To
      - Group
  /api/group/{id}/properties:
    get:
      summary: Return a list of properties that the group owns
      description: Return a list of properties that the group owns.
      operationId: Group_GroupPropertiesByidBypageSizeBypageNumber
      x-api-path-slug: apigroupidproperties-get
      parameters:
      - in: path
        name: id
      - in: query
        name: pageNumber
      - in: query
        name: pageSize
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Return
      - List
      - Of
      - Properties
      - That
      - Group
      - Owns
  /api/invoice/find:
    post:
      summary: Get filtered list of invoices
      description: Get filtered list of invoices.
      operationId: Invoice_GetInvoicesByfilterBypageSizeBypageNumber
      x-api-path-slug: apiinvoicefind-post
      parameters:
      - in: body
        name: filter
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: pageNumber
      - in: query
        name: pageSize
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Filtered
      - List
      - Of
      - Invoices
  /api/invoice/totals:
    post:
      summary: Get filtered list of invoices
      description: Get filtered list of invoices.
      operationId: Invoice_InvoiceTotalsByfilter
      x-api-path-slug: apiinvoicetotals-post
      parameters:
      - in: body
        name: filter
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Filtered
      - List
      - Of
      - Invoices
  /api/invoice/saveforlater:
    get:
      summary: Return list of receipts progress amounts
      description: Return list of receipts progress amounts.
      operationId: Invoice_SaveForLater
      x-api-path-slug: apiinvoicesaveforlater-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Return
      - List
      - Of
      - Receipts
      - Progress
      - Amounts
  /api/invoice/savereceiptlistitem:
    post:
      summary: Save receipt list item
      description: Save receipt list item.
      operationId: Invoice_SaveReceiptListItemBydataContract
      x-api-path-slug: apiinvoicesavereceiptlistitem-post
      parameters:
      - in: body
        name: dataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Save
      - Receipt
      - List
      - Item
  /api/invoice/getreceiptitems:
    get:
      summary: Return list of receipts to process
      description: Return list of receipts to process.
      operationId: Invoice_GetSavedReceiptItemsForAgency
      x-api-path-slug: apiinvoicegetreceiptitems-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Return
      - List
      - Of
      - Receipts
      - To
      - Process
  /api/invoice/removereceiptallocation:
    delete:
      summary: Remove a receipt list item allocation
      description: Remove a receipt list item allocation.
      operationId: Invoice_RemoveSavedReceiptItemAllocationByreceiptItemIdByinvoiceIdByallocationId
      x-api-path-slug: apiinvoiceremovereceiptallocation-delete
      parameters:
      - in: query
        name: allocationId
      - in: query
        name: invoiceId
      - in: query
        name: receiptItemId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Receipt
      - List
      - Item
      - Ocation
  /api/invoice/processreceiptlistitems:
    put:
      summary: Process receipt list items for a specifici negotiator.
      description: Process receipt list items for a specifici negotiator..
      operationId: Invoice_ProcessReceiptListItemsBynegotiatorId
      x-api-path-slug: apiinvoiceprocessreceiptlistitems-put
      parameters:
      - in: query
        name: negotiatorId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Process
      - Receipt
      - List
      - Itemsa
      - Specifici
      - Negotiator
  /api/list/events/filters/{id}:
    delete:
      summary: Marks Event List Filter as deleted
      description: Marks event list filter as deleted.
      operationId: List_DeleteEventFilterByid
      x-api-path-slug: apilisteventsfiltersid-delete
      parameters:
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Marks
      - Event
      - List
      - Filter
      - As
      - Deleted
  /api/list/property/filters/{id}:
    delete:
      summary: Marks Property List Filter as deleted
      description: Marks property list filter as deleted.
      operationId: List_DeletePropertyFilterByid
      x-api-path-slug: apilistpropertyfiltersid-delete
      parameters:
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Marks
      - Property
      - List
      - Filter
      - As
      - Deleted
  /api/list/groups/filters/{id}:
    delete:
      summary: Marks Groups List Filter as deleted
      description: Marks groups list filter as deleted.
      operationId: List_DeleteGroupFilterByid
      x-api-path-slug: apilistgroupsfiltersid-delete
      parameters:
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Marks
      - Groups
      - List
      - Filter
      - As
      - Deleted
  /api/list/groups/groupidsfiltered:
    post:
      summary: Get list of group ids
      description: Get list of group ids.
      operationId: List_GetGroupListFilteredByfilter
      x-api-path-slug: apilistgroupsgroupidsfiltered-post
      parameters:
      - in: body
        name: filter
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Group
      - Ids
  /api/list/groupinterests:
    post:
      summary: Get list of groups and what they are interested in.
      description: Get list of groups and what they are interested in..
      operationId: List_GroupInterestsByfilterBypageSizeBypageNumber
      x-api-path-slug: apilistgroupinterests-post
      parameters:
      - in: body
        name: filter
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: pageNumber
      - in: query
        name: pageSize
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Groups
      - What
      - They
      - Are
      - Interested
      - In
  /api/list/groupinterests/groupinterestidsfiltered:
    post:
      summary: Get list of groups and what they are interested in.
      description: Get list of groups and what they are interested in..
      operationId: List_GetInterestsFilteredByfilter
      x-api-path-slug: apilistgroupinterestsgroupinterestidsfiltered-post
      parameters:
      - in: body
        name: filter
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Groups
      - What
      - They
      - Are
      - Interested
      - In
  /api/list/groupinterests/filters/{id}:
    delete:
      summary: Marks Groups List Filter as deleted
      description: Marks groups list filter as deleted.
      operationId: List_DeleteGroupInterestListFilterByid
      x-api-path-slug: apilistgroupinterestsfiltersid-delete
      parameters:
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Marks
      - Groups
      - List
      - Filter
      - As
      - Deleted
  /api/list/property/propertyidsfiltered:
    post:
      summary: Get list of RoleIds for property marketing roles
      description: Get list of roleids for property marketing roles.
      operationId: List_GetPropertyListFilteredByfilter
      x-api-path-slug: apilistpropertypropertyidsfiltered-post
      parameters:
      - in: body
        name: filter
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - RoleIdsproperty
      - Marketing
      - Roles
  /api/list/property/csv:
    post:
      summary: Generates a csv file from selected property list items
      description: Generates a csv file from selected property list items.
      operationId: List_GeneratePropertyCsvBycommandDataContract
      x-api-path-slug: apilistpropertycsv-post
      parameters:
      - in: body
        name: commandDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Csv
      - File
      - From
      - Selected
      - Property
      - List
      - Items
  /api/list/lettingproperty/csv:
    post:
      summary: Generates a csv file from selected letting property list items
      description: Generates a csv file from selected letting property list items.
      operationId: List_GenerateLettingPropertyCsvBycommandDataContract
      x-api-path-slug: apilistlettingpropertycsv-post
      parameters:
      - in: body
        name: commandDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Csv
      - File
      - From
      - Selected
      - Letting
      - Property
      - List
      - Items
  /api/list/propertypipeline/csv:
    post:
      summary: Generates a csv file from selected property list items
      description: Generates a csv file from selected property list items.
      operationId: List_GeneratePipelinePropertyCsvBycommandDataContract
      x-api-path-slug: apilistpropertypipelinecsv-post
      parameters:
      - in: body
        name: commandDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Csv
      - File
      - From
      - Selected
      - Property
      - List
      - Items
  /api/list/events/csv:
    post:
      summary: Generates a csv file from selected event list items
      description: Generates a csv file from selected event list items.
      operationId: List_GenerateEventCsvBycommandDataContract
      x-api-path-slug: apilisteventscsv-post
      parameters:
      - in: body
        name: commandDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Csv
      - File
      - From
      - Selected
      - Event
      - List
      - Items
  /api/list/groups/csv:
    post:
      summary: Generates a csv file from selected group list items
      description: Generates a csv file from selected group list items.
      operationId: List_GenerateGroupCsvBycommandDataContract
      x-api-path-slug: apilistgroupscsv-post
      parameters:
      - in: body
        name: commandDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Csv
      - File
      - From
      - Selected
      - Group
      - List
      - Items
  /api/list/groupinterests/csv:
    post:
      summary: Generates a csv file from selected group interest list items
      description: Generates a csv file from selected group interest list items.
      operationId: List_GenerateGroupInterestCsvBycommandDataContract
      x-api-path-slug: apilistgroupinterestscsv-post
      parameters:
      - in: body
        name: commandDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Csv
      - File
      - From
      - Selected
      - Group
      - Interest
      - List
      - Items
  /api/list/activesearches/csv:
    post:
      summary: Generates a csv file from selected group list items
      description: Generates a csv file from selected group list items.
      operationId: List_GenerateActiveSearchCsvBycommandDataContract
      x-api-path-slug: apilistactivesearchescsv-post
      parameters:
      - in: body
        name: commandDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Csv
      - File
      - From
      - Selected
      - Group
      - List
      - Items
  /api/list/propertyfinancial/csv:
    post:
      summary: Generates a csv file from selected group list items
      description: Generates a csv file from selected group list items.
      operationId: List_GenerateFinancialPropertyCsvBycommandDataContract
      x-api-path-slug: apilistpropertyfinancialcsv-post
      parameters:
      - in: body
        name: commandDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Csv
      - File
      - From
      - Selected
      - Group
      - List
      - Items
  /api/list/propertynewbusiness/csv:
    post:
      summary: Generates a csv file from selected property list items
      description: Generates a csv file from selected property list items.
      operationId: List_GenerateNewBusinessPropertyCsvBycommandDataContract
      x-api-path-slug: apilistpropertynewbusinesscsv-post
      parameters:
      - in: body
        name: commandDataContract
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Generates
      - Csv
      - File
      - From
      - Selected
      - Property
      - List
      - Items
  /api/list/todos:
    post:
      summary: Get list of todos
      description: Get list of todos.
      operationId: List_TodosByfilterBypageSizeBypageNumber
      x-api-path-slug: apilisttodos-post
      parameters:
      - in: body
        name: filter
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: pageNumber
      - in: query
        name: pageSize
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Todos
  /api/list/todos/filters/{id}:
    delete:
      summary: Marks Todo List Filter as deleted
      description: Marks todo list filter as deleted.
      operationId: List_DeleteTodoListFilterByid
      x-api-path-slug: apilisttodosfiltersid-delete
      parameters:
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Marks
      - Todo
      - List
      - Filter
      - As
      - Deleted
  /api/list/todotasks:
    post:
      summary: Get list of todos tasks.
      description: Get list of todos tasks..
      operationId: List_TodoTasksByfilterBypageSizeBypageNumber
      x-api-path-slug: apilisttodotasks-post
      parameters:
      - in: body
        name: filter
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: pageNumber
      - in: query
        name: pageSize
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Todos
      - Tasks
  /api/list/todotasks/filters/{id}:
    delete:
      summary: Marks Todos task List Filter as deleted
      description: Marks todos task list filter as deleted.
      operationId: List_DeleteTodoTaskListFilterByid
      x-api-path-slug: apilisttodotasksfiltersid-delete
      parameters:
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Marks
      - Todos
      - Task
      - List
      - Filter
      - As
      - Deleted
  /api/list/followups:
    post:
      summary: Gets a list of group followups
      description: Gets a list of group followups.
      operationId: List_FollowUpsByfilterBypageSizeBypageNumber
      x-api-path-slug: apilistfollowups-post
      parameters:
      - in: body
        name: filter
        description: Filter for follow ups
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: pageNumber
        description: Page number
      - in: query
        name: pageSize
        description: Page size, limited to 100
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - S
      - List
      - Of
      - Group
      - Followups
  /api/list/followups/filters:
    get:
      summary: Get all saved follow up list filters
      description: Get all saved follow up list filters.
      operationId: List_GetFollowUpListFiltersByroleTypeBycontext
      x-api-path-slug: apilistfollowupsfilters-get
      parameters:
      - in: query
        name: context
        description: Filter context
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: roleType
        description: Filter roleType
      responses:
        200:
          description: OK
      tags:
      - Saved
      - Follow
      - Up
      - List
      - Filters
  /api/list/followups/filters/{id}:
    delete:
      summary: Marks Follow Up List Filter as deleted
      description: Marks follow up list filter as deleted.
      operationId: List_DeleteFollowUpListFilterByid
      x-api-path-slug: apilistfollowupsfiltersid-delete
      parameters:
      - in: path
        name: id
        description: Id of filter to delete
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Marks
      - Follow
      - Up
      - List
      - Filter
      - As
      - Deleted
  /api/list/feedback/followups:
    post:
      summary: Gets a list of group followups
      description: Gets a list of group followups.
      operationId: List_FeedbackFollowUpsByfilterBypageSizeBypageNumber
      x-api-path-slug: apilistfeedbackfollowups-post
      parameters:
      - in: body
        name: filter
        description: Filter for follow ups
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: pageNumber
        description: Page number
      - in: query
        name: pageSize
        description: Page size, limited to 100
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - S
      - List
      - Of
      - Group
      - Followups
  /api/list/feedback/followups/filters:
    get:
      summary: Get all saved feedback follow up list filters
      description: Get all saved feedback follow up list filters.
      operationId: List_GetFeedbackFollowUpListFiltersByroleTypeBycontext
      x-api-path-slug: apilistfeedbackfollowupsfilters-get
      parameters:
      - in: query
        name: context
        description: Filter context
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: roleType
        description: Filter roleType
      responses:
        200:
          description: OK
      tags:
      - Saved
      - Feedback
      - Follow
      - Up
      - List
      - Filters
  /api/list/feedbackfollowups/filters/{id}:
    delete:
      summary: Marks Feedback Follow Up List Filter as deleted
      description: Marks feedback follow up list filter as deleted.
      operationId: List_DeleteFeedbackFollowUpListFilterByid
      x-api-path-slug: apilistfeedbackfollowupsfiltersid-delete
      parameters:
      - in: path
        name: id
        description: Id of filter to delete
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Marks
      - Feedback
      - Follow
      - Up
      - List
      - Filter
      - As
      - Deleted
  /api/negotiator/my/properties/{roleType}:
    get:
      summary: Used for the Property Sales Dashboard to return a list of the negotiator's
        properties.
      description: Used for the property sales dashboard to return a list of the negotiator's
        properties..
      operationId: Negotiator_PropertiesByroleTypeBypageSizeBypageNumber
      x-api-path-slug: apinegotiatormypropertiesroletype-get
      parameters:
      - in: query
        name: pageNumber
        description: which page number of results to choose
      - in: query
        name: pageSize
        description: how many properties to return (default 10)
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: path
        name: roleType
        description: the PropertyMarketingRole type
      responses:
        200:
          description: OK
      tags:
      - Usedthe
      - Property
      - Sales
      - Dashboard
      - To
      - Return
      - List
      - Of
      - Negotiators
      - Properties
  /api/negotiator/my/properties/favourite/add/{propertyId}:
    post:
      summary: Add property to Negotiators favourite list
      description: Add property to negotiators favourite list.
      operationId: Negotiator_AddFavouritePropertyBypropertyIdByroleId
      x-api-path-slug: apinegotiatormypropertiesfavouriteaddpropertyid-post
      parameters:
      - in: path
        name: propertyId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: roleId
      responses:
        200:
          description: OK
      tags:
      - Property
      - To
      - Negotiators
      - Favourite
      - List
  /api/negotiator/my/properties/favourite/remove/{propertyId}:
    delete:
      summary: Remove a property from a Negotiators favourite list.
      description: Remove a property from a negotiators favourite list..
      operationId: Negotiator_RemoveFavouritePropertyBypropertyIdByroleId
      x-api-path-slug: apinegotiatormypropertiesfavouriteremovepropertyid-delete
      parameters:
      - in: path
        name: propertyId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: roleId
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Property
      - From
      - Negotiators
      - Favourite
      - List
  /api/negotiator/my/groups/favourite:
    get:
      summary: Returns a list of the logged in negotiators favourite groups.
      description: Returns a list of the logged in negotiators favourite groups..
      operationId: Negotiator_FavouriteGroupsBypageSizeBypageNumber
      x-api-path-slug: apinegotiatormygroupsfavourite-get
      parameters:
      - in: query
        name: pageNumber
      - in: query
        name: pageSize
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - Logged
      - In
      - Negotiators
      - Favourite
      - Groups
  /api/negotiator/my/groups/favourite/add/{groupId}:
    post:
      summary: Add a favourite group to the negotiators list of favourites.
      description: Add a favourite group to the negotiators list of favourites..
      operationId: Negotiator_AddFavouriteGroupBygroupId
      x-api-path-slug: apinegotiatormygroupsfavouriteaddgroupid-post
      parameters:
      - in: path
        name: groupId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Favourite
      - Group
      - To
      - Negotiators
      - List
      - Of
      - Favourites
  /api/negotiator/my/groups/favourite/remove/{groupId}:
    delete:
      summary: Remove a group from a Negotiators favourite list.
      description: Remove a group from a negotiators favourite list..
      operationId: Negotiator_RemoveFavouriteGroupBygroupId
      x-api-path-slug: apinegotiatormygroupsfavouriteremovegroupid-delete
      parameters:
      - in: path
        name: groupId
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Group
      - From
      - Negotiators
      - Favourite
      - List
  /api/negotiator/my/responsibilities:
    get:
      summary: Gets a list of the logged in users responsibilities
      description: Gets a list of the logged in users responsibilities.
      operationId: Negotiator_GetResponsibilities
      x-api-path-slug: apinegotiatormyresponsibilities-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - S
      - List
      - Of
      - Logged
      - In
      - Users
      - Responsibilities
  /api/people/findbyemail:
    get:
      summary: Returns a list of people that have the supplied email address.
      description: Returns a list of people that have the supplied email address..
      operationId: People_GetPeopleWithEmailAddressByemailAddress
      x-api-path-slug: apipeoplefindbyemail-get
      parameters:
      - in: query
        name: emailAddress
        description: The email address
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Returns
      - List
      - Of
      - People
      - That
      - Have
      - Supplied
      - Email
      - Address
  /api/property/{id}/keys:
    get:
      summary: Get a list of keys for a property
      description: Get a list of keys for a property.
      operationId: Property_KeysByid
      x-api-path-slug: apipropertyidkeys-get
      parameters:
      - in: path
        name: id
        description: The Id of the property
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Keysa
      - Property
  /api/property/{id}/alarms:
    get:
      summary: Get a list of alarms for a property
      description: Get a list of alarms for a property.
      operationId: Property_AlarmsByid
      x-api-path-slug: apipropertyidalarms-get
      parameters:
      - in: path
        name: id
        description: The Id of the property
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Alarmsa
      - Property
  /api/property/{id}/specialarrangements:
    get:
      summary: Get a list of special arrangements for a property
      description: Get a list of special arrangements for a property.
      operationId: Property_SpecialArrangementsByid
      x-api-path-slug: apipropertyidspecialarrangements-get
      parameters:
      - in: path
        name: id
        description: The Id of the property
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Special
      - Arrangementsa
      - Property
  /api/property/{id}/certificate:
    get:
      summary: Get a list of certificates for a property
      description: Get a list of certificates for a property.
      operationId: Property_CertificateByid
      x-api-path-slug: apipropertyidcertificate-get
      parameters:
      - in: path
        name: id
        description: The Id of the property
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Certificatesa
      - Property
  /api/property/{id}/tenantroles:
    get:
      summary: Get a list of all current and ended tenant roles from a property id.
      description: Get a list of all current and ended tenant roles from a property
        id..
      operationId: Property_TenantRolesByPropertyIdByid
      x-api-path-slug: apipropertyidtenantroles-get
      parameters:
      - in: path
        name: id
        description: The Id of the property
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - ""
      - Current
      - Ended
      - Tenant
      - Roles
      - From
      - Property
      - Id
  /api/region/favourites/add:
    post:
      summary: Add a region to your list of favourites
      description: Add a region to your list of favourites.
      operationId: Region_AddFavouriteBycommand
      x-api-path-slug: apiregionfavouritesadd-post
      parameters:
      - in: body
        name: command
        schema:
          $ref: '#/definitions/holder'
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Region
      - To
      - Your
      - List
      - Of
      - Favourites
  /api/role/{id}/matches:
    get:
      summary: Get a list of groups that may be interested in this property role
      description: Get a list of groups that may be interested in this property role.
      operationId: Role_MatchesByidBypageSizeBypageNumberByadjustedAskingPriceBysortByminScore
      x-api-path-slug: apiroleidmatches-get
      parameters:
      - in: query
        name: adjustedAskingPrice
        description: Override the asking price to show a different set of potential
          matches
      - in: path
        name: id
        description: The id of the role to get the group matches for
      - in: query
        name: minScore
      - in: query
        name: pageNumber
        description: Page number
      - in: query
        name: pageSize
        description: Number of results per page
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: sort
        description: Sort order of results
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Groups
      - That
      - May
      - Be
      - Interested
      - In
      - This
      - Property
      - Role
    post:
      summary: Get a list of groups that may be interested in this property role
      description: Get a list of groups that may be interested in this property role.
      operationId: Role_MatchesByidByfilterBypageSizeBypageNumberByadjustedAskingPriceBysort
      x-api-path-slug: apiroleidmatches-post
      parameters:
      - in: query
        name: adjustedAskingPrice
        description: Override the asking price to show a different set of potential
          matches
      - in: body
        name: filter
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: The id of the role to get the group matches for
      - in: query
        name: pageNumber
        description: Page number
      - in: query
        name: pageSize
        description: Number of results per page
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: sort
        description: Sort order of results
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Groups
      - That
      - May
      - Be
      - Interested
      - In
      - This
      - Property
      - Role
  /api/role/{id}/matchidsfiltered:
    post:
      summary: Get list of role ids
      description: Get list of role ids.
      operationId: Role_GetMatchListFilteredByidByfilter
      x-api-path-slug: apiroleidmatchidsfiltered-post
      parameters:
      - in: body
        name: filter
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Role
      - Ids
  /api/role/{id}/documents:
    get:
      summary: Get a list of documents belonging to a role
      description: Get a list of documents belonging to a role.
      operationId: Role_DocumentsByidBysubTypesBypageSizeBypageNumberBytypeByorderDesc
      x-api-path-slug: apiroleiddocuments-get
      parameters:
      - in: path
        name: id
        description: The id of the role to get the documents for
      - in: query
        name: orderDesc
      - in: query
        name: pageNumber
      - in: query
        name: pageSize
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: subTypes
      - in: query
        name: type
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Documents
      - Belonging
      - To
      - Role
  /api/role/{id}/images:
    get:
      summary: Get a list of ordered images belonging to a role
      description: Get a list of ordered images belonging to a role.
      operationId: Role_ImagesByidBypageSizeBypageNumberBysubtype
      x-api-path-slug: apiroleidimages-get
      parameters:
      - in: path
        name: id
        description: The id of the role to get the images for
      - in: query
        name: pageNumber
      - in: query
        name: pageSize
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: subtype
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Ordered
      - Images
      - Belonging
      - To
      - Role
  /api/role/{id}/brochures:
    get:
      summary: Get a list of ordered brochures belonging to a role
      description: Get a list of ordered brochures belonging to a role.
      operationId: Role_BrochuresByidBypageSizeBypageNumber
      x-api-path-slug: apiroleidbrochures-get
      parameters:
      - in: path
        name: id
        description: The id of the role to get the images for
      - in: query
        name: pageNumber
      - in: query
        name: pageSize
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Ordered
      - Brochures
      - Belonging
      - To
      - Role
  /api/role/{id}/offersbasic:
    get:
      summary: Get a basic list of offers associated to the current property marketing
        role.
      description: Get a basic list of offers associated to the current property marketing
        role..
      operationId: Role_OffersBasicByid
      x-api-path-slug: apiroleidoffersbasic-get
      parameters:
      - in: path
        name: id
        description: The id of the marketing role to get the offers for
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Basic
      - List
      - Of
      - Offers
      - Associated
      - To
      - Current
      - Property
      - Marketing
      - Role
  /api/role/{roleId}/viewingsbasic:
    get:
      summary: Get a basic list of all viewings for a particular marketing role.
      description: Get a basic list of all viewings for a particular marketing role..
      operationId: Role_BasicViewingsByroleId
      x-api-path-slug: apiroleroleidviewingsbasic-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: path
        name: roleId
        description: The id of the marketing role to get the viewings for
      responses:
        200:
          description: OK
      tags:
      - Basic
      - List
      - Of
      - ""
      - Viewingsa
      - Particular
      - Marketing
      - Role
  /api/roomdescription/{id}/uploadandattachdocumenttoroom:
    put:
      summary: Uploads and attaches a document to room description room - the new
        document is appended to the current list.
      description: Uploads and attaches a document to room description room - the
        new document is appended to the current list..
      operationId: RoomDescription_UploadAndAttachDocumentToRoomByidByroomIdBydocumentDetails
      x-api-path-slug: apiroomdescriptioniduploadandattachdocumenttoroom-put
      parameters:
      - in: body
        name: documentDetails
        description: Details about the document
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: The room description Id
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: roomId
        description: The roomId
      responses:
        200:
          description: OK
      tags:
      - Uploads
      - Attaches
      - Document
      - To
      - Room
      - Description
      - Room
      - '-'
      - New
      - Document
      - Is
      - Appended
      - To
      - Current
      - List
  /api/roomdescription/setimages:
    post:
      summary: Allows you to specify a list of documentIds for a roomDescriptions
        room - this list will overwrite any existing list of documents on that room,
        and order will be honoured.
      description: Allows you to specify a list of documentids for a roomdescriptions
        room - this list will overwrite any existing list of documents on that room,
        and order will be honoured..
      operationId: RoomDescription_SetImagesByroomImageOrder
      x-api-path-slug: apiroomdescriptionsetimages-post
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: body
        name: roomImageOrder
        description: The room image order
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Allows
      - You
      - To
      - Specify
      - List
      - Of
      - DocumentIdsa
      - RoomDescriptions
      - Room
      - '-'
      - This
      - List
      - Will
      - Overwrite
      - Any
      - Existing
      - List
      - Of
      - Documents
      - "On"
      - That
      - Room
      - ""
      - Order
      - Will
      - Be
      - Honoured
  /api/tag/list:
    get:
      summary: Get  a list of tags by a list of ids
      description: Get  a list of tags by a list of ids.
      operationId: Tag_GetBytagid
      x-api-path-slug: apitaglist-get
      parameters:
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      - in: query
        name: tagid
        description: the list of ids
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Tags
      - By
      - List
      - Of
      - Ids
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