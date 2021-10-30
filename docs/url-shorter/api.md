---
sidebar_label: API Reference
title: API Reference
sidebar_position: 1
---

The base url is https://short.craftions.net

#### Create Link

```http
  GET /api/v1/url/create
```

| Parameter | Type     | Description                       |
| :-------- | :------- | :-------------------------------- |
| `target` | `string` | The url target |

Returns a JSON Object with the fields `error`, `message` and `id`
