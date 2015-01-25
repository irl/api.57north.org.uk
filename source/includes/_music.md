# Space Music

Music in the space is controlled by a Raspberry Pi running MPD. You can find
more information on this system [on the
wiki](https://wiki.57north.org.uk/index.php/Projects:PiMPD). The following
API endpoints give access to information about this MPD instance.

## Fetch current track

```shell
curl "https://api.57north.org.uk/api/music/current"
```

> The above command returns JSON structured like this:

```json
{
  "album": "Best Of",
  "artist": "Various Artists",
  "track": "Track 1"
}
```

This endpoint retrieves information about the currently playing track.

### HTTP Request

`https://api.57north.org.uk/api/music/current`

### Query Parameters

Parameter | Default | Description
--------- | ------- | -----------
blame     | false   | Include a user to blame for the music.
volume    | false   | Include the current volume level.

<aside class="success">
This endpoint does not require authentication.
</aside>

