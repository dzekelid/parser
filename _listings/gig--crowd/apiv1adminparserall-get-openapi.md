---
swagger: "2.0"
x-collection-name: GIG & CROWD
x-complete: 0
info:
  title: GIGANDCROWD Get Admin Parser All
  version: 1.0.0
  description: Get admin parser all.
host: gigandcrowd.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/v1/admin/parser/config:
    get:
      summary: Get Admin Parser Config
      description: Get admin parser config.
      operationId: getApiV1AdminParserConfig
      x-api-path-slug: apiv1adminparserconfig-get
      parameters:
      - in: header
        name: Authorization
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Parser
      - Config
  /api/v1/admin/parser/all:
    get:
      summary: Get Admin Parser All
      description: Get admin parser all.
      operationId: getApiV1AdminParserAll
      x-api-path-slug: apiv1adminparserall-get
      parameters:
      - in: header
        name: Authorization
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Parser
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