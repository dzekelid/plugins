---
name: New Relic
x-slug: new-relic
description: New Relic offers SaaS Software Analytics Platform that offers Application
  Performance Management and Real User Monitoring for Cloud and Data Center deployed
  web applications implemented in Ruby, Java, .NET, Python, PHP, Node.js. New Relic
  also offers mobile monitoring solutions for iOS and Android applications.
image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/newrelic-logo-square.png
x-kinRank: "8"
x-alexaRank: ""
tags: Plugins
created: "2018-05-20"
modified: "2018-05-20"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/plugins/master/_listings/new-relic/apis.md
specificationVersion: "0.14"
apis:
- name: New Relic Add Alerts Plugins Conditions Policies Policy  . Format
  x-api-slug: new-relic
  description: "This API endpoint allows you to create Plugins conditions for your
    alert policies.\n\nNote: Admin User\u2019s API Key is required.\n\nSee our documentation
    for a discussion on creating conditions for plugins.\n\nAll fields are required
    except for \u201Crunbook_url\u201D, \u201Cenabled\u201D (defaults to false).\n\nname:
    A title for your condition.\n\nenabled: The status of your condition (optional).\n\nentities:
    An array of instance IDs associated with your condition.\n\nmetric_description:
    A title for the metric to display in notifications.\n\nmetric: The metric to evaluate
    on.\n\nvalue_function: min, max, average, sample_size, total, percent\n\nrunbook_url:
    Runbook URL to display in notifications (optional).\n\nterms[duration] (in minutes):
    5, 10, 15, 30, 60, 120.\n\nterms[operator]: above, below, equal.\n\nterms[priority]:
    critical, warning.\n\nterms[threshold]: Must be 0 or greater.\n\nterms[time_function]:
    all, any.\n\nplugin[id]: The ID of the plugin.\n\nplugin[guid]: The GUID of the
    plugin."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/newrelic-logo-square.png
  humanURL: https://newrelic.com/
  baseURL: https:///v2///alerts_plugins_conditions/policies/{policy_id}.{format}
  tags: Alerts, Plugins, Conditions, Policies, Policy, , ., Format
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/plugins/master/_listings/new-relic/alerts-plugins-conditionspoliciespolicy-idformat-post-openapi.md
- name: New Relic Put Alerts Plugins Conditions  . Format
  x-api-slug: new-relic
  description: "This API endpoint allows you to update Plugins conditions for your
    alert policies.\n\nNote: Admin User\u2019s API Key is required.\n\nSee Alerts
    Plugins Conditions &gt; Create for an explanation of the field values ued in this
    command or the online document on\nupdating conditions for plugins."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/newrelic-logo-square.png
  humanURL: https://newrelic.com/
  baseURL: https:///v2///alerts_plugins_conditions/{id}.{format}
  tags: Alerts, Plugins, Conditions, , ., Format
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/plugins/master/_listings/new-relic/alerts-plugins-conditionsidformat-put-openapi.md
- name: New Relic Delete Alerts Plugins Conditions Condition  . Format
  x-api-slug: new-relic
  description: "This API endpoint allows you to delete Plugins conditions associated
    with your alert policy.\n\nNote: Admin User\u2019s API Key is required.\n\nSee
    our documentation for a discussion on deleting Plugins conditions."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/newrelic-logo-square.png
  humanURL: https://newrelic.com/
  baseURL: https:///v2///alerts_plugins_conditions/{condition_id}.{format}
  tags: Alerts, Plugins, Conditions, Condition, , ., Format
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/plugins/master/_listings/new-relic/alerts-plugins-conditionscondition-idformat-delete-openapi.md
- name: New Relic Get Alerts Plugins Conditions. Format
  x-api-slug: new-relic
  description: "This API endpoint allows you to list the Plugins conditions for your
    alert policy.\n\nSee our documentation for a discussion on \noutput pagination."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/newrelic-logo-square.png
  humanURL: https://newrelic.com/
  baseURL: https:///v2///alerts_plugins_conditions.{format}
  tags: Alerts, Plugins, Conditions., Format
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/plugins/master/_listings/new-relic/alerts-plugins-conditionsformat-get-openapi.md
- name: New Relic Get Plugins. Format
  x-api-slug: new-relic
  description: "This API endpoint returns a list of the Plugins associated with your
    New Relic account.\n\nPlugins can be filtered by their guid or the list of plugin
    IDs.\n\nSee our documentation for a discussion on \noutput pagination."
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/newrelic-logo-square.png
  humanURL: https://newrelic.com/
  baseURL: https:///v2///plugins.{format}
  tags: Plugins., Format
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/plugins/master/_listings/new-relic/pluginsformat-get-openapi.md
- name: New Relic Get Plugins  . Format
  x-api-slug: new-relic
  description: This API endpoint returns a single plugin, identified by its ID.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/newrelic-logo-square.png
  humanURL: https://newrelic.com/
  baseURL: https:///v2///plugins/{id}.{format}
  tags: Plugins, , ., Format
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/plugins/master/_listings/new-relic/pluginsidformat-get-openapi.md
- name: New Relic
  x-api-slug: new-relic
  description: New Relic offers SaaS Software Analytics Platform that offers Application
    Performance Management and Real User Monitoring for Cloud and Data Center deployed
    web applications implemented in Ruby, Java, .NET, Python, PHP, Node.js. New Relic
    also offers mobile monitoring solutions for iOS and Android applications.
  image: http://kinlane-productions.s3.amazonaws.com/api-evangelist-site/company/logos/newrelic-logo-square.png
  humanURL: https://newrelic.com/
  baseURL: https:///v2/
  tags: Plugins
  properties:
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/plugins/master/_listings/new-relic/openapi.md
x-common:
- type: x-blog
  url: https://blog.newrelic.com/
- type: x-blog-rss
  url: https://blog.newrelic.com/feed/
- type: x-developer
  url: https://rpm.newrelic.com/api/explore/
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