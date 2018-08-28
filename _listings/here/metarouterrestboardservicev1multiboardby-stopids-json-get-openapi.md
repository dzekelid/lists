---
swagger: "2.0"
x-collection-name: HERE
x-complete: 0
info:
  title: HERE Public Transit API All Next Departures for a list of Stations
  description: "*Request a list of all next departure times and destinations for a
    give list of stations.*\n\nAll next departures for a list of stations can be requested
    using the `metarouter/rest/boardservice/v1/multiboard/by_stopIds.json` and specifying
    a `time` and `stopIds.`  \nThe maximum numbers of nearby stations and number of
    departures per station can be restricted by using the `max_stn` and `max` parameters,
    respectively.\n  \n\n\n\n* **lang**  `text`\n \\- Language of the response\n\n*
    **time**  `text`\n \\- Time in format `yyyy-mm-ddThh:mm:ss`.\n\n* **app_id**  `text`\n
    \\- A 20 bytes Base64 URL-safe encoded string used for the authentication of the
    client application.    You must include an app_code and app_code with every request.\n\n*
    **app_code**  `text`\n \\- A 20 bytes Base64 URL-safe encoded string used for
    the authentication of the client application.    You must include an app_code
    and app_code with every request.\n\n* **max**  `text`\n \\- The  maximum number
    of next departures per station to be included in the response.     The default
    value is 40.    \n\n* **max_stn**  `text`\n \\-  The maximum number of stations
    for which departures are required.     The default value is 40.    \n\n* **stopIds**
    \ `text`\n \\- Specifies a list of stopIds separated by comma. Each stopId must
    contain\n at least 6 characters and must not exceed a maximum of 1000 characters."
  version: 1.0.0
host: cit.transit.api.here.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /metarouter/rest/boardservice/v1/multiboard/by_stopids.json:
    get:
      summary: All Next Departures for a list of Stations
      description: "*Request a list of all next departure times and destinations for
        a give list of stations.*\n\nAll next departures for a list of stations can
        be requested using the `metarouter/rest/boardservice/v1/multiboard/by_stopIds.json`
        and specifying a `time` and `stopIds.`  \nThe maximum numbers of nearby stations
        and number of departures per station can be restricted by using the `max_stn`
        and `max` parameters, respectively.\n  \n\n\n\n* **lang**  `text`\n \\- Language
        of the response\n\n* **time**  `text`\n \\- Time in format `yyyy-mm-ddThh:mm:ss`.\n\n*
        **app_id**  `text`\n \\- A 20 bytes Base64 URL-safe encoded string used for
        the authentication of the client application.    You must include an app_code
        and app_code with every request.\n\n* **app_code**  `text`\n \\- A 20 bytes
        Base64 URL-safe encoded string used for the authentication of the client application.
        \   You must include an app_code and app_code with every request.\n\n* **max**
        \ `text`\n \\- The  maximum number of next departures per station to be included
        in the response.     The default value is 40.    \n\n* **max_stn**  `text`\n
        \\-  The maximum number of stations for which departures are required.     The
        default value is 40.    \n\n* **stopIds**  `text`\n \\- Specifies a list of
        stopIds separated by comma. Each stopId must contain\n at least 6 characters
        and must not exceed a maximum of 1000 characters."
      operationId: MetarouterRestBoardserviceV1MultiboardByStopidsJsonGet
      x-api-path-slug: metarouterrestboardservicev1multiboardby-stopids-json-get
      parameters:
      - in: query
        name: app_code
      - in: query
        name: app_id
      - in: query
        name: lang
      - in: query
        name: max
      - in: query
        name: max_stn
      - in: query
        name: stopIds
      - in: query
        name: time
      responses:
        200:
          description: OK
      tags:
      - All
      - Next
      - Departuresa
      - List
      - Of
      - Stations
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