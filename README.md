local OrionLib = loadstring(game:HttpGet(('https://raw.githubusercontent.com/shlexware/Orion/main/source')))()


local Window = OrionLib:MakeWindow({Name = "Puck Hub", HidePremium = false, SaveConfig = true, IntroEnabled = false})


--////////////////////////// PONTOS /////////////////////////////////////
local plr = game.Players.LocalPlayer
local char = plr.Character




--///////////////////////////   FUNC /////////////////////////////////////


function TeleportBaseTR()
    loadstring(game:HttpGet("https://raw.githubusercontent.com/sandwichk/RobloxScripts/main/Scripts/BadWare/Dupe/AFSim", true))()
end

function ZeroHud()
    loadstring(game:HttpGet("https://raw.githubusercontent.com/Discord0000/Zer0Hub/main/MainScript.lua"))()
end


--///////////////////////////    ABAS    //////////////////////////////////

local plrTab = Window:MakeTab({
	Name = "Inicio",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = false
})

local Section = plrTab:AddSection({
	Name = "Seja Muito Bem Vindo ao (Puck Hub)"
})


local plrTab = Window:MakeTab({
	Name = "Anime Fighters",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = false
})


local Section = plrTab:AddSection({
	Name = "Scripts"
})

plrTab:AddButton({
	Name = "New Dupe",
	Callback = function()
        TeleportBaseTR()
  	end    
})


plrTab:AddButton({
	Name = "Zer0 Hub",
	Callback = function()
        ZeroHud()
  	end    
})
