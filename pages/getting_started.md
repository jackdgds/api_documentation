---
layout: page
title:  "Getting Started With the Receptiviti API"
nav_order: 3
has_children: true
has_toc: false
---

# Getting Started With the Receptiviti API

Once we set up your account, you will receive an email with a link to the web interface of our API. You must get your API Key and API Secret Key (password) in order to start using the API, which you will find in the CSV file generated from the instructions below.

**To get your API Key and API Secret Key:**

1. Navigate to the Receptiviti API by clicking the link in the email we sent you.
2. Click **Generate API Key**.
![image-title-here](https://lh4.googleusercontent.com/FWDt9kqBIhDtoiwQaIb9mISBCd04B8AFCP7Pgrb86s_J-3TeTL1wbgfwAj8sx-HxLN8bH2fiLVAYq1JU-SAy90WV6s4tRXdcUx3ZODK-W-7BdQXtXRG8YwG1i8rXmg){:class="img-responsive"}
3. Open the CSV file and copy the API Key under the ```api_key``` cell.
4. Paste the key in the appropriate field, depending on how you are interacting with the API, e.g., Swagger or cURL. (See below for full details.)
5. Copy the Secret Key under the ```api_secret_key``` cell.
6. Paste the key in the appropriate field, depending on how you are interacting with the API, e.g., Swagger or cURL. (See below for full details.)


**There are several ways to interact with the Receptiviti API:**

- **Command line:** By using cURL, you can make API calls and get minified JSON results. (You can use a service like <https://pretty-print-json.js.org/> to make it more readable.) See sample code and responses [here](example_api_call) and [here](example_api_response).

- **Receptiviti Open API/Swagger page:** Here, you can post samples and get results in JSON, as well as have your calls converted to cURL format for copy-and-pasting to the command line, if you wish to do so. Access this page [here](https://api-v3.receptiviti.com/v3/api/spec).

- **Web application:** We provide a user interface where you can upload language samples and get results. This is a simple way to get quick results, but it is not designed for large-scale analysis projects. Access the UI [here](https://api-v3.receptiviti.com/#/try/analyze_content).

-  **Your programming language of choice:** This will be the method of choice for data scientists, machine learning modellers, statisticians, and other users with experience using APIs.

IMPORTANT NOTE: _Be sure to store your API Key and API Secret Key in a place where it is easy for you to access._
{: .label .label-yellow }
