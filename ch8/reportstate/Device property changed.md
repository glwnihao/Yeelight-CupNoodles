# Device property changed

```
{
    "requestId": "16349988792583564403",
    "unionId": "fPLhRVC_10gI9yQwwn3swNz4XwBqqJ8m8OrrA86A",
    "topic": "properties-changed",
 
    "properties": [
        {
            "property": "on",
            "id": "M1GAxtaW9A0LXNwZWMtdjIVgoAFGA55ZWVsaW5rLWNvbG9AyMRUUGAg0NTk2NTYwNRVoAA",
            "value": true
        }
    ]
}


{
    "requestId": "16349988792583564403",
    "unionId": "fPLhRVC_10gI9yQwwn3swNz4XwBqqJ8m8OrrA86A",
    "topic": "properties-changed",
 
    "properties": [
        {
            "property": "brightness",
            "id": "M1GAxtaW9A0LXNwZWMtdjIVgoAFGA55ZWVsaW5rLWNvbG9AyMRUUGAg0NTk2NTYwNRVoAA",
            "value": 100
        }
    ]
}
```

| Params                | Type   | Value                                    | Remarks                                                      |
| --------------------- | ------ | ---------------------------------------- | ------------------------------------------------------------ |
| requestId             | String | 4180463424101195867                      | Required. Random string as Id of each request for ease of tracing. |
| topic                 | String | properties-changed                       |                                                              |
| properties → property | String | on, brightness, color, color-temperature | Property name                                                |
| properties → id       | String |                                          | Device ID                                                    |
| properties → value    | String |                                          | Property value                                               |