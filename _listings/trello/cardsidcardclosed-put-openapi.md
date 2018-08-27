---
swagger: "2.0"
x-collection-name: Trello
x-complete: 0
info:
  title: Trello Put Cards Closed
  description: Put cards closed.
  termsOfService: https://trello.com/legal
  contact:
    name: Trello
    url: https://trello.com/home
  version: "1.0"
host: trello.com
basePath: /1
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /boards/{idBoard}/closed:
    put:
      summary: Put Boards Closed
      description: Put boards closed.
      operationId: updateBoardsClosedByIdBoard
      x-api-path-slug: boardsidboardclosed-put
      parameters:
      - in: body
        name: body
        description: Attributes of Boards Closed to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idBoard
        description: board_id
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Boards
      - Closed
  /cards/{idCard}/closed:
    put:
      summary: Put Cards Closed
      description: Put cards closed.
      operationId: updateCardsClosedByIdCard
      x-api-path-slug: cardsidcardclosed-put
      parameters:
      - in: body
        name: body
        description: Attributes of Cards Closed to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idCard
        description: card id or shortlink
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Cards
      - Closed
  /lists/{idList}/closed:
    put:
      summary: Put Lists List Closed
      description: Put lists list closed.
      operationId: updateListsClosedByIdList
      x-api-path-slug: listsidlistclosed-put
      parameters:
      - in: body
        name: body
        description: Attributes of Lists Closed to be updated
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: idList
        description: idList
      - in: query
        name: key
        description: Generate your application key
      - in: query
        name: token
        description: Getting a token from a user
      responses:
        200:
          description: OK
      tags:
      - Lists
      - List
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