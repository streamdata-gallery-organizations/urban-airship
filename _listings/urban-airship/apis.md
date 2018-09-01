---
name: Urban Airship
x-slug: urban-airship
description: A market-leading mobile app engagement, mobile analytics, mobile data
  integration and mobile wallet marketing solution.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
x-kinRank: "8"
x-alexaRank: "79571"
tags: Urban Airship
created: "2018-08-31"
modified: "2018-08-31"
url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/apis.md
specificationVersion: "0.14"
apis:
- name: Urban Airship - Put Device Tokens Token
  x-api-slug: device-tokenstoken-put
  description: Registers a device token.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
  humanURL: http://urbanairship.com/
  baseURL: https://go.urbanairship.com//api/
  tags: BaaS, Push Notifications, Stack Network, SaaS, Technology, Mobile, internet,
    Relative Data, Service API, Locations, Locations, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/device-tokenstoken-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/device-tokenstoken-put-openapi.md
- name: Urban Airship - Get Device Tokens Token
  x-api-slug: device-tokenstoken-get
  description: Gets a device token???s alias.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
  humanURL: http://urbanairship.com/
  baseURL: https://go.urbanairship.com//api/
  tags: BaaS, Push Notifications, Stack Network, SaaS, Technology, Mobile, internet,
    Relative Data, Service API, Locations, Locations, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/device-tokenstoken-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/device-tokenstoken-get-openapi.md
- name: Urban Airship - Delete Device Tokens Token
  x-api-slug: device-tokenstoken-delete
  description: Marks the device token as inactive. No notifications will be delivered
    to it until a PUT is executed again. The DELETE returns HTTP 204 No Content, and
    needs no payload. When a token is deleted in this manner, any alias or tags will
    be cleared.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
  humanURL: http://urbanairship.com/
  baseURL: https://go.urbanairship.com//api/
  tags: BaaS, Push Notifications, Stack Network, SaaS, Technology, Mobile, internet,
    Relative Data, Service API, Locations, Locations, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/device-tokenstoken-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/device-tokenstoken-delete-openapi.md
- name: Urban Airship - Post Push
  x-api-slug: push-post
  description: Sends a push message to one or more users. Only one of aliases, tags,
    or device_pins is required, but they can be mixed and matched as much as you???d
    like.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
  humanURL: http://urbanairship.com/
  baseURL: https://go.urbanairship.com//api/
  tags: BaaS, Push Notifications, Stack Network, SaaS, Technology, Mobile, internet,
    Relative Data, Service API, Locations, Locations, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/push-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/push-post-openapi.md
- name: Urban Airship - Delete Push Scheduled Notification
  x-api-slug: pushschedulednotification-delete
  description: Cancels a scheduled notification.  A successful delete will have an
    HTTP status code of 204. If the scheduled notification does not exist, has already
    been successfully deleted, or was sent, the status code will be 404.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
  humanURL: http://urbanairship.com/
  baseURL: https://go.urbanairship.com//api/
  tags: BaaS, Push Notifications, Stack Network, SaaS, Technology, Mobile, internet,
    Relative Data, Service API, Locations, Locations, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/pushschedulednotification-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/pushschedulednotification-delete-openapi.md
- name: Urban Airship - Post Push Scheduled
  x-api-slug: pushscheduled-post
  description: Bulk deletes scheduled notifications. If you include URLs or aliases
    for scheduled notifications that don???t exist or have already been sent, they
    will be ignored. Any device token in the cancel_device_tokens payload will have
    every notification that is sent to it removed. This will not prevent it from receiving
    scheduled notifications to tags or broadcast messages.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
  humanURL: http://urbanairship.com/
  baseURL: https://go.urbanairship.com//api/
  tags: BaaS, Push Notifications, Stack Network, SaaS, Technology, Mobile, internet,
    Relative Data, Service API, Locations, Locations, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/pushscheduled-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/pushscheduled-post-openapi.md
- name: Urban Airship - Put Push Scheduled Alias Alias
  x-api-slug: pushscheduledaliasalias-put
  description: Changes a scheduled notification alias. Aliases for scheduled notifications
    are unique per Urban Airship application, so you might want to hash the aliases
    with a device ID or use some other mechanism to ensure uniqueness. The only other
    limit is that they must be 255 characters or less.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
  humanURL: http://urbanairship.com/
  baseURL: https://go.urbanairship.com//api/
  tags: BaaS, Push Notifications, Stack Network, SaaS, Technology, Mobile, internet,
    Relative Data, Service API, Locations, Locations, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/pushscheduledaliasalias-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/pushscheduledaliasalias-put-openapi.md
