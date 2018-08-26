---
swagger: "2.0"
x-collection-name: OpenRouteService
x-complete: 0
info:
  title: AP Metadata Services Authority
  description: Returns a document for the specified authority and format with the
    AP vocabulary data for the  specified term GUID and the subset of the vocabulary
    located below the specified term.
  version: v1
host: cv.ap.org
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  d/{authority}/{GUID}.{format}:
    get:
      summary: Authority
      description: Returns a document for the specified authority and format with
        the AP vocabulary data for the  specified term GUID and the subset of the
        vocabulary located below the specified term.
      operationId: getDAuthorityGu.Format
      x-api-path-slug: dauthorityguid-format-get
      parameters:
      - in: query
        name: apikey
        description: API Key
      - in: path
        name: authority
        description: The name of a classification authority (not case-sensitive)
      - in: path
        name: format
        description: The format of the returned taxonomy data
      - in: path
        name: GUID
        description: The GUID of an AP term below which the returned taxonomy data  subset
          is located in the AP taxonomy hierarchy
      responses:
        200:
          description: OK
      tags:
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