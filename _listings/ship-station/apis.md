---
name: Ship Station
x-slug: ship-station
description: ShipStation is a web-based shipping solution that streamlines the order
  fulfillment process for your online business. ShipStation consolidates orders from
  over 70 ecommerce channels, creates shipping labels, packing slips, and pick lists
  in batch, communicates tracking information to your customers, provides endless
  automation, filters, and views, wireless printing, a mobile app, and a lot more.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
x-kinRank: "7"
x-alexaRank: "0"
tags: Lists
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/ship-station/apis.md
specificationVersion: "0.14"
apis:
- name: Ship Station Developer Portal - List Tags
  x-api-slug: accountslisttags-get
  description: Lists all tags defined for this account.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
  humanURL: http://bit.ly/_ShipStation
  baseURL: https://ssapi.shipstation.com//
  tags: Shipping, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/ship-station/accountslisttags-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/ship-station/accountslisttags-get-openapi.md
- name: Ship Station Developer Portal - List Carriers
  x-api-slug: carriers-get
  description: Lists all shipping providers connected to this account.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
  humanURL: http://bit.ly/_ShipStation
  baseURL: https://ssapi.shipstation.com//
  tags: Shipping, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/ship-station/carriers-get-openapi.md
- name: Ship Station Developer Portal - List Packages
  x-api-slug: carrierslistpackagescarriercodecarriercode-get
  description: Retrieves a list of packages for the specified carrier
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
  humanURL: http://bit.ly/_ShipStation
  baseURL: https://ssapi.shipstation.com//
  tags: Shipping, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/ship-station/carrierslistpackagescarriercodecarriercode-get-openapi.md
- name: Ship Station Developer Portal - List Services
  x-api-slug: carrierslistservicescarriercodecarriercode-get
  description: Retrieves the list of available shipping services provided by the specified
    carrier
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
  humanURL: http://bit.ly/_ShipStation
  baseURL: https://ssapi.shipstation.com//
  tags: Shipping, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/ship-station/carrierslistservicescarriercodecarriercode-get-openapi.md
- name: Ship Station Developer Portal - List Customers
  x-api-slug: customersstatecodestatecodecountrycodecountrycodetagidtagidmarketplaceidmarketplaceidsortbysortbysortdirsortdirpagepagepagesizepagesize-get
  description: Obtains a list of customers that match the specified criteria.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
  humanURL: http://bit.ly/_ShipStation
  baseURL: https://ssapi.shipstation.com//
  tags: Shipping, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/ship-station/customersstatecodestatecodecountrycodecountrycodetagidtagidmarketplaceidmarketplaceidsortbysortbysortdirsortdirpagepagepagesizepagesize-get-openapi.md
- name: Ship Station Developer Portal - List Fulfillments w/o parameters
  x-api-slug: fulfillments-get
  description: ""
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
  humanURL: http://bit.ly/_ShipStation
  baseURL: https://ssapi.shipstation.com//
  tags: Shipping, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/ship-station/fulfillments-get-openapi.md
- name: Ship Station Developer Portal - List Fulfillments with parameters
  x-api-slug: fulfillmentsfulfillmentidfulfillmentidorderidorderidordernumberordernumbertrackingnumbertrackingnumberrecipientnamerecipientnamecreatedatestartcreatedatestartcreatedateendcreatedateendshipdatestartshipdatestartshipda-get
  description: |-
    Obtains a list of fulfillments that match the specified criteria.  Please note the following:

    - Orders that have been marked as shipped either through the UI or the API will appear in the response as they are considered fulfillments.

    All of the available filters are optional.  They do not need to be included in the URL.  If you do include them, here's what the URL may look like:

    Url format with filters:

    ```
    fulfillments?fulfillmentId={fulfillmentId}
    &orderId={orderId}
    &orderNumber={orderNumber}
    &trackingNumber={trackingNumber}
    &recipientName={recipientName}
    &createDateStart={createDateStart}
    &createDateEnd={createDateEnd}
    &shipDateStart={shipDateStart}
    &shipDateEnd={shipDateEnd}
    &sortBy={sortBy}
    &sortDir={sortDir}
    &page={page}
    &pageSize={pageSize}
    ```
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
  humanURL: http://bit.ly/_ShipStation
  baseURL: https://ssapi.shipstation.com//
  tags: Shipping, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/ship-station/fulfillmentsfulfillmentidfulfillmentidorderidorderidordernumberordernumbertrackingnumbertrackingnumberrecipientnamerecipientnamecreatedatestartcreatedatestartcreatedateendcreatedateendshipdatestartshipdatestartshipda-get-openapi.md
- name: Ship Station Developer Portal - List Orders w/o parameters
  x-api-slug: orders-get
  description: ""
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
  humanURL: http://bit.ly/_ShipStation
  baseURL: https://ssapi.shipstation.com//
  tags: Shipping, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/ship-station/orders-get-openapi.md
