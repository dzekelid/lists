{
  "info": {
    "name": "LiveChat List all groups",
    "_postman_id": "310c8d19-692b-4ffc-826b-dc687773be9c",
    "description": "Returns all created groups.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Webhook",
      "item": [
        {
          "id": "94eb2ad0-abec-4935-a7e0-1c1c9c05fb4a",
          "name": "Webhooks12345Delete",
          "request": {
            "url": "http://api.livechatinc.com/webhooks/12345",
            "method": "DELETE",
            "header": [
              {
                "key": "X-API-Version",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a webhook with the given ID."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "efbc492b-cba5-4be8-85f3-538923bf96c2"
            }
          ]
        }
      ]
    },
    {
      "name": "Chat",
      "item": [
        {
          "id": "52e57ad1-07ed-48f0-9d1a-264e698dd579",
          "name": "ReportsChatsRatingsGet",
          "request": {
            "url": "http://api.livechatinc.com/reports/chats/ratings?date_from=%7B%7D&date_to=%7B%7D&group=%7B%7D&group_by=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "X-API-Version",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Shows how many chats have been rated and how they have been rated during a specified period."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5f003ca2-992b-4ad0-a23a-d6c4cf156053"
            }
          ]
        },
        {
          "id": "3cf925b7-db83-4bd0-b8cc-3215685742c4",
          "name": "ReportsChatsEngagementGet",
          "request": {
            "url": "http://api.livechatinc.com/reports/chats/engagement?agent=%7B%7D&date_from=%7B%7D&date_to=%7B%7D&group_by=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "X-API-Version",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "This report shows you where you get your chats from. They can come from i.e. automatic invitations, manual invitations or the visitors can start the chats by themselves."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c1f2b316-b2eb-4254-8128-595a69225978"
            }
          ]
        },
        {
          "id": "02b83166-f5ce-4231-9c7b-8536dc1f6b99",
          "name": "ReportsChatsRatingsRankingGet",
          "request": {
            "url": "http://api.livechatinc.com/reports/chats/ratings/ranking",
            "method": "GET",
            "header": [
              {
                "key": "X-API-Version",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Shows the ratio of good to bad ratings for each operator."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7c4f53b2-181d-4f5f-add9-ff99dbf28ab0"
            }
          ]
        }
      ]
    },
    {
      "name": "List",
      "item": [
        {
          "id": "13783ac9-6ef2-4f9c-93fe-c0b7152255a1",
          "name": "CannedResponsesABC123Get",
          "request": {
            "url": "http://api.livechatinc.com/canned_responses/ABC123",
            "method": "GET",
            "header": [
              {
                "key": "X-API-Version",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns the list of all currently set canned responses."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "778c7b39-391a-40fb-ad1a-9e3605897b2c"
            }
          ]
        },
        {
          "id": "382b5a69-048c-4428-b41d-f83c8b4aa597",
          "name": "GreetingsGet",
          "request": {
            "url": "http://api.livechatinc.com/greetings?groups=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "X-API-Version",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns the list of all greetings."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a7d82ef4-5ea2-40cb-8161-fd2e40f2e07c"
            }
          ]
        },
        {
          "id": "70131566-4833-4086-b661-f97f81280c9b",
          "name": "TagsGet",
          "request": {
            "url": "http://api.livechatinc.com/tags?group=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "X-API-Version",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns tags from all groups."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fa59faa8-649f-4add-86ea-9ecae5308aaf"
            }
          ]
        },
        {
          "id": "2bd33d05-9bd9-4104-8ce7-d448d354537e",
          "name": "TicketsGet",
          "request": {
            "url": "http://api.livechatinc.com/tickets?date_from=%7B%7D&status=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "X-API-Version",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns all tickets."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fa0b9971-d3f2-435f-8b99-82ec7ae020c3"
            }
          ]
        },
        {
          "id": "1ed73bc7-1311-436d-8076-aaec73d9fe03",
          "name": "CannedResponsesGet",
          "request": {
            "url": "http://api.livechatinc.com/canned_responses",
            "method": "GET",
            "header": [
              {
                "key": "X-API-Version",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns the list of all currently set canned responses."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c36c548f-bdb7-4fec-86c5-7c4f556bab01"
            }
          ]
        },
        {
          "id": "95e17471-c314-45d3-92f8-f249cb7b9f28",
          "name": "GroupsGet",
          "request": {
            "url": "http://api.livechatinc.com/groups",
            "method": "GET",
            "header": [
              {
                "key": "X-API-Version",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns all created groups."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3c194191-4a91-43ce-bfbd-8eba06a982c9"
            }
          ]
        }
      ]
    },
    {
      "name": "Canned",
      "item": [
        {
          "id": "306d0fcf-df46-4ffc-b760-3f9eaeede37f",
          "name": "CannedResponsesABC123Put",
          "request": {
            "url": "http://api.livechatinc.com/canned_responses/ABC123",
            "method": "PUT",
            "header": [
              {
                "key": "X-API-Version",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "tags[0]",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                }
              ]
            },
            "description": "Updates the specified canned response by setting the values of the parameters passed. Any parameters not provided will be left unchanged."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7c0d9d5d-dcf3-4741-991c-88e6ca62377b"
            }
          ]
        }
      ]
    },
    {
      "name": "Remove",
      "item": [
        {
          "id": "eddd9b42-e7a5-45eb-97f6-0549a0a0c3e1",
          "name": "CannedResponsesABC123Delete",
          "request": {
            "url": "http://api.livechatinc.com/canned_responses/ABC123",
            "method": "DELETE",
            "header": [
              {
                "key": "X-API-Version",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Removes a canned response with the given CANNED_RESPONSE_ID."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e76a0f25-6f2f-44c2-ab8a-ccd0f949dbf1"
            }
          ]
        },
        {
          "id": "24cf4ac5-7fc3-4981-be7a-e2a1fee6a1d5",
          "name": "GroupsABC123Delete2",
          "request": {
            "url": "http://api.livechatinc.com/groups/ABC123",
            "method": "DELETE",
            "header": [
              {
                "key": "X-API-Version",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Removes a group with the given GROUP_ID."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "23c60256-35c5-4a74-9626-fa98f9ca2fea"
            }
          ]
        },
        {
          "id": "911ded7f-1ddd-4be6-aa6e-9cc70b85ca9c",
          "name": "AgentsJohnPublicComDelete",
          "request": {
            "url": "http://api.livechatinc.com/agents/john@public.com",
            "method": "DELETE",
            "header": [
              {
                "key": "X-API-Version",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Removes an agent."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "abe4c79e-0b75-4e15-964c-c2d5d7e29414"
            }
          ]
        }
      ]
    },
    {
      "name": "Group",
      "item": [
        {
          "id": "024a4671-7121-4741-bd67-5a4a620f23d3",
          "name": "GroupsABC123Put",
          "request": {
            "url": "http://api.livechatinc.com/groups/ABC123",
            "method": "PUT",
            "header": [
              {
                "key": "X-API-Version",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "agents[0]",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "agents[1]",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "name",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                }
              ]
            },
            "description": "Updates the specified group by setting the values of the parameters passed. Any parameters not provided will be left unchanged."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "149d9fe6-81bb-4d65-9729-c6494eaffc18"
            }
          ]
        }
      ]
    },
    {
      "name": "New",
      "item": [
        {
          "id": "18b9e570-d1eb-44d6-a5af-3300cde170d2",
          "name": "GreetingsPost",
          "request": {
            "url": "http://api.livechatinc.com/greetings",
            "method": "POST",
            "header": [
              {
                "key": "X-API-Version",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "name",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "rules[0][operator]",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "rules[0][type]",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "rules[0][value]",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "rules[1][operator]",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "rules[1][type]",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "rules[1][value]",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                }
              ]
            },
            "description": "Use this function to create a new greeting."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3d076194-1d8e-417d-a659-3f210ab34c97"
            }
          ]
        },
        {
          "id": "cb513998-a043-4761-815d-c565ffb86b37",
          "name": "WebhooksPost",
          "request": {
            "url": "http://api.livechatinc.com/webhooks",
            "method": "POST",
            "header": [
              {
                "key": "X-API-Version",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "data_types",
                  "value": "[{}]",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "event_type",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "url",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                }
              ]
            },
            "description": "Creates a new webhook."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0d14e13e-75f6-4f0f-acf7-9936106d52ce"
            }
          ]
        },
        {
          "id": "e1777d0b-7c59-4d53-8ac3-7c66e8278f42",
          "name": "CannedResponsesPost",
          "request": {
            "url": "http://api.livechatinc.com/canned_responses",
            "method": "POST",
            "header": [
              {
                "key": "X-API-Version",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "tags[0]",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "tags[1]",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "text",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                }
              ]
            },
            "description": "Creates a new canned response."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b189591f-2456-41f6-8fdb-72efe5bd0398"
            }
          ]
        }
      ]
    },
    {
      "name": "Display",
      "item": [
        {
          "id": "3a617b5a-cd83-4881-b08a-30900477780d",
          "name": "WebhooksGet",
          "request": {
            "url": "http://api.livechatinc.com/webhooks",
            "method": "GET",
            "header": [
              {
                "key": "X-API-Version",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of webhooks that have been created in a LiveChat account."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d8ac85e8-9b94-418d-a17c-5951b6624022"
            }
          ]
        }
      ]
    },
    {
      "name": "Greetings",
      "item": [
        {
          "id": "a4c20738-1c52-40f8-b2a4-b11d0e9727f4",
          "name": "ReportsChatsGreetingsGet",
          "request": {
            "url": "http://api.livechatinc.com/reports/chats/greetings?date_from=%7B%7D&date_to=%7B%7D&group_by=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "X-API-Version",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns the “greetings to chats to goals” conversion rates report.\n\ndisplayed is the number of displayed greetings. accepted tells you how many chats resulted from these greetings. goals tells you how many goals resulted from these greetings."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e5fe0035-488d-4226-8a25-88dd4cdf47d4"
            }
          ]
        }
      ]
    },
    {
      "name": "Tag",
      "item": [
        {
          "id": "7d25a85c-dfa2-4092-8cf9-14cf608154b4",
          "name": "TagsPost",
          "request": {
            "url": "http://api.livechatinc.com/tags",
            "method": "POST",
            "header": [
              {
                "key": "X-API-Version",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "author",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "group",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "tag",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                }
              ]
            },
            "description": "Adds a new tag. Note that only the owner and the admins are authorized to use this."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5798a6ad-00cd-4c57-9196-6ea50c1fd0b2"
            }
          ]
        }
      ]
    },
    {
      "name": "Single",
      "item": [
        {
          "id": "602a2f32-2d51-4132-8ec5-86a11cd0e164",
          "name": "AgentsJohnPublicComGet",
          "request": {
            "url": "http://api.livechatinc.com/agents/john@public.com",
            "method": "GET",
            "header": [
              {
                "key": "X-API-Version",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Returns complete details of the agent for the given LOGIN."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "11d79bcc-8ad1-4516-81ff-b10fb4f348af"
            }
          ]
        },
        {
          "id": "7729d5e5-a58f-4afc-9fa4-edcdb3a6282d",
          "name": "AgentsJohnPublicComPut",
          "request": {
            "url": "http://api.livechatinc.com/agents/john@public.com",
            "method": "PUT",
            "header": [
              {
                "key": "X-API-Version",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "job_title",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                }
              ]
            },
            "description": "Returns complete details of the agent for the given LOGIN."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "481429fe-d2da-4c41-bd1a-71f588ccd469"
            }
          ]
        }
      ]
    },
    {
      "name": "Ticket",
      "item": [
        {
          "id": "3909498c-93c6-4370-8081-5c2e9be43c08",
          "name": "TicketsPost",
          "request": {
            "url": "http://api.livechatinc.com/tickets",
            "method": "POST",
            "header": [
              {
                "key": "X-API-Version",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "urlencoded",
              "urlencoded": [
                {
                  "key": "message",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "requester[mail]",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "requester[name]",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                },
                {
                  "key": "subject",
                  "value": "{}",
                  "disabled": false,
                  "description": ""
                }
              ]
            },
            "description": "Creates a new ticket."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bfbee1e1-d3b0-40d2-97e5-4a53e07153c1"
            }
          ]
        }
      ]
    },
    {
      "name": "Solved",
      "item": [
        {
          "id": "b78ab356-b0cb-4fdc-903f-3dc2e426d787",
          "name": "ReportsTicketsSolvedTicketsGet",
          "request": {
            "url": "http://api.livechatinc.com/reports/tickets/solved_tickets?date_from=%7B%7D&date_to=%7B%7D",
            "method": "GET",
            "header": [
              {
                "key": "X-API-Version",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Shows the number of the tickets solved during the specified period."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f3de2d7e-21cb-4952-a6f9-c92a6c66d0d0"
            }
          ]
        }
      ]
    },
    {
      "name": "Chats",
      "item": [
        {
          "id": "86762bf2-46e9-432d-b7df-ea1e921be49c",
          "name": "ReportsChatsFirstResponseTimeGet",
          "request": {
            "url": "http://api.livechatinc.com/reports/chats/first_response_time",
            "method": "GET",
            "header": [
              {
                "key": "X-API-Version",
                "value": "{}",
                "description": "",
                "disabled": false
              },
              {
                "key": "Accept",
                "value": "*/*",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "The average amount of time it takes the agents to respond to a new chat over a specified period of time."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f7a808a7-ed2c-450e-8c75-20913b065658"
            }
          ]
        }
      ]
    }
  ]
}