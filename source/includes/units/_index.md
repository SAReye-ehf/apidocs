## Get All Units

### HTTP Request

`GET https://api.sardynamics.com/units.json`

```shell
curl "https://api.sardynamics.com/units.json"
  -H "Authorization: abbe0983-7b75-53df-bc32-009b79d2c61e"
```

> The response to this request is a JSON object structured like this:

```json
{
  "units": [
    {
      "name": "Division",
      "created_at": "2018-10-13T16:34:17.592Z",
      "updated_at": "2019-08-07T11:31:13.021Z",
      "disabled": false,
      "call_sign": "Div",
      "logo": {
        "url": null,
        "thumb": {
          "url": null
        },
        "tiny": {
          "url": null
        },
        "tiny_square": {
          "url": null
        }
      },
      "id": "f747ddfa-c6a2-444d-ba9e-f849ea7a5bea",
      "area_id": "906006ae-7c44-428f-8312-df243294bad7",
      "category_id": null,
      "resource_id": "441d7391-e14c-4701-bf65-f557dc9593b7",
      "tenant_id": "196a0475-6cd1-4f30-b061-caf3e8649c06"
    },
    {
      "name": "Emergency Headquarters",
      "created_at": "2018-10-13T16:34:17.584Z",
      "updated_at": "2019-08-07T11:31:27.584Z",
      "disabled": false,
      "call_sign": "HQ",
      "logo": {
        "url": null,
        "thumb": {
          "url": null
        },
        "tiny": {
          "url": null
        },
        "tiny_square": {
          "url": null
        }
      },
      "id": "8b8a9aa6-681f-4a98-9c8f-81d3ced87c09",
      "area_id": "99d9e1d8-7f2a-4643-8982-e64615c314f4",
      "category_id": null,
      "resource_id": "ef906f9c-c1d3-4da7-801b-9bd192438962",
      "tenant_id": "196a0475-6cd1-4f30-b061-caf3e8649c06"
    }
  ]
}
```
