{
  "info": {
    "name": "Urban Airship Post Feeds",
    "_postman_id": "f1f591d6-f163-4790-80c8-e25f9f531b9c",
    "description": "Creates a new feed item.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Feeds",
      "item": [
        {
          "id": "9ee78d70-881c-4926-961b-734efa53a972",
          "name": "feeds.post",
          "request": {
            "url": "http://go.urbanairship.com/api/feeds",
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
            "description": "Creates a new feed item."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7ff9cf3f-a095-488b-b3c0-0ce99499eed7"
            }
          ]
        }
      ]
    }
  ]
}