---
title: Official API Documentation
category: HypeProxy.io v3.0
pageTitle: CacheAdvance - Never miss the cache again.
description: Cache every single thing your app could ever do ahead of time, so your code never even has to run at all.
---

Understand the basics of the Official HypeProxy.io API. {% .lead %}

## Introduction

We're proud to announce the release of our new API v3 – that brings many changes, better stability and security, the [V1 API]() is still working if you need.

Our API follows the REST specifications and use JWT authentication.

```bash
curl https://api.hypeproxy.io/v3
```

## Authentication

Our API respects the JWT authentication standards by using the `Authorization` field in HTTP headers but for convenience, the API key can also be passed through cookies and query parameter `?apikey=`.

{% see-also title="API Authentication" href="/docs/authentication" /%}

## Health check

We provide a health-check endpoint if you want to know the status of the API.

```bash
curl https://api.hypeproxy.io/health
```

You can also visit our [service status](http://status.hypeproxy.io/) page.