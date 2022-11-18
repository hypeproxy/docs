---
title: API Authentication
category: HypeProxy.io v3.0
pageTitle: CacheAdvance - Never miss the cache again.
description: Cache every single thing your app could ever do ahead of time, so your code never even has to run at all.
---

How do you authenticate to our API? {% .lead %}

## How it works?

API requests made to HypeProxy.io API are authorized using a Bearer Authentication standard, we also support cookie and query parameter authentication.

1. [Using a cookie as authentication]()
2. [Using a query parameter as authentication]()

## Get an API Token

To retrieve your token you can either use the 'sign-in' endpoint of the API, go to your dashboard or simply use this one:

{% api-token /%}

## Authorizing requests

API requests made to Better Uptime API are authorized using a Bearer Authentication standard.

That means you'll only need to add a header with `Authorization: Bearer YOUR_API_TOKEN` to your requests.

```bash
curl -X 'POST' \
    'https://api.hypeproxy.io/v3/authentication/sign-in' \
    -H 'accept: application/json' \
    -H 'Content-Type: application/json' \
    -d '{
    "email": "user@example.com",
    "password": "MY_P4SSW0RD"
}'
```