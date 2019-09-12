## Getting a list of all Tasks

### HTTP Request

`GET https://api.sardynamics.com/tasks.json`

### Available Parameters

| Key                     | Type     | Description                                                |
| ----------------------- | -------- | ---------------------------------------------------------- |
| operation_id            | Integer  | Optional filter by operation                               |
| include_attachments     | Boolean  | Return attachments in the response                         |
| include_operation_lite  | Boolean  | Include operation name and id in the response              |
| include_groups          | Boolean  | Return groups in the response                              |
| include_comments        | Boolean  | Return comments in the response                            |
| last_response_timestamp | DateTime | Only fetch tasks updated/created after the given timestamp |
| hide_finished_tasks     | Boolean  | Do not return finished tasks                               |

```shell
curl "https://api.sardynamics.com/tasks.json"
  -H "Authorization: abbe0983-7b75-53df-bc32-009b79d2c61e"
```

> The response to this request is a JSON object structured like this:

```json
{
  "data": [
    {
      "name": "Search Camping areas near PLS",
      "priority": {
        "name": "P2",
        "created_at": "2018-10-13T16:34:17.524Z",
        "updated_at": "2018-10-13T16:34:17.524Z",
        "disabled": false,
        "rank": 2,
        "default": true,
        "operation_priority": true,
        "task_priority": true,
        "id": "1437d403-f22b-44b5-875d-f58aa9020ad5",
        "tenant_id": "196a0475-6cd1-4f30-b061-caf3e8649c06",
        "fill_in_text": null
      },
      "created_at": "2018-11-24T18:49:33.908Z",
      "updated_at": "2018-11-27T17:52:44.608Z",
      "deleted": false,
      "file": null,
      "rescuers": 0,
      "done": false,
      "has_groups": false,
      "lat": "64 07.907",
      "lng": "-21 54.215",
      "pointtype": null,
      "address": null,
      "reminder": null,
      "solved": 0,
      "point_type": null,
      "mobile": false,
      "end_time": null,
      "log_time": null,
      "is_control_measure": false,
      "solved_at": null,
      "data": {
        "operation_logs_j": [],
        "user_j": {
          "id": "738d3640-3fbd-4a5e-aaeb-a085625af812",
          "email": "info@sareye.com",
          "name": "Jane Doe",
          "phone_number": "555 0100"
        },
        "groups_j": [],
        "attachments_count": null,
        "search_area_j": {
          "name": "117",
          "searched": false,
          "created_at": "2018-11-24T18:49:33.992Z",
          "updated_at": "2018-11-24T18:49:33.992Z",
          "deleted": false,
          "area_size": "0.5148",
          "json": {
            "type": "polygon",
            "center": {
              "lat": 64.131782706677,
              "lng": -21.90358400344849
            },
            "geoJSON": {
              "type": "Feature",
              "geometry": {
                "type": "Polygon",
                "coordinates": [
                  {
                    "lat": 64.12665056872358,
                    "lng": -21.8873405456543
                  },
                  {
                    "lat": 64.13079045015536,
                    "lng": -21.88382148742676
                  },
                  {
                    "lat": 64.13313173896098,
                    "lng": -21.89811229705811
                  },
                  {
                    "lat": 64.13498589968151,
                    "lng": -21.9104290008545
                  },
                  {
                    "lat": 64.13691484463044,
                    "lng": -21.92334651947022
                  }
                ]
              },
              "properties": {}
            },
            "area_size": "0.5148",
            "center_parsed": {
              "lat": "64 07.907",
              "lng": "-21 54.215"
            },
            "polyline_length": "4.6140"
          },
          "id": "14aa684e-3ffd-47f9-9c41-30163815522a",
          "operation_id": "79d077ef-9eed-49d4-8001-75c36bbea675",
          "task_id": "58d7035a-c4be-446c-a8ae-86cd9a38e0a1"
        },
        "device": "true"
      },
      "due_date": null,
      "sst_task": null,
      "decimal_lat": "64.131783333",
      "decimal_lng": "-21.903583333",
      "custom_values": {},
      "id": "58d7035a-c4be-446c-a8ae-86cd9a38e0a1",
      "creator_resource_id": null,
      "creator_tenant_id": "196a0475-6cd1-4f30-b061-caf3e8649c06",
      "marker_type_id": null,
      "operation_id": "79d077ef-9eed-49d4-8001-75c36bbea675",
      "plan_id": null,
      "priority_id": "1437d403-f22b-44b5-875d-f58aa9020ad5",
      "risk_id": null,
      "round_id": "50921b2e-bfe3-4804-add9-601ade7a6c72",
      "search_area_id": "14aa684e-3ffd-47f9-9c41-30163815522a",
      "sst_event_id": null,
      "task_priority_id": null,
      "user_id": "738d3640-3fbd-4a5e-aaeb-a085625af812",
      "accepts_groups": true,
      "comments_count": 0,
      "tags": [],
      "operation_logs": []
    }
  ],
  "operation_id": null,
  "last_response_timestamp": "2019-09-12T16:23:56.128+02:00",
  "tasks_count": 126
}
```
