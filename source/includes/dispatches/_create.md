## Create a new dispatch

### HTTP request

`POST http://example.com/dispatches`

### Parameters

| Key                            | Type                 | Description                 |
| ------------------------------ | -------------------- | --------------------------- |
| dispatch[message]              | String               | Message to send             |
| dispatch[operation_id]         | String (UUID)        | Operation ID                |
| dispatch[priority_id]          | String (UUID)        | Priority ID                 |
| dispatch[dispatch_group_ids][] | Array(String (UUID)) | Array of dispatch group ids |
