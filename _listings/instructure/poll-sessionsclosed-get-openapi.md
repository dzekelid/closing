---
swagger: "2.0"
x-collection-name: Instructure
x-complete: 0
info:
  title: Instructure Canvas Polls API List closed poll sessions
  description: List closed poll sessions.
  termsOfService: https://www.canvaslms.com/policies/api-policy
  version: v1
host: canvas.instructure.com
basePath: /api/v1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /polls/{poll_id}/poll_sessions/id/close:
    get:
      summary: Close an opened poll session
      description: Close an opened poll session.
      operationId: close-an-opened-poll-session
      x-api-path-slug: pollspoll-idpoll-sessionsidclose-get
      responses:
        200:
          description: OK
      tags:
      - Polls
      - Poll
      - Id
      - Poll
      - Sessions
      - Id
      - Close
  /poll_sessions/closed:
    get:
      summary: List closed poll sessions
      description: List closed poll sessions.
      operationId: list-closed-poll-sessions
      x-api-path-slug: poll-sessionsclosed-get
      responses:
        200:
          description: OK
      tags:
      - Poll
      - Sessions
      - Closed
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