# Request Format

| Params                          | Type    | Value                                       | Remarks                                                    |
| ------------------------------- | ------- | ------------------------------------------- | ---------------------------------------------------------- |
| intent                          | String  | action.devices.EXECUTE                      | Required.                                                  |
| id                              | String  |                                             | Device ID                                                  |
| execution → command             | String  | action.devices.commands.BrightnessIncrement | Required.                                                  |
| execution → params → brightness | Integer | 1 - 100                                     | Optional. Brightness increment value, default value is 15. |

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

