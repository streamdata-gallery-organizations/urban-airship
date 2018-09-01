{
  "info": {
    "name": "Urban Airship Get Feeds Feed",
    "_postman_id": "8fa4710c-7b69-4a96-b919-9c23d5d6e5d3",
    "description": "Returns information about a particular feed.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Feeds",
      "item": [
        {
          "id": "5e8ab1c0-588b-4a05-8e44-07115de48e9a",
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
              "id": "c1270774-8b7c-403c-9dd2-9d509d7594cf"
            }
          ]
        },
        {
          "id": "4d71eef0-6eab-4888-9263-b9f7cd094c75",
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
              "id": "d93439fd-1b4f-47fc-a182-69f62366ab3e"
            }
          ]
        },
        {
          "id": "8d15119e-9a43-456f-85ef-ad35d54ad23f",
          "name": "feeds.feed_id.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.urbanairship.com",
              "path": [
                "api",
                "feeds/:feed_id"
              ],
              "variable": [
                {
                  "id": "feed_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns information about a particular feed."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "64662914-735b-4ba6-bc75-9b5f2ff0d095"
            }
          ]
        }
      ]
    }
  ]
}