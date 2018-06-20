{
  "info": {
    "name": "Urban Airship Get Device Tokens",
    "_postman_id": "b359179d-d67b-489f-a975-4a9c7461e505",
    "description": "Gets information about all of your device tokens. If your application has a large number of device tokens, we’ll paginate the request for you. By default, we paginate at 5000 device tokens. You can receive the next page simply by retrieving the URL from \"next_page\" - in this way it is easy to export all of your device tokens and all their data.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Device",
      "item": [
        {
          "id": "95b8beaa-9fd4-41b7-acad-3a5bf44a5184",
          "name": "device_tokens.token.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.urbanairship.com",
              "path": [
                "api",
                "device_tokens/:token"
              ],
              "variable": [
                {
                  "id": "token",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets a device token’s alias."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8828d362-aa45-4de4-b5a7-6e8219840119"
            }
          ]
        },
        {
          "id": "3cfeb49a-8603-4ff0-889f-4206e8b99ae3",
          "name": "device_tokens.token.put",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.urbanairship.com",
              "path": [
                "api",
                "device_tokens/:token"
              ],
              "variable": [
                {
                  "id": "token",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Registers a device token."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9c990308-c084-4ad9-8438-d6eaddf1f4b8"
            }
          ]
        },
        {
          "id": "a70ffbec-22f5-4351-8f6f-9b2322f4dee7",
          "name": "device_tokens.token.delete",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.urbanairship.com",
              "path": [
                "api",
                "device_tokens/:token"
              ],
              "variable": [
                {
                  "id": "token",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Marks the device token as inactive. No notifications will be delivered to it until a PUT is executed again. The DELETE returns HTTP 204 No Content, and needs no payload. When a token is deleted in this manner, any alias or tags will be cleared."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b205e9db-6a2b-4018-ba85-7ccfa3d37b75"
            }
          ]
        },
        {
          "id": "4ab65d7e-bef5-4305-81fd-a52d236148bd",
          "name": "device_tokens.get",
          "request": {
            "url": "http://go.urbanairship.com/api/device_tokens?limit=%7B%7D&page=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about all of your device tokens. If your application has a large number of device tokens, we’ll paginate the request for you. By default, we paginate at 5000 device tokens. You can receive the next page simply by retrieving the URL from \"next_page\" - in this way it is easy to export all of your device tokens and all their data."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "643fcbf2-c7d3-4f8d-b55a-5e7c4c6056ea"
            }
          ]
        }
      ]
    }
  ]
}