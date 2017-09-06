# Inventory
##### Messages that pertain to users' items inventory functions.
---
### Query Player Awards
Sent to clients when they request their penguin's awards.

`qpa`

|Argument|Type|Variadic?|
|---|---|---|
|awards|Array of awards information|Yes|

##### `awards` Argument Table
Format: `awardID|creationDate|memberStatus`

|Argument|Type|
|---|---|
|awardID|Unsigned integer|
|creationDate|Timestamp|
|memberStatus|Boolean integer (0, 1)|

##### Example
`%xt%qpa%0%801|1151614800|0%802|1151614800|1%`

### Query Player Pins
Sent to clients when they request their penguin's pins.

`qpp`

|Argument|Type|Variadic?|
|---|---|---|
|pins|Array of pins information|Yes|

##### `pins` Argument Table
Format: `pinID|creationDate|memberStatus`

|Argument|Type|
|---|---|
|pinID|Unsigned integer|
|creationDate|Timestamp|
|memberStatus|Boolean integer (0, 1)|

##### Example
`%xt%qpp%0%550|1142553600|0%551|1143763200|1%`

### Get Inventory
Sent to clients when they request their penguin's items.

`gi`

|Argument|Type|Variadic?|
|---|---|---|
|itemID|Unsigned integer|Yes|

##### Example
`%xt%gi%0%413%414%567%`

### Add Item
Sent to clients after an item gets added to their penguin's inventory.

`ai`

|Argument|Type|Variadic?|
|---|---|---|
|itemID|Unsigned integer|No|
|coins|Unsigned integer|No|

##### Example
`%xt%ai%0%413%5000%`
