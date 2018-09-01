{
  "info": {
    "name": "Urban Airship Put Device Tokens Token",
    "_postman_id": "13b54c36-07f2-4c62-b488-4048b9ee27e1",
    "description": "Registers a device token.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Device",
      "item": [
        {
          "id": "0fdcab6e-f141-4e09-adc3-a701dc3842f3",
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
              "id": "a56d5957-9162-46d9-808a-a421889e44b0"
            }
          ]
        }
      ]
    }
  ]
}