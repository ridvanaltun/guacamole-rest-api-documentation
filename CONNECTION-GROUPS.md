# Connection Groups

Manage connection groups.

# Table of Contents

- [Connection Groups](#connection-groups)
- [Table of Contents](#table-of-contents)
  - [List Connection Groups](#list-connection-groups)
    - [GET /api/session/data/{{data_source}}/connectionGroups](#get-apisessiondatadatasourceconnectiongroups)
      - [Headers](#headers)
      - [Path Parameters](#path-parameters)
      - [Query Parameters](#query-parameters)
      - [Request Body](#request-body)
    - [Response](#response)
      - [Status Code](#status-code)
      - [Response Body](#response-body)
  - [List Connections and Connection Groups](#list-connections-and-connection-groups)
    - [GET /api/session/data/{{data_source}}/connectionGroups/ROOT/tree](#get-apisessiondatadatasourceconnectiongroupsroottree)
      - [Headers](#headers-1)
      - [Path Parameters](#path-parameters-1)
      - [Query Parameters](#query-parameters-1)
      - [Request Body](#request-body-1)
    - [Response](#response-1)
      - [Status Code](#status-code-1)
      - [Response Body](#response-body-1)
  - [Details of Connection Group](#details-of-connection-group)
    - [GET /api/session/data/{{data_source}}/connectionGroups/{{connection_group}}](#get-apisessiondatadatasourceconnectiongroupsconnectiongroup)
      - [Headers](#headers-2)
      - [Path Parameters](#path-parameters-2)
      - [Query Parameters](#query-parameters-2)
      - [Request Body](#request-body-2)
    - [Response](#response-2)
      - [Status Code](#status-code-2)
      - [Response Body](#response-body-2)
  - [Details of Connection Group Tree](#details-of-connection-group-tree)
    - [GET /api/session/data/{{data_source}}/connectionGroups/{{connection_group}}/tree](#get-apisessiondatadatasourceconnectiongroupsconnectiongrouptree)
      - [Headers](#headers-3)
      - [Path Parameters](#path-parameters-3)
      - [Query Parameters](#query-parameters-3)
      - [Request Body](#request-body-3)
    - [Response](#response-3)
      - [Status Code](#status-code-3)
      - [Response Body](#response-body-3)
  - [Update Connection Group](#update-connection-group)
    - [PUT /api/session/data/{{data_source}}/connectionGroups/{{connection_group}}](#put-apisessiondatadatasourceconnectiongroupsconnectiongroup)
      - [Headers](#headers-4)
      - [Path Parameters](#path-parameters-4)
      - [Query Parameters](#query-parameters-4)
      - [Request Body](#request-body-4)
    - [Response](#response-4)
      - [Status Code](#status-code-4)
      - [Response Body](#response-body-4)
  - [Create Connection Group](#create-connection-group)
    - [POST /api/session/data/{{data_source}}/connectionGroups](#post-apisessiondatadatasourceconnectiongroups)
      - [Headers](#headers-5)
      - [Path Parameters](#path-parameters-5)
      - [Query Parameters](#query-parameters-5)
      - [Request Body](#request-body-5)
    - [Response](#response-5)
      - [Status Code](#status-code-5)
      - [Response Body](#response-body-5)
  - [Delete Connection Group](#delete-connection-group)
    - [DELETE /api/session/data/{{data_source}}/connectionGroups/{{connection_group}}](#delete-apisessiondatadatasourceconnectiongroupsconnectiongroup)
      - [Headers](#headers-6)
      - [Path Parameters](#path-parameters-6)
      - [Query Parameters](#query-parameters-6)
      - [Request Body](#request-body-6)
    - [Response](#response-6)
      - [Status Code](#status-code-6)
      - [Response Body](#response-body-6)

## List Connection Groups

List connection groups.

### GET /api/session/data/{{data_source}}/connectionGroups

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

## List Connections and Connection Groups

List connection groups with connections.

### GET /api/session/data/{{data_source}}/connectionGroups/ROOT/tree

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

## Details of Connection Group

Details of connection group.

### GET /api/session/data/{{data_source}}/connectionGroups/{{connection_group}}

#### Headers

None.

#### Path Parameters

- data_source (string, required) - Data source
- connection_group (integer, required) - Connection group identifier

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

## Details of Connection Group Tree

Details of connection group tree.

### GET /api/session/data/{{data_source}}/connectionGroups/{{connection_group}}/tree

#### Headers

None.

#### Path Parameters

- data_source (string, required) - Data source
- connection_group (integer, required) - Connection group identifier

#### Query Parameters

- token (string, required) - Auth Token
- permission (string, optional) - Permission

#### Request Body

None.

### Response

#### Status Code

- 200 - OK

#### Response Body

**@TODO**

---

## Update Connection Group

Updates connection group.

### PUT /api/session/data/{{data_source}}/connectionGroups/{{connection_group}}

#### Headers

- Content-Type (string, required) - application/json

#### Path Parameters

- data_source (string, required) - Data source
- connection_group (integer, required) - Connection group identifier

#### Query Parameters

- token (string, required) - Auth Token

#### Request Body

**@TODO**

```json
{
  "name": "test",
  "identifier": "1",
  "parentIdentifier": "ROOT",
  "type": "ORGANIZATIONAL",
  "activeConnections": 0,
  "attributes": {
    "max-connections": "",
    "max-connections-per-user": "",
    "enable-session-affinity": ""
  }
}
```

### Response

#### Status Code

- 204 - No Content

#### Response Body

This request does not return a response body.

---

## Create Connection Group

Creates connection group.

### POST /api/session/data/{{data_source}}/connectionGroups

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
  "parentIdentifier": "1",
  "name": "name",
  "type": "ORGANIZATIONAL",
  "attributes": {
    "max-connections": "",
    "max-connections-per-user": "",
    "enable-session-affinity": ""
  }
}
```

### Response

#### Status Code

- 200 - OK

#### Response Body

**@TODO**

---

## Delete Connection Group

Delete connection group.

### DELETE /api/session/data/{{data_source}}/connectionGroups/{{connection_group}}

#### Headers

None.

#### Path Parameters

- data_source (string, required) - Data source
- connection_group (string, required) - Connection groups identifier

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

[Back to Top](#connection-groups)
