---
swagger: "2.0"
x-collection-name: Mattermost
x-complete: 0
info:
  title: Mattermost API Cancel a job.
  description: |-
    Cancel a job.
    __Minimum server version: 4.1__
    ##### Permissions
    Must have `manage_jobs` permission.
  termsOfService: https://about.mattermost.com/default-terms/
  version: 4.0.0
host: your-mattermost-url.com
basePath: /api/v4
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /jobs/{job_id}/cancel:
    post:
      summary: Cancel a job.
      description: |-
        Cancel a job.
        __Minimum server version: 4.1__
        ##### Permissions
        Must have `manage_jobs` permission.
      operationId: cancel-a-job-minimum-server-version-41--permissionsmust-have-manage-jobs-permission
      x-api-path-slug: jobsjob-idcancel-post
      parameters:
      - in: path
        name: job_id
        description: Job GUID
      responses:
        200:
          description: OK
      tags:
      - Cancel
      - Job.
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