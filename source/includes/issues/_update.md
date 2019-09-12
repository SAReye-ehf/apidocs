## Update a Specific Issue

```shell
curl "https://api.sardynamics.com/issues/abbe0983-7b75-53df-bc32-009b79d2c61e"
  -X PATCH
  -H "Authorization: abbe0983-7b75-53df-bc32-009b79d2c61e"
```

> The response to this request is a JSON object structured like this:

```json
{
  "id": "bc2fa047-41ab-4847-9fdf-31e02d2b3e187",
  "name": "Slippery stairs",
  "description": "Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.",
  "issue_type_id": "f3129e67-9d93-4654-b250-b76bf5c95c53",
  "anonymous": false,
  "solved": false,
  "user_id": "ga200aa8-374d-4c18-12d4-4c49f94a631d",
  "creator_resource_id": "bfd26aa9-4a1c-45e0-af2h-8268b3b38b87",
  "unit_id": "b333cb95-d1d2-47de-af2h-724518758073",
  "tenant_id": "ad9bf99e-12gv-4abb-af2h-eb9a3b47a2da",
  "created_at": "2019-09-09T17:59:40.655Z",
  "updated_at": "2019-09-09T18:03:14.279Z",
  "comments_count": 0
}
}
```

### HTTP Request

`PATCH http://example.com/issues/<ID>`

### Parameters

| Key                            | Type                 | Description                                          |
| ------------------------------ | -------------------- | ---------------------------------------------------- |
| issue[name]                    | String               | Short description of the issue                       |
| issue[description]             | String               | Explanation of the issue                             |
| issue[issue_type_id]           | String (uuid)        | Type of issue                                        |
| issue[solved]                  | Boolean              | Has the issue been solved or not                     |
| issue[anonymous]               | Boolean              | Post the issue anonymously                           |
| issue[unit_id]                 | String (uuid)        | The unit responsible for the issue                   |
| issue[tag_ids][]               | Array[String (uuid)] | Assigned tags                                        |
| issue[assigned_resource_ids][] | Array[String (uuid)] | Resources that are assigned to investigate the issue |
| issue[affected_resource_ids][] | Array[String (uuid)] | Resources that are affected by the issue             |
