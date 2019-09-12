## Getting a list of all Operation Logs

### HTTP Request

`GET https://api.sardynamics.com/operation_logs.json`

### Available Parameters

| Key                    | Type    | Description                                   |
| ---------------------- | ------- | --------------------------------------------- |
| operation_id           | Integer | Optional filter by operation                  |
| include_attachments    | Boolean | Return attachments in the response            |
| include_operation_lite | Boolean | Include operation name and id in the response |

```shell
curl "https://api.sardynamics.com/operation_logs.json"
  -H "Authorization: abbe0983-7b75-53df-bc32-009b79d2c61e"
```

> The response to this request is a JSON object structured like this:

```json
{
  "data": [
    {
      "text": "Extent of damage",
      "marked": null,
      "filename": null,
      "created_at": "2019-08-12T13:45:40.022Z",
      "updated_at": "2019-08-12T13:45:40.261Z",
      "file": {
        "url": null,
        "thumb": {
          "url": null
        }
      },
      "deleted": false,
      "lat": "",
      "lng": "",
      "log_time": "2019-08-12T13:44:07.000Z",
      "pointtype": null,
      "timeline": false,
      "end_time": null,
      "mobile": false,
      "show_on_map": true,
      "movement": null,
      "url": {
        "primary_url": "",
        "primary_url_bitly": ""
      },
      "data": {
        "radius": {
          "value": "",
          "unit": "m"
        },
        "user_j": {
          "id": "f8976e89-92ec-57be-8753-3036297723c3",
          "email": "john@gmail.com",
          "name": "John Doe",
          "phone_number": "12345678"
        },
        "tenant_j": {
          "abbreviation": "SAReye"
        },
        "creator_resource_j": {
          "identifier": "12345678",
          "name": "John Doe",
          "created_at": "2017-10-25T13:38:39.180Z",
          "updated_at": "2019-01-22T20:55:07.312Z",
          "phone_number": "1324567",
          "device_info": "{}",
          "tetra": "",
          "inactive": false,
          "id": "14f896cc-e19c-507c-9b30-24d4404b15db",
          "email": "info@sareye.com",
          "phone_number_area_code": "+354",
          "tenant_user_id": "38c7bbea-5096-59be-97c4-5fa5c21ffc67",
          "tenant_id": "0e292763-40f6-5a0b-a6aa-5befbba3830b",
          "unit_id": "7b9c0670-5a5a-5e55-a452-a85fd2f2df0f",
          "deleted": false,
          "inactive_unit": false,
          "unit": {
            "name": "Incident Command Center",
            "call_sign": "ICC"
          },
          "tenant": {
            "abbreviation": "SAReye",
            "id": "44a577f8-85b4-4f9f-8ad2-3cb86b983509"
          }
        },
        "attachments_count": 1
      },
      "decimal_lat": null,
      "decimal_lng": null,
      "custom_values": {},
      "id": "fd68138f-8b64-48d2-9374-785b6f878ff6",
      "creator_resource_id": "fe9b94bc-ac60-52a9-9183-9d31ac66738a",
      "creator_tenant_id": "7f3dffc3-77c1-5210-8b84-241dec3241d8",
      "equipment_id": null,
      "marker_type_id": null,
      "operation_id": "109a1f1e-e067-485d-ab10-e0d361b3f216",
      "task_id": null,
      "user_id": "ff57a58a-4568-50b9-baa5-33641e08742f",
      "tags": [],
      "user": {
        "name": "John Doe",
        "include_picture": {
          "name": "image.png",
          "path": "example.com/image.png",
          "created_at": "2018-10-03T09:27:20.524Z",
          "small": "example.com/small/image.png"
        }
      },
      "creator_tenant": {
        "theme_color": "#ff9300"
      }
    }
  ],
  "operation_id": null,
  "last_response_timestamp": "2019-09-12T16:06:55.305+02:00",
  "oplogs_count": 1
}
```
