# Device status changed

```

{
    "requestId": "16349988792583564403",
    "unionId": "fPLhRVC_10gI9yQwwn3swNz4XwBqqJ8m8OrrA86A",
    "topic": "devices-status-changed",
    "devices": [
        {
            "id": "M1GAxtaW9A0LXNwZWMtdjIVgoAFGA55ZWVsaW5rLWNvbG9AyMRUUGAg0NTk2NTYwNRVoAA",
            "online": true
        }
    ]
}
```

| Params           | Type    | Value                  | Remarks                                                      |
| ---------------- | ------- | ---------------------- | ------------------------------------------------------------ |
| requestId        | String  | 4180463424101195867    | Required. Random string as Id of each request for ease of tracing. |
| topic            | String  | devices-status-changed |                                                              |
| devices → id     | String  |                        | Device ID                                                    |
| devices → online | Boolean | true / false           | Device status                                                |