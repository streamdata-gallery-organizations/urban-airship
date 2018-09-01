{
  "info": {
    "name": "Urban Airship Put Feeds Feed",
    "_postman_id": "88c98d59-a56b-4555-a362-cbe5e7ba8978",
    "description": "Updates a feed.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Feeds",
      "item": [
        {
          "id": "9bf8a0d3-b99e-4404-918d-8c98b63e904b",
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
              "id": "ea1bf1e7-beca-4cba-8dcf-4b239228810b"
            }
          ]
        },
        {
          "id": "78d945cc-a5da-468f-9b00-d47c0c0d59b6",
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
              "id": "f043cb40-09ba-4424-96af-8fa69bfd3b15"
            }
          ]
        },
        {
          "id": "28529992-2a6c-4156-a1e6-afd6d2f285a2",
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
              "id": "0b1ae289-d333-4e16-b216-d76df2a6b666"
            }
          ]
        },
        {
          "id": "8dc6a75e-6df0-4023-88f8-9708dc627522",
          "name": "feeds.feed_id.put",
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
            "method": "PUT",
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
            "description": "Updates a feed."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bfa84b65-b8da-4653-94ac-b11d2272808d"
            }
          ]
        }
      ]
    }
  ]
}