<!-- omit in toc -->
# Guacamole Web REST API

Guacamole REST API gives you access and manage Guacamole Web Application.

[![Run in Postman](https://run.pstmn.io/button.svg)](https://god.gw.postman.com/run-collection/8259062-57a268f6-bee4-4cc8-9469-d2214982549f?action=collection%2Ffork&collection-url=entityId%3D8259062-57a268f6-bee4-4cc8-9469-d2214982549f%26entityType%3Dcollection%26workspaceId%3D3ea615b0-b0b9-4991-8aa0-5c1a6b603e99)

<!-- omit in toc -->
## Table of Contents

- [Overview](#overview)
- [Authentication](#authentication)
- [Common Responses](#common-responses)
- [Common Http Request Headers](#common-http-request-headers)
- [Api Ref](#api-ref)

# Overview

This documentation is **unofficial** and based on **Guacamole version 1.1.0**.

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

# Api Ref

- [Authentication](https://github.com/ridvanaltun/guacamole-rest-api-documentation/blob/master/docs/AUTHENTICATION.md)
- [Users](https://github.com/ridvanaltun/guacamole-rest-api-documentation/blob/master/docs/USERS.md)
- [User Groups](https://github.com/ridvanaltun/guacamole-rest-api-documentation/blob/master/docs/USER-GROUPS.md)
- [Connections](https://github.com/ridvanaltun/guacamole-rest-api-documentation/blob/master/docs/CONNECTIONS.md)
- [Connection Groups](https://github.com/ridvanaltun/guacamole-rest-api-documentation/blob/master/docs/CONNECTION-GROUPS.md)
- [Sharing Profiles](https://github.com/ridvanaltun/guacamole-rest-api-documentation/blob/master/docs/SHARING-PROFILES.md)
- [Permissions](https://github.com/ridvanaltun/guacamole-rest-api-documentation/blob/master/docs/PERMISSIONS.md)
- [History](https://github.com/ridvanaltun/guacamole-rest-api-documentation/blob/master/docs/HISTORY.md)
- [Schemas](https://github.com/ridvanaltun/guacamole-rest-api-documentation/blob/master/docs/SCHEMAS.md)
- [Tunnels](https://github.com/ridvanaltun/guacamole-rest-api-documentation/blob/master/docs/TUNNELS.md)
- [Patches](https://github.com/ridvanaltun/guacamole-rest-api-documentation/blob/master/docs/PATCHES.md)
- [Languages](https://github.com/ridvanaltun/guacamole-rest-api-documentation/blob/master/docs/LANGUAGES.md)
