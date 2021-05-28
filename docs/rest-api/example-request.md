# Example request

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

!!! note
    The keys and values of the JSON to be sent, must exactly match the source configuration. Want to know more about configuring a source within DutyCalls? Check out the [getting started](getting-started.md) guide.
