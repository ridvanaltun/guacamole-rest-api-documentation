<!-- omit in toc -->
# Connections

Manage connections.

<!-- omit in toc -->
# Table of Contents

- [List Connections](#list-connections)
    - [Headers](#headers)
    - [Path Parameters](#path-parameters)
- [Details of Connection](#details-of-connection)
    - [Headers](#headers-1)
    - [Path Parameters](#path-parameters-1)
    - [Query Parameters](#query-parameters)
    - [Request Body](#request-body)
  - [Response](#response)
    - [Status Code](#status-code)
    - [Response Body](#response-body)
- [Details of Connection Parameters](#details-of-connection-parameters)
    - [Headers](#headers-2)
    - [Path Parameters](#path-parameters-2)
    - [Query Parameters](#query-parameters-1)
    - [Request Body](#request-body-1)
  - [Response](#response-1)
    - [Status Code](#status-code-1)
    - [Response Body](#response-body-1)
- [Details of Connection History](#details-of-connection-history)
    - [Headers](#headers-3)
    - [Path Parameters](#path-parameters-3)
    - [Query Parameters](#query-parameters-2)
    - [Request Body](#request-body-2)
  - [Response](#response-2)
    - [Status Code](#status-code-2)
    - [Response Body](#response-body-2)
- [Details of Connection Sharing Profiles](#details-of-connection-sharing-profiles)
    - [Headers](#headers-4)
    - [Path Parameters](#path-parameters-4)
    - [Query Parameters](#query-parameters-3)
- [List Sharing Profiles](#list-sharing-profiles)
    - [Headers](#headers-5)
    - [Path Parameters](#path-parameters-5)
    - [Query Parameters](#query-parameters-4)
    - [Request Body](#request-body-3)
  - [Response](#response-3)
    - [Status Code](#status-code-3)
    - [Response Body](#response-body-3)
- [List Active Connections](#list-active-connections)
    - [Headers](#headers-6)
    - [Path Parameters](#path-parameters-6)
    - [Query Parameters](#query-parameters-5)
    - [Request Body](#request-body-4)
  - [Response](#response-4)
    - [Status Code](#status-code-4)
    - [Response Body](#response-body-4)
- [Kill Connections](#kill-connections)
    - [Headers](#headers-7)
    - [Path Parameters](#path-parameters-7)
    - [Query Parameters](#query-parameters-6)
    - [Request Body](#request-body-5)
  - [Response](#response-5)
    - [Status Code](#status-code-5)
    - [Response Body](#response-body-5)
- [Create VNC Connection](#create-vnc-connection)
    - [Headers](#headers-8)
    - [Path Parameters](#path-parameters-8)
    - [Query Parameters](#query-parameters-7)
    - [Request Body](#request-body-6)
  - [Response](#response-6)
    - [Status Code](#status-code-6)
    - [Response Body](#response-body-6)
- [Create SSH Connection](#create-ssh-connection)
    - [Headers](#headers-9)
    - [Path Parameters](#path-parameters-9)
    - [Query Parameters](#query-parameters-8)
    - [Request Body](#request-body-7)
  - [Response](#response-7)
    - [Status Code](#status-code-7)
    - [Response Body](#response-body-7)
- [Create RDP Connection](#create-rdp-connection)
    - [Headers](#headers-10)
    - [Path Parameters](#path-parameters-10)
    - [Query Parameters](#query-parameters-9)
    - [Request Body](#request-body-8)
  - [Response](#response-8)
    - [Status Code](#status-code-8)
    - [Response Body](#response-body-8)
- [Create Telnet Connection](#create-telnet-connection)
    - [Headers](#headers-11)
    - [Path Parameters](#path-parameters-11)
    - [Query Parameters](#query-parameters-10)
    - [Request Body](#request-body-9)
  - [Response](#response-9)
    - [Status Code](#status-code-9)
    - [Response Body](#response-body-9)
- [Create Kubernetes Connection](#create-kubernetes-connection)
    - [Headers](#headers-12)
    - [Path Parameters](#path-parameters-12)
    - [Query Parameters](#query-parameters-11)
    - [Request Body](#request-body-10)
  - [Response](#response-10)
    - [Status Code](#status-code-10)
    - [Response Body](#response-body-10)
- [Update VNC Connection](#update-vnc-connection)
    - [Headers](#headers-13)
    - [Path Parameters](#path-parameters-13)
    - [Query Parameters](#query-parameters-12)
    - [Request Body](#request-body-11)
  - [Response](#response-11)
    - [Status Code](#status-code-11)
    - [Response Body](#response-body-11)
- [Update SSH Connection](#update-ssh-connection)
    - [Headers](#headers-14)
    - [Path Parameters](#path-parameters-14)
    - [Query Parameters](#query-parameters-13)
    - [Request Body](#request-body-12)
  - [Response](#response-12)
    - [Status Code](#status-code-12)
    - [Response Body](#response-body-12)
- [Update RDP Connection](#update-rdp-connection)
    - [Headers](#headers-15)
    - [Path Parameters](#path-parameters-15)
    - [Query Parameters](#query-parameters-14)
    - [Request Body](#request-body-13)
  - [Response](#response-13)
    - [Status Code](#status-code-13)
    - [Response Body](#response-body-13)
- [Update Telnet Connection](#update-telnet-connection)
    - [Headers](#headers-16)
    - [Path Parameters](#path-parameters-16)
    - [Query Parameters](#query-parameters-15)
    - [Request Body](#request-body-14)
  - [Response](#response-14)
    - [Status Code](#status-code-14)
    - [Response Body](#response-body-14)
- [Update Kubernetes Connection](#update-kubernetes-connection)
    - [Headers](#headers-17)
    - [Path Parameters](#path-parameters-17)
    - [Query Parameters](#query-parameters-16)
    - [Request Body](#request-body-15)
  - [Response](#response-15)
    - [Status Code](#status-code-15)
    - [Response Body](#response-body-15)
- [Delete Connection](#delete-connection)
    - [Headers](#headers-18)
    - [Path Parameters](#path-parameters-18)
    - [Query Parameters](#query-parameters-17)
    - [Request Body](#request-body-16)
  - [Response](#response-16)
    - [Status Code](#status-code-16)
    - [Response Body](#response-body-16)

## List Connections

List connections.

<!-- omit in toc -->
### GET /api/session/data/{{data_source}}/connections

#### Headers

None.

#### Path Parameters

- data_source (string, required) - Data source

---

## Details of Connection

Details of connection.

<!-- omit in toc -->
### GET /api/session/data/{{data_source}}/connections/{{connection}}

#### Headers

None.

#### Path Parameters

- data_source (string, required) - Data source
- connection (integer, required) - Connection identifier

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

## Details of Connection Parameters

Details of connection parameters.

<!-- omit in toc -->
### GET /api/session/data/{{data_source}}/connections/{{connection}}/parameters

#### Headers

None.

#### Path Parameters

- data_source (string, required) - Data source
- connection (integer, required) - Connection identifier

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

## Details of Connection History

Details of connection history.

<!-- omit in toc -->
### GET /api/session/data/{{data_source}}/connections/{{connection}}/history

#### Headers

None.

#### Path Parameters

- data_source (string, required) - Data source
- connection (integer, required) - Connection identifier

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

## Details of Connection Sharing Profiles

Details of connection sharing profiles.

<!-- omit in toc -->
### GET /api/session/data/{{data_source}}/connections/{{connection}}/sharingProfiles

#### Headers

None.

#### Path Parameters

- data_source (string, required) - Data source
- connection (integer, required) - Connection identifier

#### Query Parameters

- token (string, required) - Auth Token

---

## List Sharing Profiles

List sharing profiles.

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

## List Active Connections

List active connections.

<!-- omit in toc -->
### GET /api/session/data/{{data_source}}/activeConnections

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

## Kill Connections

Kill connections.

<!-- omit in toc -->
### PATCH /api/session/data/{{data_source}}/activeConnections

#### Headers

- Content-Type (string, required) - application/json

#### Path Parameters

- data_source (string, required) - Data source

#### Query Parameters

- token (string, required) - Auth Token

#### Request Body

Body must be [json-patch](http://jsonpatch.com/) format.

```json
[
  {
    "op": "remove",
    "path": "/{{activeConnectionIdentifier}}"
  }
]
```

### Response

#### Status Code

- 200 - OK

#### Response Body

**@TODO**

---

## Create VNC Connection

Creates a VNC connection.

<!-- omit in toc -->
### POST /api/session/data/{{data_source}}/connections

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
  "parentIdentifier": "ROOT",
  "name": "test",
  "protocol": "vnc",
  "parameters": {
    "port": "",
    "read-only": "",
    "swap-red-blue": "",
    "cursor": "",
    "color-depth": "",
    "clipboard-encoding": "",
    "disable-copy": "",
    "disable-paste": "",
    "dest-port": "",
    "recording-exclude-output": "",
    "recording-exclude-mouse": "",
    "recording-include-keys": "",
    "create-recording-path": "",
    "enable-sftp": "true",
    "sftp-port": "",
    "sftp-server-alive-interval": "",
    "enable-audio": "",
    "audio-servername": "",
    "sftp-directory": "",
    "sftp-root-directory": "",
    "sftp-passphrase": "",
    "sftp-private-key": "",
    "sftp-username": "",
    "sftp-password": "",
    "sftp-host-key": "",
    "sftp-hostname": "",
    "recording-name": "",
    "recording-path": "",
    "dest-host": "",
    "password": "",
    "username": "",
    "hostname": ""
  },
  "attributes": {
    "max-connections": "",
    "max-connections-per-user": "",
    "weight": "",
    "failover-only": "",
    "guacd-port": "",
    "guacd-encryption": "",
    "guacd-hostname": ""
  }
}
```

### Response

#### Status Code

- 200 - OK

#### Response Body

**@TODO**

---

## Create SSH Connection

Creates a SSH connection.

<!-- omit in toc -->
### POST /api/session/data/{{data_source}}/connections

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
  "parentIdentifier": "ROOT",
  "name": "test",
  "protocol": "ssh",
  "parameters": {
    "port": "",
    "read-only": "",
    "swap-red-blue": "",
    "cursor": "",
    "color-depth": "",
    "clipboard-encoding": "",
    "disable-copy": "",
    "disable-paste": "",
    "dest-port": "",
    "recording-exclude-output": "",
    "recording-exclude-mouse": "",
    "recording-include-keys": "",
    "create-recording-path": "",
    "enable-sftp": "",
    "sftp-port": "",
    "sftp-server-alive-interval": "",
    "enable-audio": "",
    "color-scheme": "",
    "font-size": "",
    "scrollback": "",
    "timezone": null,
    "server-alive-interval": "",
    "backspace": "",
    "terminal-type": "",
    "create-typescript-path": "",
    "hostname": "",
    "host-key": "",
    "private-key": "",
    "username": "",
    "password": "",
    "passphrase": "",
    "font-name": "",
    "command": "",
    "locale": "",
    "typescript-path": "",
    "typescript-name": "",
    "recording-path": "",
    "recording-name": "",
    "sftp-root-directory": ""
  },
  "attributes": {
    "max-connections": "",
    "max-connections-per-user": "",
    "weight": "",
    "failover-only": "",
    "guacd-port": "",
    "guacd-encryption": "",
    "guacd-hostname": ""
  }
}
```

### Response

#### Status Code

- 200 - OK

#### Response Body

**@TODO**

---

## Create RDP Connection

Creates a RDP connection.

<!-- omit in toc -->
### POST /api/session/data/{{data_source}}/connections

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
  "parentIdentifier": "ROOT",
  "name": "test",
  "protocol": "rdp",
  "parameters": {
    "port": "",
    "read-only": "",
    "swap-red-blue": "",
    "cursor": "",
    "color-depth": "",
    "clipboard-encoding": "",
    "disable-copy": "",
    "disable-paste": "",
    "dest-port": "",
    "recording-exclude-output": "",
    "recording-exclude-mouse": "",
    "recording-include-keys": "",
    "create-recording-path": "",
    "enable-sftp": "",
    "sftp-port": "",
    "sftp-server-alive-interval": "",
    "enable-audio": "",
    "security": "",
    "disable-auth": "",
    "ignore-cert": "",
    "gateway-port": "",
    "server-layout": "",
    "timezone": "",
    "console": "",
    "width": "",
    "height": "",
    "dpi": "",
    "resize-method": "",
    "console-audio": "",
    "disable-audio": "",
    "enable-audio-input": "",
    "enable-printing": "",
    "enable-drive": "",
    "create-drive-path": "",
    "enable-wallpaper": "",
    "enable-theming": "",
    "enable-font-smoothing": "",
    "enable-full-window-drag": "",
    "enable-desktop-composition": "",
    "enable-menu-animations": "",
    "disable-bitmap-caching": "",
    "disable-offscreen-caching": "",
    "disable-glyph-caching": "",
    "preconnection-id": "",
    "hostname": "",
    "username": "",
    "password": "",
    "domain": "",
    "gateway-hostname": "",
    "gateway-username": "",
    "gateway-password": "",
    "gateway-domain": "",
    "initial-program": "",
    "client-name": "",
    "printer-name": "",
    "drive-name": "",
    "drive-path": "",
    "static-channels": "",
    "remote-app": "",
    "remote-app-dir": "",
    "remote-app-args": "",
    "preconnection-blob": "",
    "load-balance-info": "",
    "recording-path": "",
    "recording-name": "",
    "sftp-hostname": "",
    "sftp-host-key": "",
    "sftp-username": "",
    "sftp-password": "",
    "sftp-private-key": "",
    "sftp-passphrase": "",
    "sftp-root-directory": "",
    "sftp-directory": ""
  },
  "attributes": {
    "max-connections": "",
    "max-connections-per-user": "",
    "weight": "",
    "failover-only": "",
    "guacd-port": "",
    "guacd-encryption": "",
    "guacd-hostname": ""
  }
}
```

### Response

#### Status Code

- 200 - OK

#### Response Body

**@TODO**

---

## Create Telnet Connection

Creates a Telnet connection.

<!-- omit in toc -->
### POST /api/session/data/{{data_source}}/connections

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
  "parentIdentifier": "ROOT",
  "name": "test",
  "protocol": "telnet",
  "parameters": {
    "port": "",
    "read-only": "",
    "swap-red-blue": "",
    "cursor": "",
    "color-depth": "",
    "clipboard-encoding": "",
    "disable-copy": "",
    "disable-paste": "",
    "dest-port": "",
    "recording-exclude-output": "",
    "recording-exclude-mouse": "",
    "recording-include-keys": "",
    "create-recording-path": "",
    "enable-sftp": "",
    "sftp-port": "",
    "sftp-server-alive-interval": "",
    "enable-audio": "",
    "color-scheme": "",
    "font-size": "",
    "scrollback": "",
    "backspace": "",
    "terminal-type": "",
    "create-typescript-path": "",
    "hostname": "",
    "username": "",
    "password": "",
    "username-regex": "",
    "password-regex": "",
    "login-success-regex": "",
    "login-failure-regex": "",
    "font-name": "",
    "typescript-path": "",
    "typescript-name": "",
    "recording-path": "",
    "recording-name": ""
  },
  "attributes": {
    "max-connections": "",
    "max-connections-per-user": "",
    "weight": "",
    "failover-only": "",
    "guacd-port": "",
    "guacd-encryption": "",
    "guacd-hostname": ""
  }
}
```

### Response

#### Status Code

- 200 - OK

#### Response Body

**@TODO**

---

## Create Kubernetes Connection

Creates a Kubernetes connection.

<!-- omit in toc -->
### POST /api/session/data/{{data_source}}/connections

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
  "parentIdentifier": "ROOT",
  "name": "test",
  "protocol": "kubernetes",
  "parameters": {
    "port": "",
    "read-only": "",
    "swap-red-blue": "",
    "cursor": "",
    "color-depth": "",
    "clipboard-encoding": "",
    "disable-copy": "",
    "disable-paste": "",
    "dest-port": "",
    "recording-exclude-output": "",
    "recording-exclude-mouse": "",
    "recording-include-keys": "",
    "create-recording-path": "",
    "enable-sftp": "",
    "sftp-port": "",
    "sftp-server-alive-interval": "",
    "enable-audio": "",
    "use-ssl": "",
    "ignore-cert": "",
    "color-scheme": "",
    "font-size": "",
    "scrollback": "",
    "backspace": "",
    "create-typescript-path": "",
    "hostname": "",
    "ca-cert": "",
    "namespace": "",
    "pod": "",
    "container": "",
    "client-cert": "",
    "client-key": "",
    "font-name": "",
    "typescript-path": "",
    "typescript-name": "",
    "recording-path": "",
    "recording-name": ""
  },
  "attributes": {
    "max-connections": "",
    "max-connections-per-user": "",
    "weight": "",
    "failover-only": "",
    "guacd-port": "",
    "guacd-encryption": "",
    "guacd-hostname": ""
  }
}
```

### Response

#### Status Code

- 200 - OK

#### Response Body

**@TODO**

---

## Update VNC Connection

Updates VNC connection.

<!-- omit in toc -->
### PUT /api/session/data/{{data_source}}/connections/{{connection}}

#### Headers

- Content-Type (string, required) - application/json

#### Path Parameters

- data_source (string, required) - Data source
- connection (integer, required) - Connection identifier

#### Query Parameters

- token (string, required) - Auth Token

#### Request Body

**@TODO**

```json
{
  "parentIdentifier": "ROOT",
  "name": "test",
  "identifier": "1",
  "activeConnections": 0,
  "protocol": "vnc",
  "parameters": {
    "port": "",
    "read-only": "",
    "swap-red-blue": "",
    "cursor": "",
    "color-depth": "",
    "clipboard-encoding": "",
    "disable-copy": "",
    "disable-paste": "",
    "dest-port": "",
    "recording-exclude-output": "",
    "recording-exclude-mouse": "",
    "recording-include-keys": "",
    "create-recording-path": "",
    "enable-sftp": "true",
    "sftp-port": "",
    "sftp-server-alive-interval": "",
    "enable-audio": "",
    "audio-servername": "",
    "sftp-directory": "",
    "sftp-root-directory": "",
    "sftp-passphrase": "",
    "sftp-private-key": "",
    "sftp-username": "",
    "sftp-password": "",
    "sftp-host-key": "",
    "sftp-hostname": "",
    "recording-name": "",
    "recording-path": "",
    "dest-host": "",
    "password": "",
    "username": "",
    "hostname": ""
  },
  "attributes": {
    "max-connections": "",
    "max-connections-per-user": "",
    "weight": "",
    "failover-only": "",
    "guacd-port": "",
    "guacd-encryption": "",
    "guacd-hostname": ""
  }
}
```

### Response

#### Status Code

- 204 - No Content

#### Response Body

This request does not return a response body.

---

## Update SSH Connection

Updates SSH connection.

<!-- omit in toc -->
### PUT /api/session/data/{{data_source}}/connections/{{connection}}

#### Headers

- Content-Type (string, required) - application/json

#### Path Parameters

- data_source (string, required) - Data source
- connection (integer, required) - Connection identifier

#### Query Parameters

- token (string, required) - Auth Token

#### Request Body

**@TODO**

```json
{
  "parentIdentifier": "ROOT",
  "name": "test",
  "identifier": "1",
  "activeConnections": 0,
  "protocol": "ssh",
  "parameters": {
    "port": "",
    "read-only": "",
    "swap-red-blue": "",
    "cursor": "",
    "color-depth": "",
    "clipboard-encoding": "",
    "disable-copy": "",
    "disable-paste": "",
    "dest-port": "",
    "recording-exclude-output": "",
    "recording-exclude-mouse": "",
    "recording-include-keys": "",
    "create-recording-path": "",
    "enable-sftp": "",
    "sftp-port": "",
    "sftp-server-alive-interval": "",
    "enable-audio": "",
    "color-scheme": "",
    "font-size": "",
    "scrollback": "",
    "timezone": null,
    "server-alive-interval": "",
    "backspace": "",
    "terminal-type": "",
    "create-typescript-path": "",
    "hostname": "",
    "host-key": "",
    "private-key": "",
    "username": "",
    "password": "",
    "passphrase": "",
    "font-name": "",
    "command": "",
    "locale": "",
    "typescript-path": "",
    "typescript-name": "",
    "recording-path": "",
    "recording-name": "",
    "sftp-root-directory": ""
  },
  "attributes": {
    "max-connections": "",
    "max-connections-per-user": "",
    "weight": "",
    "failover-only": "",
    "guacd-port": "",
    "guacd-encryption": "",
    "guacd-hostname": ""
  }
}
```

### Response

#### Status Code

- 204 - No Content

#### Response Body

This request does not return a response body.

---

## Update RDP Connection

Updates RDP connection.

<!-- omit in toc -->
### PUT /api/session/data/{{data_source}}/connections/{{connection}}

#### Headers

- Content-Type (string, required) - application/json

#### Path Parameters

- data_source (string, required) - Data source
- connection (integer, required) - Connection identifier

#### Query Parameters

- token (string, required) - Auth Token

#### Request Body

**@TODO**

```json
{
  "parentIdentifier": "ROOT",
  "name": "test",
  "identifier": "1",
  "activeConnections": 0,
  "protocol": "rdp",
  "parameters": {
    "port": "",
    "read-only": "",
    "swap-red-blue": "",
    "cursor": "",
    "color-depth": "",
    "clipboard-encoding": "",
    "disable-copy": "",
    "disable-paste": "",
    "dest-port": "",
    "recording-exclude-output": "",
    "recording-exclude-mouse": "",
    "recording-include-keys": "",
    "create-recording-path": "",
    "enable-sftp": "",
    "sftp-port": "",
    "sftp-server-alive-interval": "",
    "enable-audio": "",
    "security": "",
    "disable-auth": "",
    "ignore-cert": "",
    "gateway-port": "",
    "server-layout": "",
    "timezone": "",
    "console": "",
    "width": "",
    "height": "",
    "dpi": "",
    "resize-method": "",
    "console-audio": "",
    "disable-audio": "",
    "enable-audio-input": "",
    "enable-printing": "",
    "enable-drive": "",
    "create-drive-path": "",
    "enable-wallpaper": "",
    "enable-theming": "",
    "enable-font-smoothing": "",
    "enable-full-window-drag": "",
    "enable-desktop-composition": "",
    "enable-menu-animations": "",
    "disable-bitmap-caching": "",
    "disable-offscreen-caching": "",
    "disable-glyph-caching": "",
    "preconnection-id": "",
    "hostname": "",
    "username": "",
    "password": "",
    "domain": "",
    "gateway-hostname": "",
    "gateway-username": "",
    "gateway-password": "",
    "gateway-domain": "",
    "initial-program": "",
    "client-name": "",
    "printer-name": "",
    "drive-name": "",
    "drive-path": "",
    "static-channels": "",
    "remote-app": "",
    "remote-app-dir": "",
    "remote-app-args": "",
    "preconnection-blob": "",
    "load-balance-info": "",
    "recording-path": "",
    "recording-name": "",
    "sftp-hostname": "",
    "sftp-host-key": "",
    "sftp-username": "",
    "sftp-password": "",
    "sftp-private-key": "",
    "sftp-passphrase": "",
    "sftp-root-directory": "",
    "sftp-directory": ""
  },
  "attributes": {
    "max-connections": "",
    "max-connections-per-user": "",
    "weight": "",
    "failover-only": "",
    "guacd-port": "",
    "guacd-encryption": "",
    "guacd-hostname": ""
  }
}
```

### Response

#### Status Code

- 204 - No Content

#### Response Body

This request does not return a response body.

---

## Update Telnet Connection

Updates Telnet connection.

<!-- omit in toc -->
### PUT /api/session/data/{{data_source}}/connections/{{connection}}

#### Headers

- Content-Type (string, required) - application/json

#### Path Parameters

- data_source (string, required) - Data source
- connection (integer, required) - Connection identifier

#### Query Parameters

- token (string, required) - Auth Token

#### Request Body

**@TODO**

```json
{
  "parentIdentifier": "ROOT",
  "name": "test",
  "identifier": "1",
  "activeConnections": 0,
  "protocol": "telnet",
  "parameters": {
    "port": "",
    "read-only": "",
    "swap-red-blue": "",
    "cursor": "",
    "color-depth": "",
    "clipboard-encoding": "",
    "disable-copy": "",
    "disable-paste": "",
    "dest-port": "",
    "recording-exclude-output": "",
    "recording-exclude-mouse": "",
    "recording-include-keys": "",
    "create-recording-path": "",
    "enable-sftp": "",
    "sftp-port": "",
    "sftp-server-alive-interval": "",
    "enable-audio": "",
    "color-scheme": "",
    "font-size": "",
    "scrollback": "",
    "backspace": "",
    "terminal-type": "",
    "create-typescript-path": "",
    "hostname": "",
    "username": "",
    "password": "",
    "username-regex": "",
    "password-regex": "",
    "login-success-regex": "",
    "login-failure-regex": "",
    "font-name": "",
    "typescript-path": "",
    "typescript-name": "",
    "recording-path": "",
    "recording-name": ""
  },
  "attributes": {
    "max-connections": "",
    "max-connections-per-user": "",
    "weight": "",
    "failover-only": "",
    "guacd-port": "",
    "guacd-encryption": "",
    "guacd-hostname": ""
  }
}
```

### Response

#### Status Code

- 204 - No Content

#### Response Body

This request does not return a response body.

---

## Update Kubernetes Connection

Updates Kubernetes connection.

<!-- omit in toc -->
### PUT /api/session/data/{{data_source}}/connections/{{connection}}

#### Headers

- Content-Type (string, required) - application/json

#### Path Parameters

- data_source (string, required) - Data source
- connection (integer, required) - Connection identifier

#### Query Parameters

- token (string, required) - Auth Token

#### Request Body

**@TODO**

```json
{
  "parentIdentifier": "ROOT",
  "name": "test",
  "identifier": "1",
  "activeConnections": 0,
  "protocol": "kubernetes",
  "parameters": {
    "port": "",
    "read-only": "",
    "swap-red-blue": "",
    "cursor": "",
    "color-depth": "",
    "clipboard-encoding": "",
    "disable-copy": "",
    "disable-paste": "",
    "dest-port": "",
    "recording-exclude-output": "",
    "recording-exclude-mouse": "",
    "recording-include-keys": "",
    "create-recording-path": "",
    "enable-sftp": "",
    "sftp-port": "",
    "sftp-server-alive-interval": "",
    "enable-audio": "",
    "use-ssl": "",
    "ignore-cert": "",
    "color-scheme": "",
    "font-size": "",
    "scrollback": "",
    "backspace": "",
    "create-typescript-path": "",
    "hostname": "",
    "ca-cert": "",
    "namespace": "",
    "pod": "",
    "container": "",
    "client-cert": "",
    "client-key": "",
    "font-name": "",
    "typescript-path": "",
    "typescript-name": "",
    "recording-path": "",
    "recording-name": ""
  },
  "attributes": {
    "max-connections": "",
    "max-connections-per-user": "",
    "weight": "",
    "failover-only": "",
    "guacd-port": "",
    "guacd-encryption": "",
    "guacd-hostname": ""
  }
}
```

### Response

#### Status Code

- 204 - No Content

#### Response Body

This request does not return a response body.

---

## Delete Connection

Deletes given connection.

<!-- omit in toc -->
### DELETE /api/session/data/{{data_source}}/connections/{{connection}}

#### Headers

None.

#### Path Parameters

- data_source (string, required) - Data source
- connection (integer, required) - Connection identifier

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

[Back to Top](#connections)
