# Dupe
if game.PlaceId == 6299805723 then

local OrionLib = loadstring(game:HttpGet(('https://raw.githubusercontent.com/shlexware/Orion/main/source')))()

local Window = OrionLib:MakeWindow({Name = "Puck Hub", HidePremium = false, SaveConfig = true, ConfigFolder = "Puck Hub", IntroEnabled = false,})

--Valores
_G.AutoClick = true



--Funcoes

function AutoClick()
    loadstring(game:HttpGet("https://raw.githubusercontent.com/sandwichk/RobloxScripts/main/Scripts/BadWare/Dupe/AFSim", true))()
end


--Frame

local Main = Window:MakeTab({
	Name = "Auto-Farm",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = false
})
local Section = Main:AddSection({
	Name = "PRINCIPAIS"
})
Main:AddToggle({
	Name = "Dupe-Script",
	Default = false,
	Callback = function(Value)
		_G.AutoClick = Value
        AutoClick()
	end    
})

elseif game.PlaceId == 6299805723 then

    --FV

    local plr = game.Players.LocalPlayer

    --HUB

    local OrionLib = loadstring(game:HttpGet(('https://raw.githubusercontent.com/shlexware/Orion/main/source')))()

    local Window = OrionLib:MakeWindow({Name = "Puck Hub", HidePremium = false, SaveConfig = true, ConfigFolder = "Puck Hub", IntroEnabled = false,})



    --Valores






    --Funcoes
    function Antikick()
        plr.UserId = 1216025046
        print("Alterado com sucesso")
        end

    function ForceTP()
        plr.Backpack.Antbug:Destroy()
    end


    --Abas
    local PlayerTab = Window:MakeTab({
        Name = "Player",
        Icon = "rbxassetid://4483345998",
        PremiumOnly = false
    })
    local Section = PlayerTab:AddSection({
        Name = "Jogador"
    })
    PlayerTab:AddButton({
        Name = "Anti-Kick!",
        Callback = function()
            Antikick()
          end  
    })
    PlayerTab:AddButton({
        Name = "Force TP",
        Callback = function()
            ForceTP()
          end  
    })

end
