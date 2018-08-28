{
  "info": {
    "name": "Kaltura VPaaS Get Service Businessprocessnotification Businessprocessserver Action List",
    "_postman_id": "66c39da3-67c5-4ae5-80b5-6cd50374f9ad",
    "description": "list Business-Process server objects",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Service",
      "item": [
        {
          "id": "04e7a650-8be3-4a5d-94f0-cf609469b4e4",
          "name": "businessProcessCase.abort",
          "request": {
            "url": "http://www.kaltura.com/api_v3/service/businessprocessnotification_businessprocesscase/action/abort?businessProcessStartNotificationTemplateId=%7B%7D&No Name=%7B%7D&objectId=%7B%7D&objectType=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Abort business-process case"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4c7ce7cb-dcac-482d-91c5-bf46a91f17ae"
            }
          ]
        },
        {
          "id": "04e070b1-576b-4e67-bd04-7e73cd72ced8",
          "name": "businessProcessCase.list",
          "request": {
            "url": "http://www.kaltura.com/api_v3/service/businessprocessnotification_businessprocesscase/action/list?No Name=%7B%7D&objectId=%7B%7D&objectType=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "list business-process cases"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1c0e0297-e11a-4252-8dfc-7e1ee4a8bf49"
            }
          ]
        },
        {
          "id": "0c3c88c8-64e3-42d2-83e7-a38c19c0a791",
          "name": "businessProcessCase.serveDiagram",
          "request": {
            "url": "http://www.kaltura.com/api_v3/service/businessprocessnotification_businessprocesscase/action/serveDiagram?businessProcessStartNotificationTemplateId=%7B%7D&No Name=%7B%7D&objectId=%7B%7D&objectType=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Server business-process case diagram"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "99bf0c1a-e1da-431d-bd15-60d837d54d1e"
            }
          ]
        },
        {
          "id": "22d31c5c-99c6-431c-8d50-a5af5292f8c0",
          "name": "businessProcessServer.add",
          "request": {
            "url": "http://www.kaltura.com/api_v3/service/businessprocessnotification_businessprocessserver/action/add?businessProcessServer[dc]=%7B%7D&businessProcessServer[description]=%7B%7D&businessProcessServer[host]=%7B%7D&businessProcessServer[name]=%7B%7D&businessProcessServer[objectType]=%7B%7D&businessProcessServer[password]=%7B%7D&businessProcessServer[port]=%7B%7D&businessProcessServer[protocol]=%7B%7D&businessProcessServer[systemName]=%7B%7D&businessProcessServer[username]=%7B%7D&No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Allows you to add a new Business-Process server object"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ba587a57-20d2-4514-8ffc-1eaaf59c6774"
            }
          ]
        },
        {
          "id": "07e0d339-f8d4-4a28-9566-ccef9cdc93a6",
          "name": "businessProcessServer.delete",
          "request": {
            "url": "http://www.kaltura.com/api_v3/service/businessprocessnotification_businessprocessserver/action/delete?id=%7B%7D&No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Delete an Business-Process server object"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "116ca7f6-e850-4d86-b1e9-b22e4cf96f47"
            }
          ]
        },
        {
          "id": "d9695bef-f27c-4db1-b514-09f07bea894b",
          "name": "businessProcessServer.get",
          "request": {
            "url": "http://www.kaltura.com/api_v3/service/businessprocessnotification_businessprocessserver/action/get?id=%7B%7D&No Name=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieve an Business-Process server object by id"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f4d50855-83fc-4297-9c0b-9e4aade4616e"
            }
          ]
        },
        {
          "id": "8248cd7d-7a1d-4f21-8235-8fd8c97bba50",
          "name": "businessProcessServer.list",
          "request": {
            "url": "http://www.kaltura.com/api_v3/service/businessprocessnotification_businessprocessserver/action/list?filter[advancedSearch][attribute]=%7B%7D&filter[advancedSearch][categoriesMatchOr]=%7B%7D&filter[advancedSearch][categoryEntryStatusIn]=%7B%7D&filter[advancedSearch][categoryIdEqual]=%7B%7D&filter[advancedSearch][comparison]=%7B%7D&filter[advancedSearch][contentLike]=%7B%7D&filter[advancedSearch][contentMultiLikeAnd]=%7B%7D&filter[advancedSearch][contentMultiLikeOr]=%7B%7D&filter[advancedSearch][cuePointsFreeText]=%7B%7D&filter[advancedSearch][cuePointSubTypeEqual]=%7B%7D&filter[advancedSearch][cuePointTypeIn]=%7B%7D&filter[advancedSearch][depthGreaterThanEqual]=%7B%7D&filter[advancedSearch][distributionProfileId]=%7B%7D&filter[advancedSearch][distributionSunStatus]=%7B%7D&filter[advancedSearch][entryDistributionFlag]=%7B%7D&filter[advancedSearch][entryDistributionStatus]=%7B%7D&filter[advancedSearch][entryDistributionValidationErrors]=%7B%7D&filter[advancedSearch][extendedStatusEqual]=%7B%7D&filter[advancedSearch][extendedStatusIn]=%7B%7D&filter[advancedSearch][field]=%7B%7D&filter[advancedSearch][hasEntryDistributionValidationErrors]=%7B%7D&filter[advancedSearch][idEqual]=%7B%7D&filter[advancedSearch][idIn]=%7B%7D&filter[advancedSearch][indexIdGreaterThan]=%7B%7D&filter[advancedSearch][isQuiz]=%7B%7D&filter[advancedSearch][items]=%7B%7D&filter[advancedSearch][memberIdEq]=%7B%7D&filter[advancedSearch][memberIdIn]=%7B%7D&filter[advancedSearch][memberPermissionsMatchAnd]=%7B%7D&filter[advancedSearch][memberPermissionsMatchOr]=%7B%7D&filter[advancedSearch][metadataProfileId]=%7B%7D&filter[advancedSearch][noDistributionProfiles]=%7B%7D&filter[advancedSearch][not]=%7B%7D&filter[advancedSearch][objectType]=%7B%7D&filter[advancedSearch][orderBy]=%7B%7D&filter[advancedSearch][type]=%7B%7D&filter[advancedSearch][updatedAtGreaterThanOrEqual]=%7B%7D&filter[advancedSearch][updatedAtLessThanOrEqual]=%7B%7D&filter[advancedSearch][userIdEqual]=%7B%7D&filter[advancedSearch][userIdIn]=%7B%7D&filter[advancedSearch][value]=%7B%7D&filter[advancedSearch][watermarkId]=%7B%7D&filter[createdAtGreaterThanOrEqual]=%7B%7D&filter[createdAtLessThanOrEqual]=%7B%7D&filter[currentDcOrExternal]=%7B%7D&filter[currentDc]=%7B%7D&filter[dcEqOrNull]=%7B%7D&filter[dcEqual]=%7B%7D&filter[idEqual]=%7B%7D&filter[idIn]=%7B%7D&filter[idNotIn]=%7B%7D&filter[objectType]=%7B%7D&filter[orderBy]=%7B%7D&filter[partnerIdEqual]=%7B%7D&filter[partnerIdIn]=%7B%7D&filter[statusEqual]=%7B%7D&filter[statusIn]=%7B%7D&filter[statusNotEqual]=%7B%7D&filter[statusNotIn]=%7B%7D&filter[typeEqual]=%7B%7D&filter[typeIn]=%7B%7D&filter[updatedAtGreaterThanOrEqual]=%7B%7D&filter[updatedAtLessThanOrEqual]=%7B%7D&No Name=%7B%7D&pager[pageIndex]=%7B%7D&pager[pageSize]=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "list Business-Process server objects"
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1d84a943-e905-4797-a5b0-e3089056353f"
            }
          ]
        }
      ]
    }
  ]
}