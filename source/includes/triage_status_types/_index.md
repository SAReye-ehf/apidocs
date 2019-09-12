## Get All Triage Status Types

### HTTP Request

`GET https://api.sardynamics.com/triage_status_types.json`

```shell
curl "https://api.sardynamics.com/triage_status_types.json"
  -H "Authorization: abbe0983-7b75-53df-bc32-009b79d2c61e"
```

> The response to this request is a JSON object structured like this:

```json
[
  {
    "id": "9623c4d4-71c9-4eda-9daa-5a74b706bb29",
    "shareable_triages_group_id": "9114ee94-926e-441a-85b2-f3b717321229",
    "name": "Red",
    "color": "#ff2600",
    "rank": 1,
    "deleted": false,
    "created_at": "2019-01-07T17:05:08.568Z",
    "updated_at": "2019-01-07T17:05:08.568Z"
  },
  {
    "id": "7ae14d1c-cc00-4c9b-b8f1-cc802afd8863",
    "shareable_triages_group_id": "9114ee94-926e-441a-85b2-f3b717321229",
    "name": "Yellow",
    "color": "#fffb00",
    "rank": 2,
    "deleted": false,
    "created_at": "2019-01-07T17:05:08.571Z",
    "updated_at": "2019-01-07T17:05:08.571Z"
  },
  {
    "id": "8e5d58b8-6568-466e-92cb-f6f1ae605ae5",
    "shareable_triages_group_id": "9114ee94-926e-441a-85b2-f3b717321229",
    "name": "Green",
    "color": "#5cb85c",
    "rank": 3,
    "deleted": false,
    "created_at": "2019-01-07T17:05:08.573Z",
    "updated_at": "2019-01-07T17:05:08.573Z"
  },
  {
    "id": "9a0bd94f-b47b-4704-98cd-470500f17ceb",
    "shareable_triages_group_id": "9114ee94-926e-441a-85b2-f3b717321229",
    "name": "Black",
    "color": "#000000",
    "rank": 4,
    "deleted": false,
    "created_at": "2019-01-07T17:05:08.575Z",
    "updated_at": "2019-01-07T17:05:08.575Z"
  }
]
```
