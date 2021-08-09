<!-- omit in toc -->
# User Groups

Manage user groups.

<!-- omit in toc -->
# Table of Contents

- [List User Groups](#list-user-groups)
    - [Headers](#headers)
    - [Path Parameters](#path-parameters)
    - [Query Parameters](#query-parameters)
    - [Request Body](#request-body)
  - [Response](#response)
    - [Status Code](#status-code)
    - [Response Body](#response-body)
- [Details of User Group](#details-of-user-group)
    - [Headers](#headers-1)
    - [Path Parameters](#path-parameters-1)
    - [Query Parameters](#query-parameters-1)
    - [Request Body](#request-body-1)
  - [Response](#response-1)
    - [Status Code](#status-code-1)
    - [Response Body](#response-body-1)
- [Add Members to User Group](#add-members-to-user-group)
    - [Headers](#headers-2)
    - [Path Parameters](#path-parameters-2)
    - [Query Parameters](#query-parameters-2)
    - [Request Body](#request-body-2)
  - [Response](#response-2)
    - [Status Code](#status-code-2)
    - [Response Body](#response-body-2)
- [Add Member Groups to User Group](#add-member-groups-to-user-group)
    - [Headers](#headers-3)
    - [Path Parameters](#path-parameters-3)
    - [Query Parameters](#query-parameters-3)
    - [Request Body](#request-body-3)
  - [Response](#response-3)
    - [Status Code](#status-code-3)
    - [Response Body](#response-body-3)
- [Add Parent Groups to User Group](#add-parent-groups-to-user-group)
    - [Headers](#headers-4)
    - [Path Parameters](#path-parameters-4)
    - [Query Parameters](#query-parameters-4)
    - [Request Body](#request-body-4)
  - [Response](#response-4)
    - [Status Code](#status-code-4)
    - [Response Body](#response-body-4)
- [Assign Permissions to User Group](#assign-permissions-to-user-group)
    - [Headers](#headers-5)
    - [Path Parameters](#path-parameters-5)
    - [Query Parameters](#query-parameters-5)
    - [Request Body](#request-body-5)
  - [Response](#response-5)
    - [Status Code](#status-code-5)
    - [Response Body](#response-body-5)
- [Revoke Permissions from User Group](#revoke-permissions-from-user-group)
    - [Headers](#headers-6)
    - [Path Parameters](#path-parameters-6)
    - [Query Parameters](#query-parameters-6)
    - [Request Body](#request-body-6)
  - [Response](#response-6)
    - [Status Code](#status-code-6)
    - [Response Body](#response-body-6)
- [Assign Connections to User Group](#assign-connections-to-user-group)
    - [Headers](#headers-7)
    - [Path Parameters](#path-parameters-7)
    - [Query Parameters](#query-parameters-7)
    - [Request Body](#request-body-7)
  - [Response](#response-7)
    - [Status Code](#status-code-7)
    - [Response Body](#response-body-7)
- [Revoke Connections from User Group](#revoke-connections-from-user-group)
    - [Headers](#headers-8)
    - [Path Parameters](#path-parameters-8)
    - [Query Parameters](#query-parameters-8)
    - [Request Body](#request-body-8)
  - [Response](#response-8)
    - [Status Code](#status-code-8)
    - [Response Body](#response-body-8)
- [Update User Group](#update-user-group)
    - [Headers](#headers-9)
    - [Path Parameters](#path-parameters-9)
    - [Query Parameters](#query-parameters-9)
    - [Request Body](#request-body-9)
  - [Response](#response-9)
    - [Status Code](#status-code-9)
    - [Response Body](#response-body-9)
- [Create User Group](#create-user-group)
    - [Headers](#headers-10)
    - [Path Parameters](#path-parameters-10)
    - [Query Parameters](#query-parameters-10)
    - [Request Body](#request-body-10)
  - [Response](#response-10)
    - [Status Code](#status-code-10)
    - [Response Body](#response-body-10)
- [Delete User Group](#delete-user-group)
    - [Headers](#headers-11)
    - [Path Parameters](#path-parameters-11)
    - [Query Parameters](#query-parameters-11)
    - [Request Body](#request-body-11)
  - [Response](#response-11)
    - [Status Code](#status-code-11)
    - [Response Body](#response-body-11)

## List User Groups

<!-- omit in toc -->
### GET /api/session/data/{{data_source}}/userGroups

#### Headers

None.

#### Path Parameters

- data_source (string, required) - Data source

#### Query Parameters

- token (string, required) - Auth Token

#### Request Body

None.

### Response

#### Status Code

- 200 - OK

#### Response Body

**@TODO**

---

## Details of User Group

<!-- omit in toc -->
### GET /api/session/data/{{data_source}}/userGroups/{{user_group}}

#### Headers

None.

#### Path Parameters

- data_source (string, required) - Data source
- user_group (string, required) - User group identifier

#### Query Parameters

- token (string, required) - Auth Token

#### Request Body

None.

### Response

#### Status Code

- 200 - OK

#### Response Body

**@TODO**

---

## Add Members to User Group

Add members to an user group.

<!-- omit in toc -->
### PATCH /api/session/data/{{data_source}}/userGroups/{{user_group}}/memberUsers

#### Headers

- Content-Type (string, required) - application/json

#### Path Parameters

- data_source (string, required) - Data source
- user_group (string, required) - User group identifier

#### Query Parameters

- token (string, required) - Auth Token

#### Request Body

Body must be [json-patch](http://jsonpatch.com/) format.

```json
[
  {
    "op": "add",
    "path": "/",
    "value": "{{username}}"
  }
]
```

### Response

#### Status Code

- 204 - No Content

#### Response Body

This request does not return a response body.

---

## Add Member Groups to User Group

Add member groups to an user group.

<!-- omit in toc -->
### PATCH /api/session/data/{{data_source}}/userGroups/{{user_group}}/memberUserGroups

#### Headers

- Content-Type (string, required) - application/json

#### Path Parameters

- data_source (string, required) - Data source
- user_group (string, required) - User group identifier

#### Query Parameters

- token (string, required) - Auth Token

#### Request Body

Body must be [json-patch](http://jsonpatch.com/) format.

```json
[
  {
    "op": "add",
    "path": "/",
    "value": "{{userGroupIdentifier}}"
  }
]
```

### Response

#### Status Code

- 204 - No Content

#### Response Body

This request does not return a response body.

---

## Add Parent Groups to User Group

Add parent groups to an user group.

<!-- omit in toc -->
### PATCH /api/session/data/{{data_source}}/userGroups/{{user_group}}/userGroups

#### Headers

- Content-Type (string, required) - application/json

#### Path Parameters

- data_source (string, required) - Data source
- user_group (string, required) - User group identifier

#### Query Parameters

- token (string, required) - Auth Token

#### Request Body

Body must be [json-patch](http://jsonpatch.com/) format.

```json
[
  {
    "op": "add",
    "path": "/",
    "value": "{{userGroupIdentifier}}"
  }
]
```

### Response

#### Status Code

- 204 - No Content

#### Response Body

This request does not return a response body.

---

## Assign Permissions to User Group

Assign permissions to an user group.

<!-- omit in toc -->
### PATCH /api/session/data/{{data_source}}/userGroups/{{user_group}}/permissions

#### Headers

- Content-Type (string, required) - application/json

#### Path Parameters

- data_source (string, required) - Data source
- user_group (string, required) - User group identifier

#### Query Parameters

- token (string, required) - Auth Token

#### Request Body

Body must be [json-patch](http://jsonpatch.com/) format.

```json
[
  {
    "op": "add",
    "path": "/connectionPermissions/{{user_group}}",
    "value": "READ"
  },
  {
    "op": "add",
    "path": "/systemPermissions",
    "value": "CREATE_USER"
  },
  {
    "op": "add",
    "path": "/systemPermissions",
    "value": "ADMINISTER"
  },
  {
    "op": "add",
    "path": "/systemPermissions",
    "value": "CREATE_USER_GROUP"
  },
  {
    "op": "add",
    "path": "/systemPermissions",
    "value": "CREATE_CONNECTION"
  },
  {
    "op": "add",
    "path": "/systemPermissions",
    "value": "CREATE_SHARING_PROFILE"
  },
  {
    "op": "add",
    "path": "/systemPermissions",
    "value": "CREATE_CONNECTION_GROUP"
  }
]
```

### Response

#### Status Code

- 204 - No Content

#### Response Body

This request does not return a response body.

---

## Revoke Permissions from User Group

Revoke permissions from an user group.

<!-- omit in toc -->
### PATCH /api/session/data/{{data_source}}/userGroups/{{user_group}}/permissions

#### Headers

- Content-Type (string, required) - application/json

#### Path Parameters

- data_source (string, required) - Data source
- user_group (string, required) - User group identifier

#### Query Parameters

- token (string, required) - Auth Token

#### Request Body

Body must be [json-patch](http://jsonpatch.com/) format.

```json
[
  {
    "op": "remove",
    "path": "/connectionPermissions/{{user_group}}",
    "value": "READ"
  },
  {
    "op": "remove",
    "path": "/systemPermissions",
    "value": "CREATE_USER"
  },
  {
    "op": "remove",
    "path": "/systemPermissions",
    "value": "ADMINISTER"
  },
  {
    "op": "remove",
    "path": "/systemPermissions",
    "value": "CREATE_USER_GROUP"
  },
  {
    "op": "remove",
    "path": "/systemPermissions",
    "value": "CREATE_CONNECTION"
  },
  {
    "op": "remove",
    "path": "/systemPermissions",
    "value": "CREATE_SHARING_PROFILE"
  },
  {
    "op": "remove",
    "path": "/systemPermissions",
    "value": "CREATE_CONNECTION_GROUP"
  }
]
```

### Response

#### Status Code

- 204 - No Content

#### Response Body

This request does not return a response body.

---

## Assign Connections to User Group

Assign connections to an user group

<!-- omit in toc -->
### PATCH /api/session/data/{{data_source}}/userGroups/{{user_group}}/permissions

#### Headers

- Content-Type (string, required) - application/json

#### Path Parameters

- data_source (string, required) - Data source
- user_group (string, required) - User group identifier

#### Query Parameters

- token (string, required) - Auth Token

#### Request Body

Body must be [json-patch](http://jsonpatch.com/) format.

```json
[
  {
    "op": "add",
    "path": "/connectionPermissions/{{connection}}",
    "value": "READ"
  }
]
```

### Response

#### Status Code

- 204 - No Content

#### Response Body

This request does not return a response body.

---

## Revoke Connections from User Group

Revoke connections from an user group.

<!-- omit in toc -->
### PATCH /api/session/data/{{data_source}}/userGroups/{{user_group}}/permissions

#### Headers

- Content-Type (string, required) - application/json

#### Path Parameters

- data_source (string, required) - Data source
- user_group (string, required) - User group identifier

#### Query Parameters

- token (string, required) - Auth Token

#### Request Body

Body must be [json-patch](http://jsonpatch.com/) format.

```json
[
  {
    "op": "remove",
    "path": "/connectionPermissions/{{connection}}",
    "value": "READ"
  }
]
```

### Response

#### Status Code

- 204 - No Content

#### Response Body

This request does not return a response body.

---

## Update User Group

Updates user group.

<!-- omit in toc -->
### PUT /api/session/data/{{data_source}}/userGroups/{{user_group}}

#### Headers

- Content-Type (string, required) - application/json

#### Path Parameters

- data_source (string, required) - Data source
- user_group (string, required) - User group identifier

#### Query Parameters

- token (string, required) - Auth Token

#### Request Body

**@TODO**

```json
{
  "identifier": "test",
  "attributes": {
    "disabled": ""
  }
}
```

### Response

#### Status Code

- 204 - No Content

#### Response Body

This request does not return a response body.

---

## Create User Group

Create a user group.

<!-- omit in toc -->
### POST /api/session/data/{{data_source}}/userGroups

#### Headers

- Content-Type (string, required) - application/json

#### Path Parameters

- data_source (string, required) - Data source

#### Query Parameters

- token (string, required) - Auth Token

#### Request Body

**@TODO**

```json
{
  "identifier": "test",
  "attributes": {
    "disabled": ""
  }
}
```

### Response

#### Status Code

- 204 - No Content

#### Response Body

This request does not return a response body.

---

## Delete User Group

Delete user group.

<!-- omit in toc -->
### DELETE /api/session/data/{{data_source}}/userGroups/{{user_group}}

#### Headers

None.

#### Path Parameters

- data_source (string, required) - Data source
- user_group (string, required) - User group identifier

#### Query Parameters

- token (string, required) - Auth token

#### Request Body

None.

### Response

#### Status Code

- 204 - No Content

#### Response Body

This request does not return a response body.

---

[Back to Top](#user-groups)
