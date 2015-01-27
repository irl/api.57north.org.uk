# Space Announcements

Announcements are published on the 57North [Announcements Mailing
List](http://lists.57north.co/listinfo/57north-announce).

## Fetch recent announcements

```shell
curl "https://api.57north.org.uk/api/announcements/recent"
```

> The above command returns JSON structured like this:

```json
[{
  "title": "Tuesday",
  "datetime": "Tue Jan 27 10:47:01 UTC 2015",
  "link": "http://lists.57north.co/pipermail/57north-announce/2015-January/000106.html"
},
{
  "title": "Tuesday",
  "datetime": "Tue Jan 27 10:47:05 UTC 2015",
  "link": "http://lists.57north.co/pipermail/57north-announce/2015-January/000107.html"
}]
```

This endpoint retrieves recent announcements from the announcements mailing
list archives.

### HTTP Request

`https://api.57north.org.uk/api/announcements/recent`

### Query Parameters

Parameter | Default | Description
--------- | ------- | -----------
count     | 5       | Number of recent announcements to return (Maximum: 15)

<aside class="success">
This endpoint does not require authentication.
</aside>

