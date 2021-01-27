# REST API

## Overview

A REST API is used for accessing and manipulating data within DutyCalls by third parties.

---

## Authentication

All API calls require authentication. The authentication scheme we use for HTTP requests, is Basic Authentication. In every request a combination of a username and a password must be provided. When manually sending an HTTP request to our API, the following header is required: `Authorization: Basic $CREDENTIALS`. Where `$CREDENTIALS` is a base64-encoded string of `username:password`.

You can find these credentials by:

1. Going to the sources page in your workspace.
2. Clicking on the **Setup** button of the relevant source.
3. Verifying that you are authorized to access these credentials.
4. Copying the relevant credentials from the setup dialog.

    ![image - Get credentials](images/setup-source-dialog-1.png){: style="width:500px"}

> **Important:** You should store your credentials in a secure location. It is important to keep your credentials confidential to protect your account.

---

## Example

In addition to the credentials and the data itself, the name or names of the targeted channels must also be included in the HTTP request. These must be added as the value of the query parameter `channel` in the URI of the request. An example of this can be seen below.

```curl
curl -X POST "https://dutycalls.me/api/ticket?channel=$CHANNEL_NAME"
    -H  "accept: application/json"
        -H  "Content-Type: application/json"
            -H "Authorization: Basic $CREDENTIALS"
                -d {
                        "title": "This is the title of the ticket",
                        "body": "This is the body of the ticket",
                        "severity": "medium"
                    }
```

> **Note:** The keys and values of the JSON to be sent, must exactly match the source configuration. Want to know more about configuring a source within DutyCalls? Check out the [getting started](getting-started.md) guide.

---

## API specifications and testing

For user-friendliness, we have documented and hosted the API specifications in [Swagger](https://app.swaggerhub.com/apis-docs/robbm1/DutyCalls). Besides the easy of use, this also makes it very easy for you to manually test our API.
