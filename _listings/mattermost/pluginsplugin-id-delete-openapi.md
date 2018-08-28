---
swagger: "2.0"
x-collection-name: Mattermost
x-complete: 0
info:
  title: Mattermost API Remove plugin
  description: |-
    Remove the plugin with the provided ID from the server. All plugin files are deleted. Plugins must be enabled in the server's config settings.

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
    post:
      summary: Upload plugin
      description: |-
        Upload a plugin compressed in a .tar.gz file. Plugins and plugin uploads must be enabled in the server's config settings.

        ##### Permissions
        Must have `manage_system` permission.

        __Minimum server version__: 4.4
      operationId: upload-a-plugin-compressed-in-a-targz-file-plugins-and-plugin-uploads-must-be-enabled-in-the-servers
      x-api-path-slug: plugins-post
      parameters:
      - in: formData
        name: plugin
        description: The plugin image to be uploaded
      responses:
        200:
          description: OK
      tags:
      - Upload
      - Plugin
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
  /plugins/{plugin_id}:
    delete:
      summary: Remove plugin
      description: |-
        Remove the plugin with the provided ID from the server. All plugin files are deleted. Plugins must be enabled in the server's config settings.

        ##### Permissions
        Must have `manage_system` permission.

        __Minimum server version__: 4.4
      operationId: remove-the-plugin-with-the-provided-id-from-the-server-all-plugin-files-are-deleted-plugins-must-be-
      x-api-path-slug: pluginsplugin-id-delete
      parameters:
      - in: path
        name: plugin_id
      responses:
        200:
          description: OK
      tags:
      - Remove
      - Plugin
  /plugins/{plugin_id}/activate:
    post:
      summary: Activate plugin
      description: |-
        Activate a previously uploaded plugin. Plugins must be enabled in the server's config settings.

        ##### Permissions
        Must have `manage_system` permission.

        __Minimum server version__: 4.4
      operationId: activate-a-previously-uploaded-plugin-plugins-must-be-enabled-in-the-servers-config-settings-permiss
      x-api-path-slug: pluginsplugin-idactivate-post
      parameters:
      - in: path
        name: plugin_id
      responses:
        200:
          description: OK
      tags:
      - Activate
      - Plugin
  /plugins/{plugin_id}/deactivate:
    post:
      summary: Deactivate plugin
      description: |-
        Deactivate a previously activated plugin. Plugins must be enabled in the server's config settings.

        ##### Permissions
        Must have `manage_system` permission.

        __Minimum server version__: 4.4
      operationId: deactivate-a-previously-activated-plugin-plugins-must-be-enabled-in-the-servers-config-settings-perm
      x-api-path-slug: pluginsplugin-iddeactivate-post
      parameters:
      - in: path
        name: plugin_id
      responses:
        200:
          description: OK
      tags:
      - Deactivate
      - Plugin
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