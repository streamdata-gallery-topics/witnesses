---
swagger: "2.0"
x-collection-name: Steem
x-complete: 0
info:
  title: Steem get_witnesses_by_vote
  description: get_witnesses_by_vote
  version: 1.0.0
host: api.steemjs.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /get_witnesses:
    get:
      summary: get_witnesses
      description: get_witnesses
      operationId: get-witnesses
      x-api-path-slug: get-witnesses-get
      parameters:
      - in: query
        name: witnessIds
        description: witnessIds
      responses:
        200:
          description: OK
      tags:
      - Get
      - Witnesses
  /get_witnesses_by_vote:
    get:
      summary: get_witnesses_by_vote
      description: get_witnesses_by_vote
      operationId: get-witnesses-by-vote
      x-api-path-slug: get-witnesses-by-vote-get
      parameters:
      - in: query
        name: from
        description: from witness
      - in: query
        name: limit
        description: limit
      responses:
        200:
          description: OK
      tags:
      - Get
      - Witnesses
      - By
      - Vote
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