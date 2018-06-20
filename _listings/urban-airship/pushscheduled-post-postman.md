{
  "info": {
    "name": "Urban Airship Post Push Scheduled",
    "_postman_id": "d744fe86-f652-4edc-b266-305235b0a7d1",
    "description": "Bulk deletes scheduled notifications. If you include URLs or aliases for scheduled notifications that don’t exist or have already been sent, they will be ignored. Any device token in the cancel_device_tokens payload will have every notification that is sent to it removed. This will not prevent it from receiving scheduled notifications to tags or broadcast messages.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Device",
      "item": [
        {
          "id": "848ad1b3-93ca-47b2-b39c-50c5726b85ce",
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
              "id": "a79883f4-ab68-49f3-8950-7691990b9dd0"
            }
          ]
        },
        {
          "id": "0f3a478a-6c9a-466a-85b2-34de06f13b51",
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
              "id": "efda011b-3a38-4d41-8501-12144f4d7055"
            }
          ]
        },
        {
          "id": "1305e74c-4af7-40e8-a5a3-419c0e27f431",
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
              "id": "19321050-682a-448d-94f4-6158a0b14e34"
            }
          ]
        }
      ]
    },
    {
      "name": "Push",
      "item": [
        {
          "id": "d89ad2f6-3fe0-4a91-bc70-6e3c376bb5ec",
          "name": "push.post",
          "request": {
            "url": "http://go.urbanairship.com/api/push?Content-Type=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Sends a push message to one or more users. Only one of aliases, tags, or device_pins is required, but they can be mixed and matched as much as you’d like."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "27e9802b-844b-425c-8fe4-3a525d326e8e"
            }
          ]
        },
        {
          "id": "61cc0c94-9b52-4a45-b378-a020f07e8a1c",
          "name": "push.scheduled.notification.delete",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.urbanairship.com",
              "path": [
                "api",
                "push/scheduled/:notification"
              ],
              "variable": [
                {
                  "id": "notification",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Cancels a scheduled notification.  A successful delete will have an HTTP status code of 204. If the scheduled notification does not exist, has already been successfully deleted, or was sent, the status code will be 404."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a5d3c10c-e62d-4c33-8bf1-e82ab4aaafa7"
            }
          ]
        },
        {
          "id": "95324b68-4b92-4339-9793-70c27e53829e",
          "name": "push.scheduled.post",
          "request": {
            "url": "http://go.urbanairship.com/api/push/scheduled?Content-Type=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Bulk deletes scheduled notifications. If you include URLs or aliases for scheduled notifications that don’t exist or have already been sent, they will be ignored. Any device token in the cancel_device_tokens payload will have every notification that is sent to it removed. This will not prevent it from receiving scheduled notifications to tags or broadcast messages."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e57e0798-e623-4549-9152-d7c637593083"
            }
          ]
        }
      ]
    }
  ]
}