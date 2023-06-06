# Events

An event object has it's name as a key, and the object being it's data

Example:
```jsonc
{
    "MessageCreate": {
        "message": {
            //...
        },
        "author": null
    }
}
```

## HandshakeStart

This has no data, will show as `{"HandshaskeStart": {}}`

You must respond with `{"Handshake": {"token": "TOKEN_GOES_HERE"}}`

## HandshakeComplete

This event is fired when you successfully login.

| Key  | Type                          | Notes                     |
| -    | -                             | -                         |
| user | [User](./user.md#user-model)  | The user you logged in as |

## MessageCreate

This has the same data as a [Message Request Response](./message.md#message-request-response).

## ChannelCreate

| Key     | Type                                  | Notes                             |
| -       | -                                     | -                                 |
| channel | [Channel](./channel.md#channel-model) |                                   |
| creator | [User](./user.md#user-model)          | The user that created the channel |
