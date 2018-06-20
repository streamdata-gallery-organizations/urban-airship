{
  "info": {
    "name": "Urban Airship Get Device Tokens Device Token Tags",
    "_postman_id": "868f8f4a-8513-4645-83f7-6f93805a290b",
    "description": "Gets tags for a specific device token.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Tags",
      "item": [
        {
          "id": "6db07b02-5767-4736-a7c0-19fa70a52129",
          "name": "tags.get",
          "request": {
            "url": "http://go.urbanairship.com/api/tags?feed_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns all the tags that you have created."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "184de0c1-cbc3-4ca0-87e3-ac29890bf54f"
            }
          ]
        },
        {
          "id": "e5344af5-f583-4241-8300-13e4f1f305b3",
          "name": "tags.tag.put",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.urbanairship.com",
              "path": [
                "api",
                "tags/:tag"
              ],
              "variable": [
                {
                  "id": "tag",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a tag."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "32bb5bdf-a502-4f8d-a0f2-93870a688f34"
            }
          ]
        },
        {
          "id": "1bf1e48f-9e38-419b-8d78-897aa34d0ba7",
          "name": "tags.tag.post",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.urbanairship.com",
              "path": [
                "api",
                "tags/:tag"
              ],
              "variable": [
                {
                  "id": "tag",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
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
            "description": "Modifies device tokens on a tag."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4af07be5-2541-4e1d-b078-e5f3eedaf67e"
            }
          ]
        }
      ]
    },
    {
      "name": "Device",
      "item": [
        {
          "id": "55f859bb-a48b-4532-9423-2672a7be713a",
          "name": "device_tokens.device_token.tags.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.urbanairship.com",
              "path": [
                "api",
                "device_tokens/:device_token/tags"
              ],
              "variable": [
                {
                  "id": "device_token",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets tags for a specific device token."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "739935dc-5647-4009-bb9a-157e5ef40d58"
            }
          ]
        }
      ]
    }
  ]
}