---
swagger: "2.0"
x-collection-name: Rebilly
x-complete: 0
info:
  title: Rebilly Cancel a subscription
  description: Cancel a subscription
  termsOfService: https://www.rebilly.com/terms/
  contact:
    name: Rebilly API Support
    url: https://www.rebilly.com/contact/
    email: integrations@rebilly.com
  version: "2.1"
host: api.rebilly.com
basePath: /v2.1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /coupons-redemptions/{id}/cancel:
    post:
      summary: Cancel a coupon redemption
      description: ""
      operationId: coupons_redemptions.id.cancel.post
      x-api-path-slug: couponsredemptionsidcancel-post
      responses:
        200:
          description: OK
      tags:
      - Cancel
      - Coupon
      - Redemption
  /subscriptions/{id}/cancel:
    post:
      summary: Cancel a subscription
      description: Cancel a subscription
      operationId: subscriptions.id.cancel.post
      x-api-path-slug: subscriptionsidcancel-post
      parameters:
      - in: body
        name: body
        description: Only policy
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Cancel
      - Subscription
x-streamrank:
  polling_total_time_average: 0
  polling_size_download_average: 0
  streaming_total_time_average: 0
  streaming_size_download_average: 0
  change_yes: 0
  change_no: 0
  time_percentage: 0
  size_percentage: 0
  change_percentage: 0
  last_run: ""
  days_run: 0
  minute_run: 0
---