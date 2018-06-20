{
  "info": {
    "name": "Urban Airship Get Device Tokens Token",
    "_postman_id": "e374ca04-a27a-4c87-8278-ff9ff67f417e",
    "description": "Gets a device token’s alias.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Device",
      "item": [
        {
          "id": "e512f89a-1c09-4a99-a184-3f5bbec72aa8",
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
              "id": "5110c40f-554c-4fe2-b6db-afea4de5b5ae"
            }
          ]
        },
        {
          "id": "360d267c-3cf6-4f4b-8c62-2f0e192ab17b",
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
              "id": "fa3b5ad7-c58e-4348-9efb-87864f47c4d2"
            }
          ]
        }
      ]
    }
  ]
}