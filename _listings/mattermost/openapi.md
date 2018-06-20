---
swagger: "2.0"
x-collection-name: Mattermost
x-complete: 1
info:
  title: Mattermost API Reference
  description: -api-v4-is-stable-with-the-mattermost-server-4-0-release--api-v3-was-deprecated-on-january-16th-2018-and-scheduled-for-removal-in-mattermost-v5-0--details-heretagapiv3deprecation--looking-for-the-api-v3-reference-it-has-moved-herehttpsapi-mattermost-comv3-
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
  /plugins/webapp:
    get:
      summary: Get webapp plugins
      description: |-
        Get a list of web app plugins installed and activated on the server.

        ##### Permissions
        No permissions required.

        __Minimum server version__: 4.4
      operationId: get-a-list-of-web-app-plugins-installed-and-activated-on-the-server-permissionsno-permissions-requir
      x-api-path-slug: pluginswebapp-get
      responses:
        200:
          description: OK
      tags:
      - Webapp
      - Plugins
---