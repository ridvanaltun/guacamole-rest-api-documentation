# Guacamole Web REST API

Guacamole REST API gives you access and manage Guacamole Web Application.

## Table of Contents

- [Guacamole Web REST API](#guacamole-web-rest-api)
  - [Table of Contents](#table-of-contents)
- [Overview](#overview)
- [Authentication](#authentication)
- [Common Responses](#common-responses)
- [Common Http Request Headers](#common-http-request-headers)

# Overview

This documentation is unofficial and based on Guacamole version 1.1.0.

Keep in mind, it's not fully tested.

# Authentication

Authentication is required for all requests except the following:

- Authentication
- Languages
- Patches

Token must be named as 'token' and must be placed in request query.

**Example:** `https://localhost/api/session/data/postgresql/connections?token=123456789`

# Common Responses

This section discusses various API responses.

- 200 - A request succeeded.
- 204 - No content
- 400 - Bad request
- 401 - Unauthorized
- 404 - Not found

# Common Http Request Headers

The standard Http request headers that are used in requests.

- Content-Type - The Internet media type of the request body. Used with POST, PUT and PATCH requests. Must be `application/json`.
