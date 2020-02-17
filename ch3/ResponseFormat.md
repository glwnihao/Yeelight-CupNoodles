# ResponseFormat



```
{
    "requestId": "14671248160676185539",
    "payload": {
        "devices": {
            "M1GAxtaW9A0LXNwZWMtdjIVgoAFGA15ZWVsaW5rLW1vbm8xFRQYCDQ1MTAyMzgwFWYA": {
                "online": true,
                "on": true,
                "brightness": 50
            },
            "M1GAxtaW9A0LXNwZWMtdjIVgoAFGA55ZWVsaW5rLWNvbG9AyMRUUGAg0NTk2NTYwNRVoAA": {
                "online": true,
                "on": true,
                "brightness": 100,
                "color": {
                    "spectrumRGB": 16769565,
                    "temperature": 5000
                }
            }
        }
    }
}
```

| Params                                                       | Type    | Value                      | Remarks                                                      |
| ------------------------------------------------------------ | ------- | -------------------------- | ------------------------------------------------------------ |
| requestId                                                    | String  | 4180463424101195867        | Required. Random string as Id of each request for ease of tracing. |
| `M1GAxtaW9A0LXNwZWMtdjIVgoAFGA15ZWVsaW5rLW1vbm8xFRQYCDQ1MTAyMzgwFWYA` | String  |                            | Device ID                                                    |
| `online`                                                     | Boolean | true / false               | Whether the device is online                                 |
| on                                                           | Boolean | true / false               | Whether the device is on                                     |
| brightness                                                   | Int     | 1 - 100                    | Device's current brightness                                  |
| `spectrumRGB`                                                | Int     | 0 - 16777215               | Device's current RGB color value                             |
| temperature                                                  | Int     | 1700 - 6500 or 2700 - 6500 | Device's current temperature value                           |