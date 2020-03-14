# Authentication

Authentication allows you create and delete tokens.

# Table of Contents

- [Authentication](#authentication)
- [Table of Contents](#table-of-contents)
  - [Generate Token](#generate-token)
    - [POST /api/tokens](#post-apitokens)
      - [Headers](#headers)
      - [Path Parameters](#path-parameters)
      - [Query Parameters](#query-parameters)
      - [Request Body](#request-body)
    - [Response](#response)
      - [Status Code](#status-code)
      - [Response Body](#response-body)
      - [Response Examples](#response-examples)
  - [Delete Token](#delete-token)
    - [DELETE /api/tokens/{{token}}](#delete-apitokenstoken)
      - [Headers](#headers-1)
      - [Path Parameters](#path-parameters-1)
      - [Query Parameters](#query-parameters-1)
      - [Request Body](#request-body-1)
    - [Response](#response-1)
      - [Status Code](#status-code-1)
      - [Response Body](#response-body-1)

## Generate Token

Generates token.

### POST /api/tokens

#### Headers

None.

#### Path Parameters

None.

#### Query Parameters

None.

#### Request Body

Body must be `x-www-form-urlencoded`.

- username (string, required) - Name of the user.
- password (string, required) - Password of the user.

```
username: guacadmin
password: guacadmin
```

### Response

#### Status Code

- 200 - OK

#### Response Body

Returns a JSON object.

- authToken (string) - Auth token.
- username (string) - Username.
- dataSource (string) - Datasource.
- availableDatasources (array) - List of available data sources.

#### Response Examples

```json
{
  "authToken": "0BDA2CED0580DEB052C34B596AB401993BFD66551FADEF06FC7144F1D6318EE8",
  "username": "guacadmin",
  "dataSource": "postgresql",
  "availableDataSources": ["postgresql", "postgresql-shared"]
}
```

---

## Delete Token

Deletes token.

### DELETE /api/tokens/{{token}}

#### Headers

None.

#### Path Parameters

- token (string, required) - Auth Token

#### Query Parameters

None.

#### Request Body

None.

### Response

#### Status Code

- 204 - No Content

#### Response Body

This request does not return a response body.

---

[Back to Top](#authentication)
