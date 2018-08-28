---
swagger: "2.0"
x-collection-name: Trello
x-complete: 0
info:
  title: Trello Get Lists List Cards Filter
  description: Get lists list cards filter.
  termsOfService: https://trello.com/legal
  contact:
    name: Trello
    url: https://trello.com/home
  version: "1.0"
host: trello.com
basePath: /1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /boards/{idBoard}/lists:
    get:
      summary: Get Boards Lists
      description: Get boards lists.
      operationId: getBoardsListsByIdBoard
      x-api-path-slug: boardsidboardlists-get
      parameters:
      - in: query
        name: cards
        description: 'One of: all, closed, none, open or visible'
      - in: query
        name: card_fields
        description: 'all or a comma-separated list of: badges, checkItemStates, closed,
          dateLastActivity, desc, descData, due, email, idAttachmentCover, idBoard,
          idChecklists, idLabels, idList, idMembers, idMembersVoted, idShort, labels,
          manualCoverAttachment, name, pos, shortLink, shortUrl, subscribed or url'
      - in: query
        name: fields
        description: 'all or a comma-separated list of: closed, idBoard, name, pos
          or subscribed'
      - in: query
        name: filter
        description: 'One of: all, closed, none or open'
      - in: path
        name: idBoard
        description: board_id
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Lists
    post:
      summary: Post Boards Lists
      description: Post boards lists.
      operationId: addBoardsListsByIdBoard
      x-api-path-slug: boardsidboardlists-post
      parameters:
      - in: body
        name: body
        description: Attributes of Boards Lists to be added
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idBoard
        description: board_id
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Lists
  /boards/{idBoard}/lists/{filter}:
    get:
      summary: Get Boards Lists Filter
      description: Get boards lists filter.
      operationId: getBoardsListsByIdBoardByFilter
      x-api-path-slug: boardsidboardlistsfilter-get
      parameters:
      - in: path
        name: filter
        description: filter
      - in: path
        name: idBoard
        description: board_id
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Lists
      - Filter
  /lists:
    post:
      summary: Post Lists
      description: Post lists.
      operationId: addLists
      x-api-path-slug: lists-post
      parameters:
      - in: body
        name: body
        description: Attributes of Lists to be added
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Lists
  /lists/{idList}:
    get:
      summary: Get Lists List
      description: Get lists list.
      operationId: getListsByIdList
      x-api-path-slug: listsidlist-get
      parameters:
      - in: query
        name: board
        description: true or false
      - in: query
        name: board_fields
        description: 'all or a comma-separated list of: closed, dateLastActivity,
          dateLastView, desc, descData, idOrganization, invitations, invited, labelNames,
          memberships, name, pinned, powerUps, prefs, shortLink, shortUrl, starred,
          subscribed or url'
      - in: query
        name: cards
        description: 'One of: all, closed, none or open'
      - in: query
        name: card_fields
        description: 'all or a comma-separated list of: badges, checkItemStates, closed,
          dateLastActivity, desc, descData, due, email, idAttachmentCover, idBoard,
          idChecklists, idLabels, idList, idMembers, idMembersVoted, idShort, labels,
          manualCoverAttachment, name, pos, shortLink, shortUrl, subscribed or url'
      - in: query
        name: fields
        description: 'all or a comma-separated list of: closed, idBoard, name, pos
          or subscribed'
      - in: path
        name: idList
        description: idList
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Lists
      - List
    put:
      summary: Put Lists List
      description: Put lists list.
      operationId: updateListsByIdList
      x-api-path-slug: listsidlist-put
      parameters:
      - in: body
        name: body
        description: Attributes of Lists to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idList
        description: idList
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Lists
      - List
  /lists/{idList}/actions:
    get:
      summary: Get Lists List Actions
      description: Get lists list actions.
      operationId: getListsActionsByIdList
      x-api-path-slug: listsidlistactions-get
      parameters:
      - in: query
        name: before
        description: A date, or null
      - in: query
        name: display
        description: true or false
      - in: query
        name: entities
        description: true or false
      - in: query
        name: fields
        description: 'all or a comma-separated list of: data, date, idMemberCreator
          or type'
      - in: query
        name: filter
        description: 'all or a comma-separated list of: addAttachmentToCard, addChecklistToCard,
          addMemberToBoard, addMemberToCard, addMemberToOrganization, addToOrganizationBoard,
          commentCard, convertToCardFromCheckItem, copyBoard, copyCard, copyCommentCard,
          createBoard, createCard, createList, createOrganization, deleteAttachmentFromCard,
          deleteBoardInvitation, deleteCard, deleteOrganizationInvitation, disablePowerUp,
          emailCard, enablePowerUp, makeAdminOfBoard, makeNormalMemberOfBoard, makeNormalMemberOfOrganization,
          makeObserverOfBoard, memberJoinedTrello, moveCardFromBoard, moveCardToBoard,
          moveListFromBoard, moveListToBoard, removeChecklistFromCard, removeFromOrganizationBoard,
          removeMemberFromCard, unconfirmedBoardInvitation, unconfirmedOrganizationInvitation,
          updateBoard, updateCard, updateCard:closed, updateCard:desc, updateCard:idList,
          updateCard:name, updateCheckItemStateOnCard, updateChecklist, updateList,
          updateList:closed, updateList:name, updateMember or updateOrganization'
      - in: query
        name: format
        description: 'One of: count, list or minimal'
      - in: path
        name: idList
        description: idList
      - in: query
        name: idModels
        description: Only return actions related to these model ids
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: limit
        description: a number from 0 to 1000
      - in: query
        name: member
        description: true or false
      - in: query
        name: memberCreator
        description: true or false
      - in: query
        name: memberCreator_fields
        description: 'all or a comma-separated list of: avatarHash, bio, bioData,
          confirmed, fullName, idPremOrgsAdmin, initials, memberType, products, status,
          url or username'
      - in: query
        name: member_fields
        description: 'all or a comma-separated list of: avatarHash, bio, bioData,
          confirmed, fullName, idPremOrgsAdmin, initials, memberType, products, status,
          url or username'
      - in: query
        name: page
        description: Page * limit must be less than 1000
      - in: query
        name: since
        description: A date, null or lastView
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Lists
      - List
      - Actions
  /lists/{idList}/archiveAllCards:
    post:
      summary: Post Lists List Archiveallcards
      description: Post lists list archiveallcards.
      operationId: addListsArchiveAllCardsByIdList
      x-api-path-slug: listsidlistarchiveallcards-post
      parameters:
      - in: path
        name: idList
        description: idList
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Lists
      - List
      - Archiveallcards
  /lists/{idList}/board:
    get:
      summary: Get Lists List Board
      description: Get lists list board.
      operationId: getListsBoardByIdList
      x-api-path-slug: listsidlistboard-get
      parameters:
      - in: query
        name: fields
        description: 'all or a comma-separated list of: closed, dateLastActivity,
          dateLastView, desc, descData, idOrganization, invitations, invited, labelNames,
          memberships, name, pinned, powerUps, prefs, shortLink, shortUrl, starred,
          subscribed or url'
      - in: path
        name: idList
        description: idList
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Lists
      - List
      - Board
  /lists/{idList}/board/{field}:
    get:
      summary: Get Lists List Board Field
      description: Get lists list board field.
      operationId: getListsBoardByIdListByField
      x-api-path-slug: listsidlistboardfield-get
      parameters:
      - in: path
        name: field
        description: field
      - in: path
        name: idList
        description: idList
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Lists
      - List
      - Board
      - Field
  /lists/{idList}/cards:
    get:
      summary: Get Lists List Cards
      description: Get lists list cards.
      operationId: getListsCardsByIdList
      x-api-path-slug: listsidlistcards-get
      parameters:
      - in: query
        name: actions
        description: 'all or a comma-separated list of: addAttachmentToCard, addChecklistToCard,
          addMemberToBoard, addMemberToCard, addMemberToOrganization, addToOrganizationBoard,
          commentCard, convertToCardFromCheckItem, copyBoard, copyCard, copyCommentCard,
          createBoard, createCard, createList, createOrganization, deleteAttachmentFromCard,
          deleteBoardInvitation, deleteCard, deleteOrganizationInvitation, disablePowerUp,
          emailCard, enablePowerUp, makeAdminOfBoard, makeNormalMemberOfBoard, makeNormalMemberOfOrganization,
          makeObserverOfBoard, memberJoinedTrello, moveCardFromBoard, moveCardToBoard,
          moveListFromBoard, moveListToBoard, removeChecklistFromCard, removeFromOrganizationBoard,
          removeMemberFromCard, unconfirmedBoardInvitation, unconfirmedOrganizationInvitation,
          updateBoard, updateCard, updateCard:closed, updateCard:desc, updateCard:idList,
          updateCard:name, updateCheckItemStateOnCard, updateChecklist, updateList,
          updateList:closed, updateList:name, updateMember or updateOrganization'
      - in: query
        name: attachments
        description: A boolean value or &quot;cover&quot; for only card cover attachments
      - in: query
        name: attachment_fields
        description: 'all or a comma-separated list of: bytes, date, edgeColor, idMember,
          isUpload, mimeType, name, previews or url'
      - in: query
        name: before
        description: A date, or null
      - in: query
        name: checkItemStates
        description: true or false
      - in: query
        name: checklists
        description: 'One of: all or none'
      - in: query
        name: fields
        description: 'all or a comma-separated list of: badges, checkItemStates, closed,
          dateLastActivity, desc, descData, due, email, idAttachmentCover, idBoard,
          idChecklists, idLabels, idList, idMembers, idMembersVoted, idShort, labels,
          manualCoverAttachment, name, pos, shortLink, shortUrl, subscribed or url'
      - in: query
        name: filter
        description: 'One of: all, closed, none or open'
      - in: path
        name: idList
        description: idList
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: limit
        description: a number from 1 to 1000
      - in: query
        name: members
        description: true or false
      - in: query
        name: member_fields
        description: 'all or a comma-separated list of: avatarHash, bio, bioData,
          confirmed, fullName, idPremOrgsAdmin, initials, memberType, products, status,
          url or username'
      - in: query
        name: since
        description: A date, or null
      - in: query
        name: stickers
        description: true or false
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Lists
      - List
      - Cards
    post:
      summary: Post Lists List Cards
      description: Post lists list cards.
      operationId: addListsCardsByIdList
      x-api-path-slug: listsidlistcards-post
      parameters:
      - in: body
        name: body
        description: Attributes of Lists Cards to be added
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idList
        description: idList
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Lists
      - List
      - Cards
  /lists/{idList}/cards/{filter}:
    get:
      summary: Get Lists List Cards Filter
      description: Get lists list cards filter.
      operationId: getListsCardsByIdListByFilter
      x-api-path-slug: listsidlistcardsfilter-get
      parameters:
      - in: path
        name: filter
        description: filter
      - in: path
        name: idList
        description: idList
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Lists
      - List
      - Cards
      - Filter
  /lists/{idList}/closed:
    put:
      summary: Put Lists List Closed
      description: Put lists list closed.
      operationId: updateListsClosedByIdList
      x-api-path-slug: listsidlistclosed-put
      parameters:
      - in: body
        name: body
        description: Attributes of Lists Closed to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idList
        description: idList
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Lists
      - List
      - Closed
  /lists/{idList}/idBoard:
    put:
      summary: Put Lists List Board
      description: Put lists list board.
      operationId: updateListsIdBoardByIdList
      x-api-path-slug: listsidlistidboard-put
      parameters:
      - in: body
        name: body
        description: Attributes of Lists Id Board to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idList
        description: idList
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Lists
      - List
      - Board
  /lists/{idList}/moveAllCards:
    post:
      summary: Post Lists List Moveallcards
      description: Post lists list moveallcards.
      operationId: addListsMoveAllCardsByIdList
      x-api-path-slug: listsidlistmoveallcards-post
      parameters:
      - in: body
        name: body
        description: Attributes of Lists Move All Cards to be added
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idList
        description: idList
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Lists
      - List
      - Moveallcards
  /lists/{idList}/name:
    put:
      summary: Put Lists List Name
      description: Put lists list name.
      operationId: updateListsNameByIdList
      x-api-path-slug: listsidlistname-put
      parameters:
      - in: body
        name: body
        description: Attributes of Lists Name to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idList
        description: idList
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Lists
      - List
      - Name
  /lists/{idList}/pos:
    put:
      summary: Put Lists List Pos
      description: Put lists list pos.
      operationId: updateListsPosByIdList
      x-api-path-slug: listsidlistpos-put
      parameters:
      - in: body
        name: body
        description: Attributes of Lists Pos to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idList
        description: idList
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Lists
      - List
      - Pos
  /lists/{idList}/subscribed:
    put:
      summary: Put Lists List Subscribed
      description: Put lists list subscribed.
      operationId: updateListsSubscribedByIdList
      x-api-path-slug: listsidlistsubscribed-put
      parameters:
      - in: body
        name: body
        description: Attributes of Lists Subscribed to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idList
        description: idList
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Lists
      - List
      - Subscribed
  /lists/{idList}/{field}:
    get:
      summary: Get Lists List Field
      description: Get lists list field.
      operationId: getListsByIdListByField
      x-api-path-slug: listsidlistfield-get
      parameters:
      - in: path
        name: field
        description: field
      - in: path
        name: idList
        description: idList
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Lists
      - List
      - Field
  /actions/{idAction}/list:
    get:
      summary: Get Actions List
      description: Get actions list.
      operationId: getActionsListByIdAction
      x-api-path-slug: actionsidactionlist-get
      parameters:
      - in: query
        name: fields
        description: 'all or a comma-separated list of: closed, idBoard, name, pos
          or subscribed'
      - in: path
        name: idAction
        description: idAction
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Actions
      - List
  /actions/{idAction}/list/{field}:
    get:
      summary: Get Actions List Field
      description: Get actions list field.
      operationId: getActionsListByIdActionByField
      x-api-path-slug: actionsidactionlistfield-get
      parameters:
      - in: path
        name: field
        description: field
      - in: path
        name: idAction
        description: idAction
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Actions
      - List
      - Field
  /cards/{idCard}/idList:
    put:
      summary: Put Cards List
      description: Put cards list.
      operationId: updateCardsIdListByIdCard
      x-api-path-slug: cardsidcardidlist-put
      parameters:
      - in: body
        name: body
        description: Attributes of Cards Id List to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idCard
        description: card id or shortlink
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Cards
      - List
  /cards/{idCard}/list:
    get:
      summary: Get Cards List
      description: Get cards list.
      operationId: getCardsListByIdCard
      x-api-path-slug: cardsidcardlist-get
      parameters:
      - in: query
        name: fields
        description: 'all or a comma-separated list of: closed, idBoard, name, pos
          or subscribed'
      - in: path
        name: idCard
        description: card id or shortlink
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Cards
      - List
  /cards/{idCard}/list/{field}:
    get:
      summary: Get Cards List Field
      description: Get cards list field.
      operationId: getCardsListByIdCardByField
      x-api-path-slug: cardsidcardlistfield-get
      parameters:
      - in: path
        name: field
        description: field
      - in: path
        name: idCard
        description: card id or shortlink
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Cards
      - List
      - Field
  /notifications/{idNotification}/list:
    get:
      summary: Get Notifications Notification List
      description: Get notifications notification list.
      operationId: getNotificationsListByIdNotification
      x-api-path-slug: notificationsidnotificationlist-get
      parameters:
      - in: query
        name: fields
        description: 'all or a comma-separated list of: closed, idBoard, name, pos
          or subscribed'
      - in: path
        name: idNotification
        description: idNotification
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Notifications
      - Notification
      - List
  /notifications/{idNotification}/list/{field}:
    get:
      summary: Get Notifications Notification List Field
      description: Get notifications notification list field.
      operationId: getNotificationsListByIdNotificationByField
      x-api-path-slug: notificationsidnotificationlistfield-get
      parameters:
      - in: path
        name: field
        description: field
      - in: path
        name: idNotification
        description: idNotification
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Notifications
      - Notification
      - List
      - Field
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