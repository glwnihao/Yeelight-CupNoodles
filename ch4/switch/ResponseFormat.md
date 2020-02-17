# ResponseFormat

| Params                 | Type          | Value             | Remarks              |
| ---------------------- | ------------- | ----------------- | -------------------- |
| commands → ids         | Array<String> |                   | Device ID collection |
| commands → status      | String        | `SUCCESS / ERROR` | Perform result       |
| commands → errorCode   | String        |                   | Error code           |
| commands → debugString | String        |                   | Error details        |

```
{
    "requestId": "6529877997918554205",
    "payload": {
        "commands": [
            {
                "ids": [
                    "M1GAxtaW9A0LXNwZWMtdjIVgoAFGA55ZWVsaW5rLWNvbG9AyMRUUGAg1NTAwMTk0NhVoAA"
                ],
                "status": "ERROR",
                "errorCode": "deviceNotFound",
                "debugString": ""
            },
            {
                "ids": [
                    "M1GAxtaW9A0LXNwZWMtdjIVgoAFGA55ZWVsaW5rLWNvbG9AyMRUUGAg0NTk2NTYwNRVoAA"
                ],
                "status": "SUCCESS"
            }
        ]
    }
}
```

