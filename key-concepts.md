# key concepts
## Chat App Temp Token & Chat User Temp Token
You can generate two types of chat tokens from the dashboard.
|  Type   |  Privileges  |  Recommended Use |
|  ----  | ----  | ----  |
| Chat App Temp Token  | The app temp token can be used to perform any AgoraChat operation | In your server side code  |
| Chat User Temp Token  | The user temp token can be used to login users |  In your client side code(during development)  |

## Chat User Temp Token & Chat User Token
These two tokens can be used to login users via the loginWithAgoraToken method, it looks like this `AgoraChat.instance().login(aAgoraToken)`.
If you're just testing thing out, it's okay to use the `Chat User Temp Token` to login users. But in production, you should use the `Chat User Token` to login users. As the name implies, temp is for temporary use.
Tokens used in Agora Chat need to be generated in your app server, including `Chat User Token`. For more information, see: [Secure authentication with tokens
]( https://docs.agora.io/en/agora-chat/develop/authentication?platform=ios)
