swagger: "2.0"
x-collection-name: RingCentral
x-complete: 1
info:
  title: RingCentral Connect Platform API Explorer
  description: this-is-an-interactive-api-explorer-for-the-ringcentral-connect-platform--to-use-this-service-you-will-need-to-have-a-developer-account---links--a-hrefhttpsnetstorage-ringcentral-comdpwapiexplorerrcplatform-basic-ymlv20180514092722-target-blankringcentral-api-specaspannbspnbspopenapi-fka-swagger-formatnbspnbspnbspnbspspana-hrefhttpsgithub-comoaiopenapispecification-target-blanklearn-more-about-openapia
  version: 1.0.0
host: platform.ringcentral.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /restapi/v1.0/account/{accountId}/extension/{extensionId}/message-store:
    get:
      summary: Get Message List
      description: "Returns the list of messages from an extension mailbox.\nApp Permission\nReadMessages\nUser
        Permission\nReadMessages\nUsage Plan Group\nLight\nError Codes\n\n \n  \n
        \  HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nCMN-101\nParameter
        [readStatus] value is invalid\n\n\n401\nCMN-405\nLogin to extension required\n\n\n401\nOAU-151\nAuthorization
        method not supported\n\n\n403\nCMN-401\nIn order to call this API endpoint,
        application needs to have [ReadMessages] permission\n\n\n403\nCMN-408\nIn
        order to call this API endpoint, user needs to have [ReadMessages] permission
        for requested resource.\n\n\n404\nCMN-102\nResource for parameter [extensionId]
        is not found"
      operationId: listMessages
      x-api-path-slug: restapiv1-0accountaccountidextensionextensionidmessagestore-get
      parameters:
      - in: path
        name: accountId
        description: Internal identifier of a RingCentral account or tilde (~) to
          indicate the account logged-in within the current session
      - in: query
        name: availability
        description: Specifies the availability status for the resulting messages
      - in: query
        name: conversationId
        description: Specifies the conversation identifier for the resulting messages
      - in: query
        name: dateFrom
        description: The start datetime for resulting messages in ISO 8601 format
          including timezone, for example 2016-03-10T18:07:52
      - in: query
        name: dateTo
        description: The end datetime for resulting messages in ISO 8601 format including
          timezone, for example 2016-03-10T18:07:52
      - in: query
        name: direction
        description: The direction for the resulting messages
      - in: query
        name: distinctConversations
        description: If True, then the latest messages per every conversation ID are
          returned
      - in: path
        name: extensionId
        description: Internal identifier of an extension or tilde (~) to indicate
          the extension assigned to the account logged-in within the current session
      - in: query
        name: messageType
        description: The type of the resulting messages
      - in: query
        name: page
        description: Indicates the page number to retrieve
      - in: query
        name: perPage
        description: Indicates the page size (number of items)
      - in: query
        name: phoneNumber
        description: The phone number
      - in: query
        name: readStatus
        description: The read status for the resulting messages
      responses:
        200:
          description: OK
      tags:
      - Message
      - List
  /restapi/v1.0/account/{accountId}/extension/{extensionId}/phone-number:
    get:
      summary: Get Extension Phone Number List
      description: "Returns the list of phone numbers that are used by a particular
        extension, and can be filtered by the phone number type. The returned list
        contains all numbers which are directly mapped to a given extension plus the
        features and also company-level numbers which may be used when performing
        different operations on behalf of this extension.\nApp Permission\nReadAccounts\nUser
        Permission\nReadUserPhoneNumbers\nUsage Plan Group\nLight\nError Codes\n\n
        \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nCMN-101\nParameter
        [usageType] value is invalid\n\n\n401\nCMN-405\nLogin to extension required\n\n\n401\nOAU-151\nAuthorization
        method not supported\n\n\n403\nCMN-401\nIn order to call this API endpoint,
        application needs to have [ReadAccounts] permission\n\n\n404\nCMN-102\nResource
        for parameter [extensionId] is not found"
      operationId: listExtensionPhoneNumbers
      x-api-path-slug: restapiv1-0accountaccountidextensionextensionidphonenumber-get
      parameters:
      - in: path
        name: accountId
        description: Internal identifier of a RingCentral account or tilde (~) to
          indicate the account logged-in within the current session
      - in: path
        name: extensionId
        description: Internal identifier of an extension or tilde (~) to indicate
          the extension assigned to the account logged-in within the current session
      - in: query
        name: page
        description: Indicates the page number to retrieve
      - in: query
        name: perPage
        description: Indicates the page size (number of items)
      - in: query
        name: usageType
        description: Usage type of a phone number
      responses:
        200:
          description: OK
      tags:
      - Extension
      - Phone
      - Number
      - List
  /restapi/v1.0/dictionary/language:
    get:
      summary: Get Language List
      description: "Returns the information about supported languages.\nUsage Plan
        Group\nLight\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error
        Message\n   \n \n\n400\nCMN-101\nParameter [perPage] value is invalid"
      operationId: listLanguages
      x-api-path-slug: restapiv1-0dictionarylanguage-get
      responses:
        200:
          description: OK
      tags:
      - Language
      - List
  /restapi/v1.0/dictionary/country:
    get:
      summary: Get Country List
      description: "Returns all the countries available for calling.\nUsage Plan Group\nLight\nError
        Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nCMN-101\nParameter
        [perPage] value is invalid\n\n\n401\nAGW-401\nAuthorization header is not
        specified\n\n\n401\nOAU-129\nAccess token corrupted"
      operationId: listCountries
      x-api-path-slug: restapiv1-0dictionarycountry-get
      parameters:
      - in: query
        name: freeSoftphoneLine
        description: Specifies if free phone line for softphone is available for a
          country or not
      - in: query
        name: loginAllowed
        description: Specifies whether login with the phone numbers of this country
          is enabled or not
      - in: query
        name: numberSelling
        description: Specifies if RingCentral sells phone numbers of this country
      - in: query
        name: page
        description: Indicates the page number to retrieve
      - in: query
        name: perPage
        description: Indicates the page size (number of items)
      - in: query
        name: signupAllowed
        description: Indicates whether signup/billing is allowed for a country
      responses:
        200:
          description: OK
      tags:
      - Country
      - List
  /restapi/v1.0/dictionary/location:
    get:
      summary: Get Location List
      description: "Returns all available locations for a certain state.\nUsage Plan
        Group\nLight\nError Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error
        Message\n   \n \n\n400\nCMN-101\nParameter [orderBy] value is invalid\n\n\n404\nCMN-102\nResource
        for parameter [location] is not found"
      operationId: listLocations
      x-api-path-slug: restapiv1-0dictionarylocation-get
      parameters:
      - in: query
        name: orderBy
        description: Sorts results by the property specified
      - in: query
        name: page
        description: Indicates the page number to retrieve
      - in: query
        name: perPage
        description: Indicates the page size (number of items)
      - in: query
        name: stateId
        description: Internal identifier of a state
      - in: query
        name: withNxx
        description: Specifies if nxx codes are returned
      responses:
        200:
          description: OK
      tags:
      - Location
      - List
  /restapi/v1.0/dictionary/state:
    get:
      summary: Get State List
      description: "Returns all the states of a certain country\nUsage Plan Group\nLight\nError
        Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nCMN-101\nParameter
        [perPage] value is invalid\n\n\n404\nCMN-102\nResource for parameter [stateId]
        is not found"
      operationId: listStates
      x-api-path-slug: restapiv1-0dictionarystate-get
      parameters:
      - in: query
        name: countryId
        description: Internal identifier of a country
      - in: query
        name: page
        description: Indicates the page number to retrieve
      - in: query
        name: perPage
        description: Indicates the page size (number of items)
      - in: query
        name: withPhoneNumbers
        description: If True, the list of states with phone numbers available for
          buying is returned
      responses:
        200:
          description: OK
      tags:
      - State
      - List
  /restapi/v1.0/dictionary/timezone:
    get:
      summary: Get Timezone List
      description: "Returns all available timezones.\nUsage Plan Group\nLight\nError
        Codes\n\n \n  \n   HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nCMN-101\nParameter
        [perPage] value is invalid"
      operationId: listTimezones
      x-api-path-slug: restapiv1-0dictionarytimezone-get
      parameters:
      - in: query
        name: page
        description: Indicates the page number to retrieve
      - in: query
        name: perPage
        description: Indicates the page size (number of items)
      responses:
        200:
          description: OK
      tags:
      - Timezone
      - List
  /restapi/v1.0/account/{accountId}/department/{departmentId}/members:
    get:
      summary: Get Department Member List
      description: "[Deprecated] Viewing user account info (including name, business
        name, address and phone number/account number)\nApp Permission\nReadAccounts\nUser
        Permission\nReadExtensions\nUsage Plan Group\nLight\nError Codes\n\n \n  \n
        \  HTTP Code\n   Error Code\n   Error Message\n   \n \n\n400\nCMN-101\nParameter
        [page] value is invalid\n\n\n401\nCMN-405\nLogin to extension required\n\n\n401\nOAU-151\nAuthorization
        method not supported\n\n\n403\nCMN-401\nIn order to call this API endpoint,
        application needs to have [ReadAccounts] permission\n\n\n404\nCMN-102\nResource
        for parameter [departmentId] is not found"
      operationId: listDepartmentMembers
      x-api-path-slug: restapiv1-0accountaccountiddepartmentdepartmentidmembers-get
      parameters:
      - in: path
        name: accountId
        description: Internal identifier of a RingCentral account or tilde (~) to
          indicate the account logged-in within the current session
      - in: path
        name: departmentId
        description: Internal identifier of a Department extension (same as extensionId
          but only the ID of a department extension is valid)
      - in: query
        name: page
        description: Indicates the page number to retrieve
      - in: query
        name: perPage
        description: Indicates the page size (number of items)
      responses:
        200:
          description: OK
      tags:
      - Department
      - Member
      - List
  /scim/v2/Users:
    get:
      summary: search or list users
      description: ""
      operationId: searchViaGet
      x-api-path-slug: scimv2users-get
      parameters:
      - in: query
        name: count
        description: page size
      - in: query
        name: filter
        description: only support userName or email filter expressions for now
      - in: query
        name: startIndex
        description: start index (1-based)
      responses:
        200:
          description: OK
      tags:
      - Search
      - List
      - Users
  /scim/v2/Users/.search:
    post:
      summary: search or list users
      description: ""
      operationId: searchViaPost
      x-api-path-slug: scimv2users-search-post
      parameters:
      - in: body
        name: body
        description: search parameters
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Search
      - List
      - Users