---
name: New Relic
x-slug: new-relic
description: New Relic???s digital intelligence platform lets developers, ops, and
  tech teams measure and monitor the performance of their applications and infrastructure.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
x-kinRank: "8"
x-alexaRank: "10322"
tags: Plugins
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/plugins/master/_listings/new-relic/apis.md
specificationVersion: "0.14"
apis:
- name: New Relic - Add Alerts Plugins Conditions Policies Policy  . Format
  x-api-slug: alerts-plugins-conditionspoliciespolicy-id-format-post
  description: |-
    This API endpoint allows you to create Plugins conditions for your alert policies.

    Note: Admin User???s API Key is required.

    See our documentation for a discussion on creating conditions for plugins.

    All fields are required except for ???runbook_url???, ???enabled??? (defaults to false).

    name: A title for your condition.

    enabled: The status of your condition (optional).

    entities: An array of instance IDs associated with your condition.

    metric_description: A title for the metric to display in notifications.

    metric: The metric to evaluate on.

    value_function: min, max, average, sample_size, total, percent

    runbook_url: Runbook URL to display in notifications (optional).

    terms[duration] (in minutes): 5, 10, 15, 30, 60, 120.

    terms[operator]: above, below, equal.

    terms[priority]: critical, warning.

    terms[threshold]: Must be 0 or greater.

    terms[time_function]: all, any.

    plugin[id]: The ID of the plugin.

    plugin[guid]: The GUID of the plugin.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2/
  tags: Monitoring, Performance, Stack Network, Technology, SaaS, API Service Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/plugins/master/_listings/new-relic/alerts-plugins-conditionspoliciespolicy-id-format-post-openapi.md
- name: New Relic - Put Alerts Plugins Conditions  . Format
  x-api-slug: alerts-plugins-conditionsid-format-put
  description: |-
    This API endpoint allows you to update Plugins conditions for your alert policies.

    Note: Admin User???s API Key is required.

    See Alerts Plugins Conditions &gt; Create for an explanation of the field values ued in this command or the online document on
    updating conditions for plugins.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2/
  tags: Monitoring, Performance, Stack Network, Technology, SaaS, API Service Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/plugins/master/_listings/new-relic/alerts-plugins-conditionsid-format-put-openapi.md
- name: New Relic - Delete Alerts Plugins Conditions Condition  . Format
  x-api-slug: alerts-plugins-conditionscondition-id-format-delete
  description: |-
    This API endpoint allows you to delete Plugins conditions associated with your alert policy.

    Note: Admin User???s API Key is required.

    See our documentation for a discussion on deleting Plugins conditions.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2/
  tags: Monitoring, Performance, Stack Network, Technology, SaaS, API Service Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/plugins/master/_listings/new-relic/alerts-plugins-conditionscondition-id-format-delete-openapi.md
- name: New Relic - Get Alerts Plugins Conditions. Format
  x-api-slug: alerts-plugins-conditions-format-get
  description: "This API endpoint allows you to list the Plugins conditions for your
    alert policy.\n\nSee our documentation for a discussion on \noutput pagination."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2/
  tags: Monitoring, Performance, Stack Network, Technology, SaaS, API Service Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/plugins/master/_listings/new-relic/alerts-plugins-conditions-format-get-openapi.md
- name: New Relic - Get Plugins  . Format
  x-api-slug: pluginsid-format-get
  description: This API endpoint returns a single plugin, identified by its ID.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2/
  tags: Monitoring, Performance, Stack Network, Technology, SaaS, API Service Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/plugins/master/_listings/new-relic/pluginsid-format-get-openapi.md
- name: New Relic - Get Plugins. Format
  x-api-slug: plugins-format-get
  description: "This API endpoint returns a list of the Plugins associated with your
    New Relic account.\n\nPlugins can be filtered by their guid or the list of plugin
    IDs.\n\nSee our documentation for a discussion on \noutput pagination."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2/
  tags: Monitoring, Performance, Stack Network, Technology, SaaS, API Service Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/plugins/master/_listings/new-relic/plugins-format-get-openapi.md
