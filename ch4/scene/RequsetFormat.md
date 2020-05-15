# Request Format

| Params              | Type   | Value                                 | Remarks   |
| ------------------- | ------ | ------------------------------------- | --------- |
| intent              | String | action.devices.EXECUTE                | Required. |
| id                  | String |                                       | Device ID |
| execution → command | String | action.devices.commands.ActivateScene | Required. |
|                     |        |                                       |           |

```
{
				"inputs": [{
						"intent": "action.devices.EXECUTE",
						"payload": {
						
							"commands": [
			                    {
			                        "devices": [{
											"id": "6-199"
										}
									], 
			                        "execution": [
			                            {
			                                "command": "action.devices.commands.ActivateScene"
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

