## Getting a list of all Operations

### HTTP Request

`GET https://api.sardynamics.com/all_operations.json`

### Available Parameters

| Key              | Type    | Description                         |
| ---------------- | ------- | ----------------------------------- |
| skip             | Integer | How many operations to skip         |
| take             | String  | How many operations to fetch        |
| category_id      | String  |                                     |
| call_level_id    | String  |                                     |
| hide_finished    | Boolean |                                     |
| priority_id      |         |                                     |
| regarding_id     |         |                                     |
| scale_id         |         |                                     |
| show_hidden      | Boolean |                                     |
| get_all          | Boolean |                                     |
| operations_count | Integer |                                     |
| begin_at         | Date    | DD-MM-YYYY                          |
| end_at           | Date    | DD-MM-YYYY                          |
| bounding_box     | String  | [[68.656,-21.521],[69.066,-18.249]] |

```shell
curl "https://api.sardynamics.com/all_operations.json"
  -H "Authorization: abbe0983-7b75-53df-bc32-009b79d2c61e"
```

> The response to this request is a JSON object structured like this:

```json
{
  "operations": [
    {
      "name": "Cave collapsed - people feared trapped",
      "updated_at": "2019-08-29T07:20:36.188Z",
      "visible": true,
      "max_members": 0,
      "started_at": "2019-08-05T09:52:00.000Z",
      "number_of_coordinates": 0,
      "lat": "0 02.390",
      "lng": "32 26.805",
      "data": {
        "risks_j": [
          {
            "hazard": "Collapse hazard",
            "who_might_be_harmed": null,
            "risk_factor": 20,
            "in_place": null,
            "by_when": "2019-08-07T23:59:59.999Z",
            "new_risk_assessment": 10,
            "created_at": "2019-08-07T12:56:40.766Z",
            "updated_at": "2019-08-07T12:56:40.777Z",
            "action": "Working in caves",
            "id": "ce944b42-cc62-4eff-b05c-9e0b18c03dfb",
            "operation_id": "bebf1a2c-ecbf-4a56-9632-0a5fdf809f2d",
            "risk_template_id": null
          },
          {
            "hazard": "Loss of communications",
            "who_might_be_harmed": null,
            "risk_factor": 15,
            "in_place": null,
            "by_when": "2019-08-07T23:59:59.999Z",
            "new_risk_assessment": 5,
            "created_at": "2019-08-07T12:56:40.909Z",
            "updated_at": "2019-08-07T12:56:41.005Z",
            "action": "Communication",
            "id": "57ece3a6-ece0-4647-8190-bb364f390a6e",
            "operation_id": "bebf1a2c-ecbf-4a56-9632-0a5fdf809f2d",
            "risk_template_id": null
          },
          {
            "hazard": "Oxygen deprivation",
            "who_might_be_harmed": null,
            "risk_factor": 20,
            "in_place": null,
            "by_when": "2019-08-07T23:59:59.999Z",
            "new_risk_assessment": 5,
            "created_at": "2019-08-07T12:56:41.090Z",
            "updated_at": "2019-08-07T12:56:41.272Z",
            "action": "Working in caves",
            "id": "bcad707d-444a-4be5-b901-7d74ae3c02ca",
            "operation_id": "bebf1a2c-ecbf-4a56-9632-0a5fdf809f2d",
            "risk_template_id": null
          }
        ],
        "shared_operation_tenants_j": [],
        "priority_j": {
          "name": "P1",
          "created_at": "2018-10-13T16:34:17.517Z",
          "updated_at": "2018-10-13T16:34:17.517Z",
          "disabled": false,
          "rank": 1,
          "default": null,
          "operation_priority": true,
          "task_priority": true,
          "id": "413e41e2-c0eb-4450-a455-826b5ce0dd4f",
          "tenant_id": "196a0475-6cd1-4f30-b061-caf3e8649c06",
          "fill_in_text": null
        },
        "kind_j": {
          "name": "Search and Rescue",
          "disabled": null,
          "created_at": "2018-11-24T13:09:52.950Z",
          "updated_at": "2018-11-24T13:09:52.950Z",
          "id": "47a01245-a88a-4b60-a2cf-da60915b958d",
          "tenant_id": "196a0475-6cd1-4f30-b061-caf3e8649c06"
        },
        "area_j": {
          "name": "North",
          "created_at": "2018-11-24T13:13:14.202Z",
          "updated_at": "2019-08-05T12:11:54.243Z",
          "disabled": false,
          "json": null,
          "description": "",
          "lat": "0 02.390",
          "lng": "32 26.805",
          "zoom": 13,
          "has_polygon": false,
          "id": "09e9f28c-7b25-4b71-8ebf-febdb0d4dac0",
          "tenant_id": "196a0475-6cd1-4f30-b061-caf3e8649c06"
        }
      },
      "custom_values": {},
      "privacy": "closed",
      "id": "bebf1a2c-ecbf-4a56-9632-0a5fdf809f2d",
      "kind_id": "47a01245-a88a-4b60-a2cf-da60915b958d",
      "priority_id": "413e41e2-c0eb-4450-a455-826b5ce0dd4f",
      "tenant_id": "196a0475-6cd1-4f30-b061-caf3e8649c06",
      "area_id": "09e9f28c-7b25-4b71-8ebf-febdb0d4dac0",
      "operation_type_id": "816db5bd-a108-4e45-a3a1-48eda91e3f31",
      "has_password": false,
      "kind": {
        "name": "Search and Rescue",
        "id": "47a01245-a88a-4b60-a2cf-da60915b958d"
      },
      "priority": {
        "name": "P1",
        "id": "413e41e2-c0eb-4450-a455-826b5ce0dd4f"
      },
      "dispatches": [
        {
          "id": "297ef783-7548-41d4-bf0d-e6b0b2b6b837",
          "message": "First responders needed for wilderness rescue.",
          "operation_id": "bebf1a2c-ecbf-4a56-9632-0a5fdf809f2d",
          "tenant_id": "196a0475-6cd1-4f30-b061-caf3e8649c06",
          "priority_id": "1437d403-f22b-44b5-875d-f58aa9020ad5",
          "user_id": "94a15900-7fe4-4a44-b850-02d66f274485",
          "created_at": "2019-08-07T13:20:33.446Z",
          "updated_at": "2019-08-07T13:20:33.446Z",
          "resources_count": 1
        }
      ],
      "operation_type": {
        "id": "816db5bd-a108-4e45-a3a1-48eda91e3f31",
        "name": "Dispatch"
      },
      "area": {
        "name": "North",
        "id": "09e9f28c-7b25-4b71-8ebf-febdb0d4dac0"
      },
      "allowed_units": [],
      "shared_operation_tenants": []
    },
    {
      "name": "Earthquake response",
      "updated_at": "2019-08-05T09:48:29.787Z",
      "visible": true,
      "max_members": 1,
      "started_at": "2018-11-24T13:24:00.000Z",
      "number_of_coordinates": 1,
      "lat": "64 08.000",
      "lng": "-21 56.000",
      "data": {
        "risks_j": [],
        "shared_operation_tenants_j": [],
        "priority_j": {
          "name": "P1",
          "created_at": "2018-10-13T16:34:17.517Z",
          "updated_at": "2018-10-13T16:34:17.517Z",
          "disabled": false,
          "rank": 1,
          "default": null,
          "operation_priority": true,
          "task_priority": true,
          "id": "413e41e2-c0eb-4450-a455-826b5ce0dd4f",
          "tenant_id": "196a0475-6cd1-4f30-b061-caf3e8649c06",
          "fill_in_text": null
        },
        "operation_scale_j": {
          "name": "Black",
          "created_at": "2018-10-13T16:34:17.677Z",
          "updated_at": "2018-10-13T16:34:17.677Z",
          "disabled": false,
          "background_color": "#000000",
          "text_color": "#FFFFFF",
          "id": "0695eebf-f6a4-4f50-a32b-50e1afcc497a",
          "tenant_id": "196a0475-6cd1-4f30-b061-caf3e8649c06"
        },
        "kind_j": {
          "name": "Natural disaster",
          "disabled": null,
          "created_at": "2018-10-13T16:34:17.618Z",
          "updated_at": "2018-10-13T16:34:17.618Z",
          "id": "f5d78797-8e6e-488c-b5f1-796d9b4c530d",
          "tenant_id": "196a0475-6cd1-4f30-b061-caf3e8649c06"
        },
        "area_j": {
          "name": "South",
          "created_at": "2018-11-24T13:13:04.962Z",
          "updated_at": "2018-11-24T13:13:04.962Z",
          "disabled": false,
          "json": null,
          "description": null,
          "lat": null,
          "lng": null,
          "zoom": 10,
          "has_polygon": false,
          "id": "99d9e1d8-7f2a-4643-8982-e64615c314f4",
          "tenant_id": "196a0475-6cd1-4f30-b061-caf3e8649c06"
        }
      },
      "custom_values": {},
      "privacy": "open",
      "id": "bd241c9d-38e6-4e44-8a0a-df53b9e3bb92",
      "kind_id": "f5d78797-8e6e-488c-b5f1-796d9b4c530d",
      "operation_scale_id": "0695eebf-f6a4-4f50-a32b-50e1afcc497a",
      "priority_id": "413e41e2-c0eb-4450-a455-826b5ce0dd4f",
      "tenant_id": "196a0475-6cd1-4f30-b061-caf3e8649c06",
      "area_id": "99d9e1d8-7f2a-4643-8982-e64615c314f4",
      "operation_type_id": "816db5bd-a108-4e45-a3a1-48eda91e3f31",
      "has_password": false,
      "kind": {
        "name": "Natural disaster",
        "id": "f5d78797-8e6e-488c-b5f1-796d9b4c530d"
      },
      "priority": {
        "name": "P1",
        "id": "413e41e2-c0eb-4450-a455-826b5ce0dd4f"
      },
      "dispatches": [],
      "operation_type": {
        "id": "816db5bd-a108-4e45-a3a1-48eda91e3f31",
        "name": "Dispatch"
      },
      "operation_scale": {
        "name": "Black",
        "background_color": "#000000",
        "text_color": "#FFFFFF",
        "id": "0695eebf-f6a4-4f50-a32b-50e1afcc497a"
      },
      "area": {
        "name": "South",
        "id": "99d9e1d8-7f2a-4643-8982-e64615c314f4"
      },
      "allowed_units": [],
      "shared_operation_tenants": []
    },
    {
      "name": "Hazmat response",
      "updated_at": "2018-11-24T13:22:05.066Z",
      "visible": true,
      "max_members": 0,
      "started_at": "2018-11-24T13:06:00.000Z",
      "number_of_coordinates": 0,
      "lat": "64 08.000",
      "lng": "-21 56.000",
      "data": {
        "risks_j": [],
        "shared_operation_tenants_j": [],
        "priority_j": {
          "name": "P2",
          "created_at": "2018-10-13T16:34:17.524Z",
          "updated_at": "2018-10-13T16:34:17.524Z",
          "disabled": false,
          "rank": 2,
          "default": true,
          "operation_priority": true,
          "task_priority": true,
          "id": "1437d403-f22b-44b5-875d-f58aa9020ad5",
          "tenant_id": "196a0475-6cd1-4f30-b061-caf3e8649c06"
        },
        "operation_scale_j": {
          "name": "Red",
          "created_at": "2018-10-13T16:34:17.672Z",
          "updated_at": "2018-10-13T16:34:17.672Z",
          "disabled": false,
          "background_color": "#FF5E5B",
          "text_color": "#000000",
          "id": "891d23f3-5920-493f-b575-0e949611ef99",
          "tenant_id": "196a0475-6cd1-4f30-b061-caf3e8649c06"
        },
        "kind_j": {
          "name": "Man made disaster",
          "disabled": null,
          "created_at": "2018-11-24T13:07:37.829Z",
          "updated_at": "2018-11-24T13:07:37.829Z",
          "id": "27569411-8d96-4f83-ac46-61145e3794fd",
          "tenant_id": "196a0475-6cd1-4f30-b061-caf3e8649c06"
        },
        "area_j": {
          "name": "East",
          "created_at": "2018-11-24T13:11:59.436Z",
          "updated_at": "2018-11-24T13:11:59.436Z",
          "disabled": false,
          "json": null,
          "description": null,
          "lat": null,
          "lng": null,
          "zoom": 10,
          "has_polygon": false,
          "id": "906006ae-7c44-428f-8312-df243294bad7",
          "tenant_id": "196a0475-6cd1-4f30-b061-caf3e8649c06"
        }
      },
      "custom_values": {},
      "privacy": "open",
      "id": "b7aedf3d-9a58-48d1-b820-6f8043fcffbd",
      "kind_id": "27569411-8d96-4f83-ac46-61145e3794fd",
      "operation_scale_id": "891d23f3-5920-493f-b575-0e949611ef99",
      "priority_id": "1437d403-f22b-44b5-875d-f58aa9020ad5",
      "tenant_id": "196a0475-6cd1-4f30-b061-caf3e8649c06",
      "area_id": "906006ae-7c44-428f-8312-df243294bad7",
      "operation_type_id": "816db5bd-a108-4e45-a3a1-48eda91e3f31",
      "has_password": false,
      "kind": {
        "name": "Man made disaster",
        "id": "27569411-8d96-4f83-ac46-61145e3794fd"
      },
      "priority": {
        "name": "P2",
        "id": "1437d403-f22b-44b5-875d-f58aa9020ad5"
      },
      "dispatches": [],
      "operation_type": {
        "id": "816db5bd-a108-4e45-a3a1-48eda91e3f31",
        "name": "Dispatch"
      },
      "operation_scale": {
        "name": "Red",
        "background_color": "#FF5E5B",
        "text_color": "#000000",
        "id": "891d23f3-5920-493f-b575-0e949611ef99"
      },
      "area": {
        "name": "East",
        "id": "906006ae-7c44-428f-8312-df243294bad7"
      },
      "allowed_units": [],
      "shared_operation_tenants": []
    },
    {
      "name": "Flash flood",
      "updated_at": "2019-08-12T13:45:40.293Z",
      "visible": true,
      "max_members": 0,
      "started_at": "2018-11-24T11:27:00.000Z",
      "number_of_coordinates": 1,
      "lat": "64 08.000",
      "lng": "-21 56.000",
      "data": {
        "risks_j": [],
        "shared_operation_tenants_j": [],
        "priority_j": {
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
        "operation_scale_j": {
          "name": "Yellow",
          "created_at": "2018-10-13T16:34:17.667Z",
          "updated_at": "2018-10-13T16:34:17.667Z",
          "disabled": false,
          "background_color": "#FAFF5A",
          "text_color": "#000000",
          "id": "25a2fe8f-c9d5-4894-b258-bd2bf245cfe0",
          "tenant_id": "196a0475-6cd1-4f30-b061-caf3e8649c06"
        },
        "kind_j": {
          "name": "Natural disaster",
          "disabled": null,
          "created_at": "2018-10-13T16:34:17.618Z",
          "updated_at": "2018-10-13T16:34:17.618Z",
          "id": "f5d78797-8e6e-488c-b5f1-796d9b4c530d",
          "tenant_id": "196a0475-6cd1-4f30-b061-caf3e8649c06"
        },
        "area_j": {
          "name": "North",
          "created_at": "2018-11-24T13:13:14.202Z",
          "updated_at": "2019-08-05T12:11:54.243Z",
          "disabled": false,
          "json": null,
          "description": "",
          "lat": "0 02.390",
          "lng": "32 26.805",
          "zoom": 13,
          "has_polygon": false,
          "id": "09e9f28c-7b25-4b71-8ebf-febdb0d4dac0",
          "tenant_id": "196a0475-6cd1-4f30-b061-caf3e8649c06"
        }
      },
      "custom_values": {},
      "privacy": "open",
      "id": "109a1f1e-e067-485d-ab10-e0d361b3f216",
      "kind_id": "f5d78797-8e6e-488c-b5f1-796d9b4c530d",
      "operation_scale_id": "25a2fe8f-c9d5-4894-b258-bd2bf245cfe0",
      "priority_id": "1437d403-f22b-44b5-875d-f58aa9020ad5",
      "tenant_id": "196a0475-6cd1-4f30-b061-caf3e8649c06",
      "area_id": "09e9f28c-7b25-4b71-8ebf-febdb0d4dac0",
      "operation_type_id": "816db5bd-a108-4e45-a3a1-48eda91e3f31",
      "has_password": false,
      "kind": {
        "name": "Natural disaster",
        "id": "f5d78797-8e6e-488c-b5f1-796d9b4c530d"
      },
      "priority": {
        "name": "P2",
        "id": "1437d403-f22b-44b5-875d-f58aa9020ad5"
      },
      "dispatches": [],
      "operation_type": {
        "id": "816db5bd-a108-4e45-a3a1-48eda91e3f31",
        "name": "Dispatch"
      },
      "operation_scale": {
        "name": "Yellow",
        "background_color": "#FAFF5A",
        "text_color": "#000000",
        "id": "25a2fe8f-c9d5-4894-b258-bd2bf245cfe0"
      },
      "area": {
        "name": "North",
        "id": "09e9f28c-7b25-4b71-8ebf-febdb0d4dac0"
      },
      "allowed_units": [],
      "shared_operation_tenants": []
    },
    {
      "name": "Search for missing hiker",
      "updated_at": "2019-08-07T12:06:35.557Z",
      "visible": true,
      "max_members": 0,
      "started_at": "2018-11-12T22:26:00.000Z",
      "number_of_coordinates": -4,
      "lat": "64 08.000",
      "lng": "-21 56.000",
      "data": {
        "risks_j": [],
        "shared_operation_tenants_j": [],
        "priority_j": {
          "name": "P1",
          "created_at": "2018-10-13T16:34:17.517Z",
          "updated_at": "2018-10-13T16:34:17.517Z",
          "disabled": false,
          "rank": 1,
          "default": null,
          "operation_priority": true,
          "task_priority": true,
          "id": "413e41e2-c0eb-4450-a455-826b5ce0dd4f",
          "tenant_id": "196a0475-6cd1-4f30-b061-caf3e8649c06",
          "fill_in_text": null
        },
        "operation_scale_j": {
          "name": "Green",
          "created_at": "2018-10-13T16:34:17.658Z",
          "updated_at": "2018-10-13T16:34:17.658Z",
          "disabled": false,
          "background_color": "#62c462",
          "text_color": "#000000",
          "id": "318d00bb-c933-4ecf-9689-63cb4034809c",
          "tenant_id": "196a0475-6cd1-4f30-b061-caf3e8649c06"
        },
        "kind_j": {
          "name": "Search and Rescue",
          "disabled": null,
          "created_at": "2018-11-24T13:09:52.950Z",
          "updated_at": "2018-11-24T13:09:52.950Z",
          "id": "47a01245-a88a-4b60-a2cf-da60915b958d",
          "tenant_id": "196a0475-6cd1-4f30-b061-caf3e8649c06"
        },
        "area_j": {
          "name": "South",
          "created_at": "2018-11-24T13:13:04.962Z",
          "updated_at": "2019-08-05T12:11:57.934Z",
          "disabled": false,
          "json": null,
          "description": "",
          "lat": "0 02.390",
          "lng": "32 26.805",
          "zoom": 13,
          "has_polygon": false,
          "id": "99d9e1d8-7f2a-4643-8982-e64615c314f4",
          "tenant_id": "196a0475-6cd1-4f30-b061-caf3e8649c06"
        }
      },
      "custom_values": {},
      "privacy": "open",
      "id": "79d077ef-9eed-49d4-8001-75c36bbea675",
      "kind_id": "47a01245-a88a-4b60-a2cf-da60915b958d",
      "operation_scale_id": "318d00bb-c933-4ecf-9689-63cb4034809c",
      "priority_id": "413e41e2-c0eb-4450-a455-826b5ce0dd4f",
      "tenant_id": "196a0475-6cd1-4f30-b061-caf3e8649c06",
      "area_id": "99d9e1d8-7f2a-4643-8982-e64615c314f4",
      "operation_type_id": "816db5bd-a108-4e45-a3a1-48eda91e3f31",
      "has_password": false,
      "kind": {
        "name": "Search and Rescue",
        "id": "47a01245-a88a-4b60-a2cf-da60915b958d"
      },
      "priority": {
        "name": "P1",
        "id": "413e41e2-c0eb-4450-a455-826b5ce0dd4f"
      },
      "dispatches": [],
      "operation_type": {
        "id": "816db5bd-a108-4e45-a3a1-48eda91e3f31",
        "name": "Dispatch"
      },
      "operation_scale": {
        "name": "Green",
        "background_color": "#62c462",
        "text_color": "#000000",
        "id": "318d00bb-c933-4ecf-9689-63cb4034809c"
      },
      "area": {
        "name": "South",
        "id": "99d9e1d8-7f2a-4643-8982-e64615c314f4"
      },
      "allowed_units": [],
      "shared_operation_tenants": []
    },
    {
      "name": "Blackout in Kópasker",
      "updated_at": "2019-08-07T11:34:11.888Z",
      "visible": true,
      "max_members": 0,
      "started_at": "2018-10-24T23:58:00.000Z",
      "number_of_coordinates": 0,
      "lat": "0 02.390",
      "lng": "32 26.805",
      "data": {
        "risks_j": [],
        "shared_operation_tenants_j": [],
        "area_j": {
          "name": "East",
          "created_at": "2018-11-24T13:11:59.436Z",
          "updated_at": "2019-08-05T12:11:50.028Z",
          "disabled": false,
          "json": null,
          "description": "",
          "lat": "0 02.390",
          "lng": "32 26.805",
          "zoom": 13,
          "has_polygon": false,
          "id": "906006ae-7c44-428f-8312-df243294bad7",
          "tenant_id": "196a0475-6cd1-4f30-b061-caf3e8649c06"
        },
        "priority_j": {
          "name": "P1",
          "created_at": "2018-10-13T16:34:17.517Z",
          "updated_at": "2018-10-13T16:34:17.517Z",
          "disabled": false,
          "rank": 1,
          "default": null,
          "operation_priority": true,
          "task_priority": true,
          "id": "413e41e2-c0eb-4450-a455-826b5ce0dd4f",
          "tenant_id": "196a0475-6cd1-4f30-b061-caf3e8649c06",
          "fill_in_text": null
        },
        "operation_scale_j": {
          "name": "Yellow",
          "created_at": "2018-10-13T16:34:17.667Z",
          "updated_at": "2018-10-13T16:34:17.667Z",
          "disabled": false,
          "background_color": "#FAFF5A",
          "text_color": "#000000",
          "id": "25a2fe8f-c9d5-4894-b258-bd2bf245cfe0",
          "tenant_id": "196a0475-6cd1-4f30-b061-caf3e8649c06"
        },
        "kind_j": {
          "name": "Man made disaster",
          "disabled": null,
          "created_at": "2018-11-24T13:07:37.829Z",
          "updated_at": "2018-11-24T13:07:37.829Z",
          "id": "27569411-8d96-4f83-ac46-61145e3794fd",
          "tenant_id": "196a0475-6cd1-4f30-b061-caf3e8649c06"
        }
      },
      "custom_values": {},
      "privacy": "closed",
      "id": "d31a94bf-af6b-4447-b74e-c191304ad09b",
      "creator_resource_id": "162f2599-caed-43a8-9e51-8dac10017523",
      "kind_id": "27569411-8d96-4f83-ac46-61145e3794fd",
      "operation_scale_id": "25a2fe8f-c9d5-4894-b258-bd2bf245cfe0",
      "priority_id": "413e41e2-c0eb-4450-a455-826b5ce0dd4f",
      "tenant_id": "196a0475-6cd1-4f30-b061-caf3e8649c06",
      "area_id": "906006ae-7c44-428f-8312-df243294bad7",
      "operation_type_id": "816db5bd-a108-4e45-a3a1-48eda91e3f31",
      "has_password": false,
      "kind": {
        "name": "Man made disaster",
        "id": "27569411-8d96-4f83-ac46-61145e3794fd"
      },
      "priority": {
        "name": "P1",
        "id": "413e41e2-c0eb-4450-a455-826b5ce0dd4f"
      },
      "dispatches": [],
      "operation_type": {
        "id": "816db5bd-a108-4e45-a3a1-48eda91e3f31",
        "name": "Dispatch"
      },
      "operation_scale": {
        "name": "Yellow",
        "background_color": "#FAFF5A",
        "text_color": "#000000",
        "id": "25a2fe8f-c9d5-4894-b258-bd2bf245cfe0"
      },
      "area": {
        "name": "East",
        "id": "906006ae-7c44-428f-8312-df243294bad7"
      },
      "allowed_units": [],
      "creator_resource": {
        "identifier": "1401683949",
        "name": "John Doe",
        "created_at": "2017-10-25T13:38:39.180Z",
        "updated_at": "2019-01-22T20:55:07.312Z",
        "phone_number": "6954555",
        "on_call": null,
        "vehicle": null,
        "device_info": "{}",
        "year": null,
        "last_time_in_operation": null,
        "latest_operation_name": null,
        "device_type": null,
        "tetra": "",
        "inactive": false,
        "id": "162f2599-caed-43a8-9e51-8dac10017523",
        "email": "brandur@sareye.com",
        "phone_number_area_code": "+354",
        "call_id": null,
        "custodian_id": null,
        "latest_operation_id": null,
        "tenant_user_id": "55860fb9-06a3-4495-a096-8d17d3534827",
        "tenant_id": "44a577f8-85b4-4f9f-8ad2-3cb86b983509",
        "unit_id": "433b3ae5-351c-479b-bcfc-7cb2bd4679fc",
        "watch_id": null,
        "deleted": false,
        "inactive_unit": false
      },
      "shared_operation_tenants": []
    },
    {
      "name": "Engine Room Fire aboard Towing Vessel",
      "updated_at": "2019-08-07T12:46:39.814Z",
      "visible": true,
      "max_members": 0,
      "started_at": "2018-10-14T19:16:00.000Z",
      "number_of_coordinates": 1,
      "lat": "64 08.000",
      "lng": "-21 56.000",
      "data": {
        "device": "true",
        "risks_j": [],
        "shared_operation_tenants_j": [],
        "priority_j": {
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
        "operation_scale_j": {
          "name": "Yellow",
          "created_at": "2018-10-13T16:34:17.667Z",
          "updated_at": "2018-10-13T16:34:17.667Z",
          "disabled": false,
          "background_color": "#FAFF5A",
          "text_color": "#000000",
          "id": "25a2fe8f-c9d5-4894-b258-bd2bf245cfe0",
          "tenant_id": "196a0475-6cd1-4f30-b061-caf3e8649c06"
        },
        "kind_j": {
          "name": "Maritime incident",
          "disabled": null,
          "created_at": "2018-10-13T16:34:17.614Z",
          "updated_at": "2018-10-13T16:34:17.614Z",
          "id": "e64c3b06-5bf5-402f-9200-93c460de2039",
          "tenant_id": "196a0475-6cd1-4f30-b061-caf3e8649c06"
        },
        "area_j": {
          "name": "West",
          "created_at": "2018-11-24T13:12:04.150Z",
          "updated_at": "2019-08-05T12:12:01.165Z",
          "disabled": false,
          "json": null,
          "description": "",
          "lat": "0 02.390",
          "lng": "32 26.805",
          "zoom": 13,
          "has_polygon": false,
          "id": "ad77b9a2-77c6-43b3-a33b-4feabfcfcd7e",
          "tenant_id": "196a0475-6cd1-4f30-b061-caf3e8649c06"
        }
      },
      "custom_values": {},
      "privacy": "open",
      "id": "73222fec-c89b-45ef-9a5c-1ff64ccb0da2",
      "kind_id": "e64c3b06-5bf5-402f-9200-93c460de2039",
      "operation_scale_id": "25a2fe8f-c9d5-4894-b258-bd2bf245cfe0",
      "priority_id": "1437d403-f22b-44b5-875d-f58aa9020ad5",
      "tenant_id": "196a0475-6cd1-4f30-b061-caf3e8649c06",
      "area_id": "ad77b9a2-77c6-43b3-a33b-4feabfcfcd7e",
      "operation_type_id": "816db5bd-a108-4e45-a3a1-48eda91e3f31",
      "has_password": false,
      "kind": {
        "name": "Maritime incident",
        "id": "e64c3b06-5bf5-402f-9200-93c460de2039"
      },
      "priority": {
        "name": "P2",
        "id": "1437d403-f22b-44b5-875d-f58aa9020ad5"
      },
      "dispatches": [],
      "operation_type": {
        "id": "816db5bd-a108-4e45-a3a1-48eda91e3f31",
        "name": "Dispatch"
      },
      "operation_scale": {
        "name": "Yellow",
        "background_color": "#FAFF5A",
        "text_color": "#000000",
        "id": "25a2fe8f-c9d5-4894-b258-bd2bf245cfe0"
      },
      "area": {
        "name": "West",
        "id": "ad77b9a2-77c6-43b3-a33b-4feabfcfcd7e"
      },
      "allowed_units": [],
      "shared_operation_tenants": []
    },
    {
      "name": "Search for a missing plane",
      "updated_at": "2019-08-05T12:12:42.363Z",
      "visible": true,
      "max_members": 0,
      "started_at": "2018-10-14T19:13:00.000Z",
      "number_of_coordinates": 0,
      "lat": "0 02.405",
      "lng": "32 26.774",
      "data": {
        "device": "true",
        "risks_j": [],
        "shared_operation_tenants_j": [],
        "priority_j": {
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
        "operation_scale_j": {
          "name": "Red",
          "created_at": "2018-10-13T16:34:17.672Z",
          "updated_at": "2018-10-13T16:34:17.672Z",
          "disabled": false,
          "background_color": "#FF5E5B",
          "text_color": "#000000",
          "id": "891d23f3-5920-493f-b575-0e949611ef99",
          "tenant_id": "196a0475-6cd1-4f30-b061-caf3e8649c06"
        },
        "kind_j": {
          "name": "Aviation incident",
          "disabled": null,
          "created_at": "2018-10-13T16:34:17.604Z",
          "updated_at": "2018-10-13T16:34:17.604Z",
          "id": "a591a125-e5b9-4fd5-8179-17e52cf5ab14",
          "tenant_id": "196a0475-6cd1-4f30-b061-caf3e8649c06"
        },
        "area_j": {
          "name": "East",
          "created_at": "2018-11-24T13:11:59.436Z",
          "updated_at": "2019-08-05T12:11:50.028Z",
          "disabled": false,
          "json": null,
          "description": "",
          "lat": "0 02.390",
          "lng": "32 26.805",
          "zoom": 13,
          "has_polygon": false,
          "id": "906006ae-7c44-428f-8312-df243294bad7",
          "tenant_id": "196a0475-6cd1-4f30-b061-caf3e8649c06"
        }
      },
      "custom_values": {},
      "privacy": "open",
      "id": "aa033db4-450c-4abb-8bd3-e9b123439e2d",
      "kind_id": "a591a125-e5b9-4fd5-8179-17e52cf5ab14",
      "operation_scale_id": "891d23f3-5920-493f-b575-0e949611ef99",
      "priority_id": "1437d403-f22b-44b5-875d-f58aa9020ad5",
      "tenant_id": "196a0475-6cd1-4f30-b061-caf3e8649c06",
      "area_id": "906006ae-7c44-428f-8312-df243294bad7",
      "operation_type_id": "816db5bd-a108-4e45-a3a1-48eda91e3f31",
      "has_password": false,
      "kind": {
        "name": "Aviation incident",
        "id": "a591a125-e5b9-4fd5-8179-17e52cf5ab14"
      },
      "priority": {
        "name": "P2",
        "id": "1437d403-f22b-44b5-875d-f58aa9020ad5"
      },
      "dispatches": [],
      "operation_type": {
        "id": "816db5bd-a108-4e45-a3a1-48eda91e3f31",
        "name": "Dispatch"
      },
      "operation_scale": {
        "name": "Red",
        "background_color": "#FF5E5B",
        "text_color": "#000000",
        "id": "891d23f3-5920-493f-b575-0e949611ef99"
      },
      "area": {
        "name": "East",
        "id": "906006ae-7c44-428f-8312-df243294bad7"
      },
      "allowed_units": [],
      "shared_operation_tenants": []
    },
    {
      "name": "Forest fire",
      "updated_at": "2019-08-07T12:47:52.317Z",
      "visible": true,
      "max_members": 0,
      "started_at": "2018-10-13T16:37:00.000Z",
      "number_of_coordinates": 2,
      "lat": "64 08.000",
      "lng": "-21 56.000",
      "data": {
        "risks_j": [],
        "shared_operation_tenants_j": [],
        "priority_j": {
          "name": "P1",
          "created_at": "2018-10-13T16:34:17.517Z",
          "updated_at": "2018-10-13T16:34:17.517Z",
          "disabled": false,
          "rank": 1,
          "default": null,
          "operation_priority": true,
          "task_priority": true,
          "id": "413e41e2-c0eb-4450-a455-826b5ce0dd4f",
          "tenant_id": "196a0475-6cd1-4f30-b061-caf3e8649c06",
          "fill_in_text": null
        },
        "operation_scale_j": {
          "name": "Green",
          "created_at": "2018-10-13T16:34:17.658Z",
          "updated_at": "2018-10-13T16:34:17.658Z",
          "disabled": false,
          "background_color": "#62c462",
          "text_color": "#000000",
          "id": "318d00bb-c933-4ecf-9689-63cb4034809c",
          "tenant_id": "196a0475-6cd1-4f30-b061-caf3e8649c06"
        },
        "kind_j": {
          "name": "Natural disaster",
          "disabled": null,
          "created_at": "2018-10-13T16:34:17.618Z",
          "updated_at": "2018-10-13T16:34:17.618Z",
          "id": "f5d78797-8e6e-488c-b5f1-796d9b4c530d",
          "tenant_id": "196a0475-6cd1-4f30-b061-caf3e8649c06"
        },
        "area_j": {
          "name": "North",
          "created_at": "2018-11-24T13:13:14.202Z",
          "updated_at": "2019-08-05T12:11:54.243Z",
          "disabled": false,
          "json": null,
          "description": "",
          "lat": "0 02.390",
          "lng": "32 26.805",
          "zoom": 13,
          "has_polygon": false,
          "id": "09e9f28c-7b25-4b71-8ebf-febdb0d4dac0",
          "tenant_id": "196a0475-6cd1-4f30-b061-caf3e8649c06"
        }
      },
      "custom_values": {},
      "privacy": "open",
      "id": "2ef1be22-5855-4b2a-8434-c3ccae5513d0",
      "kind_id": "f5d78797-8e6e-488c-b5f1-796d9b4c530d",
      "operation_scale_id": "318d00bb-c933-4ecf-9689-63cb4034809c",
      "priority_id": "413e41e2-c0eb-4450-a455-826b5ce0dd4f",
      "tenant_id": "196a0475-6cd1-4f30-b061-caf3e8649c06",
      "area_id": "09e9f28c-7b25-4b71-8ebf-febdb0d4dac0",
      "operation_type_id": "816db5bd-a108-4e45-a3a1-48eda91e3f31",
      "has_password": false,
      "kind": {
        "name": "Natural disaster",
        "id": "f5d78797-8e6e-488c-b5f1-796d9b4c530d"
      },
      "priority": {
        "name": "P1",
        "id": "413e41e2-c0eb-4450-a455-826b5ce0dd4f"
      },
      "dispatches": [],
      "operation_type": {
        "id": "816db5bd-a108-4e45-a3a1-48eda91e3f31",
        "name": "Dispatch"
      },
      "operation_scale": {
        "name": "Green",
        "background_color": "#62c462",
        "text_color": "#000000",
        "id": "318d00bb-c933-4ecf-9689-63cb4034809c"
      },
      "area": {
        "name": "North",
        "id": "09e9f28c-7b25-4b71-8ebf-febdb0d4dac0"
      },
      "allowed_units": [],
      "shared_operation_tenants": []
    }
  ],
  "ops_count": 9,
  "admin": true,
  "manager": true,
  "tenant": {
    "name": "Demo",
    "created_at": "2018-10-13T16:34:17.488Z",
    "updated_at": "2019-08-07T13:48:34.485Z",
    "domain": "",
    "subdomain": "demo",
    "tenant_logo": {
      "url": null
    },
    "theme_color": "#ff9300",
    "header_title": "SAReye IMS",
    "no_access_title": "Looks like you don't have access to this page",
    "no_access_body": "Contact your system administrator",
    "open_operations": false,
    "bitly": {
      "bitly_api_key": "",
      "bitly_username": ""
    },
    "abbreviation": "SAReye",
    "nexmo_key": "",
    "nexmo_secret": "",
    "survey_request_body": null,
    "send_monthly_reports": null,
    "default_phone_number_area_code": "+354",
    "id": "196a0475-6cd1-4f30-b061-caf3e8649c06",
    "default_language_id": "9d626e73-1249-44be-9733-3583683d1ff6",
    "tenant_type_id": "ec3d40bb-f7a9-4a7a-a7a3-e4765d32fc3a",
    "shareable_triages_group_id": "9114ee94-926e-441a-85b2-f3b717321229",
    "settings": {
      "allow_signup": "1",
      "enabled_operation_attributes": [
        "{\"i18n_name\"=>\"operation.setup.op_speed\", \"id\"=>\"priority_id\"}",
        "{\"i18n_name\"=>\"operation.setup.op_call\", \"id\"=>\"kind_id\"}",
        "{\"i18n_name\"=>\"operation.setup.area\", \"id\"=>\"area_id\"}",
        "{\"i18n_name\"=>\"operation.setup.scope\", \"id\"=>\"operation_scale_id\"}",
        "{\"i18n_name\"=>\"operation.basic_info.basic_info\", \"id\"=>\"info\"}",
        "{\"i18n_name\"=>\"operation.basic_info.private_info\", \"id\"=>\"privatetext\"}"
      ]
    },
    "tenant_type": {
      "name": "SAR",
      "short_name": "sar",
      "description": null,
      "created_at": "2017-10-25T13:07:14.776Z",
      "updated_at": "2017-10-25T13:07:14.776Z",
      "id": "ec3d40bb-f7a9-4a7a-a7a3-e4765d32fc3a"
    },
    "custom_fields": []
  }
}
```
