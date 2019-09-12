## Delete a Specific Issue

```shell
curl "https://api.sardynamics.com/issues/27522917-bb28-530e-979d-c4b77a335114"
  -X DELETE
  -H "Authorization: abbe0983-7b75-53df-bc32-009b79d2c61e"
```

This endpoint deletes a specific issue.

### HTTP Request

`DELETE http://example.com/issues/<ID>`

### URL Parameters

| Parameter | Description                   |
| --------- | ----------------------------- |
| ID        | The ID of the issue to delete |
