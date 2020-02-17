# Request Format

| Params                  | Type    | Value                         | Remarks                                                      |
| ----------------------- | ------- | ----------------------------- | ------------------------------------------------------------ |
| requestId               | String  | 4180463424101195867           | Required. Id of request for ease of tracing, random string.  |
| locale_language         | String  | `en`                          | Optional. Language code <https://cloud.google.com/translate/docs/languages> |
| intent                  | String  | action.devices.EXECUTE        | Required.                                                    |
| id                      | String  |                               | Device ID                                                    |
| execution → command     | String  | action.devices.commands.OnOff | Required.                                                    |
| execution → params → on | Boolean | true / false                  | true: turn onfalse: turn off                                 |

```

{
    "inputs": [
        {
            "context": {
                "locale_language": "en"
            }, 
            "intent": "action.devices.EXECUTE", 
            "payload": {
                "commands": [
                    {
                        "devices": [
                            {
                                "customData": {
                                    "region": "cn",
                                    "model": "yeelink-mono1"
                                }, 
                                "id": "M1GAxtaW9A0LXNwZWMtdjIVgoAFGA15ZWVsaW5rLW1vbm8xFRQYCDQ1MTAyMzgwFWYA"
                            }
                        ], 
                        "execution": [
                            {
                                "command": "action.devices.commands.OnOff", 
                                "params": {
                                    "on": true
                                }
                            }
                        ]
                    }
                ]
            }
        }
    ], 
    "requestId": "6529877997918554205"
}
```

