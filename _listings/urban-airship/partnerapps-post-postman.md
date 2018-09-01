{
  "info": {
    "name": "Urban Airship Post Partner Apps",
    "_postman_id": "13db22fb-7aab-4e58-b871-f0a9f462515a",
    "description": "Adds a new application.",
    "schema": "https://schema.getpostman.com/json/collection/v2.0.0/"
  },
  "item": [
    {
      "name": "Device",
      "item": [
        {
          "id": "f50009ba-36a2-4752-a620-5fa9e258a317",
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
              "id": "6f6fa38b-3579-455f-8fd7-ffaf784720dd"
            }
          ]
        },
        {
          "id": "e5818137-3d48-4f11-84f1-46cf2d4f6eb4",
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
              "id": "57065747-5d57-4823-92ac-3dc42d8884b8"
            }
          ]
        },
        {
          "id": "24830d7d-4a11-42b9-a7d3-93d9f8735404",
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
              "id": "f5fb495f-045e-47cc-a8bb-d3d4ca005393"
            }
          ]
        },
        {
          "id": "5ba33f22-0a24-46c6-9fa8-ab058b68a12e",
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
              "id": "48865b98-54fc-41ea-9e6b-7b9d7e02a3d2"
            }
          ]
        },
        {
          "id": "b264fc96-731f-4a29-891d-43fe4d8a099d",
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
              "id": "f30c9495-f1e9-4ddb-bc32-2935c5566e5a"
            }
          ]
        },
        {
          "id": "133a2df8-89e6-4161-88b7-c9f70a57586e",
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
              "id": "881ff158-0fc2-41f6-bbbf-ec9abd3a2658"
            }
          ]
        },
        {
          "id": "dabf6a88-f8b0-450d-bc2a-0681776d18c3",
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
              "id": "ce8c6914-cbc5-49b2-b877-7202f3c25f29"
            }
          ]
        },
        {
          "id": "54ac07c1-4501-4edb-8441-1959d8e039c9",
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
              "id": "bac7d30a-22ae-48ab-80a0-8c466a9b4648"
            }
          ]
        },
        {
          "id": "36ba9d15-0c3b-48ea-a678-83b75e095ae0",
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
              "id": "dd2320af-49b2-4571-9550-d7a6d2b3e331"
            }
          ]
        },
        {
          "id": "84970dfb-bb27-4ac8-9440-7c0341907a1d",
          "name": "device_tokens.device_token.tags.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.urbanairship.com",
              "path": [
                "api",
                "device_tokens/:device_token/tags"
              ],
              "variable": [
                {
                  "id": "device_token",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets tags for a specific device token."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d86d067a-e708-497e-b0ef-297c877dfe2e"
            }
          ]
        },
        {
          "id": "aa0d0105-a501-4569-8582-6926d27c3403",
          "name": "device_tokens.device_token.tags.tag.put",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.urbanairship.com",
              "path": [
                "api",
                "device_tokens/:device_token/tags/:tag"
              ],
              "variable": [
                {
                  "id": "device_token",
                  "value": "{}",
                  "type": "string"
                },
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
            "description": "Creates a tag and associate it with the specific device token."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "2bc0c99b-81e0-422a-bfb0-8fa3500967a3"
            }
          ]
        },
        {
          "id": "6737f7e7-a8fd-4023-ba6b-927fe350814c",
          "name": "device_tokens.device_token.tags.tag.delete",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.urbanairship.com",
              "path": [
                "api",
                "device_tokens/:device_token/tags/:tag"
              ],
              "variable": [
                {
                  "id": "device_token",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "tag",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Removes a single tag from a device token."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "844db648-b10c-4a98-840a-664b33c77d63"
            }
          ]
        }
      ]
    },
    {
      "name": "Push",
      "item": [
        {
          "id": "e1c8345c-eb74-4b85-8dc7-a8532c4a5bce",
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
              "id": "af6de051-91f4-4344-93e7-a283f9d31c1e"
            }
          ]
        },
        {
          "id": "72ff5cc0-d9c1-4da6-9b27-bb7dc86e7fd1",
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
              "id": "3754e30e-0c6d-4b14-9729-e899a64ae541"
            }
          ]
        },
        {
          "id": "5c27a112-b80e-437e-af4f-e314d5cd97ea",
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
              "id": "bf68b980-f61a-4b04-93e7-d6f9052e8f72"
            }
          ]
        },
        {
          "id": "4d2b43d0-1991-4a53-ad59-673ffb00a6ce",
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
              "id": "719c177b-3398-4789-9f4e-89530a69b258"
            }
          ]
        },
        {
          "id": "63c411f6-f3ac-48ef-9377-faee57ecb247",
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
              "id": "f77a9b26-51c6-43ea-8551-828ca0f974fe"
            }
          ]
        },
        {
          "id": "e0e502b2-0adf-4590-b6ac-a9bdd24ccdfe",
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
              "id": "1421592c-b4f4-4395-bc9a-d4d9a046f7f8"
            }
          ]
        },
        {
          "id": "8eaab533-935b-4e5b-b62f-98ef4b270f87",
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
              "id": "4e44935c-70c5-4ad5-86ca-8dd84e0db0d0"
            }
          ]
        },
        {
          "id": "485f8438-19f0-4036-8812-80edbf88d5dd",
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
              "id": "dbc20365-2100-4aa7-9bc7-ccd252a96097"
            }
          ]
        }
      ]
    },
    {
      "name": "Apids",
      "item": [
        {
          "id": "4717a4bf-3433-4101-8006-1e1ee188cb54",
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
              "id": "b582c0f3-a98d-47a9-b466-3b6f5769afef"
            }
          ]
        },
        {
          "id": "dc2acbed-44b7-4e53-bc56-0624cd5835ba",
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
              "id": "290d6209-2625-4af3-a954-2e759f5be355"
            }
          ]
        },
        {
          "id": "98c246a8-d9ee-487e-b3c2-d7cbeff5327d",
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
              "id": "0e8e3862-4f5f-41f3-b7cd-c4591edfe937"
            }
          ]
        },
        {
          "id": "5a384e16-3d78-47fe-acad-662dbc26fbe7",
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
              "id": "fa0671ba-27ce-46a2-952b-d1d707baa952"
            }
          ]
        }
      ]
    },
    {
      "name": "User",
      "item": [
        {
          "id": "bda14a96-bb24-4ac9-9bfb-ffd349e47cbd",
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
              "id": "424bf35b-fa29-4a6d-9bde-4453599920e7"
            }
          ]
        },
        {
          "id": "8da40b5d-70dc-42b9-8f70-7c8ae8ad61db",
          "name": "user.user_id.get",
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
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves an user???s subscription information."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "7d71eddc-7309-4054-96e1-d753c9d5d9dc"
            }
          ]
        },
        {
          "id": "250eb77b-07b4-42e4-93d4-b621fa2ace29",
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
              "id": "a750c2f4-09e2-4cd6-9044-9465e3ce99f7"
            }
          ]
        },
        {
          "id": "2733fa04-8a14-4bab-84cf-2e27f45dc0ee",
          "name": "user.user_id.delete",
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
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes an user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "8ee63417-df22-4268-88b6-273e76679351"
            }
          ]
        },
        {
          "id": "b05ab2e8-24ee-4d3f-9ab1-60c264795daf",
          "name": "user.user_id.creds.reset.post",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.urbanairship.com",
              "path": [
                "api",
                "user/:user_id/creds/reset"
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
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
            "description": "Changes the password of an user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "c30123c5-d424-47d9-b12e-10ca7f94111a"
            }
          ]
        },
        {
          "id": "bac54b74-0fa0-406e-8bb0-086f0ea7975a",
          "name": "user.user_id.messages.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.urbanairship.com",
              "path": [
                "api",
                "user/:user_id/messages"
              ],
              "query": [
                {
                  "key": "full_list",
                  "value": "%7B%7D",
                  "disabled": false
                },
                {
                  "key": "since",
                  "value": "%7B%7D",
                  "disabled": false
                }
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of messages and some metadata about them. It will also include some metadata about the user."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "15a18f8f-e16b-499c-9c26-dbf2622382e6"
            }
          ]
        },
        {
          "id": "13070d21-d276-4e84-b89b-0db5cde6e172",
          "name": "user.user_id.messages.unread.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.urbanairship.com",
              "path": [
                "api",
                "user/:user_id/messages/unread"
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of unread message IDs and their URLs."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ed20786f-30c0-4a91-89ae-ca4bb3670688"
            }
          ]
        },
        {
          "id": "98540a06-43e5-4888-85d6-ca9d222f2ba4",
          "name": "user.user_id.messages.unread.post",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.urbanairship.com",
              "path": [
                "api",
                "user/:user_id/messages/unread"
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
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
            "description": "Marks multiple messages as read at once. If a message has already been marked as read, it will be silently skipped."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "93d37db7-31e7-4eed-82e5-b1b6420f38fe"
            }
          ]
        },
        {
          "id": "1970a3f4-27ed-45e0-9802-de4fa07d6a92",
          "name": "user.user_id.messages.message.message_id.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.urbanairship.com",
              "path": [
                "api",
                "user/:user_id/messages/message/:message_id"
              ],
              "variable": [
                {
                  "id": "message_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "user_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets a message."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9fa6f85c-836b-47ed-b7a6-a5e622bcc737"
            }
          ]
        },
        {
          "id": "5f338c1f-2513-4a7d-b88f-4023bdb81e2d",
          "name": "user.user_id.messages.message.message_id.delete",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.urbanairship.com",
              "path": [
                "api",
                "user/:user_id/messages/message/:message_id"
              ],
              "variable": [
                {
                  "id": "message_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "user_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a message."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ed547bda-67e8-4ea1-a0cf-9ff6653f4f8b"
            }
          ]
        },
        {
          "id": "753ad495-21da-4640-bb9b-5a1406432a45",
          "name": "user.user_id.messages.message.message_id.body.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.urbanairship.com",
              "path": [
                "api",
                "user/:user_id/messages/message/:message_id/body"
              ],
              "variable": [
                {
                  "id": "message_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "user_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Gets a message's body."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "70822849-8231-4e47-ada4-67e3ce67bef1"
            }
          ]
        },
        {
          "id": "d57cd2bb-1d03-45d7-b63e-33ce28c4ef6a",
          "name": "user.user_id.messages.message.message_id.read.post",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.urbanairship.com",
              "path": [
                "api",
                "user/:user_id/messages/message/:message_id/read"
              ],
              "variable": [
                {
                  "id": "message_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "user_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Marks a message as read."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "9ed13645-2762-4b08-9450-02b20858805f"
            }
          ]
        },
        {
          "id": "773838f1-3015-4af9-985d-708514fc2be7",
          "name": "user.user_id.messages.delete.post",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.urbanairship.com",
              "path": [
                "api",
                "user/:user_id/messages/delete"
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
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
            "description": "Deletes multiple messages at once. If a message has already been deleted, it will be silently skipped."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "717dfe14-4140-417a-9410-493b6d3a839f"
            }
          ]
        },
        {
          "id": "c36141fc-372a-470f-962d-974a85b20025",
          "name": "user.recover.post",
          "request": {
            "url": "http://go.urbanairship.com/api/user/recover",
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
            "description": "Uses the user???s email address as a way to restore subscription content across devices."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "592c95da-a060-42c6-9043-510896d84d8d"
            }
          ]
        },
        {
          "id": "0aaefb13-c95c-4bc6-b693-289b3baa82f4",
          "name": "user.recover.id.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.urbanairship.com",
              "path": [
                "api",
                "user/recover/:id"
              ],
              "variable": [
                {
                  "id": "id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Checks the recovery status."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "722d198c-480e-4798-b447-cab9c7a8e332"
            }
          ]
        },
        {
          "id": "f0ee2d28-9b0d-409a-afe7-6e377607c37b",
          "name": "user.user_id.available_subscriptions.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.urbanairship.com",
              "path": [
                "api",
                "user/:user_id/available_subscriptions"
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Retrieves subscription options."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "a1455359-0a3c-4a93-bb08-79f39f216634"
            }
          ]
        },
        {
          "id": "732106d7-9424-428b-ad85-d28f4dcd64f6",
          "name": "user.user_id.subscriptions.subscription_key.purchase.post",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.urbanairship.com",
              "path": [
                "api",
                "user/:user_id/subscriptions/:subscription_key/purchase"
              ],
              "variable": [
                {
                  "id": "subscription_key",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "user_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
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
            "description": "Adds a new subscription."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "5982f187-65b6-4191-87b3-0d425f9665a1"
            }
          ]
        },
        {
          "id": "93515a41-9267-4282-88cc-1f8b55412368",
          "name": "user.user_id.subscription_content.get",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.urbanairship.com",
              "path": [
                "api",
                "user/:user_id/subscription_content"
              ],
              "variable": [
                {
                  "id": "user_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "Returns a list of available content."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "991eff0f-bf51-4821-a2ac-8c48b69badd6"
            }
          ]
        },
        {
          "id": "e72454eb-0d82-40a3-84cd-a5271e4fa572",
          "name": "user.user_id.subscriptions.content.content_id.download.post",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.urbanairship.com",
              "path": [
                "api",
                "user/:user_id/subscriptions/content/:content_id/download"
              ],
              "variable": [
                {
                  "id": "content_id",
                  "value": "{}",
                  "type": "string"
                },
                {
                  "id": "user_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
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
            "description": "Downloads the content."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "3a9f9093-f5a7-46c2-9cc0-1b1120973728"
            }
          ]
        }
      ]
    },
    {
      "name": "Airmail",
      "item": [
        {
          "id": "60cf8176-72f6-4728-9df6-234da5a6808e",
          "name": "airmail.send.post",
          "request": {
            "url": "http://go.urbanairship.com/api/airmail/send",
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
            "description": "Sends a message. All fields except message are optional, but at least one of tags, users or aliases must be specified. Much like the push API, we have a batch API call that can make sending multiple messages easier. It???s located at /api/airmail/send/batch/ and accepts a list of messages in the same format as the standard push call."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "d7a09cac-bcc4-48f5-b701-7141c4d37f55"
            }
          ]
        },
        {
          "id": "e6f1d073-078f-4f07-b342-267c4b9b9313",
          "name": "airmail.send.broadcast.post",
          "request": {
            "url": "http://go.urbanairship.com/api/airmail/send/broadcast?Content-Type=%7B%7D",
            "method": "POST",
            "body": {
              "mode": "raw"
            },
            "description": "Sends a message to all users (broadcast). Only message is required. The message will be sent out to every registered user. Badge numbers will be handled automatically as long as the push key is present."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "40b322d1-3931-49f6-8afb-e3a936208b26"
            }
          ]
        }
      ]
    },
    {
      "name": "App",
      "item": [
        {
          "id": "3329f7f9-0294-4fb6-be7f-3a134e237289",
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
              "id": "5b197e35-69cd-4ff8-be99-342ff795020e"
            }
          ]
        },
        {
          "id": "a0a962f9-53d5-4f3e-9ff1-0348571e6b34",
          "name": "app.content.product_id.download.post",
          "request": {
            "url": {
              "protocol": "http",
              "host": "go.urbanairship.com",
              "path": [
                "api",
                "app/content/:product_id/download"
              ],
              "variable": [
                {
                  "id": "product_id",
                  "value": "{}",
                  "type": "string"
                }
              ]
            },
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
            "description": "Returns a temporary URL where the client can download the content. In the payload, the receipt string is the receipt data from the purchase. It should be unaltered from how Apple delivers it to your application.udid is an optional field to help identify a particular user???s purchases, which can aid debugging. It should always be a hash of the UDID, not the actual UDID, to ensure compliance with Apple???s TOS. The optional version field should be the StoreFront library version, or custom if you???re building your own."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "0a4ea381-e14e-43cc-85b4-f19e0b0d34c9"
            }
          ]
        },
        {
          "id": "c93e199c-5d21-4556-a207-369446234850",
          "name": "app.updates.post",
          "request": {
            "url": "http://go.urbanairship.com/api/app/updates?product_id=%7B%7D",
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
            "description": "Checks for updates. It can be useful on application launch to compare a list of installed updates with our server to see if there are any updates to be had for the content."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "ba109f31-a41f-4e71-b53c-093b3b48767d"
            }
          ]
        }
      ]
    },
    {
      "name": "Feeds",
      "item": [
        {
          "id": "6721518b-886b-4b93-832d-17663ab72c35",
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
              "id": "6fc8d707-6243-449f-8c5a-82aa9ab3bf3e"
            }
          ]
        },
        {
          "id": "d5d3c265-2540-4e21-aef8-b1fe3e81ec06",
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
              "id": "99d410bf-2b0c-46eb-ba5a-3d81e4bc08b8"
            }
          ]
        },
        {
          "id": "e80c3228-2ece-4479-bc81-196ed67f84fc",
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
              "id": "0fb6f253-1057-4ab2-88d3-6257fb475de8"
            }
          ]
        },
        {
          "id": "b82e9e82-45b9-47f0-9c3c-98dd24add8fc",
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
              "id": "56f278a6-8ebc-45f8-bc1a-1ca382520451"
            }
          ]
        },
        {
          "id": "0e2da72b-aba2-4ffd-8e7d-177c646cc47d",
          "name": "feeds.feed_id.delete",
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
            "method": "DELETE",
            "body": {
              "mode": "raw"
            },
            "description": "Deletes a feed."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "85fe78cd-e179-40b1-92bc-f3b2efc57d31"
            }
          ]
        }
      ]
    },
    {
      "name": "Tags",
      "item": [
        {
          "id": "246eb232-4770-4dab-b4ba-cfc1368ee5f4",
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
              "id": "0a9a550a-f926-47c6-8528-86e5cc9ddccf"
            }
          ]
        },
        {
          "id": "1881cf7a-f440-4efc-8ac1-736730bdcdba",
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
              "id": "a4235eb4-c538-43e3-96f4-c208434f8c5b"
            }
          ]
        },
        {
          "id": "4906e4a3-1e62-4ea7-aafb-444e82d2d638",
          "name": "tags.tag.post",
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
            "description": "Modifies device tokens on a tag."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "f710468b-d57d-4063-a1de-46312cff2881"
            }
          ]
        }
      ]
    },
    {
      "name": "Partner",
      "item": [
        {
          "id": "728c076f-023f-464d-91c6-5f13fc9e131e",
          "name": "partner.apps.get",
          "request": {
            "url": "http://go.urbanairship.com/api/partner/apps?device_token=%7B%7D&tag=%7B%7D",
            "method": "GET",
            "body": {
              "mode": "raw"
            },
            "description": "List applications."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "67ff364e-0cd0-420e-81a4-4735dccc2f7e"
            }
          ]
        },
        {
          "id": "4a7b7582-4937-4a83-9d1b-62f76083f577",
          "name": "partner.apps.post",
          "request": {
            "url": "http://go.urbanairship.com/api/partner/apps",
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
            "description": "Adds a new application."
          },
          "response": [
            {
              "status": "OK",
              "code": 200,
              "name": "Response_200",
              "id": "e98e88b6-2f98-4444-bd0c-f5f44239a788"
            }
          ]
        }
      ]
    }
  ]
}