- name: Urban Airship - Delete Push Scheduled Alias Alias
  x-api-slug: pushscheduledaliasalias-delete
  description: Deletes a scheduled notification alias.  If you attempt to schedule
    an aliased scheduled notification with an alias that already exists for your application,
    it will overwrite the existing one.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
  humanURL: http://urbanairship.com/
  baseURL: https://go.urbanairship.com//api/
  tags: BaaS, Push Notifications, Stack Network, SaaS, Technology, Mobile, internet,
    Relative Data, Service API, Locations, Locations, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/pushscheduledaliasalias-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/pushscheduledaliasalias-delete-openapi.md
- name: Urban Airship - Post Push Batch
  x-api-slug: pushbatch-post
  description: Sends a push message to all the listed PINs. Each item in the list
    can contain 0 or many device_pins and 0 or many aliases or tags, and the blackberry
    payload is in the same format as for individual pushes.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
  humanURL: http://urbanairship.com/
  baseURL: https://go.urbanairship.com//api/
  tags: BaaS, Push Notifications, Stack Network, SaaS, Technology, Mobile, internet,
    Relative Data, Service API, Locations, Locations, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/pushbatch-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/pushbatch-post-openapi.md
- name: Urban Airship - Post Push Broadcast
  x-api-slug: pushbroadcast-post
  description: 'Sends a push message to all active APIDs (Broadcast). Important: The
    maximum message size is 1024 bytes. This is calculated as the UTF-8 lengths of
    alert and extra fields together.'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
  humanURL: http://urbanairship.com/
  baseURL: https://go.urbanairship.com//api/
  tags: BaaS, Push Notifications, Stack Network, SaaS, Technology, Mobile, internet,
    Relative Data, Service API, Locations, Locations, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/pushbroadcast-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/pushbroadcast-post-openapi.md
- name: Urban Airship - Get Push Stats
  x-api-slug: pushstats-get
  description: 'Returns hourly message counts for your application. By default, results
    are returned in JSON. For CSV, either add the header:Accept:text/csv or append
    &format=csv to the query string. Times are in UTC, and data is provided for each
    push platform (currently: iOS, BlackBerry, Android, and C2DM, in that order).
    The statistics system is updated every 15 minutes, so the final count for an hour
    will be done at the latest 15 minutes after the hour is done.'
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
  humanURL: http://urbanairship.com/
  baseURL: https://go.urbanairship.com//api/
  tags: BaaS, Push Notifications, Stack Network, SaaS, Technology, Mobile, internet,
    Relative Data, Service API, Locations, Locations, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/pushstats-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/pushstats-get-openapi.md
- name: Urban Airship - Get Device Tokens
  x-api-slug: device-tokens-get
  description: Gets information about all of your device tokens. If your application
    has a large number of device tokens, we???ll paginate the request for you. By
    default, we paginate at 5000 device tokens. You can receive the next page simply
    by retrieving the URL from "next_page" - in this way it is easy to export all
    of your device tokens and all their data.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
  humanURL: http://urbanairship.com/
  baseURL: https://go.urbanairship.com//api/
  tags: BaaS, Push Notifications, Stack Network, SaaS, Technology, Mobile, internet,
    Relative Data, Service API, Locations, Locations, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/device-tokens-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/device-tokens-get-openapi.md
- name: Urban Airship - Get Device Tokens Count
  x-api-slug: device-tokenscount-get
  description: Gets the number of device tokens you have registered.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
  humanURL: http://urbanairship.com/
  baseURL: https://go.urbanairship.com//api/
  tags: BaaS, Push Notifications, Stack Network, SaaS, Technology, Mobile, internet,
    Relative Data, Service API, Locations, Locations, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/device-tokenscount-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/device-tokenscount-get-openapi.md
