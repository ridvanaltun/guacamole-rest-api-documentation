# Permissions

Manage permissions.

# Table of Contents

- [Permissions](#permissions)
- [Table of Contents](#table-of-contents)
  - [Assign System Permissions to User](#assign-system-permissions-to-user)
    - [PATCH /api/session/data/{{data_source}}/users/{{username}}/permissions](#patch-apisessiondatadatasourceusersusernamepermissions)
      - [Headers](#headers)
      - [Path Parameters](#path-parameters)
      - [Query Parameters](#query-parameters)
      - [Request Body](#request-body)
    - [Response](#response)
      - [Status Code](#status-code)
      - [Response Body](#response-body)
  - [Revoke System Permissions from User](#revoke-system-permissions-from-user)
    - [PATCH /api/session/data/{{data_source}}/users/{{username}}/permissions](#patch-apisessiondatadatasourceusersusernamepermissions-1)
      - [Headers](#headers-1)
      - [Path Parameters](#path-parameters-1)
      - [Query Parameters](#query-parameters-1)
      - [Request Body](#request-body-1)
    - [Response](#response-1)
      - [Status Code](#status-code-1)
      - [Response Body](#response-body-1)
  - [Assign Connection Groups to User](#assign-connection-groups-to-user)
    - [PATCH /api/session/data/{{data_source}}/users/{{username}}/permissions](#patch-apisessiondatadatasourceusersusernamepermissions-2)
      - [Headers](#headers-2)
      - [Path Parameters](#path-parameters-2)
      - [Query Parameters](#query-parameters-2)
      - [Request Body](#request-body-2)
    - [Response](#response-2)
      - [Status Code](#status-code-2)
      - [Response Body](#response-body-2)
  - [Revoke Connection Group from User](#revoke-connection-group-from-user)
    - [PATCH /api/session/data/{{data_source}}/users/{{username}}/permissions](#patch-apisessiondatadatasourceusersusernamepermissions-3)
      - [Headers](#headers-3)
      - [Path Parameters](#path-parameters-3)
      - [Query Parameters](#query-parameters-3)
      - [Request Body](#request-body-3)
    - [Response](#response-3)
      - [Status Code](#status-code-3)
      - [Response Body](#response-body-3)

## Assign System Permissions to User

Assign system permissions to an user.

### PATCH /api/session/data/{{data_source}}/users/{{username}}/permissions

#### Headers

- Content-Type (string, required) - application/json

#### Path Parameters

- data_source (string, required) - Data source
- username (string, required) - Username

#### Query Parameters

- token (string, required) - Auth token

#### Request Body

Body must be [json-patch](http://jsonpatch.com/) format.

```json
[
  {
    "op": "add",
    "path": "/userPermissions/test1",
    "value": "UPDATE"
  },
  {
    "op": "add",
    "path": "/systemPermissions",
    "value": "CREATE_USER"
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
    "value": "CREATE_CONNECTION_GROUP"
  },
  {
    "op": "add",
    "path": "/systemPermissions",
    "value": "CREATE_SHARING_PROFILE"
  },
  {
    "op": "add",
    "path": "/systemPermissions",
    "value": "ADMINISTER"
  }
]
```

### Response

#### Status Code

- 204 - No Content

#### Response Body

This request does not return a response body.

---

## Revoke System Permissions from User

Revoke system permissions from an user.

### PATCH /api/session/data/{{data_source}}/users/{{username}}/permissions

#### Headers

- Content-Type (string, required) - application/json

#### Path Parameters

- data_source (string, required) - Data source
- username (string, required) - Username

#### Query Parameters

- token (string, required) - Auth Token

#### Request Body

Body must be [json-patch](http://jsonpatch.com/) format.

```json
[
  {
    "op": "remove",
    "path": "/userPermissions/test1",
    "value": "UPDATE"
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
  },
  {
    "op": "remove",
    "path": "/systemPermissions",
    "value": "CREATE_CONNECTION"
  },
  {
    "op": "remove",
    "path": "/systemPermissions",
    "value": "CREATE_USER_GROUP"
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
  }
]
```

### Response

#### Status Code

- 204 - No Content

#### Response Body

This request does not return a response body.

---

## Assign Connection Groups to User

Assign connection groups to an user.

### PATCH /api/session/data/{{data_source}}/users/{{username}}/permissions

#### Headers

- Content-Type (string, required) - application/json

#### Path Parameters

- data_source (string, required) - Data source
- username (string, required) - Username

#### Query Parameters

- token (string, required) - Auth Token

#### Request Body

Body must be [json-patch](http://jsonpatch.com/) format.

```json
[
  {
    "op": "add",
    "path": "/connectionGroupPermissions/{{connection_group}}",
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

## Revoke Connection Group from User

Revoke connection groups from an user.

### PATCH /api/session/data/{{data_source}}/users/{{username}}/permissions

#### Headers

- Content-Type (string, required) - application/json

#### Path Parameters

- data_source (string, required) - Data source
- username (string, required) - Username

#### Query Parameters

- token (string, required) - Auth Token

#### Request Body

Body must be [json-patch](http://jsonpatch.com/) format.

```json
[
  {
    "op": "remove",
    "path": "/connectionGroupPermissions/{{connection_group}}",
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

[Back to Top](#permissions)