- name: Ship Station Developer Portal - List Orders by Tag
  x-api-slug: orderslistbytagorderstatusorderstatustagidtagidpagepagepagesizepagesize-get
  description: |-
    Lists all orders that match the specified status and tag ID.

    Url format with filters:

    ```
    /listbytag?orderStatus={orderStatus}
    &tagId={tagId}
    &page={page}
    &pageSize={pageSize}
    ```
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
  humanURL: http://bit.ly/_ShipStation
  baseURL: https://ssapi.shipstation.com//
  tags: Shipping, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/ship-station/orderslistbytagorderstatusorderstatustagidtagidpagepagepagesizepagesize-get-openapi.md
- name: Ship Station Developer Portal - List Orders with parameters
  x-api-slug: orderscustomernamecustomernameitemkeyworditemkeywordcreatedatestartcreatedatestartcreatedateendcreatedateendmodifydatestartmodifydatestartmodifydateendmodifydateendorderdatestartorderdatestartorderdateendorderdateend-get
  description: |-
    Obtains a list of orders that match the specified criteria.  All of the available filters are optional.  They do not need to be included in the URL.  If you do include them, here's what the URL may look like:

    Url format with filters:

    ```
    /orders?customerName={customerName}
    &itemKeyword={itemKeyword}
    &createDateStart={createDateStart}
    &createDateEnd={createDateEnd}
    &modifyDateStart={modifyDateStart}
    &modifyDateEnd={modifyDateEnd}
    &orderDateStart={orderDateStart}
    &orderDateEnd={orderDateEnd}
    &orderNumber={orderNumber}
    &orderStatus={orderStatus}
    &paymentDateStart={paymentDateStart}
    &paymentDateEnd={paymentDateEnd}
    &storeId={storeId}
    &sortBy={sortBy}
    &sortDir={sortDir}
    &page={page}
    &pageSize={pageSize}
    ```
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
  humanURL: http://bit.ly/_ShipStation
  baseURL: https://ssapi.shipstation.com//
  tags: Shipping, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/ship-station/orderscustomernamecustomernameitemkeyworditemkeywordcreatedatestartcreatedatestartcreatedateendcreatedateendmodifydatestartmodifydatestartmodifydateendmodifydateendorderdatestartorderdatestartorderdateendorderdateend-get-openapi.md
- name: Ship Station Developer Portal - List Products w/o parameters
  x-api-slug: products-get
  description: ""
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
  humanURL: http://bit.ly/_ShipStation
  baseURL: https://ssapi.shipstation.com//
  tags: Shipping, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/ship-station/products-get-openapi.md
- name: Ship Station Developer Portal - List Products with parameters
  x-api-slug: productsskuskunamenameproductcategoryidproductcategoryidproducttypeidproducttypeidtagidtagidstartdatestartdateenddateenddateshowinactiveshowinactivesortbysortbysortdirsortdirpagepagepagesizepagesize-get
  description: |-
    Obtains a list of products that match the specified criteria.  All of the available filters are optional.  They do not need to be included in the URL.  If you do include them, here's what the URL may look like:

    Url format with filters:

    ```
    /products?sku={sku}
    &name={name}
    &productCategoryId={productCategoryId}
    &productTypeId={productTypeId}
    &tagId={tagId}
    &startDate={startDate}
    &endDate={endDate}
    &showInactive={showInactive}
    &sortBy={sortBy}
    &sortDir={sortDir}
    &page={page}
    &pageSize={pageSize}
    ```
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
  humanURL: http://bit.ly/_ShipStation
  baseURL: https://ssapi.shipstation.com//
  tags: Shipping, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/ship-station/productsskuskunamenameproductcategoryidproductcategoryidproducttypeidproducttypeidtagidtagidstartdatestartdateenddateenddateshowinactiveshowinactivesortbysortbysortdirsortdirpagepagepagesizepagesize-get-openapi.md
- name: Ship Station Developer Portal - List Shipments w/o parameters
  x-api-slug: shipments-get
  description: ""
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
  humanURL: http://bit.ly/_ShipStation
  baseURL: https://ssapi.shipstation.com//
  tags: Shipping, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/ship-station/shipments-get-openapi.md