- name: Urban Airship - Get Device Tokens Feedback
  x-api-slug: device-tokensfeedback-get
  description: Gets what device tokens are now invalid. Apple informs us when a push
    notification is sent to a device that can???t receive it because the application
    has been uninstalled. We mark the device token as inactive and immediately stop
    sending notifications to that device. Once a day is a good interval for querying
    the feedback service, but you can do it more often to save on bandwidth from unnecessary
    notifications. In the response, what does marked_inactive_on mean? Apple sends
    a timestamp for each device token returned via the feedback service. Since a device
    can be off the network for a while, this can be a point in the recent past. In
    order to make this API work smoothly for you, we record the timestamp we marked
    as inactive. This means you only need to query for data since the last time you
    queried. Once a day is a good timeframe, or once a week for very small or infrequently
    used applications. A few times a day is good for applications with heavy use.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
  humanURL: http://urbanairship.com/
  baseURL: https://go.urbanairship.com//api/
  tags: BaaS, Push Notifications, Stack Network, SaaS, Technology, Mobile, internet,
    Relative Data, Service API, Locations, Locations, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/device-tokensfeedback-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/device-tokensfeedback-get-openapi.md
- name: Urban Airship - Put Aps Ap
  x-api-slug: apidsapid-put
  description: Registers an APID. Unlike registration for iOS and BlackBerry applications,
    basic registration tying an APID to your application happens automatically. The
    registration API can be used to set aliases or tags. This returns HTTP 200 OK
    for any updates. Registering without any body is a no-op. Not including the alias
    field will clear it. To clear the list of tags, set it to the empty list []. If
    you are registering an APID to be used with C2DM, you will also need to include
    a C2DM registration ID.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
  humanURL: http://urbanairship.com/
  baseURL: https://go.urbanairship.com//api/
  tags: BaaS, Push Notifications, Stack Network, SaaS, Technology, Mobile, internet,
    Relative Data, Service API, Locations, Locations, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/apidsapid-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/apidsapid-put-openapi.md
- name: Urban Airship - Get Aps Ap
  x-api-slug: apidsapid-get
  description: Gets APID information.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
  humanURL: http://urbanairship.com/
  baseURL: https://go.urbanairship.com//api/
  tags: BaaS, Push Notifications, Stack Network, SaaS, Technology, Mobile, internet,
    Relative Data, Service API, Locations, Locations, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/apidsapid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/apidsapid-get-openapi.md
- name: Urban Airship - Delete Aps Ap
  x-api-slug: apidsapid-delete
  description: Marks an APID as invalid. No notifications will be delivered to it
    until it re-registers.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
  humanURL: http://urbanairship.com/
  baseURL: https://go.urbanairship.com//api/
  tags: BaaS, Push Notifications, Stack Network, SaaS, Technology, Mobile, internet,
    Relative Data, Service API, Locations, Locations, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/apidsapid-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/apidsapid-delete-openapi.md
- name: Urban Airship - Get Aps
  x-api-slug: apids-get
  description: Gets APIDs. You can control how many APIDs are returned at a time by
    using the limit GET argument. The maximum limit is 5000.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
  humanURL: http://urbanairship.com/
  baseURL: https://go.urbanairship.com//api/
  tags: BaaS, Push Notifications, Stack Network, SaaS, Technology, Mobile, internet,
    Relative Data, Service API, Locations, Locations, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/apids-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/apids-get-openapi.md
- name: Urban Airship - Put Device Pins Pin
  x-api-slug: device-pinspin-put
  description: Registers a BlackBerry PIN. This is optional, but recommended, for
    BlackBerry push messages. This returns HTTP 201 Created for the first registration
    and 200 OK for any updates. If you wish to include additional information about
    a device pin, for instance an alias or tags, include a JSON payload along with
    this request. Not including one of these keys removes it from the device pin.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
  humanURL: http://urbanairship.com/
  baseURL: https://go.urbanairship.com//api/
  tags: BaaS, Push Notifications, Stack Network, SaaS, Technology, Mobile, internet,
    Relative Data, Service API, Locations, Locations, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/device-pinspin-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/device-pinspin-put-openapi.md
- name: Urban Airship - Get Device Pins Pin
  x-api-slug: device-pinspin-get
  description: Gets Device PIN information.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
  humanURL: http://urbanairship.com/
  baseURL: https://go.urbanairship.com//api/
  tags: BaaS, Push Notifications, Stack Network, SaaS, Technology, Mobile, internet,
    Relative Data, Service API, Locations, Locations, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/device-pinspin-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/device-pinspin-get-openapi.md
