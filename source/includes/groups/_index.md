## Getting a list of all Groups for a given operation

### HTTP Request

`GET https://api.sardynamics.com/groups.json?operation_id=:operation_id`

<aside class="notice">
You must replace <code>:operation_id</code> with the corresponding operation id.
</aside>

### Available Parameters

| Key                    | Type    | Description                                   |
| ---------------------- | ------- | --------------------------------------------- |
| operation_id           | Integer | Optional filter by operation                  |
| include_attachments    | Boolean | Return attachments in the response            |
| include_operation_lite | Boolean | Include operation name and id in the response |
| include_resources      | Boolean | Return resources in the response              |
| include_tasks          | Boolean | Return tasks in the response                  |
| hide_inactive_groups   | Boolean | Hide inactive groups(default: false)          |
| filter                 | String  | Optional search query                         |

```shell
curl "https://api.sardynamics.com/operation_logs.json"
  -H "Authorization: abbe0983-7b75-53df-bc32-009b79d2c61e"
```

> The response to this request is a JSON object structured like this:

```json
{
  "users_active_group": [],
  "data": [
    {
      "name": "Incident managers",
      "number": 0,
      "created_at": "2018-11-24T14:04:30.817Z",
      "updated_at": "2018-11-24T14:04:31.097Z",
      "deleted": false,
      "newest": null,
      "common_id": null,
      "file": {
        "url": null,
        "thumb": {
          "url": null
        }
      },
      "group_leader": null,
      "extra": 0,
      "tetra": null,
      "number_of_vehicles": 0,
      "has_tasks": false,
      "can_have_tasks": true,
      "operational": true,
      "data": {
        "device": "true",
        "tasks_j": [],
        "attachments_count": null,
        "creator_resource_j": {
          "identifier": "123456",
          "name": "Demo User",
          "created_at": "2018-11-24T13:59:17.553Z",
          "updated_at": "2018-11-24T13:59:45.037Z",
          "phone_number": "(555) 1234 1234",
          "device_info": "{}",
          "tetra": "",
          "inactive": false,
          "id": "ef906f9c-c1d3-4da7-801b-9bd192438962",
          "email": "example@sareye.com",
          "phone_number_area_code": "+1",
          "tenant_user_id": "4245bd51-df24-47d4-b9e5-541add586eec",
          "tenant_id": "196a0475-6cd1-4f30-b061-caf3e8649c06",
          "unit_id": "8b8a9aa6-681f-4a98-9c8f-81d3ced87c09",
          "deleted": false,
          "inactive_unit": false,
          "unit": {
            "name": "Emergency Headquarters",
            "call_sign": "HQ"
          },
          "tenant": {
            "abbreviation": "demo",
            "id": "196a0475-6cd1-4f30-b061-caf3e8649c06"
          }
        }
      },
      "custom_values": {},
      "id": "a10e605f-4bb6-4c83-8fc3-eea25d3863f3",
      "creator_resource_id": "ef906f9c-c1d3-4da7-801b-9bd192438962",
      "creator_tenant_id": "196a0475-6cd1-4f30-b061-caf3e8649c06",
      "operation_id": "bd241c9d-38e6-4e44-8a0a-df53b9e3bb92",
      "user_id": "d428602f-f854-4a8b-a259-bf0858a474cd",
      "group_leader_uuid": null,
      "group_leader_id": null,
      "tags": []
    },
    {
      "name": "Response group",
      "number": 0,
      "created_at": "2018-11-24T14:01:09.513Z",
      "updated_at": "2018-11-24T14:03:12.834Z",
      "deleted": false,
      "newest": null,
      "common_id": null,
      "file": {
        "url": null,
        "thumb": {
          "url": null
        }
      },
      "group_leader": null,
      "extra": 0,
      "tetra": "",
      "number_of_vehicles": 0,
      "has_tasks": false,
      "can_have_tasks": true,
      "operational": true,
      "data": {
        "device": "true",
        "tasks_j": [],
        "attachments_count": null,
        "creator_resource_j": {
          "identifier": "1235678",
          "name": "Demo User",
          "created_at": "2018-11-24T13:59:17.553Z",
          "updated_at": "2018-11-24T13:59:45.037Z",
          "phone_number": "(555) 1234 1234",
          "device_info": "{}",
          "tetra": "",
          "inactive": false,
          "id": "ef906f9c-c1d3-4da7-801b-9bd192438962",
          "email": "example@sareye.com",
          "phone_number_area_code": "+1",
          "tenant_user_id": "4245bd51-df24-47d4-b9e5-541add586eec",
          "tenant_id": "196a0475-6cd1-4f30-b061-caf3e8649c06",
          "unit_id": "8b8a9aa6-681f-4a98-9c8f-81d3ced87c09",
          "deleted": false,
          "inactive_unit": false,
          "unit": {
            "name": "Emergency Headquarters",
            "call_sign": "HQ"
          },
          "tenant": {
            "abbreviation": "demo",
            "id": "196a0475-6cd1-4f30-b061-caf3e8649c06"
          }
        }
      },
      "custom_values": {},
      "id": "04f3be24-d054-44e2-84a7-ff87e6dadf00",
      "creator_resource_id": "ef906f9c-c1d3-4da7-801b-9bd192438962",
      "creator_tenant_id": "196a0475-6cd1-4f30-b061-caf3e8649c06",
      "operation_id": "bd241c9d-38e6-4e44-8a0a-df53b9e3bb92",
      "user_id": "d428602f-f854-4a8b-a259-bf0858a474cd",
      "group_leader_uuid": null,
      "group_leader_id": null,
      "tags": []
    }
  ],
  "operation_id": "bd241c9d-38e6-4e44-8a0a-df53b9e3bb92",
  "active_groups_count": 2,
  "last_response_timestamp": "2019-09-12T16:35:13.793+02:00",
  "groups_count": 2
}
```
