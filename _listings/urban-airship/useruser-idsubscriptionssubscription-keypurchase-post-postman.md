{
  "info": {
    "name": "Urban Airship Post User User Subscriptions Subscription Key Purchase",
    "_postman_id": "ec1033f2-a388-4e82-95e4-1be905a97d2b",
    "description": "Adds a new subscription.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "User",
      "item": [
        {
          "id": "f653734c-c07f-449e-9767-97e7d0057581",
          "name": "user.user_id.available_subscriptions.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.urbanairship.com",
              "path": [
                "api",
                "user/:user_id/available_subscriptions"
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
            "description": "Retrieves subscription options."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "344819a6-90d3-4ada-a40d-54e907d3f788"
            }
          ]
        },
        {
          "id": "7c326dd9-2ffe-45e1-ae4d-cc2662a20aa8",
          "name": "user.user_id.subscriptions.subscription_key.purchase.post",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.urbanairship.com",
              "path": [
                "api",
                "user/:user_id/subscriptions/:subscription_key/purchase"
              ],
              "variable": [
                {
                  "id": "subscription_key",
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
            "description": "Adds a new subscription."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b0389664-fd51-453e-a8d8-5d40269d502c"
            }
          ]
        }
      ]
    }
  ]
}