# Issues

## Get All Issues

### Available Parameters

| key      | type    | description                               |
| -------- | ------- | ----------------------------------------- |
| show_all | Boolean | If true - include completed/solved issues |
| search   | String  | Search String                             |
| page     | String  | Issues are paginated, 20 per page         |

```shell
curl "https://api.sardynamics.com/issues?get_all=true&search=Lorem&page=1"
  -H "Authorization: abbe0983-7b75-53df-bc32-009b79d2c61e"
```

> The above command returns JSON structured like this:

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

`GET https://api.sardynamics.com/issues`

## Get a Specific Issue

```shell
curl "https://api.sardynamics.com/issues/abbe0983-7b75-53df-bc32-009b79d2c61e"
  -H "Authorization: abbe0983-7b75-53df-bc32-009b79d2c61e"
```

> The above command returns JSON structured like this:

```json
{
  "name": "02",
  "created_at": "2017-10-25T13:07:15.283Z",
  "updated_at": "2017-12-04T14:19:08.239Z",
  "disabled": false,
  "json": null,
  "description": "",
  "lat": "65 32.000",
  "lng": "-23 04.000",
  "zoom": 8,
  "has_polygon": false,
  "id": "614ec74c-2749-541a-ab68-e8ccc3da2b26",
  "tenant_id": "ecaf17fa-df8b-51e9-b370-9963438b1fb3"
}
```

This endpoint retrieves a specific issue.

### HTTP Request

`GET http://example.com/issues/<ID>`

### URL Parameters

| Parameter | Description                     |
| --------- | ------------------------------- |
| ID        | The ID of the issue to retrieve |

## Create a new issue

### HTTP request

`POST http://example.com/issues`

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

## Update a Specific Issue

```shell
curl "https://api.sardynamics.com/issues/abbe0983-7b75-53df-bc32-009b79d2c61e"
  -X PATCH
  -H "Authorization: abbe0983-7b75-53df-bc32-009b79d2c61e"
```

> The above command returns JSON structured like this:

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

This endpoint retrieves a specific issue.

### HTTP Request

`PATCH http://example.com/issues/<ID>`

### URL Parameters

| Parameter | Description                     |
| --------- | ------------------------------- |
| ID        | The ID of the issue to retrieve |

## Delete a Specific Issue

```shell
curl "https://api.sardynamics.com/issues/27522917-bb28-530e-979d-c4b77a335114"
  -X DELETE
  -H "Authorization: abbe0983-7b75-53df-bc32-009b79d2c61e"
```

This endpoint deletes a specific issue.

### HTTP Request

`DELETE http://example.com/issues/<ID>`

### URL Parameters

| Parameter | Description                   |
| --------- | ----------------------------- |
| ID        | The ID of the issue to delete |