- name: Ship Station Developer Portal - List Shipments with parameters
  x-api-slug: shipmentsrecipientnamerecipientnamerecipientcountrycoderecipientcountrycodeordernumberordernumberorderidorderidcarriercodecarriercodeservicecodeservicecodetrackingnumbertrackingnumbercreatedatestartcreatedatestartcre-get
  description: |-
    Obtains a list of shipments that match the specified criteria.  Please note the following:

    - Only valid shipments with labels generated in ShipStation will be returned in the response. Orders that have been marked as shipped either through the UI or the API will not appear as they are considered external shipments.

    - To include every shipment's associated shipmentItems in the response, be sure to set the `includeShipmentItems` parameter to `true`.

    All of the available filters are optional.  They do not need to be included in the URL.  If you do include them, here's what the URL may look like:

    Url format with filters:

    ```
    shipments?recipientName={recipientName}
    &recipientCountryCode={recipientCountryCode}
    &orderNumber={orderNumber}
    &orderId={orderId}
    &carrierCode={carrierCode}
    &serviceCode={serviceCode}
    &trackingNumber={trackingNumber}
    &createDateStart={createDateStart}
    &createDateEnd={createDateEnd}
    &shipDateStart={shipDateStart}
    &shipDateEnd={shipDateEnd}
    &voidDateStart={voidDateStart}
    &voidDateEnd={voidDateEnd}
    &includeShipmentItems={includeShipmentItems}
    &sortBy={sortBy}
    &sortDir={sortDir}
    &page={page}
    &pageSize={pageSize}
    ```
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
  humanURL: http://bit.ly/_ShipStation
  baseURL: https://ssapi.shipstation.com//
  tags: Shipping, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/ship-station/shipmentsrecipientnamerecipientnamerecipientcountrycoderecipientcountrycodeordernumberordernumberorderidorderidcarriercodecarriercodeservicecodeservicecodetrackingnumbertrackingnumbercreatedatestartcreatedatestartcre-get-openapi.md
- name: Ship Station Developer Portal - List Marketplaces
  x-api-slug: storesmarketplaces-get
  description: Lists the marketplaces that can be integrated with ShipStation.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
  humanURL: http://bit.ly/_ShipStation
  baseURL: https://ssapi.shipstation.com//
  tags: Shipping, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/ship-station/storesmarketplaces-get-openapi.md
- name: Ship Station Developer Portal - List Stores
  x-api-slug: storesshowinactiveshowinactivemarketplaceidmarketplaceid-get
  description: Retrieve the list of installed stores on the account.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
  humanURL: http://bit.ly/_ShipStation
  baseURL: https://ssapi.shipstation.com//
  tags: Shipping, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/ship-station/storesshowinactiveshowinactivemarketplaceidmarketplaceid-get-openapi.md
- name: Ship Station Developer Portal - List Users
  x-api-slug: usersshowinactiveshowinactive-get
  description: ""
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
  humanURL: http://bit.ly/_ShipStation
  baseURL: https://ssapi.shipstation.com//
  tags: Shipping, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/ship-station/usersshowinactiveshowinactive-get-openapi.md
- name: Ship Station Developer Portal - List Warehouses
  x-api-slug: warehouses-get
  description: Retrieves a list of your Ship From Locations (formerly known as warehouses).
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
  humanURL: http://bit.ly/_ShipStation
  baseURL: https://ssapi.shipstation.com//
  tags: Shipping, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/ship-station/warehouses-get-openapi.md
- name: Ship Station Developer Portal - List Webhooks
  x-api-slug: webhooks-get
  description: Retrieves a list of registered webhooks for the account
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
  humanURL: http://bit.ly/_ShipStation
  baseURL: https://ssapi.shipstation.com//
  tags: Shipping, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/ship-station/webhooks-get-openapi.md
- name: Ship Station Developer Portal - List Webhooks
  x-api-slug: webhooks-get
  description: Retrieves a list of registered webhooks for the account
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
  humanURL: http://bit.ly/_ShipStation
  baseURL: https://ssapi.shipstation.com//
  tags: Shipping, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/ship-station/webhooks-get-openapi.md
- name: Ship Station Developer Portal - List Webhooks
  x-api-slug: webhooks-get
  description: Retrieves a list of registered webhooks for the account
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
  humanURL: http://bit.ly/_ShipStation
  baseURL: https://ssapi.shipstation.com//
  tags: Shipping, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/ship-station/webhooks-get-openapi.md
- name: Ship Station Developer Portal - List Warehouses
  x-api-slug: warehouses-get
  description: Retrieves a list of your Ship From Locations (formerly known as warehouses).
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
  humanURL: http://bit.ly/_ShipStation
  baseURL: https://ssapi.shipstation.com//
  tags: Shipping, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/ship-station/warehouses-get-openapi.md
- name: Ship Station Developer Portal - List Warehouses
  x-api-slug: warehouses-get
  description: Retrieves a list of your Ship From Locations (formerly known as warehouses).
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
  humanURL: http://bit.ly/_ShipStation
  baseURL: https://ssapi.shipstation.com//
  tags: Shipping, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/ship-station/warehouses-get-openapi.md
