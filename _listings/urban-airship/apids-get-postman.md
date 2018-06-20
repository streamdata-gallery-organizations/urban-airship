{
  "info": {
    "name": "Urban Airship Get Aps",
    "_postman_id": "f5d4f1c7-255b-4b91-ae30-e689f558b920",
    "description": "Gets APIDs. You can control how many APIDs are returned at a time by using the limit GET argument. The maximum limit is 5000.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Device",
      "item": [
        {
          "id": "00481497-54b3-4a70-9550-68935183cb06",
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
              "id": "996f3e59-4401-4b7f-9cc4-1cdac3f087ab"
            }
          ]
        },
        {
          "id": "e08b2bc6-ddc2-4f75-a98a-86064b9fe679",
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
              "id": "9cae7cbc-428d-48ae-84b1-a0ef37def91f"
            }
          ]
        },
        {
          "id": "3235d320-7f35-42c9-b153-a71a37291711",
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
              "id": "2904278f-ec56-4509-a75d-4fd480f38cf2"
            }
          ]
        },
        {
          "id": "0d4018d0-7a77-4f12-bd88-dba83bfe82e7",
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
              "id": "d02f6cc7-c2e9-4399-859c-02c5a36459a1"
            }
          ]
        },
        {
          "id": "cbeed8a4-76e7-47ea-9ff0-8c2a1b72d6af",
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
              "id": "1dc4d7fe-4eb0-45be-8d68-3168d6f8b848"
            }
          ]
        },
        {
          "id": "ecf98315-166a-4fca-8a0f-7ba52c763e8a",
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
              "id": "af5dec69-896b-4526-9e42-ee9b8ddd7915"
            }
          ]
        }
      ]
    },
    {
      "name": "Push",
      "item": [
        {
          "id": "07248dc3-59dc-495e-9e4a-9174edc37ba4",
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
              "id": "717579ff-58ba-402d-b593-bf21bb61d1fe"
            }
          ]
        },
        {
          "id": "ca705441-4171-4b20-bd73-9076222e34ea",
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
              "id": "20351665-6123-480e-8a7c-dd81cb9aea4c"
            }
          ]
        },
        {
          "id": "6697a259-a465-48d0-8a2e-f3f18cead03f",
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
              "id": "3d65ddf6-bba0-4ada-b651-dd1b51d1e698"
            }
          ]
        },
        {
          "id": "443740fe-b1bb-46f7-b780-ae6b90b2177c",
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
              "id": "580dfaae-f0c3-4c8f-aa76-e67bc82ba3b6"
            }
          ]
        },
        {
          "id": "2e7075fb-f4a9-4e74-9ac5-9360c3be22e7",
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
              "id": "0dffd067-592c-47a2-88f3-07dd68d2c0d5"
            }
          ]
        },
        {
          "id": "f2826090-e4ba-4194-96fb-51c0b6f54cc8",
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
              "id": "975e60b3-8c6a-469c-8eaa-32182352498e"
            }
          ]
        },
        {
          "id": "3e5d2c31-864d-404b-a778-8704ac8dfb60",
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
              "id": "7f1d9799-c2bc-456b-aee1-4537e1c68f9c"
            }
          ]
        },
        {
          "id": "a4fa55ab-778c-4d8a-b8a6-801c1873754a",
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
              "id": "8b82c07b-0c28-4c1d-ae2e-f34c17265a7d"
            }
          ]
        }
      ]
    },
    {
      "name": "Apids",
      "item": [
        {
          "id": "ad6bbf52-cb04-4607-82e1-5ca2bd01b09f",
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
              "id": "1beb1212-c670-4d78-a2c9-2a453db671ae"
            }
          ]
        },
        {
          "id": "8a36b835-8ca6-4603-97bb-a501e4a2d6b1",
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
              "id": "ac4fff36-31ed-40d9-8912-dd3943bbf293"
            }
          ]
        },
        {
          "id": "f293046e-b66d-499a-a290-9909a9d2c62a",
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
              "id": "266826d0-b027-4597-9e2e-3657e904eea9"
            }
          ]
        },
        {
          "id": "37bd2086-22a1-40df-ac89-686e4be7b86a",
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
              "id": "1a427c04-67ce-4faa-9d25-a7d6d72c407d"
            }
          ]
        }
      ]
    }
  ]
}