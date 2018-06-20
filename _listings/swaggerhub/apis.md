---
name: SwaggerHub
x-slug: swaggerhub
description: The place for teams to collaborate and coordinate the entire workflow
  of an APIs lifecycle. SwaggerHub&rsquo;s built-in editors let you rapidly create
  the Swagger definition that everything else is based on, in an intuitive interface
  that lets you write, visualize and validate all at the same time.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/SwaggerHub_Logo_Horizontal_Color.png
x-kinRank: "8"
x-alexaRank: "0"
tags: Plugins
created: "2018-06-20"
modified: "2018-06-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/plugins/master/_listings/swaggerhub/apis.md
specificationVersion: "0.14"
apis:
- name: Swagger Hub Registry Retrieves a list of all available plugins (ignore system
    plugins)
  x-api-slug: swagger-hub-registry
  description: Retrieves a list of all available plugins (ignore system plugins).
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/SwaggerHub_Logo_Horizontal_Color.png
  humanURL: http://swaggerhub.com
  baseURL: https://api.swaggerhub.com////plugins
  tags: Plugins
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/plugins/master/_listings/swaggerhub/plugins-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/plugins/master/_listings/swaggerhub/plugins-get-openapi.md
- name: Swagger Hub Registry Deletes the provided Plugin configuration
  x-api-slug: swagger-hub-registry
  description: Deletes the provided plugin configuration.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/SwaggerHub_Logo_Horizontal_Color.png
  humanURL: http://swaggerhub.com
  baseURL: https://api.swaggerhub.com////plugins/configurations
  tags: Plugins,Configurations
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/plugins/master/_listings/swaggerhub/pluginsconfigurations-delete-openapi.md
- name: Swagger Hub Registry Retrieves a list of enabled plugin configurations
  x-api-slug: swagger-hub-registry
  description: Retrieves a list of enabled plugin configurations.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/SwaggerHub_Logo_Horizontal_Color.png
  humanURL: http://swaggerhub.com
  baseURL: https://api.swaggerhub.com////plugins/configurations
  tags: Plugins,Configurations
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/plugins/master/_listings/swaggerhub/pluginsconfigurations-get-openapi.md
- name: Swagger Hub Registry Saves the provided Plugin configuration
  x-api-slug: swagger-hub-registry
  description: Saves the provided plugin configuration.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/SwaggerHub_Logo_Horizontal_Color.png
  humanURL: http://swaggerhub.com
  baseURL: https://api.swaggerhub.com////plugins/configurations
  tags: Plugins,Configurations
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/plugins/master/_listings/swaggerhub/pluginsconfigurations-post-openapi.md
- name: Swagger Hub Registry Updated the provided Plugin configuration
  x-api-slug: swagger-hub-registry
  description: Updated the provided plugin configuration.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/SwaggerHub_Logo_Horizontal_Color.png
  humanURL: http://swaggerhub.com
  baseURL: https://api.swaggerhub.com////plugins/configurations
  tags: Plugins,Configurations
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/plugins/master/_listings/swaggerhub/pluginsconfigurations-put-openapi.md
- name: Swagger Hub Registry triggers execution of plugin configuration identified
    by id
  x-api-slug: swagger-hub-registry
  description: Triggers execution of plugin configuration identified by id.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/SwaggerHub_Logo_Horizontal_Color.png
  humanURL: http://swaggerhub.com
  baseURL: https://api.swaggerhub.com////plugins/configurations/execute/{id}
  tags: Plugins,Configurations,Execute,Id
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/plugins/master/_listings/swaggerhub/pluginsconfigurationsexecuteid-post-openapi.md
- name: Swagger Hub Registry get configuration schema for the provided Plugin configuration
  x-api-slug: swagger-hub-registry
  description: Get configuration schema for the provided plugin configuration.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/SwaggerHub_Logo_Horizontal_Color.png
  humanURL: http://swaggerhub.com
  baseURL: https://api.swaggerhub.com////plugins/configurations/schema
  tags: Plugins,Configurations,Schema
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/plugins/master/_listings/swaggerhub/pluginsconfigurationsschema-post-openapi.md
- name: Swagger Hub Registry
  x-api-slug: swagger-hub-registry
  description: The place for teams to collaborate and coordinate the entire workflow
    of an APIs lifecycle. SwaggerHub&rsquo;s built-in editors let you rapidly create
    the Swagger definition that everything else is based on, in an intuitive interface
    that lets you write, visualize and validate all at the same time.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/SwaggerHub_Logo_Horizontal_Color.png
  humanURL: http://swaggerhub.com
  baseURL: https://api.swaggerhub.com//
  tags: Plugins
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/plugins/master/_listings/swaggerhub/openapi.md
x-common:
- type: x-github
  url: https://github.com/swagger-hub
- type: x-twitter
  url: https://twitter.com/swaggerhub
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