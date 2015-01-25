# Space Status

## Fetch current status

```shell
curl "https://api.57north.org.uk/api/status/current"
```

> The above command returns JSON structured like this:

```json
{
  "open": true,
  "message": "Hacking in progress",
  "last_change": "1422139146",
  "trigger_person": "irl"
}
```

This endpoint retrieves the current space status.

### HTTP Request

`https://api.57north.org.uk/api/status/current`

<aside class="success">
This endpoint does not require authentication.
</aside>

## Fetch recent statuses

```shell
curl "https://api.57north.org.uk/api/status/recent"
```

> The above command returns JSON structured like this:

```json
[{
  "open": false,
  "message": "Hacking not in progress",
  "last_change": "1422139146",
  "trigger_person": "irl"
},
{
  "open": true,
  "message": "Hacking in progress",
  "last_change": "1422138146",
  "trigger_person": "irl"
},
{
  "open": false,
  "message": "Hacking not in progress",
  "last_change": "1422137146",
  "trigger_person": "irl"
},
{
  "open": true,
  "message": "Hacking in progress",
  "last_change": "1422136146",
  "trigger_person": "irl"
},
{
  "open": false,
  "message": "Hacking not in progress",
  "last_change": "1422135146",
  "trigger_person": "irl"
}]
```

This endpoint retrieves a number of recent statuses. By default it will
retrieve the latest 5 statuses.

### HTTP Request

`https://api.57north.org.uk/api/status/recent`

### Query Parameters

Parameter | Default | Description
--------- | ------- | -----------
count     | 5       | The number of statuses to return. (Maximum allowed: 20)
type      | both    | The type of statuses to return. Allowed values are: `open`, `closed` and `both`.

<aside class="success">
This endpoint does not require authentication.
</aside>

