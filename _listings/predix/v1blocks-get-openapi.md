---
swagger: "2.0"
x-collection-name: Predix
x-complete: 0
info:
  title: Predix BlockChain Get Blocks
  description: Get current blockchain root info
  version: 1.0.0
host: predix-apphub-arcs-prod.run.aws-usw02-pr.ice.predix.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v1/blocks:
    get:
      summary: Get Blocks
      description: Get current blockchain root info
      operationId: get-current-blockchain-root-info
      x-api-path-slug: v1blocks-get
      parameters:
      - in: header
        name: Authorization
        description: access token
      - in: header
        name: predix-zone-id
        description: tenantId
      responses:
        200:
          description: OK
      tags:
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