- name: Ship Station Developer Portal - List Users
  x-api-slug: usersshowinactiveshowinactive-get
  description: ""
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
  humanURL: http://bit.ly/_ShipStation
  baseURL: https://ssapi.shipstation.com//
  tags: Shipping, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/ship-station/usersshowinactiveshowinactive-get-openapi.md
- name: Ship Station Developer Portal - List Users
  x-api-slug: usersshowinactiveshowinactive-get
  description: ""
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
  humanURL: http://bit.ly/_ShipStation
  baseURL: https://ssapi.shipstation.com//
  tags: Shipping, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/ship-station/usersshowinactiveshowinactive-get-openapi.md
- name: Ship Station Developer Portal - List Stores
  x-api-slug: storesshowinactiveshowinactivemarketplaceidmarketplaceid-get
  description: Retrieve the list of installed stores on the account.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
  humanURL: http://bit.ly/_ShipStation
  baseURL: https://ssapi.shipstation.com//
  tags: Shipping, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/ship-station/storesshowinactiveshowinactivemarketplaceidmarketplaceid-get-openapi.md
- name: Ship Station Developer Portal - List Stores
  x-api-slug: storesshowinactiveshowinactivemarketplaceidmarketplaceid-get
  description: Retrieve the list of installed stores on the account.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
  humanURL: http://bit.ly/_ShipStation
  baseURL: https://ssapi.shipstation.com//
  tags: Shipping, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/ship-station/storesshowinactiveshowinactivemarketplaceidmarketplaceid-get-openapi.md
- name: Ship Station Developer Portal - List Marketplaces
  x-api-slug: storesmarketplaces-get
  description: Lists the marketplaces that can be integrated with ShipStation.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
  humanURL: http://bit.ly/_ShipStation
  baseURL: https://ssapi.shipstation.com//
  tags: Shipping, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/ship-station/storesmarketplaces-get-openapi.md
- name: Ship Station Developer Portal - List Marketplaces
  x-api-slug: storesmarketplaces-get
  description: Lists the marketplaces that can be integrated with ShipStation.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
  humanURL: http://bit.ly/_ShipStation
  baseURL: https://ssapi.shipstation.com//
  tags: Shipping, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/ship-station/storesmarketplaces-get-openapi.md
- name: Ship Station Developer Portal - List Shipments with parameters
  x-api-slug: shipmentsrecipientnamerecipientnamerecipientcountrycoderecipientcountrycodeordernumberordernumberorderidorderidcarriercodecarriercodeservicecodeservicecodetrackingnumbertrackingnumbercreatedatestartcreatedatestartcre-get
  description: |-
    Obtains a list of shipments that match the specified criteria.  Please note the following:

    - Only valid shipments with labels generated in ShipStation will be returned in the response. Orders that have been marked as shipped either through the UI or the API will not appear as they are considered external shipments.

    - To include every shipment's associated shipmentItems in the response, be sure to set the `includeShipmentItems` parameter to `true`.

    All of the available filters are optional.  They do not need to be included in the URL.  If you do include them, here's what the URL may look like:

    Url format with filters:

    ```
    shipments?recipientName={recipientName}
    &recipientCountryCode={recipientCountryCode}
    &orderNumber={orderNumber}
    &orderId={orderId}
    &carrierCode={carrierCode}
    &serviceCode={serviceCode}
    &trackingNumber={trackingNumber}
    &createDateStart={createDateStart}
    &createDateEnd={createDateEnd}
    &shipDateStart={shipDateStart}
    &shipDateEnd={shipDateEnd}
    &voidDateStart={voidDateStart}
    &voidDateEnd={voidDateEnd}
    &includeShipmentItems={includeShipmentItems}
    &sortBy={sortBy}
    &sortDir={sortDir}
    &page={page}
    &pageSize={pageSize}
    ```
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
  humanURL: http://bit.ly/_ShipStation
  baseURL: https://ssapi.shipstation.com//
  tags: Shipping, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/ship-station/shipmentsrecipientnamerecipientnamerecipientcountrycoderecipientcountrycodeordernumberordernumberorderidorderidcarriercodecarriercodeservicecodeservicecodetrackingnumbertrackingnumbercreatedatestartcreatedatestartcre-get-openapi.md
