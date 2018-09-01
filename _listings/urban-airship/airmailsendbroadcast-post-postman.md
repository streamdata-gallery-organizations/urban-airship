{
  "info": {
    "name": "Urban Airship Post Airmail Send Broadcast",
    "_postman_id": "412c7b37-0708-4f2d-9efa-1007061e2ca1",
    "description": "Sends a message to all users (broadcast). Only message is required. The message will be sent out to every registered user. Badge numbers will be handled automatically as long as the push key is present.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Airmail",
      "item": [
        {
          "id": "cd9677af-6f84-4b44-b7be-22325b3ebc97",
          "name": "airmail.send.post",
          "request": {
            "url": "http://go.urbanairship.com/api/airmail/send",
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
            "description": "Sends a message. All fields except message are optional, but at least one of tags, users or aliases must be specified. Much like the push API, we have a batch API call that can make sending multiple messages easier. It???s located at /api/airmail/send/batch/ and accepts a list of messages in the same format as the standard push call."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "16475c45-f5b7-4102-9599-bb792b255932"
            }
          ]
        },
        {
          "id": "eeeda3d6-7ab2-4545-9ecd-97ae3e643cdf",
          "name": "airmail.send.broadcast.post",
          "request": {
            "url": "http://go.urbanairship.com/api/airmail/send/broadcast?Content-Type=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Sends a message to all users (broadcast). Only message is required. The message will be sent out to every registered user. Badge numbers will be handled automatically as long as the push key is present."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d30db656-052b-4e47-aca7-45c1122dd790"
            }
          ]
        }
      ]
    }
  ]
}