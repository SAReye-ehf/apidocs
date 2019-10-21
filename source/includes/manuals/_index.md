## Getting a list of all Manuals

### HTTP Request

`GET https://api.sardynamics.com/manuals.json`

```shell
curl "https://api.sardynamics.com/manuals.json"
  -H "Authorization: abbe0983-7b75-53df-bc32-009b79d2c61e"
```

> The response to this request is a JSON object structured like this:

```json
[
  {
    "items": "Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. ",
    "created_at": "2013-09-30T21:46:10.446Z",
    "updated_at": "2019-08-21T01:30:24.445Z",
    "global": true,
    "name": "First Checklist",
    "deleted": null,
    "link": "",
    "id": "030f1ecf-ebc5-5431-b83b-dcb1dacd4966",
    "operation_id": null,
    "tenant_id": "c6c781db-65d3-5b20-9a96-08a4e5870566",
    "user_id": "795c3d32-4c6d-5c27-b51b-ca249ceca6cc"
  },
  {
    "items": "Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.",
    "created_at": "2017-02-08T20:45:29.122Z",
    "updated_at": "2017-02-08T20:55:02.882Z",
    "global": null,
    "name": "Second Checklist",
    "deleted": null,
    "link": null,
    "id": "d34a25e5-390f-528c-bf95-9272af5b4409",
    "operation_id": null,
    "tenant_id": "2cf5285c-dadd-5fa2-a72f-dda5fcf666b3",
    "user_id": "58cd8419-5ece-5209-9099-e31b9acb9e12"
  }
]
```
