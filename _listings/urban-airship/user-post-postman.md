{
  "info": {
    "name": "Urban Airship Post User",
    "_postman_id": "4caf8237-da11-4b42-be18-8ea7a7f34c02",
    "description": "Creates a new user and returns the credentials.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Device",
      "item": [
        {
          "id": "8d6e386d-9e8d-42af-9a33-66ef4174ca03",
          "name": "device_tokens.token.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.urbanairship.com",
              "path": [
                "api",
                "device_tokens/:token"
              ],
              "variable": [
                {
                  "id": "token",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets a device token’s alias."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "4e2ad1c4-cdf1-43e9-879d-e00c781d0043"
            }
          ]
        },
        {
          "id": "10b61a4b-869f-4d24-baea-3746cb30a2ef",
          "name": "device_tokens.token.put",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.urbanairship.com",
              "path": [
                "api",
                "device_tokens/:token"
              ],
              "variable": [
                {
                  "id": "token",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Registers a device token."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "6f6a6854-d83a-458f-8d35-86f886c32b10"
            }
          ]
        },
        {
          "id": "9630c531-6bc3-4fea-b350-7aaec42bc5a0",
          "name": "device_tokens.token.delete",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.urbanairship.com",
              "path": [
                "api",
                "device_tokens/:token"
              ],
              "variable": [
                {
                  "id": "token",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Marks the device token as inactive. No notifications will be delivered to it until a PUT is executed again. The DELETE returns HTTP 204 No Content, and needs no payload. When a token is deleted in this manner, any alias or tags will be cleared."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "34346e24-2b65-4ed6-9fc9-fbe6e96865e1"
            }
          ]
        },
        {
          "id": "19641ee7-808b-4dbd-9a81-d0ff6fc4efb5",
          "name": "device_tokens.get",
          "request": {
            "url": "http://go.urbanairship.com/api/device_tokens?limit=%7B%7D&page=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about all of your device tokens. If your application has a large number of device tokens, we’ll paginate the request for you. By default, we paginate at 5000 device tokens. You can receive the next page simply by retrieving the URL from \"next_page\" - in this way it is easy to export all of your device tokens and all their data."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "059529cc-1325-4135-bb4c-6df6afbc2bc8"
            }
          ]
        },
        {
          "id": "f2e4c56f-1278-422d-b154-9e3a7f8e3a70",
          "name": "device_tokens.count.get",
          "request": {
            "url": "http://go.urbanairship.com/api/device_tokens/count?limit=%7B%7D&page=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets the number of device tokens you have registered."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "bb5af2b9-cce7-487b-bd5c-f3841a1110b1"
            }
          ]
        },
        {
          "id": "15c111ac-f5f8-4aa7-bd46-b841b65b907d",
          "name": "device_tokens.feedback.get",
          "request": {
            "url": "http://go.urbanairship.com/api/device_tokens/feedback?since=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets what device tokens are now invalid. Apple informs us when a push notification is sent to a device that can’t receive it because the application has been uninstalled. We mark the device token as inactive and immediately stop sending notifications to that device. Once a day is a good interval for querying the feedback service, but you can do it more often to save on bandwidth from unnecessary notifications. In the response, what does marked_inactive_on mean? Apple sends a timestamp for each device token returned via the feedback service. Since a device can be off the network for a while, this can be a point in the recent past. In order to make this API work smoothly for you, we record the timestamp we marked as inactive. This means you only need to query for data since the last time you queried. Once a day is a good timeframe, or once a week for very small or infrequently used applications. A few times a day is good for applications with heavy use."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "04f606c4-7bed-41b3-9c81-4b6a23866d65"
            }
          ]
        },
        {
          "id": "a5f57ca8-64fe-4131-be57-e0c059ddeb3d",
          "name": "device_pins.pin.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.urbanairship.com",
              "path": [
                "api",
                "device_pins/:pin"
              ],
              "variable": [
                {
                  "id": "pin",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets Device PIN information."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "99f853e3-8078-4001-b843-a03ecb8ff2a6"
            }
          ]
        },
        {
          "id": "7d206d41-2ad4-435b-8c4b-740d54d0a63c",
          "name": "device_pins.pin.put",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.urbanairship.com",
              "path": [
                "api",
                "device_pins/:pin"
              ],
              "variable": [
                {
                  "id": "pin",
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
            "description": "Registers a BlackBerry PIN. This is optional, but recommended, for BlackBerry push messages. This returns HTTP 201 Created for the first registration and 200 OK for any updates. If you wish to include additional information about a device pin, for instance an alias or tags, include a JSON payload along with this request. Not including one of these keys removes it from the device pin."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "cac86735-7cf4-48e2-8385-b609da325786"
            }
          ]
        },
        {
          "id": "0e62f2b2-b191-43eb-9fee-389fadcb903a",
          "name": "device_pins.pin.delete",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.urbanairship.com",
              "path": [
                "api",
                "device_pins/:pin"
              ],
              "variable": [
                {
                  "id": "pin",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Marks a PIN as inactive. No notifications will be delivered to it until a PUT is executed again."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d6cd9540-6f88-4711-9c66-10feb1e14bcb"
            }
          ]
        }
      ]
    },
    {
      "name": "Push",
      "item": [
        {
          "id": "804679a0-9439-4cb7-8e9f-642c25ca63a9",
          "name": "push.post",
          "request": {
            "url": "http://go.urbanairship.com/api/push?Content-Type=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Sends a push message to one or more users. Only one of aliases, tags, or device_pins is required, but they can be mixed and matched as much as you’d like."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "51d5e424-3ea0-4618-b7b8-e1e5e6026292"
            }
          ]
        },
        {
          "id": "fbe174b4-d539-4f74-9426-28800d512933",
          "name": "push.scheduled.notification.delete",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.urbanairship.com",
              "path": [
                "api",
                "push/scheduled/:notification"
              ],
              "variable": [
                {
                  "id": "notification",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Cancels a scheduled notification.  A successful delete will have an HTTP status code of 204. If the scheduled notification does not exist, has already been successfully deleted, or was sent, the status code will be 404."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7eaacea4-59d9-4517-80ca-f322e5810db7"
            }
          ]
        },
        {
          "id": "4ddcdaa1-5d7d-40e2-9d82-afe958bad1db",
          "name": "push.scheduled.post",
          "request": {
            "url": "http://go.urbanairship.com/api/push/scheduled?Content-Type=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Bulk deletes scheduled notifications. If you include URLs or aliases for scheduled notifications that don’t exist or have already been sent, they will be ignored. Any device token in the cancel_device_tokens payload will have every notification that is sent to it removed. This will not prevent it from receiving scheduled notifications to tags or broadcast messages."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e561f105-567c-4b0e-8bd4-149522e7b29c"
            }
          ]
        },
        {
          "id": "566d34c2-0df4-496f-be38-2769caec2592",
          "name": "push.scheduled.alias.alias.put",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.urbanairship.com",
              "path": [
                "api",
                "push/scheduled/alias/:alias"
              ],
              "query": [
                {
                  "key": "Content-Type",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "alias",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "PUT",
            "body": {
              "mode": "raw"
            },
            "description": "Changes a scheduled notification alias. Aliases for scheduled notifications are unique per Urban Airship application, so you might want to hash the aliases with a device ID or use some other mechanism to ensure uniqueness. The only other limit is that they must be 255 characters or less."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "783d7607-6e46-4958-863a-e8bcae09477a"
            }
          ]
        },
        {
          "id": "0c91ea9e-2559-4ffc-8508-0368feb588f1",
          "name": "push.scheduled.alias.alias.delete",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.urbanairship.com",
              "path": [
                "api",
                "push/scheduled/alias/:alias"
              ],
              "variable": [
                {
                  "id": "alias",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a scheduled notification alias.  If you attempt to schedule an aliased scheduled notification with an alias that already exists for your application, it will overwrite the existing one."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ff60004f-105b-4be7-9ac2-89c5d0069405"
            }
          ]
        },
        {
          "id": "94f736df-9542-4565-8b7c-cb7b18f64eb4",
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
              "id": "24b04555-c4e9-4c90-a6e0-9d429ec7c099"
            }
          ]
        },
        {
          "id": "4014146b-5772-4277-a58a-317934c4095c",
          "name": "push.broadcast.post",
          "request": {
            "url": "http://go.urbanairship.com/api/push/broadcast?Content-Type=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Sends a push message to all active APIDs (Broadcast). Important: The maximum message size is 1024 bytes. This is calculated as the UTF-8 lengths of alert and extra fields together."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ba8623ff-039a-423f-911a-21ca23eeb93d"
            }
          ]
        },
        {
          "id": "a8e80a67-6384-4d09-8f9a-7a7f2c0f250d",
          "name": "push.stats.get",
          "request": {
            "url": "http://go.urbanairship.com/api/push/stats?end=%7B%7D&format=%7B%7D&start=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns hourly message counts for your application. By default, results are returned in JSON. For CSV, either add the header:Accept:text/csv or append &format=csv to the query string. Times are in UTC, and data is provided for each push platform (currently: iOS, BlackBerry, Android, and C2DM, in that order). The statistics system is updated every 15 minutes, so the final count for an hour will be done at the latest 15 minutes after the hour is done."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c52efcf3-db9e-49a4-b28b-f1e54c675d96"
            }
          ]
        }
      ]
    },
    {
      "name": "Apids",
      "item": [
        {
          "id": "7659a340-6494-43e6-845b-3e5aa0394b0d",
          "name": "apids.apid.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.urbanairship.com",
              "path": [
                "api",
                "apids/:apid"
              ],
              "variable": [
                {
                  "id": "apid",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets APID information."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f8b33852-2beb-46de-8fb3-24c7f5aa1671"
            }
          ]
        },
        {
          "id": "6e61ff8c-2f88-4fa6-9c1e-a872c2fc3333",
          "name": "apids.apid.put",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.urbanairship.com",
              "path": [
                "api",
                "apids/:apid"
              ],
              "variable": [
                {
                  "id": "apid",
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
            "description": "Registers an APID. Unlike registration for iOS and BlackBerry applications, basic registration tying an APID to your application happens automatically. The registration API can be used to set aliases or tags. This returns HTTP 200 OK for any updates. Registering without any body is a no-op. Not including the alias field will clear it. To clear the list of tags, set it to the empty list []. If you are registering an APID to be used with C2DM, you will also need to include a C2DM registration ID."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ea3ded0d-595a-415e-a3f6-57ca5946305b"
            }
          ]
        },
        {
          "id": "09acb95d-a6d8-4705-a8d9-e8f455323930",
          "name": "apids.apid.delete",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.urbanairship.com",
              "path": [
                "api",
                "apids/:apid"
              ],
              "variable": [
                {
                  "id": "apid",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Marks an APID as invalid. No notifications will be delivered to it until it re-registers."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c21789f6-e6ae-430e-8fd3-e6af99d4ca9c"
            }
          ]
        },
        {
          "id": "a8e9214e-8ad5-4108-9a3f-02b53cb2a37a",
          "name": "apids.get",
          "request": {
            "url": "http://go.urbanairship.com/api/apids?limit=%7B%7D&start=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets APIDs. You can control how many APIDs are returned at a time by using the limit GET argument. The maximum limit is 5000."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "b0496289-7bb5-40c7-aa57-345b582974a0"
            }
          ]
        }
      ]
    },
    {
      "name": "User",
      "item": [
        {
          "id": "1d4ba8e9-4918-4845-91a1-24ba24fc995f",
          "name": "user.post",
          "request": {
            "url": "http://go.urbanairship.com/api/user",
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
            "description": "Creates a new user and returns the credentials."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e1a4579a-3783-4cbf-920e-8da7a4681526"
            }
          ]
        }
      ]
    }
  ]
}