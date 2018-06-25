---
name: Swagger
x-slug: swagger
description: Swagger aides in development across the entire API lifecycle, from design
  and documentation, to test and deployment. Try it today!
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/18963-swaggerhub.jpg
x-kinRank: "8"
x-alexaRank: "23056"
tags: Plugins
created: "2018-06-25"
modified: "2018-06-25"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/plugins/master/_listings/swagger/apis.md
specificationVersion: "0.14"
apis:
- name: Swagger Hub Registry Retrieves a list of all available plugins (ignore system
    plugins)
  x-api-slug: swagger-hub-registry
  description: Retrieves a list of all available plugins (ignore system plugins).
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/18963-swaggerhub.jpg
  humanURL: https://swagger.io/
  baseURL: https://api.swaggerhub.com////plugins
  tags: Plugins
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/plugins/master/_listings/swagger/plugins-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/plugins/master/_listings/swagger/plugins-get-openapi.md
- name: Swagger Hub Registry Deletes the provided Plugin configuration
  x-api-slug: swagger-hub-registry
  description: Deletes the provided plugin configuration.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/18963-swaggerhub.jpg
  humanURL: https://swagger.io/
  baseURL: https://api.swaggerhub.com////plugins/configurations
  tags: Plugins,Configurations
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/plugins/master/_listings/swagger/pluginsconfigurations-delete-openapi.md
- name: Swagger Hub Registry Retrieves a list of enabled plugin configurations
  x-api-slug: swagger-hub-registry
  description: Retrieves a list of enabled plugin configurations.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/18963-swaggerhub.jpg
  humanURL: https://swagger.io/
  baseURL: https://api.swaggerhub.com////plugins/configurations
  tags: Plugins,Configurations
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/plugins/master/_listings/swagger/pluginsconfigurations-get-openapi.md
- name: Swagger Hub Registry Saves the provided Plugin configuration
  x-api-slug: swagger-hub-registry
  description: Saves the provided plugin configuration.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/18963-swaggerhub.jpg
  humanURL: https://swagger.io/
  baseURL: https://api.swaggerhub.com////plugins/configurations
  tags: Plugins,Configurations
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/plugins/master/_listings/swagger/pluginsconfigurations-post-openapi.md
- name: Swagger Hub Registry Updated the provided Plugin configuration
  x-api-slug: swagger-hub-registry
  description: Updated the provided plugin configuration.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/18963-swaggerhub.jpg
  humanURL: https://swagger.io/
  baseURL: https://api.swaggerhub.com////plugins/configurations
  tags: Plugins,Configurations
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/plugins/master/_listings/swagger/pluginsconfigurations-put-openapi.md
- name: Swagger Hub Registry triggers execution of plugin configuration identified
    by id
  x-api-slug: swagger-hub-registry
  description: Triggers execution of plugin configuration identified by id.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/18963-swaggerhub.jpg
  humanURL: https://swagger.io/
  baseURL: https://api.swaggerhub.com////plugins/configurations/execute/{id}
  tags: Plugins,Configurations,Execute,Id
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/plugins/master/_listings/swagger/pluginsconfigurationsexecuteid-post-openapi.md
- name: Swagger Hub Registry get configuration schema for the provided Plugin configuration
  x-api-slug: swagger-hub-registry
  description: Get configuration schema for the provided plugin configuration.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/18963-swaggerhub.jpg
  humanURL: https://swagger.io/
  baseURL: https://api.swaggerhub.com////plugins/configurations/schema
  tags: Plugins,Configurations,Schema
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/plugins/master/_listings/swagger/pluginsconfigurationsschema-post-openapi.md
- name: Swagger Hub Registry
  x-api-slug: swagger-hub-registry
  description: Swagger aides in development across the entire API lifecycle, from
    design and documentation, to test and deployment. Try it today!
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/18963-swaggerhub.jpg
  humanURL: https://swagger.io/
  baseURL: https://api.swaggerhub.com//
  tags: Plugins
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/plugins/master/_listings/swagger/openapi.md
x-common:
- type: x-website
  url: https://swagger.io/
- type: x-crunchbase
  url: https://crunchbase.com/organization/swagger
- type: x-github
  url: https://github.com/swagger-hub
- type: x-twitter
  url: https://twitter.com/swaggerhub
- type: x-twitter
  url: https://twitter.com/SwaggerApi
- type: x-website
  url: http://swaggerhub.com
- type: x-website
  url: https://swaggerhub.com/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---