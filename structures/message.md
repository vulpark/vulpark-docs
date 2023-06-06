
## Message model

| Key        | Type    | Notes                  |
| -          | -       | -                      |
| id         | String  |                        |
| channel_id | String  |                        |
| author_id  | String? |                        |
| content    | String  |                        |
| created    | String  | rfc3339 formatted date |

## Message Request Response

| Key     | Type                               |
| -       | -                                  |
| message | [Message](#message-model)          |
| channel | [Channel](./channel.md#channel-model) |
| author  | [User](./user.md#user-model)       |
