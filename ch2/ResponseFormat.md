# Response Format

```
{
    "requestId": "4180463424101195867",
    "payload": {
        "devices": [
            {
                "id": "M1GAxtaW9A0LXNwZWMtdjIVgoAFGA15ZWVsaW5rLW1vbm8xFRQYCDQ1MTAyMzgwFWYA",
                "type": "action.devices.types.LIGHT",
                "traits": [
                    "action.devices.traits.OnOff",
                    "action.devices.traits.Brightness"
                ],
                "name": {
                    "deviceName": "fairy"
                },
                "customData": {
                    "region": "cn",
                    "model": "yeelink-mono1"
                }
            },
            {
                "id": "M1GAxtaW9A0LXNwZWMtdjIVgoAFGA55ZWVsaW5rLWNvbG9AyMRUUGAg0NTk2NTYwNRVoAA",
                "type": "action.devices.types.LIGHT",
                "traits": [
                    "action.devices.traits.OnOff",
                    "action.devices.traits.Brightness",
                    "action.devices.traits.ColorTemperature",
                    "action.devices.traits.ColorSpectrum"
                ],
                "name": "living room",
                "attributes": {
                    "TemperatureMinK": 1700,
                    "TemperatureMaxK": 6500
                },
                "customData": {
                    "region": "cn",
                    "model": "yeelink-color1"
                }
            },
            {
                "id": "M1GAxtaW9A0LXNwZWMtdjIVgoAFGAt5ZWVsaW5rLWN0MhUUGAg4NzEzMDQyMhWcCAA",
                "type": "action.devices.types.LIGHT",
                "traits": [
                    "action.devices.traits.OnOff",
                    "action.devices.traits.Brightness",
                    "action.devices.traits.ColorTemperature"
                ],
                "name": {
                    "deviceName": "gorgeous"
                },
                "attributes": {
                    "TemperatureMinK": 2700,
                    "TemperatureMaxK": 6500
                },
                "customData": {
                    "region": "cn",
                    "model": "yeelink-ct2"
                }
            }
        ]
    }
}
```

| Params                         | Type          | Value                                                        | Remarks                                                      |
| ------------------------------ | ------------- | ------------------------------------------------------------ | ------------------------------------------------------------ |
| requestId                      | String        | 4180463424101195867                                          | Required. Random string as Id of each request for ease of tracing. |
| `id`                           | String        | `M1GAxtaW9A0LXNwZWMtdjIVgoAFGA15ZWVsaW5rLW1vbm8xFRQYCDQ1MTAyMzgwFWYA` | Device ID                                                    |
| type                           | String        | action.devices.types.LIGHT                                   | Device type                                                  |
| traits                         | Array<String> | action.devices.traits.OnOffaction.devices.traits.Brightnessaction.devices.traits.ColorTemperatureaction.devices.traits.ColorSpectrum | Device traits**OnOff**: The basic on and off functionality for any device that has binary on and off.**Brightness**: Absolute brightness setting is in a normalized range from 0 to 100.**ColorSpectrum**: This applies to "full" color bulbs that take RGB color ranges.**ColorTemperature**: This applies to "warmth" bulbs that take a color point in Kelvin. |
| deviceName                     | String        | living room                                                  | Device name                                                  |
| TemperatureMinKTemperatureMaxK |               |                                                              | Optional. temperature range.                                 |
| customData                     | Object        | String                                                       | This is a special object which need to be carried in future **QUERY** and **EXECUTE** requests to help Yeelight understand the execution context, third-party doesn't need to proceed the data inside this section. |