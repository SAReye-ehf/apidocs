## Get All Dispatch Responses

### HTTP Request

`GET https://api.sardynamics.com/dispatch_responses.json`

```shell
curl "https://api.sardynamics.com/dispatch_responses.json"
  -H "Authorization: abbe0983-7b75-53df-bc32-009b79d2c61e"
```

> The response to this request is a JSON object structured like this:

```json
{
  "dispatch_responses": [
    {
      "id": "f861e944-da5c-5b80-9ce6-9d90d1b4a135",
      "resource_id": "3b5e1861-8e33-59d7-95fe-fc677b399db7",
      "tenant_id": "196a0475-6cd1-4f30-b061-caf3e8649c06",
      "dispatch_group_id": null,
      "operation_id": null,
      "dispatch_response_type_id": "91b4705d-c15a-46d0-bac5-66236ad58727",
      "time": "2019-09-11T15:32:00.000Z",
      "created_at": "2019-09-11T15:32:28.840Z",
      "updated_at": "2019-09-11T15:32:28.840Z",
      "resource": {
        "name": "John Smith",
        "unit_id": "39771f3d-eacc-534f-a50f-85cb1b76da56",
        "unit": {
          "name": "Command Center"
        }
      }
    }
  ],
  "dispatch_response_types": [
    {
      "id": "47a9aa18-f574-4a78-901c-20e3bb28975b",
      "name": "Can attend",
      "tenant_id": "196a0475-6cd1-4f30-b061-caf3e8649c06",
      "deleted": false,
      "require_time": true,
      "created_at": "2018-11-24T09:39:40.612Z",
      "updated_at": "2018-11-24T09:39:40.612Z"
    },
    {
      "id": "54957e36-84dc-48f0-be07-7082f4f7a7aa",
      "name": "Can not attend",
      "tenant_id": "196a0475-6cd1-4f30-b061-caf3e8649c06",
      "deleted": false,
      "require_time": false,
      "created_at": "2018-11-24T09:40:00.546Z",
      "updated_at": "2018-11-24T09:40:00.546Z"
    },
    {
      "id": "91b4705d-c15a-46d0-bac5-66236ad58727",
      "name": "Will attend",
      "tenant_id": "196a0475-6cd1-4f30-b061-caf3e8649c06",
      "deleted": false,
      "require_time": true,
      "created_at": "2018-11-24T09:39:18.026Z",
      "updated_at": "2018-11-24T09:39:18.026Z"
    }
  ]
}
```
