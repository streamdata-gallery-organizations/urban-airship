{
  "info": {
    "name": "Urban Airship Put Device Tokens Device Token Tags Tag",
    "_postman_id": "40d500d2-de4e-4b2a-922d-a453524957f6",
    "description": "Creates a tag and associate it with the specific device token.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Tags",
      "item": [
        {
          "id": "bb851b55-d7a8-4179-afa1-c3ca3ed4eee6",
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
              "id": "417c77ea-ef09-4a98-bf6c-7c0082957a8a"
            }
          ]
        },
        {
          "id": "e154fa6a-dfb4-46ac-8875-0b42b01ff43d",
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
              "id": "eff163c5-07a9-4406-bf5f-e284259942ba"
            }
          ]
        },
        {
          "id": "b229a1db-518b-44bc-8395-ce84c513476f",
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
              "id": "8bf0f429-b527-4bf2-914e-696b9ad8cd36"
            }
          ]
        }
      ]
    },
    {
      "name": "Device",
      "item": [
        {
          "id": "9a7983f1-d709-42e0-a515-855addd1e7a1",
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
              "id": "8bf13cc5-697f-460b-a2cd-95b0838eab6b"
            }
          ]
        },
        {
          "id": "3d97047c-4df2-473f-92de-8e38a190b8ee",
          "name": "device_tokens.device_token.tags.tag.put",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.urbanairship.com",
              "path": [
                "api",
                "device_tokens/:device_token/tags/:tag"
              ],
              "variable": [
                {
                  "id": "device_token",
                  "value": "{}",
                  "type": "string"
                },
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
            "description": "Creates a tag and associate it with the specific device token."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "36beab29-bef5-463f-98f9-12f344292c5d"
            }
          ]
        }
      ]
    }
  ]
}