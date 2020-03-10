# Request Format

| Params                          | Type    | Value                                      | Remarks           |
| ------------------------------- | ------- | ------------------------------------------ | ----------------- |
| intent                          | String  | action.devices.EXECUTE                     | Required.         |
| id                              | String  |                                            | Device ID         |
| execution → command             | String  | action.devices.commands.BrightnessAbsolute | Required.         |
| execution → params → brightness | Integer | 1 - 100                                    | Brightness value. |

```
{
    "inputs": [
        {
            "intent": "action.devices.EXECUTE", 
            "payload": {
                "commands": [
                    {
                        "devices": [
                            {
                                "customData": { 
                                    "model": "yeelink-mono1", 
                                    "region": "CN"
                                }, 
                                "id": "M1GAxtaW9A0LXNwZWMtdjIVgoAFGA55ZWVsaW5rLWNvbG9AyMRUUGAg0NTk2NTYwNRVoAA"
                            }
                        ], 
                        "execution": [
                            {
                                "command": "action.devices.commands.BrightnessAbsolute", 
                                "params": {
                                    "brightness": 100
                                }
                            }
                        ]
                    }
                ]
            }
        }
    ], 
    "requestId": "18210843532278199762"
}
```