- name: Urban Airship - Delete Device Pins Pin
  x-api-slug: device-pinspin-delete
  description: Marks a PIN as inactive. No notifications will be delivered to it until
    a PUT is executed again.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
  humanURL: http://urbanairship.com/
  baseURL: https://go.urbanairship.com//api/
  tags: BaaS, Push Notifications, Stack Network, SaaS, Technology, Mobile, internet,
    Relative Data, Service API, Locations, Locations, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/device-pinspin-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/device-pinspin-delete-openapi.md
- name: Urban Airship - Post User
  x-api-slug: user-post
  description: Creates a new user and returns the credentials.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
  humanURL: http://urbanairship.com/
  baseURL: https://go.urbanairship.com//api/
  tags: BaaS, Push Notifications, Stack Network, SaaS, Technology, Mobile, internet,
    Relative Data, Service API, Locations, Locations, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/user-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/user-post-openapi.md
- name: Urban Airship - Put User User
  x-api-slug: useruser-id-put
  description: Changes properties of an user - for example, changing or adding an
    email address.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
  humanURL: http://urbanairship.com/
  baseURL: https://go.urbanairship.com//api/
  tags: BaaS, Push Notifications, Stack Network, SaaS, Technology, Mobile, internet,
    Relative Data, Service API, Locations, Locations, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/useruser-id-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/useruser-id-put-openapi.md
- name: Urban Airship - Delete User User
  x-api-slug: useruser-id-delete
  description: Deletes an user.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
  humanURL: http://urbanairship.com/
  baseURL: https://go.urbanairship.com//api/
  tags: BaaS, Push Notifications, Stack Network, SaaS, Technology, Mobile, internet,
    Relative Data, Service API, Locations, Locations, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/useruser-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/useruser-id-delete-openapi.md
- name: Urban Airship - Get User User
  x-api-slug: useruser-id-get
  description: Retrieves an user???s subscription information.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
  humanURL: http://urbanairship.com/
  baseURL: https://go.urbanairship.com//api/
  tags: BaaS, Push Notifications, Stack Network, SaaS, Technology, Mobile, internet,
    Relative Data, Service API, Locations, Locations, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/useruser-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/useruser-id-get-openapi.md
- name: Urban Airship - Post User User Creds Reset
  x-api-slug: useruser-idcredsreset-post
  description: Changes the password of an user.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
  humanURL: http://urbanairship.com/
  baseURL: https://go.urbanairship.com//api/
  tags: BaaS, Push Notifications, Stack Network, SaaS, Technology, Mobile, internet,
    Relative Data, Service API, Locations, Locations, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/useruser-idcredsreset-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/useruser-idcredsreset-post-openapi.md
- name: Urban Airship - Post Airmail Send
  x-api-slug: airmailsend-post
  description: Sends a message. All fields except message are optional, but at least
    one of tags, users or aliases must be specified. Much like the push API, we have
    a batch API call that can make sending multiple messages easier. It???s located
    at /api/airmail/send/batch/ and accepts a list of messages in the same format
    as the standard push call.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
  humanURL: http://urbanairship.com/
  baseURL: https://go.urbanairship.com//api/
  tags: BaaS, Push Notifications, Stack Network, SaaS, Technology, Mobile, internet,
    Relative Data, Service API, Locations, Locations, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/airmailsend-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/airmailsend-post-openapi.md
- name: Urban Airship - Post Airmail Send Broadcast
  x-api-slug: airmailsendbroadcast-post
  description: Sends a message to all users (broadcast). Only message is required.
    The message will be sent out to every registered user. Badge numbers will be handled
    automatically as long as the push key is present.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
  humanURL: http://urbanairship.com/
  baseURL: https://go.urbanairship.com//api/
  tags: BaaS, Push Notifications, Stack Network, SaaS, Technology, Mobile, internet,
    Relative Data, Service API, Locations, Locations, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/airmailsendbroadcast-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/airmailsendbroadcast-post-openapi.md
- name: Urban Airship - Get User User Messages
  x-api-slug: useruser-idmessages-get
  description: Returns a list of messages and some metadata about them. It will also
    include some metadata about the user.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
  humanURL: http://urbanairship.com/
  baseURL: https://go.urbanairship.com//api/
  tags: BaaS, Push Notifications, Stack Network, SaaS, Technology, Mobile, internet,
    Relative Data, Service API, Locations, Locations, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/useruser-idmessages-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/useruser-idmessages-get-openapi.md
