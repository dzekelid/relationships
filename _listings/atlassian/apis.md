---
name: Atlassian
x-slug: atlassian
description: Millions of users globally rely on Atlassian products every day for improving
  software development, project management, collaboration, and code quality.
image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
x-kinRank: "8"
x-alexaRank: "1656"
tags: Relationships
created: "2018-08-28"
modified: "2018-08-28"
url: https://raw.githubusercontent.com/streamdata-gallery-topics/relationships/master/_listings/atlassian/apis.md
specificationVersion: "0.14"
apis:
- name: The Confluence Cloud REST API - Find relationship from source to target
  x-api-slug: relationrelationnamefromsourcetypesourcekeytotargettypetargetkey-get
  description: "Find whether a particular type of relationship exists from a source
    \nentity to a target entity. Note, relationships are one way.\n\nFor example,
    you can use this method to find whether the current user has \nselected a particular
    page as a favorite (i.e. 'save for later'):\n`GET https://your-domain.atlassian.net/wiki/rest/api/relation/favourite/from/user/current/to/content/123`\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
    required**: \nPermission to view both the target entity and source entity."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/relationships/master/_listings/atlassian/relationrelationnamefromsourcetypesourcekeytotargettypetargetkey-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/relationships/master/_listings/atlassian/relationrelationnamefromsourcetypesourcekeytotargettypetargetkey-get-openapi.md
- name: The Confluence Cloud REST API - Create relationship
  x-api-slug: relationrelationnamefromsourcetypesourcekeytotargettypetargetkey-put
  description: "Creates a relationship between two entities (user, space, content).
    The \n'favourite' relationship is supported by default, but you can use this method
    \nto create any type of relationship between two entities.\n\nFor example, the
    following method creates a 'sibling' relationship between \ntwo pieces of content:\n`GET
    https://your-domain.atlassian.net/wiki/rest/api/relation/sibling/from/content/123/to/content/456`\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
    required**: \nPermission to access the Confluence site ('Can use' global permission)."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/relationships/master/_listings/atlassian/relationrelationnamefromsourcetypesourcekeytotargettypetargetkey-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/relationships/master/_listings/atlassian/relationrelationnamefromsourcetypesourcekeytotargettypetargetkey-put-openapi.md
- name: The Confluence Cloud REST API - Find relationship from source to target
  x-api-slug: relationrelationnamefromsourcetypesourcekeytotargettypetargetkey-get
  description: "Find whether a particular type of relationship exists from a source
    \nentity to a target entity. Note, relationships are one way.\n\nFor example,
    you can use this method to find whether the current user has \nselected a particular
    page as a favorite (i.e. 'save for later'):\n`GET https://your-domain.atlassian.net/wiki/rest/api/relation/favourite/from/user/current/to/content/123`\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
    required**: \nPermission to view both the target entity and source entity."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/relationships/master/_listings/atlassian/relationrelationnamefromsourcetypesourcekeytotargettypetargetkey-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/relationships/master/_listings/atlassian/relationrelationnamefromsourcetypesourcekeytotargettypetargetkey-get-openapi.md
- name: The Confluence Cloud REST API - Create relationship
  x-api-slug: relationrelationnamefromsourcetypesourcekeytotargettypetargetkey-put
  description: "Creates a relationship between two entities (user, space, content).
    The \n'favourite' relationship is supported by default, but you can use this method
    \nto create any type of relationship between two entities.\n\nFor example, the
    following method creates a 'sibling' relationship between \ntwo pieces of content:\n`GET
    https://your-domain.atlassian.net/wiki/rest/api/relation/sibling/from/content/123/to/content/456`\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
    required**: \nPermission to access the Confluence site ('Can use' global permission)."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/relationships/master/_listings/atlassian/relationrelationnamefromsourcetypesourcekeytotargettypetargetkey-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/relationships/master/_listings/atlassian/relationrelationnamefromsourcetypesourcekeytotargettypetargetkey-put-openapi.md
- name: The Confluence Cloud REST API - Create relationship
  x-api-slug: relationrelationnamefromsourcetypesourcekeytotargettypetargetkey-put
  description: "Creates a relationship between two entities (user, space, content).
    The \n'favourite' relationship is supported by default, but you can use this method
    \nto create any type of relationship between two entities.\n\nFor example, the
    following method creates a 'sibling' relationship between \ntwo pieces of content:\n`GET
    https://your-domain.atlassian.net/wiki/rest/api/relation/sibling/from/content/123/to/content/456`\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
    required**: \nPermission to access the Confluence site ('Can use' global permission)."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/relationships/master/_listings/atlassian/relationrelationnamefromsourcetypesourcekeytotargettypetargetkey-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/relationships/master/_listings/atlassian/relationrelationnamefromsourcetypesourcekeytotargettypetargetkey-put-openapi.md
