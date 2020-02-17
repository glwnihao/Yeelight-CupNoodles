# Request Format

```
{
    "inputs": [
        {
            "intent": "action.devices.QUERY", 
            "payload": {
                "devices": [
                    {
                        "customData": {
                            "region": "cn",
                            "model": "yeelink-mono1"
                        }, 
                        "id": "M1GAxtaW9A0LXNwZWMtdjIVgoAFGA15ZWVsaW5rLW1vbm8xFRQYCDQ1MTAyMzgwFWYA"
                    }, 
                    {
                        "customData": {
                            "region": "cn",
                            "model": "yeelink-color1"
                        }, 
                        "id": "M1GAxtaW9A0LXNwZWMtdjIVgoAFGA55ZWVsaW5rLWNvbG9AyMRUUGAg0NTk2NTYwNRVoAA"
                    }
                ]
            }
        }
    ], 
    "requestId": "14671248160676185539"
}
```

| **Params** | **Type** | **Value**            | **Remarks**                                               |
| ---------- | -------- | -------------------- | --------------------------------------------------------- |
| requestId  | String   | 4180463424101195867  | Random string as Id of each request for  ease of tracing. |
| intent     | String   | action.devices.QUERY | Required.                                                 |