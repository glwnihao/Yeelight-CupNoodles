# Request Format

| Params                          | Type    | Value                                       | Remarks                                                    |
| ------------------------------- | ------- | ------------------------------------------- | ---------------------------------------------------------- |
| intent                          | String  | action.devices.EXECUTE                      | Required.                                                  |
| id                              | String  |                                             | Device ID                                                  |
| execution → command             | String  | action.devices.commands.BrightnessIncrement | Required.                                                  |
| execution → params → brightness | Integer | 1 - 100                                     | Optional. Brightness increment value, default value is 15. |

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
                                    "region": "cn"
                                },
                                "id": "M1GAxtaW9A0LXNwZWMtdjIVgoAFGA55ZWVsaW5rLWNvbG9AyMRUUGAg0NTk2NTYwNRVoAA"
                            }
                        ],
                        "execution": [
                            {
                                "command": "action.devices.commands.BrightnessIncrement",
                                "params": {
                                    "brightness": 15
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

