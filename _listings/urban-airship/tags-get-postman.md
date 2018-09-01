{
  "info": {
    "name": "Urban Airship Get Tags",
    "_postman_id": "bd20a438-69ce-4327-b50b-35b5d26e3d2a",
    "description": "Returns all the tags that you have created.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Tags",
      "item": [
        {
          "id": "527b13c4-8cbf-4caf-8fc6-b5690f6a7c3d",
          "name": "tags.get",
          "request": {
            "url": "http://go.urbanairship.com/api/tags?feed_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns all the tags that you have created."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "325d85ca-05d1-4a0c-93de-b817ed478b08"
            }
          ]
        }
      ]
    }
  ]
}