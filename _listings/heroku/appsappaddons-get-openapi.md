---
swagger: "2.0"
x-collection-name: Heroku
x-complete: 0
info:
  title: Heroku Get Application Addons
  description: List addons installed on an app.
  version: "1"
host: api.heroku.com
basePath: /
schemes:
- http
produces:
- application/json
consumes:
- application/json
paths:
  /addons:
    parameters:
      summary: Parameters Addons
      description: Parameters addons.
      operationId: parametersAddons
      x-api-path-slug: addons-parameters
      responses:
        200:
          description: OK
      tags:
      - Parameters
      - ons
    get:
      summary: Get Addons
      description: List all available addons.
      operationId: getAddons
      x-api-path-slug: addons-get
      parameters:
      - in: header
        name: Accept
        description: Content type
      responses:
        200:
          description: OK
      tags:
      - ons
  /apps/{app}/addons:
    parameters:
      summary: Parameter Application Addons
      description: Parameter application addons.
      operationId: parametersAppsAppAddons
      x-api-path-slug: appsappaddons-parameters
      responses:
        200:
          description: OK
      tags:
      - Parameter
      - Application
      - ons
    get:
      summary: Get Application Addons
      description: List addons installed on an app.
      operationId: getAppsAppAddons
      x-api-path-slug: appsappaddons-get
      parameters:
      - in: header
        name: Accept
        description: Content type
      responses:
        200:
          description: OK
      tags:
      - Application
      - ons
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