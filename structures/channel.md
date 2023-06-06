
## Channel model

| Key      | Type                                | Notes |
| -        | -                                   | -     |
| id       | String                              |       |
| name     | String                              | [^1]  |
| location | [Location](#channel-location-model) |       |

[^1]: `/[\\s\u{200b}-\u{200f}\u{2060}]/` is disallowed,
length is capped at 32

## Channel Location model

### DM type

| Key   | Type     | Notes            |
| -     | -        | -                |
| type  | "dm"     |                  |
| users | String[] | List of user IDs |

## Channel Request Response

| Key     | Type                      |
| -       | -                         |
| channel | [Channel](#channel-model) |
