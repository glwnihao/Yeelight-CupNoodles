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
                                        "name": "red", 
                                        "spectrumRGB": 16721680
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

| Params                                   | Type    | Value                                 | Remarks                    |
| ---------------------------------------- | ------- | ------------------------------------- | -------------------------- |
| context → locale_language                | String  | en                                    | Optional. Language code.   |
| intent                                   | String  | action.devices.EXECUTE                | Required.                  |
| id                                       | String  |                                       | Device ID                  |
| execution → command                      | String  | action.devices.commands.ColorAbsolute | Required.                  |
| execution → params → color → name        | String  | red                                   | Optional. Color name.      |
| execution → params → color → spectrumRGB | Integer | 0 - 16777215                          | Required. RGB color value. |