## Get All Operation Scales

### HTTP Request

`GET https://api.sardynamics.com/operation_scales.json`

```shell
curl "https://api.sardynamics.com/operation_scales.json?page=1"
  -H "Authorization: abbe0983-7b75-53df-bc32-009b79d2c61e"
```

> The response to this request is a JSON object structured like this:

```json
[
  {
    "name": "Black",
    "created_at": "2018-10-13T16:34:17.677Z",
    "updated_at": "2018-10-13T16:34:17.677Z",
    "disabled": false,
    "background_color": "#000000",
    "text_color": "#FFFFFF",
    "id": "0695eebf-f6a4-4f50-a32b-50e1afcc497a",
    "tenant_id": "196a0475-6cd1-4f30-b061-caf3e8649c06"
  },
  {
    "name": "Green",
    "created_at": "2018-10-13T16:34:17.658Z",
    "updated_at": "2018-10-13T16:34:17.658Z",
    "disabled": false,
    "background_color": "#62c462",
    "text_color": "#000000",
    "id": "318d00bb-c933-4ecf-9689-63cb4034809c",
    "tenant_id": "196a0475-6cd1-4f30-b061-caf3e8649c06"
  },
  {
    "name": "Red",
    "created_at": "2018-10-13T16:34:17.672Z",
    "updated_at": "2018-10-13T16:34:17.672Z",
    "disabled": false,
    "background_color": "#FF5E5B",
    "text_color": "#000000",
    "id": "891d23f3-5920-493f-b575-0e949611ef99",
    "tenant_id": "196a0475-6cd1-4f30-b061-caf3e8649c06"
  },
  {
    "name": "Yellow",
    "created_at": "2018-10-13T16:34:17.667Z",
    "updated_at": "2018-10-13T16:34:17.667Z",
    "disabled": false,
    "background_color": "#FAFF5A",
    "text_color": "#000000",
    "id": "25a2fe8f-c9d5-4894-b258-bd2bf245cfe0",
    "tenant_id": "196a0475-6cd1-4f30-b061-caf3e8649c06"
  }
]
```
