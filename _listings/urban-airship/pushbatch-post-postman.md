{
  "info": {
    "name": "Urban Airship Post Push Batch",
    "_postman_id": "9a4f74a1-c3a8-4431-b4d1-7c10bb1a3ce4",
    "description": "Sends a push message to all the listed PINs. Each item in the list can contain 0 or many device_pins and 0 or many aliases or tags, and the blackberry payload is in the same format as for individual pushes.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Push",
      "item": [
        {
          "id": "61f0b383-181a-4d6a-9f19-f5e79fef9942",
          "name": "push.batch.post",
          "request": {
            "url": "http://go.urbanairship.com/api/push/batch?Content-Type=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Sends a push message to all the listed PINs. Each item in the list can contain 0 or many device_pins and 0 or many aliases or tags, and the blackberry payload is in the same format as for individual pushes."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "707ee98d-56e4-4c9b-b517-786194201ee2"
            }
          ]
        }
      ]
    }
  ]
}