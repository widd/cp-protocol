# Clothing
##### Messages that handle clothing updates of penguins in a room.
---
### Update Color
Sent to all penguins in a room to show a penguin's new color when they change their current one.

`upc`

|Argument|Type|Variadic?|
|---|---|---|
|penguinID|Unsigned integer|No|
|itemID|Unsigned integer|No|

##### Example
`%xt%upc%0%123%1%`

### Update Head
Sent to all penguins in a room to show a penguin's new head item when they change their current one.

`uph`

|Argument|Type|Variadic?|
|---|---|---|
|penguinID|Unsigned integer|No|
|itemID|Unsigned integer|No|

##### Example
`%xt%uph%0%123%1%`

### Update Face
Sent to all penguins in a room to show a penguin's new face item when they change their current one.

`upf`

|Argument|Type|Variadic?|
|---|---|---|
|penguinID|Unsigned integer|No|
|itemID|Unsigned integer|No|

##### Example
`%xt%upf%0%123%1%`

### Update Neck
Sent to all penguins in a room to show a penguin's new neck item when they change their current one.

`upn`

|Argument|Type|Variadic?|
|---|---|---|
|penguinID|Unsigned integer|No|
|itemID|Unsigned integer|No|

##### Example
`%xt%upn%0%123%1%`

### Update Body
Sent to all penguins in a room to show a penguin's new body item when they change their current one.

`upb`

|Argument|Type|Variadic?|
|---|---|---|
|penguinID|Unsigned integer|No|
|itemID|Unsigned integer|No|

##### Example
`%xt%upb%0%123%1%`

### Update Hands
Sent to all penguins in a room to show a penguin's new hand item when they change their current one.

`upa`

|Argument|Type|Variadic?|
|---|---|---|
|penguinID|Unsigned integer|No|
|itemID|Unsigned integer|No|

##### Example
`%xt%upa%0%123%1%`

### Update Feet
Sent to all penguins in a room to show a penguin's new feet item when they change their current one.

`upe`

|Argument|Type|Variadic?|
|---|---|---|
|penguinID|Unsigned integer|No|
|itemID|Unsigned integer|No|

##### Example
`%xt%upe%0%123%1%`

### Update Photo
Sent to all penguins in a room to show a penguin's new playercard photo/background when they change their current one.

This has no visible changes on the client unless you have the penguin's playercard open at the time, but the client will keep track of it.

`upp`

|Argument|Type|Variadic?|
|---|---|---|
|penguinID|Unsigned integer|No|
|itemID|Unsigned integer|No|

##### Example
`%xt%upp%0%123%1%`

### Update Pin
Sent to all penguins in a room to show a penguin's new playercard pin when they change their current one.

This has no visible changes on the client unless you have the penguin's playercard open at the time, but the client will keep track of it.

`upl`

|Argument|Type|Variadic?|
|---|---|---|
|penguinID|Unsigned integer|No|
|itemID|Unsigned integer|No|

##### Example
`%xt%upl%0%123%1%`
