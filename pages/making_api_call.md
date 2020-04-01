---
layout: page
title:  "Making a Call to the Receptiviti API"
nav_order: 5
has_children: true
has_toc: false

# This section is to be updated when Swagger to HTML interactivity is implemented and can be placed (if using) at the bottom before the final note.

### Using Python to call the API

#The following is a basic code sample in Python to help you get started with the Receptiviti API: _(This section is to be updated when Swagger to HTML interactivity is implemented)_

#```
#import requests

#def get_liwc_scores(text, api_secret_key, api_key):
#    text = text.encode('ascii', 'ignore').decode('utf-8')
#    text_repl = text.replace('"', r'\"')
#    url = 'https://api-v3.receptiviti.com/v3/api/content'
#    headers = {'accept': 'application/json', 'X-API-SECRET-KEY': api_secret_key, 'X-API-# # KEY': api_key, 'Content-Type': 'application/json'}
#    data = "{ \"content_tags\": [ \"string\" ], \"content_handle\": \"string\", #\"language\": \"pa_english\", \"content_source\": 0, \"content_date\": \"2020-01-01\", #\"recipient_id\": \"string\", \"language_content\": \"" + text_repl + "\"}"
#    r = requests.post(url, data=data, headers=headers)
#    return r

#    text = “paste your text sample here”
#    api_secret_key = “paste your api secret key here”
#    api_key = “paste your api key here”
#    r = get_liwc_scores(text, api_secret_key, api_key)
#    r
#```
---

# Making a Call to the Receptiviti API
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

The model below indicates the parameters that are passed on the API call. The asterisk indicates required fields. Note that we recommend at least 300 words per text sample to most accurately reflect the extent of a psychological state at the time of a sample’s creation.

| Parameters        | Type          | Description |
|:-------------|:------------------|:------|
| `language_content`* |String  | This is the actual content of the text sample(s) you provide to the API.  |
| `content_tags` | String | If using, list your tags here. (Default: [])  |
| `content_handle` | String   | A reference ID for the content.<br> This is stored and returned on subsequent GET calls.  |
| `language` |  String     | This specifies the language of the content. Currently, the supported languages are English, Spanish, Dutch, French, and German.|
| `content_source`* |Integer| This is the source of the material of the text sample being provided. <br>1=Personal Writing<br>2=Personal Email Correspondence<br>3=Professional Correspondence<br>4=Social Media<br>5=Commercial Writing<br>6=Professional or Scientific Writing<br>0=Other<br>(Default: 0) |
| `content_date`* |String  | This specifies the date of the content.<br> The default will be the date the call is made.<br> Format: YYYY-MM-DDT00:00:00.00000  |
| `recipient_id` |String  |If the writing sample was a conversation with another<br> person who has been created in the system, provide the recipient_ID for that person.    |

<br>
<br>
### Making a call to the API using cURL

1. Copy the cURL example code below.
```
curl -X POST "https://api-v3.receptiviti.com/v3/api/content" -H "accept: application/json"
-H "X-API-SECRET-KEY: Enter your API Secret Key here" -H "X-API-KEY: Enter your API Key here"
-H "Content-Type: application/json" -d "{ \"content_tags\": [ \"string\" ], \"content_handle\":
\"string\", \"language\": \"English\", \"content_source\": 0, \"content_date\": \"2020-01-01\",
\"recipient_id\": \"string\", \"language_content\":
\"Enter your language sample here\"}
```

2. Paste the cURL call into your text editor of choice. (Sublime Text, Atom, etc.).
3. Copy your API Key and API Secret Key and paste them into the sections of the cURL code fields and paste to replace where it says _Enter your API Secret Key here_ and _Enter your API Key here_.
4. Copy your language sample and paste to replace where it says _Enter your language sample here_.
5. Copy the code and paste it to your command line terminal.
6. Press **return**.

NOTE: _To read the results more clearly you can paste your response into an online tool such as <https://pretty-print-json.js.org>_.
{: .label .label-yellow }

