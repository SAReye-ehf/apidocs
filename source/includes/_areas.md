# Areas

## Get All Areas

```ruby
require 'sareye'

api = Kittn::APIClient.authorize!('meowmeowmeow')
api.areas.get
```

```python
import sareye

api = sareye.authorize('meowmeowmeow')
api.areas.get()
```

```shell
curl "http://example.com/api/areas"
  -H "Authorization: meowmeowmeow"
```

```javascript
const sareye = require("sareye");

let api = sareye.authorize("meowmeowmeow");
let areas = api.areas.get();
```

> The above command returns JSON structured like this:

```json
[
  {
    "id": 1,
    "name": "Fluffums",
    "breed": "calico",
    "fluffiness": 6,
    "cuteness": 7
  },
  {
    "id": 2,
    "name": "Max",
    "breed": "unknown",
    "fluffiness": 5,
    "cuteness": 10
  }
]
```

This endpoint retrieves all areas.

### HTTP Request

`GET http://example.com/api/areas`

### Query Parameters

| Parameter    | Default | Description                                                                    |
| ------------ | ------- | ------------------------------------------------------------------------------ |
| include_cats | false   | If set to true, the result will also include cats.                             |
| available    | true    | If set to false, the result will include areas that have already been adopted. |

<aside class="success">
Remember — a happy area is an authenticated area!
</aside>

## Get a Specific Area

```ruby
require 'sareye'

api = Kittn::APIClient.authorize!('meowmeowmeow')
api.areas.get(2)
```

```python
import sareye

api = sareye.authorize('meowmeowmeow')
api.areas.get(2)
```

```shell
curl "http://example.com/api/areas/2"
  -H "Authorization: meowmeowmeow"
```

```javascript
const sareye = require("sareye");

let api = sareye.authorize("meowmeowmeow");
let max = api.areas.get(2);
```

> The above command returns JSON structured like this:

```json
{
  "id": 2,
  "name": "Max",
  "breed": "unknown",
  "fluffiness": 5,
  "cuteness": 10
}
```

This endpoint retrieves a specific area.

<aside class="warning">Inside HTML code blocks like this one, you can't use Markdown, so use <code>&lt;code&gt;</code> blocks to denote code.</aside>

### HTTP Request

`GET http://example.com/areas/<ID>`

### URL Parameters

| Parameter | Description                    |
| --------- | ------------------------------ |
| ID        | The ID of the area to retrieve |

## Delete a Specific Area

```ruby
require 'sareye'

api = Kittn::APIClient.authorize!('meowmeowmeow')
api.areas.delete(2)
```

```python
import sareye

api = sareye.authorize('meowmeowmeow')
api.areas.delete(2)
```

```shell
curl "http://example.com/api/areas/2"
  -X DELETE
  -H "Authorization: meowmeowmeow"
```

```javascript
const sareye = require("sareye");

let api = sareye.authorize("meowmeowmeow");
let max = api.areas.delete(2);
```

> The above command returns JSON structured like this:

```json
{
  "id": 2,
  "deleted": ":("
}
```

This endpoint deletes a specific area.

### HTTP Request

`DELETE http://example.com/areas/<ID>`

### URL Parameters

| Parameter | Description                  |
| --------- | ---------------------------- |
| ID        | The ID of the area to delete |