- name: Urban Airship - Get User User Messages Unread
  x-api-slug: useruser-idmessagesunread-get
  description: Returns a list of unread message IDs and their URLs.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
  humanURL: http://urbanairship.com/
  baseURL: https://go.urbanairship.com//api/
  tags: BaaS, Push Notifications, Stack Network, SaaS, Technology, Mobile, internet,
    Relative Data, Service API, Locations, Locations, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/useruser-idmessagesunread-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/useruser-idmessagesunread-get-openapi.md
- name: Urban Airship - Post User User Messages Unread
  x-api-slug: useruser-idmessagesunread-post
  description: Marks multiple messages as read at once. If a message has already been
    marked as read, it will be silently skipped.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
  humanURL: http://urbanairship.com/
  baseURL: https://go.urbanairship.com//api/
  tags: BaaS, Push Notifications, Stack Network, SaaS, Technology, Mobile, internet,
    Relative Data, Service API, Locations, Locations, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/useruser-idmessagesunread-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/useruser-idmessagesunread-post-openapi.md
- name: Urban Airship - Get User User Messages Message Message
  x-api-slug: useruser-idmessagesmessagemessage-id-get
  description: Gets a message.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
  humanURL: http://urbanairship.com/
  baseURL: https://go.urbanairship.com//api/
  tags: BaaS, Push Notifications, Stack Network, SaaS, Technology, Mobile, internet,
    Relative Data, Service API, Locations, Locations, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/useruser-idmessagesmessagemessage-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/useruser-idmessagesmessagemessage-id-get-openapi.md
- name: Urban Airship - Delete User User Messages Message Message
  x-api-slug: useruser-idmessagesmessagemessage-id-delete
  description: Deletes a message.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
  humanURL: http://urbanairship.com/
  baseURL: https://go.urbanairship.com//api/
  tags: BaaS, Push Notifications, Stack Network, SaaS, Technology, Mobile, internet,
    Relative Data, Service API, Locations, Locations, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/useruser-idmessagesmessagemessage-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/useruser-idmessagesmessagemessage-id-delete-openapi.md
- name: Urban Airship - Get User User Messages Message Message Body
  x-api-slug: useruser-idmessagesmessagemessage-idbody-get
  description: Gets a message's body.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
  humanURL: http://urbanairship.com/
  baseURL: https://go.urbanairship.com//api/
  tags: BaaS, Push Notifications, Stack Network, SaaS, Technology, Mobile, internet,
    Relative Data, Service API, Locations, Locations, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/useruser-idmessagesmessagemessage-idbody-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/useruser-idmessagesmessagemessage-idbody-get-openapi.md
- name: Urban Airship - Post User User Messages Message Message Read
  x-api-slug: useruser-idmessagesmessagemessage-idread-post
  description: Marks a message as read.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
  humanURL: http://urbanairship.com/
  baseURL: https://go.urbanairship.com//api/
  tags: BaaS, Push Notifications, Stack Network, SaaS, Technology, Mobile, internet,
    Relative Data, Service API, Locations, Locations, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/useruser-idmessagesmessagemessage-idread-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/useruser-idmessagesmessagemessage-idread-post-openapi.md
- name: Urban Airship - Post User User Messages Delete
  x-api-slug: useruser-idmessagesdelete-post
  description: Deletes multiple messages at once. If a message has already been deleted,
    it will be silently skipped.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
  humanURL: http://urbanairship.com/
  baseURL: https://go.urbanairship.com//api/
  tags: BaaS, Push Notifications, Stack Network, SaaS, Technology, Mobile, internet,
    Relative Data, Service API, Locations, Locations, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/useruser-idmessagesdelete-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/useruser-idmessagesdelete-post-openapi.md
- name: Urban Airship - Get App Content
  x-api-slug: appcontent-get
  description: Gets the store inventory.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
  humanURL: http://urbanairship.com/
  baseURL: https://go.urbanairship.com//api/
  tags: BaaS, Push Notifications, Stack Network, SaaS, Technology, Mobile, internet,
    Relative Data, Service API, Locations, Locations, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/appcontent-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/appcontent-get-openapi.md
