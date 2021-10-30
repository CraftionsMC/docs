---
sidebar_label: API Reference
title: API Reference
sidebar_position: 1
id: api
---

The base url is https://analyze.craftions.net

#### Submit data for a website

```http
  POST /api/v1/analyze
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `location` | `object` |  |
| `location.protocol` | `string` | The protocol of the webpage |
| `location.host` | `string` | The host |
| `location.path` | `string` | The path |
| `location.port` | `string` | The port |
| `location.origin` | `string` | The origin (e.g. https://craftions.net) |
| `location.href` | `string` | The href (e.g. https://craftions.net/) || `location` | `object` |  |
| `siteData` | `object` |  |
| `siteData.title` | `string` | The title of the document |
| `clientData` | `object` |  |
| `clientData.browser` | `string` | The user agent |
| `clientData.screenColors` | `string` | The screen colors (bit mode) |
| `clientData.language` | `string` | The navigator language |
| `clientData.darkMode` | `boolean` | Darkmode enabled |

Returns a JSON Object with the fields `error`, `message`

#### Get Analytics for website

```http
  POST /api/v1/analytics
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `host` | `string` |  The hostname (e.g craftions.net)|