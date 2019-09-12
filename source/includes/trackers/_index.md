## Get All Trackers

### HTTP Request

`GET https://api.sardynamics.com/trackers.json`

```shell
curl "https://api.sardynamics.com/trackers.json"
  -H "Authorization: abbe0983-7b75-53df-bc32-009b79d2c61e"
```

> The response to this request is a JSON object structured like this:

```json
[
  {
    "location": {
      "speed": "-1",
      "heading": "-1",
      "accuracy": "65",
      "altitude": "3.4865448474884033",
      "latitude": "55.67768226454645",
      "longitude": "12.569639968728195",
      "timestamp": "1566571691612.3691",
      "altitudeAccuracy": "10"
    },
    "created_at": "2019-08-23T14:48:22.138Z",
    "updated_at": "2019-08-23T14:48:22.138Z",
    "tenant_id": "44a577f8-85b4-4f9f-8ad2-3cb86b983509",
    "user_id": "8f43a355-17cc-5c69-a60c-69d8ef0b5fa5",
    "id": "b251aa59-b948-41a0-9f89-d46aba4aa872"
  }
]
```
