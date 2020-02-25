# REST API

## Overview

A REST API is used for accessing and manipulating data within DutyCalls by third parties.

## Authentication

All API calls require authentication. The authentication scheme we use for HTTP requests, is Basic Authentication. In every request a combination of a username (consumerKey) and a password (consumerSecret) must be provided. It is also possible to provide the following `Authorization` header: `Basic <credentials>` in a request. Where credentials is a base64-encoded string of `username:password`.

You can find these credentials by:

1. Going to the sources page in your workspace.
2. Clicking on the **Setup** button of the relevant source.
3. Verifying that you are authorized to access these credentials.
4. Copying the relevant credentials from the setup dialog.

![image - Get credentials](images/setup-source-dialog-1.png)

> **Important**: You should store your credentials in a secure location. It is important to keep your credentials confidential to protect your account.

## API specifications and testing

For user-friendliness, we have documented and hosted the API specifications in [Swagger](https://app.swaggerhub.com/apis-docs/robbm1/DutyCalls). Besides the easy of use, this also makes it very easy for you to manually test our API.
