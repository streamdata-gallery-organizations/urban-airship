{
  "info": {
    "name": "Urban Airship Get Feeds",
    "_postman_id": "f0075d58-a03f-43c6-8500-0d2caff03bae",
    "description": "Gets a list of feeds.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Feeds",
      "item": [
        {
          "id": "3413ed61-f297-4d81-bb3f-ff868bd2937f",
          "name": "feeds.get",
          "request": {
            "url": "http://go.urbanairship.com/api/feeds?Content-Type=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets a list of feeds."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a740b66b-2ec3-42b1-924c-3ddf493a3074"
            }
          ]
        },
        {
          "id": "16df73b3-ff7a-4004-a264-85ddb6a46bd5",
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
              "id": "9584965d-f9bc-46ff-84ec-3549c4db7321"
            }
          ]
        }
      ]
    }
  ]
}