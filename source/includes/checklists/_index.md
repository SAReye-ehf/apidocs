## Get All Checklists for a specific operation

### HTTP Request

`GET https://api.sardynamics.com/operation/:operation_id/checklists.json`

```shell
curl "https://api.sardynamics.com/operation/:operation_id/checklists.json"
  -H "Authorization: abbe0983-7b75-53df-bc32-009b79d2c61e"
```

> The response to this request is a JSON object structured like this:

```json
[
  {
    "id": "456603f6-dd71-4158-9b41-9451eb9301fe",
    "name": "SÁBF - Björgun",
    "description": "",
    "template": false,
    "round_id": "efc820f3-3a1c-4be6-87f2-89e8d8d08cc1",
    "user_id": null,
    "deleted": false,
    "tenant_id": "ad9bf99e-ecce-4abb-be35-eb9a3b47a2da",
    "created_at": "2019-09-19T15:22:25.136Z",
    "updated_at": "2019-09-19T15:22:25.136Z",
    "tasks": [{"..."}]
  }
]
```
