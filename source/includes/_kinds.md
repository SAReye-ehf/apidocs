# Kinds

## Get All Kinds

### HTTP Request

`GET https://api.sardynamics.com/kinds.json`

```shell
curl "https://api.sardynamics.com/kinds.json"
  -H "Authorization: abbe0983-7b75-53df-bc32-009b79d2c61e"
```

> The response to this request is a JSON object structured like this:

```json
[
  {
    "name": "Aviation incident",
    "disabled": null,
    "created_at": "2018-10-13T16:34:17.604Z",
    "updated_at": "2018-10-13T16:34:17.604Z",
    "id": "a591a125-e5b9-4fd5-8179-17e52cf5ab14",
    "tenant_id": "196a0475-6cd1-4f30-b061-caf3e8649c06"
  },
  {
    "name": "Car accident",
    "disabled": null,
    "created_at": "2018-10-13T16:34:17.642Z",
    "updated_at": "2018-10-13T16:34:17.642Z",
    "id": "5cda40f4-b136-42a9-9eb7-3276717fe859",
    "tenant_id": "196a0475-6cd1-4f30-b061-caf3e8649c06"
  },
  {
    "name": "Disease",
    "disabled": null,
    "created_at": "2018-10-13T16:34:17.648Z",
    "updated_at": "2018-10-13T16:34:17.648Z",
    "id": "cc4584b2-caab-45a3-995d-b7aae378c7d1",
    "tenant_id": "196a0475-6cd1-4f30-b061-caf3e8649c06"
  },
  {
    "name": "Emergency assistance abroad",
    "disabled": null,
    "created_at": "2018-10-13T16:34:17.637Z",
    "updated_at": "2018-10-13T16:34:17.637Z",
    "id": "b66593ea-0d33-4cc8-80c3-0ae595d1b972",
    "tenant_id": "196a0475-6cd1-4f30-b061-caf3e8649c06"
  }
]
```
