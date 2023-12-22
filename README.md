local OrionLib = loadstring(game:HttpGet(('https://raw.githubusercontent.com/shlexware/Orion/main/source')))()
local Window = OrionLib:MakeWindow({Name = "KeySystem", HidePremium = true, SaveConfig = true, IntroText = "Key System"})

OrionLib:MakeNotification({
	Name = "Welcome",
	Content = "Your In A Key System",
	Image = "rbxassetid://4483345998",
	Time = 5
})

_G.Key = "AlexisXAloneoV4" -- You Put Your Key Here
_G.KeyInput = "string"

function MakeScriptHub()
loadstring(game:HttpGet("https://raw.githubusercontent.com/YogaProjectRblx/ALONEV4ALEXIS/main/README.md"))();

end

function CorrectKeyNotifications()
    OrionLib:MakeNotification({
        Name = "Correct Key",
        Content = "You Entered The Correct Key",
        Image = "rbxassetid://4483345998",
        Time = 5
    })
end

function WrongKeyNotifications()
    OrionLib:MakeNotification({
        Name = " Wrong Key",
        Content = "You Entered A Wrong Key",
        Image = "rbxassetid://4483345998",
        Time = 5
    })
end

local Tab = Window:MakeTab({
	Name = "Key",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = false
})

Tab:AddTextbox({
	Name = "Enter Key",
	Default = "",
	TextDisappear = true,
	Callback = function(Value)
        _G.KeyInput = Value
	end	  
})

Tab:AddButton({
	Name = "Check Key!",
	Callback = function()
        if _G.KeyInput == _G.Key then
         MakeScriptHub()
         CorrectKeyNotifications()
     else
        WrongKeyNotifications()
        end
  	end    
})

Tab:AddButton({
	Name = "Click To Get The Key",
	Callback = function()
setclipboard("https://discord.com/invite/ZSnZPMBscb")
toclipboard("https://discord.com/invite/ZSnZPMBscb")
      		print("button pressed")
  	end    
})

Tab:AddLabel("Marry Chrismas")
Tab:AddLabel("Thanks For Using Our Script")

local Tab = Window:MakeTab({
	Name = "Links",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = false
})

Tab:AddButton({
	Name = "Aloneo YouTube Link",
	Callback = function()
setclipboard("https://www.youtube.com/@YogaExploits")
toclipboard("https://www.youtube.com/@YogaExploits")
      		print("button pressed")
  	end    
})

Tab:AddButton({
	Name = "ClickTab:AddButton",
	Name = "Aloneo Discord Server",
	Callback = function()
setclipboard("https://discord.com/invite/ZSnZPMBscb")
toclipboard("https://discord.com/invite/ZSnZPMBscb")
      		print("button pressed")
  	end    
})
