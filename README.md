# Configuring Utility Chips
Some utility chips are able to be configured. You can require them like a regular module and edit properties of them. For example, adding a new option in Micromanage:
```lua
--@include utility_chips/micromanage.txt

local Micromanage = require("utility_chips/micromanage.txt")

Micromanage:addOption({
    Name = "Maul",
    Icon = "icon16/bug.png",
    Use = function( self, plr )
        Micromanage.useCommandOn( "ulx maul", plr )
    end
})
```

Take a look at the utility chips themselves to see how they can be configured!