- name: Ship Station Developer Portal - List Shipments with parameters
  x-api-slug: shipmentsrecipientnamerecipientnamerecipientcountrycoderecipientcountrycodeordernumberordernumberorderidorderidcarriercodecarriercodeservicecodeservicecodetrackingnumbertrackingnumbercreatedatestartcreatedatestartcre-get
  description: |-
    Obtains a list of shipments that match the specified criteria.  Please note the following:

    - Only valid shipments with labels generated in ShipStation will be returned in the response. Orders that have been marked as shipped either through the UI or the API will not appear as they are considered external shipments.

    - To include every shipment's associated shipmentItems in the response, be sure to set the `includeShipmentItems` parameter to `true`.

    All of the available filters are optional.  They do not need to be included in the URL.  If you do include them, here's what the URL may look like:

    Url format with filters:

    ```
    shipments?recipientName={recipientName}
    &recipientCountryCode={recipientCountryCode}
    &orderNumber={orderNumber}
    &orderId={orderId}
    &carrierCode={carrierCode}
    &serviceCode={serviceCode}
    &trackingNumber={trackingNumber}
    &createDateStart={createDateStart}
    &createDateEnd={createDateEnd}
    &shipDateStart={shipDateStart}
    &shipDateEnd={shipDateEnd}
    &voidDateStart={voidDateStart}
    &voidDateEnd={voidDateEnd}
    &includeShipmentItems={includeShipmentItems}
    &sortBy={sortBy}
    &sortDir={sortDir}
    &page={page}
    &pageSize={pageSize}
    ```
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
  humanURL: http://bit.ly/_ShipStation
  baseURL: https://ssapi.shipstation.com//
  tags: Shipping, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/ship-station/shipmentsrecipientnamerecipientnamerecipientcountrycoderecipientcountrycodeordernumberordernumberorderidorderidcarriercodecarriercodeservicecodeservicecodetrackingnumbertrackingnumbercreatedatestartcreatedatestartcre-get-openapi.md
- name: Ship Station Developer Portal - List Shipments w/o parameters
  x-api-slug: shipments-get
  description: ""
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
  humanURL: http://bit.ly/_ShipStation
  baseURL: https://ssapi.shipstation.com//
  tags: Shipping, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/ship-station/shipments-get-openapi.md
- name: Ship Station Developer Portal - List Shipments w/o parameters
  x-api-slug: shipments-get
  description: ""
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
  humanURL: http://bit.ly/_ShipStation
  baseURL: https://ssapi.shipstation.com//
  tags: Shipping, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/ship-station/shipments-get-openapi.md
- name: Ship Station Developer Portal - List Products with parameters
  x-api-slug: productsskuskunamenameproductcategoryidproductcategoryidproducttypeidproducttypeidtagidtagidstartdatestartdateenddateenddateshowinactiveshowinactivesortbysortbysortdirsortdirpagepagepagesizepagesize-get
  description: |-
    Obtains a list of products that match the specified criteria.  All of the available filters are optional.  They do not need to be included in the URL.  If you do include them, here's what the URL may look like:

    Url format with filters:

    ```
    /products?sku={sku}
    &name={name}
    &productCategoryId={productCategoryId}
    &productTypeId={productTypeId}
    &tagId={tagId}
    &startDate={startDate}
    &endDate={endDate}
    &showInactive={showInactive}
    &sortBy={sortBy}
    &sortDir={sortDir}
    &page={page}
    &pageSize={pageSize}
    ```
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
  humanURL: http://bit.ly/_ShipStation
  baseURL: https://ssapi.shipstation.com//
  tags: Shipping, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/ship-station/productsskuskunamenameproductcategoryidproductcategoryidproducttypeidproducttypeidtagidtagidstartdatestartdateenddateenddateshowinactiveshowinactivesortbysortbysortdirsortdirpagepagepagesizepagesize-get-openapi.md
- name: Ship Station Developer Portal - List Products with parameters
  x-api-slug: productsskuskunamenameproductcategoryidproductcategoryidproducttypeidproducttypeidtagidtagidstartdatestartdateenddateenddateshowinactiveshowinactivesortbysortbysortdirsortdirpagepagepagesizepagesize-get
  description: |-
    Obtains a list of products that match the specified criteria.  All of the available filters are optional.  They do not need to be included in the URL.  If you do include them, here's what the URL may look like:

    Url format with filters:

    ```
    /products?sku={sku}
    &name={name}
    &productCategoryId={productCategoryId}
    &productTypeId={productTypeId}
    &tagId={tagId}
    &startDate={startDate}
    &endDate={endDate}
    &showInactive={showInactive}
    &sortBy={sortBy}
    &sortDir={sortDir}
    &page={page}
    &pageSize={pageSize}
    ```
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
  humanURL: http://bit.ly/_ShipStation
  baseURL: https://ssapi.shipstation.com//
  tags: Shipping, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/ship-station/productsskuskunamenameproductcategoryidproductcategoryidproducttypeidproducttypeidtagidtagidstartdatestartdateenddateenddateshowinactiveshowinactivesortbysortbysortdirsortdirpagepagepagesizepagesize-get-openapi.md
- name: Ship Station Developer Portal - List Products w/o parameters
  x-api-slug: products-get
  description: ""
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
  humanURL: http://bit.ly/_ShipStation
  baseURL: https://ssapi.shipstation.com//
  tags: Shipping, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/ship-station/products-get-openapi.md
