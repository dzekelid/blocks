---
swagger: "2.0"
x-collection-name: RipaEx
x-complete: 0
info:
  title: RipaEx Blocks Get Fees
  description: Get the network fees.
  version: 1.0.0
host: api.ripaex.io
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/blocks/get:
    get:
      summary: Blocks Get
      description: Get block by id.
      operationId: blocks.getBlock
      x-api-path-slug: apiblocksget-get
      parameters:
      - in: query
        name: id
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Blocks
  /api/blocks:
    get:
      summary: Blocks
      description: Get all blocks.
      operationId: blocks.getBlocks
      x-api-path-slug: apiblocks-get
      parameters:
      - in: query
        name: generatorPublicKey
        description: A valid RIPA Public Key
      - in: query
        name: height
      - in: query
        name: limit
        description: An unsigned integer that specifies the maximum number of records
      - in: query
        name: offset
        description: An unsigned integer that specified the number of records to skip
      - in: query
        name: orderBy
        description: A string that specifies the column by which to sort the records
      - in: query
        name: previousBlock
      - in: query
        name: reward
      - in: query
        name: totalAmount
      - in: query
        name: totalFee
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Blocks
  /api/blocks/getEpoch:
    get:
      summary: Blocks Get Epoch
      description: Get the blockchain epoch.
      operationId: blocks.getEpoch
      x-api-path-slug: apiblocksgetepoch-get
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Blocks
      - ""
      - Epoch
  /api/blocks/getHeight:
    get:
      summary: Blocks Get Height
      description: Get the blockchain height.
      operationId: blocks.getHeight
      x-api-path-slug: apiblocksgetheight-get
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Blocks
      - ""
      - Height
  /api/blocks/getNethash:
    get:
      summary: Blocks Get Nethash
      description: Get the blockchain nethash.
      operationId: blocks.getNethash
      x-api-path-slug: apiblocksgetnethash-get
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Blocks
      - ""
      - Nethash
  /api/blocks/getFee:
    get:
      summary: Blocks Get Fee
      description: Get the transaction fee for sending "normal" transactions.
      operationId: blocks.getFee
      x-api-path-slug: apiblocksgetfee-get
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Blocks
      - ""
      - Fee
  /api/blocks/getFees:
    get:
      summary: Blocks Get Fees
      description: Get the network fees.
      operationId: blocks.getFees
      x-api-path-slug: apiblocksgetfees-get
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Blocks
      - ""
      - Fees
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