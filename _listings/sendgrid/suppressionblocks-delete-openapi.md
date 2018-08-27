---
swagger: "2.0"
x-collection-name: SendGrid
x-complete: 0
info:
  title: SendGrid Delete Suppression Blocks
  description: "**This endpoint allows you to delete all email addresses on your blocks
    list.**\n\nThere are two options for deleting blocked emails: \n\n1. You can delete
    all blocked emails by setting `delete_all` to true in the request body. \n2. You
    can delete some blocked emails by specifying the email addresses in an array in
    the request body.\n\n[Blocks](https://sendgrid.com/docs/Glossary/blocks.html)
    happen when your message was rejected for a reason related to the message, not
    the recipient address. This can happen when your mail server IP address has been
    added to a blacklist or blocked by an ISP, or if the message content is flagged
    by a filter on the receiving server.\n\nFor more information, please see our [User
    Guide](https://sendgrid.com/docs/User_Guide/Suppressions/blocks.html)."
  version: 1.0.0
host: api.sendgrid.com
basePath: /v3
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /suppression/blocks:
    delete:
      summary: Delete Suppression Blocks
      description: "**This endpoint allows you to delete all email addresses on your
        blocks list.**\n\nThere are two options for deleting blocked emails: \n\n1.
        You can delete all blocked emails by setting `delete_all` to true in the request
        body. \n2. You can delete some blocked emails by specifying the email addresses
        in an array in the request body.\n\n[Blocks](https://sendgrid.com/docs/Glossary/blocks.html)
        happen when your message was rejected for a reason related to the message,
        not the recipient address. This can happen when your mail server IP address
        has been added to a blacklist or blocked by an ISP, or if the message content
        is flagged by a filter on the receiving server.\n\nFor more information, please
        see our [User Guide](https://sendgrid.com/docs/User_Guide/Suppressions/blocks.html)."
      operationId: suppression.blocks.delete
      x-api-path-slug: suppressionblocks-delete
      parameters:
      - in: body
        name: body
        schema:
          $ref: '#/definitions/holder'
      - in: query
        name: No Name
      responses:
        200:
          description: OK
      tags:
      - Email
      - Suppression
      - Blocks
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