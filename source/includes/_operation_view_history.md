# Operation View History

## Get All Operation Views

### Available Parameters

| Key          | Type   | Description                                        |
| ------------ | ------ | -------------------------------------------------- |
| start_date   | String | Start Date                                         |
| end_date     | String | End Date                                           |
| resource_id  | String | id of the resource you want to look up (optional)  |
| operation_id | String | id of the operation you want to look up (optional) |

### HTTP Request

`GET https://api.sardynamics.com/devices.json`

```shell
curl "https://api.sardynamics.com/devices.json?page=1"
  -H "Authorization: abbe0983-7b75-53df-bc32-009b79d2c61e"
```

> The response to this request is a JSON object structured like this:

```json
[
  {
    "created_at": "2019-09-02T13:54:46.073Z",
    "updated_at": "2019-09-02T13:54:46.073Z",
    "id": "1a9bc8ab-f49f-4430-bbff-b82f6ea47d31",
    "operation_id": "bd241c9d-38e6-4e44-8a0a-df53b9e3bb92",
    "user_id": "738d3640-3fbd-4a5e-aaeb-a085625af812",
    "resource_id": "441d7391-e14c-4701-bf65-f557dc9593b7"
  },
  {
    "created_at": "2019-09-02T13:51:32.214Z",
    "updated_at": "2019-09-02T13:51:32.214Z",
    "id": "18978ae3-3d06-489c-8015-5b5dc10e50a0",
    "operation_id": "73222fec-c89b-45ef-9a5c-1ff64ccb0da2",
    "user_id": "738d3640-3fbd-4a5e-aaeb-a085625af812",
    "resource_id": "441d7391-e14c-4701-bf65-f557dc9593b7"
  }
]
```
