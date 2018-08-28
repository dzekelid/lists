---
swagger: "2.0"
x-collection-name: Plentymarkets
x-complete: 0
info:
  title: Plentymarkets List properties
  description: Lists properties.
  contact:
    name: plentymarkets
    url: https://forum.plentymarkets.com/c/rest-api
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
  /rest/accounting/locations/{locationId}/debtor_accounts/{mode}:
    get:
      summary: Lists the debtor accounts by mode.
      description: Lists the debtor accounts of an accounting location by mode. The
        ID of the accounting location and the mode have to be specified.
      operationId: getRestAccountingLocationsLocationDebtorAccountsMode
      x-api-path-slug: restaccountinglocationslocationiddebtor-accountsmode-get
      parameters:
      - in: path
        name: locationId
      - in: path
        name: mode
      responses:
        200:
          description: OK
      tags:
      - Lists
      - Debtor
      - Accounts
      - By
      - Mode
  /rest/boards:
    get:
      summary: Lists all boards.
      description: Lists all boards..
      operationId: getRestBoards
      x-api-path-slug: restboards-get
      responses:
        200:
          description: OK
      tags:
      - Lists
      - ""
      - Boards
  /rest/boards/{boardId}/columns:
    get:
      summary: Lists all columns for a given board
      description: Lists all columns for a given board.
      operationId: getRestBoardsBoardColumns
      x-api-path-slug: restboardsboardidcolumns-get
      parameters:
      - in: path
        name: boardId
      responses:
        200:
          description: OK
      tags:
      - Lists
      - ""
      - Columnsa
      - Given
      - Board
  /rest/boards/{boardId}/columns/{columnId}/tasks:
    get:
      summary: Lists all tasks for a given column.
      description: Lists all tasks for a given column..
      operationId: getRestBoardsBoardColumnsColumnTasks
      x-api-path-slug: restboardsboardidcolumnscolumnidtasks-get
      parameters:
      - in: path
        name: boardId
      - in: path
        name: columnId
      - in: query
        name: startAt
        description: Position of a task to start listing at
      - in: query
        name: tasksPerPage
        description: Number of tasks to list per page
      responses:
        200:
          description: OK
      tags:
      - Lists
      - ""
      - Tasksa
      - Given
      - Column
  /rest/items/attributes/maps:
    get:
      summary: Lists all attribute maps.
      description: Lists all attribute maps..
      operationId: getRestItemsAttributesMaps
      x-api-path-slug: restitemsattributesmaps-get
      responses:
        200:
          description: OK
      tags:
      - Lists
      - ""
      - Attribute
      - Maps
  /rest/items/attributes/values/maps:
    get:
      summary: Lists all attribute value maps.
      description: Lists all attribute value maps..
      operationId: getRestItemsAttributesValuesMaps
      x-api-path-slug: restitemsattributesvaluesmaps-get
      responses:
        200:
          description: OK
      tags:
      - Lists
      - ""
      - Attribute
      - Value
      - Maps
  /rest/items/{id}/variations/{variationId}/variation_suppliers:
    get:
      summary: Lists suppliers for a variation
      description: Lists all supplier data linked to a variation. The ID of the variation
        must be specified.
      operationId: getRestItemsVariationsVariationVariationSuppliers
      x-api-path-slug: restitemsidvariationsvariationidvariation-suppliers-get
      parameters:
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - Lists
      - Suppliersa
      - Variation
  /rest/orders/shipping/presets/{presetId}/parcel_service_regions:
    get:
      summary: Lists parcel service regions by parcel service preset id.
      description: Lists parcel service regions. The ID of the parcel service preset
        must be specified.
      operationId: getRestOrdersShippingPresetsPresetParcelServiceRegions
      x-api-path-slug: restordersshippingpresetspresetidparcel-service-regions-get
      parameters:
      - in: query
        name: $parcelServicePresetId
        description: The ID of the parcel service preset
      - in: query
        name: columns
        description: The properties to be loaded
      - in: path
        name: presetId
      responses:
        200:
          description: OK
      tags:
      - Lists
      - Parcel
      - Service
      - Regions
      - By
      - Parcel
      - Service
      - Preset
      - Id
  /rest/accounting/locations/revenue_account_configurations:
    get:
      summary: List revenue account configurations
      description: Lists revenue account configurations of a system. The revenue accounts
        are returned as paginated result. By default 50 revenue accounts are on one
        page.
      operationId: getRestAccountingLocationsRevenueAccountConfigurations
      x-api-path-slug: restaccountinglocationsrevenue-account-configurations-get
      parameters:
      - in: query
        name: itemsPerPage
        description: The number of revenue accounts to be displayed per page
      - in: query
        name: page
        description: The page to get
      responses:
        200:
          description: OK
      tags:
      - List
      - Revenue
      - Account
      - Configurations
  /rest/accounting/stores/locations:
    get:
      summary: List all accounting locations
      description: List all accounting locations.
      operationId: getRestAccountingStoresLocations
      x-api-path-slug: restaccountingstoreslocations-get
      responses:
        200:
          description: OK
      tags:
      - List
      - ""
      - Accounting
      - Locations
  /rest/accounting/stores/{plentyId}/locations:
    get:
      summary: List accounting locations of a client
      description: Lists accounting locations of a client. The plenty ID of the client
        must be specified.
      operationId: getRestAccountingStoresPlentyLocations
      x-api-path-slug: restaccountingstoresplentyidlocations-get
      parameters:
      - in: query
        name: locationId
        description: The plenty ID
      - in: path
        name: plentyId
      responses:
        200:
          description: OK
      tags:
      - List
      - Accounting
      - Locations
      - Of
      - Client
  /rest/accounts:
    get:
      summary: List accounts
      description: List accounts.
      operationId: getRestAccounts
      x-api-path-slug: restaccounts-get
      parameters:
      - in: query
        name: createdAt
        description: Filter that restricts the search result to accounts that were
          created according to given filters
      - in: query
        name: updatedAt
        description: Filter that restricts the search result to accounts that were
          updated according to given filters
      responses:
        200:
          description: OK
      tags:
      - List
      - Accounts
  /rest/accounts/addresses/contact_relations:
    get:
      summary: List address contact relations
      description: List address contact relations.
      operationId: getRestAccountsAddressesContactRelations
      x-api-path-slug: restaccountsaddressescontact-relations-get
      parameters:
      - in: query
        name: addressId
        description: Filter that restricts the search result to addresses with a specific
          ID
      - in: query
        name: contactId
        description: Filter that restricts the search result to contacts with a specific
          ID
      - in: query
        name: id
        description: Filter that restricts the search result to address contact relations
          with a specific ID
      - in: query
        name: isPrimary
        description: Filter that restricts the search result depending on the flag
          used
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: page
        description: The page of results to search for
      - in: query
        name: typeId
        description: Filter that restricts the search result to address types with
          a specific ID
      - in: query
        name: with
        description: Includes the specified address contact relation information in
          the results
      responses:
        200:
          description: OK
      tags:
      - List
      - Address
      - Contact
      - Relations
  /rest/accounts/addresses/option_types:
    get:
      summary: List address option types
      description: List address option types.
      operationId: getRestAccountsAddressesOptionTypes
      x-api-path-slug: restaccountsaddressesoption-types-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Address
      - Option
      - Types
  /rest/accounts/addresses/pos_relations:
    get:
      summary: List address POS relations
      description: List address pos relations.
      operationId: getRestAccountsAddressesPosRelations
      x-api-path-slug: restaccountsaddressespos-relations-get
      parameters:
      - in: query
        name: itemsPerPage
        description: items per page
      - in: query
        name: page
        description: page
      - in: query
        name: with
        description: Includes the specified address pos relation information in the
          results
      responses:
        200:
          description: OK
      tags:
      - List
      - Address
      - POS
      - Relations
  /rest/accounts/addresses/relation_types:
    get:
      summary: List address relation types
      description: List address relation types.
      operationId: getRestAccountsAddressesRelationTypes
      x-api-path-slug: restaccountsaddressesrelation-types-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Address
      - Relation
      - Types
  /rest/accounts/addresses/relations/types/applications/{application}/{lang}:
    get:
      summary: List address relation types
      description: |-
        Lists address relation types. The application and the language must be specified.
        <br>Possible applications:
        <ul>
        <li>contact</li>
        <li>order</li>
        <li>warehouse</li>
        <li>pos</li>
        </ul>
      operationId: getRestAccountsAddressesRelationsTypesApplicationsApplicationLang
      x-api-path-slug: restaccountsaddressesrelationstypesapplicationsapplicationlang-get
      parameters:
      - in: path
        name: application
      - in: path
        name: lang
      responses:
        200:
          description: OK
      tags:
      - List
      - Address
      - Relation
      - Types
  /rest/accounts/addresses/{addressId}/options:
    get:
      summary: List address options
      description: Lists address options. The ID of the address must be specified.
      operationId: getRestAccountsAddressesAddressOptions
      x-api-path-slug: restaccountsaddressesaddressidoptions-get
      parameters:
      - in: path
        name: addressId
      responses:
        200:
          description: OK
      tags:
      - List
      - Address
      - Options
  /rest/accounts/contacts:
    get:
      summary: List contacts
      description: List contacts.
      operationId: getRestAccountsContacts
      x-api-path-slug: restaccountscontacts-get
      parameters:
      - in: query
        name: billingAddressId
        description: Filter that restricts the search result to contacts with a billing
          address with the id provided
      - in: query
        name: contactAddress
        description: Filter that restricts the search result to contacts with a specific
          address
      - in: query
        name: contactEmail
        description: Filter that restricts the search result to contacts resembling
          to the given email address
      - in: query
        name: contactId
        description: Filter that restricts the search result to a specific contact
      - in: query
        name: countryId
        description: Filter that restricts the search result to contacts with a specific
          country
      - in: query
        name: createdAtAfter
        description: Filter that restricts the search result to contacts that were
          created after a specific date
      - in: query
        name: createdAtBefore
        description: Filter that restricts the search result to contacts that were
          created before a specific date
      - in: query
        name: deliveryAddressId
        description: Filter that restricts the search result to contacts with a delivery
          address with the id provided
      - in: query
        name: email
        description: Filter that restricts the search result to contacts with a specific
          email address
      - in: query
        name: externalId
        description: Filter that restricts the search result to contacts with a specific
          externalId
      - in: query
        name: fullText
        description: Filter for a fulltext search
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: name
        description: Filter that restricts the search result to contacts with a specific
          name
      - in: query
        name: newsletterAllowance
        description: Filter that restricts the search result to contacts who registered
          for the newsletter
      - in: query
        name: newsletterAllowanceAfter
        description: Filter that restricts the search result to contacts who registered
          for the newsletter after a specific date
      - in: query
        name: newsletterAllowanceBefore
        description: Filter that restricts the search result to contacts who registered
          for the newsletter before a specific date
      - in: query
        name: number
        description: Filter that restricts the search result to contacts with a specific
          number
      - in: query
        name: page
        description: The page of results to search for
      - in: query
        name: plentyId
        description: Filter that restricts the search result to contacts with a specific
          plentyId
      - in: query
        name: postalCode
        description: Filter that restricts the search result to contacts with a specific
          postal code
      - in: query
        name: privatePhone
        description: Filter that restricts the search result to contacts with a private
          phone number
      - in: query
        name: referrerId
        description: Filter that restricts the search result to contacts with a specific
          referrer
      - in: query
        name: town
        description: Filter that restricts the search result to contacts with a specific
          town
      - in: query
        name: typeId
        description: Filter that restricts the search result to contacts with a specific
          contact type
      - in: query
        name: updatedAtAfter
        description: Filter that restricts the search result to contacts that were
          updated after a specific date
      - in: query
        name: updatedAtBefore
        description: Filter that restricts the search result to contacts that were
          updated before a specific date
      - in: query
        name: userId
        description: Filter that restricts the search result to contacts with a specific
          user
      - in: query
        name: with
        description: Includes the specified contact information in the results
      responses:
        200:
          description: OK
      tags:
      - List
      - Contacts
  /rest/accounts/contacts/classes:
    get:
      summary: List contact classes
      description: List contact classes.
      operationId: getRestAccountsContactsClasses
      x-api-path-slug: restaccountscontactsclasses-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Contact
      - Classes
  /rest/accounts/contacts/contact_events:
    get:
      summary: List contact events
      description: Lists contact events.
      operationId: getRestAccountsContactsContactEvents
      x-api-path-slug: restaccountscontactscontact-events-get
      parameters:
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: page
        description: The page of results to search for
      responses:
        200:
          description: OK
      tags:
      - List
      - Contact
      - Events
  /rest/accounts/contacts/departments:
    get:
      summary: List contact departments
      description: List contact departments.
      operationId: getRestAccountsContactsDepartments
      x-api-path-slug: restaccountscontactsdepartments-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Contact
      - Departments
  /rest/accounts/contacts/group_functions:
    get:
      summary: List all group function related data
      description: Lists all data that is related to the contact group function contents.
      operationId: getRestAccountsContactsGroupFunctions
      x-api-path-slug: restaccountscontactsgroup-functions-get
      responses:
        200:
          description: OK
      tags:
      - List
      - ""
      - Group
      - Function
      - Related
      - Data
  /rest/accounts/contacts/option_sub_types:
    get:
      summary: List contact option sub-types
      description: List contact option sub-types.
      operationId: getRestAccountsContactsOptionSubTypes
      x-api-path-slug: restaccountscontactsoption-sub-types-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Contact
      - Option
      - Sub-types
  /rest/accounts/contacts/option_types:
    get:
      summary: List contact option types
      description: List contact option types.
      operationId: getRestAccountsContactsOptionTypes
      x-api-path-slug: restaccountscontactsoption-types-get
      parameters:
      - in: query
        name: with
        description: Lists possible option sub-types for each listed option if the
          parameter subTypes is set
      responses:
        200:
          description: OK
      tags:
      - List
      - Contact
      - Option
      - Types
  /rest/accounts/contacts/positions:
    get:
      summary: List contact positions
      description: List contact positions.
      operationId: getRestAccountsContactsPositions
      x-api-path-slug: restaccountscontactspositions-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Contact
      - Positions
  /rest/accounts/contacts/types:
    get:
      summary: List contact types
      description: List contact types.
      operationId: getRestAccountsContactsTypes
      x-api-path-slug: restaccountscontactstypes-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Contact
      - Types
  /rest/accounts/contacts/{contactId}/addresses/{addressTypeId?}:
    get:
      summary: List addresses that are linked with contacts
      description: Lists addresses of the contact. The ID of the contact must be specified.
      operationId: getRestAccountsContactsContactAddressesAddresstype
      x-api-path-slug: restaccountscontactscontactidaddressesaddresstypeid-get
      parameters:
      - in: path
        name: addressTypeId?
      - in: path
        name: contactId
      responses:
        200:
          description: OK
      tags:
      - List
      - Addresses
      - That
      - Are
      - Linked
      - Contacts
  /rest/accounts/contacts/{contactId}/banks:
    get:
      summary: List bank accounts
      description: Lists bank accounts of the contact. The ID of the contact must
        be specified.
      operationId: getRestAccountsContactsContactBanks
      x-api-path-slug: restaccountscontactscontactidbanks-get
      parameters:
      - in: path
        name: contactId
      responses:
        200:
          description: OK
      tags:
      - List
      - Bank
      - Accounts
  /rest/accounts/contacts/{contactId}/contact_events:
    get:
      summary: List contact events by contact ID
      description: Lists contact events by contact ID. The ID of the contact must
        be specified.
      operationId: getRestAccountsContactsContactContactEvents
      x-api-path-slug: restaccountscontactscontactidcontact-events-get
      parameters:
      - in: path
        name: contactId
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: page
        description: The page of results to search for
      responses:
        200:
          description: OK
      tags:
      - List
      - Contact
      - Events
      - By
      - Contact
      - ID
  /rest/accounts/contacts/{contactId}/documents:
    get:
      summary: List documents for a single contact
      description: List documents for a single contact.
      operationId: getRestAccountsContactsContactDocuments
      x-api-path-slug: restaccountscontactscontactiddocuments-get
      parameters:
      - in: path
        name: contactId
      - in: query
        name: continuationToken
        description: token from previous request to continue listing documents
      responses:
        200:
          description: OK
      tags:
      - List
      - Documentsa
      - Single
      - Contact
  /rest/accounts/contacts/{contactId}/options:
    get:
      summary: List contact options by the contact ID
      description: Lists contact options. The ID of the contact must be specified.
      operationId: getRestAccountsContactsContactOptions
      x-api-path-slug: restaccountscontactscontactidoptions-get
      parameters:
      - in: path
        name: contactId
      responses:
        200:
          description: OK
      tags:
      - List
      - Contact
      - Options
      - By
      - Contact
      - ID
  /rest/accounts/order_summaries:
    get:
      summary: List order summaries
      description: List order summaries.
      operationId: getRestAccountsOrderSummaries
      x-api-path-slug: restaccountsorder-summaries-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Order
      - Summaries
  /rest/accounts/{accountId}/contacts:
    get:
      summary: List contacts
      description: Lists contacts of the account. The ID of the account must be specified.
      operationId: getRestAccountsAccountContacts
      x-api-path-slug: restaccountsaccountidcontacts-get
      parameters:
      - in: path
        name: accountId
      responses:
        200:
          description: OK
      tags:
      - List
      - Contacts
  /rest/availabilities:
    get:
      summary: List item availabilities
      description: Lists all item availabilities.
      operationId: getRestAvailabilities
      x-api-path-slug: restavailabilities-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Item
      - Availabilities
  /rest/basket/items:
    get:
      summary: List basket items
      description: Lists all items in the shopping cart for the current customer session.
      operationId: getRestBasketItems
      x-api-path-slug: restbasketitems-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Basket
      - Items
  /rest/categories:
    get:
      summary: List categories
      description: List categories.
      operationId: getRestCategories
      x-api-path-slug: restcategories-get
      parameters:
      - in: query
        name: categoryId
        description: The ID of the category
      - in: query
        name: itemsPerPage
        description: The number of results per page
      - in: query
        name: lang
        description: The languages of the category detail information
      - in: query
        name: level
        description: The level of the category
      - in: query
        name: linklist
        description: Filter for the linklist of categories
      - in: query
        name: name
        description: The name of the category
      - in: query
        name: page
        description: The requested page of results
      - in: query
        name: parentId
        description: The unique ID of the parent category
      - in: query
        name: plentyId
        description: The unique plenty ID of the client (store)
      - in: query
        name: type
        description: The category type
      - in: query
        name: updatedAt
        description: Filter restricts the list of results to items updated after the
          specified date
      - in: query
        name: with
        description: Includes the detail information, the active clients (stores)
          list of the category and/or the linked Elmar category for each client
      responses:
        200:
          description: OK
      tags:
      - List
      - Categories
  /rest/categories/{categoryId}/documents:
    get:
      summary: List documents of a category
      description: Lists the documents of a category. The ID of the category must
        be specified.
      operationId: getRestCategoriesCategoryDocuments
      x-api-path-slug: restcategoriescategoryiddocuments-get
      parameters:
      - in: path
        name: categoryId
      responses:
        200:
          description: OK
      tags:
      - List
      - Documents
      - Of
      - Category
  /rest/categories/{id}:
    get:
      summary: List categories
      description: List categories.
      operationId: getRestCategories
      x-api-path-slug: restcategoriesid-get
      parameters:
      - in: query
        name: categoryId
        description: The ID of the category
      - in: path
        name: id
      - in: query
        name: itemsPerPage
        description: The number of results per page
      - in: query
        name: lang
        description: The languages of the category detail information
      - in: query
        name: level
        description: The level of the category
      - in: query
        name: linklist
        description: Filter for the linklist of categories
      - in: query
        name: name
        description: The name of the category
      - in: query
        name: page
        description: The requested page of results
      - in: query
        name: parentId
        description: The unique ID of the parent category
      - in: query
        name: plentyId
        description: The unique plenty ID of the client (store)
      - in: query
        name: type
        description: The category type
      - in: query
        name: updatedAt
        description: Filter restricts the list of results to items updated after the
          specified date
      - in: query
        name: with
        description: Includes the detail information, the active clients (stores)
          list of the category and/or the linked Elmar category for each client
      responses:
        200:
          description: OK
      tags:
      - List
      - Categories
  /rest/comments/{referenceType}/{referenceValue}:
    get:
      summary: List comments
      description: Lists comments. The reference type and the reference value must
        be specified (e.g. the reference type is 'order' and the reference value is
        the ID of the order).
      operationId: getRestCommentsReferencetypeReferencevalue
      x-api-path-slug: restcommentsreferencetypereferencevalue-get
      parameters:
      - in: query
        name: isVisibleForContact
        description: If true, the comment is visible for the associated contact
      - in: path
        name: referenceType
      - in: path
        name: referenceValue
      - in: query
        name: userId
        description: The ID of the user the comment belongs to
      responses:
        200:
          description: OK
      tags:
      - List
      - Comments
  /rest/customer_contracts:
    get:
      summary: List contracts
      description: List contracts.
      operationId: getRestCustomerContracts
      x-api-path-slug: restcustomer-contracts-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Contracts
  /rest/exports:
    get:
      summary: List elastic exports
      description: Lists elastic exports.
      operationId: getRestExports
      x-api-path-slug: restexports-get
      parameters:
      - in: query
        name: formatKey
        description: The format of the export
      - in: query
        name: id
        description: The ID of the export
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: name
        description: The name of the export
      - in: query
        name: page
        description: The page of results to search for
      - in: query
        name: type
        description: The type of the export
      responses:
        200:
          description: OK
      tags:
      - List
      - Elastic
      - Exports
  /rest/feedbacks/comments:
    get:
      summary: List feedback comments
      description: Lists feedback comments.
      operationId: getRestFeedbacksComments
      x-api-path-slug: restfeedbackscomments-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Feedback
      - Comments
  /rest/feedbacks/feedback/replies/{feedbackId}:
    get:
      summary: List feedback replies
      description: Lists feedback replies. The ID of the feedback must be specified.
      operationId: getRestFeedbacksFeedbackRepliesFeedback
      x-api-path-slug: restfeedbacksfeedbackrepliesfeedbackid-get
      parameters:
      - in: path
        name: feedbackId
      responses:
        200:
          description: OK
      tags:
      - List
      - Feedback
      - Replies
  /rest/feedbacks/feedbacks:
    get:
      summary: List feedbacks
      description: Lists feedbacks. The reference type and the reference value must
        be specified (e.g. the reference type is 'order' and the reference value is
        the ID of the order).
      operationId: getRestFeedbacksFeedbacks
      x-api-path-slug: restfeedbacksfeedbacks-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Feedbacks
  /rest/feedbacks/ratings:
    get:
      summary: List feedback ratings
      description: Lists feedback ratings.
      operationId: getRestFeedbacksRatings
      x-api-path-slug: restfeedbacksratings-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Feedback
      - Ratings
  /rest/item_sets:
    get:
      summary: List item sets
      description: Lists all item sets.
      operationId: getRestItemSets
      x-api-path-slug: restitem-sets-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Item
      - Sets
  /rest/item_sets/{setId}/components:
    get:
      summary: List item set components of an item set
      description: Lists the item set components of an item set. The ID of the item
        set must be specified.
      operationId: getRestItemSetsSetComponents
      x-api-path-slug: restitem-setssetidcomponents-get
      parameters:
      - in: path
        name: setId
      responses:
        200:
          description: OK
      tags:
      - List
      - Item
      - Set
      - Components
      - Of
      - Item
      - Set
  /rest/items/attributes:
    get:
      summary: List attributes
      description: Lists all attributes.
      operationId: getRestItemsAttributes
      x-api-path-slug: restitemsattributes-get
      parameters:
      - in: query
        name: updatedAt
        description: Filter restricts the list of results to items updated after the
          specified date
      - in: query
        name: with
        description: Includes the specified attribute information in the results
      responses:
        200:
          description: OK
      tags:
      - List
      - Attributes
  /rest/items/attributes/{attributeId}/names/{lang}:
    get:
      summary: List attribute names
      description: Lists the attribute names of an attribute.
      operationId: getRestItemsAttributesAttributeNamesLang
      x-api-path-slug: restitemsattributesattributeidnameslang-get
      parameters:
      - in: path
        name: attributeId
      - in: path
        name: lang
      responses:
        200:
          description: OK
      tags:
      - List
      - Attribute
      - Names
  /rest/items/attributes/{attributeId}/values:
    get:
      summary: List attribute values
      description: Lists the attribute values for an attribute. The attribute ID must
        be specified.
      operationId: getRestItemsAttributesAttributeValues
      x-api-path-slug: restitemsattributesattributeidvalues-get
      parameters:
      - in: path
        name: attributeId
      - in: query
        name: updatedAt
        description: Filter restricts the list of results to items updated after the
          specified date
      - in: query
        name: with
        description: Includes the specified attribute value information in the results
      responses:
        200:
          description: OK
      tags:
      - List
      - Attribute
      - Values
  /rest/items/barcodes:
    get:
      summary: List barcodes
      description: Lists all barcodes.
      operationId: getRestItemsBarcodes
      x-api-path-slug: restitemsbarcodes-get
      parameters:
      - in: query
        name: updatedAt
        description: Filter restricts the list of results to items updated after the
          specified date
      responses:
        200:
          description: OK
      tags:
      - List
      - Barcodes
  /rest/items/barcodes/referrer/{referrerId}:
    get:
      summary: List barcodes by referrer
      description: Lists barcodes linked to the specified referrer. The ID of the
        referrer must be specified.
      operationId: getRestItemsBarcodesReferrerReferrer
      x-api-path-slug: restitemsbarcodesreferrerreferrerid-get
      parameters:
      - in: path
        name: referrerId
      responses:
        200:
          description: OK
      tags:
      - List
      - Barcodes
      - By
      - Referrer
  /rest/items/barcodes/type/{type}:
    get:
      summary: List barcodes by type
      description: Lists all barcodes of a specific type. The type must be specified.
      operationId: getRestItemsBarcodesTypeType
      x-api-path-slug: restitemsbarcodestypetype-get
      parameters:
      - in: path
        name: type
      responses:
        200:
          description: OK
      tags:
      - List
      - Barcodes
      - By
      - Type
  /rest/items/item_shipping_profiles:
    get:
      summary: List all shipping profiles of all items
      description: |-
        Lists all shipping profiles of all items. Results can be filtered by the timestamp of the link between items and shipping profiles (eq, lt, lte, gt, gte, between).
        <ul>
        <li>eq = Equal to</li>
        <li>gte = Greater than or equal to</li>
        <li>gt = Greater than</li>
        <li>lte = Less than or equal to</li>
        <li>lt = Less than</li>
        <li>between = Date range</li>
        </ul>
        Example: updated=gt:2018-04-16 16:00:00 returns all items with shipping profiles that were activated after 4pm on the 16th of April 2018.
      operationId: getRestItemsItemShippingProfiles
      x-api-path-slug: restitemsitem-shipping-profiles-get
      responses:
        200:
          description: OK
      tags:
      - List
      - ""
      - Shipping
      - Profiles
      - Of
      - ""
      - Items
  /rest/items/labels:
    get:
      summary: List item label templates
      description: Lists the ID and name of all item label templates saved in the
        system.
      operationId: getRestItemsLabels
      x-api-path-slug: restitemslabels-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Item
      - Label
      - Templates
  /rest/items/manufacturers:
    get:
      summary: List manufacturers
      description: |-
        Lists all manufacturers in the system.

        Display a listing of the resource.
      operationId: getRestItemsManufacturers
      x-api-path-slug: restitemsmanufacturers-get
      parameters:
      - in: query
        name: name
        description: Filter restricts the list of results to records with specified
          name
      - in: query
        name: updatedAt
        description: Filter restricts the list of results to records updated after
          the specified date
      responses:
        200:
          description: OK
      tags:
      - List
      - Manufacturers
  /rest/items/manufacturers/{id}/commissions:
    get:
      summary: List commissions
      description: Lists all commissions associated with a manufacturer. The ID of
        the manufacturer must be specified.
      operationId: getRestItemsManufacturersCommissions
      x-api-path-slug: restitemsmanufacturersidcommissions-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - List
      - Commissions
  /rest/items/properties:
    get:
      summary: List properties
      description: Lists all properties.
      operationId: getRestItemsProperties
      x-api-path-slug: restitemsproperties-get
      parameters:
      - in: query
        name: groupId
        description: Filter restricts the list of results to items linked to a specified
          property group
      - in: query
        name: updatedAt
        description: Filter restricts the list of results to items updated after the
          specified date
      - in: query
        name: with
        description: Includes the specified property information in the results
      responses:
        200:
          description: OK
      tags:
      - List
      - Properties
  /rest/items/properties/{id}/market_references:
    get:
      summary: List property market references
      description: Lists the property market references of a property. The ID of the
        property must be specified.
      operationId: getRestItemsPropertiesMarketReferences
      x-api-path-slug: restitemspropertiesidmarket-references-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - List
      - Property
      - Market
      - References
  /rest/items/properties/{id}/names:
    get:
      summary: List the property names
      description: Lists the names of a property in all languages. The ID of the property
        must be specified.
      operationId: getRestItemsPropertiesNames
      x-api-path-slug: restitemspropertiesidnames-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - List
      - Property
      - Names
  /rest/items/properties/{propertyId}/selections:
    get:
      summary: List property selections
      description: Lists the property selections of a property. The ID of the property
        must be specified.
      operationId: getRestItemsPropertiesPropertySelections
      x-api-path-slug: restitemspropertiespropertyidselections-get
      parameters:
      - in: path
        name: propertyId
      responses:
        200:
          description: OK
      tags:
      - List
      - Property
      - Selections
  /rest/items/properties/{propertyId}/selections/{id}/{lang}:
    get:
      summary: List property selections by language
      description: Lists the property selections of a property for a specific language.
        The ID and language of the property must be specified.
      operationId: getRestItemsPropertiesPropertySelectionsLang
      x-api-path-slug: restitemspropertiespropertyidselectionsidlang-get
      parameters:
      - in: path
        name: id
      - in: path
        name: lang
      - in: path
        name: propertyId
      responses:
        200:
          description: OK
      tags:
      - List
      - Property
      - Selections
      - By
      - Language
  /rest/items/properties/{propertyId}/selections/{lang}:
    get:
      summary: List property selections
      description: Lists the property selections of a property. The ID of the property
        must be specified.
      operationId: getRestItemsPropertiesPropertySelectionsLang
      x-api-path-slug: restitemspropertiespropertyidselectionslang-get
      parameters:
      - in: path
        name: lang
      - in: path
        name: propertyId
      responses:
        200:
          description: OK
      tags:
      - List
      - Property
      - Selections
  /rest/items/property_groups:
    get:
      summary: List property groups
      description: Lists the property groups.
      operationId: getRestItemsPropertyGroups
      x-api-path-slug: restitemsproperty-groups-get
      parameters:
      - in: query
        name: with
        description: Includes the specified property group information in the results
      responses:
        200:
          description: OK
      tags:
      - List
      - Property
      - Groups
  /rest/items/property_groups/{id}/names:
    get:
      summary: List the property group names of a property group
      description: Lists the property group names of a property group in all languages.
        The ID of the property group must be specified.
      operationId: getRestItemsPropertyGroupsNames
      x-api-path-slug: restitemsproperty-groupsidnames-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - List
      - Property
      - Group
      - Names
      - Of
      - Property
      - Group
  /rest/items/sales_prices:
    get:
      summary: List sales prices
      description: Lists all sales prices.
      operationId: getRestItemsSalesPrices
      x-api-path-slug: restitemssales-prices-get
      parameters:
      - in: query
        name: updatedAt
        description: Filter restricts the list of results to items updated after the
          specified date
      responses:
        200:
          description: OK
      tags:
      - List
      - Sales
      - Prices
  /rest/items/sales_prices/{id}/accounts:
    get:
      summary: List referrer accounts
      description: Lists all activated referrer accounts of a sales price.
      operationId: getRestItemsSalesPricesAccounts
      x-api-path-slug: restitemssales-pricesidaccounts-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - List
      - Referrer
      - Accounts
  /rest/items/sales_prices/{id}/countries:
    get:
      summary: List countries by sales price
      description: Lists active countries for a sales price. The ID of the sales price
        must be specified.
      operationId: getRestItemsSalesPricesCountries
      x-api-path-slug: restitemssales-pricesidcountries-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - List
      - Countries
      - By
      - Sales
      - Price
  /rest/items/sales_prices/{id}/currencies:
    get:
      summary: List activated currencies
      description: List all currencies activated for a sales price. The ID of the
        sales price must be specified.
      operationId: getRestItemsSalesPricesCurrencies
      x-api-path-slug: restitemssales-pricesidcurrencies-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - List
      - Activated
      - Currencies
  /rest/items/sales_prices/{id}/customer_classes:
    get:
      summary: List activated customer classes
      description: Lists the activated customer classes for a sales price. The ID
        of the sales price must be specified.
      operationId: getRestItemsSalesPricesCustomerClasses
      x-api-path-slug: restitemssales-pricesidcustomer-classes-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - List
      - Activated
      - Customer
      - Classes
  /rest/items/sales_prices/{id}/names:
    get:
      summary: List names of a sales price
      description: Lists the names of a sales price in all languages. The ID of the
        sales price must be specified.
      operationId: getRestItemsSalesPricesNames
      x-api-path-slug: restitemssales-pricesidnames-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - List
      - Names
      - Of
      - Sales
      - Price
  /rest/items/sales_prices/{id}/online_stores:
    get:
      summary: List activated clients (stores)
      description: Lists all activated clients (stores) for a sales price. The ID
        of the sales price must be specified.
      operationId: getRestItemsSalesPricesOnlineStores
      x-api-path-slug: restitemssales-pricesidonline-stores-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - List
      - Activated
      - Clients
      - (stores)
  /rest/items/sales_prices/{id}/referrers:
    get:
      summary: List activated referrers
      description: Lists all activated referrers for a sales price. The ID of the
        sales price must be specified.
      operationId: getRestItemsSalesPricesReferrers
      x-api-path-slug: restitemssales-pricesidreferrers-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - List
      - Activated
      - Referrers
  /rest/items/units:
    get:
      summary: List units
      description: Lists all units.
      operationId: getRestItemsUnits
      x-api-path-slug: restitemsunits-get
      parameters:
      - in: query
        name: updatedAt
        description: Filter restricts the list of results to items updated after the
          specified date
      responses:
        200:
          description: OK
      tags:
      - List
      - Units
  /rest/items/units/{id}/names:
    get:
      summary: List unit names
      description: Lists the unit names of a unit. The ID of the unit must be specified.
      operationId: getRestItemsUnitsNames
      x-api-path-slug: restitemsunitsidnames-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - List
      - Unit
      - Names
  /rest/items/variations/variation_markets:
    get:
      summary: List all links between variations and markets
      description: |-
        Lists all links between variations and markets.
        Results can be filtered by the ID of the variation and by the ID of the market, e.g. "variationId=1030"
        lists all links of the variation with the ID 1030.
      operationId: getRestItemsVariationsVariationMarkets
      x-api-path-slug: restitemsvariationsvariation-markets-get
      responses:
        200:
          description: OK
      tags:
      - List
      - ""
      - Links
      - Between
      - Variations
      - Markets
  /rest/items/{id}/images:
    get:
      summary: List images of an item
      description: Lists all images of an item. The item ID must be specified.
      operationId: getRestItemsImages
      x-api-path-slug: restitemsidimages-get
      parameters:
      - in: path
        name: id
      - in: query
        name: updatedAt
        description: Filter restricts the list of results to items updated after the
          specified date
      responses:
        200:
          description: OK
      tags:
      - List
      - Images
      - Of
      - Item
  /rest/items/{id}/images/attribute_value_markets:
    get:
      summary: List attribute value image link
      description: Lists the images linked to an attribute value.
      operationId: getRestItemsImagesAttributeValueMarkets
      x-api-path-slug: restitemsidimagesattribute-value-markets-get
      parameters:
      - in: query
        name: attributeId
        description: The unique ID of the attribute
      - in: path
        name: id
      - in: query
        name: imageId
        description: The unique ID of the image
      - in: query
        name: itemId
        description: The unique ID of the item
      - in: query
        name: valueId
        description: The unique ID of the attribute value
      responses:
        200:
          description: OK
      tags:
      - List
      - Attribute
      - Value
      - Image
      - Link
  /rest/items/{id}/images/{imageId}/availabilities:
    get:
      summary: List availabilities
      description: List all availabilities of an image. The image ID must be specified.
      operationId: getRestItemsImagesImageAvailabilities
      x-api-path-slug: restitemsidimagesimageidavailabilities-get
      parameters:
      - in: path
        name: id
      - in: path
        name: imageId
      responses:
        200:
          description: OK
      tags:
      - List
      - Availabilities
  /rest/items/{id}/images/{imageId}/names:
    get:
      summary: List names of an image
      description: Lists all names of an image. The image ID must be specified.
      operationId: getRestItemsImagesImageNames
      x-api-path-slug: restitemsidimagesimageidnames-get
      parameters:
      - in: path
        name: id
      - in: path
        name: imageId
      responses:
        200:
          description: OK
      tags:
      - List
      - Names
      - Of
      - Image
  /rest/items/{id}/images/{imageId}/variation_images:
    get:
      summary: List image links of an image
      description: Lists all variations linked to an image. The image ID must be specified.
      operationId: getRestItemsImagesImageVariationImages
      x-api-path-slug: restitemsidimagesimageidvariation-images-get
      parameters:
      - in: path
        name: id
      - in: path
        name: imageId
      responses:
        200:
          description: OK
      tags:
      - List
      - Image
      - Links
      - Of
      - Image
  /rest/items/{id}/item_cross_selling:
    get:
      summary: List cross-selling links
      description: Lists all cross-selling items linked to an item. The ID of the
        item must be specified.
      operationId: getRestItemsItemCrossSelling
      x-api-path-slug: restitemsiditem-cross-selling-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - List
      - Cross-selling
      - Links
  /rest/items/{id}/variation_images:
    get:
      summary: List image links of an item
      description: Lists all images linked to an item. The item ID must be specified.
      operationId: getRestItemsVariationImages
      x-api-path-slug: restitemsidvariation-images-get
      parameters:
      - in: path
        name: id
      responses:
        200:
          description: OK
      tags:
      - List
      - Image
      - Links
      - Of
      - Item
  /rest/items/{id}/variations/{variationId}/descriptions:
    get:
      summary: List texts
      description: Lists the texts for an item in all available languages. The ID
        of the variation must be specified.
      operationId: getRestItemsVariationsVariationDescriptions
      x-api-path-slug: restitemsidvariationsvariationiddescriptions-get
      parameters:
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - List
      - Texts
  /rest/items/{id}/variations/{variationId}/images:
    get:
      summary: List images of a variation
      description: Lists all images of a variation. The variation ID must be specified.
      operationId: getRestItemsVariationsVariationImages
      x-api-path-slug: restitemsidvariationsvariationidimages-get
      parameters:
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - List
      - Images
      - Of
      - Variation
  /rest/items/{id}/variations/{variationId}/market_ident_numbers:
    get:
      summary: List ident number of a variation
      description: Lists the ident number (ASIN/ePID) of a variation. The ID of the
        item and the ID of the variation must be specified.
      operationId: getRestItemsVariationsVariationMarketEntNumbers
      x-api-path-slug: restitemsidvariationsvariationidmarket-ident-numbers-get
      parameters:
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - List
      - Ident
      - Number
      - Of
      - Variation
  /rest/items/{id}/variations/{variationId}/stock:
    get:
      summary: List stock of a variation per warehouse
      description: Lists stock of a variation per warehouse. The ID of the item and
        the ID of the variation must be specified.
      operationId: getRestItemsVariationsVariationStock
      x-api-path-slug: restitemsidvariationsvariationidstock-get
      parameters:
      - in: query
        name: columns
        description: The properties to be loaded
      - in: path
        name: id
      - in: query
        name: itemId
        description: The ID of the item
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - List
      - Stock
      - Of
      - Variation
      - Per
      - Warehouse
  /rest/items/{id}/variations/{variationId}/stock/movements:
    get:
      summary: List stock movements
      description: |-
        Lists stock movements for a variation. The ID of the item and the ID of the variation must be specified. To get movements older than 3 months, set the 'year' parameter.
        NOTE: You can either get archive entries or non-archive entries. You can not get entries for the current year that are younger and older than 3 months with one request. You need separate requests to get entries older and younger than 3 months. To get all entries younger than 3 month you do not need to specify a year or any createdAt parameter.
      operationId: getRestItemsVariationsVariationStockMovements
      x-api-path-slug: restitemsidvariationsvariationidstockmovements-get
      parameters:
      - in: query
        name: columns
        description: The properties to be loaded
      - in: query
        name: createdAtFrom
        description: Get entries with createdAt date after this date
      - in: query
        name: createdAtTo
        description: Get entries with createdAt date before this date
      - in: path
        name: id
      - in: query
        name: itemId
        description: The ID of the item
      - in: query
        name: itemsPerPage
        description: The number of items per page
      - in: query
        name: page
        description: The requested page
      - in: path
        name: variationId
      - in: query
        name: warehouseId
        description: The ID of the warehouse
      - in: query
        name: year
        description: Get entries from the archive for the given year
      responses:
        200:
          description: OK
      tags:
      - List
      - Stock
      - Movements
  /rest/items/{id}/variations/{variationId}/stock/storageLocations:
    get:
      summary: List stock of a variation per storage locations
      description: Lists stock of a variation per storage location. The ID of the
        item and the ID of the variation must be specified.
      operationId: getRestItemsVariationsVariationStockStoragelocations
      x-api-path-slug: restitemsidvariationsvariationidstockstoragelocations-get
      parameters:
      - in: query
        name: columns
        description: The properties to be loaded
      - in: path
        name: id
      - in: query
        name: itemId
        description: The ID of the item
      - in: query
        name: itemsPerPage
        description: The number of items per page
      - in: query
        name: page
        description: The requested page
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - List
      - Stock
      - Of
      - Variation
      - Per
      - Storage
      - Locations
  /rest/items/{id}/variations/{variationId}/variation_additional_skus:
    get:
      summary: List additional SKUs
      description: Lists the additional SKUs of a variation. Filters must be specified.
      operationId: getRestItemsVariationsVariationVariationAdditionalSkus
      x-api-path-slug: restitemsidvariationsvariationidvariation-additional-skus-get
      parameters:
      - in: body
        name: /rest/items/{id}/variations/{variationId}/variation_additional_skus
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - List
      - Additional
      - SKUs
  /rest/items/{id}/variations/{variationId}/variation_barcodes:
    get:
      summary: List variation barcodes
      description: Lists all barcodes of a variation. The ID of the item and the ID
        of the variation must be specified.
      operationId: getRestItemsVariationsVariationVariationBarcodes
      x-api-path-slug: restitemsidvariationsvariationidvariation-barcodes-get
      parameters:
      - in: path
        name: id
      - in: path
        name: variationId
      - in: query
        name: with
        description: Includes the specified variation barcode information in the results
      responses:
        200:
          description: OK
      tags:
      - List
      - Variation
      - Barcodes
  /rest/items/{id}/variations/{variationId}/variation_bundles:
    get:
      summary: List bundle components
      description: List all components of a bundle. The ID of the item and the ID
        of the variation to which bundle components were added must be specified.
      operationId: getRestItemsVariationsVariationVariationBundles
      x-api-path-slug: restitemsidvariationsvariationidvariation-bundles-get
      parameters:
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - List
      - Bundle
      - Components
  /rest/items/{id}/variations/{variationId}/variation_categories:
    get:
      summary: List categories linked to a variation
      description: Lists all categories linked to a variation.
      operationId: getRestItemsVariationsVariationVariationCategories
      x-api-path-slug: restitemsidvariationsvariationidvariation-categories-get
      parameters:
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - List
      - Categories
      - Linked
      - To
      - Variation
  /rest/items/{id}/variations/{variationId}/variation_clients:
    get:
      summary: List clients linked to a variation
      description: Lists all clients (stores) linked to a variation. The ID of the
        variation must be specified.
      operationId: getRestItemsVariationsVariationVariationClients
      x-api-path-slug: restitemsidvariationsvariationidvariation-clients-get
      parameters:
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - List
      - Clients
      - Linked
      - To
      - Variation
  /rest/items/{id}/variations/{variationId}/variation_default_categories:
    get:
      summary: List default category links
      description: Lists the default category of a variation for all clients (stores).
        The ID of the item and the ID of the variation must be specified.
      operationId: getRestItemsVariationsVariationVariationDefaultCategories
      x-api-path-slug: restitemsidvariationsvariationidvariation-default-categories-get
      parameters:
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - List
      - Default
      - Category
      - Links
  /rest/items/{id}/variations/{variationId}/variation_images:
    get:
      summary: List image links of a variation
      description: Lists all images linked to a variation. The variation ID must be
        specified.
      operationId: getRestItemsVariationsVariationVariationImages
      x-api-path-slug: restitemsidvariationsvariationidvariation-images-get
      parameters:
      - in: path
        name: id
      - in: query
        name: updatedAt
        description: Filter restricts the list of results to variation images updated
          after the specified date
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - List
      - Image
      - Links
      - Of
      - Variation
  /rest/items/{id}/variations/{variationId}/variation_markets:
    get:
      summary: List markets linked to a variation
      description: Lists all markets linked to a variation. The ID of the item and
        the ID of the variation must be specified.
      operationId: getRestItemsVariationsVariationVariationMarkets
      x-api-path-slug: restitemsidvariationsvariationidvariation-markets-get
      parameters:
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - List
      - Markets
      - Linked
      - To
      - Variation
  /rest/items/{id}/variations/{variationId}/variation_properties:
    get:
      summary: List property values linked to a variation
      description: Lists the property values linked to a variation. The ID of the
        item and the ID of the variation must be specified.
      operationId: getRestItemsVariationsVariationVariationProperties
      x-api-path-slug: restitemsidvariationsvariationidvariation-properties-get
      parameters:
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - List
      - Property
      - Values
      - Linked
      - To
      - Variation
  /rest/items/{id}/variations/{variationId}/variation_sales_prices:
    get:
      summary: List sales prices of a variation
      description: Lists the sales prices of a variation. The ID of the variation
        must be specified.
      operationId: getRestItemsVariationsVariationVariationSalesPrices
      x-api-path-slug: restitemsidvariationsvariationidvariation-sales-prices-get
      parameters:
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - List
      - Sales
      - Prices
      - Of
      - Variation
  /rest/items/{id}/variations/{variationId}/variation_skus:
    get:
      summary: List SKUs
      description: Lists the SKUs of a variation. Filters must be specified.
      operationId: getRestItemsVariationsVariationVariationSkus
      x-api-path-slug: restitemsidvariationsvariationidvariation-skus-get
      parameters:
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - List
      - SKUs
  /rest/items/{id}/variations/{variationId}/variation_warehouses:
    get:
      summary: List the warehouses linked to a variation
      description: Lists the warehouses linked to a variation. The ID of the item
        and the ID of the variation must be specified.
      operationId: getRestItemsVariationsVariationVariationWarehouses
      x-api-path-slug: restitemsidvariationsvariationidvariation-warehouses-get
      parameters:
      - in: path
        name: id
      - in: path
        name: variationId
      responses:
        200:
          description: OK
      tags:
      - List
      - Warehouses
      - Linked
      - To
      - Variation
  /rest/items/{itemId}/item_shipping_profiles:
    get:
      summary: List shipping profiles of an item
      description: Lists the shipping profiles linked to an item. The ID of the item
        must be specified.
      operationId: getRestItemsItemItemShippingProfiles
      x-api-path-slug: restitemsitemiditem-shipping-profiles-get
      parameters:
      - in: path
        name: itemId
      responses:
        200:
          description: OK
      tags:
      - List
      - Shipping
      - Profiles
      - Of
      - Item
  /rest/items/{itemId}/variations:
    get:
      summary: List variations of an item
      description: Lists all variations of an item. The ID of the item must be specified.
      operationId: getRestItemsItemVariations
      x-api-path-slug: restitemsitemidvariations-get
      parameters:
      - in: query
        name: barcode
        description: Filter restricts the list of results to variations with the specified
          barcode
      - in: query
        name: createdBetween
        description: Filter restricts the list of results to variations created during
          the specified period
      - in: query
        name: isActive
        description: Filter restricts the list of results to variations that are active
      - in: query
        name: isBundle
        description: Filter restricts the list of results to variations to which variations
          were added to create a bundle
      - in: query
        name: isMain
        description: Filter restricts the list of results to variations that are main
          variations
      - in: path
        name: itemId
      - in: query
        name: itemsPerPage
        description: Limits the number of results listed per page to a specific number
      - in: query
        name: lang
        description: The language of the variation information
      - in: query
        name: manufacturerId
        description: Filter restricts the list of results to variations with the specified
          manufacturer ID
      - in: query
        name: numberExact
        description: Filter restricts the list of results to the variation with the
          variation number specified
      - in: query
        name: numberFuzzy
        description: Filter restricts the list of results to variations with numbers
          that contain the variation number specified (SQL LIKE operator)
      - in: query
        name: page
        description: Limits the results to a specific page
      - in: query
        name: relatedUpdatedBetween
        description: Filter restricts the list of results to those variations for
          which related information was updated during the specified period
      - in: query
        name: supplierNumber
        description: Filter restricts the list of results to variations with the specified
          supplier number
      - in: query
        name: updatedBetween
        description: Filter restricts the list of results to variations updated during
          the specified period
      - in: query
        name: with
        description: Includes the specified variation information in the results
      responses:
        200:
          description: OK
      tags:
      - List
      - Variations
      - Of
      - Item
  /rest/listings:
    get:
      summary: List listing
      description: Lists listings by filter options.
      operationId: getRestListings
      x-api-path-slug: restlistings-get
      parameters:
      - in: query
        name: id
        description: Filter that restricts the search result to listings with specific
          listing ID
      - in: query
        name: itemId
        description: Filter that restricts the search result to listings with specific
          item ID
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: page
        description: The page of results to search for
      - in: query
        name: stockDependenceTypeId
        description: Filter that restricts the search result to listings with specific
          stock dependence type ID
      - in: query
        name: typeId
        description: Filter that restricts the search result to listings with specific
          type ID
      - in: query
        name: unitCombinationId
        description: Filter that restricts the search result to listings with specific
          unit combination ID
      - in: query
        name: with
        description: An array with child instances to be loaded
      responses:
        200:
          description: OK
      tags:
      - List
      - Listing
  /rest/listings/markets:
    get:
      summary: List listing markets
      description: Lists listing market by filter options.
      operationId: getRestListingsMarkets
      x-api-path-slug: restlistingsmarkets-get
      parameters:
      - in: query
        name: credentialsId
        description: Filter that restricts the search result to listing markets with
          given credential ID
      - in: query
        name: directoryId
        description: Filter that restricts the search result to listing markets with
          a given directory ID
      - in: query
        name: duration
        description: Filter that restricts the search result to listing markets with
          given duration
      - in: query
        name: id
        description: Filter that restricts the search result to listing markets that
          match the given ID(s)
      - in: query
        name: itemId
        description: Filter that restricts the search result to listing markets that
          belong to a given item ID
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: listingId
        description: Filter that restricts the search result to listing markets that
          belong to a given listing ID
      - in: query
        name: listingTypeId
        description: Filter that restricts the search result to listing markets that
          belong to a listing of a custom type ID
      - in: query
        name: page
        description: The page of results to search for
      - in: query
        name: referrerId
        description: Filter that restricts the search result to listing markets with
          given referrer ID
      - in: query
        name: shippingProfileId
        description: Filter that restricts the search result to listing markets that
          belong to a given shipping profile ID
      - in: query
        name: status
        description: Filter that restricts the search result to listing markets with
          a custom status condition
      - in: query
        name: stockCondition
        description: Filter that restricts the search result to listing markets with
          a custom stock condition
      - in: query
        name: stockDependenceTypeId
        description: Filter that restricts the search result to listing markets that
          belong to a listing with a custom stock dependence type ID
      - in: query
        name: updatedAtFrom
        description: Filter that restricts the search result to listing markets that
          were last updated on the specified date
      - in: query
        name: updatedAtTo
        description: Filter that restricts the search result to listing markets that
          were last updated within a specified period of time
      - in: query
        name: variationId
        description: Filter that restricts the search result to listing markets that
          match the given variation ID(s)
      - in: query
        name: variations
        description: Filter that restricts the search result to listing markets with
          a custom variation condition
      - in: query
        name: verified
        description: Filter that restricts the search result to listing markets that
          are verified
      - in: query
        name: with
        description: An array with child instances to be loaded
      responses:
        200:
          description: OK
      tags:
      - List
      - Listing
      - Markets
  /rest/listings/markets/histories:
    get:
      summary: List listing market history
      description: Lists listing market history by filter options.
      operationId: getRestListingsMarketsHistories
      x-api-path-slug: restlistingsmarketshistories-get
      parameters:
      - in: query
        name: credentialsId
        description: Filter that restricts the search result to listing market histories
          with given credential ID
      - in: query
        name: directoryId
        description: Filter that restricts the search result to listing market histories
          with a given directory ID
      - in: query
        name: duration
        description: Filter that restricts the search result to listing market histories
          with given duration
      - in: query
        name: externalId
        description: Filter that restricts the search result to listing market histories
          with given external id
      - in: query
        name: firstPlatformCategoryId
        description: Filter that restricts the search result to listing market histories
          with first platform category ID equal to the given ID
      - in: query
        name: firstShopCategoryId
        description: Filter that restricts the search result to listing market histories
          with first shop category ID equal to the given ID
      - in: query
        name: isClickAndCollect
        description: Filter that restricts the search result to listing market histories
          that belong to eBay Click & Collect
      - in: query
        name: isEbayPlus
        description: Filter that restricts the search result to listing market histories
          that belong to eBay Plus
      - in: query
        name: itemId
        description: Filter that restricts the search result to listing market histories
          that belong to a given item ID
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: lastSale
        description: Filter that restricts the search result to listing market histories
          with last sale before given date
      - in: query
        name: listingId
        description: Filter that restricts the search result to listing market histories
          that belong to a given listing ID
      - in: query
        name: listingMarketId
        description: Filter that restricts the search result to listing market histories
          that match the given listing market ID(s)
      - in: query
        name: listingTypeId
        description: Filter that restricts the search result to listing market histories
          that belong to a listing of a custom type ID
      - in: query
        name: page
        description: The page of results to search for
      - in: query
        name: referrerId
        description: Filter that restricts the search result to listing market histories
          with given referrer ID
      - in: query
        name: secondPlatformCategoryId
        description: Filter that restricts the search result to listing market histories
          with second platform category ID equal to the given ID
      - in: query
        name: secondShopCategoryId
        description: Filter that restricts the search result to listing market histories
          with second shop category ID equal to the given ID
      - in: query
        name: shippingProfileId
        description: Filter that restricts the search result to listing market histories
          that belong to a given shipping profile
      - in: query
        name: statusId
        description: Filter that restricts the search result to listing market histories
          with a custom status status ID
      - in: query
        name: stockCondition
        description: Filter that restricts the search result to listing market histories
          with a custom stock condition
      - in: query
        name: stockDependenceTypeId
        description: Filter that restricts the search result to listing market histories
          that belong to a listing with a custom stock dependence type ID
      - in: query
        name: textData
        description: Filter that restricts the search result to listing market histories
          that match given text in listing title or description
      - in: query
        name: thirdShopCategoryId
        description: Filter that restricts the search result to listing market histories
          with third shop category ID equal to the given ID
      - in: query
        name: updatedAtFrom
        description: Filter that restricts the search result to listing market histories
          that were last updated on the specified date
      - in: query
        name: updatedAtTo
        description: Filter that restricts the search result to listing market histories
          that were last updated within a specified period of time
      - in: query
        name: variationId
        description: Filter that restricts the search result to listing market histories
          that match the given variation ID(s)
      - in: query
        name: variations
        description: Filter that restricts the search result to listing market histories
          with a custom variation condition
      - in: query
        name: verified
        description: Filter that restricts the search result to listing market histories
          that are verified
      - in: query
        name: with
        description: An array with child instances to be loaded
      responses:
        200:
          description: OK
      tags:
      - List
      - Listing
      - Market
      - History
  /rest/listings/markets/texts:
    get:
      summary: List listing market texts
      description: Lists listing market texts by filter options.
      operationId: getRestListingsMarketsTexts
      x-api-path-slug: restlistingsmarketstexts-get
      parameters:
      - in: query
        name: contains
        description: Filter that restricts the search result to listing market texts
          which title, subtitle or description contain the given value
      - in: query
        name: id
        description: Filter that restricts the search result to listing market texts
          with specific ID
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: language
        description: Filter that restricts the search result to listing market texts
          for a specific language
      - in: query
        name: listingMarketId
        description: Filter that restricts the search result to listing market texts
          with specific listing market IDs
      - in: query
        name: page
        description: The page of results to search for
      responses:
        200:
          description: OK
      tags:
      - List
      - Listing
      - Market
      - Texts
  /rest/listings/option_templates/preview:
    get:
      summary: Get a preview list of option templates
      description: Gets a preview list of all available listing option templates.
      operationId: getRestListingsOptionTemplatesPreview
      x-api-path-slug: restlistingsoption-templatespreview-get
      responses:
        200:
          description: OK
      tags:
      - Preview
      - List
      - Of
      - Option
      - Templates
  /rest/listings/shipping_profiles:
    get:
      summary: List listing shipping profiles
      description: Lists listing shipping profiles.
      operationId: getRestListingsShippingProfiles
      x-api-path-slug: restlistingsshipping-profiles-get
      parameters:
      - in: query
        name: credentialsId
        description: Filter that restricts the search result to listing shipping profiles
          with given credential ID(s)
      - in: query
        name: id
        description: Filter that restricts the search result to listing shipping profiles
          that match the given ID(s)
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: page
        description: The page of results to search for
      - in: query
        name: referrerId
        description: Filter that restricts the search result to listing shipping profiles
          with given referrer ID(s)
      responses:
        200:
          description: OK
      tags:
      - List
      - Listing
      - Shipping
      - Profiles
  /rest/listings/stock_dependence_types:
    get:
      summary: List listing stock dependence types
      description: Lists listing stock dependence types.
      operationId: getRestListingsStockDependenceTypes
      x-api-path-slug: restlistingsstock-dependence-types-get
      parameters:
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: page
        description: The page of results to search for
      - in: query
        name: with
        description: An array with child instances to be loaded
      responses:
        200:
          description: OK
      tags:
      - List
      - Listing
      - Stock
      - Dependence
      - Types
  /rest/listings/types:
    get:
      summary: List listing types
      description: Lists all listing types.
      operationId: getRestListingsTypes
      x-api-path-slug: restlistingstypes-get
      parameters:
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: page
        description: The page of results to search for
      responses:
        200:
          description: OK
      tags:
      - List
      - Listing
      - Types
  /rest/markets/credentials:
    get:
      summary: List credentials
      description: List credentials.
      operationId: getRestMarketsCredentials
      x-api-path-slug: restmarketscredentials-get
      parameters:
      - in: query
        name: itemsPerPage
        description: The items per page to search for
      - in: query
        name: page
        description: The page of results to search for
      responses:
        200:
          description: OK
      tags:
      - List
      - Credentials
  /rest/markets/ebay/categories:
    get:
      summary: List categories
      description: Lists categories. By passing category ID as filter, only subcategories
        of that category will be returned. The marketplace ID filter is required.
      operationId: getRestMarketsEbayCategories
      x-api-path-slug: restmarketsebaycategories-get
      parameters:
      - in: query
        name: categoryId
        description: Filter that restricts the search result to categories that belong
          to the specified category ID
      - in: query
        name: marketplaceId
        description: Filter that restricts the search result to categories that belong
          to the specified marketplace ID
      responses:
        200:
          description: OK
      tags:
      - List
      - Categories
  /rest/markets/ebay/item_specifics:
    get:
      summary: List item specifics
      description: List item specifics for a given category Id and referrerId.
      operationId: getRestMarketsEbayItemSpecifics
      x-api-path-slug: restmarketsebayitem-specifics-get
      parameters:
      - in: query
        name: categoryId
        description: The ID of the category for which to list item specifics
      - in: query
        name: marketplaceId
        description: Filter that restricts the search result to categories that belong
          to the specified marketplace ID
      responses:
        200:
          description: OK
      tags:
      - List
      - Item
      - Specifics
  /rest/markets/ebay/parts-fitments:
    get:
      summary: List fitments
      description: Lists fitments.
      operationId: getRestMarketsEbayPartsFitments
      x-api-path-slug: restmarketsebaypartsfitments-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Fitments
  /rest/markets/ebay/shop_categories:
    get:
      summary: List all eBay shop categories
      description: Lists all eBay shop categories.
      operationId: getRestMarketsEbayShopCategories
      x-api-path-slug: restmarketsebayshop-categories-get
      parameters:
      - in: query
        name: credentialsId
        description: The credentials ID for whom to fetch eBay shop categories
      - in: query
        name: viewType
        description: How should the eBay shop categories be returned
      responses:
        200:
          description: OK
      tags:
      - List
      - ""
      - EBay
      - Shop
      - Categories
  /rest/markets/settings:
    get:
      summary: List market settings
      description: Lists market settings. The marketplace ID and the type must be
        specified.
      operationId: getRestMarketsSettings
      x-api-path-slug: restmarketssettings-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Market
      - Settings
  /rest/markets/settings/correlations:
    get:
      summary: List correlation
      description: Lists correlations. The type, the market settings ID and the correlation
        ID must be specified.
      operationId: getRestMarketsSettingsCorrelations
      x-api-path-slug: restmarketssettingscorrelations-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Correlation
  /rest/newsletters:
    get:
      summary: List newsletter entries
      description: List newsletter entries.
      operationId: getRestNewsletters
      x-api-path-slug: restnewsletters-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Newsletter
      - Entries
  /rest/newsletters/folders:
    get:
      summary: List newsletter folders
      description: List newsletter folders.
      operationId: getRestNewslettersFolders
      x-api-path-slug: restnewslettersfolders-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Newsletter
      - Folders
  /rest/newsletters/folders/{folderId}:
    get:
      summary: List details of a folder
      description: Lists details of a folder. The ID of the folder must be specified.
      operationId: getRestNewslettersFoldersFolder
      x-api-path-slug: restnewslettersfoldersfolderid-get
      parameters:
      - in: path
        name: folderId
      responses:
        200:
          description: OK
      tags:
      - List
      - Details
      - Of
      - Folder
  /rest/newsletters/folders/{folderId}/recipients:
    get:
      summary: List all recipients of a folder
      description: Lists all recipients of a folder. The ID of the folder must be
        specified.
      operationId: getRestNewslettersFoldersFolderRecipients
      x-api-path-slug: restnewslettersfoldersfolderidrecipients-get
      parameters:
      - in: path
        name: folderId
      responses:
        200:
          description: OK
      tags:
      - List
      - ""
      - Recipients
      - Of
      - Folder
  /rest/newsletters/list_recipients:
    get:
      summary: List recipients
      description: List recipients.
      operationId: getRestNewslettersListRecipients
      x-api-path-slug: restnewsletterslist-recipients-get
      parameters:
      - in: query
        name: columns
        description: Filter that restricts the search result to specific columns
      - in: query
        name: folderId
        description: Filter that restricts the search result to a specific folderId
      - in: query
        name: isConfirmed
        description: Filter that restricts the search result to confirmed recipients
      - in: query
        name: itemsPerPage
        description: The number of orders to be displayed per page
      - in: query
        name: page
        description: The page to get
      - in: query
        name: with
        description: Load additional relations for a Recipient
      responses:
        200:
          description: OK
      tags:
      - List
      - Recipients
  /rest/newsletters/recipients:
    get:
      summary: List recipients of a folder
      description: List recipients of a folder.
      operationId: getRestNewslettersRecipients
      x-api-path-slug: restnewslettersrecipients-get
      parameters:
      - in: query
        name: email
        description: Filter that restricts the search result to the email address
          of the recipient
      - in: query
        name: folderId
        description: Filter that restricts the search result to the folder ID
      - in: query
        name: recipientId
        description: Filter that restricts the search result to the recipient ID
      responses:
        200:
          description: OK
      tags:
      - List
      - Recipients
      - Of
      - Folder
  /rest/newsletters/recipients/{recipientId}:
    get:
      summary: List a recipient
      description: Lists a recipient. The ID of the recipient must be specified.
      operationId: getRestNewslettersRecipientsRecipient
      x-api-path-slug: restnewslettersrecipientsrecipientid-get
      parameters:
      - in: path
        name: recipientId
      - in: query
        name: recipientsId
        description: The ID of the newsletter folder
      responses:
        200:
          description: OK
      tags:
      - List
      - Recipient
  /rest/newsletters/{entryId}:
    get:
      summary: List details of an entry
      description: Lists details of an entry. The ID of the entry must be specified.
      operationId: getRestNewslettersEntry
      x-api-path-slug: restnewslettersentryid-get
      parameters:
      - in: path
        name: entryId
      responses:
        200:
          description: OK
      tags:
      - List
      - Details
      - Of
      - Entry
  /rest/orders:
    get:
      summary: List orders by filter options
      description: List orders by filter options.
      operationId: getRestOrders
      x-api-path-slug: restorders-get
      parameters:
      - in: query
        name: clientId
        description: Filter that restricts the search result to order from one client
      - in: query
        name: contactId
        description: Filter that restricts the search result to orders of one order
          contact
      - in: query
        name: createdAtFrom
        description: Filter that restricts the search result to orders that were created
          on the specified date
      - in: query
        name: createdAtTo
        description: Filter that restricts the search result to orders that were created
          within a certain period of time
      - in: query
        name: externalOrderId
        description: Filter that restricts the search result to an external order
          id
      - in: query
        name: hasDocument
        description: Filter that restricts the search result to orders which hold
          the given document type
      - in: query
        name: includedItem
        description: Filter that restricts the search result to orders with a certain
          item
      - in: query
        name: includedVariation
        description: Filter that restricts the search result to orders with a certain
          variation
      - in: query
        name: isEbayPlus
        description: Filter that restricts the search result to orders with ebay plus
      - in: query
        name: itemsPerPage
        description: The number of orders to be displayed per page
      - in: query
        name: orderIds
        description: Filter that restricts the search result to orders
      - in: query
        name: orderType
        description: Filter that restricts the search result to orders of specific
          order types
      - in: query
        name: outgoingItemsBookedAtFrom
        description: Filter that restricts the search result to orders where the outgoing
          items were booked on the specified date
      - in: query
        name: outgoingItemsBookedAtTo
        description: Filter that restricts the search result to orders where the outgoing
          items were booked within a specified period of time
      - in: query
        name: ownerUserId
        description: Filter that restricts the search result to orders of one owner
      - in: query
        name: page
        description: The page to get
      - in: query
        name: paidAtFrom
        description: Filter that restricts the search result to orders that received
          a payment on the specified date
      - in: query
        name: paidAtTo
        description: Filter that restricts the search result to orders that received
          a payment within a certain period of time
      - in: query
        name: paymentStatus
        description: Filter that restricts the search result to order with a specific
          payment status
      - in: query
        name: referrerId
        description: Filter that restricts the search result to orders from one order
          referrer
      - in: query
        name: shippingProfileId
        description: Filter that restricts the search result to orders with a specific
          shipping profile
      - in: query
        name: statusFrom
        description: Filter that restricts the search result to orders in a specific
          order status
      - in: query
        name: statusTo
        description: Filter that restricts the search result to orders within a range
          of order statuses
      - in: query
        name: supplierId
        description: Filter that restricts the search result to orders that include
          order items with variations from a supplier
      - in: query
        name: updatedAtFrom
        description: Filter that restricts the search result to orders that were last
          updated on the specified date
      - in: query
        name: updatedAtTo
        description: Filter that restricts the search result to orders that were last
          updated within a specified period of time
      - in: query
        name: warehouseId
        description: Filter that restricts the search result to orders with a specific
          main warehouse
      - in: query
        name: with
        description: Load additional relations for an order
      responses:
        200:
          description: OK
      tags:
      - List
      - Orders
      - By
      - Filter
      - Options
  /rest/orders/contacts/{contactId}:
    get:
      summary: List orders of a contact
      description: Lists all orders of a contact. The ID of the contact must be specified.
      operationId: getRestOrdersContactsContact
      x-api-path-slug: restorderscontactscontactid-get
      parameters:
      - in: path
        name: contactId
      - in: query
        name: itemsPerPage
        description: The number of orders to be displayed per page
      - in: query
        name: page
        description: The page to get
      - in: query
        name: with
        description: Load additional relations for an order
      responses:
        200:
          description: OK
      tags:
      - List
      - Orders
      - Of
      - Contact
  /rest/orders/coupons/codes/contacts/{contactId}:
    get:
      summary: List redeemed coupon codes of a contact
      description: Lists the redeemed coupon codes of contact. The ID of the contact
        must be specified.
      operationId: getRestOrdersCouponsCodesContactsContact
      x-api-path-slug: restorderscouponscodescontactscontactid-get
      parameters:
      - in: path
        name: contactId
      - in: query
        name: itemsPerPage
        description: The number of coupons to be displayed per page
      - in: query
        name: page
        description: The page to get
      responses:
        200:
          description: OK
      tags:
      - List
      - Redeemed
      - Coupon
      - Codes
      - Of
      - Contact
  /rest/orders/currencies:
    get:
      summary: List currencies
      description: List currencies.
      operationId: getRestOrdersCurrencies
      x-api-path-slug: restorderscurrencies-get
      parameters:
      - in: query
        name: columns
        description: The attributes to be loaded
      - in: query
        name: with
        description: The relations to be loaded
      responses:
        200:
          description: OK
      tags:
      - List
      - Currencies
  /rest/orders/currencies/{currencyIso}/countries:
    get:
      summary: List countries for a currency
      description: List countries for a currency. The ISO 4271 code of the currency
        must be specified.
      operationId: getRestOrdersCurrenciesCurrencyisoCountries
      x-api-path-slug: restorderscurrenciescurrencyisocountries-get
      parameters:
      - in: query
        name: columns
        description: The attributes to be loaded
      - in: path
        name: currencyIso
      responses:
        200:
          description: OK
      tags:
      - List
      - Countriesa
      - Currency
  /rest/orders/dates/types:
    get:
      summary: List order date types
      description: List order date types.
      operationId: getRestOrdersDatesTypes
      x-api-path-slug: restordersdatestypes-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Order
      - Date
      - Types
  /rest/orders/dates/types/{typeId}/names:
    get:
      summary: List names of an order date type
      description: Lists names in all languages available of an order date type. The
        ID of the date type must be specified.
      operationId: getRestOrdersDatesTypesTypeNames
      x-api-path-slug: restordersdatestypestypeidnames-get
      parameters:
      - in: path
        name: typeId
      responses:
        200:
          description: OK
      tags:
      - List
      - Names
      - Of
      - Order
      - Date
      - Type
  /rest/orders/documents/accounting_summary:
    get:
      summary: List document accounting summaries
      description: Lists document accounting summaries. A document accounting summary
        is saved along with each reversal document (for invoice and credit note).
        It contains accounting information about the order for this point in time.
        The summary is saved because an order can be updated after a reversal_document
        is generated. The information about the order before the update is needed
        for accounting.
      operationId: getRestOrdersDocumentsAccountingSummary
      x-api-path-slug: restordersdocumentsaccounting-summary-get
      parameters:
      - in: query
        name: createdAtFrom
        description: Get entries with createdAt date after this date
      - in: query
        name: createdAtTo
        description: Get entries with createdAt date before this date
      - in: query
        name: documentType
        description: The document type
      - in: query
        name: itemsPerPage
        description: The number of summaries to be displayed per page
      - in: query
        name: orderId
        description: The ID of the order
      - in: query
        name: page
        description: The page to get
      responses:
        200:
          description: OK
      tags:
      - List
      - Document
      - Accounting
      - Summaries
  /rest/orders/documents/{type}:
    get:
      summary: List documents of a type
      description: Lists documents of a type. The type must be specified.
      operationId: getRestOrdersDocumentsType
      x-api-path-slug: restordersdocumentstype-get
      parameters:
      - in: query
        name: createdAtFrom
        description: Filter that restricts the search result to documents that were
          created on the specified date
      - in: query
        name: createdAtTo
        description: Filter that restricts the search result to documents that were
          created within a certain period of time
      - in: query
        name: displayDateFrom
        description: Filter that restricts the search result to documents that were
          displayed on the specified date
      - in: query
        name: displayDateTo
        description: Filter that restricts the search result to documents that were
          displayed within a certain period of time
      - in: query
        name: itemsPerPage
        description: The items per page to search for
      - in: query
        name: page
        description: The page of results to search for
      - in: path
        name: type
      - in: query
        name: with
        description: Load additional relations for a document
      - in: query
        name: withContent
        description: Load also the document content as base64 encoded string
      responses:
        200:
          description: OK
      tags:
      - List
      - Documents
      - Of
      - Type
  /rest/orders/items/{orderItemId}/dates:
    get:
      summary: List dates of an order item
      description: Lists the dates of an order item. The ID of the order item must
        be specified.
      operationId: getRestOrdersItemsOrderitemDates
      x-api-path-slug: restordersitemsorderitemiddates-get
      parameters:
      - in: path
        name: orderItemId
      responses:
        200:
          description: OK
      tags:
      - List
      - Dates
      - Of
      - Order
      - Item
  /rest/orders/items/{orderItemId}/transactions:
    get:
      summary: List transactions
      description: Lists transactions for an order item. The ID of the order item
        must be specified.
      operationId: getRestOrdersItemsOrderitemTransactions
      x-api-path-slug: restordersitemsorderitemidtransactions-get
      parameters:
      - in: query
        name: columns
        description: The properties to be loaded
      - in: path
        name: orderItemId
      - in: query
        name: with
        description: Load additional relations for a transaction
      responses:
        200:
          description: OK
      tags:
      - List
      - Transactions
  /rest/orders/properties/types:
    get:
      summary: List order property types
      description: Lists property types and their names in all languages. Optionally
        one or more languages can be specified to get a limited response.
      operationId: getRestOrdersPropertiesTypes
      x-api-path-slug: restorderspropertiestypes-get
      parameters:
      - in: query
        name: lang
        description: Languages to be loaded with the type model
      responses:
        200:
          description: OK
      tags:
      - List
      - Order
      - Property
      - Types
  /rest/orders/referrers:
    get:
      summary: List referrers
      description: Lists referrers with the desired columns/attributes.
      operationId: getRestOrdersReferrers
      x-api-path-slug: restordersreferrers-get
      parameters:
      - in: query
        name: columns
        description: The desired columns/attributes of the order referrer to be loaded
      responses:
        200:
          description: OK
      tags:
      - List
      - Referrers
  /rest/orders/shipping/countries:
    get:
      summary: List shipping countries
      description: List shipping countries.
      operationId: getRestOrdersShippingCountries
      x-api-path-slug: restordersshippingcountries-get
      parameters:
      - in: query
        name: active
        description: Returns only the active shipping countries
      - in: query
        name: with
        description: The relations to be loaded
      responses:
        200:
          description: OK
      tags:
      - List
      - Shipping
      - Countries
  /rest/orders/shipping/export_documents/{orderId}:
    get:
      summary: List export documents by order ID
      description: List export documents by order id.
      operationId: getRestOrdersShippingExportDocumentsOrder
      x-api-path-slug: restordersshippingexport-documentsorderid-get
      parameters:
      - in: path
        name: orderId
      responses:
        200:
          description: OK
      tags:
      - List
      - Export
      - Documents
      - By
      - Order
      - ID
  /rest/orders/shipping/package_types:
    get:
      summary: List shipping package types
      description: List shipping package types.
      operationId: getRestOrdersShippingPackageTypes
      x-api-path-slug: restordersshippingpackage-types-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Shipping
      - Package
      - Types
  /rest/orders/shipping/presets:
    get:
      summary: List shipping profiles
      description: List shipping profiles.
      operationId: getRestOrdersShippingPresets
      x-api-path-slug: restordersshippingpresets-get
      parameters:
      - in: query
        name: columns
        description: The attributes to be loaded in the shipping profile
      - in: query
        name: parcelServiceName
        description: Filter that restricts the search result to parcel service presets
          with a specified service name (e
      - in: query
        name: shippingServiceProvider
        description: Filter that restricts the search result to a shipping service
          provider
      - in: query
        name: updatedAtAfter
        description: Filter that restricts the search result to presets that were
          updated after a specific date
      - in: query
        name: updatedAtBefore
        description: Filter that restricts the search result to presets that were
          updated before a specific date
      - in: query
        name: with
        description: The name of an relation to the preset
      responses:
        200:
          description: OK
      tags:
      - List
      - Shipping
      - Profiles
  /rest/orders/shipping/returns/returns_service_providers/plugins:
    get:
      summary: List shipping service provider plugins
      description: List shipping service provider plugins.
      operationId: getRestOrdersShippingReturnsReturnsServiceProversPlugins
      x-api-path-slug: restordersshippingreturnsreturns-service-providersplugins-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Shipping
      - Service
      - Provider
      - Plugins
  /rest/orders/shipping/shipping_service_providers:
    get:
      summary: List shipping service providers
      description: List shipping service providers.
      operationId: getRestOrdersShippingShippingServiceProvers
      x-api-path-slug: restordersshippingshipping-service-providers-get
      parameters:
      - in: query
        name: updatedAtAfter
        description: Filter that restricts the search result to shipping providers
          that were updated after a specific date
      - in: query
        name: updatedAtBefore
        description: Filter that restricts the search result to shipping providers
          that were updated before a specific date
      - in: query
        name: with
        description: The name of an relation to the shipping provider
      responses:
        200:
          description: OK
      tags:
      - List
      - Shipping
      - Service
      - Providers
  /rest/orders/shipping/shipping_service_providers/plugins:
    get:
      summary: List shipping service provider plugins
      description: List shipping service provider plugins.
      operationId: getRestOrdersShippingShippingServiceProversPlugins
      x-api-path-slug: restordersshippingshipping-service-providersplugins-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Shipping
      - Service
      - Provider
      - Plugins
  /rest/orders/status-history:
    get:
      summary: List status histories of orders
      description: Lists the status histories of all orders. The result can be limited
        to an order, a status type, a period of time or a user.
      operationId: getRestOrdersStatusHistory
      x-api-path-slug: restordersstatushistory-get
      parameters:
      - in: query
        name: createdAtFrom
        description: Get entries with createdAt date after this date
      - in: query
        name: createdAtTo
        description: Get entries with createdAt date before this date
      - in: query
        name: orderId
        description: The ID of the order
      - in: query
        name: statusId
        description: The ID of the status
      - in: query
        name: userId
        description: The ID of the user
      responses:
        200:
          description: OK
      tags:
      - List
      - Status
      - Histories
      - Of
      - Orders
  /rest/orders/{orderId}/addresses/{relationTypeId?}:
    get:
      summary: List order addresses
      description: Lists order addresses. The ID of the order must be specified.
      operationId: getRestOrdersOrderAddressesRelationtype
      x-api-path-slug: restordersorderidaddressesrelationtypeid-get
      parameters:
      - in: path
        name: orderId
      - in: path
        name: relationTypeId?
      responses:
        200:
          description: OK
      tags:
      - List
      - Order
      - Addresses
  /rest/orders/{orderId}/dates:
    get:
      summary: List dates of an order
      description: Lists dates of an order. The ID of the order must be specified.
      operationId: getRestOrdersOrderDates
      x-api-path-slug: restordersorderiddates-get
      parameters:
      - in: path
        name: orderId
      responses:
        200:
          description: OK
      tags:
      - List
      - Dates
      - Of
      - Order
  /rest/orders/{orderId}/documents/{type?}:
    get:
      summary: List documents of an order
      description: Lists documents of an order. The ID of the order must be specified.
        In addition a type can be specified.
      operationId: getRestOrdersOrderDocumentsType
      x-api-path-slug: restordersorderiddocumentstype-get
      parameters:
      - in: query
        name: createdAtFrom
        description: Filter that restricts the search result to documents that were
          created on the specified date
      - in: query
        name: createdAtTo
        description: Filter that restricts the search result to documents that were
          created within a certain period of time
      - in: query
        name: displayDateFrom
        description: Filter that restricts the search result to documents that were
          displayed on the specified date
      - in: query
        name: displayDateTo
        description: Filter that restricts the search result to documents that were
          displayed within a certain period of time
      - in: path
        name: orderId
      - in: query
        name: type
        description: The type of the order documents
      - in: path
        name: type?
      - in: query
        name: with
        description: Load additional relations for a document
      - in: query
        name: withContent
        description: Load also the document content as base64 encoded string
      responses:
        200:
          description: OK
      tags:
      - List
      - Documents
      - Of
      - Order
  /rest/orders/{orderId}/items/serialNumbers:
    get:
      summary: List serial numbers of an order
      description: Lists all serial numbers of an order. The ID of the order must
        be specified.
      operationId: getRestOrdersOrderItemsSerialnumbers
      x-api-path-slug: restordersorderiditemsserialnumbers-get
      parameters:
      - in: path
        name: orderId
      responses:
        200:
          description: OK
      tags:
      - List
      - Serial
      - Numbers
      - Of
      - Order
  /rest/orders/{orderId}/items/{orderItemId}/serialNumbers:
    get:
      summary: List serial numbers of an order item
      description: Lists all serial numbers of an order item. The ID of the order
        and the ID of the order item must be specified.
      operationId: getRestOrdersOrderItemsOrderitemSerialnumbers
      x-api-path-slug: restordersorderiditemsorderitemidserialnumbers-get
      parameters:
      - in: path
        name: orderId
      - in: path
        name: orderItemId
      responses:
        200:
          description: OK
      tags:
      - List
      - Serial
      - Numbers
      - Of
      - Order
      - Item
  /rest/orders/{orderId}/packagenumbers:
    get:
      summary: List package numbers of an order
      description: Lists the package numbers of an order. The ID of the order must
        be specified.
      operationId: getRestOrdersOrderPackagenumbers
      x-api-path-slug: restordersorderidpackagenumbers-get
      parameters:
      - in: path
        name: orderId
      responses:
        200:
          description: OK
      tags:
      - List
      - Package
      - Numbers
      - Of
      - Order
  /rest/orders/{orderId}/properties/{typeId?}:
    get:
      summary: List properties of an order
      description: Lists properties of an order. The ID of the order must be specified.
      operationId: getRestOrdersOrderPropertiesType
      x-api-path-slug: restordersorderidpropertiestypeid-get
      parameters:
      - in: path
        name: orderId
      - in: query
        name: typeId
        description: The property type ID
      - in: path
        name: typeId?
      responses:
        200:
          description: OK
      tags:
      - List
      - Properties
      - Of
      - Order
  /rest/orders/{orderId}/shipping/packages:
    get:
      summary: List order shipping packages
      description: Lists order shipping packages. The ID of the order must be specified.
      operationId: getRestOrdersOrderShippingPackages
      x-api-path-slug: restordersorderidshippingpackages-get
      parameters:
      - in: query
        name: columns
        description: The properties to be loaded
      - in: path
        name: orderId
      - in: query
        name: with
        description: Possible value is labelBase64
      responses:
        200:
          description: OK
      tags:
      - List
      - Order
      - Shipping
      - Packages
  /rest/payment/properties/types/names/{lang?}:
    get:
      summary: List names of property types
      description: List names of property types.
      operationId: getRestPaymentPropertiesTypesNamesLang
      x-api-path-slug: restpaymentpropertiestypesnameslang-get
      parameters:
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: path
        name: lang?
      - in: query
        name: page
        description: The page of results to search for
      responses:
        200:
          description: OK
      tags:
      - List
      - Names
      - Of
      - Property
      - Types
  /rest/payments:
    get:
      summary: List payments
      description: List payments.
      operationId: getRestPayments
      x-api-path-slug: restpayments-get
      parameters:
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: page
        description: The page of results to search for
      responses:
        200:
          description: OK
      tags:
      - List
      - Payments
  /rest/payments/entrydate:
    get:
      summary: List payments by entry date
      description: Lists all payments by entry date within a certain date range. The
        start and the end of the date range must be specified.
      operationId: getRestPaymentsEntrydate
      x-api-path-slug: restpaymentsentrydate-get
      parameters:
      - in: query
        name: endDate
        description: The end date of the date range for the entry date of the payment
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: page
        description: The page of results to search for
      - in: query
        name: startDate
        description: The start date of the date range for the entry date of the payment
      responses:
        200:
          description: OK
      tags:
      - List
      - Payments
      - By
      - Entry
      - Date
  /rest/payments/importdate:
    get:
      summary: List payments by import date
      description: Lists all payments by import date within a certain date range.
        The start and the end of the date range must be specified.
      operationId: getRestPaymentsImportdate
      x-api-path-slug: restpaymentsimportdate-get
      parameters:
      - in: query
        name: endDate
        description: The end date of the date range for the import date of the payment
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: page
        description: The page of results to search for
      - in: query
        name: startDate
        description: The start date of the date range for the import date of the payment
      responses:
        200:
          description: OK
      tags:
      - List
      - Payments
      - By
      - Import
      - Date
  /rest/payments/methodNames:
    get:
      summary: List payment methods names
      description: Lists all payment method names.
      operationId: getRestPaymentsMethodnames
      x-api-path-slug: restpaymentsmethodnames-get
      parameters:
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: page
        description: The page of results to search for
      responses:
        200:
          description: OK
      tags:
      - List
      - Payment
      - Methods
      - Names
  /rest/payments/methodNames/{paymentMethodId}:
    get:
      summary: List all payment method names for a payment method id
      description: List all payment method names for a payment method id. The payment
        method id must be specified.
      operationId: getRestPaymentsMethodnamesPaymentmethod
      x-api-path-slug: restpaymentsmethodnamespaymentmethodid-get
      parameters:
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: page
        description: The page of results to search for
      - in: path
        name: paymentMethodId
      responses:
        200:
          description: OK
      tags:
      - List
      - ""
      - Payment
      - Method
      - Namesa
      - Payment
      - Method
      - Id
  /rest/payments/methods:
    get:
      summary: List payment methods
      description: Lists all payment method plugins.
      operationId: getRestPaymentsMethods
      x-api-path-slug: restpaymentsmethods-get
      parameters:
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: page
        description: The page of results to search for
      responses:
        200:
          description: OK
      tags:
      - List
      - Payment
      - Methods
  /rest/payments/methods/{methodId}:
    get:
      summary: List payments of a payment method
      description: Lists all payments of the a payment method. The ID of the payment
        method must be specified.
      operationId: getRestPaymentsMethodsMethod
      x-api-path-slug: restpaymentsmethodsmethodid-get
      parameters:
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: path
        name: methodId
      - in: query
        name: page
        description: The page of results to search for
      responses:
        200:
          description: OK
      tags:
      - List
      - Payments
      - Of
      - Payment
      - Method
  /rest/payments/orders/{orderId}:
    get:
      summary: List payments of an order
      description: Lists all payments of an order. The ID of the order must be specified.
      operationId: getRestPaymentsOrdersOrder
      x-api-path-slug: restpaymentsordersorderid-get
      parameters:
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: path
        name: orderId
      - in: query
        name: page
        description: The page of results to search for
      responses:
        200:
          description: OK
      tags:
      - List
      - Payments
      - Of
      - Order
  /rest/payments/properties:
    get:
      summary: List properties
      description: List properties.
      operationId: getRestPaymentsProperties
      x-api-path-slug: restpaymentsproperties-get
      parameters:
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: page
        description: The page of results to search for
      responses:
        200:
          description: OK
      tags:
      - List
      - Properties
  /rest/payments/properties/date:
    get:
      summary: List properties by creation date
      description: Lists all properties by creation date. The start and the end of
        the date range must be specified.
      operationId: getRestPaymentsPropertiesDate
      x-api-path-slug: restpaymentspropertiesdate-get
      parameters:
      - in: query
        name: endDate
        description: The end date of the date range for the date of creation of the
          property
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: page
        description: The page of results to search for
      - in: query
        name: startDate
        description: The start date of the date range for the date of creation of
          the property
      responses:
        200:
          description: OK
      tags:
      - List
      - Properties
      - By
      - Creation
      - Date
  /rest/payments/properties/types:
    get:
      summary: List property types
      description: Lists all property types. The language must be specified.
      operationId: getRestPaymentsPropertiesTypes
      x-api-path-slug: restpaymentspropertiestypes-get
      parameters:
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: page
        description: The page of results to search for
      responses:
        200:
          description: OK
      tags:
      - List
      - Property
      - Types
  /rest/payments/property/{propertyTypeId}/{propertyValue}:
    get:
      summary: List payments by property type ID and value
      description: Lists all payments by the given property type ID and the value.
      operationId: getRestPaymentsPropertyPropertytypePropertyvalue
      x-api-path-slug: restpaymentspropertypropertytypeidpropertyvalue-get
      parameters:
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: page
        description: The page of results to search for
      - in: path
        name: propertyTypeId
      - in: path
        name: propertyValue
      responses:
        200:
          description: OK
      tags:
      - List
      - Payments
      - By
      - Property
      - Type
      - ID
      - Value
  /rest/payments/status/{statusId}:
    get:
      summary: List payments of a payment status
      description: Lists all payments of a payment status. The ID of the <a href='https://developers.plentymarkets.com/rest-doc/introduction#payment-statuses'  target='_blank'>payment
        status</a> must be specified.
      operationId: getRestPaymentsStatusStatus
      x-api-path-slug: restpaymentsstatusstatusid-get
      parameters:
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: page
        description: The page of results to search for
      - in: path
        name: statusId
      responses:
        200:
          description: OK
      tags:
      - List
      - Payments
      - Of
      - Payment
      - Status
  /rest/payments/transactions/{transactionTypeId}:
    get:
      summary: List payments of a transaction type
      description: Lists all payments of a transaction type. The ID of the transaction
        type must be specified.
      operationId: getRestPaymentsTransactionsTransactiontype
      x-api-path-slug: restpaymentstransactionstransactiontypeid-get
      parameters:
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: page
        description: The page of results to search for
      - in: path
        name: transactionTypeId
      responses:
        200:
          description: OK
      tags:
      - List
      - Payments
      - Of
      - Transaction
      - Type
  /rest/payments/{paymentId}/properties:
    get:
      summary: List properties for a payment
      description: Lists all properties for a payment. The ID of the payment must
        be specified.
      operationId: getRestPaymentsPaymentProperties
      x-api-path-slug: restpaymentspaymentidproperties-get
      parameters:
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: page
        description: The page of results to search for
      - in: path
        name: paymentId
      responses:
        200:
          description: OK
      tags:
      - List
      - Propertiesa
      - Payment
  /rest/plugin_sets:
    get:
      summary: List all Sets
      description: Lists all available sets.
      operationId: getRestPluginSets
      x-api-path-slug: restplugin-sets-get
      responses:
        200:
          description: OK
      tags:
      - List
      - ""
      - Sets
  /rest/plugin_sets/{pluginSetId}/languages:
    get:
      summary: List all the plugins translations for a plugin set
      description: Lists all the plugins translations for a plugin set
      operationId: getRestPluginSetsPluginsetLanguages
      x-api-path-slug: restplugin-setspluginsetidlanguages-get
      parameters:
      - in: query
        name: $pluginSetId
        description: The ID of the plugin set
      - in: path
        name: pluginSetId
      responses:
        200:
          description: OK
      tags:
      - List
      - ""
      - Plugins
      - Translationsa
      - Plugin
      - Set
  /rest/plugin_sets/{setId}/plugins:
    get:
      summary: List all Plugins of Set
      description: Lists all active Plugins of given Set.
      operationId: getRestPluginSetsSetPlugins
      x-api-path-slug: restplugin-setssetidplugins-get
      parameters:
      - in: query
        name: includeStage
        description: Include staged plugins in the result
      - in: path
        name: setId
      responses:
        200:
          description: OK
      tags:
      - List
      - ""
      - Plugins
      - Of
      - Set
  /rest/plugin_sets/{setId}/set_entries:
    get:
      summary: List all SetEntries of Set
      description: List all setentries of set.
      operationId: getRestPluginSetsSetSetEntries
      x-api-path-slug: restplugin-setssetidset-entries-get
      parameters:
      - in: path
        name: setId
      responses:
        200:
          description: OK
      tags:
      - List
      - ""
      - SetEntries
      - Of
      - Set
  /rest/plugins:
    get:
      summary: List plugins
      description: |-
        Lists all plugins saved in the inbox folder. Plugins that have not been provisioned to Stage or Productive will
        also be shown.
      operationId: getRestPlugins
      x-api-path-slug: restplugins-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Plugins
  /rest/plugins/plugin_sets/{pluginSetId}/plugins:
    get:
      summary: List all Plugins of Set
      description: Lists all active Plugins of given Set.
      operationId: getRestPluginsPluginSetsPluginsetPlugins
      x-api-path-slug: restpluginsplugin-setspluginsetidplugins-get
      parameters:
      - in: query
        name: includeStage
        description: Include staged plugins in the result
      - in: path
        name: pluginSetId
      responses:
        200:
          description: OK
      tags:
      - List
      - ""
      - Plugins
      - Of
      - Set
  /rest/plugins/search:
    get:
      summary: List plugins
      description: |-
        Lists all plugins saved in the inbox folder. Plugins that have not been provisioned to Stage or Productive will
        also be shown.
      operationId: getRestPluginsSearch
      x-api-path-slug: restpluginssearch-get
      parameters:
      - in: query
        name: itemsPerPage
        description: The number of items to list per page
      - in: query
        name: name
        description: The name of the plugin
      - in: query
        name: page
        description: The page of results to search for
      - in: query
        name: type
        description: The type of the plugin (template, theme, etc
      - in: query
        name: webstoreId
        description: The ID of the client (store)
      responses:
        200:
          description: OK
      tags:
      - List
      - Plugins
  /rest/plugins/ui:
    get:
      summary: List plugins for backend UI
      description: Lists all plugins provisioned in Stage or Productive that contain
        a plugin.js file.
      operationId: getRestPluginsUi
      x-api-path-slug: restpluginsui-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Pluginsbackend
      - UI
  /rest/properties:
    get:
      summary: List properties
      description: Lists properties.
      operationId: getRestProperties
      x-api-path-slug: restproperties-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Properties
  /rest/properties/availabilities:
    get:
      summary: List availabilities
      description: Lists availabilities.
      operationId: getRestPropertiesAvailabilities
      x-api-path-slug: restpropertiesavailabilities-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Availabilities
  /rest/properties/groups:
    get:
      summary: List property groups
      description: Lists property groups.
      operationId: getRestPropertiesGroups
      x-api-path-slug: restpropertiesgroups-get
      parameters:
      - in: query
        name: groupId
        description: The ID of the group
      responses:
        200:
          description: OK
      tags:
      - List
      - Property
      - Groups
  /rest/properties/groups/names:
    get:
      summary: List group names
      description: Lists group names.
      operationId: getRestPropertiesGroupsNames
      x-api-path-slug: restpropertiesgroupsnames-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Group
      - Names
  /rest/properties/groups/options:
    get:
      summary: List group options
      description: Lists group options.
      operationId: getRestPropertiesGroupsOptions
      x-api-path-slug: restpropertiesgroupsoptions-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Group
      - Options
  /rest/properties/markets:
    get:
      summary: List property markets
      description: Lists property markets
      operationId: getRestPropertiesMarkets
      x-api-path-slug: restpropertiesmarkets-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Property
      - Markets
  /rest/properties/names:
    get:
      summary: List names
      description: Lists names.
      operationId: getRestPropertiesNames
      x-api-path-slug: restpropertiesnames-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Names
  /rest/properties/options:
    get:
      summary: List property options
      description: Lists property options.
      operationId: getRestPropertiesOptions
      x-api-path-slug: restpropertiesoptions-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Property
      - Options
  /rest/properties/relations:
    get:
      summary: List property relations
      description: Lists property relations.
      operationId: getRestPropertiesRelations
      x-api-path-slug: restpropertiesrelations-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Property
      - Relations
  /rest/properties/relations/markups:
    get:
      summary: List relation markups
      description: Lists relation markups.
      operationId: getRestPropertiesRelationsMarkups
      x-api-path-slug: restpropertiesrelationsmarkups-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Relation
      - Markups
  /rest/properties/relations/values:
    get:
      summary: List property relation values
      description: Lists property relation values.
      operationId: getRestPropertiesRelationsValues
      x-api-path-slug: restpropertiesrelationsvalues-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Property
      - Relation
      - Values
  /rest/properties/selections:
    get:
      summary: List property selections
      description: Lists property selections
      operationId: getRestPropertiesSelections
      x-api-path-slug: restpropertiesselections-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Property
      - Selections
  /rest/shop_builder/content_links:
    get:
      summary: List all content links for a given plugin set
      description: List all content links for a given plugin set.
      operationId: getRestShopBuilderContentLinks
      x-api-path-slug: restshop-buildercontent-links-get
      responses:
        200:
          description: OK
      tags:
      - List
      - ""
      - Content
      - Linksa
      - Given
      - Plugin
      - Set
  /rest/shop_builder/contents:
    get:
      summary: List all contents.
      description: List all contents..
      operationId: getRestShopBuilderContents
      x-api-path-slug: restshop-buildercontents-get
      responses:
        200:
          description: OK
      tags:
      - List
      - ""
      - Contents
  /rest/shop_builder/pages:
    get:
      summary: List content pages from all plugins in a given plugin set.
      description: List content pages from all plugins in a given plugin set..
      operationId: getRestShopBuilderPages
      x-api-path-slug: restshop-builderpages-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Content
      - Pages
      - From
      - ""
      - Plugins
      - In
      - Given
      - Plugin
      - Set
  /rest/shop_builder/widgets:
    get:
      summary: List all widgets provided by all frontend plugins of a given plugin
        set.
      description: List all widgets provided by all frontend plugins of a given plugin
        set..
      operationId: getRestShopBuilderWgets
      x-api-path-slug: restshop-builderwidgets-get
      parameters:
      - in: query
        name: identifier
        description: Filter results by widget identifier
      responses:
        200:
          description: OK
      tags:
      - List
      - ""
      - Widgets
      - Provided
      - By
      - ""
      - Frontend
      - Plugins
      - Of
      - Given
      - Plugin
      - Set
  /rest/stockmanagement/stock:
    get:
      summary: List stock
      description: Lists stock of all warehouses.
      operationId: getRestStockmanagementStock
      x-api-path-slug: reststockmanagementstock-get
      parameters:
      - in: query
        name: columns
        description: The properties to be loaded
      - in: query
        name: itemsPerPage
        description: The number of items per page
      - in: query
        name: page
        description: The requested page
      - in: query
        name: updatedAtFrom
        description: Filter that restricts the search result to stock that were last
          updated on the specified date
      - in: query
        name: updatedAtTo
        description: Filter that restricts the search result to stock that were last
          updated within a specified period of time
      - in: query
        name: variationId
        description: Filter that restricts the search result to stock with a variation
      responses:
        200:
          description: OK
      tags:
      - List
      - Stock
  /rest/stockmanagement/stock/types/{type}:
    get:
      summary: List stock by warehouse type
      description: Lists stock for all warehouses of the same warehouse type. The
        name of the type must be specified. Currently the only type available is 'sales'.
      operationId: getRestStockmanagementStockTypesType
      x-api-path-slug: reststockmanagementstocktypestype-get
      parameters:
      - in: query
        name: columns
        description: The properties to be loaded
      - in: query
        name: itemsPerPage
        description: The number of items per page
      - in: query
        name: page
        description: The requested page
      - in: path
        name: type
      - in: query
        name: updatedAtFrom
        description: Filter that restricts the search result to stock that were last
          updated on the specified date
      - in: query
        name: updatedAtTo
        description: Filter that restricts the search result to stock that were last
          updated within a specified period of time
      - in: query
        name: variationId
        description: Filter that restricts the search result to stock with a variation
      responses:
        200:
          description: OK
      tags:
      - List
      - Stock
      - By
      - Warehouse
      - Type
  /rest/stockmanagement/warehouses:
    get:
      summary: List warehouses
      description: Lists warehouses without applying any filters.
      operationId: getRestStockmanagementWarehouses
      x-api-path-slug: reststockmanagementwarehouses-get
      parameters:
      - in: query
        name: with
        description: Related objects to be loaded
      responses:
        200:
          description: OK
      tags:
      - List
      - Warehouses
  /rest/stockmanagement/warehouses/{warehouseId}/addresses/{relationTypeId?}:
    get:
      summary: List warehouse addresses
      description: List warehouse addresses. The ID of the warehouse must be specified.
      operationId: getRestStockmanagementWarehousesWarehouseAddressesRelationtype
      x-api-path-slug: reststockmanagementwarehouseswarehouseidaddressesrelationtypeid-get
      parameters:
      - in: path
        name: relationTypeId?
      - in: path
        name: warehouseId
      responses:
        200:
          description: OK
      tags:
      - List
      - Warehouse
      - Addresses
  /rest/stockmanagement/warehouses/{warehouseId}/management/racks:
    get:
      summary: List racks
      description: Lists racks for a warehouse. The id of the warehouse must be specified.
      operationId: getRestStockmanagementWarehousesWarehouseManagementRacks
      x-api-path-slug: reststockmanagementwarehouseswarehouseidmanagementracks-get
      parameters:
      - in: query
        name: columns
        description: The attributes to be loaded
      - in: query
        name: itemsPerPage
        description: Number of items per page
      - in: query
        name: page
        description: The requested page
      - in: path
        name: warehouseId
      - in: query
        name: with
        description: The relations to be loaded
      responses:
        200:
          description: OK
      tags:
      - List
      - Racks
  /rest/stockmanagement/warehouses/{warehouseId}/management/racks/{rackId}/shelves:
    get:
      summary: List shelves
      description: Lists shelves for a warehouse. The id of the rack and the id of
        the warehouse must be specified.
      operationId: getRestStockmanagementWarehousesWarehouseManagementRacksRackShelves
      x-api-path-slug: reststockmanagementwarehouseswarehouseidmanagementracksrackidshelves-get
      parameters:
      - in: query
        name: columns
        description: The attributes to be loaded
      - in: query
        name: itemsPerPage
        description: Number of items per page
      - in: query
        name: page
        description: The requested page
      - in: path
        name: rackId
      - in: path
        name: warehouseId
      - in: query
        name: with
        description: The relations to be loaded
      responses:
        200:
          description: OK
      tags:
      - List
      - Shelves
  /rest/stockmanagement/warehouses/{warehouseId}/management/racks/{rackId}/shelves/{shelfId}/storageLocations:
    get:
      summary: List storage locations
      description: Lists storage locations. The id of the warehouse, the id of the
        rack and the id of the shelf must be specified.
      operationId: getRestStockmanagementWarehousesWarehouseManagementRacksRackShelvesShelfStoragelocations
      x-api-path-slug: reststockmanagementwarehouseswarehouseidmanagementracksrackidshelvesshelfidstoragelocations-get
      parameters:
      - in: query
        name: columns
        description: The attributes to be loaded
      - in: query
        name: itemsPerPage
        description: Number of items per page
      - in: query
        name: page
        description: The requested page
      - in: path
        name: rackId
      - in: path
        name: shelfId
      - in: path
        name: warehouseId
      - in: query
        name: with
        description: The relations to be loaded
      responses:
        200:
          description: OK
      tags:
      - List
      - Storage
      - Locations
  /rest/stockmanagement/warehouses/{warehouseId}/management/storageLocations:
    get:
      summary: List storage locations
      description: Lists storage locations that belong to a warehouse. The id of the
        warehouse must be specified.
      operationId: getRestStockmanagementWarehousesWarehouseManagementStoragelocations
      x-api-path-slug: reststockmanagementwarehouseswarehouseidmanagementstoragelocations-get
      parameters:
      - in: query
        name: columns
        description: The attributes to be loaded
      - in: query
        name: itemsPerPage
        description: Number of items per page
      - in: query
        name: page
        description: The requested page
      - in: path
        name: warehouseId
      - in: query
        name: with
        description: The relations to be loaded
      responses:
        200:
          description: OK
      tags:
      - List
      - Storage
      - Locations
  /rest/stockmanagement/warehouses/{warehouseId}/stock:
    get:
      summary: List stock by warehouse
      description: Lists stock for a warehouse. The ID of the warehouse must be specified.
      operationId: getRestStockmanagementWarehousesWarehouseStock
      x-api-path-slug: reststockmanagementwarehouseswarehouseidstock-get
      parameters:
      - in: query
        name: columns
        description: The properties to be loaded
      - in: query
        name: itemsPerPage
        description: The number of items per page
      - in: query
        name: page
        description: The requested page
      - in: query
        name: updatedAtFrom
        description: Filter that restricts the search result to stock that were last
          updated on the specified date
      - in: query
        name: updatedAtTo
        description: Filter that restricts the search result to stock that were last
          updated within a specified period of time
      - in: query
        name: variationId
        description: Filter that restricts the search result to stock with a variation
      - in: path
        name: warehouseId
      responses:
        200:
          description: OK
      tags:
      - List
      - Stock
      - By
      - Warehouse
  /rest/stockmanagement/warehouses/{warehouseId}/stock/movements:
    get:
      summary: List stock movements
      description: |-
        Lists stock movements for a warehouse. The ID of the warehouse must be specified. To get movements older than 3 months, set the 'year' parameter.
        NOTE: You can either get archive entries or non-archive entries. You can not get entries for the current year that are younger and older than 3 months with one request. You need separate requests to get entries older and younger than 3 months. To get all entries younger than 3 month you do not need to specify a year or any createdAt parameter.
      operationId: getRestStockmanagementWarehousesWarehouseStockMovements
      x-api-path-slug: reststockmanagementwarehouseswarehouseidstockmovements-get
      parameters:
      - in: query
        name: columns
        description: The properties to be loaded
      - in: query
        name: createdAtFrom
        description: Get entries with createdAt date after this date
      - in: query
        name: createdAtTo
        description: Get entries with createdAt date before this date
      - in: query
        name: itemId
        description: The ID of the item
      - in: query
        name: itemsPerPage
        description: The number of items per page
      - in: query
        name: page
        description: The requested page
      - in: query
        name: variationId
        description: The ID of the variation
      - in: path
        name: warehouseId
      - in: query
        name: year
        description: Get entries from the archive for the given year
      responses:
        200:
          description: OK
      tags:
      - List
      - Stock
      - Movements
  /rest/stockmanagement/warehouses/{warehouseId}/stock/storageLocations:
    get:
      summary: List stock of a warehouse per storage location
      description: Lists stock of a warehouse for each variation and storage location.
        The stock will only be listed if the stock is positive. Negative stock will
        not be listed. The ID of the warehouse must be specified.
      operationId: getRestStockmanagementWarehousesWarehouseStockStoragelocations
      x-api-path-slug: reststockmanagementwarehouseswarehouseidstockstoragelocations-get
      parameters:
      - in: query
        name: columns
        description: The properties to be loaded
      - in: query
        name: itemsPerPage
        description: The number of items per page
      - in: query
        name: page
        description: The requested page
      - in: query
        name: storageLocationId
        description: Filter that restricts the search result to stock of a storage
          location
      - in: query
        name: updatedAtFrom
        description: Filter that restricts the search result to stock that were last
          updated on the specified date
      - in: query
        name: updatedAtTo
        description: Filter that restricts the search result to stock that were last
          updated within a specified period of time
      - in: query
        name: variationId
        description: Filter that restricts the search result to stock with a variation
      - in: path
        name: warehouseId
      - in: query
        name: with
        description: Load additional relations for a StockStorageLocation
      responses:
        200:
          description: OK
      tags:
      - List
      - Stock
      - Of
      - Warehouse
      - Per
      - Storage
      - Location
  /rest/storage/frontend/files:
    get:
      summary: List files from frontend storage. Append public cloudfront url to each
        retrieved object.
      description: List files from frontend storage. append public cloudfront url
        to each retrieved object..
      operationId: getRestStorageFrontendFiles
      x-api-path-slug: reststoragefrontendfiles-get
      parameters:
      - in: query
        name: continuationToken
        description: The continuationToken of a previous request to continue listing
          objects with
      responses:
        200:
          description: OK
      tags:
      - List
      - Files
      - From
      - Frontend
      - Storage
      - ""
      - Append
      - Public
      - Cloudfront
      - Url
      - To
      - Each
      - Retrieved
      - Object
  /rest/storage/layout/list:
    get:
      summary: List layout documents
      description: |-
        Lists up to 1000 layout documents per request. If more than 1000 layout documents are available,
        a <code>nextContinuationToken</code> is returned. Use this token to get the next (up to) 1000 layout documents.
        Use the same request and include a field with the key <code>continuationToken</code> as well as the returned
        token from the previous call as the value.

        Check the <code>isTruncated</code> field in the response to see if more results are available. If <code>isTruncated</code> is true,
        repeat the request using the token from the <code>nextContinuationToken</code> field of the previous response to get all
        results.
      operationId: getRestStorageLayoutList
      x-api-path-slug: reststoragelayoutlist-get
      parameters:
      - in: query
        name: continuationToken
        description: Token for listing the next (up to) 1000 layout documents
      responses:
        200:
          description: OK
      tags:
      - List
      - Layout
      - Documents
  /rest/storage/plugins/inbox/list:
    get:
      summary: List files from the inbox
      description: |-
        Lists all files of all plugins stored in the inbox. A prefix can be specified to list all files of a specific
        plugin folder only.
      operationId: getRestStoragePluginsInboxList
      x-api-path-slug: reststoragepluginsinboxlist-get
      parameters:
      - in: query
        name: prefix
        description: Prefix to list all files of a specific plugin folder only
      responses:
        200:
          description: OK
      tags:
      - List
      - Files
      - From
      - Inbox
  /rest/tickets:
    get:
      summary: List tickets by filters
      description: List tickets by filters.
      operationId: getRestTickets
      x-api-path-slug: resttickets-get
      parameters:
      - in: query
        name: confidential
        description: Filter that restricts the search result to tickets of a specific
          confidential value
      - in: query
        name: contactId
        description: Filter that restricts the search result to tickets with a specified
          contact ID
      - in: query
        name: customerClassId
        description: Filter that restricts the search result to tickets with a specified
          customer class ID
      - in: query
        name: deadlineAt
        description: Filter that restricts the search result to tickets with a specified
          deadline
      - in: query
        name: fulltext
        description: Filter that restricts the search result to tickets with full-text
          search
      - in: query
        name: id
        description: Filter that restricts the search result to tickets of a specific
          ticket ID
      - in: query
        name: ownerId
        description: Filter that restricts the search result to tickets with a specified
          owner ID
      - in: query
        name: parentTicketId
        description: Filter that restricts the search result to tickets with a specified
          parent ticket ID
      - in: query
        name: plentyId
        description: Filter that restricts the search result to tickets with a specified
          client (store) ID
      - in: query
        name: priorityId
        description: Filter that restricts the search result to tickets of a specific
          ticket priority ID
      - in: query
        name: progress
        description: Filter that restricts the search result to tickets with a specified
          progress in percent
      - in: query
        name: resubmissionAt
        description: Filter that restricts the search result to tickets with a specified
          resubmission date
      - in: query
        name: roleId
        description: Filter that restricts the search result to tickets with a specified
          role ID
      - in: query
        name: source
        description: Filter that restricts the search result to tickets with a specific
          source value
      - in: query
        name: statusGroupId
        description: Filter that restricts the search result to tickets with a specified
          status group ID
      - in: query
        name: statusId
        description: Filter that restricts the search result to tickets with a specified
          status ID
      - in: query
        name: title
        description: Filter that restricts the search result to tickets with a specified
          phrase in title
      - in: query
        name: typeId
        description: Filter that restricts the search result to tickets of specific
          ticket types
      responses:
        200:
          description: OK
      tags:
      - List
      - Tickets
      - By
      - Filters
  /rest/vat:
    get:
      summary: List VAT configurations.
      description: Lists the VAT configurations for the given filter. Possible filters
        are <code>locationId</code>, <code>countryId</code>, <code>taxIdNumber</code>
        and <code>startedAt</code>.
      operationId: getRestVat
      x-api-path-slug: restvat-get
      parameters:
      - in: query
        name: columns
        description: The properties to be loaded
      - in: query
        name: itemsPerPage
        description: The number of items per page
      - in: query
        name: page
        description: The requested page
      - in: query
        name: with
        description: The relations to load with the VAT object
      responses:
        200:
          description: OK
      tags:
      - List
      - VAT
      - Configurations
  /rest/vat/locations/{locationId}:
    get:
      summary: List VAT configurations of an accounting location
      description: Lists the VAT configurations for all countries of one accounting
        location
      operationId: getRestVatLocationsLocation
      x-api-path-slug: restvatlocationslocationid-get
      parameters:
      - in: query
        name: columns[]
        description: The attributes of the VAT configuration
      - in: path
        name: locationId
      - in: query
        name: with[]
        description: The relations to load with the VAT object
      responses:
        200:
          description: OK
      tags:
      - List
      - VAT
      - Configurations
      - Of
      - Accounting
      - Location
  /rest/vat/locations/{locationId}/countries/{countryId}:
    get:
      summary: List VAT configurations for one country of delivery
      description: Lists the VAT configurations for a country of delivery of one accounting
        location. The ID of the accounting location and the ID of the country of delivery
        must be specified.
      operationId: getRestVatLocationsLocationCountriesCountry
      x-api-path-slug: restvatlocationslocationidcountriescountryid-get
      parameters:
      - in: query
        name: columns[]
        description: The attributes of the VAT configuration
      - in: path
        name: countryId
      - in: path
        name: locationId
      - in: query
        name: with[]
        description: The relations to load with the VAT object
      responses:
        200:
          description: OK
      tags:
      - List
      - VAT
      - Configurationsone
      - Country
      - Of
      - Delivery
  /rest/warehouses/{warehouseId}/locations:
    get:
      summary: List warehouse locations
      description: Lists all warehouse locations.
      operationId: getRestWarehousesWarehouseLocations
      x-api-path-slug: restwarehouseswarehouseidlocations-get
      parameters:
      - in: path
        name: warehouseId
      responses:
        200:
          description: OK
      tags:
      - List
      - Warehouse
      - Locations
  /rest/warehouses/{warehouseId}/locations/dimensions:
    get:
      summary: List warehouse location dimensions
      description: Lists all warehouse location dimensions.
      operationId: getRestWarehousesWarehouseLocationsDimensions
      x-api-path-slug: restwarehouseswarehouseidlocationsdimensions-get
      parameters:
      - in: path
        name: warehouseId
      responses:
        200:
          description: OK
      tags:
      - List
      - Warehouse
      - Location
      - Dimensions
  /rest/warehouses/{warehouseId}/locations/levels:
    get:
      summary: List warehouse location levels
      description: Lists all warehouse location levels.
      operationId: getRestWarehousesWarehouseLocationsLevels
      x-api-path-slug: restwarehouseswarehouseidlocationslevels-get
      parameters:
      - in: path
        name: warehouseId
      responses:
        200:
          description: OK
      tags:
      - List
      - Warehouse
      - Location
      - Levels
  /rest/webstores:
    get:
      summary: List clients (stores)
      description: List clients (stores).
      operationId: getRestWebstores
      x-api-path-slug: restwebstores-get
      responses:
        200:
          description: OK
      tags:
      - List
      - Clients
      - (stores)
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