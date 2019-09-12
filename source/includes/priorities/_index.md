## Get All Priorities

### HTTP Request

`GET https://api.sardynamics.com/priorities.json`

```shell
curl "https://api.sardynamics.com/priorities.json"
  -H "Authorization: abbe0983-7b75-53df-bc32-009b79d2c61e"
```

> The response to this request is a JSON object structured like this:

```json
[
  {
    "name": "P1",
    "created_at": "2018-10-13T16:34:17.517Z",
    "updated_at": "2018-10-13T16:34:17.517Z",
    "disabled": false,
    "rank": 1,
    "default": null,
    "operation_priority": true,
    "task_priority": true,
    "id": "413e41e2-c0eb-4450-a455-826b5ce0dd4f",
    "tenant_id": "196a0475-6cd1-4f30-b061-caf3e8649c06",
    "fill_in_text": null
  },
  {
    "name": "P2",
    "created_at": "2018-10-13T16:34:17.524Z",
    "updated_at": "2018-10-13T16:34:17.524Z",
    "disabled": false,
    "rank": 2,
    "default": true,
    "operation_priority": true,
    "task_priority": true,
    "id": "1437d403-f22b-44b5-875d-f58aa9020ad5",
    "tenant_id": "196a0475-6cd1-4f30-b061-caf3e8649c06",
    "fill_in_text": null
  },
  {
    "name": "P3",
    "created_at": "2018-10-13T16:34:17.539Z",
    "updated_at": "2018-10-13T16:34:17.539Z",
    "disabled": false,
    "rank": 3,
    "default": null,
    "operation_priority": true,
    "task_priority": true,
    "id": "117c73fd-dfd0-4b2e-abbc-0a874c1e35b8",
    "tenant_id": "196a0475-6cd1-4f30-b061-caf3e8649c06",
    "fill_in_text": null
  }
]
```
