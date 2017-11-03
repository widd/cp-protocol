# Moderation
##### Messages that allow in-game moderators to perform privileged actions.
---
### Moderator Action
Sent from the server in response to a client message for performing a privileged action.
The requesting client must have the proper permissions to do so; implementation of this is up to the server.
The _type_ argument represents the action type - either a kick, mute, or ban.

`ma`

|Argument|Type|Variadic?|
|---|---|---|
|type|Character|No|
|penguinID|Unsigned integer|No|
|username|String|No|

##### Example
`%xt%ma%0%m%100%Nickname1%`

##### Action Types
|ID|Description|
|---|---|
|m|Mute Player|
|k|Kick Player|
|b|Ban Player|