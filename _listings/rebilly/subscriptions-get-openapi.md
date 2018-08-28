---
swagger: "2.0"
x-collection-name: Rebilly
x-complete: 0
info:
  title: Rebilly Retrieve a list of subscriptions
  description: Retrieve a list of subscriptions
  termsOfService: https://www.rebilly.com/terms/
  contact:
    name: Rebilly API Support
    url: https://www.rebilly.com/contact/
    email: integrations@rebilly.com
  version: "2.1"
host: api.rebilly.com
basePath: /v2.1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /lists:
    get:
      summary: Retrieve a collection of Lists (latest version of each List)
      description: Retrieve a collection of Lists
      operationId: retrieve-a-collection-of-lists
      x-api-path-slug: lists-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Collection
      - Of
      - Lists
      - (latest
      - Version
      - Of
      - Each
      - List)
    post:
      summary: Create a List
      description: Create a List
      operationId: create-a-list
      x-api-path-slug: lists-post
      parameters:
      - in: body
        name: body
        description: List resource
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - List
  /lists/{id}:
    get:
      summary: Retrieve list's latest version
      description: Retrieve latest version of List with specified identifier string
      operationId: retrieve-latest-version-of-list-with-specified-identifier-string
      x-api-path-slug: listsid-get
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Lists
      - Latest
      - Version
    delete:
      summary: Delete a list
      description: Delete a list with predefined identifier string
      operationId: delete-a-list-with-predefined-identifier-string
      x-api-path-slug: listsid-delete
      responses:
        200:
          description: OK
      tags:
      - List
    put:
      summary: Create or update a list with predefined ID
      description: Create or update a list with predefined identifier string
      operationId: create-or-update-a-list-with-predefined-identifier-string
      x-api-path-slug: listsid-put
      parameters:
      - in: body
        name: body
        description: List resource
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Update
      - List
      - Predefined
      - ID
  /lists/{id}/{version}:
    get:
      summary: Retrieve List's exact version
      description: ""
      operationId: ""
      x-api-path-slug: listsidversion-get
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Lists
      - Exact
      - Version
  /tracking/lists:
    get:
      summary: Retrieve Lists changes history
      description: ""
      operationId: ""
      x-api-path-slug: trackinglists-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Lists
      - Changes
      - History
  /3dsecure:
    get:
      summary: Retrieve a list of ThreeDSecure entries
      description: Retrieve a list of ThreeDSecure entries
      operationId: 3dsecure.get
      x-api-path-slug: 3dsecure-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - List
      - Of
      - ThreeDSecure
      - Entries
  /attachments:
    get:
      summary: Retrieve a list of Attachments
      description: Retrieve a list of Attachments
      operationId: attachments.get
      x-api-path-slug: attachments-get
      parameters:
      - in: query
        name: No Name
      - in: query
        name: sort
        description: The collection items sort field and order (prefix with - for
          descending sort)
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - List
      - Of
      - Attachments
  /authentication-tokens:
    get:
      summary: Retrieve a list of auth tokens
      description: Retrieve a list of auth tokens
      operationId: authentication_tokens.get
      x-api-path-slug: authenticationtokens-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - List
      - Of
      - Auth
      - Tokens
  /bank-accounts:
    get:
      summary: Retrieve a list of bank accounts
      description: Retrieve a list of Bank Accounts
      operationId: bank_accounts.get
      x-api-path-slug: bankaccounts-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - List
      - Of
      - Bank
      - Accounts
  /blacklists:
    get:
      summary: Retrieve a list of blacklists
      description: Retrieve a list of blacklists
      operationId: blacklists.get
      x-api-path-slug: blacklists-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - List
      - Of
      - Blacklists
  /contacts:
    get:
      summary: Retrieve a list of contacts
      description: Retrieve a list of contacts
      operationId: contacts.get
      x-api-path-slug: contacts-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - List
      - Of
      - Contacts
  /coupons:
    get:
      summary: Retrieve a list of coupons
      description: Retrieve a list of coupons
      operationId: coupons.get
      x-api-path-slug: coupons-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - List
      - Of
      - Coupons
  /coupons-redemptions:
    get:
      summary: Retrieve a list of coupon redemptions
      description: ""
      operationId: coupons_redemptions.get
      x-api-path-slug: couponsredemptions-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - List
      - Of
      - Coupon
      - Redemptions
  /credentials:
    get:
      summary: Retrieve a list of credentials
      description: Retrieve a list of credentials
      operationId: credentials.get
      x-api-path-slug: credentials-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - List
      - Of
      - Credentials
  /customers:
    get:
      summary: Retrieve a list of customers
      description: Retrieve a list of customers
      operationId: customers.get
      x-api-path-slug: customers-get
      parameters:
      - in: header
        name: Accept
        description: The response media type
      - in: query
        name: No Name
      - in: query
        name: sort
        description: The collection items sort field and order (prefix with - for
          descending sort)
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - List
      - Of
      - Customers
  /disputes:
    get:
      summary: Retrieve a list of disputes
      description: Retrieve a list of disputes
      operationId: disputes.get
      x-api-path-slug: disputes-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - List
      - Of
      - Disputes
  /files:
    get:
      summary: Retrieve a list of files
      description: Retrieve a list of files
      operationId: files.get
      x-api-path-slug: files-get
      parameters:
      - in: query
        name: No Name
      - in: query
        name: sort
        description: The collection items sort field and order (prefix with - for
          descending sort)
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - List
      - Of
      - Files
  /invoices:
    get:
      summary: Retrieve a list of invoices
      description: Retrieve a list of invoices
      operationId: invoices.get
      x-api-path-slug: invoices-get
      parameters:
      - in: header
        name: Accept
        description: The response media type
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - List
      - Of
      - Invoices
  /password-tokens:
    get:
      summary: Retrieve a list of tokens
      description: Retrieve a list of tokens
      operationId: password_tokens.get
      x-api-path-slug: passwordtokens-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - List
      - Of
      - Tokens
  /payment-cards:
    get:
      summary: Retrieve a list of Payment Cards
      description: Retrieve a list of Payments Cards
      operationId: payment_cards.get
      x-api-path-slug: paymentcards-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - List
      - Of
      - Payment
      - Cards
  /payments:
    get:
      summary: Retrieve a payment list
      description: Retrieve a payment list
      operationId: payments.get
      x-api-path-slug: payments-get
      parameters:
      - in: header
        name: Accept
        description: The response media type
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Payment
      - List
  /paypal-accounts:
    get:
      summary: Retrieve a list of PayPal accounts
      description: Retrieve a list of PayPal Accounts
      operationId: paypal_accounts.get
      x-api-path-slug: paypalaccounts-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - List
      - Of
      - PayPal
      - Accounts
  /plans:
    get:
      summary: Retrieve a list of plans
      description: Retrieve a list of plans
      operationId: plans.get
      x-api-path-slug: plans-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - List
      - Of
      - Plans
  /products:
    get:
      summary: Retrieve a list of products
      description: Retrieve a list of products
      operationId: products.get
      x-api-path-slug: products-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - List
      - Of
      - Products
  /queue/payments:
    get:
      summary: Retrieve a scheduled payment list
      description: Retrieve a scheduled payment list
      operationId: queue.payments.get
      x-api-path-slug: queuepayments-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Scheduled
      - Payment
      - List
  /shipping-zones:
    get:
      summary: Retrieve a list of shipping zones
      description: Retrieve a list of shipping zones
      operationId: shipping_zones.get
      x-api-path-slug: shippingzones-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - List
      - Of
      - Shipping
      - Zones
  /subscriptions:
    get:
      summary: Retrieve a list of subscriptions
      description: Retrieve a list of subscriptions
      operationId: subscriptions.get
      x-api-path-slug: subscriptions-get
      parameters:
      - in: header
        name: Accept
        description: The response media type
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - List
      - Of
      - Subscriptions
  /tax-categories:
    get:
      summary: Retrieve a list of tax categories
      description: Retrieve a list of tax categories
      operationId: tax_categories.get
      x-api-path-slug: taxcategories-get
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - List
      - Of
      - Tax
      - Categories
  /tokens:
    get:
      summary: Retrieve a list of tokens
      description: Retrieve a list of tokens
      operationId: tokens.get
      x-api-path-slug: tokens-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - List
      - Of
      - Tokens
  /transactions:
    get:
      summary: Retrieve a list of transactions
      description: Retrieve a list of transactions
      operationId: transactions.get
      x-api-path-slug: transactions-get
      parameters:
      - in: header
        name: Accept
        description: The response media type
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - List
      - Of
      - Transactions
  /api-keys:
    get:
      summary: Retrieve a list of api keys
      description: Retrieve a list of api keys
      operationId: retrieve-a-list-of-api-keys
      x-api-path-slug: apikeys-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - List
      - Of
      - Api
      - Keys
  /checkout-pages:
    get:
      summary: Retrieve a list of checkout pages
      description: Retrieve a list of checkout pages
      operationId: retrieve-a-list-of-checkout-pages
      x-api-path-slug: checkoutpages-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - List
      - Of
      - Checkout
      - Pages
  /custom-events:
    get:
      summary: Retrieve a list of custom events
      description: Retrieve a list of custom events
      operationId: retrieve-a-list-of-custom-events
      x-api-path-slug: customevents-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - List
      - Of
      - Custom
      - Events
  /custom-events/{id}/rules:
    get:
      summary: Retrieve a list of rules for custom event
      description: ""
      operationId: ""
      x-api-path-slug: customeventsidrules-get
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - List
      - Of
      - Rulescustom
      - Event
  /events:
    get:
      summary: Retrieve a list of existing events
      description: ""
      operationId: ""
      x-api-path-slug: events-get
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - List
      - Of
      - Existing
      - Events
  /events/{eventType}/rules:
    get:
      summary: Retrieve a list of rules for event
      description: ""
      operationId: ""
      x-api-path-slug: eventseventtyperules-get
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - List
      - Of
      - Rulesevent
  /gateway-accounts:
    get:
      summary: Retrieve a list of gateway accounts
      description: Retrieve a list of gateway accounts
      operationId: retrieve-a-list-of-gateway-accounts
      x-api-path-slug: gatewayaccounts-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - List
      - Of
      - Gateway
      - Accounts
  /layouts:
    get:
      summary: Retrieve a layout list
      description: Retrieve a layout list
      operationId: retrieve-a-layout-list
      x-api-path-slug: layouts-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - Layout
      - List
  /notes:
    get:
      summary: Retrieve a list of notes
      description: Retrieve a list of notes
      operationId: retrieve-a-list-of-notes
      x-api-path-slug: notes-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - List
      - Of
      - Notes
  /organizations:
    get:
      summary: Retrieve a list of organizations
      description: Retrieve a list of organizations
      operationId: retrieve-a-list-of-organizations
      x-api-path-slug: organizations-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - List
      - Of
      - Organizations
  /payment-cards-migrations:
    get:
      summary: Retrieve a list of payment cards ready for migration
      description: Retrieve a list of payment cards ready for migration
      operationId: retrieve-a-list-of-payment-cards-ready-for-migration
      x-api-path-slug: paymentcardsmigrations-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - List
      - Of
      - Payment
      - Cards
      - Readymigration
  /queue/custom-events:
    get:
      summary: Retrieve a list of scheduled custom events
      description: Retrieve a list of scheduled custom events
      operationId: retrieve-a-list-of-scheduled-custom-events
      x-api-path-slug: queuecustomevents-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - List
      - Of
      - Scheduled
      - Custom
      - Events
  /sessions:
    get:
      summary: Retrieve a list of sessions
      description: Retrieve a list of sessions
      operationId: retrieve-a-list-of-sessions
      x-api-path-slug: sessions-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - List
      - Of
      - Sessions
  /tracking/api:
    get:
      summary: Retrieve a list of tracking API logs
      description: ""
      operationId: ""
      x-api-path-slug: trackingapi-get
      parameters:
      - in: header
        name: Accept
        description: The response media type
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - List
      - Of
      - Tracking
      - Logs
  /tracking/subscriptions:
    get:
      summary: Retrieve a list of tracking subscription logs
      description: ""
      operationId: ""
      x-api-path-slug: trackingsubscriptions-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - List
      - Of
      - Tracking
      - Subscription
      - Logs
  /tracking/website-webhooks:
    get:
      summary: Retrieve a list of tracking webhook notifications
      description: ""
      operationId: ""
      x-api-path-slug: trackingwebsitewebhooks-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - List
      - Of
      - Tracking
      - Webhook
      - Notifications
  /users:
    get:
      summary: Retrieve a list of users
      description: Retrieve a list of users
      operationId: retrieve-a-list-of-users
      x-api-path-slug: users-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - List
      - Of
      - Users
  /webhooks:
    get:
      summary: Retrieve a list of webhooks
      description: Retrieve a list of webhooks
      operationId: retrieve-a-list-of-webhooks
      x-api-path-slug: webhooks-get
      parameters:
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - List
      - Of
      - Webhooks
  /websites:
    get:
      summary: Retrieve a list of websites
      description: Retrieve a list of websites
      operationId: retrieve-a-list-of-websites
      x-api-path-slug: websites-get
      parameters:
      - in: header
        name: Accept
        description: The response media type
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Retrieve
      - List
      - Of
      - Websites
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