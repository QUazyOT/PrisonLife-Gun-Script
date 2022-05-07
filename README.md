# PrisonLife-Gun-Script
Idk dont claim as own
--Made by Quazy#4648

local allguns = false -- Change to true if you want all guns on execution
local gun = "AK-47" -- AK-47 | Remington 870 | M9 | M4A1

if allguns then
    local args = {
    [1] = workspace.Prison_ITEMS.giver:FindFirstChild("AK-47").ITEMPICKUP
    } 
local args3 = {
    [1] = workspace.Prison_ITEMS.giver:FindFirstChild("Remington 870").ITEMPICKUP
    }   
local args2 = {
    [1] = workspace.Prison_ITEMS.giver:FindFirstChild("M9").ITEMPICKUP
    }   
    workspace.Remote.ItemHandler:InvokeServer(unpack(args))
    workspace.Remote.ItemHandler:InvokeServer(unpack(args2))
    workspace.Remote.ItemHandler:InvokeServer(unpack(args3))
else
    local args16 = {
    [1] = workspace.Prison_ITEMS.giver:FindFirstChild(gun).ITEMPICKUP
    }
    
    workspace.Remote.ItemHandler:InvokeServer(unpack(args16))
end
