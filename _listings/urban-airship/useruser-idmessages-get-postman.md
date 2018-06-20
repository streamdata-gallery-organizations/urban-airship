{
  "info": {
    "name": "Urban Airship Get User User Messages",
    "_postman_id": "97ed5d8b-114c-4a3c-9d6c-4b62b2897544",
    "description": "Returns a list of messages and some metadata about them. It will also include some metadata about the user.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "User",
      "item": [
        {
          "id": "032425cb-2b70-4954-ad2b-f7e90acd097d",
          "name": "user.user_id.messages.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.urbanairship.com",
              "path": [
                "api",
                "user/:user_id/messages"
              ],
              "query": [
                {
                  "key": "full_list",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "since",
                  "value": "%7B%7D",
                  "disabled": false
                }
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
            "description": "Returns a list of messages and some metadata about them. It will also include some metadata about the user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9b041087-03b4-49e2-8ad7-faff19f82ce2"
            }
          ]
        }
      ]
    }
  ]
}