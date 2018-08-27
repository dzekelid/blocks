---
swagger: "2.0"
x-collection-name: Lisk
x-complete: 0
info:
  title: Lisk Requests blocks data
  description: Search for a specified block in the system.
  version: 1.0.0
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /blocks:
    get:
      summary: Requests blocks data
      description: Search for a specified block in the system.
      operationId: getBlocks
      x-api-path-slug: blocks-get
      parameters:
      - in: query
        name: blockId
        description: Block id to query
      - in: query
        name: generatorPublicKey
        description: Public key of the forger of the block
      - in: query
        name: height
        description: Current height of the network
      - in: query
        name: limit
        description: Limit applied to results
      - in: query
        name: offset
        description: Offset value for results
      - in: query
        name: sort
        description: Fields to sort results by
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Blocks
      - Data
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