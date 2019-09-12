## Get All Dispatch Groups

### HTTP Request

`GET https://api.sardynamics.com/dispatch_groups.json`

```shell
curl "https://api.sardynamics.com/dispatch_groups.json"
  -H "Authorization: abbe0983-7b75-53df-bc32-009b79d2c61e"
```

> The response to this request is a JSON object structured like this:

```json
[
  {
    "name": "Division",
    "created_at": "2019-08-07T11:31:52.836Z",
    "updated_at": "2019-08-07T11:31:52.836Z",
    "id": "1229b512-ce0d-4082-aa42-d241ad65566b",
    "tenant_id": "196a0475-6cd1-4f30-b061-caf3e8649c06",
    "unit_id": "f747ddfa-c6a2-444d-ba9e-f849ea7a5bea",
    "resources_count": 2,
    "resources": [
      {
        "identifier": "00001",
        "name": "Fire Truck 21",
        "created_at": "2018-11-24T15:32:57.690Z",
        "updated_at": "2018-11-24T15:32:57.690Z",
        "phone_number": "",
        "on_call": null,
        "vehicle": null,
        "device_info": {
          "url": "",
          "url_description": "",
          "device_type": "Fire Truck"
        },
        "year": null,
        "last_time_in_operation": null,
        "latest_operation_name": null,
        "device_type": "Fire Truck",
        "tetra": "",
        "inactive": false,
        "id": "c88e1a75-1fd6-4b7a-86ed-273cfe14d88a",
        "email": null,
        "phone_number_area_code": null,
        "call_id": null,
        "custodian_id": null,
        "latest_operation_id": null,
        "tenant_user_id": null,
        "tenant_id": "196a0475-6cd1-4f30-b061-caf3e8649c06",
        "unit_id": "f747ddfa-c6a2-444d-ba9e-f849ea7a5bea",
        "watch_id": null,
        "deleted": false,
        "inactive_unit": false
      },
      {
        "identifier": "demo",
        "name": "Jane Doe",
        "created_at": "2018-10-13T16:35:35.460Z",
        "updated_at": "2018-11-27T17:41:34.569Z",
        "phone_number": "91844161",
        "on_call": null,
        "vehicle": null,
        "device_info": "{}",
        "year": null,
        "last_time_in_operation": null,
        "latest_operation_name": null,
        "device_type": null,
        "tetra": "",
        "inactive": false,
        "id": "441d7391-e14c-4701-bf65-f557dc9593b7",
        "email": "info@sareye.com",
        "phone_number_area_code": "+45",
        "call_id": null,
        "custodian_id": null,
        "latest_operation_id": null,
        "tenant_user_id": "c389fa22-8fa1-4b3d-9c55-ab80f894c120",
        "tenant_id": "196a0475-6cd1-4f30-b061-caf3e8649c06",
        "unit_id": "f747ddfa-c6a2-444d-ba9e-f849ea7a5bea",
        "watch_id": null,
        "deleted": false,
        "inactive_unit": false
      }
    ]
  },
  {
    "name": "Emergency Headquarters",
    "created_at": "2019-08-07T11:32:11.016Z",
    "updated_at": "2019-08-07T11:32:11.016Z",
    "id": "71526340-2352-453f-b7a5-e1eb89f78e5b",
    "tenant_id": "196a0475-6cd1-4f30-b061-caf3e8649c06",
    "unit_id": "8b8a9aa6-681f-4a98-9c8f-81d3ced87c09",
    "resources_count": 1,
    "resources": [
      {
        "identifier": "demo1",
        "name": "John Doe",
        "created_at": "2018-11-24T13:59:17.553Z",
        "updated_at": "2019-08-07T11:29:57.044Z",
        "phone_number": "(555) 1234 1234",
        "on_call": null,
        "vehicle": null,
        "device_info": "{}",
        "year": null,
        "last_time_in_operation": null,
        "latest_operation_name": null,
        "device_type": null,
        "tetra": "",
        "inactive": false,
        "id": "ef906f9c-c1d3-4da7-801b-9bd192438962",
        "email": "info@sareye.com",
        "phone_number_area_code": "+354",
        "call_id": null,
        "custodian_id": null,
        "latest_operation_id": null,
        "tenant_user_id": "4245bd51-df24-47d4-b9e5-541add586eec",
        "tenant_id": "196a0475-6cd1-4f30-b061-caf3e8649c06",
        "unit_id": "8b8a9aa6-681f-4a98-9c8f-81d3ced87c09",
        "watch_id": null,
        "deleted": false,
        "inactive_unit": false
      }
    ]
  }
]
```