- name: Urban Airship - Post App Content Product Download
  x-api-slug: appcontentproduct-iddownload-post
  description: Returns a temporary URL where the client can download the content.
    In the payload, the receipt string is the receipt data from the purchase. It should
    be unaltered from how Apple delivers it to your application.udid is an optional
    field to help identify a particular user???s purchases, which can aid debugging.
    It should always be a hash of the UDID, not the actual UDID, to ensure compliance
    with Apple???s TOS. The optional version field should be the StoreFront library
    version, or custom if you???re building your own.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
  humanURL: http://urbanairship.com/
  baseURL: https://go.urbanairship.com//api/
  tags: BaaS, Push Notifications, Stack Network, SaaS, Technology, Mobile, internet,
    Relative Data, Service API, Locations, Locations, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/appcontentproduct-iddownload-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/appcontentproduct-iddownload-post-openapi.md
- name: Urban Airship - Post App Updates
  x-api-slug: appupdates-post
  description: Checks for updates. It can be useful on application launch to compare
    a list of installed updates with our server to see if there are any updates to
    be had for the content.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
  humanURL: http://urbanairship.com/
  baseURL: https://go.urbanairship.com//api/
  tags: BaaS, Push Notifications, Stack Network, SaaS, Technology, Mobile, internet,
    Relative Data, Service API, Locations, Locations, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/appupdates-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/appupdates-post-openapi.md
- name: Urban Airship - Post User Recover
  x-api-slug: userrecover-post
  description: Uses the user???s email address as a way to restore subscription content
    across devices.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
  humanURL: http://urbanairship.com/
  baseURL: https://go.urbanairship.com//api/
  tags: BaaS, Push Notifications, Stack Network, SaaS, Technology, Mobile, internet,
    Relative Data, Service API, Locations, Locations, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/userrecover-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/userrecover-post-openapi.md
- name: Urban Airship - Get User Recover
  x-api-slug: userrecoverid-get
  description: Checks the recovery status.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
  humanURL: http://urbanairship.com/
  baseURL: https://go.urbanairship.com//api/
  tags: BaaS, Push Notifications, Stack Network, SaaS, Technology, Mobile, internet,
    Relative Data, Service API, Locations, Locations, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/userrecoverid-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/userrecoverid-get-openapi.md
- name: Urban Airship - Get User User Available Subscriptions
  x-api-slug: useruser-idavailable-subscriptions-get
  description: Retrieves subscription options.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
  humanURL: http://urbanairship.com/
  baseURL: https://go.urbanairship.com//api/
  tags: BaaS, Push Notifications, Stack Network, SaaS, Technology, Mobile, internet,
    Relative Data, Service API, Locations, Locations, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/useruser-idavailable-subscriptions-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/useruser-idavailable-subscriptions-get-openapi.md
- name: Urban Airship - Post User User Subscriptions Subscription Key Purchase
  x-api-slug: useruser-idsubscriptionssubscription-keypurchase-post
  description: Adds a new subscription.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
  humanURL: http://urbanairship.com/
  baseURL: https://go.urbanairship.com//api/
  tags: BaaS, Push Notifications, Stack Network, SaaS, Technology, Mobile, internet,
    Relative Data, Service API, Locations, Locations, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/useruser-idsubscriptionssubscription-keypurchase-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/useruser-idsubscriptionssubscription-keypurchase-post-openapi.md
- name: Urban Airship - Get User User Subscription Content
  x-api-slug: useruser-idsubscription-content-get
  description: Returns a list of available content.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
  humanURL: http://urbanairship.com/
  baseURL: https://go.urbanairship.com//api/
  tags: BaaS, Push Notifications, Stack Network, SaaS, Technology, Mobile, internet,
    Relative Data, Service API, Locations, Locations, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/useruser-idsubscription-content-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/useruser-idsubscription-content-get-openapi.md
- name: Urban Airship - Post User User Subscriptions Content Content Download
  x-api-slug: useruser-idsubscriptionscontentcontent-iddownload-post
  description: Downloads the content.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
  humanURL: http://urbanairship.com/
  baseURL: https://go.urbanairship.com//api/
  tags: BaaS, Push Notifications, Stack Network, SaaS, Technology, Mobile, internet,
    Relative Data, Service API, Locations, Locations, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/useruser-idsubscriptionscontentcontent-iddownload-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/useruser-idsubscriptionscontentcontent-iddownload-post-openapi.md
