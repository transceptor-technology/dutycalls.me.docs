# Authentication

All API calls require authentication. The authentication scheme we use for HTTP requests, is Basic Authentication. In every request a combination of a username and a password must be provided. When manually sending an HTTP request to our API, the following header is required: `Authorization: Basic $CREDENTIALS`. Where `$CREDENTIALS` is a base64-encoded string of `username:password`.

You can find these credentials by:

1. Going to the **Sources** page in your workspace.
2. Clicking on the **Setup** button of the relevant source.
3. Verifying that you are authorized to access these credentials.
4. Copying the relevant credentials from the setup dialog.

    ![image - Get credentials](../images/setup-source-dialog-1.png){: style="width:500px"}

!!! warning
    You should store your credentials in a secure location. It is important to keep your credentials confidential to protect your account.
