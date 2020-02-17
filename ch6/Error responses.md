# Error responses

These are some error codes that can be returned in our responses.

```
{
    "requestId": "ff36a3cc-ec34-11e6-b1a0-64510650abcf", 
    "payload": {
        "errorCode": "notSupported"
    }
}
```

| Error code      | Details                                                      |
| --------------- | ------------------------------------------------------------ |
| authFailure     | General failure to authenticate.                             |
| deviceOffline   | The target is unreachable.                                   |
| timeout         | Internal timeout.                                            |
| deviceNotFound  | The device doesn't exist on the partner's side. This normally indicates a failure in data synchronization or a race condition. |
| valueOutOfRange | The range in parameters is out of bounds.                    |
| notSupported    | The command or its parameters are unsupported (this should generally not happen, as traits and business logic should prevent it). |
| protocolError   | Failure in processing the request.                           |
| unknownError    | Everything else, although anything that throws this should be replaced with a real error code. |