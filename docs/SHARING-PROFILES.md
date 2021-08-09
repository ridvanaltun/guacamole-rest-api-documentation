<!-- omit in toc -->
# Sharing Profiles

Manage sharing profiles.

<!-- omit in toc -->
# Table of Contents

- [List Sharing Profiles](#list-sharing-profiles)
    - [Headers](#headers)
    - [Path Parameters](#path-parameters)
    - [Query Parameters](#query-parameters)
    - [Request Body](#request-body)
  - [Response](#response)
    - [Status Code](#status-code)
    - [Response Body](#response-body)
- [Details of Sharing Profile](#details-of-sharing-profile)
    - [Headers](#headers-1)
    - [Path Parameters](#path-parameters-1)
    - [Query Parameters](#query-parameters-1)
    - [Request Body](#request-body-1)
  - [Response](#response-1)
    - [Status Code](#status-code-1)
    - [Response Body](#response-body-1)
- [Create Sharing Profile](#create-sharing-profile)
    - [Headers](#headers-2)
    - [Path Parameters](#path-parameters-2)
    - [Query Parameters](#query-parameters-2)
    - [Request Body](#request-body-2)
  - [Response](#response-2)
    - [Status Code](#status-code-2)
    - [Response Body](#response-body-2)
- [Delete Sharing Profile](#delete-sharing-profile)
    - [Headers](#headers-3)
    - [Path Parameters](#path-parameters-3)
    - [Query Parameters](#query-parameters-3)
    - [Request Body](#request-body-3)
  - [Response](#response-3)
    - [Status Code](#status-code-3)
    - [Response Body](#response-body-3)

## List Sharing Profiles

<!-- omit in toc -->
### GET /api/session/data/{{data_source}}/sharingProfiles

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

## Details of Sharing Profile

Details of sharing profile.

<!-- omit in toc -->
### GET /api/session/data/{{data_source}}/sharingProfiles/{{sharing_profile}}

#### Headers

None.

#### Path Parameters

- data_source (string, required) - Data source
- sharing_profile (string, required) - Sharing profile identifier

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

## Create Sharing Profile

Create a sharing profile.

<!-- omit in toc -->
### POST /api/session/data/{{data_source}}/sharingProfiles

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
  "primaryConnectionIdentifier": "8",
  "name": "test",
  "parameters": {
    "read-only": ""
  },
  "attributes": {}
}
```

### Response

#### Status Code

- 200 - OK

#### Response Body

**@TODO**

---

## Delete Sharing Profile

Delete sharing profile.

<!-- omit in toc -->
### DELETE /api/session/data/{{data_source}}/sharingProfiles/{{sharing_profile}}

#### Headers

None.

#### Path Parameters

- data_source (string, required) - Data source
- sharing_profile (string, required) - Sharing profile identifier

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

[Back to Top](#sharing-profiles)
