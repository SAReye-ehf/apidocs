## Getting a list of all Plans

### HTTP Request

`GET https://api.sardynamics.com/plans.json`

```shell
curl "https://api.sardynamics.com/plans.json"
  -H "Authorization: abbe0983-7b75-53df-bc32-009b79d2c61e"
```

> The response to this request is a JSON object structured like this:

```json
[
  {
    "name": "Forest fires in zone 1",
    "created_at": "2019-04-09T19:06:24.358Z",
    "updated_at": "2019-04-09T19:06:24.358Z",
    "id": "2418127d-e198-4b8f-8a32-108161bbbcee",
    "area_id": null,
    "plan_type_id": "4803f954-e918-43ba-8a18-e37819badf58",
    "tenant_id": "ad9bf99e-ecce-4abb-be35-eb9a3b47a2da",
    "operation_type_id": "1ffca27a-081e-45dc-a9d6-f909a8d899aa",
    "deleted": false,
    "chapters": [
      {
        "text": "",
        "title": "Location info",
        "created_at": "2019-08-05T01:16:23.808Z",
        "updated_at": "2019-08-05T01:16:23.808Z",
        "id": "a3289bf3-b509-4278-b800-1e36ce705161",
        "chapter_type_id": "f8984b18-f129-425e-ada1-07e818d0df3a",
        "plan_id": "2418127d-e198-4b8f-8a32-108161bbbcee",
        "tenant_id": null,
        "position": 2
      },
      {
        "text": "",
        "title": "Areas of operation",
        "created_at": "2019-08-05T01:16:23.816Z",
        "updated_at": "2019-08-05T01:16:23.816Z",
        "id": "5dd2b4c3-fad2-4c51-b816-f583bb99fd6e",
        "chapter_type_id": "f8984b18-f129-425e-ada1-07e818d0df3a",
        "plan_id": "2418127d-e198-4b8f-8a32-108161bbbcee",
        "tenant_id": null,
        "position": 6
      },
      {
        "text": "Laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.",
        "title": "Leader structure",
        "created_at": "2019-08-05T01:16:23.814Z",
        "updated_at": "2019-08-05T01:31:05.168Z",
        "id": "56ae04ec-b122-40bc-a617-1410fa01d22f",
        "chapter_type_id": "f8984b18-f129-425e-ada1-07e818d0df3a",
        "plan_id": "2418127d-e198-4b8f-8a32-108161bbbcee",
        "tenant_id": null,
        "position": 5
      },
      {
        "text": "Officia deserunt mollit anim id est laborum.",
        "title": "Dispatch",
        "created_at": "2019-08-05T01:16:23.812Z",
        "updated_at": "2019-08-05T01:31:05.170Z",
        "id": "d636f0f0-28bf-45de-a135-7085e275e2b9",
        "chapter_type_id": "f8984b18-f129-425e-ada1-07e818d0df3a",
        "plan_id": "2418127d-e198-4b8f-8a32-108161bbbcee",
        "tenant_id": null,
        "position": 4
      },
      {
        "text": "",
        "title": "Definitions",
        "created_at": "2019-08-05T01:16:23.810Z",
        "updated_at": "2019-08-05T01:31:05.172Z",
        "id": "73c0b27c-32ee-473d-be53-04cd11ee0ec1",
        "chapter_type_id": "f8984b18-f129-425e-ada1-07e818d0df3a",
        "plan_id": "2418127d-e198-4b8f-8a32-108161bbbcee",
        "tenant_id": null,
        "position": 3
      },
      {
        "text": "Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.",
        "title": "Communication plan",
        "created_at": "2019-08-05T01:16:23.819Z",
        "updated_at": "2019-08-05T01:34:10.145Z",
        "id": "54f3394d-e6bd-4639-b2b1-301d7d0bb1d7",
        "chapter_type_id": "f8984b18-f129-425e-ada1-07e818d0df3a",
        "plan_id": "2418127d-e198-4b8f-8a32-108161bbbcee",
        "tenant_id": null,
        "position": 9
      },
      {
        "text": "Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.",
        "title": "Foreword",
        "created_at": "2019-08-05T01:07:39.562Z",
        "updated_at": "2019-08-29T14:14:51.155Z",
        "id": "88bdb65e-eebe-4fdb-954b-82733dc050be",
        "chapter_type_id": "f8984b18-f129-425e-ada1-07e818d0df3a",
        "plan_id": "2418127d-e198-4b8f-8a32-108161bbbcee",
        "tenant_id": null,
        "position": 1
      },
      {
        "text": "Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.",
        "title": "Special chapter",
        "created_at": "2019-08-05T01:16:23.818Z",
        "updated_at": "2019-08-07T15:52:38.651Z",
        "id": "1533f6fb-9d95-40af-b56c-de64e39d66e6",
        "chapter_type_id": "f8984b18-f129-425e-ada1-07e818d0df3a",
        "plan_id": "2418127d-e198-4b8f-8a32-108161bbbcee",
        "tenant_id": null,
        "position": 7
      }
    ]
  }
]
```
