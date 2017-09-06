# System
##### Messages that take care of unseen background logic unknown to the user.
---
### Heartbeat
Sent from the server in response to a client heartbeat/ping.
This message has no arguments, but the __internal room ID__ is still required.

`h`

|Argument|Type|Variadic?|
|---|---|---|
|None|N/A|N/A|

##### Example
`%xt%h%0%`