swagger: "2.0"
x-collection-name: GitLab
x-complete: 1
info:
  title: API title
  version: 1.0.0
host: localhost:3000
basePath: /api
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /v3/projects/{id}/merge_request/{merge_request_id}/closes_issues:
    get:
      summary: Get Projects Merge Request Merge Request Closes Issues
      description: Get projects merge request merge request closes issues.
      operationId: getV3ProjectsIdMergeRequestMergeRequestIdClosesIssues
      x-api-path-slug: v3projectsidmerge-requestmerge-request-idcloses-issues-get
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: merge_request_id
      - in: query
        name: page
        description: Current page number
      - in: query
        name: per_page
        description: Number of items per page
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Merge
      - Request
      - Merge
      - Request
      - Closes
      - Issues
  /v3/projects/{id}/merge_requests/{merge_request_id}/closes_issues:
    get:
      summary: Get Projects Merge Requests Merge Request Closes Issues
      description: Get projects merge requests merge request closes issues.
      operationId: getV3ProjectsIdMergeRequestsMergeRequestIdClosesIssues
      x-api-path-slug: v3projectsidmerge-requestsmerge-request-idcloses-issues-get
      parameters:
      - in: path
        name: id
        description: The ID of a project
      - in: path
        name: merge_request_id
      - in: query
        name: page
        description: Current page number
      - in: query
        name: per_page
        description: Number of items per page
      responses:
        200:
          description: OK
      tags:
      - Projects
      - Merge
      - Requests
      - Merge
      - Request
      - Closes
      - Issues