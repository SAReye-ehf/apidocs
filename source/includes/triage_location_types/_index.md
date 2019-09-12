## Get All Triage Location Types

### HTTP Request

`GET https://api.sardynamics.com/triage_location_types.json`

```shell
curl "https://api.sardynamics.com/triage_location_types.json"
  -H "Authorization: abbe0983-7b75-53df-bc32-009b79d2c61e"
```

> The response to this request is a JSON object structured like this:

```json
[
  {
    "id": "a82d55b5-44fd-40a7-a713-2ebe2c40c315",
    "shareable_triages_group_id": "9114ee94-926e-441a-85b2-f3b717321229",
    "name": "Accident Site",
    "rank": 1,
    "deleted": false,
    "created_at": "2019-01-07T17:05:08.577Z",
    "updated_at": "2019-01-07T17:05:08.577Z"
  },
  {
    "id": "9f79dece-fe6c-49f5-898c-e52ee15fd294",
    "shareable_triages_group_id": "9114ee94-926e-441a-85b2-f3b717321229",
    "name": "Treatment Area",
    "rank": 2,
    "deleted": false,
    "created_at": "2019-01-07T17:05:08.579Z",
    "updated_at": "2019-01-07T17:05:08.579Z"
  },
  {
    "id": "c4c8d083-9581-4636-be1f-49288b0bea3a",
    "shareable_triages_group_id": "9114ee94-926e-441a-85b2-f3b717321229",
    "name": "Transport",
    "rank": 3,
    "deleted": false,
    "created_at": "2019-01-07T17:05:08.585Z",
    "updated_at": "2019-01-07T17:05:08.585Z"
  },
  {
    "id": "7d22cb6f-e0f6-4166-9a05-65528a1b6bc5",
    "shareable_triages_group_id": "9114ee94-926e-441a-85b2-f3b717321229",
    "name": "Mass Aid Center",
    "rank": 4,
    "deleted": false,
    "created_at": "2019-01-07T17:05:08.587Z",
    "updated_at": "2019-01-07T17:05:08.587Z"
  },
  {
    "id": "79b3f01d-f34b-4524-b9fb-85ea3c2071fd",
    "shareable_triages_group_id": "9114ee94-926e-441a-85b2-f3b717321229",
    "name": "Hospital",
    "rank": 5,
    "deleted": false,
    "created_at": "2019-01-07T17:05:08.589Z",
    "updated_at": "2019-01-07T17:05:08.589Z"
  }
]
```