- name: New Relic - Get Alerts Entity Conditions Entity  . Format
  x-api-slug: alerts-entity-conditionsentity-id-format-get
  description: |-
    This API endpoint allows you to list the Alerts conditions an entity is part of.

    Entity type options (Synthetics is not yet supported):

    BrowserApplication

    Application

    MobileApplication

    Server

    KeyTransaction

    Plugin
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2/
  tags: Monitoring, Performance, Stack Network, Technology, SaaS, API Service Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/plugins/master/_listings/new-relic/alerts-entity-conditionsentity-id-format-get-openapi.md
- name: New Relic - Put Alerts Entity Conditions Entity  . Format
  x-api-slug: alerts-entity-conditionsentity-id-format-put
  description: "This API endpoint allows you to add an entity to a specified Alerts
    condition.\n\nNote: Admin User???s API Key is required.\n \n  Entity type options
    (Synthetics is not yet supported):\n\nBrowserApplication\n\nApplication\n\nMobileApplication\n\nServer\n\nKeyTransaction\n\nPlugin"
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2/
  tags: Monitoring, Performance, Stack Network, Technology, SaaS, API Service Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/plugins/master/_listings/new-relic/alerts-entity-conditionsentity-id-format-put-openapi.md
- name: New Relic - Delete Alerts Entity Conditions Entity  . Format
  x-api-slug: alerts-entity-conditionsentity-id-format-delete
  description: |-
    This API endpoint allows you to disassociate an entity with a specified Alerts condition.

    Note: Admin User???s API Key is required.

    Entity type options (Synthetics is not yet supported):

    BrowserApplication

    Application

    MobileApplication

    Server

    KeyTransaction

    Plugin
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2/
  tags: Monitoring, Performance, Stack Network, Technology, SaaS, API Service Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/plugins/master/_listings/new-relic/alerts-entity-conditionsentity-id-format-delete-openapi.md
- name: New Relic - Get Alerts Events. Format
  x-api-slug: alerts-events-format-get
  description: "This API endpoint allows you to list the alert events for your account.\n\nAlerts
    events can be filter by product, target type, group ID, instance ID, and event
    type.\n\nThe options for products are: APM, BROWSER, MOBILE, SERVERS, PLUGINS,
    SYNTHETICS, and ALERTS.\n\nThe options for entity type are: Application, Server,
    KeyTransaction, Plugin, MobileApplication, BrowserApplication, and Monitor.\n\nThe
    options for event type are: NOTIFICATION, DEPLOYMENT, VIOLATION_OPEN, VIOLATION_CLOSE,
    VIOLATION, and INSTRUMENTATION.\n\nThe group ID option is normally the same as
    the entity ID (e.g. an Application group ID and entity ID will be the same), however
    PLUGINS have a group ID representing the PLUGIN itself, and entity IDs for all
    instances of that PLUGIN type.\n\nSee our documentation for a discussion on \noutput
    pagination."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2/
  tags: Monitoring, Performance, Stack Network, Technology, SaaS, API Service Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/plugins/master/_listings/new-relic/alerts-events-format-get-openapi.md
- name: New Relic - Get Alerts Plugins Conditions. Format
  x-api-slug: alerts-plugins-conditions-format-get
  description: "This API endpoint allows you to list the Plugins conditions for your
    alert policy.\n\nSee our documentation for a discussion on \noutput pagination."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2/
  tags: Monitoring, Performance, Stack Network, Technology, SaaS, API Service Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/plugins/master/_listings/new-relic/alerts-plugins-conditions-format-get-openapi.md
