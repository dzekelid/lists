---
swagger: "2.0"
x-collection-name: Vinli
x-complete: 0
info:
  title: Vinli List Dummy Routes
  description: List dummy routes.
  version: 1.0.0
host: events.vin.li
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /devices/cf217c2d-df3c-41f7-b610-8bc3e11b4b79/vehicles:
    get:
      summary: List a Device's Vehicles
      description: List a device's vehicles.
      operationId: DevicesCf217c2dDf3c41f7B6108bc3e11b4b79VehiclesGet
      x-api-path-slug: devicescf217c2ddf3c41f7b6108bc3e11b4b79vehicles-get
      parameters:
      - in: header
        name: Accept
      responses:
        200:
          description: OK
      tags:
      - List
      - Devices
      - Vehicles
  /devices/7eac0d62-854f-41c1-a5b2-ba13c460058a/collisions:
    get:
      summary: Get a List of Collisions for a Device
      description: Get a list of collisions for a device.
      operationId: Devices7eac0d62854f41c1A5b2Ba13c460058aCollisionsGet
      x-api-path-slug: devices7eac0d62854f41c1a5b2ba13c460058acollisions-get
      parameters:
      - in: header
        name: Accept
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Collisionsa
      - Device
  /vehicles/9aa35c64-b046-43cc-9cd8-4c353a6d0b30/odometer_triggers:
    get:
      summary: List all Odometer Triggers for a Vehicle
      description: List all odometer triggers for a vehicle.
      operationId: Vehicles9aa35c64B04643cc9cd84c353a6d0b30OdometerTriggersGet
      x-api-path-slug: vehicles9aa35c64b04643cc9cd84c353a6d0b30odometer-triggers-get
      parameters:
      - in: header
        name: Accept
      responses:
        200:
          description: OK
      tags:
      - List
      - ""
      - Odometer
      - Triggersa
      - Vehicle
  /vehicles/9aa35c64-b046-43cc-9cd8-4c353a6d0b30/trips:
    get:
      summary: List All of a Vehicle's Trips
      description: List all of a vehicle's trips.
      operationId: Vehicles9aa35c64B04643cc9cd84c353a6d0b30TripsGet
      x-api-path-slug: vehicles9aa35c64b04643cc9cd84c353a6d0b30trips-get
      parameters:
      - in: header
        name: Accept
      responses:
        200:
          description: OK
      tags:
      - List
      - ""
      - Of
      - Vehicles
      - Trips
  /devices:
    get:
      summary: List all devices
      description: List all devices.
      operationId: DevicesGet
      x-api-path-slug: devices-get
      responses:
        200:
          description: OK
      tags:
      - List
      - ""
      - Devices
  /vehicles/428bc621-16e7-489b-a02a-eb98526d01ef/collisions:
    get:
      summary: Get a List of Collisions for a Vehicle
      description: Get a list of collisions for a vehicle.
      operationId: Vehicles428bc62116e7489bA02aEb98526d01efCollisionsGet
      x-api-path-slug: vehicles428bc62116e7489ba02aeb98526d01efcollisions-get
      parameters:
      - in: header
        name: Accept
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - Collisionsa
      - Vehicle
  /vehicles/9aa35c64-b046-43cc-9cd8-4c353a6d0b30/odometers:
    get:
      summary: List All Odometer Reports for a Vehicle
      description: List all odometer reports for a vehicle.
      operationId: Vehicles9aa35c64B04643cc9cd84c353a6d0b30OdometersGet
      x-api-path-slug: vehicles9aa35c64b04643cc9cd84c353a6d0b30odometers-get
      parameters:
      - in: header
        name: Accept
      responses:
        200:
          description: OK
      tags:
      - List
      - ""
      - Odometer
      - Reportsa
      - Vehicle
  /dummies:
    get:
      summary: List Dummy Devices
      description: List dummy devices.
      operationId: DummiesGet
      x-api-path-slug: dummies-get
      parameters:
      - in: header
        name: Accept
      responses:
        200:
          description: OK
      tags:
      - List
      - Dummy
      - Devices
  /routes:
    get:
      summary: List Dummy Routes
      description: List dummy routes.
      operationId: RoutesGet
      x-api-path-slug: routes-get
      parameters:
      - in: header
        name: Accept
      responses:
        200:
          description: OK
      tags:
      - List
      - Dummy
      - Routes
  /vehicles/9aa35c64-b046-43cc-9cd8-4c353a6d0b30/distances:
    get:
      summary: Get list of  a Vehicles Distances
      description: Get list of  a vehicles distances.
      operationId: Vehicles9aa35c64B04643cc9cd84c353a6d0b30DistancesGet
      x-api-path-slug: vehicles9aa35c64b04643cc9cd84c353a6d0b30distances-get
      parameters:
      - in: header
        name: Accept
      responses:
        200:
          description: OK
      tags:
      - List
      - Of
      - ""
      - Vehicles
      - Distances
  /devices/cf217c2d-df3c-41f7-b610-8bc3e11b4b79/messages:
    get:
      summary: List Telemetry Messages
      description: List telemetry messages.
      operationId: DevicesCf217c2dDf3c41f7B6108bc3e11b4b79MessagesGet
      x-api-path-slug: devicescf217c2ddf3c41f7b6108bc3e11b4b79messages-get
      parameters:
      - in: header
        name: Accept
      responses:
        200:
          description: OK
      tags:
      - List
      - Telemetry
      - Messages
  /devices/cf217c2d-df3c-41f7-b610-8bc3e11b4b79/rules:
    get:
      summary: List all Rules for a Device
      description: List all rules for a device.
      operationId: DevicesCf217c2dDf3c41f7B6108bc3e11b4b79RulesGet
      x-api-path-slug: devicescf217c2ddf3c41f7b6108bc3e11b4b79rules-get
      parameters:
      - in: header
        name: Accept
      responses:
        200:
          description: OK
      tags:
      - List
      - ""
      - Rulesa
      - Device
  /vehicles/9aa35c64-b046-43cc-9cd8-4c353a6d0b30/codes:
    get:
      summary: List all DTCs for a Device
      description: List all dtcs for a device.
      operationId: Vehicles9aa35c64B04643cc9cd84c353a6d0b30CodesGet
      x-api-path-slug: vehicles9aa35c64b04643cc9cd84c353a6d0b30codes-get
      parameters:
      - in: header
        name: Accept
      responses:
        200:
          description: OK
      tags:
      - List
      - ""
      - DTCsa
      - Device
  /devices/cf217c2d-df3c-41f7-b610-8bc3e11b4b79/trips:
    get:
      summary: List All of a Device's Trips
      description: List all of a device's trips.
      operationId: DevicesCf217c2dDf3c41f7B6108bc3e11b4b79TripsGet
      x-api-path-slug: devicescf217c2ddf3c41f7b6108bc3e11b4b79trips-get
      parameters:
      - in: header
        name: Accept
      responses:
        200:
          description: OK
      tags:
      - List
      - ""
      - Of
      - Devices
      - Trips
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