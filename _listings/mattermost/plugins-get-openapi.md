---
swagger: "2.0"
x-collection-name: Mattermost
x-complete: 0
info:
  title: Mattermost API Get plugins
  description: |-
    Get a list of inactive and a list of active plugin manifests. Plugins must be enabled in the server's config settings.

    ##### Permissions
    Must have `manage_system` permission.

    __Minimum server version__: 4.4
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
  /plugins:
    get:
      summary: Get plugins
      description: |-
        Get a list of inactive and a list of active plugin manifests. Plugins must be enabled in the server's config settings.

        ##### Permissions
        Must have `manage_system` permission.

        __Minimum server version__: 4.4
      operationId: get-a-list-of-inactive-and-a-list-of-active-plugin-manifests-plugins-must-be-enabled-in-the-servers-
      x-api-path-slug: plugins-get
      responses:
        200:
          description: OK
      tags:
      - Plugins
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