<br>
<br>
### Making a call to the API using the Receptiviti Open API/Swagger page

1. Go to <http://api-v3.receptiviti.com/auth/login> and log in using your credentials.
2. Click **Explore API**. This opens the Receptiviti Open API/Swagger page.

    ![image-title-here](https://lh5.googleusercontent.com/tqyw1ztPs1geaVZoq1vYua7zDiT__6pp1jWVRUEeI7CQAwm7fCVXXXku33emOoce3XHsVQu4niwX9TiIxWJxm8zoxUlp3vbc-p3387odndSoQATn42hSsnKpSjI09w){:class="img-responsive"}

3. Click **Post**, then click **Try it out**.

    ![image-title-here](https://lh6.googleusercontent.com/CUggMD4PB4eDdUpu6wbugs2Ijt6mP3XV97n8BFIqhZ-cqJYnLizDoBt0yBSODafR93kljyJsikYmlAGIHl4Wlj5WGX9ve8AZWiTGJxBz-37X6ICT0TcLgJxuCyGw1g){:class="img-responsive"}
4. In the **Edit Value | Model** box, replace “string” with your values and text sample.
```
{
  "language_content": "",
  "content_handle": "string",
  "content_date": "string",
  "content_source": 0,
  "recipient_id": "string",
  "content_tags": [
    "string"
  ],
  "language": "string"
}
```
The only mandatory fields are `language`, `content_date`, and `language_content`. The date format is YYYY-MM-DD.

5. Below the **Edit Value / Model** box, paste your API Key and API Secret Key in their respective fields.
6. Click **Execute**.
<br>
<br>

### Making a call to the API using the web interface

1. Go to <http://api-v3.receptiviti.com/auth/login> and log in using your credentials.
2. On the **Analyze Content** page, paste your text sample in the **Paste Text Here** box.  
3. From the **Content Source** drop-down menu, select the applicable source of your text sample.
4. Click **Analyze**.

    ![image-title-here](https://lh5.googleusercontent.com/0msDZjyou6pXfEIazyrtBxKwjfN0kUEH6iByfEEe4iQ9cAeCaZeNXmeWkwQLFV6YfXUcqkiXQtFFM02_XX0x1nj9Y7YOZuzvv7iK0scKxWvZAhZn_sU5dy57b2BJrQ){:class="img-responsive"}


NOTE:_This page is intended for ad-hoc analysis. ~~Any data entered and results generated on this page are not stored, and are not retrievable once you leave this page.~~_
{: .label .label-yellow }

You will see below the pasted text sample a section that contains the API response formatted in a series of boxes, including:
* **Receptiviti Scores:** The percentiles of each metric.
* **Snapshot:** An overview of the personality type of the person who spoke or wrote the text sample.
* **Communication Recommendation:** Advice on how to approach and communicate with the person.
* **Thinking Style:** A scale indicating where the person’s thinking style lies between being an emotion-based decision maker and an analytical decision maker.
* **Authenticity Detector:** A scale indicating where the person lies between being likely inauthentic versus being likely authentic in their speaking or writing.

![image-title-here](https://lh4.googleusercontent.com/mZm3ZC8sjQPrAxpZWD8QPlPivNpNqh-2Robw4vnMg1K2Er8gxhxujq4199VIDewOBpDYiDz4QmRxGqTcaqPn6JMYvRxIbspU-cnqSerdINixDElpyGejaz0x-mvS5A){:class="img-responsive"}

<br>
<br>

NOTE: _We strongly advise against merging text from multiple sources into one post (e.g., Twitter, Facebook, transcripts, etc.). If you plan to analyze content from multiple sources, we recommend creating a separate Person ID for each type of content. For example, to analyze Person A's Twitter and Facebook samples, create one Person_A_Twitter person_ID to which only Person A's Twitter samples are sent, and one Person_A_Facebook person_ID to which only Person A's Facebook samples are sent._
{: .label .label-yellow }
