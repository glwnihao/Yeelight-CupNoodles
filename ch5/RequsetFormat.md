# Request Format

```
{
    "inputs": [
        {
            "intent": "action.devices.DISCONNECT"
        }
    ],
    "requestId": "508610314576360567"
}
```

| Params    | Type   | Value                     | Remarks                                                      |
| --------- | ------ | ------------------------- | ------------------------------------------------------------ |
| requestId | String | 4180463424101195867       | Required. Random string as Id of each request for ease of tracing. |
| intent    | String | action.devices.DISCONNECT | Required.                                                    |