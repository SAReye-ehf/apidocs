## Get All Issues

### Available Parameters

| Key      | Type    | Description                               |
| -------- | ------- | ----------------------------------------- |
| show_all | Boolean | If true - include completed/solved issues |
| search   | String  | Search String                             |
| page     | String  | Issues are paginated, 20 per page         |

```shell
curl "https://api.sardynamics.com/issues.json?get_all=true&search=Lorem&page=1"
  -H "Authorization: abbe0983-7b75-53df-bc32-009b79d2c61e"
```

> The response to this request is a JSON object structured like this:

```json
[
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
  },
  {
    "id": "7dfbb5bc-7790-5b5d-af5e-28335b88aa12",
    "name": "Lorem ipsum2",
    "description": "Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.",
    "issue_type_id": null,
    "anonymous": false,
    "solved": false,
    "user_id": "4943e7bd-c292-53c6-91d2-dc9bb3ae2ea3",
    "creator_resource_id": "d020fd3e-d385-55d9-88f7-0504b35336ef",
    "unit_id": null,
    "tenant_id": "e3968f1d-4c57-518d-8e5a-a924ad0e8029",
    "created_at": "2019-08-26T13:15:37.321Z",
    "updated_at": "2019-09-09T22:36:26.963Z",
    "comments_count": 3
  }
]
```

This endpoint retrieves all issues.

### HTTP Request

`GET https://api.sardynamics.com/issues.json`
