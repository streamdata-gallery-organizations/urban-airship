{
  "info": {
    "name": "Urban Airship Put Tags Tag",
    "_postman_id": "ea80cbd8-88e4-4d26-8505-e1bccce98971",
    "description": "Deletes a tag.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Tags",
      "item": [
        {
          "id": "990478cc-9a19-43fa-bf47-e093330b7083",
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
              "id": "a81fb4fe-90a6-47f5-b715-dc7d8cd88af2"
            }
          ]
        },
        {
          "id": "564b6bf4-b68b-4cf0-be27-be217b8dfa56",
          "name": "tags.tag.put",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.urbanairship.com",
              "path": [
                "api",
                "tags/:tag"
              ],
              "variable": [
                {
                  "id": "tag",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a tag."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4fd24d67-c1e2-4575-84cb-99253a5ed6bf"
            }
          ]
        }
      ]
    }
  ]
}