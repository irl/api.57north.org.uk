# Errors

The API uses the following error codes:

Error Code | Meaning
---------- | -------
400        | Bad Request -- Your request sucks
401        | Unauthorized -- Your API key is wrong
403        | Forbidden -- Your API key does not have permissions to perform the requested action
404        | Not Found -- You requested something that doesn't exist
405        | Method Not Allowed -- Your request used a method that is invalid
406        | Not Acceptable -- You requested a format not supported by the endpoint
410        | Gone -- You requested a resource that is no longer available
418        | I'm a Teapot -- I'm a teapot
429        | Too Many Requests -- Slown down!
500        | Internal Server Error -- There is a problem with the server. Try again later.
503        | Service Unavailable -- The server is temporarially offline. Try again later.

