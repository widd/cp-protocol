# Buddies
##### Messages that pertain to users' buddy list functions.
---
### Get Buddies
Sent to clients when they request their penguin's buddy list.

`gb`

|Argument|Type|Variadic?|
|---|---|---|
|buddies|Array of buddy information; `penguinID|username|onlineStatus`|Yes|

##### `buddies` Argument Table

|Argument|Type|
|---|---|
|penguinID|Unsigned integer|
|username|String|
|onlineStatus|Boolean integer (0, 1)|

##### Example
`%xt%gb%0%123|Nickname1|0%100|Online Penguin|1%`

### Buddy Request
Sent to clients when they receive a buddy request from another user.

`br`

|Argument|Type|Variadic?|
|---|---|---|
|penguinID|Unsigned integer|No|
|username|String|No|

##### Example
`%xt%br%0%123%Nickname1%`

### Buddy Accepted
Sent to clients when the server is notified the target user has accepted their buddy request.

At this point the client will add the target user to the in-game buddy list.

`ba`

|Argument|Type|Variadic?|
|---|---|---|
|penguinID|Unsigned integer|No|
|username|String|No|

##### Example
`%xt%ba%0%123%Nickname1%`

### Buddy Removed
Sent to clients when the server wishes to remove a player from their buddy list, generally when a user requests it.

`rb`

|Argument|Type|Variadic?|
|---|---|---|
|penguinID|Unsigned integer|No|
|username|String|No|

##### Example
`%xt%rb%0%123%Nickname1%`

### Buddy Found
Sent to clients in response to a buddy find request message.

The client ignores this unless a request has been sent - hence the lack of a user-identifying argument.

`bf`

|Argument|Type|Variadic?|
|---|---|---|
|roomID|Unsigned integer|No|

##### Example
`%xt%bf%0%100%`

### Buddy Online
Sent to clients when a buddy logs into the same game server as them.

`bon`

|Argument|Type|Variadic?|
|---|---|---|
|penguinID|Unsigned integer|No|

##### Example
`%xt%bon%0%123%`

### Buddy Offline
Sent to clients when a buddy that was previously on the same game server disconnects.

`bof`

|Argument|Type|Variadic?|
|---|---|---|
|penguinID|Unsigned integer|No|

##### Example
`%xt%bof%0%123%`