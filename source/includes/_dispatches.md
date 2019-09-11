# Dispatches

## Getting a list of all Dispatches

### HTTP Request

`GET https://api.sardynamics.com/dispatches.json`

```shell
curl "https://api.sardynamics.com/dispatches.json"
  -H "Authorization: abbe0983-7b75-53df-bc32-009b79d2c61e"
```

> The response to this request is a JSON object structured like this:

```json
[
  {
    "id": "bbc9580e-fdfd-41f7-ac96-dee91131f64d",
    "message": "test",
    "operation_id": "d6af1803-5020-4326-bcf3-017c55ea1ed6",
    "tenant_id": "44a577f8-85b4-4f9f-8ad2-3cb86b983509",
    "priority_id": "fe48fc85-603f-4841-bd03-8d760cc7553d",
    "user_id": "94a15900-7fe4-4a44-b850-02d66f274485",
    "created_at": "2019-09-11T11:16:29.958Z",
    "updated_at": "2019-09-11T11:16:29.958Z",
    "resources_count": 3
  },
  {
    "id": "f8fd787c-b350-41f8-b11a-28f40c6c964d",
    "message": "First responders needed for wilderness rescue.",
    "operation_id": "d6af1803-5020-4326-bcf3-017c55ea1ed6",
    "tenant_id": "44a577f8-85b4-4f9f-8ad2-3cb86b983509",
    "priority_id": "d1f09aed-e591-4a33-85cf-0f7649ed9805",
    "user_id": "94a15900-7fe4-4a44-b850-02d66f274485",
    "created_at": "2019-08-07T13:22:02.773Z",
    "updated_at": "2019-08-07T13:22:02.773Z",
    "resources_count": 3
  }
]
```
