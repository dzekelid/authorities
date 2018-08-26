---
swagger: "2.0"
x-collection-name: OpenRouteService
x-complete: 1
info:
  title: AP Metadata Services
  description: add-value-to-your-news-content-with-apu2019s-industryleading-metadata--accurate-comprehensive-richly-detailed-data-designed-specifically-for-use-by-news-publishers--ap-metadata-services-is-a-new-set-of-apis-that-gives-you-direct-access-to-the-same-metadata-system-that-supports-apu2019s-awardwinning-global-news-operation-
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
---