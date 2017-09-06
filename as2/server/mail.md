# Mail
##### Messages that pertain to users' mail system.
---
### Delete Mail From Player
Sent to clients when a postcard has been deleted from their penguin's mail.

`mdp`

|Argument|Type|Variadic?|
|---|---|---|
|newMailCount|Unsigned integer|No|

##### Example
`%xt%mdp%0%15%`

### Send Mail
Sent to clients after a send postcard request with either a successful result or an error.

`ms`

|Argument|Type|Variadic?|
|---|---|---|
|newCoinsAmount|Unsigned integer|No|
|postCardStatus|Unsigned integer|No|

##### `postCardStatus` Possibilities Table
|Status ID|Definition|
|---|---|
|0|Max Mail Count Reached|
|1|Mail Sent(Success)|
|2|Not Enough Coins|

##### Example
`%xt%ms%0%550%1%`

### Receive Mail
Sent to client that received a postcard.

`mr`

|Argument|Type|Variadic?|
|---|---|---|
|senderUsername|String|No|
|senderID|Unsigned integer|No|
|mailType|Unsigned integer|No|
|mailDetails|String|No|
|mailCreatedAt|Timestamp|No|
|mailID|Unsigned integer|No|

##### Example
`%xt%mr%0%Jad%1%50%%1504711291%1%`


### Get Mail
Sent to clients when they request their penguin's mail.

`mg`

|Argument|Type|Variadic?|
|---|---|---|
|postcards|Array of postcard information|Yes|

##### `postcards` Argument Table
Format: `senderName|senderID|mailType|mailDetails|mailCreatedAt|mailID`

|Argument|Type|
|---|---|
|senderUsername|String|
|senderID|Unsigned integer|
|mailType|Unsigned integer|
|mailDetails|String|
|mailCreatedAt|Timestamp|
|mailID|Unsigned integer|

##### Example
`%xt%mg%0%Nickname1|101|217||1454107091|4%Nickname2|101|37||1453826828|2%`

### Mail Start Engine
Sent to client in order to start the mail engine. Also pertains to the notification system on the mail button.

`mst`

|Argument|Type|Variadic?|
|---|---|---|
|unreadCount|Unsigned integer|No|
|mailCount|Unsigned integer|No|

##### Example
`%xt%mst%0%5%7%`
