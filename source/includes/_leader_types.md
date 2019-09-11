# Leader Types

## Get All Leader Types

### HTTP Request

`GET https://api.sardynamics.com/leader_types.json`

```shell
curl "https://api.sardynamics.com/leader_types.json"
  -H "Authorization: abbe0983-7b75-53df-bc32-009b79d2c61e"
```

> The response to this request is a JSON object structured like this:

```json
  {
    "name": "Finance",
    "deleted": false,
    "created_at": "2018-10-13T16:34:17.711Z",
    "updated_at": "2018-11-24T09:41:47.570Z",
    "id": "0deb1019-6788-4e9d-8628-c5902a2fbb06",
    "tenant_id": "196a0475-6cd1-4f30-b061-caf3e8649c06",
    "manager_id": "0c291cc6-46c3-47b1-bce7-0321948bf116"
  },
  {
    "name": "Incident Manager",
    "deleted": false,
    "created_at": "2018-10-13T16:34:17.694Z",
    "updated_at": "2018-11-24T09:40:52.008Z",
    "id": "0c291cc6-46c3-47b1-bce7-0321948bf116",
    "tenant_id": "196a0475-6cd1-4f30-b061-caf3e8649c06",
    "manager_id": null
  },
  {
    "name": "Media",
    "deleted": null,
    "created_at": "2018-10-13T16:34:17.721Z",
    "updated_at": "2018-10-13T16:34:17.721Z",
    "id": "a3f8ebb5-ba8e-4160-8073-5668da744ed5",
    "tenant_id": "196a0475-6cd1-4f30-b061-caf3e8649c06",
    "manager_id": null
  },
  {
    "name": "Operations",
    "deleted": false,
    "created_at": "2018-10-13T16:34:17.706Z",
    "updated_at": "2018-11-24T09:41:14.325Z",
    "id": "85779f44-aa2c-4235-ac55-64e01ce49f50",
    "tenant_id": "196a0475-6cd1-4f30-b061-caf3e8649c06",
    "manager_id": "0c291cc6-46c3-47b1-bce7-0321948bf116"
  },
  {
    "name": "Planning",
    "deleted": false,
    "created_at": "2018-10-13T16:34:17.702Z",
    "updated_at": "2018-11-24T09:41:28.429Z",
    "id": "97abc723-78a0-46ac-93ac-08fa57c22f8d",
    "tenant_id": "196a0475-6cd1-4f30-b061-caf3e8649c06",
    "manager_id": "0c291cc6-46c3-47b1-bce7-0321948bf116"
  },
  {
    "name": "Resources",
    "deleted": false,
    "created_at": "2018-11-24T09:42:11.882Z",
    "updated_at": "2018-11-24T09:42:11.882Z",
    "id": "2ee2bd0a-285b-497f-9615-efd3dda5cb55",
    "tenant_id": "196a0475-6cd1-4f30-b061-caf3e8649c06",
    "manager_id": "0c291cc6-46c3-47b1-bce7-0321948bf116"
  },
  {
    "name": "Safety",
    "deleted": null,
    "created_at": "2018-10-13T16:34:17.716Z",
    "updated_at": "2018-10-13T16:34:17.716Z",
    "id": "77e30bed-0188-4b37-b70f-fd6050b8306f",
    "tenant_id": "196a0475-6cd1-4f30-b061-caf3e8649c06",
    "manager_id": null
  }
]
```
