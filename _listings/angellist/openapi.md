swagger: "2.0"
x-collection-name: AngelList
x-complete: 1
info:
  title: AngelList
  description: the-angellist-api-provides-developers-with-a-restful-interface-to-the-angellist-data-set--for-more-information-read-the-oauth-faq-
  termsOfService: https://angel.co/terms
  contact:
    name: AngelList
    url: https://angel.co/api
    email: api@angel.co
  version: v1
host: api.angel.co
basePath: /1/
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /follows/relationship:
    get:
      summary: Get Follows Relationship
      description: Gets the relationships for followers
      operationId: followsRelationship
      x-api-path-slug: followsrelationship-get
      parameters:
      - in: query
        name: source_id
      - in: query
        name: target_id
      - in: query
        name: target_type
      responses:
        200:
          description: OK
      tags:
      - Startups
      - Businesses
      - Relationships