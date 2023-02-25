# Fivem Crypto Mining for QB-Core Framework.

### Dependencies
- [qb-crypto](https://github.com/QBCore-framework/qb-crypto)
- [qb-phone-npstyle](https://github.com/llbooya/qb-phone-npstyle)
- [qb-phone](https://github.com/qbcore-framework/qb-phone)
- [qb-houses](https://github.com/qbcore-framework/qb-houses)
- [zdiscord](https://github.com/zfbx/zdiscord)


### Preview
- [Youtube](https://www.youtube.com/watch?v=AMOcXzHLYLU)


### Features
- Easy To Configuration
- Mining With 10+ Different PC Parts
- Easy Dashboard For Miner
- Discord Subscription System

### Installation
# Add qb-houses/config.lua
```
	["miningsetup"] = {
		label = "Mining Setup",
		items = {
			[1] = { ["object"] = "xm_prop_base_staff_desk_01", ["price"] = 1000, ["label"] = "desk + setup" },
			[2] = { ["object"] = "xm_base_cia_server_01", ["price"] = 1000, ["label"] = "Mining Server" },			
		},
	},
```
## Add qb-houses/client/main.lua
- Find This
```
Wait(5000)
---- Put Target Code Here ---
RegisterHouseExitZone(house)
```

- Put Target Code Here
```
                            ------- Mining Target ----------
                            exports['pdrp-target']:AddTargetModel("xm_base_cia_server_01", {
                                options = {
                                    {
                                        type = "client",
                                        event = "kael-cryptomining:client:openservermenu",
                                        icon = "fas fa-server",
                                        label = "Open Server",
                                        housename = CurrentHouse,
                                    },
                                },
                                distance = 4.0
                            })
                        
                            exports['pdrp-target']:AddTargetModel("xm_prop_base_staff_desk_01", {
                                options = {
                                    {
                                        type = "client",
                                        event = "kael-cryptomining:client:openMiningSystem",
                                        icon = "fas fa-laptop-house",
                                        label = "Open Mining System",
                                        housename = CurrentHouse,
                                    },
                                },
                                distance = 4.0
                            })
                            ------- Mining Target ----------
```
# Add Image qb-inventory/html/images
# Add qb-core/shared/items.lua
```
	--- Kael Crypto Mining
	["cpu"] 	 			= {["name"] = "cpu",				["label"] = "Mining CPU",			    	["weight"] = 300,    	  ["type"] = "item",		["image"] = "cpu.png",  		["unique"] = false,		["useable"] = false,	["shouldClose"] = true,    ["combinable"] = nil,   ["description"] = "A CPU For Crypto Mining"},
	["motherboard"] 	 	= {["name"] = "motherboard",		["label"] = "Mining Motherboard",			["weight"] = 300,    	  ["type"] = "item",		["image"] = "motherboard.png",  ["unique"] = false,		["useable"] = false,	["shouldClose"] = true,    ["combinable"] = nil,   ["description"] = "A Motherboard For Crypto Mining"},
	["ram"] 	 			= {["name"] = "ram",				["label"] = "Mining Ram",			    	["weight"] = 300,    	  ["type"] = "item",		["image"] = "ram.png",  		["unique"] = false,		["useable"] = false,	["shouldClose"] = true,    ["combinable"] = nil,   ["description"] = "A Ram For Crypto Mining"},
	["psu"] 	 			= {["name"] = "psu",				["label"] = "Mining PowerSupply",			["weight"] = 300,    	  ["type"] = "item",		["image"] = "psu.png",  		["unique"] = false,		["useable"] = false,	["shouldClose"] = true,    ["combinable"] = nil,   ["description"] = "A PSU For Crypto Mining"},
	["gpu3090"] 	 		= {["name"] = "gpu3090",			["label"] = "Mining GPU 3090",			    ["weight"] = 300,    	  ["type"] = "item",		["image"] = "gpu3090.png", 		["unique"] = false,		["useable"] = false,	["shouldClose"] = true,    ["combinable"] = nil,   ["description"] = "A GPU 3090 For Crypto Mining"},
	["gpu2080super"] 	 	= {["name"] = "gpu2080super",		["label"] = "Mining GPU 2080 Super",		["weight"] = 300,    	  ["type"] = "item",		["image"] = "gpu2080super.png", ["unique"] = false,		["useable"] = false,	["shouldClose"] = true,    ["combinable"] = nil,   ["description"] = "A GPU 2080 super For Crypto Mining"},
	["gpu1080ti"] 	 		= {["name"] = "gpu1080ti",			["label"] = "Mining GPU 1080 TI",			["weight"] = 300,    	  ["type"] = "item",		["image"] = "gpu1080ti.png",  	["unique"] = false,		["useable"] = false,	["shouldClose"] = true,    ["combinable"] = nil,   ["description"] = "A GPU 1080 TI For Crypto Mining"},
	["gpu1660super"] 	 	= {["name"] = "gpu1660super",		["label"] = "Mining GPU 1660 Super",		["weight"] = 300,    	  ["type"] = "item",		["image"] = "gpu1660super.png", ["unique"] = false,		["useable"] = false,	["shouldClose"] = true,    ["combinable"] = nil,   ["description"] = "A GPU 1660 Super For Crypto Mining"},
```


## Contains encrypted file to prevent leaks, everything necessary for changes is changeable

## Join With Us
- [Discord](https://discord.gg/NbpHD9RaSJ)
- [Tebex](https://kael.tebex.io/)
