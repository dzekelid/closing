---
swagger: "2.0"
x-collection-name: VersaPay
x-complete: 0
info:
  title: VersaPay Open and Closed Disputes
  description: Open and closed disputes since watermark, limited to 100 disputes at
    a time.
  contact:
    name: VersaPay Support
    url: https://www.versapay.com/support
    email: support@versapay.com
  version: 1.0.0
host: secure.versapay.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/exports/disputes:
    get:
      summary: Open and Closed Disputes
      description: Open and closed disputes since watermark, limited to 100 disputes
        at a time.
      operationId: getDisputes
      x-api-path-slug: apiexportsdisputes-get
      parameters:
      - in: query
        name: watermark
        description: The date value to base a subsequent extract of the next 100 disputes
      responses:
        200:
          description: OK
      tags:
      - OpenClosed
      - Disputes
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