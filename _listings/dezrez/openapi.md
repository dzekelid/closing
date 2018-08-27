swagger: "2.0"
x-collection-name: Dezrez
x-complete: 1
info:
  title: Dezrez.Rezi.Client.Api
  version: 1.0.0
host: api.dezrez.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /api/role/{id}/setclosingdate:
    post:
      summary: Sets the role closing date
      description: Sets the role closing date.
      operationId: Role_SetClosingDateByidBydataContract
      x-api-path-slug: apiroleidsetclosingdate-post
      parameters:
      - in: body
        name: dataContract
        description: The closing data datacontract
        schema:
          $ref: '#/definitions/holder'
      - in: path
        name: id
        description: The id of the role
      - in: header
        name: Rezi-Api-Version
        description: Specifies which version of the API to call
      responses:
        200:
          description: OK
      tags:
      - Sets
      - Role
      - Closing
      - Date