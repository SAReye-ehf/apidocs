## Delete a Specific Course

```shell
curl "https://api.sardynamics.com/courses/27522917-bb28-530e-979d-c4b77a335114.json"
  -X DELETE
  -H "Authorization: abbe0983-7b75-53df-bc32-009b79d2c61e"
```

This endpoint deletes a specific area.

### HTTP Request

`DELETE https://api.sardynamics.com/courses/<ID>`

### URL Parameters

| Parameter | Description                  |
| --------- | ---------------------------- |
| ID        | The ID of the area to delete |
