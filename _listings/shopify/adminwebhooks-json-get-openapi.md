---
swagger: "2.0"
x-collection-name: Shopify
x-complete: 0
info:
  title: Shopify Get a list of all webhooks for your shop.
  description: Get a list of all webhooks for your shop..
  version: 1.0.0
host: DefaultParameterValue:DefaultParameterValue@DefaultParameterValue.myshopify.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /admin/custom_collections.json:
    get:
      summary: Get a list of all custom collections
      description: Get a list of all custom collections.
      operationId: getAdminCustomCollections.json
      x-api-path-slug: admincustom-collections-json-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - List
      - Custom
      - Collections
  /admin/collects.json:
    get:
      summary: List all collects
      description: List all collects.
      operationId: getAdminCollects.json
      x-api-path-slug: admincollects-json-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - List
      - Collects
  /admin/blogs/62581763/articles.json:
    get:
      summary: Get a list of all articles from a certain blog
      description: Get a list of all articles from a certain blog.
      operationId: getAdminBlogs62581763Articles.json
      x-api-path-slug: adminblogs62581763articles-json-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - List
      - Articles
      - From
      - Certain
      - Blog
  /admin/blogs.json:
    get:
      summary: Get a list of all blogs
      description: Get a list of all blogs.
      operationId: getAdminBlogs.json
      x-api-path-slug: adminblogs-json-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - List
      - Blogs
  /admin/countries.json:
    get:
      summary: Get a list of all countries
      description: Get a list of all countries.
      operationId: getAdminCountries.json
      x-api-path-slug: admincountries-json-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - List
      - Countries
  /admin/fulfillment_services.json:
    get:
      summary: List your app's fulfillment services
      description: List your app's fulfillment services.
      operationId: getAdminFulfillmentServices.json
      x-api-path-slug: adminfulfillment-services-json-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - List
      - Your
      - Apps
      - Fulfillment
      - Services
  /admin/gift_cards.json:
    get:
      summary: Get a list of all gift cards
      description: Get a list of all gift cards.
      operationId: getAdminGiftCards.json
      x-api-path-slug: admingift-cards-json-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - List
      - Gift
      - Cards
  /admin/articles/tags.json:
    get:
      summary: Get a list of all the tags of articles
      description: Get a list of all the tags of articles.
      operationId: getAdminArticlesTags.json
      x-api-path-slug: adminarticlestags-json-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - List
      - Tags
      - Articles
  /admin/orders/4495703502/fulfillments.json:
    get:
      summary: Get a list of all fulfillments for an order.
      description: Get a list of all fulfillments for an order..
      operationId: getAdminOrders4495703502Fulfillments.json
      x-api-path-slug: adminorders4495703502fulfillments-json-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - List
      - Fulfillmentsan
      - Order
  /admin/events/58706658318.json:
    get:
      summary: Shows the same fields as the list action.
      description: Shows the same fields as the list action..
      operationId: getAdminEvents58706658318.json
      x-api-path-slug: adminevents58706658318-json-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Shows
      - Same
      - Fields
      - As
      - List
      - Action
  /admin/webhooks.json:
    get:
      summary: Get a list of all webhooks for your shop.
      description: Get a list of all webhooks for your shop..
      operationId: getAdminWebhooks.json
      x-api-path-slug: adminwebhooks-json-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - List
      - Webhooksyour
      - Shop
  /admin/carrier_services.json:
    get:
      summary: List carrier services
      description: List carrier services.
      operationId: getAdminCarrierServices.json
      x-api-path-slug: admincarrier-services-json-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - List
      - Carrier
      - Services
  /admin/pages.json:
    get:
      summary: Get a list of all pages
      description: Get a list of all pages.
      operationId: getAdminPages.json
      x-api-path-slug: adminpages-json-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - List
      - Pages
  /admin/themes/110163843/assets.json:
    get:
      summary: Get a list of all theme assets
      description: Get a list of all theme assets.
      operationId: getAdminThemes110163843Assets.json
      x-api-path-slug: adminthemes110163843assets-json-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - List
      - Theme
      - Assets
  /admin/comments.json:
    get:
      summary: Get a list of all comments
      description: Get a list of all comments.
      operationId: getAdminComments.json
      x-api-path-slug: admincomments-json-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - List
      - Comments
  /admin/discounts.json:
    get:
      summary: List all discounts
      description: List all discounts.
      operationId: getAdminDiscounts.json
      x-api-path-slug: admindiscounts-json-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - List
      - Discounts
  /admin/locations.json:
    get:
      summary: Get a list of all locations for a shop
      description: Get a list of all locations for a shop.
      operationId: getAdminLocations.json
      x-api-path-slug: adminlocations-json-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - List
      - Locationsa
      - Shop
  /admin/checkouts.json:
    get:
      summary: List all abandoned checkouts
      description: List all abandoned checkouts.
      operationId: getAdminCheckouts.json
      x-api-path-slug: admincheckouts-json-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - List
      - Abandoned
      - Checkouts
  /admin/redirects.json:
    get:
      summary: Get a list of all URL redirect
      description: Get a list of all url redirect.
      operationId: getAdminRedirects.json
      x-api-path-slug: adminredirects-json-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - List
      - URL
      - Redirect
  /admin/orders/4528049998/fulfillments/3770145678/events.json:
    get:
      summary: Get a list of all fulfillment events for a fulfillment
      description: Get a list of all fulfillment events for a fulfillment.
      operationId: getAdminOrders4528049998Fulfillments3770145678Events.json
      x-api-path-slug: adminorders4528049998fulfillments3770145678events-json-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - List
      - Fulfillment
      - Eventsa
      - Fulfillment
  /admin/script_tags.json:
    get:
      summary: Get a list of all script tags
      description: Get a list of all script tags.
      operationId: getAdminScriptTags.json
      x-api-path-slug: adminscript-tags-json-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - List
      - Script
      - Tags
  /admin/articles/authors.json:
    get:
      summary: Get a list of all the authors of articles
      description: Get a list of all the authors of articles.
      operationId: getAdminArticlesAuthors.json
      x-api-path-slug: adminarticlesauthors-json-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - List
      - Authors
      - Articles
  /admin/shipping_zones.json:
    get:
      summary: Show list of shipping zones
      description: Show list of shipping zones.
      operationId: getAdminShippingZones.json
      x-api-path-slug: adminshipping-zones-json-get
      parameters:
      - in: header
        name: Content-Type
      responses:
        200:
          description: OK
      tags:
      - Commerce
      - Show
      - List
      - Shipping
      - Zones
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