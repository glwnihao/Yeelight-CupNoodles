# Device bind/unbind

```
{
    "requestId": "16349988792583564403",
    "unionId": "fPLhRVC_10gI9yQwwn3swNz4XwBqqJ8m8OrrA86A",
    "topic": "bind-device"
}
```

| Params    | Type   | Value                       | Remarks                                                      |
| --------- | ------ | --------------------------- | ------------------------------------------------------------ |
| requestId | String | 4180463424101195867         | Required. Random string as Id of each request for ease of tracing. |
| topic     | String | bind-device / unbind-device | When user bind or unbind a new device, Yeelight will send this topic to third-party, and expect a SYNC request from third-party to refresh user's device list. |