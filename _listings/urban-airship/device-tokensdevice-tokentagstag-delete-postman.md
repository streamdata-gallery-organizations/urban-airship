{
  "info": {
    "name": "Urban Airship Delete Device Tokens Device Token Tags Tag",
    "_postman_id": "adf829a3-d82f-439d-a60e-58a9add0c5e4",
    "description": "Removes a single tag from a device token.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Tags",
      "item": [
        {
          "id": "5c38b874-0652-44af-9e24-8da6f70700c2",
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
              "id": "51ba6d1f-69fe-427d-8ccb-04504a96afb4"
            }
          ]
        },
        {
          "id": "857086cd-a5ba-4b20-8c5c-39e6754ffa82",
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
              "id": "ffe5bb71-d8bd-48f0-952b-2e6f08b8a652"
            }
          ]
        },
        {
          "id": "7e14729e-4f47-4765-adb4-20352711bdaf",
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
              "id": "52341790-9ef3-4e61-ab88-67d3f439a5c2"
            }
          ]
        }
      ]
    },
    {
      "name": "Device",
      "item": [
        {
          "id": "4b26e4e0-2331-4058-98eb-e669bf58041c",
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
              "id": "b7063ee5-731a-4c5c-bcaa-9c6813b68cda"
            }
          ]
        },
        {
          "id": "a187bf0e-3f9a-4caa-ae67-bb3ab8e3d1fd",
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
              "id": "6bc465d4-73d9-418a-9ab0-89fa85d80153"
            }
          ]
        },
        {
          "id": "f3600fa0-3a08-41a6-a465-74e0c57dc7ce",
          "name": "device_tokens.device_token.tags.tag.delete",
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
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Removes a single tag from a device token."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5f3b6fef-0f95-47f4-926e-f8e113e4b002"
            }
          ]
        }
      ]
    }
  ]
}