swagger: "2.0"
x-collection-name: Blockchain
x-complete: 1
info:
  title: Blockchain
  version: 1.0.0
host: blockchain.info
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /rawblock/{block_hash}:
    get:
      summary: Raw Block
      description: Returns a single raw block.
      operationId: getRawBlock
      x-api-path-slug: rawblockblock-hash-get
      parameters:
      - in: path
        name: block_hash
        description: The block hash
        type: string
        format: string
      responses:
        200:
          description: OK
      tags:
      - Blockchain
      - Blocks