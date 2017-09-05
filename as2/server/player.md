# Player
##### Messages pertaining to the player actions.
---
### Send Frame
Sent to all penguins in a room to update a player frame.

|Argument|Type|Variadic?|
|---|---|---|
|penguinID|Unsigned integer|No|
|Frame|Unsigned integer|No|

##### Example
`%xt%sf%0%123%5%`

### Send Move
Sent to all penguins in a room to update a player location.

|Argument|Type|Variadic?|
|---|---|---|
|penguinID|Unsigned integer|No|
|X Postion|Unsigned integer|No|
|Y Postion|Unsigned integer|No|

##### Example
`%xt%sp%0%123%0%0%`

### Send Emote
Sent to all penguins in a room to show an emote sent by a penguin.

|Argument|Type|Variadic?|
|---|---|---|
|penguinID|Unsigned integer|No|
|Emote ID|Unsigned integer|No|

##### Example
`%xt%se%0%123%3%`

### Send Joke
Sent to all penguins in a room to show a joke sent by a penguin.

|Argument|Type|Variadic?|
|---|---|---|
|penguinID|Unsigned integer|No|
|Joke ID|Unsigned integer|No|

##### Example
`%xt%sj%0%123%3%`


### Send Message
Sent to all penguins in a room to show a message sent by a penguin.

|Argument|Type|Variadic?|
|---|---|---|
|penguinID|Unsigned integer|No|
|Message|String|No|

##### Example
`%xt%sm%0%123%Hello%`


### Send Safe Message
Sent to all penguins in a room to show a safe message sent by a penguin.

|Argument|Type|Variadic?|
|---|---|---|
|penguinID|Unsigned integer|No|
|Safe Message ID|Unsigned integer|No|

##### Example
`%xt%ss%0%123%5%`