- name: Urban Airship - Post Feeds
  x-api-slug: feeds-post
  description: Creates a new feed item.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
  humanURL: http://urbanairship.com/
  baseURL: https://go.urbanairship.com//api/
  tags: BaaS, Push Notifications, Stack Network, SaaS, Technology, Mobile, internet,
    Relative Data, Service API, Locations, Locations, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/feeds-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/feeds-post-openapi.md
- name: Urban Airship - Get Feeds
  x-api-slug: feeds-get
  description: Gets a list of feeds.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
  humanURL: http://urbanairship.com/
  baseURL: https://go.urbanairship.com//api/
  tags: BaaS, Push Notifications, Stack Network, SaaS, Technology, Mobile, internet,
    Relative Data, Service API, Locations, Locations, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/feeds-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/feeds-get-openapi.md
- name: Urban Airship - Get Feeds Feed
  x-api-slug: feedsfeed-id-get
  description: Returns information about a particular feed.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
  humanURL: http://urbanairship.com/
  baseURL: https://go.urbanairship.com//api/
  tags: BaaS, Push Notifications, Stack Network, SaaS, Technology, Mobile, internet,
    Relative Data, Service API, Locations, Locations, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/feedsfeed-id-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/feedsfeed-id-get-openapi.md
- name: Urban Airship - Put Feeds Feed
  x-api-slug: feedsfeed-id-put
  description: Updates a feed.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
  humanURL: http://urbanairship.com/
  baseURL: https://go.urbanairship.com//api/
  tags: BaaS, Push Notifications, Stack Network, SaaS, Technology, Mobile, internet,
    Relative Data, Service API, Locations, Locations, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/feedsfeed-id-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/feedsfeed-id-put-openapi.md
- name: Urban Airship - Delete Feeds Feed
  x-api-slug: feedsfeed-id-delete
  description: Deletes a feed.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
  humanURL: http://urbanairship.com/
  baseURL: https://go.urbanairship.com//api/
  tags: BaaS, Push Notifications, Stack Network, SaaS, Technology, Mobile, internet,
    Relative Data, Service API, Locations, Locations, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/feedsfeed-id-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/feedsfeed-id-delete-openapi.md
- name: Urban Airship - Get Tags
  x-api-slug: tags-get
  description: Returns all the tags that you have created.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
  humanURL: http://urbanairship.com/
  baseURL: https://go.urbanairship.com//api/
  tags: BaaS, Push Notifications, Stack Network, SaaS, Technology, Mobile, internet,
    Relative Data, Service API, Locations, Locations, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/tags-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/tags-get-openapi.md
- name: Urban Airship - Put Tags Tag
  x-api-slug: tagstag-put
  description: Deletes a tag.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
  humanURL: http://urbanairship.com/
  baseURL: https://go.urbanairship.com//api/
  tags: BaaS, Push Notifications, Stack Network, SaaS, Technology, Mobile, internet,
    Relative Data, Service API, Locations, Locations, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/tagstag-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/tagstag-put-openapi.md
- name: Urban Airship - Post Tags Tag
  x-api-slug: tagstag-post
  description: Modifies device tokens on a tag.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
  humanURL: http://urbanairship.com/
  baseURL: https://go.urbanairship.com//api/
  tags: BaaS, Push Notifications, Stack Network, SaaS, Technology, Mobile, internet,
    Relative Data, Service API, Locations, Locations, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/tagstag-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/tagstag-post-openapi.md
- name: Urban Airship - Get Device Tokens Device Token Tags
  x-api-slug: device-tokensdevice-tokentags-get
  description: Gets tags for a specific device token.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
  humanURL: http://urbanairship.com/
  baseURL: https://go.urbanairship.com//api/
  tags: BaaS, Push Notifications, Stack Network, SaaS, Technology, Mobile, internet,
    Relative Data, Service API, Locations, Locations, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/device-tokensdevice-tokentags-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/device-tokensdevice-tokentags-get-openapi.md
