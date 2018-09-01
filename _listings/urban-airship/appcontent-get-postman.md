{
  "info": {
    "name": "Urban Airship Get App Content",
    "_postman_id": "aea07869-eb58-4daf-80a1-1c5d5d42b23f",
    "description": "Gets the store inventory.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "App",
      "item": [
        {
          "id": "0749d6be-9f6d-4463-83a4-33d99c35de4d",
          "name": "app.content.get",
          "request": {
            "url": "http://go.urbanairship.com/api/app/content?Content-Type=%7B%7D&user_id=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets the store inventory."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7e234a5a-a98f-4ecf-aed2-4868c62a9e25"
            }
          ]
        }
      ]
    }
  ]
}