---
layout: "page"
title: API Status and Error Codes
nav_order: 6
---

# API Status and Error Codes

The Receptiviti API returns HTTP status codes as well as JSON-based error codes and messages.

| Code       | Description        |
|:-------------|:------------------|
| 200          | OK - The request was received, understood, and is being processed. |
| 201 | Created — this is a successful API call.|
| 400          |Bad request — there is something wrong or missing in the formatting of the API call.|
| 401          |Unauthorized — something is missing or inaccurate in the credentials.|
| 5xx          |Server error. (**Note**: If you see anything like this, feel free to report it to us.)|

## Response Header Example

```
access-control-allow-credentials: true
access-control-allow-origin: https://api-v3.receptiviti.com
access-control-expose-headers: Content-Type, X-Total-Count
content-length: 10257
content-type: application/hal+json
date: Thu, 12 Mar 2020 16:50:12 GMT
retry-after: 2590118
server: nginx/1.16.1
status: 200
vary: Origin, Cookie
x-ratelimit-limit: 150000000
x-ratelimit-remaining: 149999997
x-ratelimit-reset: 1586621931
```
