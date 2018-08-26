---
swagger: "2.0"
x-collection-name: Steem
x-complete: 0
info:
  title: Steem verify_account_authority
  description: verify_account_authority
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
  /verify_authority:
    get:
      summary: verify_authority
      description: verify_authority
      operationId: verify-authority
      x-api-path-slug: verify-authority-get
      parameters:
      - in: query
        name: trx
        description: transaction
      responses:
        200:
          description: OK
      tags:
      - Verify
      - Authority
  /verify_account_authority:
    get:
      summary: verify_account_authority
      description: verify_account_authority
      operationId: verify-account-authority
      x-api-path-slug: verify-account-authority-get
      parameters:
      - in: query
        name: nameOrId
        description: nameOrId
      - in: query
        name: signers
        description: signers
      responses:
        200:
          description: OK
      tags:
      - Verify
      - Account
      - Authority
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