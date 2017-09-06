# Newspapers
##### Messages pertaining to the open/closed newspaper status shown on penguin avatars on the client.
---
### Open Newspaper
Sent to all penguins in a room to show a penguin opening their newspaper.

`at`

|Argument|Type|Variadic?|
|---|---|---|
|penguinID|Unsigned integer|No|

##### Example
`%xt%at%0%123%`

### Close Newspaper
Sent to all penguins in a room to show a penguin closing their newspaper.

`rt`

|Argument|Type|Variadic?|
|---|---|---|
|penguinID|Unsigned integer|No|

##### Example
`%xt%rt%0%123%`