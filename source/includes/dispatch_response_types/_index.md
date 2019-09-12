## Get All Dispatch Response Types

### HTTP Request

`GET https://api.sardynamics.com/dispatch_response_types.json`

```shell
curl "https://api.sardynamics.com/dispatch_response_types.json"
  -H "Authorization: abbe0983-7b75-53df-bc32-009b79d2c61e"
```

> The response to this request is a JSON object structured like this:

```json
[
  {
    "id": "47a9aa18-f574-4a78-901c-20e3bb28975b",
    "name": "Can attend",
    "tenant_id": "196a0475-6cd1-4f30-b061-caf3e8649c06",
    "deleted": false,
    "require_time": true,
    "created_at": "2018-11-24T09:39:40.612Z",
    "updated_at": "2018-11-24T09:39:40.612Z"
  },
  {
    "id": "54957e36-84dc-48f0-be07-7082f4f7a7aa",
    "name": "Can not attend",
    "tenant_id": "196a0475-6cd1-4f30-b061-caf3e8649c06",
    "deleted": false,
    "require_time": false,
    "created_at": "2018-11-24T09:40:00.546Z",
    "updated_at": "2018-11-24T09:40:00.546Z"
  },
  {
    "id": "91b4705d-c15a-46d0-bac5-66236ad58727",
    "name": "Will attend",
    "tenant_id": "196a0475-6cd1-4f30-b061-caf3e8649c06",
    "deleted": false,
    "require_time": true,
    "created_at": "2018-11-24T09:39:18.026Z",
    "updated_at": "2018-11-24T09:39:18.026Z"
  }
]
```
