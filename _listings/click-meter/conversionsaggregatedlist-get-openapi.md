---
swagger: "2.0"
x-collection-name: Click Meter
x-complete: 0
info:
  title: Click Meter Retrieve statistics about this customer for a timeframe related
    to a subset of conversions grouped by some temporal entity (day/week/month)
  description: Retrieve statistics about this customer for a timeframe related to
    a subset of conversions grouped by some temporal entity (day/week/month).
  contact:
    name: Api Support
    url: http://www.clickmeter.com/api
    email: api@clickmeter.com
  version: v2
host: apiv2.clickmeter.com:80
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /aggregated/list:
    get:
      summary: Retrieve statistics about this customer for a timeframe grouped by
        some temporal entity (day/week/month)
      description: Retrieve statistics about this customer for a timeframe grouped
        by some temporal entity (day/week/month).
      operationId: getAggregatedList
      x-api-path-slug: aggregatedlist-get
      parameters:
      - in: query
        name: fromDay
        description: If using a custom timeFrame you can specify the starting day
          (YYYYMMDD)
      - in: query
        name: groupBy
        description: The temporal entity you want to group by (week/month)
      - in: query
        name: timeFrame
        description: Timeframe of the request
      - in: query
        name: toDay
        description: If using a custom timeFrame you can specify the ending day (YYYYMMDD)
      responses:
        200:
          description: OK
      tags:
      - Aggregated
      - List
  /conversions/aggregated/list:
    get:
      summary: Retrieve statistics about this customer for a timeframe related to
        a subset of conversions grouped by some temporal entity (day/week/month)
      description: Retrieve statistics about this customer for a timeframe related
        to a subset of conversions grouped by some temporal entity (day/week/month).
      operationId: getConversionsAggregatedList
      x-api-path-slug: conversionsaggregatedlist-get
      parameters:
      - in: query
        name: fromDay
        description: If using a custom timeFrame you can specify the starting day
          (YYYYMMDD)
      - in: query
        name: groupBy
        description: The temporal entity you want to group by (week/month)
      - in: query
        name: status
        description: Status of conversion (deleted/active)
      - in: query
        name: timeFrame
        description: Timeframe of the request
      - in: query
        name: toDay
        description: If using a custom timeFrame you can specify the ending day (YYYYMMDD)
      responses:
        200:
          description: OK
      tags:
      - Conversions
      - Aggregated
      - List
  /conversions/{conversionId}/aggregated/list:
    get:
      summary: Retrieve statistics about this conversion for a timeframe grouped by
        some temporal entity (day/week/month)
      description: Retrieve statistics about this conversion for a timeframe grouped
        by some temporal entity (day/week/month).
      operationId: getConversionsConversionAggregatedList
      x-api-path-slug: conversionsconversionidaggregatedlist-get
      parameters:
      - in: path
        name: conversionId
        description: Id of the conversion
      - in: query
        name: fromDay
        description: If using a custom timeFrame you can specify the starting day
          (YYYYMMDD)
      - in: query
        name: groupBy
        description: The temporal entity you want to group by (week/month)
      - in: query
        name: timeFrame
        description: Timeframe of the request
      - in: query
        name: toDay
        description: If using a custom timeFrame you can specify the ending day (YYYYMMDD)
      responses:
        200:
          description: OK
      tags:
      - Conversions
      - ConversionId
      - Aggregated
      - List
  /datapoints/aggregated/list:
    get:
      summary: Retrieve statistics about all datapoints of this customer for a timeframe
        grouped by some temporal entity (day/week/month)
      description: Retrieve statistics about all datapoints of this customer for a
        timeframe grouped by some temporal entity (day/week/month).
      operationId: getDatapointsAggregatedList
      x-api-path-slug: datapointsaggregatedlist-get
      parameters:
      - in: query
        name: favourite
        description: Is the datapoint is marked as favourite
      - in: query
        name: fromDay
        description: If using a custom timeFrame you can specify the starting day
          (YYYYMMDD)
      - in: query
        name: groupBy
        description: The temporal entity you want to group by (week/month)
      - in: query
        name: status
        description: Status of datapoint (deleted/active/paused/spam)
      - in: query
        name: tag
        description: A comma separated list of tags you want to filter with
      - in: query
        name: timeFrame
        description: Timeframe of the request
      - in: query
        name: toDay
        description: If using a custom timeFrame you can specify the ending day (YYYYMMDD)
      - in: query
        name: type
        description: Type of datapoint (tl/tp)
      responses:
        200:
          description: OK
      tags:
      - Datapoints
      - Aggregated
      - List
  /datapoints/{id}/aggregated/list:
    get:
      summary: Retrieve statistics about this datapoint for a timeframe grouped by
        some temporal entity (day/week/month)
      description: Retrieve statistics about this datapoint for a timeframe grouped
        by some temporal entity (day/week/month).
      operationId: getDatapointsAggregatedList
      x-api-path-slug: datapointsidaggregatedlist-get
      parameters:
      - in: query
        name: fromDay
        description: If using a custom timeFrame you can specify the starting day
          (YYYYMMDD)
      - in: query
        name: groupBy
        description: The temporal entity you want to group by (week/month)
      - in: path
        name: id
        description: Id of the datapoint
      - in: query
        name: timeFrame
        description: Timeframe of the request
      - in: query
        name: toDay
        description: If using a custom timeFrame you can specify the ending day (YYYYMMDD)
      responses:
        200:
          description: OK
      tags:
      - Datapoints
      - Id
      - Aggregated
      - List
  /groups/aggregated/list:
    get:
      summary: Retrieve statistics about all groups of this customer for a timeframe
        grouped by some temporal entity (day/week/month)
      description: Retrieve statistics about all groups of this customer for a timeframe
        grouped by some temporal entity (day/week/month).
      operationId: getGroupsAggregatedList
      x-api-path-slug: groupsaggregatedlist-get
      parameters:
      - in: query
        name: favourite
        description: Is the group is marked as favourite
      - in: query
        name: fromDay
        description: If using a custom timeFrame you can specify the starting day
          (YYYYMMDD)
      - in: query
        name: groupBy
        description: The temporal entity you want to group by (week/month)
      - in: query
        name: status
        description: Status of group (deleted/active)
      - in: query
        name: tag
        description: A comma separated list of tags you want to filter with
      - in: query
        name: timeFrame
        description: Timeframe of the request
      - in: query
        name: toDay
        description: If using a custom timeFrame you can specify the ending day (YYYYMMDD)
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Aggregated
      - List
  /groups/{id}/aggregated/list:
    get:
      summary: Retrieve statistics about this group for a timeframe grouped by some
        temporal entity (day/week/month)
      description: Retrieve statistics about this group for a timeframe grouped by
        some temporal entity (day/week/month).
      operationId: getGroupsAggregatedList
      x-api-path-slug: groupsidaggregatedlist-get
      parameters:
      - in: query
        name: fromDay
        description: If using a custom timeFrame you can specify the starting day
          (YYYYMMDD)
      - in: query
        name: groupBy
        description: The temporal entity you want to group by (week/month)
      - in: path
        name: id
        description: Id of the group
      - in: query
        name: timeFrame
        description: Timeframe of the request
      - in: query
        name: toDay
        description: If using a custom timeFrame you can specify the ending day (YYYYMMDD)
      responses:
        200:
          description: OK
      tags:
      - Groups
      - Id
      - Aggregated
      - List
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