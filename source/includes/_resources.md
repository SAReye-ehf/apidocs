# Resources

## Get All Resources

### HTTP Request

`GET https://api.sardynamics.com/resources.json`

### URL Parameters

| Parameter               | Format  | Description                                   |
| ----------------------- | ------- | --------------------------------------------- |
| last_response_timestamp | ISO8601 | Get all resources updated after the timestamp |

```shell
curl "https://api.sardynamics.com/resources.json"
  -H "Authorization: abbe0983-7b75-53df-bc32-009b79d2c61e"
```

> The response to this request is a JSON object structured like this:

```json
{
  "last_response_timestamp": "2019-09-12T11:11:39.232+02:00",
  "tenant_id": "196a0475-6cd1-4f30-b061-caf3e8649c06",
  "data": [
    {
      "identifier": "demo",
      "name": "Jane Doe",
      "created_at": "2018-10-13T16:35:35.460Z",
      "updated_at": "2018-11-27T17:41:34.569Z",
      "phone_number": "91844161",
      "device_info": "{}",
      "tetra": "",
      "inactive": false,
      "id": "441d7391-e14c-4701-bf65-f557dc9593b7",
      "email": "info@sareye.com",
      "phone_number_area_code": "+45",
      "tenant_user_id": "c389fa22-8fa1-4b3d-9c55-ab80f894c120",
      "tenant_id": "196a0475-6cd1-4f30-b061-caf3e8649c06",
      "unit_id": "f747ddfa-c6a2-444d-ba9e-f849ea7a5bea",
      "deleted": false,
      "inactive_unit": false,
      "unit": {
        "name": "Division",
        "disabled": false,
        "call_sign": "Div",
        "id": "f747ddfa-c6a2-444d-ba9e-f849ea7a5bea",
        "area_id": "906006ae-7c44-428f-8312-df243294bad7",
        "tenant_id": "196a0475-6cd1-4f30-b061-caf3e8649c06",
        "area": {
          "name": "East",
          "id": "906006ae-7c44-428f-8312-df243294bad7"
        }
      }
    },
    {
      "identifier": "demo1",
      "name": "John Doe",
      "created_at": "2018-11-24T13:59:17.553Z",
      "updated_at": "2019-08-07T11:29:57.044Z",
      "phone_number": "(555) 1234 1234",
      "device_info": "{}",
      "tetra": "",
      "inactive": false,
      "id": "ef906f9c-c1d3-4da7-801b-9bd192438962",
      "email": "info@sareye.com",
      "phone_number_area_code": "+354",
      "tenant_user_id": "4245bd51-df24-47d4-b9e5-541add586eec",
      "tenant_id": "196a0475-6cd1-4f30-b061-caf3e8649c06",
      "unit_id": "8b8a9aa6-681f-4a98-9c8f-81d3ced87c09",
      "deleted": false,
      "inactive_unit": false,
      "unit": {
        "name": "Emergency Headquarters",
        "disabled": false,
        "call_sign": "HQ",
        "id": "8b8a9aa6-681f-4a98-9c8f-81d3ced87c09",
        "area_id": "99d9e1d8-7f2a-4643-8982-e64615c314f4",
        "tenant_id": "196a0475-6cd1-4f30-b061-caf3e8649c06",
        "area": {
          "name": "South",
          "id": "99d9e1d8-7f2a-4643-8982-e64615c314f4"
        }
      }
    }
  ]
}
```