- name: Ship Station Developer Portal - List Products w/o parameters
  x-api-slug: products-get
  description: ""
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
  humanURL: http://bit.ly/_ShipStation
  baseURL: https://ssapi.shipstation.com//
  tags: Shipping, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/ship-station/products-get-openapi.md
- name: Ship Station Developer Portal - List Orders with parameters
  x-api-slug: orderscustomernamecustomernameitemkeyworditemkeywordcreatedatestartcreatedatestartcreatedateendcreatedateendmodifydatestartmodifydatestartmodifydateendmodifydateendorderdatestartorderdatestartorderdateendorderdateend-get
  description: |-
    Obtains a list of orders that match the specified criteria.  All of the available filters are optional.  They do not need to be included in the URL.  If you do include them, here's what the URL may look like:

    Url format with filters:

    ```
    /orders?customerName={customerName}
    &itemKeyword={itemKeyword}
    &createDateStart={createDateStart}
    &createDateEnd={createDateEnd}
    &modifyDateStart={modifyDateStart}
    &modifyDateEnd={modifyDateEnd}
    &orderDateStart={orderDateStart}
    &orderDateEnd={orderDateEnd}
    &orderNumber={orderNumber}
    &orderStatus={orderStatus}
    &paymentDateStart={paymentDateStart}
    &paymentDateEnd={paymentDateEnd}
    &storeId={storeId}
    &sortBy={sortBy}
    &sortDir={sortDir}
    &page={page}
    &pageSize={pageSize}
    ```
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
  humanURL: http://bit.ly/_ShipStation
  baseURL: https://ssapi.shipstation.com//
  tags: Shipping, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/ship-station/orderscustomernamecustomernameitemkeyworditemkeywordcreatedatestartcreatedatestartcreatedateendcreatedateendmodifydatestartmodifydatestartmodifydateendmodifydateendorderdatestartorderdatestartorderdateendorderdateend-get-openapi.md
- name: Ship Station Developer Portal - List Orders with parameters
  x-api-slug: orderscustomernamecustomernameitemkeyworditemkeywordcreatedatestartcreatedatestartcreatedateendcreatedateendmodifydatestartmodifydatestartmodifydateendmodifydateendorderdatestartorderdatestartorderdateendorderdateend-get
  description: |-
    Obtains a list of orders that match the specified criteria.  All of the available filters are optional.  They do not need to be included in the URL.  If you do include them, here's what the URL may look like:

    Url format with filters:

    ```
    /orders?customerName={customerName}
    &itemKeyword={itemKeyword}
    &createDateStart={createDateStart}
    &createDateEnd={createDateEnd}
    &modifyDateStart={modifyDateStart}
    &modifyDateEnd={modifyDateEnd}
    &orderDateStart={orderDateStart}
    &orderDateEnd={orderDateEnd}
    &orderNumber={orderNumber}
    &orderStatus={orderStatus}
    &paymentDateStart={paymentDateStart}
    &paymentDateEnd={paymentDateEnd}
    &storeId={storeId}
    &sortBy={sortBy}
    &sortDir={sortDir}
    &page={page}
    &pageSize={pageSize}
    ```
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
  humanURL: http://bit.ly/_ShipStation
  baseURL: https://ssapi.shipstation.com//
  tags: Shipping, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/ship-station/orderscustomernamecustomernameitemkeyworditemkeywordcreatedatestartcreatedatestartcreatedateendcreatedateendmodifydatestartmodifydatestartmodifydateendmodifydateendorderdatestartorderdatestartorderdateendorderdateend-get-openapi.md
- name: Ship Station Developer Portal - List Orders by Tag
  x-api-slug: orderslistbytagorderstatusorderstatustagidtagidpagepagepagesizepagesize-get
  description: |-
    Lists all orders that match the specified status and tag ID.

    Url format with filters:

    ```
    /listbytag?orderStatus={orderStatus}
    &tagId={tagId}
    &page={page}
    &pageSize={pageSize}
    ```
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
  humanURL: http://bit.ly/_ShipStation
  baseURL: https://ssapi.shipstation.com//
  tags: Shipping, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/ship-station/orderslistbytagorderstatusorderstatustagidtagidpagepagepagesizepagesize-get-openapi.md
- name: Ship Station Developer Portal - List Orders by Tag
  x-api-slug: orderslistbytagorderstatusorderstatustagidtagidpagepagepagesizepagesize-get
  description: |-
    Lists all orders that match the specified status and tag ID.

    Url format with filters:

    ```
    /listbytag?orderStatus={orderStatus}
    &tagId={tagId}
    &page={page}
    &pageSize={pageSize}
    ```
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
  humanURL: http://bit.ly/_ShipStation
  baseURL: https://ssapi.shipstation.com//
  tags: Shipping, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/ship-station/orderslistbytagorderstatusorderstatustagidtagidpagepagepagesizepagesize-get-openapi.md
