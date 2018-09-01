{
  "info": {
    "name": "Urban Airship Put User User",
    "_postman_id": "c8ae6934-0e29-4031-adf6-50e54024dae6",
    "description": "Changes properties of an user - for example, changing or adding an email address.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Device",
      "item": [
        {
          "id": "354e4df9-d091-4fee-ad03-82682f3b162d",
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
            "description": "Gets a device token???s alias."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "1d9a0828-bdd5-4ab5-9be3-711b98fa5e67"
            }
          ]
        },
        {
          "id": "7ffdb52c-c448-4d92-af53-93edbbfe195c",
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
              "id": "3d441705-c232-4496-94f6-f4a45ba0ce7f"
            }
          ]
        },
        {
          "id": "a5187e70-3079-414d-a33f-fffabdf5308b",
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
              "id": "a9ed9e9e-d5c5-4213-8190-d7eee57b1634"
            }
          ]
        },
        {
          "id": "86c86e3f-ec7d-4812-83ee-775d8ce6c93e",
          "name": "device_tokens.get",
          "request": {
            "url": "http://go.urbanairship.com/api/device_tokens?limit=%7B%7D&page=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets information about all of your device tokens. If your application has a large number of device tokens, we???ll paginate the request for you. By default, we paginate at 5000 device tokens. You can receive the next page simply by retrieving the URL from \"next_page\" - in this way it is easy to export all of your device tokens and all their data."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9895858f-7c71-4801-8166-2ad0c527e88f"
            }
          ]
        },
        {
          "id": "f22bf1cd-d0e8-4d88-a217-22c83d057f61",
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
              "id": "89adacf6-df85-4cc4-9817-b80df6c258b1"
            }
          ]
        },
        {
          "id": "f189e77e-0036-43fd-9c02-b46aa7089d8a",
          "name": "device_tokens.feedback.get",
          "request": {
            "url": "http://go.urbanairship.com/api/device_tokens/feedback?since=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets what device tokens are now invalid. Apple informs us when a push notification is sent to a device that can???t receive it because the application has been uninstalled. We mark the device token as inactive and immediately stop sending notifications to that device. Once a day is a good interval for querying the feedback service, but you can do it more often to save on bandwidth from unnecessary notifications. In the response, what does marked_inactive_on mean? Apple sends a timestamp for each device token returned via the feedback service. Since a device can be off the network for a while, this can be a point in the recent past. In order to make this API work smoothly for you, we record the timestamp we marked as inactive. This means you only need to query for data since the last time you queried. Once a day is a good timeframe, or once a week for very small or infrequently used applications. A few times a day is good for applications with heavy use."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "35869ba3-a9d3-47ae-8f03-c05f374a4002"
            }
          ]
        },
        {
          "id": "19849122-c9ae-46ac-b025-2dc2f17f8a16",
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
              "id": "0f31cba0-0e39-4630-947b-5ba5d91e7cc5"
            }
          ]
        },
        {
          "id": "f3c61b17-47fd-4db0-aa82-0b1f48e1b3be",
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
              "id": "5ecad0a2-b5bd-44dc-8872-af3564b91138"
            }
          ]
        },
        {
          "id": "375966e8-2bc4-4269-ab5c-27522ad8a396",
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
              "id": "4d4994ea-d187-4d6f-9adc-daec0d251ca6"
            }
          ]
        }
      ]
    },
    {
      "name": "Push",
      "item": [
        {
          "id": "e18df1ac-514e-4c8d-a532-5f0f127a2d25",
          "name": "push.post",
          "request": {
            "url": "http://go.urbanairship.com/api/push?Content-Type=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Sends a push message to one or more users. Only one of aliases, tags, or device_pins is required, but they can be mixed and matched as much as you???d like."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "12dc7ecc-861c-473a-998e-f594a815486b"
            }
          ]
        },
        {
          "id": "b5ce1a87-ab81-48c4-b443-a42aa83c7569",
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
              "id": "e7415aa0-42f8-4360-ba97-e0cb1745a311"
            }
          ]
        },
        {
          "id": "1d2c8fb6-a91f-4c4e-9d1e-8b72eced06f9",
          "name": "push.scheduled.post",
          "request": {
            "url": "http://go.urbanairship.com/api/push/scheduled?Content-Type=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Bulk deletes scheduled notifications. If you include URLs or aliases for scheduled notifications that don???t exist or have already been sent, they will be ignored. Any device token in the cancel_device_tokens payload will have every notification that is sent to it removed. This will not prevent it from receiving scheduled notifications to tags or broadcast messages."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "15511b4e-983f-4299-9c67-43fd6c85b7fe"
            }
          ]
        },
        {
          "id": "04b70c3b-f090-481d-ad23-60b275b7ff2c",
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
              "id": "df7ef84d-c1d5-4cc4-acb2-c4f1c406453f"
            }
          ]
        },
        {
          "id": "0921971a-ea59-4636-b722-aa88b9fc9d96",
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
              "id": "409c629c-0658-4369-bb8b-4c812669cd10"
            }
          ]
        },
        {
          "id": "80212649-fe54-40d5-9167-70fa329d42c8",
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
              "id": "5b09b3cb-b51a-4c89-a730-2d459386d874"
            }
          ]
        },
        {
          "id": "b21ff877-8529-4593-b8fe-74595c57d6a1",
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
              "id": "95b7be38-b77d-47aa-a4f3-89d6ab8eb128"
            }
          ]
        },
        {
          "id": "abe4221a-9a53-4d28-a21f-866d09aca661",
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
              "id": "cf61f319-00a6-4365-b490-39cf7e594852"
            }
          ]
        }
      ]
    },
    {
      "name": "Apids",
      "item": [
        {
          "id": "ca6edc2f-af75-45eb-974e-d960c2cf170b",
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
              "id": "d10d190b-737d-4aba-9a30-5faa4061b10e"
            }
          ]
        },
        {
          "id": "04ee9b48-4443-47f2-ad57-68bc6417ff7c",
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
              "id": "e81c3cfd-547d-407e-847e-df226032bf21"
            }
          ]
        },
        {
          "id": "5bf26d61-5c1e-4357-b170-15836fce4951",
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
              "id": "11dfdcb9-2023-4c91-b39f-04121cfc113b"
            }
          ]
        },
        {
          "id": "fcca5030-e90a-40b7-a59a-9bc2d3c7f7da",
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
              "id": "5fcb9b8c-1f7f-45d7-8d63-47f56c6e78d1"
            }
          ]
        }
      ]
    },
    {
      "name": "User",
      "item": [
        {
          "id": "126b5432-208d-421c-a83f-e7694d68aba7",
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
              "id": "735fd2ea-b3f1-48c3-8f28-21b4c3eb4a1e"
            }
          ]
        },
        {
          "id": "a155b222-c270-40e7-9606-90298a975218",
          "name": "user.user_id.put",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.urbanairship.com",
              "path": [
                "api",
                "user/:user_id"
              ],
              "variable": [
                {
                  "id": "user_id",
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
            "description": "Changes properties of an user - for example, changing or adding an email address."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "537b4395-1fcd-48ec-adb8-0d1da97a98cf"
            }
          ]
        }
      ]
    }
  ]
}