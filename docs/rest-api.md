# REST API

## Overview

A REST API is used for accessing and manipulating data within DutyCalls by third parties.

## Authentication

All API calls require authentication. The authentication scheme we use for HTTP requests, is Basic Authentication. In every request the header field in the form of `Authorization: Basic <credentials>` must be added. Where credentials is the API key of a source.

You can find this API key by:

1. Going to the sources page in your workspace.
2. Clicking on the **Setup** button of the relevant source.
3. Copying the API key from the setup dialog.

![image - Get API key - Step 2](/images/setup-source-dialog.png)

> **Important**: You should store your API key in a secure location. It is important to keep your API key confidential to protect your account.

## API specifications and testing

For user-friendliness, we have documented and hosted the API specifications in [Swagger](https://app.swaggerhub.com/apis-docs/robbm1/DutyCalls/1.0.0). Besides the easy of use, this also makes it very easy for you to manually test our API.