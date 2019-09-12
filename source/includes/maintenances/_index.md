## Get All Maintenances

### Available Parameters

| Key      | Type    | Description                                              |
| -------- | ------- | -------------------------------------------------------- |
| show_all | Boolean | Default: false, If true - include completed maintenances |

### HTTP Request

`GET https://api.sardynamics.com/maintenances.json?get_all=true`

```shell
curl "https://api.sardynamics.com/maintenances.json?get_all=true"
  -H "Authorization: abbe0983-7b75-53df-bc32-009b79d2c61e"
```

> The response to this request is a JSON object structured like this:

```json
[
  {
    "id": "1f72861d-e697-41fd-851e-67370f421b43",
    "device_id": "c88e1a75-1fd6-4b7a-86ed-273cfe14d88a",
    "user_id": "738d3640-3fbd-4a5e-aaeb-a085625af812",
    "tenant_id": "196a0475-6cd1-4f30-b061-caf3e8649c06",
    "name": "Rear axle replacement",
    "description": "",
    "maintenance_date": "2019-08-07T11:26:00.000Z",
    "reminder": false,
    "reminder_date": "2019-08-07T11:26:00.000Z",
    "created_at": "2019-08-07T11:26:53.681Z",
    "updated_at": "2019-08-07T11:26:53.681Z",
    "reminder_sent": false,
    "completed": false,
    "operation_id": null,
    "resource_id": "ef906f9c-c1d3-4da7-801b-9bd192438962"
  }
]
```
