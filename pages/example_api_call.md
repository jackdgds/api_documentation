---
layout: "page"
title: Example API Call
nav_order: 5
parent: Making a Call to the Receptiviti API
---

# Example API Call

```
curl -X POST "https://api-v3.receptiviti.com/v3/api/content" -H "accept: application/json"
-H "X-API-SECRET-KEY: Enter your API Secret Key here" -H "X-API-KEY: Enter your API Key here"
-H "Content-Type: application/json" -d "{ \"content_tags\": [ \"string\" ], \"content_handle\":
\"string\", \"language\": \"English\", \"content_source\": 0, \"content_date\": \"2020-01-01\",
\"recipient_id\": \"string\", \"language_content\":
\"Enter your language sample here\"}
```
