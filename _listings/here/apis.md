---
name: HERE
x-slug: here
description: HERE Technologies enables people, enterprises and cities around the world
  to harness the power of location and create innovative solutions that make our lives
  safer and more efficient. We transform information from devices, vehicles, infrastructure
  and...
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20089-here-maps.jpg
x-kinRank: "7"
x-alexaRank: "3011"
tags: Lists
created: "2018-08-27"
modified: "2018-08-27"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/here/apis.md
specificationVersion: "0.14"
apis:
- name: Public Transport API - All Next Departures for a list of Stations
  x-api-slug: metarouterrestboardservicev1multiboardby-stopids-json-get
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
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20089-here-maps.jpg
  humanURL: https://developer.here.com
  baseURL: https://cit.transit.api.here.com//
  tags: Technology, Mobile, internet, API Provider, Profiles, General Data, Relative
    Data, Maps
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/here/metarouterrestboardservicev1multiboardby-stopids-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/here/metarouterrestboardservicev1multiboardby-stopids-json-get-openapi.md
- name: Public Transport API - All Next Departures for a list of Stations
  x-api-slug: metarouterrestboardservicev1multiboardby-stopids-json-get
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
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20089-here-maps.jpg
  humanURL: https://developer.here.com
  baseURL: https://cit.transit.api.here.com//
  tags: Technology, Mobile, internet, API Provider, Profiles, General Data, Relative
    Data, Maps
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/here/metarouterrestboardservicev1multiboardby-stopids-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/here/metarouterrestboardservicev1multiboardby-stopids-json-get-openapi.md
- name: Public Transport API - All Next Departures for a list of Stations
  x-api-slug: metarouterrestboardservicev1multiboardby-stopids-json-get
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
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20089-here-maps.jpg
  humanURL: https://developer.here.com
  baseURL: https://cit.transit.api.here.com//
  tags: Technology, Mobile, internet, API Provider, Profiles, General Data, Relative
    Data, Maps
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/here/metarouterrestboardservicev1multiboardby-stopids-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/here/metarouterrestboardservicev1multiboardby-stopids-json-get-openapi.md
- name: Public Transport API - All Next Departures for a list of Stations
  x-api-slug: metarouterrestboardservicev1multiboardby-stopids-json-get
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
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20089-here-maps.jpg
  humanURL: https://developer.here.com
  baseURL: https://cit.transit.api.here.com//
  tags: Technology, Mobile, internet, API Provider, Profiles, General Data, Relative
    Data, Maps
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/here/metarouterrestboardservicev1multiboardby-stopids-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/here/metarouterrestboardservicev1multiboardby-stopids-json-get-openapi.md
- name: Public Transport API - All Next Departures for a list of Stations
  x-api-slug: metarouterrestboardservicev1multiboardby-stopids-json-get
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
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20089-here-maps.jpg
  humanURL: https://developer.here.com
  baseURL: https://cit.transit.api.here.com//
  tags: Technology, Mobile, internet, API Provider, Profiles, General Data, Relative
    Data, Maps
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/here/metarouterrestboardservicev1multiboardby-stopids-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/here/metarouterrestboardservicev1multiboardby-stopids-json-get-openapi.md
- name: Public Transport API - All Next Departures for a list of Stations
  x-api-slug: metarouterrestboardservicev1multiboardby-stopids-json-get
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
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/20089-here-maps.jpg
  humanURL: https://developer.here.com
  baseURL: https://cit.transit.api.here.com//
  tags: Technology, Mobile, internet, API Provider, Profiles, General Data, Relative
    Data, Maps
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/here/metarouterrestboardservicev1multiboardby-stopids-json-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/lists/master/_listings/here/metarouterrestboardservicev1multiboardby-stopids-json-get-openapi.md
x-common:
- type: x-blog-rss
  url: https://developer.here.com/blog/feed
- type: x-github
  url: https://github.com/heremaps
- type: x-postman-collection
  url: https://github.com/heremaps/postman-collections
- type: x-api-gallery
  url: http://healthcare.gov.api.gallery.streamdata.io
- type: x-api-stack
  url: http://here.stack.network
- type: x-blog
  url: https://developer.here.com/blog
- type: x-crunchbase
  url: https://crunchbase.com/organization/here-inc
- type: x-developer
  url: https://developer.here.com
- type: x-email
  url: dirk.popp@here.com
- type: x-email
  url: sebastian.kurme@here.com
- type: x-email
  url: jordan.stark@here.com
- type: x-email
  url: amy.stupavsky@here.com
- type: x-email
  url: minna.laub@here.com
- type: x-email
  url: stefanie.sirc@here.com
- type: x-email
  url: rachel.kuta@here.com
- type: x-email
  url: laurel.davis-lyons@here.com
- type: x-email
  url: linda.bradley@here.com
- type: x-email
  url: press@here.com
- type: x-twitter
  url: https://twitter.com/here
- type: x-website
  url: https://here.com
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---