- name: Urban Airship - Put Device Tokens Device Token Tags Tag
  x-api-slug: device-tokensdevice-tokentagstag-put
  description: Creates a tag and associate it with the specific device token.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
  humanURL: http://urbanairship.com/
  baseURL: https://go.urbanairship.com//api/
  tags: BaaS, Push Notifications, Stack Network, SaaS, Technology, Mobile, internet,
    Relative Data, Service API, Locations, Locations, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/device-tokensdevice-tokentagstag-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/device-tokensdevice-tokentagstag-put-openapi.md
- name: Urban Airship - Delete Device Tokens Device Token Tags Tag
  x-api-slug: device-tokensdevice-tokentagstag-delete
  description: Removes a single tag from a device token.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
  humanURL: http://urbanairship.com/
  baseURL: https://go.urbanairship.com//api/
  tags: BaaS, Push Notifications, Stack Network, SaaS, Technology, Mobile, internet,
    Relative Data, Service API, Locations, Locations, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/device-tokensdevice-tokentagstag-delete-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/device-tokensdevice-tokentagstag-delete-openapi.md
- name: Urban Airship - Get Partner Apps
  x-api-slug: partnerapps-get
  description: List applications.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
  humanURL: http://urbanairship.com/
  baseURL: https://go.urbanairship.com//api/
  tags: BaaS, Push Notifications, Stack Network, SaaS, Technology, Mobile, internet,
    Relative Data, Service API, Locations, Locations, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/partnerapps-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/partnerapps-get-openapi.md
- name: Urban Airship - Post Partner Apps
  x-api-slug: partnerapps-post
  description: Adds a new application.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
  humanURL: http://urbanairship.com/
  baseURL: https://go.urbanairship.com//api/
  tags: BaaS, Push Notifications, Stack Network, SaaS, Technology, Mobile, internet,
    Relative Data, Service API, Locations, Locations, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/partnerapps-post-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/partnerapps-post-openapi.md
- name: Urban Airship - Put Partner Apps App
  x-api-slug: partnerappsapp-id-put
  description: Updates an application.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/75-urban-airship.jpg
  humanURL: http://urbanairship.com/
  baseURL: https://go.urbanairship.com//api/
  tags: BaaS, Push Notifications, Stack Network, SaaS, Technology, Mobile, internet,
    Relative Data, Service API, Locations, Locations, Relative StreamRank, Streams
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/partnerappsapp-id-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-organizations/urban-airship/master/_listings/urban-airship/partnerappsapp-id-put-openapi.md
x-common:
- type: x-website
  url: http://urbanairship.com/
- type: x-android-sdk
  url: http://docs.urbanairship.com/platform/android.html
- type: x-api-gallery
  url: http://ulster.bank.api.gallery.streamdata.io
- type: x-api-stack
  url: http://urban.airship.stack.network
- type: x-blackberry-sdk
  url: http://docs.urbanairship.com/platform/blackberry.html
- type: x-blog
  url: http://urbanairship.com/blog
- type: x-blog-rss
  url: http://urbanairship.com/blog/rss
- type: x-case-studies
  url: http://urbanairship.com/resources/case-studies
- type: x-crunchbase
  url: http://www.crunchbase.com/company/urban-airship
- type: x-crunchbase
  url: https://crunchbase.com/organization/urban-airship
- type: x-developer
  url: http://docs.urbanairship.com/
- type: x-email
  url: legal@urbanairship.com
- type: x-email
  url: privacy@urbanairship.com
- type: x-email
  url: support@urbanairship.com
- type: x-github
  url: https://github.com/urbanairship
- type: x-glossary
  url: http://docs.urbanairship.com/reference/glossary.html
- type: x-ios-sdk
  url: http://docs.urbanairship.com/platform/ios.html
- type: x-linkedin
  url: https://www.linkedin.com/company/urban-airship/
- type: x-phonegap-sdk
  url: http://docs.urbanairship.com/platform/phonegap.html
- type: x-pricing
  url: https://www.urbanairship.com/products/engage/pricing
- type: x-privacy
  url: http://urbanairship.com/legal/privacy-policy
- type: x-security
  url: http://docs.urbanairship.com/reference/app_keys_secrets.html
- type: x-twitter
  url: https://twitter.com/urbanairship
- type: x-website
  url: http://urbanairship.com
- type: x-white-papers
  url: http://urbanairship.com/resources/whitepapers
- type: x-windows-sdk
  url: http://docs.urbanairship.com/platform/windows.html
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---