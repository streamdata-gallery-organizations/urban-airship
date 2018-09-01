{
  "info": {
    "name": "Urban Airship Get Device Tokens Count",
    "_postman_id": "bca99b52-e89f-4eb6-94ac-cd295fc62245",
    "description": "Gets the number of device tokens you have registered.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Device",
      "item": [
        {
          "id": "5765bfb2-89ec-41ac-adc4-407cd73b44d9",
          "name": "device_tokens.count.get",
          "request": {
            "url": "http://go.urbanairship.com/api/device_tokens/count?limit=%7B%7D&page=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets the number of device tokens you have registered."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6b65a90e-c08f-4da6-96e5-705287ce7bbd"
            }
          ]
        }
      ]
    }
  ]
}