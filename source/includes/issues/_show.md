## Get a Specific Issue

```shell
curl "https://api.sardynamics.com/issues/abbe0983-7b75-53df-bc32-009b79d2c61e"
  -H "Authorization: abbe0983-7b75-53df-bc32-009b79d2c61e"
```

> The response to this request is a JSON object structured like this:

```json
{
  "id": "aee23f75-ead3-5c15-853d-fb27a85ed512",
  "name": "Lorem ipsum",
  "description": "Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.",
  "issue_type_id": "ec79e69c-6720-54d0-84e2-bd700704763e",
  "anonymous": false,
  "solved": true,
  "user_id": "a8e74080-e8cd-58e3-a881-cb98c4514547",
  "creator_resource_id": "118f00e0-184f-5744-884b-657eb4b3c1ca",
  "unit_id": "fb694644-ab61-5564-8f35-ce1d16012715",
  "tenant_id": "48c47225-a6e2-5e66-a415-0a84f93a1808",
  "created_at": "2019-09-09T17:59:40.655Z",
  "updated_at": "2019-09-09T18:03:14.279Z",
  "comments_count": 0
}
```

This endpoint retrieves a specific issue.

### HTTP Request

`GET http://example.com/issues/<ID>.json`

### URL Parameters

| Parameter | Description                     |
| --------- | ------------------------------- |
| ID        | The ID of the issue to retrieve |
