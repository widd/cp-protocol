# Player
##### Messages pertaining to the player actions.
---
### Send Frame
Sent to all penguins in a room to update a player frame. 
`sf`

|Argument|Type|Variadic?|
|---|---|---|
|penguinID|Unsigned integer|No|
|frame|Unsigned integer|No|

##### Example
`%xt%sf%0%123%5%`

### Send Move
Sent to all penguins in a room to update a player location. 
`sp`

|Argument|Type|Variadic?|
|---|---|---|
|penguinID|Unsigned integer|No|
|positionX|Unsigned integer|No|
|positionY|Unsigned integer|No|

##### Example
`%xt%sp%0%123%0%0%`

### Send Throw Snowball
Sent to all penguins in a room to show a snowball thrown by a penguin. 
`sb`

|Argument|Type|Variadic?|
|---|---|---|
|penguinID|Unsigned integer|No|
|positionX|Unsigned integer|No|
|positionY|Unsigned integer|No|

##### Example
`%xt%sb%0%123%0%0%`


### Send Emote
Sent to all penguins in a room to show an emote sent by a penguin. 
`se`

|Argument|Type|Variadic?|
|---|---|---|
|penguinID|Unsigned integer|No|
|emoteID|Unsigned integer|No|

##### Example
`%xt%se%0%123%3%`

### Send Joke
Sent to all penguins in a room to show a joke said by a penguin. 
`sj`

|Argument|Type|Variadic?|
|---|---|---|
|penguinID|Unsigned integer|No|
|jokeID|Unsigned integer|No|

##### Example
`%xt%sj%0%123%3%`


### Send Message
Sent to all penguins in a room to show a message said by a penguin. 
`sm`

|Argument|Type|Variadic?|
|---|---|---|
|penguinID|Unsigned integer|No|
|message|String|No|

##### Example
`%xt%sm%0%123%Hello%`


### Send Safe Message
Sent to all penguins in a room to show a safe message said by a penguin. 
`ss`

|Argument|Type|Variadic?|
|---|---|---|
|penguinID|Unsigned integer|No|
|safeMessageID|Unsigned integer|No|

##### Example
`%xt%ss%0%123%5%`
