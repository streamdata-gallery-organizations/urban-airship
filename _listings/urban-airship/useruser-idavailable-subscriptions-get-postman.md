{
  "info": {
    "name": "Urban Airship Get User User Available Subscriptions",
    "_postman_id": "2ad4322a-ade4-41a2-8351-d22fdc73367e",
    "description": "Retrieves subscription options.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "User",
      "item": [
        {
          "id": "1e2e9cee-b09b-4e3d-bf6c-c285eb3f91b4",
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
              "id": "74c673ae-5b5f-437f-a6fe-512336cf66eb"
            }
          ]
        }
      ]
    }
  ]
}