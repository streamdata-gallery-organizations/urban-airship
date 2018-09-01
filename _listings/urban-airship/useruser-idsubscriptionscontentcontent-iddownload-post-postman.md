{
  "info": {
    "name": "Urban Airship Post User User Subscriptions Content Content Download",
    "_postman_id": "1dc2717d-f098-4831-b96d-f07a8f3ec453",
    "description": "Downloads the content.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "App",
      "item": [
        {
          "id": "111014fa-0f63-4045-8a18-51953fea285d",
          "name": "app.content.get",
          "request": {
            "url": "http://go.urbanairship.com/api/app/content?Content-Type=%7B%7D&user_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets the store inventory."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8615c5c8-df58-42cc-8556-790071e32a9c"
            }
          ]
        },
        {
          "id": "1c3f4e75-2c0b-474d-9528-b96dba66f003",
          "name": "app.content.product_id.download.post",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.urbanairship.com",
              "path": [
                "api",
                "app/content/:product_id/download"
              ],
              "variable": [
                {
                  "id": "product_id",
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
            "description": "Returns a temporary URL where the client can download the content. In the payload, the receipt string is the receipt data from the purchase. It should be unaltered from how Apple delivers it to your application.udid is an optional field to help identify a particular user???s purchases, which can aid debugging. It should always be a hash of the UDID, not the actual UDID, to ensure compliance with Apple???s TOS. The optional version field should be the StoreFront library version, or custom if you???re building your own."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0cd88660-a8fc-46ab-8a54-ca114b23bce1"
            }
          ]
        }
      ]
    },
    {
      "name": "User",
      "item": [
        {
          "id": "e5f5b0dc-abc0-4b17-9736-b527bb523c00",
          "name": "user.user_id.subscription_content.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.urbanairship.com",
              "path": [
                "api",
                "user/:user_id/subscription_content"
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of available content."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "05062519-d326-4564-826f-39e4251e492e"
            }
          ]
        },
        {
          "id": "10c95485-53e8-4b6e-921f-89e52e0a0659",
          "name": "user.user_id.subscriptions.content.content_id.download.post",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.urbanairship.com",
              "path": [
                "api",
                "user/:user_id/subscriptions/content/:content_id/download"
              ],
              "variable": [
                {
                  "id": "content_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "user_id",
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
            "description": "Downloads the content."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1aa0fae6-7b0d-487c-b269-17049b6de0a7"
            }
          ]
        }
      ]
    }
  ]
}