- name: Ship Station Developer Portal - List Orders w/o parameters
  x-api-slug: orders-get
  description: ""
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
  humanURL: http://bit.ly/_ShipStation
  baseURL: https://ssapi.shipstation.com//
  tags: Shipping, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/ship-station/orders-get-openapi.md
- name: Ship Station Developer Portal - List Orders w/o parameters
  x-api-slug: orders-get
  description: ""
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
  humanURL: http://bit.ly/_ShipStation
  baseURL: https://ssapi.shipstation.com//
  tags: Shipping, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/ship-station/orders-get-openapi.md
- name: Ship Station Developer Portal - List Fulfillments with parameters
  x-api-slug: fulfillmentsfulfillmentidfulfillmentidorderidorderidordernumberordernumbertrackingnumbertrackingnumberrecipientnamerecipientnamecreatedatestartcreatedatestartcreatedateendcreatedateendshipdatestartshipdatestartshipda-get
  description: |-
    Obtains a list of fulfillments that match the specified criteria.  Please note the following:

    - Orders that have been marked as shipped either through the UI or the API will appear in the response as they are considered fulfillments.

    All of the available filters are optional.  They do not need to be included in the URL.  If you do include them, here's what the URL may look like:

    Url format with filters:

    ```
    fulfillments?fulfillmentId={fulfillmentId}
    &orderId={orderId}
    &orderNumber={orderNumber}
    &trackingNumber={trackingNumber}
    &recipientName={recipientName}
    &createDateStart={createDateStart}
    &createDateEnd={createDateEnd}
    &shipDateStart={shipDateStart}
    &shipDateEnd={shipDateEnd}
    &sortBy={sortBy}
    &sortDir={sortDir}
    &page={page}
    &pageSize={pageSize}
    ```
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
  humanURL: http://bit.ly/_ShipStation
  baseURL: https://ssapi.shipstation.com//
  tags: Shipping, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/ship-station/fulfillmentsfulfillmentidfulfillmentidorderidorderidordernumberordernumbertrackingnumbertrackingnumberrecipientnamerecipientnamecreatedatestartcreatedatestartcreatedateendcreatedateendshipdatestartshipdatestartshipda-get-openapi.md
- name: Ship Station Developer Portal - List Fulfillments with parameters
  x-api-slug: fulfillmentsfulfillmentidfulfillmentidorderidorderidordernumberordernumbertrackingnumbertrackingnumberrecipientnamerecipientnamecreatedatestartcreatedatestartcreatedateendcreatedateendshipdatestartshipdatestartshipda-get
  description: |-
    Obtains a list of fulfillments that match the specified criteria.  Please note the following:

    - Orders that have been marked as shipped either through the UI or the API will appear in the response as they are considered fulfillments.

    All of the available filters are optional.  They do not need to be included in the URL.  If you do include them, here's what the URL may look like:

    Url format with filters:

    ```
    fulfillments?fulfillmentId={fulfillmentId}
    &orderId={orderId}
    &orderNumber={orderNumber}
    &trackingNumber={trackingNumber}
    &recipientName={recipientName}
    &createDateStart={createDateStart}
    &createDateEnd={createDateEnd}
    &shipDateStart={shipDateStart}
    &shipDateEnd={shipDateEnd}
    &sortBy={sortBy}
    &sortDir={sortDir}
    &page={page}
    &pageSize={pageSize}
    ```
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
  humanURL: http://bit.ly/_ShipStation
  baseURL: https://ssapi.shipstation.com//
  tags: Shipping, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/ship-station/fulfillmentsfulfillmentidfulfillmentidorderidorderidordernumberordernumbertrackingnumbertrackingnumberrecipientnamerecipientnamecreatedatestartcreatedatestartcreatedateendcreatedateendshipdatestartshipdatestartshipda-get-openapi.md
- name: Ship Station Developer Portal - List Fulfillments w/o parameters
  x-api-slug: fulfillments-get
  description: ""
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
  humanURL: http://bit.ly/_ShipStation
  baseURL: https://ssapi.shipstation.com//
  tags: Shipping, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/ship-station/fulfillments-get-openapi.md
- name: Ship Station Developer Portal - List Fulfillments w/o parameters
  x-api-slug: fulfillments-get
  description: ""
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
  humanURL: http://bit.ly/_ShipStation
  baseURL: https://ssapi.shipstation.com//
  tags: Shipping, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/ship-station/fulfillments-get-openapi.md
