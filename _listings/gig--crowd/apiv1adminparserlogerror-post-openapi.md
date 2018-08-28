---
swagger: "2.0"
x-collection-name: GIG & CROWD
x-complete: 0
info:
  title: GIGANDCROWD Post Admin Parser Log Error
  version: 1.0.0
  description: Post admin parser log error.
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
  /api/v1/admin/parser/logs:
    get:
      summary: Get Admin Parser Logs
      description: Get admin parser logs.
      operationId: getApiV1AdminParserLogs
      x-api-path-slug: apiv1adminparserlogs-get
      parameters:
      - in: header
        name: Authorization
      - in: query
        name: request.from
      - in: query
        name: request.query
      - in: query
        name: request.to
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Parser
      - Logs
  /api/v1/admin/parser/statistic:
    get:
      summary: Get Admin Parser Statistic
      description: Get admin parser statistic.
      operationId: getApiV1AdminParserStatistic
      x-api-path-slug: apiv1adminparserstatistic-get
      parameters:
      - in: header
        name: Authorization
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Parser
      - Statistic
  /api/v1/admin/parser/log/error:
    post:
      summary: Post Admin Parser Log Error
      description: Post admin parser log error.
      operationId: postApiV1AdminParserLogError
      x-api-path-slug: apiv1adminparserlogerror-post
      parameters:
      - in: header
        name: Authorization
      - in: body
        name: request
        schema:
          $ref: '#/definitions/holder'
      responses:
        200:
          description: OK
      tags:
      - Admin
      - Parser
      - Log
      - Error
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