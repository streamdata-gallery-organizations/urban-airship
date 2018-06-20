{
  "info": {
    "name": "Urban Airship Delete User User Messages Message Message",
    "_postman_id": "9e65973e-0986-4927-94d0-f374c6a98bec",
    "description": "Deletes a message.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "User",
      "item": [
        {
          "id": "be286274-c0c4-4f82-9a90-55cfd254e734",
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
              "id": "47dcaef4-c264-40a4-85cc-37fe9396a6c1"
            }
          ]
        },
        {
          "id": "12912ab4-fa83-4b8d-a624-e49ab336b432",
          "name": "user.user_id.messages.unread.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.urbanairship.com",
              "path": [
                "api",
                "user/:user_id/messages/unread"
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
            "description": "Returns a list of unread message IDs and their URLs."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "33f1c45f-f531-4116-be5f-4fae28e7dccc"
            }
          ]
        },
        {
          "id": "03fd4849-281b-4e71-aaab-bc386f8e5080",
          "name": "user.user_id.messages.unread.post",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.urbanairship.com",
              "path": [
                "api",
                "user/:user_id/messages/unread"
              ],
              "variable": [
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
            "description": "Marks multiple messages as read at once. If a message has already been marked as read, it will be silently skipped."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "dc0f6d78-999c-4e2b-be2c-928756b1b810"
            }
          ]
        },
        {
          "id": "59a3e0fa-58f2-41d5-8d46-dfffb33b33d8",
          "name": "user.user_id.messages.message.message_id.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.urbanairship.com",
              "path": [
                "api",
                "user/:user_id/messages/message/:message_id"
              ],
              "variable": [
                {
                  "id": "message_id",
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
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets a message."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f444b013-3ca0-4436-bf25-61f202ba50bd"
            }
          ]
        },
        {
          "id": "ae360611-d979-413e-b609-1b255cd328fb",
          "name": "user.user_id.messages.message.message_id.delete",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.urbanairship.com",
              "path": [
                "api",
                "user/:user_id/messages/message/:message_id"
              ],
              "variable": [
                {
                  "id": "message_id",
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
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a message."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9e708dbe-02a7-4e1e-83ff-b7060696a93d"
            }
          ]
        }
      ]
    }
  ]
}