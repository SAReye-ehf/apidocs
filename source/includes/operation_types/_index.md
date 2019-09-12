## Get All Operation Types

### HTTP Request

`GET https://api.sardynamics.com/operation_types.json`

```shell
curl "https://api.sardynamics.com/operation_types.json?page=1"
  -H "Authorization: abbe0983-7b75-53df-bc32-009b79d2c61e"
```

> The response to this request is a JSON object structured like this:

```json
[
  {
    "id": "816db5bd-a108-4e45-a3a1-48eda91e3f31",
    "name": "Dispatch",
    "default_layout": "normal",
    "restrict_to_unit_by_default": false,
    "created_at": "2019-01-14T18:06:24.851Z",
    "updated_at": "2019-01-30T15:16:37.803Z",
    "tenant_id": "196a0475-6cd1-4f30-b061-caf3e8649c06",
    "show_on_frontpage": true,
    "rank": 1,
    "deleted": false
  },
  {
    "id": "db66f430-270f-45fa-b3bc-3e03dfde1f26",
    "name": "Meeting",
    "default_layout": "meetingNotes",
    "restrict_to_unit_by_default": false,
    "created_at": "2019-01-14T18:06:24.858Z",
    "updated_at": "2019-01-30T15:16:50.477Z",
    "tenant_id": "196a0475-6cd1-4f30-b061-caf3e8649c06",
    "show_on_frontpage": true,
    "rank": 2,
    "deleted": false
  },
  {
    "id": "21b0aac6-a337-4196-b577-6b9216aadd4e",
    "name": "Exercise",
    "default_layout": "normal",
    "restrict_to_unit_by_default": false,
    "created_at": "2019-01-14T18:06:24.853Z",
    "updated_at": "2019-01-30T15:17:08.058Z",
    "tenant_id": "196a0475-6cd1-4f30-b061-caf3e8649c06",
    "show_on_frontpage": true,
    "rank": 3,
    "deleted": false
  }
]
```
