# Authentication

```shell
# With the shell, you can just pass the correct header with each request
curl "https://api.57north.org.uk/api/<endpoint>"
  -H "Authorization: <apikey>"
```

> Make sure to replace `<apikey>` with your API key.

The API uses API keys to allow access to the API and expects for the API key to
be included in all API requests that require authentication in a header that
looks like the following:

`Authorization: <apikey>`

<aside class="notice">
You must replace <code>&lt;apikey&gt;</code> with your personal API key.
</aside>