- name: New Relic - Add Alerts Plugins Conditions Policies Policy  . Format
  x-api-slug: alerts-plugins-conditionspoliciespolicy-id-format-post
  description: |-
    This API endpoint allows you to create Plugins conditions for your alert policies.

    Note: Admin User???s API Key is required.

    See our documentation for a discussion on creating conditions for plugins.

    All fields are required except for ???runbook_url???, ???enabled??? (defaults to false).

    name: A title for your condition.

    enabled: The status of your condition (optional).

    entities: An array of instance IDs associated with your condition.

    metric_description: A title for the metric to display in notifications.

    metric: The metric to evaluate on.

    value_function: min, max, average, sample_size, total, percent

    runbook_url: Runbook URL to display in notifications (optional).

    terms[duration] (in minutes): 5, 10, 15, 30, 60, 120.

    terms[operator]: above, below, equal.

    terms[priority]: critical, warning.

    terms[threshold]: Must be 0 or greater.

    terms[time_function]: all, any.

    plugin[id]: The ID of the plugin.

    plugin[guid]: The GUID of the plugin.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2/
  tags: Monitoring, Performance, Stack Network, Technology, SaaS, API Service Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/plugins/master/_listings/new-relic/alerts-plugins-conditionspoliciespolicy-id-format-post-openapi.md
- name: New Relic - Delete Alerts Plugins Conditions Condition  . Format
  x-api-slug: alerts-plugins-conditionscondition-id-format-delete
  description: |-
    This API endpoint allows you to delete Plugins conditions associated with your alert policy.

    Note: Admin User???s API Key is required.

    See our documentation for a discussion on deleting Plugins conditions.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2/
  tags: Monitoring, Performance, Stack Network, Technology, SaaS, API Service Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/plugins/master/_listings/new-relic/alerts-plugins-conditionscondition-id-format-delete-openapi.md
- name: New Relic - Put Alerts Plugins Conditions  . Format
  x-api-slug: alerts-plugins-conditionsid-format-put
  description: |-
    This API endpoint allows you to update Plugins conditions for your alert policies.

    Note: Admin User???s API Key is required.

    See Alerts Plugins Conditions &gt; Create for an explanation of the field values ued in this command or the online document on
    updating conditions for plugins.
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2/
  tags: Monitoring, Performance, Stack Network, Technology, SaaS, API Service Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/plugins/master/_listings/new-relic/alerts-plugins-conditionsid-format-put-openapi.md
- name: New Relic - Get Plugins. Format
  x-api-slug: plugins-format-get
  description: "This API endpoint returns a list of the Plugins associated with your
    New Relic account.\n\nPlugins can be filtered by their guid or the list of plugin
    IDs.\n\nSee our documentation for a discussion on \noutput pagination."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2/
  tags: Monitoring, Performance, Stack Network, Technology, SaaS, API Service Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/plugins/master/_listings/new-relic/plugins-format-get-openapi.md
- name: New Relic - Get Plugins. Format
  x-api-slug: plugins-format-get
  description: "This API endpoint returns a list of the Plugins associated with your
    New Relic account.\n\nPlugins can be filtered by their guid or the list of plugin
    IDs.\n\nSee our documentation for a discussion on \noutput pagination."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/22963-new-relic.jpg
  humanURL: https://newrelic.com/
  baseURL: https:///v2/
  tags: Monitoring, Performance, Stack Network, Technology, SaaS, API Service Provider,
    Profiles, Relative Data, Service API
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/plugins/master/_listings/new-relic/plugins-format-get-openapi.md
x-common:
- type: x-api-gallery
  url: http://netlicensing.api.gallery.streamdata.io
- type: x-api-stack
  url: http://new.relic.stack.network
- type: x-blog
  url: https://blog.newrelic.com/
- type: x-blog-rss
  url: https://blog.newrelic.com/feed/
- type: x-crunchbase
  url: https://crunchbase.com/organization/new-relic
- type: x-developer
  url: https://rpm.newrelic.com/api/explore/
- type: x-email
  url: billing@newrelic.com
- type: x-email
  url: resume@newrelic.com
- type: x-email
  url: PR@newrelic.com
- type: x-email
  url: copyright@newrelic.com
- type: x-email
  url: dataprivacy@newrelic.com
- type: x-email
  url: PersonalDataRequest@newrelic.com
- type: x-email
  url: support@newrelic.com
- type: x-email
  url: compliance@newrelic.com
- type: x-github
  url: https://github.com/newrelic
- type: x-twitter
  url: https://twitter.com/NewRelic
- type: x-website
  url: https://newrelic.com/
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---