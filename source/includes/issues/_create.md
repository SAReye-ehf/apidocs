## Create a new issue

### HTTP request

`POST http://example.com/issues`

### Parameters

| Key                            | Type                 | Description                                          |
| ------------------------------ | -------------------- | ---------------------------------------------------- |
| issue[name]                    | String               | Short description of the issue                       |
| issue[description]             | String               | Explanation of the issue                             |
| issue[issue_type_id]           | String (uuid)        | Type of issue                                        |
| issue[solved]                  | Boolean              | Has the issue been solved or not                     |
| issue[anonymous]               | Boolean              | Post the issue anonymously                           |
| issue[unit_id]                 | String (uuid)        | The unit responsible for the issue                   |
| issue[tag_ids][]               | Array[String (uuid)] | Assigned tags                                        |
| issue[assigned_resource_ids][] | Array[String (uuid)] | Resources that are assigned to investigate the issue |
| issue[affected_resource_ids][] | Array[String (uuid)] | Resources that are affected by the issue             |