- name: Ship Station Developer Portal - List Customers
  x-api-slug: customersstatecodestatecodecountrycodecountrycodetagidtagidmarketplaceidmarketplaceidsortbysortbysortdirsortdirpagepagepagesizepagesize-get
  description: Obtains a list of customers that match the specified criteria.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
  humanURL: http://bit.ly/_ShipStation
  baseURL: https://ssapi.shipstation.com//
  tags: Shipping, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/ship-station/customersstatecodestatecodecountrycodecountrycodetagidtagidmarketplaceidmarketplaceidsortbysortbysortdirsortdirpagepagepagesizepagesize-get-openapi.md
- name: Ship Station Developer Portal - List Customers
  x-api-slug: customersstatecodestatecodecountrycodecountrycodetagidtagidmarketplaceidmarketplaceidsortbysortbysortdirsortdirpagepagepagesizepagesize-get
  description: Obtains a list of customers that match the specified criteria.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
  humanURL: http://bit.ly/_ShipStation
  baseURL: https://ssapi.shipstation.com//
  tags: Shipping, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/ship-station/customersstatecodestatecodecountrycodecountrycodetagidtagidmarketplaceidmarketplaceidsortbysortbysortdirsortdirpagepagepagesizepagesize-get-openapi.md
- name: Ship Station Developer Portal - List Services
  x-api-slug: carrierslistservicescarriercodecarriercode-get
  description: Retrieves the list of available shipping services provided by the specified
    carrier
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
  humanURL: http://bit.ly/_ShipStation
  baseURL: https://ssapi.shipstation.com//
  tags: Shipping, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/ship-station/carrierslistservicescarriercodecarriercode-get-openapi.md
- name: Ship Station Developer Portal - List Services
  x-api-slug: carrierslistservicescarriercodecarriercode-get
  description: Retrieves the list of available shipping services provided by the specified
    carrier
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
  humanURL: http://bit.ly/_ShipStation
  baseURL: https://ssapi.shipstation.com//
  tags: Shipping, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/ship-station/carrierslistservicescarriercodecarriercode-get-openapi.md
- name: Ship Station Developer Portal - List Packages
  x-api-slug: carrierslistpackagescarriercodecarriercode-get
  description: Retrieves a list of packages for the specified carrier
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
  humanURL: http://bit.ly/_ShipStation
  baseURL: https://ssapi.shipstation.com//
  tags: Shipping, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/ship-station/carrierslistpackagescarriercodecarriercode-get-openapi.md
- name: Ship Station Developer Portal - List Packages
  x-api-slug: carrierslistpackagescarriercodecarriercode-get
  description: Retrieves a list of packages for the specified carrier
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
  humanURL: http://bit.ly/_ShipStation
  baseURL: https://ssapi.shipstation.com//
  tags: Shipping, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/ship-station/carrierslistpackagescarriercodecarriercode-get-openapi.md
- name: Ship Station Developer Portal - List Carriers
  x-api-slug: carriers-get
  description: Lists all shipping providers connected to this account.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
  humanURL: http://bit.ly/_ShipStation
  baseURL: https://ssapi.shipstation.com//
  tags: Shipping, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/ship-station/carriers-get-openapi.md
- name: Ship Station Developer Portal - List Carriers
  x-api-slug: carriers-get
  description: Lists all shipping providers connected to this account.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
  humanURL: http://bit.ly/_ShipStation
  baseURL: https://ssapi.shipstation.com//
  tags: Shipping, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/ship-station/carriers-get-openapi.md
- name: Ship Station Developer Portal - List Tags
  x-api-slug: accountslisttags-get
  description: Lists all tags defined for this account.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
  humanURL: http://bit.ly/_ShipStation
  baseURL: https://ssapi.shipstation.com//
  tags: Shipping, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/ship-station/accountslisttags-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/ship-station/accountslisttags-get-openapi.md
- name: Ship Station Developer Portal - List Tags
  x-api-slug: accountslisttags-get
  description: Lists all tags defined for this account.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/ShipStation-stacked-blue.png
  humanURL: http://bit.ly/_ShipStation
  baseURL: https://ssapi.shipstation.com//
  tags: Shipping, Relative Data, Service API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/ship-station/accountslisttags-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/ship-station/accountslisttags-get-openapi.md
x-common:
- type: x-website
  url: http://bit.ly/_ShipStation
- type: x-api-gallery
  url: http://server.density.api.gallery.streamdata.io
- type: x-api-stack
  url: http://ship.station.stack.network
- type: x-blog
  url: https://www.shipstation.com/blog/
- type: x-developer
  url: https://shipstation.docs.apiary.io/#
- type: x-github
  url: https://github.com/shipstation
- type: x-partners
  url: https://www.shipstation.com/partners/
- type: x-pricing
  url: https://www.shipstation.com/pricing/
- type: x-twitter
  url: https://twitter.com/ShipStation
- type: x-website
  url: http://shipstation.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---