# Languages

Manage languages.

# Table of Contents

- [Languages](#languages)
- [Table of Contents](#table-of-contents)
  - [List Languages](#list-languages)
    - [GET /api/languages](#get-apilanguages)
      - [Headers](#headers)
      - [Path Parameters](#path-parameters)
      - [Query Parameters](#query-parameters)
      - [Request Body](#request-body)
    - [Response](#response)
      - [Status Code](#status-code)
      - [Response Body](#response-body)

## List Languages

List languages.

### GET /api/languages

#### Headers

None.

#### Path Parameters

None.

#### Query Parameters

None.

#### Request Body

None.

### Response

#### Status Code

- 200 - OK

#### Response Body

List of languages.

```json
{
  "de": "Deutsch",
  "no": "Norsk Bokmål",
  "ru": "Русский",
  "cz": "Čeština",
  "ja": "日本語",
  "en": "English",
  "it": "Italiano",
  "fr": "Français",
  "nl": "Nederlands",
  "zh": "简体中文",
  "es": "Spanish"
}
```

---

[Back to Top](#languages)
