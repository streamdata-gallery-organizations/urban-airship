{
  "info": {
    "name": "Urban Airship Get User User Subscription Content",
    "_postman_id": "ae732335-75da-403f-8212-ba4051ef8276",
    "description": "Returns a list of available content.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "App",
      "item": [
        {
          "id": "d878f1a2-557b-448f-8845-e26ebf9f155a",
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
              "id": "f566cd37-2920-4f49-9875-7152036ac7e4"
            }
          ]
        },
        {
          "id": "fa586ac6-4602-405f-8f8c-6dcc98048c41",
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
            "description": "Returns a temporary URL where the client can download the content. In the payload, the receipt string is the receipt data from the purchase. It should be unaltered from how Apple delivers it to your application.udid is an optional field to help identify a particular user’s purchases, which can aid debugging. It should always be a hash of the UDID, not the actual UDID, to ensure compliance with Apple’s TOS. The optional version field should be the StoreFront library version, or custom if you’re building your own."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f2242826-eee4-4ed7-bba6-6655c5501129"
            }
          ]
        }
      ]
    },
    {
      "name": "User",
      "item": [
        {
          "id": "3a77a447-d3bc-4a24-b5b0-1c2f97663861",
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
              "id": "f7e1b598-0999-4fd9-ad06-32ea9e2bcc03"
            }
          ]
        }
      ]
    }
  ]
}