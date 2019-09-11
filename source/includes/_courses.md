# Courses

## Getting a list of all Courses

### HTTP Request

`GET https://api.sardynamics.com/courses.json`

```shell
curl "https://api.sardynamics.com/courses.json"
  -H "Authorization: abbe0983-7b75-53df-bc32-009b79d2c61e"
```

> The response to this request is a JSON object structured like this:

```json
[
  {
    "id": "7139c3ec-d15f-4af1-940b-dacd863e2a84",
    "name": "Operation Management",
    "description": "Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.",
    "days_valid": null,
    "expires": true,
    "disabled": false,
    "tenant_id": "ad9bf99e-ecce-4abb-be35-eb9a3b47a2da",
    "data": {
      "type": "",
      "field": "",
      "price": "",
      "program": "",
      "minimum_age": "18"
    },
    "created_at": "2019-04-19T11:38:26.377Z",
    "updated_at": "2019-04-19T11:38:26.377Z",
    "tag_id": "ddee449f-23dc-46f6-abba-33d1a98922d7"
  },
  {
    "id": "d23bd5ca-fab1-503a-bb0a-726d565ad562",
    "name": "First Response",
    "description": "",
    "days_valid": null,
    "expires": false,
    "disabled": false,
    "tenant_id": "ad9bf99e-ecce-4abb-be35-eb9a3b47a2da",
    "data": {
      "type": "",
      "field": "",
      "price": "",
      "program": "",
      "minimum_age": ""
    },
    "created_at": "2019-04-19T12:51:18.310Z",
    "updated_at": "2019-04-19T12:51:18.310Z",
    "tag_id": "80b253e0-a9f1-4d0d-9c3a-97022b9e3e9f"
  }
]
```
