---
swagger: "2.0"
x-collection-name: Steem
x-complete: 0
info:
  title: Steem witness_update
  description: witness_update
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
  /get_active_witnesses:
    get:
      summary: get_active_witnesses
      description: get_active_witnesses
      operationId: get-active-witnesses
      x-api-path-slug: get-active-witnesses-get
      responses:
        200:
          description: OK
      tags:
      - Get
      - Active
      - Witnesses
  /get_witness_count:
    get:
      summary: get_witness_count
      description: get_witness_count
      operationId: get-witness-count
      x-api-path-slug: get-witness-count-get
      responses:
        200:
          description: OK
      tags:
      - Get
      - Witness
      - Count
  /lookup_witness_accounts:
    get:
      summary: lookup_witness_accounts
      description: lookup_witness_accounts regex search
      operationId: lookup-witness-accounts-regex-search
      x-api-path-slug: lookup-witness-accounts-get
      parameters:
      - in: query
        name: limit
        description: limit
      - in: query
        name: lowerBoundName
        description: lowerBoundName
      responses:
        200:
          description: OK
      tags:
      - Lookup
      - Witness
      - Accounts
  /get_witness_schedule:
    get:
      summary: get_witness_schedule
      description: get_witness_schedule
      operationId: get-witness-schedule
      x-api-path-slug: get-witness-schedule-get
      responses:
        200:
          description: OK
      tags:
      - Get
      - Witness
      - Schedule
  /get_witness_by_account:
    get:
      summary: get_witness_by_account
      description: get_witness_by_account
      operationId: get-witness-by-account
      x-api-path-slug: get-witness-by-account-get
      parameters:
      - in: query
        name: accountName
        description: witness account name
      responses:
        200:
          description: OK
      tags:
      - Get
      - Witness
      - By
      - Account
  /witness_update:
    get:
      summary: witness_update
      description: witness_update
      operationId: witness-update
      x-api-path-slug: witness-update-get
      parameters:
      - in: query
        name: block_signing_key
        description: block_signing_key
      - in: query
        name: fee
        description: fee
      - in: query
        name: owner
        description: witness name
      - in: query
        name: props
        description: props
      - in: query
        name: url
        description: url
      responses:
        200:
          description: OK
      tags:
      - Witness
      - Update
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