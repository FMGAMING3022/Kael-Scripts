# Fivem Item Rob With Menu for QB-Core Framework.

### Dependencies
- [qb-menu](https://github.com/qbcore-framework/qb-menu) - You Can Use Any Menu


### Preview
- [Youtube](https://youtu.be/GEnwjLEttac)
- ![Image Preview](https://media.discordapp.net/attachments/1079128394320580668/1079153230681997442/image.png)
- ![Image Preview](https://media.discordapp.net/attachments/1079128394320580668/1079153506549760170/image.png)


### Features
- Easy To Configuration
- Loot Cash
- Loot Any Item From Config

### Installation

# Add Image qb-inventory/html/images

# Add qb-core/shared/items.lua
```
	["itemrob_toolbox"] 			 = {["name"] = "itemrob_toolbox", 					["label"] = "Robbing Kit", 				["weight"] = 100, 		["type"] = "item", 		["image"] = "itemrob_toolbox.png", 		["unique"] = true, 		["useable"] = true, 	["shouldClose"] = false,	["combinable"] = nil,   ["description"] = "Robbing Kit"},

```

### For Radialmenu Event
```
    [1] = {
        id = 'rob',
        title = 'Rob',
        icon = 'wallet',
        items = {
            {
                id = 'robpolice',
                title = 'Rob Player',
                icon = 'search-dollar',
                type = 'client',
                event = 'kael-rob:client:useitemrobtoolbox',
                shouldClose = true
            },
        }
    },
```


## Contains encrypted file to prevent leaks, everything necessary for changes is changeable

## Join With Us
- [Discord](https://discord.gg/NbpHD9RaSJ)
- [Tebex](https://kael.tebex.io/)
