{
  "info": {
    "name": "Urban Airship Post Airmail Send",
    "_postman_id": "abceffa0-28bc-4973-b4aa-4b3b5435d88c",
    "description": "Sends a message. All fields except message are optional, but at least one of tags, users or aliases must be specified. Much like the push API, we have a batch API call that can make sending multiple messages easier. It’s located at /api/airmail/send/batch/ and accepts a list of messages in the same format as the standard push call.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Airmail",
      "item": [
        {
          "id": "1a085ef7-b60d-4d9b-96bc-6048e5607151",
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
            "description": "Sends a message. All fields except message are optional, but at least one of tags, users or aliases must be specified. Much like the push API, we have a batch API call that can make sending multiple messages easier. It’s located at /api/airmail/send/batch/ and accepts a list of messages in the same format as the standard push call."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "678dc377-2d05-47a7-aa68-429cd5e59d07"
            }
          ]
        }
      ]
    }
  ]
}