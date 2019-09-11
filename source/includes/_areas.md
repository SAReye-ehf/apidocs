# Areas

## Get All Areas

```shell
curl "https://api.sardynamics.com/areas.json"
  -H "Authorization: abbe0983-7b75-53df-bc32-009b79d2c61e"
```

> The response to this request is a JSON object structured like this:

```json
[
  {
    "name": "01",
    "created_at": "2017-10-25T13:07:15.275Z",
    "updated_at": "2017-12-04T14:18:52.782Z",
    "disabled": false,
    "json": null,
    "description": "",
    "lat": "64 54.500",
    "lng": "-22 52.500",
    "zoom": 8,
    "has_polygon": false,
    "id": "73f9ea82-1dde-5636-a139-ee0822c26726",
    "tenant_id": "ecaf17fa-df8b-51e9-b370-9963438b1fb3"
  },
  {
    "name": "02",
    "created_at": "2017-10-25T13:07:15.283Z",
    "updated_at": "2017-12-04T14:19:08.239Z",
    "disabled": false,
    "json": null,
    "description": "",
    "lat": "65 32.000",
    "lng": "-23 04.000",
    "zoom": 8,
    "has_polygon": false,
    "id": "614ec74c-2749-541a-ab68-e8ccc3da2b26",
    "tenant_id": "ecaf17fa-df8b-51e9-b370-9963438b1fb3"
  }
]
```

This endpoint retrieves all areas.

### HTTP Request

`GET https://api.sardynamics.com/areas.json`

## Get a Specific Area

```shell
curl "https://api.sardynamics.com/areas/abbe0983-7b75-53df-bc32-009b79d2c61e.json"
  -H "Authorization: abbe0983-7b75-53df-bc32-009b79d2c61e"
```

> The response to this request is a JSON object structured like this:

```json
{
  "name": "02",
  "created_at": "2017-10-25T13:07:15.283Z",
  "updated_at": "2017-12-04T14:19:08.239Z",
  "disabled": false,
  "json": null,
  "description": "",
  "lat": "65 32.000",
  "lng": "-23 04.000",
  "zoom": 8,
  "has_polygon": false,
  "id": "614ec74c-2749-541a-ab68-e8ccc3da2b26",
  "tenant_id": "ecaf17fa-df8b-51e9-b370-9963438b1fb3"
}
```

This endpoint retrieves a specific area.

### HTTP Request

`GET http://example.com/areas.json/<ID>`

### URL Parameters

| Parameter | Description                    |
| --------- | ------------------------------ |
| ID        | The ID of the area to retrieve |

## Delete a Specific Area

```shell
curl "https://api.sardynamics.com/areas/27522917-bb28-530e-979d-c4b77a335114.json"
  -X DELETE
  -H "Authorization: abbe0983-7b75-53df-bc32-009b79d2c61e"
```

This endpoint deletes a specific area.

### HTTP Request

`DELETE http://example.com/areas/<ID>`

### URL Parameters

| Parameter | Description                  |
| --------- | ---------------------------- |
| ID        | The ID of the area to delete |
