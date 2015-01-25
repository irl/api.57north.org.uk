# Space Infoscreen

## Fetch Screenshot

```shell
curl "https://api.57north.org.uk/api/infoscreen/screenshot"
```

> The above command returns a PNG image showing the current view of the
> infoscreen.

This endpoint retrieves a screenshot from the infoscreen. If the infoscreen is
currently unavailable, an old screenshot will be retrieved instead.

### HTTP Request

`https://api.57north.org.uk/api/infoscreen/screenshot`

<aside class="warning">
This is not a bandwidth friendly endpoint. Please do not call it more than
necessary, and use caching as appropriate. If you're calling this more than
once an hour on average, you're calling this too often.
</aside>

