## Get All Devices

### Available Parameters

| Key    | Type   | Description                        |
| ------ | ------ | ---------------------------------- |
| search | String | Search String                      |
| page   | String | Devices are paginated, 20 per page |

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
    "identifier": "00001",
    "name": "Fire Truck 21",
    "created_at": "2018-11-24T15:32:57.690Z",
    "updated_at": "2018-11-24T15:32:57.690Z",
    "phone_number": "",
    "device_info": {
      "url": "",
      "url_description": "",
      "device_type": "Fire Truck"
    },
    "device_type": "Fire Truck",
    "tetra": "",
    "inactive": false,
    "id": "c88e1a75-1fd6-4b7a-86ed-273cfe14d88a",
    "tenant_id": "196a0475-6cd1-4f30-b061-caf3e8649c06",
    "unit_id": "f747ddfa-c6a2-444d-ba9e-f849ea7a5bea",
    "deleted": false,
    "inactive_unit": false,
    "type": "Device"
  }
]
```
