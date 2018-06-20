{
  "info": {
    "name": "Urban Airship Delete Feeds Feed",
    "_postman_id": "101f7174-a5c6-41c3-baa6-8bfc271b4866",
    "description": "Deletes a feed.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Feeds",
      "item": [
        {
          "id": "ce7b7afe-9730-4ffb-bc1e-2c25a6d70a01",
          "name": "feeds.get",
          "request": {
            "url": "http://go.urbanairship.com/api/feeds?Content-Type=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets a list of feeds."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "fc9f329c-3056-43b4-a117-a3c6c7b1ddb5"
            }
          ]
        },
        {
          "id": "84523dd2-123f-4f35-9f57-5e87528a0394",
          "name": "feeds.post",
          "request": {
            "url": "http://go.urbanairship.com/api/feeds",
            "method": "POST",
            "header": [
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "Content type",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Creates a new feed item."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "770a9846-094e-48c7-be52-9721a58a4b86"
            }
          ]
        },
        {
          "id": "d958d694-853b-41a0-9337-4185aeb447a2",
          "name": "feeds.feed_id.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.urbanairship.com",
              "path": [
                "api",
                "feeds/:feed_id"
              ],
              "variable": [
                {
                  "id": "feed_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns information about a particular feed."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5cb3d571-6bb9-4676-9e94-99276a0b02cf"
            }
          ]
        },
        {
          "id": "24621e29-9239-4ec8-b551-51da97ba8aa8",
          "name": "feeds.feed_id.put",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.urbanairship.com",
              "path": [
                "api",
                "feeds/:feed_id"
              ],
              "variable": [
                {
                  "id": "feed_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "header": [
              {
                "key": "Content-Type",
                "value": "{}",
                "description": "Content type",
                "disabled": false
              }
            ],
            "body": {
              "mode": "raw"
            },
            "description": "Updates a feed."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8e41db41-78bc-4a1e-b216-cbd15716dd59"
            }
          ]
        },
        {
          "id": "36c1f765-19ca-445e-a8b4-987666e260e2",
          "name": "feeds.feed_id.delete",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.urbanairship.com",
              "path": [
                "api",
                "feeds/:feed_id"
              ],
              "variable": [
                {
                  "id": "feed_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a feed."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c7e154df-ede8-4cd5-abba-bf95d56c174e"
            }
          ]
        }
      ]
    }
  ]
}