# Tags

## Get All Tags

### HTTP Request

`GET https://api.sardynamics.com/tags.json`

### URL Parameters

| Parameter | Format  | Description                |
| --------- | ------- | -------------------------- |
| show_all  | Boolean | If true, show deleted tags |

```shell
curl "https://api.sardynamics.com/tags.json"
  -H "Authorization: abbe0983-7b75-53df-bc32-009b79d2c61e"
```

> The response to this request is a JSON object structured like this:

```json
[
  {
    "id": "f55ca8ce-56b3-48c0-85fb-d8550108e586",
    "name": "First Responder",
    "shared": null,
    "tenant": "SAReye",
    "color": "#fffb00"
  },
  {
    "id": "0bc3a6e8-6eb3-5df4-a998-567195c373e5",
    "name": "Doctor",
    "shared": null,
    "tenant": "SAReye",
    "color": "#fffb00"
  }
]
```
