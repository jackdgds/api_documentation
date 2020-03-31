---
layout: "page"
title: Receptiviti API Endpoints
nav_order: 12
---

# Receptiviti API Endpoints

---
```GET``` /<span style="color: blue;">ping</span>
{: .fs-6 }

Sends a ping to the Receptiviti API, validating the API Key and Secret Key, and returns a pong response if successful.

### Example Request

``` https://api-v3.receptiviti.com/v3/api/ping ```

### Example Response


 ```"pong": "Hello Your Name"```

---
```GET``` /<span style="color: blue;">content</span>
{: .fs-6 }


Makes a call to the API and analyzes text sample(s) and returns LIWC and Receptiviti scores.

### Example Request

``` https://api-v3.receptiviti.com/v3/api/content ```

### Example Response

```
{
  "submitted_text": "Hello how are you?",
  "user": {
    "email": "myemail@mystartup.com",
    "organization": "mystartup.com",
    "roles": [
      "liwc_scorers",
      "recep_scorers"
    ],
    "rate_limit": "100000/month",
    "remaining_this_month": 95670,
    "available_bundles": [
      "jokes_bundle_47",
      "swear_words_bundle_22"
    ],
    "available_packages": [
      "jokes_bundle_47_pack23",
      "jokes_bundle_47_pack24",
      "swear_words_bundle_22_pack40"
    ]
  },  
  "context": "RPA",
  "recep_subscription": [
    "openness",
    "conscientiousness",
    "extraversion",
    "agreeableness",
    "neuroticism",
    "artistic",
    "adventurous",
    "intellectual",
    "liberal",
    "imaginative",
    "emotionally_aware",
    "sociable",
    "friendly",
    "assertive",
    "active",
    "energetic",
    "cheerful"
  ],
  "matrix": "pa_english",
  "matrix_version": 43,
  "recep_codebase": "recep-shannon",
  "recep_codebase_version": "x58jg4o6hg",
  "errors": [
    {
      "error_string": "100 - ContextNotFound",
      "error_code": 100,
      "description": "100 - \"Context not found\". The context name submitted was not found. It may be misspelled. Check the list of contexts for your organization or account to find the available contexts and their correct spelling. Alternatively the context you submitted may not be owned by your account or organization.",
      "detail": "The receptiviti scoring matrix with the name \"mybogusmatrix\" was not found in the list of dictionaries for your organization \"mystartup.org\" nor your account \"myemail@mystartup.com\"."
    }
  ]
}
```

### Query String Parameters

The asterisk indicates a required field.

| Query String Parameters        | Type          | Description |
|:-------------|:------------------|:------|
| `language_content`* |String  | This is the actual content of the text sample(s) you provide to the API.  |
| `content_tags` | String | If using, list your tags here. (Default: [])  |
| `content_handle` | String   | A reference ID for the content.<br> This is stored and returned on subsequent GET calls.  |
| `language` |  String     | This specifies the language of the content. Currently, the supported languages are English, Spanish, Dutch, French, and German.|
| `content_source`* |Integer| This is the source of the material of the text sample being provided. <br>1=Personal Writing<br>2=Personal Email Correspondence<br>3=Professional Correspondence<br>4=Social Media<br>5=Commercial Writing<br>6=Professional or Scientific Writing<br>0=Other<br>(Default: 0) |
| `content_date`* |String  | This specifies the date of the content.<br> The default will be the date the call is made.<br> Format: YYYY-MM-DDT00:00:00.00000  |
| `recipient_id` |String  |If the writing sample was a conversation with another<br> person who has been created in the system, provide the recipient_ID for that person.   |

<br>
<br>
