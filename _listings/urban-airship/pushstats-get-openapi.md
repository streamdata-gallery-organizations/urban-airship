---
swagger: "2.0"
x-collection-name: Urban Airship
x-complete: 0
info:
  title: Urban Airship Get Push Stats
  description: 'Returns hourly message counts for your application. By default, results
    are returned in JSON. For CSV, either add the header:Accept:text/csv or append
    &format=csv to the query string. Times are in UTC, and data is provided for each
    push platform (currently: iOS, BlackBerry, Android, and C2DM, in that order).
    The statistics system is updated every 15 minutes, so the final count for an hour
    will be done at the latest 15 minutes after the hour is done.'
  version: v3
host: go.urbanairship.com
basePath: /api/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /device_tokens/{token}:
    put:
      summary: Put Device Tokens Token
      description: Registers a device token.
      operationId: device_tokens.token.put
      x-api-path-slug: device-tokenstoken-put
      parameters:
      - in: query
        name: token
        description: Device tokens should be represented as an uppercase string, 64
          characters long, without spaces or other separators
      - in: path
        name: token
      responses:
        200:
          description: OK
      tags:
      - Device
      - Tokens
      - Token
    get:
      summary: Get Device Tokens Token
      description: Gets a device token???s alias.
      operationId: device_tokens.token.get
      x-api-path-slug: device-tokenstoken-get
      parameters:
      - in: query
        name: token
        description: Device tokens should be represented as an uppercase string, 64
          characters long, without spaces or other separators
      - in: path
        name: token
      responses:
        200:
          description: OK
      tags:
      - Device
      - Tokens
      - Token
    delete:
      summary: Delete Device Tokens Token
      description: Marks the device token as inactive. No notifications will be delivered
        to it until a PUT is executed again. The DELETE returns HTTP 204 No Content,
        and needs no payload. When a token is deleted in this manner, any alias or
        tags will be cleared.
      operationId: device_tokens.token.delete
      x-api-path-slug: device-tokenstoken-delete
      parameters:
      - in: query
        name: token
        description: Device tokens should be represented as an uppercase string, 64
          characters long, without spaces or other separators
      - in: path
        name: token
      responses:
        200:
          description: OK
      tags:
      - Device
      - Tokens
      - Token
  /push:
    post:
      summary: Post Push
      description: Sends a push message to one or more users. Only one of aliases,
        tags, or device_pins is required, but they can be mixed and matched as much
        as you???d like.
      operationId: push.post
      x-api-path-slug: push-post
      parameters:
      - in: query
        name: Content-Type
        description: Content type
      - in: header
        name: Content-Type
        description: Content type
      responses:
        200:
          description: OK
      tags:
      - Push
  /push/scheduled/{notification}:
    delete:
      summary: Delete Push Scheduled Notification
      description: Cancels a scheduled notification.  A successful delete will have
        an HTTP status code of 204. If the scheduled notification does not exist,
        has already been successfully deleted, or was sent, the status code will be
        404.
      operationId: push.scheduled.notification.delete
      x-api-path-slug: pushschedulednotification-delete
      parameters:
      - in: query
        name: notification
        description: Scheduled notification ID
      - in: path
        name: notification
      responses:
        200:
          description: OK
      tags:
      - Push
      - Scheduled
      - Notification
  /push/scheduled:
    post:
      summary: Post Push Scheduled
      description: Bulk deletes scheduled notifications. If you include URLs or aliases
        for scheduled notifications that don???t exist or have already been sent,
        they will be ignored. Any device token in the cancel_device_tokens payload
        will have every notification that is sent to it removed. This will not prevent
        it from receiving scheduled notifications to tags or broadcast messages.
      operationId: push.scheduled.post
      x-api-path-slug: pushscheduled-post
      parameters:
      - in: query
        name: Content-Type
        description: Content type
      - in: header
        name: Content-Type
        description: Content type
      responses:
        200:
          description: OK
      tags:
      - Push
      - Scheduled
  /push/scheduled/alias/{alias}:
    put:
      summary: Put Push Scheduled Alias Alias
      description: Changes a scheduled notification alias. Aliases for scheduled notifications
        are unique per Urban Airship application, so you might want to hash the aliases
        with a device ID or use some other mechanism to ensure uniqueness. The only
        other limit is that they must be 255 characters or less.
      operationId: push.scheduled.alias.alias.put
      x-api-path-slug: pushscheduledaliasalias-put
      parameters:
      - in: query
        name: alias
        description: Scheduled notification alias
      - in: path
        name: alias
      - in: query
        name: Content-Type
        description: Content type
      - in: header
        name: Content-Type
        description: Content type
      responses:
        200:
          description: OK
      tags:
      - Push
      - Scheduled
      - Alias
      - Alias
    delete:
      summary: Delete Push Scheduled Alias Alias
      description: Deletes a scheduled notification alias.  If you attempt to schedule
        an aliased scheduled notification with an alias that already exists for your
        application, it will overwrite the existing one.
      operationId: push.scheduled.alias.alias.delete
      x-api-path-slug: pushscheduledaliasalias-delete
      parameters:
      - in: query
        name: alias
        description: Scheduled notification alias
      - in: path
        name: alias
      responses:
        200:
          description: OK
      tags:
      - Push
      - Scheduled
      - Alias
      - Alias
  /push/batch:
    post:
      summary: Post Push Batch
      description: Sends a push message to all the listed PINs. Each item in the list
        can contain 0 or many device_pins and 0 or many aliases or tags, and the blackberry
        payload is in the same format as for individual pushes.
      operationId: push.batch.post
      x-api-path-slug: pushbatch-post
      parameters:
      - in: query
        name: Content-Type
        description: Content type
      - in: header
        name: Content-Type
        description: Content type
      responses:
        200:
          description: OK
      tags:
      - Push
      - Batch
  /push/broadcast:
    post:
      summary: Post Push Broadcast
      description: 'Sends a push message to all active APIDs (Broadcast). Important:
        The maximum message size is 1024 bytes. This is calculated as the UTF-8 lengths
        of alert and extra fields together.'
      operationId: push.broadcast.post
      x-api-path-slug: pushbroadcast-post
      parameters:
      - in: query
        name: Content-Type
        description: Content type
      - in: header
        name: Content-Type
        description: Content type
      responses:
        200:
          description: OK
      tags:
      - Push
      - Broadcast
  /push/stats:
    get:
      summary: Get Push Stats
      description: 'Returns hourly message counts for your application. By default,
        results are returned in JSON. For CSV, either add the header:Accept:text/csv
        or append &format=csv to the query string. Times are in UTC, and data is provided
        for each push platform (currently: iOS, BlackBerry, Android, and C2DM, in
        that order). The statistics system is updated every 15 minutes, so the final
        count for an hour will be done at the latest 15 minutes after the hour is
        done.'
      operationId: push.stats.get
      x-api-path-slug: pushstats-get
      parameters:
      - in: query
        name: end
        description: End date in UTC format
      - in: query
        name: format
        description: Response format
      - in: query
        name: start
        description: Start date in UTC format
      responses:
        200:
          description: OK
      tags:
      - Push
      - Stats
x-streamrank:
  polling_total_time_average: "0"
  polling_size_download_average: "0"
  streaming_total_time_average: "0"
  streaming_size_download_average: "0"
  change_yes: "0"
  change_no: "0"
  time_percentage: "0"
  size_percentage: "0"
  change_percentage: "200"
  last_run: ~
  days_run: "0"
  minute_run: "0"
---