- name: The Confluence Cloud REST API - Create relationship
  x-api-slug: relationrelationnamefromsourcetypesourcekeytotargettypetargetkey-put
  description: "Creates a relationship between two entities (user, space, content).
    The \n'favourite' relationship is supported by default, but you can use this method
    \nto create any type of relationship between two entities.\n\nFor example, the
    following method creates a 'sibling' relationship between \ntwo pieces of content:\n`GET
    https://your-domain.atlassian.net/wiki/rest/api/relation/sibling/from/content/123/to/content/456`\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
    required**: \nPermission to access the Confluence site ('Can use' global permission)."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/relationships/master/_listings/atlassian/relationrelationnamefromsourcetypesourcekeytotargettypetargetkey-put-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/relationships/master/_listings/atlassian/relationrelationnamefromsourcetypesourcekeytotargettypetargetkey-put-openapi.md
- name: The Confluence Cloud REST API - Find relationship from source to target
  x-api-slug: relationrelationnamefromsourcetypesourcekeytotargettypetargetkey-get
  description: "Find whether a particular type of relationship exists from a source
    \nentity to a target entity. Note, relationships are one way.\n\nFor example,
    you can use this method to find whether the current user has \nselected a particular
    page as a favorite (i.e. 'save for later'):\n`GET https://your-domain.atlassian.net/wiki/rest/api/relation/favourite/from/user/current/to/content/123`\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
    required**: \nPermission to view both the target entity and source entity."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/relationships/master/_listings/atlassian/relationrelationnamefromsourcetypesourcekeytotargettypetargetkey-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/relationships/master/_listings/atlassian/relationrelationnamefromsourcetypesourcekeytotargettypetargetkey-get-openapi.md
- name: The Confluence Cloud REST API - Find relationship from source to target
  x-api-slug: relationrelationnamefromsourcetypesourcekeytotargettypetargetkey-get
  description: "Find whether a particular type of relationship exists from a source
    \nentity to a target entity. Note, relationships are one way.\n\nFor example,
    you can use this method to find whether the current user has \nselected a particular
    page as a favorite (i.e. 'save for later'):\n`GET https://your-domain.atlassian.net/wiki/rest/api/relation/favourite/from/user/current/to/content/123`\n\n**[Permissions](https://confluence.atlassian.com/x/_AozKw)
    required**: \nPermission to view both the target entity and source entity."
  image: http://kinlane-productions.s3.amazonaws.com/screen-capture-api/691-atlassian.jpg
  humanURL: http://atlassian.com/
  baseURL: https:////
  tags: Coding, Programming, Wiki, Issues, Code Issues, Stack Network, SaaS, Technology,
    Enterprise, API Provider, API Service Provider, Profiles, Relative Data, Service
    API
  properties:
  - type: x-postman-collection
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/relationships/master/_listings/atlassian/relationrelationnamefromsourcetypesourcekeytotargettypetargetkey-get-postman.md
  - type: x-openapi-spec
    url: https://raw.githubusercontent.com/streamdata-gallery-topics/relationships/master/_listings/atlassian/relationrelationnamefromsourcetypesourcekeytotargettypetargetkey-get-openapi.md
x-common:
- type: x-openapi
  url: https://developer.atlassian.com/cloud/jira/platform/swagger.v3.json
- type: x-openapi
  url: https://developer.atlassian.com/cloud/confluence/swagger.v3.json
- type: x-openapi
  url: https://developer.atlassian.com/cloud/jira/software/swagger.v3.json
- type: x-openapi
  url: https://developer.atlassian.com/cloud/jira/service-desk/swagger.v3.json
- type: x-website
  url: http://atlassian.com/
- type: x-website
  url: http://www.atlassian.com
- type: x-api-gallery
  url: http://att.dev.program.api.gallery.streamdata.io
- type: x-api-stack
  url: http://atlassian.stack.network
- type: x-blog
  url: http://blogs.atlassian.com/
- type: x-crunchbase
  url: https://crunchbase.com/organization/atlassian
- type: x-crunchbase
  url: http://www.crunchbase.com/company/atlassian
- type: x-email
  url: copyright@atlassian.com
- type: x-email
  url: trademarks@atlassian.com
- type: x-email
  url: sales@atlassian.com
- type: x-email
  url: ar_enterprise@atlassian.com
- type: x-email
  url: privacy@atlassian.com
- type: x-email
  url: eudatarep@atlassian.com
- type: x-email
  url: experts@atlassian.com
- type: x-email
  url: remittance@atlassian.com
- type: x-email
  url: ap@atlassian.com
- type: x-email
  url: procurement@atlassian.com
- type: x-github
  url: https://github.com/atlassian
- type: x-privacy-policy
  url: https://www.atlassian.com/legal/privacy-policy?_ga=2.188884514.868776184.1519225620-845241124.1519225620
- type: x-twitter
  url: https://twitter.com/atlassian
include: []
maintainers:
- FN: Kin Lane
  x-twitter: apievangelist
  email: info@apievangelist.com
---