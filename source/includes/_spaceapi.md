# SpaceAPI

The purpose of the Space API is to define a unified specification across the
hackerspaces that can be used to expose information to web apps or any other
application.

You can find more information about SpaceAPI at
[spaceapi.net](http://spaceapi.net/).


## Fetch the SpaceAPI JSON

```shell
curl "https://api.57north.org.uk/api/spaceapi"
```

> The above command returns JSON structured like this:

```json
{
    "api": "0.13",
    "contact": {
        "irc": "irc://irc.freenode.net/#57N",
        "issue_mail": "irl@sdf.org",
        "ml": "57north-discuss@lists.57north.co",
        "phone": "+441224583491",
        "twitter": "@57NorthHacklab",
        "email": "contact@57north.co"
    },
    "events": [
        {
            "extra": "Unlocked the door",
            "name": "nordin",
            "timestamp": 1421951635,
            "type": "door-unlock"
        },
        {
            "extra": "Unlocked the door",
            "name": "Derecho",
            "timestamp": 1421939544,
            "type": "door-unlock"
        },
        {
            "extra": "Unlocked the door",
            "name": "Derecho",
            "timestamp": 1421934955,
            "type": "door-unlock"
        },
        {
            "extra": "Unlocked the door",
            "name": "Derecho",
            "timestamp": 1421846364,
            "type": "door-unlock"
        },
        {
            "extra": "Unlocked the door",
            "name": "hibby",
            "timestamp": 1421621786,
            "type": "door-unlock"
        },
        {
            "extra": "Unlocked the door",
            "name": "hibby",
            "timestamp": 1421621780,
            "type": "door-unlock"
        },
        {
            "extra": "Unlocked the door",
            "name": "hibby",
            "timestamp": 1421621779,
            "type": "door-unlock"
        },
        {
            "extra": "Unlocked the door",
            "name": "hibby",
            "timestamp": 1421621779,
            "type": "door-unlock"
        },
        {
            "extra": "Unlocked the door",
            "name": "hibby",
            "timestamp": 1421621779,
            "type": "door-unlock"
        },
        {
            "extra": "Unlocked the door",
            "name": "hibby",
            "timestamp": 1421621778,
            "type": "door-unlock"
        }
    ],
    "issue_report_channels": [
        "issue_mail"
    ],
    "location": {
        "address": "35a Union Street, Aberdeen, United Kingdom",
        "lat": 57.14731,
        "lon": -2.095607
    },
    "logo": "http://bodaegl.ormiret.com/foo/57Nlogo.png",
    "space": "57North Hacklab",
    "state": {
        "icon": {
            "closed": "http://hackerdeen.org/static/closed.png",
            "open": "http://hackerdeen.org/static/open.png"
        },
        "lastchange": 1422139146,
        "message": "Space is lonely",
        "open": false,
        "trigger_person": "irl"
    },
    "url": "http://57north.co/",
    "sensors": {
        "total_member_count": [
            {
                "value": 13,
                "location": "January 2015"
            },
            {
                "value": 13,
                "location": "December 2014"
            },
            {
                "value": 17,
                "location": "November 2014"
            }
        ]
    },
    "feeds": {
        "calendar": {
            "type": "ical",
            "url": "http://opentechcalendar.co.uk/api1/group/151/events.ical"
        },
        "wiki": {
            "type": "atom",
            "url": "http://57north.co/w/index.php?title=Special:RecentChanges&feed=atom"
        }
    },
    "projects": [
        "http://57north.co/wiki/Doorbot",
        "http://57north.co/wiki/Hackerdeenbot",
        "http://57north.co/wiki/RIPE_Atlas",
        "http://57north.co/wiki/SpaceRDF"
    ]
}
```

This endpoint retrieves the SpaceAPI JSON.

### HTTP Request

`GET https://api.57north.org.uk/api/spaceapi`

### Query Parameters

Parameter | Default | Description
--------- | ------- | -----------
simple    | false   | If set to true, the returned JSON will only contain base information, contact information and the space status.

<aside class="notice">
Please use the <code>simple</code> parameter if you do not need the extra
information. This helps to reduce the bandwidth used by our server.
</aside>
<aside class="success">
This endpoint does not require authentication.
</aside>

