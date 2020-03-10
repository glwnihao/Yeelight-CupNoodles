# Request Format

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
                                    "model": "yeelink-mono1", 
                                    "region": "CN"
                                }, 
                                "id": "M1GAxtaW9A0LXNwZWMtdjIVgoAFGA55ZWVsaW5rLWNvbG9AyMRUUGAg0NTk2NTYwNRVoAA"
                            }
                        ], 
                        "execution": [
                            {
                                "command": "action.devices.commands.ColorAbsolute", 
                                "params": {
                                    "color": {
                                        "name": "white", 
										"temperature": 5000
                                    }
                                }
                            }
                        ]
                    }
                ]
            }
        }
    ], 
    "requestId": "16349988792583564403"
}
```

| Params                                   | Type    | Value                                 | Remarks                            |
| ---------------------------------------- | ------- | ------------------------------------- | ---------------------------------- |
| context → locale_language                | String  | en                                    | Optional. Language code.           |
| intent                                   | String  | action.devices.EXECUTE                | Required.                          |
| id                                       | String  |                                       | Device ID                          |
| execution → command                      | String  | action.devices.commands.ColorAbsolute | Required.                          |
| execution → params → color → name        | String  | white                                 | Optional. Color name.              |
| execution → params → color → temperature | Integer | 1700 - 2700 / 2700 - 6500             | Required. Color temperature value. |