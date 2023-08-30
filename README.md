--Loader
local OrionLib = loadstring(game:HttpGet(('https://raw.githubusercontent.com/shlexware/Orion/main/source')))()

--Config Geral
local Window = OrionLib:MakeWindow({Name = "Menu V2", HidePremium = false, SaveConfig = true, IntroEnabled = false})
local Window = OrionLib:MakeWindow({Name = "Menu V2", HidePremium = false, SaveConfig = true, IntroEnabled = false})
local Player = game.Players.LocalPlayer

OrionLib:MakeNotification({
	Name = "Logado!",
	Content = "Logado no Menu V2 EM..."..Player.Name.." ",
	Image = "rbxassetid://4483345998",
	Time = 5
})

--Valor funcional
_G.Aimbot = true
_G.Loop = true
_G.Key = "V2TROLL"
_G.KeyInput = "string"

--Funcao do Serial Killer loop by
function Loop()
	while _G.Loop == true do
		local DR = game:GetService("ReplicatedStorage")["ACS_Engine"].Eventos.Damage

		for PlayerIndex,GivenPlayer in pairs(game.Players:GetPlayers()) do
			local Char = GivenPlayer.Character
			DR:FireServer(Char.Humanoid,Char.Humanoid.MaxHealth,0,0)
		end
	end    
	wait(0.1)
end

function MakeScriptHub()
	local Window = OrionLib:MakeWindow({Name = "Menu V2", HidePremium = false, SaveConfig = true, IntroEnabled = true, IntroText = "Menu V2"})
end

function CorrectKeyNotification()
	OrionLib:MakeNotification({
		Name = "Correta key",
		Content = "Key Injetada",
		Image = "rbxassetid://4483345998",
		Time = 5
	})
end   

function IncorrectKeyNotification()
	OrionLib:MakeNotification({
		Name = "Key Incorreta",
		Content = "Key Error",
		Image = "rbxassetid://4483345998",
		Time = 5
	})
end       

--Funcao ativar/desativar
function Aimbot()
	while _G.Aimbot == true do
		loadstring(game:HttpGet('https://raw.githubusercontent.com/fatesc/fates-esp/main/main.lua'))()
		wait(0.1)
	end
end

--Scripts Section e botao
local KeyTab = Window:MakeTab({
	Name = "Keys",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = false      
})    
KeyTab:AddTextbox({
	Name = "Key Menu Troll",
	Default = "Coloque a key aqui!",
	TextDisappear = true,
	Callback = function(Value)
		_G.KeyInput = Value
	end	  
})
KeyTab:AddButton({
	Name = "Checkar Key",
	Callback = function()
		if _G.KeyInput == _G.Key then
			MakeScriptHub()
			CorrectKeyNotification()
		else
			IncorrectKeyNotification()
		end
	end    
})

local JogadorTab = Window:MakeTab({
	Name = "Jogador",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = false      
})
local PlayersTab = Window:MakeTab({
	Name = "Players",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = false  
})
local ArmaTab = Window:MakeTab({
	Name = "Weapon",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = false     
})
local EspTab = Window:MakeTab({
	Name = "Visual",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = false              
})    
local TrollTab = Window:MakeTab({
	Name = "Destruição",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = false      
})    
local MenusTab = Window:MakeTab({
	Name = "Menus",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = false         
})    
local HubTab = Window:MakeTab({
	Name = "Hub Trolls",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = false                
})    
local BypassTab = Window:MakeTab({
	Name = "Anti Cheat",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = false                    
})    
local RoleplayTab = Window:MakeTab({
	Name = "Roleplay",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = false      
})    
local CarroTab = Window:MakeTab({
	Name = "Veiculos",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = false                        
})    
local AdmTab = Window:MakeTab({
	Name = "Adm",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = false    
})       
local Arceus = Window:MakeTab({
	Name = "Arceus Leak",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = false    
})   
--Pontos
local plr = game.Players.LocalPlayer
local char = plr.Character




--Funcao farm teleporte favela do batata


function TeleportBaseTR1()
	char.HumanoidRootPart.CFrame = CFrame.new(-1380.51526, 29.3764763, 1138.62524, 1, 0, 0, 0, 1, 0, 0, 0, 1)
end

function TeleportBaseTR2()
	char.HumanoidRootPart.CFrame = CFrame.new(-1448.61536, 28.8764763, 1222.62524, 1, 0, 0, 0, 1, 0, 0, 0, 1)
end

function TeleportBaseTR3()
	char.HumanoidRootPart.CFrame = CFrame.new(-2719.37646, 0.714344025, -97.993187, 1, 0, 0, 0, 1, 0, 0, 0, 1)
end

function TeleportBaseTR4()
	char.HumanoidRootPart.CFrame = CFrame.new(-2775.80005, 26.1462669, -71.699173, 1, 0, 0, 0, 0.726554513, -0.687108874, 0, 0.687108874, 0.726554513)
end


--Abas Farm

local plrTab = Window:MakeTab({
	Name = "Farm",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = false
})

local Section = plrTab:AddSection({
	Name = "Farm - Favela do batata (USEM EM 5 SEGUNDOS SEMPRE)"
})

plrTab:AddButton({
	Name = "Pegar lixo - Favela do batata",
	Callback = function()
		TeleportBaseTR1()
	end
})

plrTab:AddButton({
	Name = "Entregar lixo - Favela do batata",
	Callback = function()
		TeleportBaseTR2()
	end
})plrTab:AddButton({
	Name = "Pegar cimento - Favela do batata",
	Callback = function()
		TeleportBaseTR3()
	end
})plrTab:AddButton({
	Name = "Entregar cimento - Favela do batata",
	Callback = function()
		TeleportBaseTR4()
	end
})
local ConfigTab = Window:MakeTab({
	Name = "Settings",
	Icon = "rbxassetid://4483345998",
	PremiumOnly = false                                  
})
local Section = JogadorTab:AddSection({
	Name = "Alterador de Speed/Pulo"
})
JogadorTab:AddButton({
	Name = "Valor Speed Hub (Risco)",
	Callback = function()
		loadstring(game:HttpGet('https://raw.githubusercontent.com/Pedroxz63/Kill-by-pedroxz63/main/Kill%20by%20Pedroxz63.md'))()
	end 
})
local Section = ConfigTab:AddSection({
	Name = "Config Menu"
})
ConfigTab:AddBind({
	Name = "Bind Menu",
	Default = Enum.KeyCode.E,
	Hold = false,
	Callback = function()
		print("press")
	end    
})
ConfigTab:AddColorpicker({
	Name = "Colorpicker",
	Default = Color3.fromRGB(255, 0, 0),
	Callback = function(Value)
		print(Value)
	end	  
})
ConfigTab:AddButton({
	Name = "Alterar Cursor Anti Bug",
	Callback = function()
		local mouse = game.Players.LocalPlayer:GetMouse()

		mouse.Icon = "rbxassetid://5992580992"
	end    
})
local Section = ArmaTab:AddSection({
	Name = "Weapon Hacks"
})
ArmaTab:AddButton({
	Name = "Inf Ammo",
	Callback = function()
		_G.Damage = 1003 -- might not work
		_G.FireRate = 0
		_G.Clips = 999999
		_G.AmmoInClip = 999999
		_G.Auto = true


		--\\ Load string By Pedroxz

		loadstring(game:HttpGet("https://raw.githubusercontent.com/RIPExploit/23452tr2t423t3t34tg34gg/master/ryewifwfripexloit.lua", true))()
	end    
})
ArmaTab:AddButton({
	Name = "Puxar armas",
	Callback = function()
		for i, v in pairs(game:GetDescendants()) do
			if v:IsA('Tool') then
				v.Parent = game:GetService('Players').LocalPlayer.Backpack
			end
		end

		game:GetService('Players').LocalPlayer.Character.Humanoid.Died:Connect(function()
			for i, v in pairs(game:GetService('Players').LocalPlayer.Backpack:GetDescendants()) do
				if v:IsA('Tool') then
					v.Parent = game:GetService('Teams')
				end
			end
			for i, v in pairs(game:GetService('Players').LocalPlayer.Character:GetDescendants()) do
				if v:IsA('Tool') then
					v.Parent = game:GetService('Teams')
				end
			end
		end)
	end    
})
ArmaTab:AddButton({
	Name = "Puxar e clonar itens",
	Callback = function()
		local function ClonarTool(tool, player)
			local backpack = player:WaitForChild("Backpack")
			local clonedTool = tool:Clone()
			clonedTool.Parent = backpack
		end

		local function procurarTools()
			local player = game.Players.LocalPlayer

			for _, tool in pairs(game:GetDescendants()) do
				if tool:IsA("Tool") then
					ClonarTool(tool, player)
				end
			end
		end

		procurarTools()
	end    
}) 
local Section = CarroTab:AddSection({
	Name = "Veiculos"
})
CarroTab:AddButton({
	Name = "Reparar Veiculo - Depende da ACS",
	Callback = function()
		wait(0.2)
		game.StarterGui:SetCore("SendNotification", {
			Title = "Veiculo Reperado!"; -- the title 
			Text = "Reparado com sucesso!"; -- what the text says 
			Duration = 5; -- how long the notification should in secounds
		})
	end    
})
CarroTab:AddButton({
	Name = "Puxar Fusca - Cidade Alta",
	Callback = function()
		local args = {
			[1] = "spawner",
			[2] = "Fusca",
			[3] = workspace.EstacionamentoModel.Spawns
		}

		game:GetService("ReplicatedStorage").ConcessionariaRS.Remotes.Check:InvokeServer(unpack(args))
		wait(0.5)

	end    
})
Arceus:AddButton({
	Name = "Aimbot Arceus",
	Callback = function()
--[[
		AIMBOT SCRIPT

		Remade and optimized by Riky47#3355 for Arceus X
		# spdmteam.com
		
		Edited and fixed by AZY#0348 for Fluxus / Hydrogen Compatibility
        # Chillz and Maik
]]

		local Script_Title = "Arceus X <font color=\"rgb(255, 0, 0)\">|</font> Aimbot"

		-- Instances:
		local Arceus = Instance.new("ScreenGui")
		local Main = Instance.new("Frame")
		local UICorner = Instance.new("UICorner")
		local Intro = Instance.new("Frame")
		local UICorner_2 = Instance.new("UICorner")
		local Logo = Instance.new("ImageButton")
		local UIAspectRatioConstraint = Instance.new("UIAspectRatioConstraint")
		local Title = Instance.new("TextLabel")
		local Menu = Instance.new("ScrollingFrame")
		local UIListLayout = Instance.new("UIListLayout")
		local Toggle = Instance.new("ImageButton")
		local UICorner_3 = Instance.new("UICorner")
		local Enabled = Instance.new("Frame")
		local UIAspectRatioConstraint_2 = Instance.new("UIAspectRatioConstraint")
		local UICorner_4 = Instance.new("UICorner")
		local Check = Instance.new("Frame")
		local UIAspectRatioConstraint_3 = Instance.new("UIAspectRatioConstraint")
		local UICorner_5 = Instance.new("UICorner")
		local Name = Instance.new("TextLabel")
		local UIGradient = Instance.new("UIGradient")
		local Button = Instance.new("ImageButton")
		local UICorner_6 = Instance.new("UICorner")
		local Name_2 = Instance.new("TextLabel")
		local UIGradient_2 = Instance.new("UIGradient")
		local tab = Instance.new("Frame")
		local Close = Instance.new("TextButton")
		local ComboElem = Instance.new("ImageButton")
		local UICorner_7 = Instance.new("UICorner")
		local Name_3 = Instance.new("TextLabel")
		local UIGradient_3 = Instance.new("UIGradient")
		local Img = Instance.new("TextLabel")
		local UIAspectRatioConstraint_4 = Instance.new("UIAspectRatioConstraint")
		local ComboBox = Instance.new("ImageButton")
		local UICorner_8 = Instance.new("UICorner")
		local Name_4 = Instance.new("TextLabel")
		local UIGradient_4 = Instance.new("UIGradient")
		local Img_2 = Instance.new("TextLabel")
		local UIAspectRatioConstraint_5 = Instance.new("UIAspectRatioConstraint")

		--Properties:

		Arceus.Name = "Arceus"
		Arceus.Enabled = true
		Arceus.ResetOnSpawn = true
		Arceus.ZIndexBehavior = Enum.ZIndexBehavior.Sibling
		Arceus.DisplayOrder = 999999999

		Main.Name = "Main"
		Main.Parent = Arceus
		Main.Active = true
		Main.Draggable = true
		Main.AnchorPoint = Vector2.new(0.5, 0.5)
		Main.BackgroundColor3 = Color3.fromRGB(40, 40, 40)
		Main.BorderSizePixel = 0
		Main.Position = UDim2.new(0.5, 0, -0.2, 0) --UDim2.new(0.5, 0, 0.5, 0)
		Main.Size = UDim2.new(0.3, 0, 0.3, 0)

		UICorner.CornerRadius = UDim.new(0.1, 0)
		UICorner.Parent = Main

		Intro.Name = "Intro"
		Intro.Parent = Main
		Intro.BackgroundColor3 = Color3.fromRGB(40, 40, 40)
		Intro.ClipsDescendants = true
		Intro.Size = UDim2.new(1, 0, 1, 0)
		Intro.ZIndex = 2

		UICorner_2.CornerRadius = UDim.new(0.1, 0)
		UICorner_2.Parent = Intro

		Logo.Parent = Intro
		Logo.AnchorPoint = Vector2.new(0.5, 0.5)
		Logo.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
		Logo.BackgroundTransparency = 1
		Logo.BorderSizePixel = 0
		Logo.Position = UDim2.new(0.5, 0, 0.5, 0)
		Logo.Size = UDim2.new(0.75, 0, 0.75, 0)
		Logo.ZIndex = 2
		Logo.Image = "http://www.roblox.com/asset/?id=9178187770"
		Logo.ScaleType = Enum.ScaleType.Fit
		Logo.Active = false

		UIAspectRatioConstraint.Parent = Logo

		Title.Name = "Title"
		Title.Parent = Main
		Title.AnchorPoint = Vector2.new(1, 0)
		Title.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
		Title.BackgroundTransparency = 1
		Title.BorderSizePixel = 0
		Title.Position = UDim2.new(0.975, 0, 0.075, 0)
		Title.Size = UDim2.new(0.85, 0, 0.155, 0)
		Title.Font = Enum.Font.TitilliumWeb
		Title.FontFace = Font.new("rbxasset://fonts/families/TitilliumWeb.json", Enum.FontWeight.Bold)
		Title.RichText = true
		Title.Text = Script_Title
		Title.TextColor3 = Color3.fromRGB(255, 255, 255)
		Title.TextScaled = true
		Title.TextSize = 14
		Title.TextWrapped = true
		Title.TextXAlignment = Enum.TextXAlignment.Left
		Title.TextYAlignment = Enum.TextYAlignment.Center

		Menu.Name = "Menu"
		Menu.Parent = Main
		Menu.Active = true
		Menu.AnchorPoint = Vector2.new(0.5, 1)
		Menu.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
		Menu.BackgroundTransparency = 1
		Menu.AutomaticCanvasSize = Enum.AutomaticSize.Y
		Menu.BorderSizePixel = 0
		Menu.Position = UDim2.new(0.5, 0, 0.95, 0)
		Menu.Size = UDim2.new(0.95, 0, 0.65, 0)
		Menu.CanvasSize = UDim2.new(0, 0, 0, 0)
		Menu.ScrollBarImageColor3 = Color3.fromRGB(255, 255, 255)
		Menu.ScrollBarThickness = Menu.AbsoluteSize.X/25

		UIListLayout.Parent = Menu
		--UIListLayout.Padding = UDim.new(0.025, 0)
		UIListLayout.SortOrder = Enum.SortOrder.LayoutOrder

		Toggle.Name = "Toggle"
		Toggle.Visible = false
		--Toggle.Parent = Arceus
		Toggle.BackgroundColor3 = Color3.fromRGB(55, 55, 55)
		Toggle.Size = UDim2.new(0.95, 0, 0, 50)

		UICorner_3.CornerRadius = UDim.new(0.25, 0)
		UICorner_3.Parent = Toggle

		Enabled.Name = "Enabled"
		Enabled.Parent = Toggle
		Enabled.AnchorPoint = Vector2.new(1, 0.5)
		Enabled.BackgroundColor3 = Color3.fromRGB(50, 50, 50)
		Enabled.Position = UDim2.new(0.975, 0, 0.5, 0)
		Enabled.Size = UDim2.new(0.75, 0, 0.75, 0)

		UIAspectRatioConstraint_2.Parent = Enabled

		UICorner_4.CornerRadius = UDim.new(0.3, 0)
		UICorner_4.Parent = Enabled

		Check.Name = "Check"
		Check.Parent = Enabled
		Check.AnchorPoint = Vector2.new(0.5, 0.5)
		Check.BackgroundColor3 = Color3.fromRGB(255, 0, 0)
		Check.Position = UDim2.new(0.5, 0, 0.5, 0)
		Check.Size = UDim2.new(0.65, 0, 0.65, 0)

		UIAspectRatioConstraint_3.Parent = Check

		UICorner_5.CornerRadius = UDim.new(0.3, 0)
		UICorner_5.Parent = Check

		Name.Name = "Name"
		Name.Parent = Toggle
		Name.AnchorPoint = Vector2.new(0, 0.5)
		Name.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
		Name.BackgroundTransparency = 1
		Name.BorderSizePixel = 0
		Name.Position = UDim2.new(0.05, 0, 0.5, 0)
		Name.Size = UDim2.new(0.75, 0, 0.8, 0)
		Name.Font = Enum.Font.TitilliumWeb
		Name.Text = "Script"
		Name.TextColor3 = Color3.fromRGB(255, 255, 255)
		Name.TextScaled = true
		Name.TextSize = 14
		Name.TextWrapped = true
		Name.TextXAlignment = Enum.TextXAlignment.Left
		Name.TextYAlignment = Enum.TextYAlignment.Bottom

		UIGradient.Color = ColorSequence.new{ColorSequenceKeypoint.new(0.00, Color3.fromRGB(255, 255, 255)), ColorSequenceKeypoint.new(1.00, Color3.fromRGB(180, 180, 180))}
		UIGradient.Parent = Toggle

		Button.Name = "Button"
		--Button.Parent = Arceus
		Button.BackgroundColor3 = Color3.fromRGB(55, 55, 55)
		Button.Size = UDim2.new(0.95, 0, 0, 50)

		UICorner_6.CornerRadius = UDim.new(0.25, 0)
		UICorner_6.Parent = Button

		Name_2.Name = "Name"
		Name_2.Parent = Button
		Name_2.AnchorPoint = Vector2.new(0, 0.5)
		Name_2.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
		Name_2.BackgroundTransparency = 1
		Name_2.BorderSizePixel = 0
		Name_2.Position = UDim2.new(0.05, 0, 0.5, 0)
		Name_2.Size = UDim2.new(0.95, 0, 0.82, 0)
		Name_2.Font = Enum.Font.TitilliumWeb
		Name_2.Text = "Enabled"
		Name_2.TextColor3 = Color3.fromRGB(255, 255, 255)
		Name_2.TextScaled = true
		Name_2.TextSize = 14
		Name_2.TextWrapped = true
		Name_2.TextXAlignment = Enum.TextXAlignment.Left
		Name_2.TextYAlignment = Enum.TextYAlignment.Bottom

		UIGradient_2.Color = ColorSequence.new{ColorSequenceKeypoint.new(0.00, Color3.fromRGB(255, 255, 255)), ColorSequenceKeypoint.new(1.00, Color3.fromRGB(180, 180, 180))}
		UIGradient_2.Parent = Button

		tab.Name = "Tab"
		tab.Visible = false
		--tab.Parent = Arceus
		tab.BackgroundTransparency = 1
		tab.Size = UDim2.new(0.95, 0, 0.025, 0)

		Close.Name = "Close"
		Close.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
		Close.BackgroundTransparency = 1
		Close.BorderSizePixel = 0
		Close.Position = UDim2.new(0.8, 0, 0.1, 0)
		Close.Size = UDim2.new(0.15, 0, 0.125, 0)
		Close.Font = Enum.Font.FredokaOne
		Close.Text = "X"
		Close.TextColor3 = Color3.fromRGB(255, 0, 0)
		Close.TextScaled = true
		Close.TextSize = 14
		Close.TextWrapped = true
		Close.TextXAlignment = Enum.TextXAlignment.Right
		Close.Parent = Main

		ComboElem.Name = "ComboElem"
		ComboElem.BackgroundColor3 = Color3.fromRGB(55, 55, 55)
		ComboElem.Size = UDim2.new(0.95, 0, 0, 50)

		UICorner_7.CornerRadius = UDim.new(0.25, 0)
		UICorner_7.Parent = ComboElem

		Name_3.Name = "Name"
		Name_3.Parent = ComboElem
		Name_3.AnchorPoint = Vector2.new(0, 0.5)
		Name_3.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
		Name_3.BackgroundTransparency = 1
		Name_3.BorderSizePixel = 0
		Name_3.Position = UDim2.new(0.05, 0, 0.5, 0)
		Name_3.Size = UDim2.new(0.75, 0, 0.8, 0)
		Name_3.Font = Enum.Font.TitilliumWeb
		Name_3.Text = "Enabled"
		Name_3.TextColor3 = Color3.fromRGB(255, 0, 0)
		Name_3.TextScaled = true
		Name_3.TextSize = 14
		Name_3.TextWrapped = true
		Name_3.TextXAlignment = Enum.TextXAlignment.Left
		Name_3.TextYAlignment = Enum.TextYAlignment.Bottom

		UIGradient_3.Color = ColorSequence.new{ColorSequenceKeypoint.new(0.00, Color3.fromRGB(255, 255, 255)), ColorSequenceKeypoint.new(1.00, Color3.fromRGB(180, 180, 180))}
		UIGradient_3.Rotation = 180
		UIGradient_3.Parent = ComboElem

		Img.Name = "Img"
		Img.Parent = ComboElem
		Img.AnchorPoint = Vector2.new(1, 0.5)
		Img.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
		Img.BackgroundTransparency = 1
		Img.BorderSizePixel = 0
		Img.Position = UDim2.new(0.975, 0, 0.5, 0)
		Img.Rotation = 90
		Img.Size = UDim2.new(0.75, 0, 0.75, 0)
		Img.Font = Enum.Font.FredokaOne
		Img.Text = "^"
		Img.TextColor3 = Color3.fromRGB(255, 255, 255)
		Img.TextScaled = true
		Img.TextSize = 14
		Img.TextWrapped = true

		UIAspectRatioConstraint_4.Parent = Img

		ComboBox.Name = "ComboBox"
		ComboBox.BackgroundColor3 = Color3.fromRGB(55, 55, 55)
		ComboBox.Size = UDim2.new(0.95, 0, 0, 50)

		UICorner_8.CornerRadius = UDim.new(0.25, 0)
		UICorner_8.Parent = ComboBox

		Name_4.Name = "Name"
		Name_4.Parent = ComboBox
		Name_4.AnchorPoint = Vector2.new(0, 0.5)
		Name_4.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
		Name_4.BackgroundTransparency = 1.000
		Name_4.BorderSizePixel = 0
		Name_4.Position = UDim2.new(0.05, 0, 0.5, 0)
		Name_4.Size = UDim2.new(0.75, 0, 0.8, 0)
		Name_4.Font = Enum.Font.TitilliumWeb
		Name_4.Text = "Enabled"
		Name_4.TextColor3 = Color3.fromRGB(255, 255, 255)
		Name_4.TextScaled = true
		Name_4.TextSize = 14
		Name_4.TextWrapped = true
		Name_4.TextXAlignment = Enum.TextXAlignment.Left
		Name_4.TextYAlignment = Enum.TextYAlignment.Bottom

		UIGradient_4.Color = ColorSequence.new{ColorSequenceKeypoint.new(0.00, Color3.fromRGB(255, 255, 255)), ColorSequenceKeypoint.new(1.00, Color3.fromRGB(180, 180, 180))}
		UIGradient_4.Parent = ComboBox

		Img_2.Name = "Img"
		Img_2.Parent = ComboBox
		Img_2.AnchorPoint = Vector2.new(1, 0.5)
		Img_2.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
		Img_2.BackgroundTransparency = 1
		Img_2.BorderSizePixel = 0
		Img_2.Rotation = 180
		Img_2.Position = UDim2.new(0.975, 0, 0.5, 0)
		Img_2.Size = UDim2.new(0.75, 0, 0.75, 0)
		Img_2.Font = Enum.Font.FredokaOne
		Img_2.Text = "^"
		Img_2.TextColor3 = Color3.fromRGB(255, 0, 0)
		Img_2.TextScaled = true
		Img_2.TextSize = 14
		Img_2.TextWrapped = true

		UIAspectRatioConstraint_5.Parent = Img_2

		-- SCRIPT

		local TweenService = game:GetService("TweenService")
		Close.MouseButton1Click:Connect(function()
			Logo.Active = true
			TweenService:Create(Intro, TweenInfo.new(0.25, Enum.EasingStyle.Linear, Enum.EasingDirection.In), {BackgroundTransparency = 0}):Play()

			task.wait(0.3)
			Logo:TweenSizeAndPosition(
				UDim2.fromScale(0.75, 0.75),
				UDim2.fromScale(0.5, 0.5),
				Enum.EasingDirection.Out,
				Enum.EasingStyle.Quad,
				0.25, true, nil
			)

			task.wait(0.3)
			Main:TweenSize(
				UDim2.fromScale(0.1, 0.175),
				Enum.EasingDirection.Out,
				Enum.EasingStyle.Quad,
				0.25, true, nil
			)

			task.wait(0.3)
			for _, obj in pairs(Main:GetChildren()) do
				if obj:IsA("GuiObject") and obj ~= Intro then
					obj.Visible = false
				end
			end

			TweenService:Create(Logo, TweenInfo.new(0.25, Enum.EasingStyle.Linear, Enum.EasingDirection.In), {ImageTransparency = 0.8}):Play()
			TweenService:Create(Intro, TweenInfo.new(0.25, Enum.EasingStyle.Linear, Enum.EasingDirection.In), {BackgroundTransparency = 1}):Play()
			TweenService:Create(Main, TweenInfo.new(0.25, Enum.EasingStyle.Linear, Enum.EasingDirection.In), {BackgroundTransparency = 0.8}):Play()
		end)

		Logo.MouseButton1Click:Connect(function()
			Logo.Active = false
			TweenService:Create(Logo, TweenInfo.new(0.25, Enum.EasingStyle.Linear, Enum.EasingDirection.In), {ImageTransparency = 0}):Play()
			TweenService:Create(Intro, TweenInfo.new(0.25, Enum.EasingStyle.Linear, Enum.EasingDirection.In), {BackgroundTransparency = 0}):Play()
			TweenService:Create(Main, TweenInfo.new(0.25, Enum.EasingStyle.Linear, Enum.EasingDirection.In), {BackgroundTransparency = 0}):Play()

			task.wait(0.3)
			Main:TweenSize(
				UDim2.fromScale(0.3, 0.3),
				Enum.EasingDirection.Out,
				Enum.EasingStyle.Quad,
				0.25, true, nil
			)

			task.wait(0.3)
			Logo:TweenSizeAndPosition(
				UDim2.fromScale(0.175, 0.175),
				UDim2.fromScale(0.075, 0.15),
				Enum.EasingDirection.Out,
				Enum.EasingStyle.Quad,
				0.25, true, nil
			)

			for _, obj in pairs(Main:GetChildren()) do
				if obj:IsA("GuiObject") and obj ~= Intro then
					obj.Visible = true
				end
			end

			task.wait(0.3)
			TweenService:Create(Intro, TweenInfo.new(0.25, Enum.EasingStyle.Linear, Enum.EasingDirection.In), {BackgroundTransparency = 1}):Play()
		end)

		local function uiparent()
			local success, parent = pcall(function()
				return gethui()
			end)

			if not success then
				return game:GetService("CoreGui")
			end

			return parent
		end

		local success, err = pcall(function()
			Arceus.Parent = uiparent()
		end)

		if not success then
			Arceus.Parent = game:GetService("Players").LocalPlayer.PlayerGui
		end

		local element_height = 50*Menu.AbsoluteSize.Y/210
		local elements = 0

		local function addSpace(parent)
			local space = tab:Clone()
			space.Parent = parent
			space.LayoutOrder = elements
			space.Visible = true

			elements += 1
		end

		local function addToggle(name, funct, enabled, ...)
			local newTog = Toggle:Clone()
			local args = {...}

			newTog.MouseButton1Click:Connect(function()
				enabled = not enabled
				newTog:WaitForChild("Enabled"):WaitForChild("Check").Visible = enabled
				funct(enabled, unpack(args))
			end)

			newTog:WaitForChild("Enabled"):WaitForChild("Check").Visible = enabled
			newTog:WaitForChild("Name").Text = name

			newTog.Size = UDim2.new(0.95, 0, 0, element_height) -- Y1 = 50 : Y2 = X
			newTog.Name = name
			newTog.Parent = Menu
			newTog.LayoutOrder = elements
			newTog.Visible = true

			elements += 1
			addSpace(Menu)

			return newTog
		end

		local function addButton(name, funct, ...)
			local newBut = Button:Clone()
			local args = {...}

			newBut.MouseButton1Click:Connect(function()
				funct(unpack(args))
			end)

			newBut:WaitForChild("Name").Text = name
			newBut.Size = UDim2.new(0.95, 0, 0, element_height)
			newBut.Name = name
			newBut.Parent = Menu
			newBut.LayoutOrder = elements
			newBut.Visible = true

			elements += 1
			addSpace(Menu)

			return newBut
		end

		local function addComboBox(text, options, funct, ...) -- ADD CUSTOM ELEMENT INSTEAD
			local newCombo = ComboBox:Clone()
			local enabled = false
			local elems = {}
			local args = {...}

			local function setBoxState()
				newCombo:WaitForChild("Img").Rotation = enabled and 0 or 180
				for _, elem in ipairs(elems) do
					elem.Visible = enabled
				end
			end

			newCombo.MouseButton1Click:Connect(function()
				enabled = not enabled
				setBoxState()
			end)

			newCombo:WaitForChild("Name").Text = text .. ": " .. (#options > 0 and options[1] or "")
			newCombo.Size = UDim2.new(0.95, 0, 0, element_height)
			newCombo.Name = #options > 0 and options[1] or ""
			newCombo.Parent = Menu
			newCombo.LayoutOrder = elements
			newCombo.Parent = Menu
			newCombo.Visible = true

			elements += 1
			addSpace(Menu)

			for _, name in ipairs(options) do
				local newElem = ComboElem:Clone()
				table.insert(elems, newElem)

				newElem.MouseButton1Click:Connect(function()
					newCombo:WaitForChild("Name").Text = text .. ": " .. name
					enabled = false
					setBoxState()

					funct(name, unpack(args))
				end)

				newElem:WaitForChild("Name").Text = name
				newElem.Size = UDim2.new(0.95, 0, 0, element_height)
				newElem.Name = name
				newElem.Parent = Menu
				newElem.LayoutOrder = elements
				newElem.Visible = false

				elements += 1
				addSpace(Menu)
			end

			return newCombo
		end

		-- Actual Script

		local runService = game:GetService("RunService")
		local plrsService = game:GetService("Players")
		local enabled = false
		local teamcheck = false
		local aimpart = "Head"

		function lookAt(target, eye)
			workspace.CurrentCamera.CFrame = CFrame.new(target, eye)
		end

		function getClosestPlayerToCursor(trg_part)
			local nearest = nil
			local last = math.huge

			for i, v in ipairs(plrsService:GetPlayers()) do
				if v ~= plrsService.LocalPlayer and plrsService.LocalPlayer.Character and plrsService.LocalPlayer.Character:FindFirstChildWhichIsA("Humanoid") and plrsService.LocalPlayer.Character:FindFirstChildWhichIsA("Humanoid").Health > 0
					and v.Character and v.Character:FindFirstChildWhichIsA("Humanoid") and v.Character:FindFirstChildWhichIsA("Humanoid").Health > 0
				then
					local allowed = not teamcheck
					if teamcheck and v.Team ~= plrsService.LocalPlayer.Team then
						allowed = true
					end

					if allowed then
						local aimobj = v.Character:FindFirstChild(trg_part) or v.Character:FindFirstChild("UpperTorso")
						if aimobj then
							if plrsService.LocalPlayer.Character:FindFirstChild("Head") then
								local ePos, vissss = workspace.CurrentCamera:WorldToViewportPoint(aimobj.Position)
								local AccPos = Vector2.new(ePos.x, ePos.y)
								local mousePos = Vector2.new(workspace.CurrentCamera.ViewportSize.x / 2, workspace.CurrentCamera.ViewportSize.y / 2)
								local distance = (AccPos - mousePos).magnitude
								if distance < last and vissss and distance < 400 then
									last = distance
									nearest = v
								end
							end
						end
					end
				end
			end
			return nearest
		end

		local toggleBtn
		toggleBtn = addToggle("Toggle aimbot", function(state)
			enabled = state
		end, false)

		local toggleTeamCheckBtn
		toggleTeamCheckBtn = addToggle("Team check", function(state)
			teamcheck = state
		end)

		local aimPartCombo
		aimPartCombo = addComboBox("Aim part", {"Head", "Torso"}, function(selection)
			aimpart = selection
		end)

		runService.RenderStepped:Connect(function()
			local closest = getClosestPlayerToCursor(aimpart)
			if enabled and closest then
				local aimobj = closest.Character:FindFirstChild(aimpart) or closest.Character:FindFirstChild("UpperTorso") -- If not found then should be R15 Torso
				if aimobj then
					lookAt(workspace.CurrentCamera.CFrame.p, aimobj.Position)
				end
			end
		end)

		-- INIT

		Main:TweenPosition(
			UDim2.fromScale(0.5, 0.5),
			Enum.EasingDirection.In,
			Enum.EasingStyle.Quad,
			1, true, nil
		)

		task.wait(1.5)
		Logo:TweenSizeAndPosition(
			UDim2.fromScale(0.175, 0.175),
			UDim2.fromScale(0.075, 0.15),
			Enum.EasingDirection.In,
			Enum.EasingStyle.Quad,
			1, true, nil
		)

		task.wait(1.5)
		TweenService:Create(Intro, TweenInfo.new(1, Enum.EasingStyle.Linear, Enum.EasingDirection.In), {BackgroundTransparency = 1}):Play()

	end    
})
Arceus:AddButton({
	Name = "Fly Arceus",
	Callback = function()
--[[
		MOBILE FLYING SCRIPTS
		Original: me_ozoneYT & Lucifear
		
		Remade and optimized by Riky47#3355 for Arceus X
		# spdmteam.com
		
		Edited and fixed by AZY#0348 for Fluxus / Hydrogen Compatibility
        # Chillz and Maik
]]

		local Script_Title = "Arceus X <font color=\"rgb(255, 0, 0)\">|</font> Mobile fly"


		-- Instances:
		local Arceus = Instance.new("ScreenGui")
		local Main = Instance.new("Frame")
		local UICorner = Instance.new("UICorner")
		local Intro = Instance.new("Frame")
		local UICorner_2 = Instance.new("UICorner")
		local Logo = Instance.new("ImageButton")
		local UIAspectRatioConstraint = Instance.new("UIAspectRatioConstraint")
		local Title = Instance.new("TextLabel")
		local Menu = Instance.new("ScrollingFrame")
		local UIListLayout = Instance.new("UIListLayout")
		local Toggle = Instance.new("ImageButton")
		local UICorner_3 = Instance.new("UICorner")
		local Enabled = Instance.new("Frame")
		local UIAspectRatioConstraint_2 = Instance.new("UIAspectRatioConstraint")
		local UICorner_4 = Instance.new("UICorner")
		local Check = Instance.new("Frame")
		local UIAspectRatioConstraint_3 = Instance.new("UIAspectRatioConstraint")
		local UICorner_5 = Instance.new("UICorner")
		local Name = Instance.new("TextLabel")
		local UIGradient = Instance.new("UIGradient")
		local Button = Instance.new("ImageButton")
		local UICorner_6 = Instance.new("UICorner")
		local Name_2 = Instance.new("TextLabel")
		local UIGradient_2 = Instance.new("UIGradient")
		local tab = Instance.new("Frame")
		local Close = Instance.new("TextButton")
		local ComboElem = Instance.new("ImageButton")
		local UICorner_7 = Instance.new("UICorner")
		local Name_3 = Instance.new("TextLabel")
		local UIGradient_3 = Instance.new("UIGradient")
		local Img = Instance.new("TextLabel")
		local UIAspectRatioConstraint_4 = Instance.new("UIAspectRatioConstraint")
		local ComboBox = Instance.new("ImageButton")
		local UICorner_8 = Instance.new("UICorner")
		local Name_4 = Instance.new("TextLabel")
		local UIGradient_4 = Instance.new("UIGradient")
		local Img_2 = Instance.new("TextLabel")
		local UIAspectRatioConstraint_5 = Instance.new("UIAspectRatioConstraint")

		--Properties:

		Arceus.Name = "Arceus"
		Arceus.Enabled = true
		Arceus.ResetOnSpawn = true
		Arceus.ZIndexBehavior = Enum.ZIndexBehavior.Sibling
		Arceus.DisplayOrder = 999999999

		Main.Name = "Main"
		Main.Parent = Arceus
		Main.Active = true
		Main.Draggable = true
		Main.AnchorPoint = Vector2.new(0.5, 0.5)
		Main.BackgroundColor3 = Color3.fromRGB(40, 40, 40)
		Main.BorderSizePixel = 0
		Main.Position = UDim2.new(0.5, 0, -0.2, 0) --UDim2.new(0.5, 0, 0.5, 0)
		Main.Size = UDim2.new(0.3, 0, 0.3, 0)

		UICorner.CornerRadius = UDim.new(0.1, 0)
		UICorner.Parent = Main

		Intro.Name = "Intro"
		Intro.Parent = Main
		Intro.BackgroundColor3 = Color3.fromRGB(40, 40, 40)
		Intro.ClipsDescendants = true
		Intro.Size = UDim2.new(1, 0, 1, 0)
		Intro.ZIndex = 2

		UICorner_2.CornerRadius = UDim.new(0.1, 0)
		UICorner_2.Parent = Intro

		Logo.Parent = Intro
		Logo.AnchorPoint = Vector2.new(0.5, 0.5)
		Logo.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
		Logo.BackgroundTransparency = 1
		Logo.BorderSizePixel = 0
		Logo.Position = UDim2.new(0.5, 0, 0.5, 0)
		Logo.Size = UDim2.new(0.75, 0, 0.75, 0)
		Logo.ZIndex = 2
		Logo.Image = "http://www.roblox.com/asset/?id=9178187770"
		Logo.ScaleType = Enum.ScaleType.Fit
		Logo.Active = false

		UIAspectRatioConstraint.Parent = Logo

		Title.Name = "Title"
		Title.Parent = Main
		Title.AnchorPoint = Vector2.new(1, 0)
		Title.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
		Title.BackgroundTransparency = 1
		Title.BorderSizePixel = 0
		Title.Position = UDim2.new(0.975, 0, 0.075, 0)
		Title.Size = UDim2.new(0.85, 0, 0.155, 0)
		Title.Font = Enum.Font.TitilliumWeb
		Title.FontFace = Font.new("rbxasset://fonts/families/TitilliumWeb.json", Enum.FontWeight.Bold)
		Title.RichText = true
		Title.Text = Script_Title
		Title.TextColor3 = Color3.fromRGB(255, 255, 255)
		Title.TextScaled = true
		Title.TextSize = 14
		Title.TextWrapped = true
		Title.TextXAlignment = Enum.TextXAlignment.Left
		Title.TextYAlignment = Enum.TextYAlignment.Center

		Menu.Name = "Menu"
		Menu.Parent = Main
		Menu.Active = true
		Menu.AnchorPoint = Vector2.new(0.5, 1)
		Menu.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
		Menu.BackgroundTransparency = 1
		Menu.AutomaticCanvasSize = Enum.AutomaticSize.Y
		Menu.BorderSizePixel = 0
		Menu.Position = UDim2.new(0.5, 0, 0.95, 0)
		Menu.Size = UDim2.new(0.95, 0, 0.65, 0)
		Menu.CanvasSize = UDim2.new(0, 0, 0, 0)
		Menu.ScrollBarImageColor3 = Color3.fromRGB(255, 255, 255)
		Menu.ScrollBarThickness = Menu.AbsoluteSize.X/25

		UIListLayout.Parent = Menu
		--UIListLayout.Padding = UDim.new(0.025, 0)
		UIListLayout.SortOrder = Enum.SortOrder.LayoutOrder

		Toggle.Name = "Toggle"
		Toggle.Visible = false
		--Toggle.Parent = Arceus
		Toggle.BackgroundColor3 = Color3.fromRGB(55, 55, 55)
		Toggle.Size = UDim2.new(0.95, 0, 0, 50)

		UICorner_3.CornerRadius = UDim.new(0.25, 0)
		UICorner_3.Parent = Toggle

		Enabled.Name = "Enabled"
		Enabled.Parent = Toggle
		Enabled.AnchorPoint = Vector2.new(1, 0.5)
		Enabled.BackgroundColor3 = Color3.fromRGB(50, 50, 50)
		Enabled.Position = UDim2.new(0.975, 0, 0.5, 0)
		Enabled.Size = UDim2.new(0.75, 0, 0.75, 0)

		UIAspectRatioConstraint_2.Parent = Enabled

		UICorner_4.CornerRadius = UDim.new(0.3, 0)
		UICorner_4.Parent = Enabled

		Check.Name = "Check"
		Check.Parent = Enabled
		Check.AnchorPoint = Vector2.new(0.5, 0.5)
		Check.BackgroundColor3 = Color3.fromRGB(255, 0, 0)
		Check.Position = UDim2.new(0.5, 0, 0.5, 0)
		Check.Size = UDim2.new(0.65, 0, 0.65, 0)

		UIAspectRatioConstraint_3.Parent = Check

		UICorner_5.CornerRadius = UDim.new(0.3, 0)
		UICorner_5.Parent = Check

		Name.Name = "Name"
		Name.Parent = Toggle
		Name.AnchorPoint = Vector2.new(0, 0.5)
		Name.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
		Name.BackgroundTransparency = 1
		Name.BorderSizePixel = 0
		Name.Position = UDim2.new(0.05, 0, 0.5, 0)
		Name.Size = UDim2.new(0.75, 0, 0.8, 0)
		Name.Font = Enum.Font.TitilliumWeb
		Name.Text = "Script"
		Name.TextColor3 = Color3.fromRGB(255, 255, 255)
		Name.TextScaled = true
		Name.TextSize = 14
		Name.TextWrapped = true
		Name.TextXAlignment = Enum.TextXAlignment.Left
		Name.TextYAlignment = Enum.TextYAlignment.Bottom

		UIGradient.Color = ColorSequence.new{ColorSequenceKeypoint.new(0.00, Color3.fromRGB(255, 255, 255)), ColorSequenceKeypoint.new(1.00, Color3.fromRGB(180, 180, 180))}
		UIGradient.Parent = Toggle

		Button.Name = "Button"
		--Button.Parent = Arceus
		Button.BackgroundColor3 = Color3.fromRGB(55, 55, 55)
		Button.Size = UDim2.new(0.95, 0, 0, 50)

		UICorner_6.CornerRadius = UDim.new(0.25, 0)
		UICorner_6.Parent = Button

		Name_2.Name = "Name"
		Name_2.Parent = Button
		Name_2.AnchorPoint = Vector2.new(0, 0.5)
		Name_2.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
		Name_2.BackgroundTransparency = 1
		Name_2.BorderSizePixel = 0
		Name_2.Position = UDim2.new(0.05, 0, 0.5, 0)
		Name_2.Size = UDim2.new(0.95, 0, 0.82, 0)
		Name_2.Font = Enum.Font.TitilliumWeb
		Name_2.Text = "Enabled"
		Name_2.TextColor3 = Color3.fromRGB(255, 255, 255)
		Name_2.TextScaled = true
		Name_2.TextSize = 14
		Name_2.TextWrapped = true
		Name_2.TextXAlignment = Enum.TextXAlignment.Left
		Name_2.TextYAlignment = Enum.TextYAlignment.Bottom

		UIGradient_2.Color = ColorSequence.new{ColorSequenceKeypoint.new(0.00, Color3.fromRGB(255, 255, 255)), ColorSequenceKeypoint.new(1.00, Color3.fromRGB(180, 180, 180))}
		UIGradient_2.Parent = Button

		tab.Name = "Tab"
		tab.Visible = false
		--tab.Parent = Arceus
		tab.BackgroundTransparency = 1
		tab.Size = UDim2.new(0.95, 0, 0.025, 0)

		Close.Name = "Close"
		Close.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
		Close.BackgroundTransparency = 1
		Close.BorderSizePixel = 0
		Close.Position = UDim2.new(0.8, 0, 0.1, 0)
		Close.Size = UDim2.new(0.15, 0, 0.125, 0)
		Close.Font = Enum.Font.FredokaOne
		Close.Text = "X"
		Close.TextColor3 = Color3.fromRGB(255, 0, 0)
		Close.TextScaled = true
		Close.TextSize = 14
		Close.TextWrapped = true
		Close.TextXAlignment = Enum.TextXAlignment.Right
		Close.Parent = Main

		ComboElem.Name = "ComboElem"
		ComboElem.BackgroundColor3 = Color3.fromRGB(55, 55, 55)
		ComboElem.Size = UDim2.new(0.95, 0, 0, 50)

		UICorner_7.CornerRadius = UDim.new(0.25, 0)
		UICorner_7.Parent = ComboElem

		Name_3.Name = "Name"
		Name_3.Parent = ComboElem
		Name_3.AnchorPoint = Vector2.new(0, 0.5)
		Name_3.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
		Name_3.BackgroundTransparency = 1
		Name_3.BorderSizePixel = 0
		Name_3.Position = UDim2.new(0.05, 0, 0.5, 0)
		Name_3.Size = UDim2.new(0.75, 0, 0.8, 0)
		Name_3.Font = Enum.Font.TitilliumWeb
		Name_3.Text = "Enabled"
		Name_3.TextColor3 = Color3.fromRGB(255, 0, 0)
		Name_3.TextScaled = true
		Name_3.TextSize = 14
		Name_3.TextWrapped = true
		Name_3.TextXAlignment = Enum.TextXAlignment.Left
		Name_3.TextYAlignment = Enum.TextYAlignment.Bottom

		UIGradient_3.Color = ColorSequence.new{ColorSequenceKeypoint.new(0.00, Color3.fromRGB(255, 255, 255)), ColorSequenceKeypoint.new(1.00, Color3.fromRGB(180, 180, 180))}
		UIGradient_3.Rotation = 180
		UIGradient_3.Parent = ComboElem

		Img.Name = "Img"
		Img.Parent = ComboElem
		Img.AnchorPoint = Vector2.new(1, 0.5)
		Img.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
		Img.BackgroundTransparency = 1
		Img.BorderSizePixel = 0
		Img.Position = UDim2.new(0.975, 0, 0.5, 0)
		Img.Rotation = 90
		Img.Size = UDim2.new(0.75, 0, 0.75, 0)
		Img.Font = Enum.Font.FredokaOne
		Img.Text = "^"
		Img.TextColor3 = Color3.fromRGB(255, 255, 255)
		Img.TextScaled = true
		Img.TextSize = 14
		Img.TextWrapped = true

		UIAspectRatioConstraint_4.Parent = Img

		ComboBox.Name = "ComboBox"
		ComboBox.BackgroundColor3 = Color3.fromRGB(55, 55, 55)
		ComboBox.Size = UDim2.new(0.95, 0, 0, 50)

		UICorner_8.CornerRadius = UDim.new(0.25, 0)
		UICorner_8.Parent = ComboBox

		Name_4.Name = "Name"
		Name_4.Parent = ComboBox
		Name_4.AnchorPoint = Vector2.new(0, 0.5)
		Name_4.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
		Name_4.BackgroundTransparency = 1.000
		Name_4.BorderSizePixel = 0
		Name_4.Position = UDim2.new(0.05, 0, 0.5, 0)
		Name_4.Size = UDim2.new(0.75, 0, 0.8, 0)
		Name_4.Font = Enum.Font.TitilliumWeb
		Name_4.Text = "Enabled"
		Name_4.TextColor3 = Color3.fromRGB(255, 255, 255)
		Name_4.TextScaled = true
		Name_4.TextSize = 14
		Name_4.TextWrapped = true
		Name_4.TextXAlignment = Enum.TextXAlignment.Left
		Name_4.TextYAlignment = Enum.TextYAlignment.Bottom

		UIGradient_4.Color = ColorSequence.new{ColorSequenceKeypoint.new(0.00, Color3.fromRGB(255, 255, 255)), ColorSequenceKeypoint.new(1.00, Color3.fromRGB(180, 180, 180))}
		UIGradient_4.Parent = ComboBox

		Img_2.Name = "Img"
		Img_2.Parent = ComboBox
		Img_2.AnchorPoint = Vector2.new(1, 0.5)
		Img_2.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
		Img_2.BackgroundTransparency = 1
		Img_2.BorderSizePixel = 0
		Img_2.Rotation = 180
		Img_2.Position = UDim2.new(0.975, 0, 0.5, 0)
		Img_2.Size = UDim2.new(0.75, 0, 0.75, 0)
		Img_2.Font = Enum.Font.FredokaOne
		Img_2.Text = "^"
		Img_2.TextColor3 = Color3.fromRGB(255, 0, 0)
		Img_2.TextScaled = true
		Img_2.TextSize = 14
		Img_2.TextWrapped = true

		UIAspectRatioConstraint_5.Parent = Img_2

		-- SCRIPT

		local TweenService = game:GetService("TweenService")
		Close.MouseButton1Click:Connect(function()
			Logo.Active = true
			TweenService:Create(Intro, TweenInfo.new(0.25, Enum.EasingStyle.Linear, Enum.EasingDirection.In), {BackgroundTransparency = 0}):Play()

			task.wait(0.3)
			Logo:TweenSizeAndPosition(
				UDim2.fromScale(0.75, 0.75),
				UDim2.fromScale(0.5, 0.5),
				Enum.EasingDirection.Out,
				Enum.EasingStyle.Quad,
				0.25, true, nil
			)

			task.wait(0.3)
			Main:TweenSize(
				UDim2.fromScale(0.1, 0.175),
				Enum.EasingDirection.Out,
				Enum.EasingStyle.Quad,
				0.25, true, nil
			)

			task.wait(0.3)
			for _, obj in pairs(Main:GetChildren()) do
				if obj:IsA("GuiObject") and obj ~= Intro then
					obj.Visible = false
				end
			end

			TweenService:Create(Logo, TweenInfo.new(0.25, Enum.EasingStyle.Linear, Enum.EasingDirection.In), {ImageTransparency = 0.8}):Play()
			TweenService:Create(Intro, TweenInfo.new(0.25, Enum.EasingStyle.Linear, Enum.EasingDirection.In), {BackgroundTransparency = 1}):Play()
			TweenService:Create(Main, TweenInfo.new(0.25, Enum.EasingStyle.Linear, Enum.EasingDirection.In), {BackgroundTransparency = 0.8}):Play()
		end)

		Logo.MouseButton1Click:Connect(function()
			Logo.Active = false
			TweenService:Create(Logo, TweenInfo.new(0.25, Enum.EasingStyle.Linear, Enum.EasingDirection.In), {ImageTransparency = 0}):Play()
			TweenService:Create(Intro, TweenInfo.new(0.25, Enum.EasingStyle.Linear, Enum.EasingDirection.In), {BackgroundTransparency = 0}):Play()
			TweenService:Create(Main, TweenInfo.new(0.25, Enum.EasingStyle.Linear, Enum.EasingDirection.In), {BackgroundTransparency = 0}):Play()

			task.wait(0.3)
			Main:TweenSize(
				UDim2.fromScale(0.3, 0.3),
				Enum.EasingDirection.Out,
				Enum.EasingStyle.Quad,
				0.25, true, nil
			)

			task.wait(0.3)
			Logo:TweenSizeAndPosition(
				UDim2.fromScale(0.175, 0.175),
				UDim2.fromScale(0.075, 0.15),
				Enum.EasingDirection.Out,
				Enum.EasingStyle.Quad,
				0.25, true, nil
			)

			for _, obj in pairs(Main:GetChildren()) do
				if obj:IsA("GuiObject") and obj ~= Intro then
					obj.Visible = true
				end
			end

			task.wait(0.3)
			TweenService:Create(Intro, TweenInfo.new(0.25, Enum.EasingStyle.Linear, Enum.EasingDirection.In), {BackgroundTransparency = 1}):Play()
		end)

		local function uiparent()
			local success, parent = pcall(function()
				return gethui()
			end)

			if not success then
				return game:GetService("CoreGui")
			end

			return parent
		end

		local success, err = pcall(function()
			Arceus.Parent = uiparent()
		end)

		if not success then
			Arceus.Parent = game:GetService("Players").LocalPlayer.PlayerGui
		end

		local element_height = 50*Menu.AbsoluteSize.Y/210
		local elements = 0

		local function addSpace(parent)
			local space = tab:Clone()
			space.Parent = parent
			space.LayoutOrder = elements
			space.Visible = true

			elements += 1
		end

		local function addToggle(name, funct, enabled, ...)
			local newTog = Toggle:Clone()
			local args = {...}

			newTog.MouseButton1Click:Connect(function()
				enabled = not enabled
				newTog:WaitForChild("Enabled"):WaitForChild("Check").Visible = enabled
				funct(enabled, unpack(args))
			end)

			newTog:WaitForChild("Enabled"):WaitForChild("Check").Visible = enabled
			newTog:WaitForChild("Name").Text = name

			newTog.Size = UDim2.new(0.95, 0, 0, element_height) -- Y1 = 50 : Y2 = X
			newTog.Name = name
			newTog.Parent = Menu
			newTog.LayoutOrder = elements
			newTog.Visible = true

			elements += 1
			addSpace(Menu)

			return newTog
		end

		local function addButton(name, funct, ...)
			local newBut = Button:Clone()
			local args = {...}

			newBut.MouseButton1Click:Connect(function()
				funct(unpack(args))
			end)

			newBut:WaitForChild("Name").Text = name
			newBut.Size = UDim2.new(0.95, 0, 0, element_height)
			newBut.Name = name
			newBut.Parent = Menu
			newBut.LayoutOrder = elements
			newBut.Visible = true

			elements += 1
			addSpace(Menu)

			return newBut
		end

		local function addComboBox(text, options, funct, ...) -- ADD CUSTOM ELEMENT INSTEAD
			local newCombo = ComboBox:Clone()
			local enabled = false
			local elems = {}
			local args = {...}

			local function setBoxState()
				newCombo:WaitForChild("Img").Rotation = enabled and 0 or 180
				for _, elem in ipairs(elems) do
					elem.Visible = enabled
				end
			end

			newCombo.MouseButton1Click:Connect(function()
				enabled = not enabled
				setBoxState()
			end)

			newCombo:WaitForChild("Name").Text = text .. ": " .. (#options > 0 and options[1] or "")
			newCombo.Size = UDim2.new(0.95, 0, 0, element_height)
			newCombo.Name = #options > 0 and options[1] or ""
			newCombo.Parent = Menu
			newCombo.LayoutOrder = elements
			newCombo.Parent = Menu
			newCombo.Visible = true

			elements += 1
			addSpace(Menu)

			for _, name in ipairs(options) do
				local newElem = ComboElem:Clone()
				table.insert(elems, newElem)

				newElem.MouseButton1Click:Connect(function()
					newCombo:WaitForChild("Name").Text = text .. ": " .. name
					enabled = false
					setBoxState()

					funct(name, unpack(args))
				end)

				newElem:WaitForChild("Name").Text = name
				newElem.Size = UDim2.new(0.95, 0, 0, element_height)
				newElem.Name = name
				newElem.Parent = Menu
				newElem.LayoutOrder = elements
				newElem.Visible = false

				elements += 1
				addSpace(Menu)
			end

			return newCombo
		end

		-- Actual Script

		local speeds = 5
		local nowe = false
		local tpwalking = false
		local speaker = game:GetService("Players").LocalPlayer
		local heartbeat = game:GetService("RunService").Heartbeat

		local function updatespeed(char, hum)
			if nowe == true then
				tpwalking = false
				heartbeat:Wait()
				task.wait(.1)
				heartbeat:Wait() -- Make sure old threads are terminated

				for i = 1, speeds do
					spawn(function()
						tpwalking = true

						while tpwalking and heartbeat:Wait() and char and hum and hum.Parent do
							if hum.MoveDirection.Magnitude > 0 then
								char:TranslateBy(hum.MoveDirection)
							end
						end
					end)
				end
			end
		end

		speaker.CharacterAdded:Connect(function(char)
			local char = speaker.Character
			if char then
				task.wait(0.7)
				char.Humanoid.PlatformStand = false
				char.Animate.Disabled = false
			end
		end)

		local toggleBtn
		toggleBtn = addToggle("Toggle fly: " .. speeds, function(enabled)
			local char = speaker.Character
			if not char or not char.Humanoid then
				return
			end

			local hum = char.Humanoid
			if nowe == true then
				nowe = false

				hum:SetStateEnabled(Enum.HumanoidStateType.Climbing,true)
				hum:SetStateEnabled(Enum.HumanoidStateType.FallingDown,true)
				hum:SetStateEnabled(Enum.HumanoidStateType.Flying,true)
				hum:SetStateEnabled(Enum.HumanoidStateType.Freefall,true)
				hum:SetStateEnabled(Enum.HumanoidStateType.GettingUp,true)
				hum:SetStateEnabled(Enum.HumanoidStateType.Jumping,true)
				hum:SetStateEnabled(Enum.HumanoidStateType.Landed,true)
				hum:SetStateEnabled(Enum.HumanoidStateType.Physics,true)
				hum:SetStateEnabled(Enum.HumanoidStateType.PlatformStanding,true)
				hum:SetStateEnabled(Enum.HumanoidStateType.Ragdoll,true)
				hum:SetStateEnabled(Enum.HumanoidStateType.Running,true)
				hum:SetStateEnabled(Enum.HumanoidStateType.RunningNoPhysics,true)
				hum:SetStateEnabled(Enum.HumanoidStateType.Seated,true)
				hum:SetStateEnabled(Enum.HumanoidStateType.StrafingNoPhysics,true)
				hum:SetStateEnabled(Enum.HumanoidStateType.Swimming,true)
				hum:ChangeState(Enum.HumanoidStateType.RunningNoPhysics)	
			else
				nowe = true
				updatespeed(char, hum)

				char.Animate.Disabled = true
				for i,v in next, hum:GetPlayingAnimationTracks() do
					v:AdjustSpeed(0)
				end

				hum:SetStateEnabled(Enum.HumanoidStateType.Climbing,false)
				hum:SetStateEnabled(Enum.HumanoidStateType.FallingDown,false)
				hum:SetStateEnabled(Enum.HumanoidStateType.Flying,false)
				hum:SetStateEnabled(Enum.HumanoidStateType.Freefall,false)
				hum:SetStateEnabled(Enum.HumanoidStateType.GettingUp,false)
				hum:SetStateEnabled(Enum.HumanoidStateType.Jumping,false)
				hum:SetStateEnabled(Enum.HumanoidStateType.Landed,false)
				hum:SetStateEnabled(Enum.HumanoidStateType.Physics,false)
				hum:SetStateEnabled(Enum.HumanoidStateType.PlatformStanding,false)
				hum:SetStateEnabled(Enum.HumanoidStateType.Ragdoll,false)
				hum:SetStateEnabled(Enum.HumanoidStateType.Running,false)
				hum:SetStateEnabled(Enum.HumanoidStateType.RunningNoPhysics,false)
				hum:SetStateEnabled(Enum.HumanoidStateType.Seated,false)
				hum:SetStateEnabled(Enum.HumanoidStateType.StrafingNoPhysics,false)
				hum:SetStateEnabled(Enum.HumanoidStateType.Swimming,false)
				hum:ChangeState(Enum.HumanoidStateType.Swimming)
			end

			local function CheckRig()
				if speaker.Character and speaker.Character:FindFirstChild("Torso") then
					return speaker.Character.Torso
				elseif speaker.Character and speaker.Character:FindFirstChild("LowerTorso") then
					return speaker.Character.LowerTorso
				end
			end


			local UpperTorso = CheckRig()
			local flying = true
			local deb = true
			local ctrl = {f = 0, b = 0, l = 0, r = 0}
			local lastctrl = {f = 0, b = 0, l = 0, r = 0}
			local maxspeed = 50
			local speed = 0

			local bg = Instance.new("BodyGyro", UpperTorso)
			bg.P = 9e4
			bg.maxTorque = Vector3.new(9e9, 9e9, 9e9)
			bg.cframe = UpperTorso.CFrame

			local bv = Instance.new("BodyVelocity", UpperTorso)
			bv.velocity = Vector3.new(0,0.1,0)
			bv.maxForce = Vector3.new(9e9, 9e9, 9e9)

			if nowe == true then
				hum.PlatformStand = true
			end

			while nowe == true or hum.Health == 0 do
				task.wait()

				if ctrl.l + ctrl.r ~= 0 or ctrl.f + ctrl.b ~= 0 then
					speed = speed+.5+(speed/maxspeed)
					if speed > maxspeed then
						speed = maxspeed
					end
				elseif not (ctrl.l + ctrl.r ~= 0 or ctrl.f + ctrl.b ~= 0) and speed ~= 0 then
					speed = speed-1
					if speed < 0 then
						speed = 0
					end
				end
				if (ctrl.l + ctrl.r) ~= 0 or (ctrl.f + ctrl.b) ~= 0 then
					bv.velocity = ((game.Workspace.CurrentCamera.CoordinateFrame.lookVector * (ctrl.f+ctrl.b)) + ((game.Workspace.CurrentCamera.CoordinateFrame * CFrame.new(ctrl.l+ctrl.r,(ctrl.f+ctrl.b)*.2,0).p) - game.Workspace.CurrentCamera.CoordinateFrame.p))*speed
					lastctrl = {f = ctrl.f, b = ctrl.b, l = ctrl.l, r = ctrl.r}
				elseif (ctrl.l + ctrl.r) == 0 and (ctrl.f + ctrl.b) == 0 and speed ~= 0 then
					bv.velocity = ((game.Workspace.CurrentCamera.CoordinateFrame.lookVector * (lastctrl.f+lastctrl.b)) + ((game.Workspace.CurrentCamera.CoordinateFrame * CFrame.new(lastctrl.l+lastctrl.r,(lastctrl.f+lastctrl.b)*.2,0).p) - game.Workspace.CurrentCamera.CoordinateFrame.p))*speed
				else
					bv.velocity = Vector3.new(0,0,0)
				end

				bg.cframe = game.Workspace.CurrentCamera.CoordinateFrame * CFrame.Angles(-math.rad((ctrl.f+ctrl.b)*50*speed/maxspeed),0,0)
			end

			ctrl = {f = 0, b = 0, l = 0, r = 0}
			lastctrl = {f = 0, b = 0, l = 0, r = 0}
			speed = 0
			bg:Destroy()
			bv:Destroy()

			hum.PlatformStand = false
			char.Animate.Disabled = false
			tpwalking = false
		end, false)

		local incraseBtn
		incraseBtn = addButton("Incrase speed", function()
			local char = speaker.Character
			if char and char.Humanoid then
				local hum = char.Humanoid

				speeds = speeds + 1
				updatespeed(char, hum)

				toggleBtn:WaitForChild("Name").Text = "Toggle fly: " .. speeds
			end
		end)

		local decraseBtn
		decraseBtn = addButton("Decrase speed", function()
			local char = speaker.Character
			if char and char.Humanoid then
				local hum = char.Humanoid

				if speeds > 1 then
					speeds = speeds - 1
					updatespeed(char, hum)
				end

				toggleBtn:WaitForChild("Name").Text = "Toggle fly: " .. speeds
			end
		end)

		local goUp
		goUp = addButton("Go up", function()
			local char = speaker.Character
			if char then
				char.HumanoidRootPart.CFrame = char.HumanoidRootPart.CFrame * CFrame.new(0,2,0)
			end
		end)

		local goDown
		goDown = addButton("Go down", function()
			local char = speaker.Character
			if char then
				char.HumanoidRootPart.CFrame = char.HumanoidRootPart.CFrame * CFrame.new(0,-2,0)
			end
		end)

		-- INIT

		Main:TweenPosition(
			UDim2.fromScale(0.5, 0.5),
			Enum.EasingDirection.In,
			Enum.EasingStyle.Quad,
			1, true, nil
		)

		task.wait(1.5)
		Logo:TweenSizeAndPosition(
			UDim2.fromScale(0.175, 0.175),
			UDim2.fromScale(0.075, 0.15),
			Enum.EasingDirection.In,
			Enum.EasingStyle.Quad,
			1, true, nil
		)

		task.wait(1.5)
		TweenService:Create(Intro, TweenInfo.new(1, Enum.EasingStyle.Linear, Enum.EasingDirection.In), {BackgroundTransparency = 1}):Play()

	end    
})
Arceus:AddButton({
	Name = "Arceus",
	Callback = function()
--[=[

    ___      _  _     __     _         _         ____   
  ,"___".   FJ  L]    FJ    FJ        FJ        [__  '. 
  FJ---L]  J |__| L  J  L  J |       J |        `--7 .' 
 J |   LJ  |  __  |  |  |  | |       | |         .'.'.' 
 | \___--. F L__J J  F  J  F L_____  F L_____  .' (_(__ 
 J\_____/FJ__L  J__LJ____LJ________LJ________LJ________L
  J_____F |__L  J__||____||________||________||________|
                                                        
 
]=]

		--Huge thanks for Bread for good textbox and remake the sliders :D
		--GuiToLua By Creator of Backdoor.exe

		-- Arceus X v3 Remake
		local AZY = {};

		-- StarterGui.ArceusXV3
		AZY["1"] = Instance.new("ScreenGui", game.CoreGui);
		AZY["1"]["Name"] = [[ArceusXV3]];
		AZY["1"]["ZIndexBehavior"] = Enum.ZIndexBehavior.Sibling;
		AZY["1"]["ResetOnSpawn"] = false;

		-- StarterGui.ArceusXV3.Welcome
		AZY["2"] = Instance.new("Folder", AZY["1"]);
		AZY["2"]["Name"] = [[Welcome]];

		-- StarterGui.ArceusXV3.Welcome.Frame
		AZY["3"] = Instance.new("Frame", AZY["2"]);
		AZY["3"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["3"]["BackgroundTransparency"] = 0.699999988079071;
		AZY["3"]["Size"] = UDim2.new(100.58300018310547, 0, 10.576000213623047, 0);
		AZY["3"]["BorderColor3"] = Color3.fromRGB(28, 43, 54);
		AZY["3"]["Position"] = UDim2.new(-0.012608751654624939, 0, -1.0678343772888184, 0);

		-- StarterGui.ArceusXV3.Welcome.Frame.UIAspectRatioConstraint
		AZY["4"] = Instance.new("UIAspectRatioConstraint", AZY["3"]);
		AZY["4"]["AspectRatio"] = 2.0052521228790283;

		-- StarterGui.ArceusXV3.Welcome.Welcome
		AZY["5"] = Instance.new("Frame", AZY["2"]);
		AZY["5"]["BackgroundColor3"] = Color3.fromRGB(52, 52, 52);
		AZY["5"]["Size"] = UDim2.new(0.666020393371582, 0, 0.8211921453475952, 0);
		AZY["5"]["Position"] = UDim2.new(0.17622511088848114, 0, 0.0894039198756218, 0);
		AZY["5"]["Name"] = [[Welcome]];

		-- StarterGui.ArceusXV3.Welcome.Welcome.UIAspectRatioConstraint
		AZY["6"] = Instance.new("UIAspectRatioConstraint", AZY["5"]);
		AZY["6"]["AspectRatio"] = 1.6193960905075073;

		-- StarterGui.ArceusXV3.Welcome.Welcome.ScrollingFrame
		AZY["7"] = Instance.new("ScrollingFrame", AZY["5"]);
		AZY["7"]["Active"] = true;
		AZY["7"]["CanvasSize"] = UDim2.new(0, 0, 1.2000000476837158, 0);
		AZY["7"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["7"]["BackgroundTransparency"] = 1;
		AZY["7"]["Size"] = UDim2.new(1.0180450677871704, 0, 1, 0);
		AZY["7"]["ScrollBarImageColor3"] = Color3.fromRGB(0, 0, 0);
		AZY["7"]["BorderColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["7"]["ScrollBarThickness"] = 7;

		-- StarterGui.ArceusXV3.Welcome.Welcome.ScrollingFrame.Text
		AZY["8"] = Instance.new("TextLabel", AZY["7"]);
		AZY["8"]["TextWrapped"] = true;
		AZY["8"]["TextYAlignment"] = Enum.TextYAlignment.Top;
		AZY["8"]["TextScaled"] = true;
		AZY["8"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["8"]["TextXAlignment"] = Enum.TextXAlignment.Left;
		AZY["8"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Regular, Enum.FontStyle.Normal);
		AZY["8"]["TextSize"] = 29;
		AZY["8"]["TextColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["8"]["Size"] = UDim2.new(0.8902860283851624, 0, 0.6482642889022827, 0);
		AZY["8"]["Text"] = [[Dear User,

We are writing to welcome you as one of you first bete testers of Arceus X!
We are thrilled to have your collaboration and to offer you the oppoturnity
to try out the new features we are developing.

We are confident that your experience and creativity will help us make
Arceus X an even more effective and user-friendly application.
Please feel free to share any feedback and suggestion that can help us further
improve our platform.

Thank you so much your support, and we look forward to working with
you in this exciting journey!

Best regards,
SPDM Team]];
		AZY["8"]["Name"] = [[Text]];
		AZY["8"]["BackgroundTransparency"] = 1;
		AZY["8"]["Position"] = UDim2.new(0.04280221089720726, 0, 0.14032021164894104, 0);

		-- StarterGui.ArceusXV3.Welcome.Welcome.ScrollingFrame.Text.LocalScript
		AZY["9"] = Instance.new("LocalScript", AZY["8"]);


		-- StarterGui.ArceusXV3.Welcome.Welcome.ScrollingFrame.TextButton
		AZY["a"] = Instance.new("TextButton", AZY["7"]);
		AZY["a"]["TextWrapped"] = true;
		AZY["a"]["TextScaled"] = true;
		AZY["a"]["BackgroundColor3"] = Color3.fromRGB(255, 0, 0);
		AZY["a"]["TextSize"] = 24;
		AZY["a"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Bold, Enum.FontStyle.Normal);
		AZY["a"]["TextColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["a"]["Size"] = UDim2.new(0.2372465580701828, 0, 0.10296772420406342, 0);
		AZY["a"]["Text"] = [[Get started]];
		AZY["a"]["Position"] = UDim2.new(0.3705448806285858, 0, 0.8786289095878601, 0);

		-- StarterGui.ArceusXV3.Welcome.Welcome.ScrollingFrame.TextButton.UICorner
		AZY["b"] = Instance.new("UICorner", AZY["a"]);
		AZY["b"]["CornerRadius"] = UDim.new(0, 12);

		-- StarterGui.ArceusXV3.Welcome.Welcome.ScrollingFrame.TextButton.UITextSizeConstraint
		AZY["c"] = Instance.new("UITextSizeConstraint", AZY["a"]);
		AZY["c"]["MaxTextSize"] = 24;

		-- StarterGui.ArceusXV3.Welcome.Welcome.ScrollingFrame.TextButton.LocalScriptNew
		AZY["d"] = Instance.new("LocalScript", AZY["a"]);
		AZY["d"]["Name"] = [[LocalScriptNew]];

		-- StarterGui.ArceusXV3.Welcome.Welcome.ScrollingFrame.Title
		AZY["e"] = Instance.new("TextLabel", AZY["7"]);
		AZY["e"]["TextWrapped"] = true;
		AZY["e"]["TextScaled"] = true;
		AZY["e"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["e"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Bold, Enum.FontStyle.Normal);
		AZY["e"]["TextSize"] = 45;
		AZY["e"]["TextColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["e"]["Size"] = UDim2.new(0.624912440776825, 0, 0.12905988097190857, 0);
		AZY["e"]["Text"] = [[Welcome to Arceus X 3.0!]];
		AZY["e"]["Name"] = [[Title]];
		AZY["e"]["BackgroundTransparency"] = 1;
		AZY["e"]["Position"] = UDim2.new(0.1773233860731125, 0, 0.011320043355226517, 0);

		-- StarterGui.ArceusXV3.Welcome.Welcome.ScrollingFrame.Title.UITextSizeConstraint
		AZY["f"] = Instance.new("UITextSizeConstraint", AZY["e"]);
		AZY["f"]["MaxTextSize"] = 45;

		-- StarterGui.ArceusXV3.Welcome.Welcome.UICorner
		AZY["10"] = Instance.new("UICorner", AZY["5"]);
		AZY["10"]["CornerRadius"] = UDim.new(0, 40);

		-- StarterGui.ArceusXV3.AnimationIntro
		AZY["11"] = Instance.new("Folder", AZY["1"]);
		AZY["11"]["Name"] = [[AnimationIntro]];

		-- StarterGui.ArceusXV3.AnimationIntro.Background
		AZY["12"] = Instance.new("Frame", AZY["11"]);
		AZY["12"]["BackgroundColor3"] = Color3.fromRGB(28, 28, 28);
		AZY["12"]["Size"] = UDim2.new(0, 1806, 0, 1604);
		AZY["12"]["Position"] = UDim2.new(-0.11024535447359085, 0, -0.16887417435646057, 0);
		AZY["12"]["Visible"] = false;
		AZY["12"]["Name"] = [[Background]];

		-- StarterGui.ArceusXV3.AnimationIntro.Frame
		AZY["13"] = Instance.new("Frame", AZY["11"]);
		AZY["13"]["BackgroundColor3"] = Color3.fromRGB(255, 0, 0);
		AZY["13"]["Size"] = UDim2.new(0.03313452750444412, 0, 0.06622516363859177, 0);
		AZY["13"]["Position"] = UDim2.new(0.48293575644493103, 0, 0.4668874144554138, 0);
		AZY["13"]["Visible"] = false;

		-- StarterGui.ArceusXV3.AnimationIntro.Frame.UICorner
		AZY["14"] = Instance.new("UICorner", AZY["13"]);
		AZY["14"]["CornerRadius"] = UDim.new(1, 100);

		-- StarterGui.ArceusXV3.AnimationIntro.ImageLabel
		AZY["15"] = Instance.new("ImageLabel", AZY["11"]);
		AZY["15"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["15"]["ImageTransparency"] = 1;
		AZY["15"]["Visible"] = false;
		AZY["15"]["Image"] = [[rbxassetid://12564267060]];
		AZY["15"]["Size"] = UDim2.new(0.09526176750659943, 0, 0.27649006247520447, 0);
		AZY["15"]["BackgroundTransparency"] = 1;
		AZY["15"]["Position"] = UDim2.new(0.4423459470272064, 0, 0.36092716455459595, 0);

		-- StarterGui.ArceusXV3.AnimationIntro.NameLogo
		AZY["16"] = Instance.new("TextLabel", AZY["11"]);
		AZY["16"]["TextWrapped"] = true;
		AZY["16"]["TextScaled"] = true;
		AZY["16"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["16"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Bold, Enum.FontStyle.Normal);
		AZY["16"]["TextTransparency"] = 1;
		AZY["16"]["TextSize"] = 50;
		AZY["16"]["TextColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["16"]["Size"] = UDim2.new(0.13893571496009827, 0, 0.09271523356437683, 0);
		AZY["16"]["Text"] = [[Arceus X]];
		AZY["16"]["Name"] = [[NameLogo]];
		AZY["16"]["Visible"] = false;
		AZY["16"]["BackgroundTransparency"] = 1;
		AZY["16"]["Position"] = UDim2.new(0.3928734362125397, 0, 0.4523245096206665, 0);

		-- StarterGui.ArceusXV3.AnimationIntro.NameLogo.UITextSizeConstraint
		AZY["17"] = Instance.new("UITextSizeConstraint", AZY["16"]);
		AZY["17"]["MaxTextSize"] = 50;

		-- StarterGui.ArceusXV3.MainUI
		AZY["18"] = Instance.new("Folder", AZY["1"]);
		AZY["18"]["Name"] = [[MainUI]];

		-- StarterGui.ArceusXV3.MainUI.MainFrame
		AZY["19"] = Instance.new("Frame", AZY["18"]);
		AZY["19"]["BackgroundColor3"] = Color3.fromRGB(0, 0, 0);
		AZY["19"]["BackgroundTransparency"] = 0.44999998807907104;
		AZY["19"]["Size"] = UDim2.new(0, 459, 0, 276);
		AZY["19"]["Position"] = UDim2.new(0.1498919129371643, 0, 0.12086091935634613, 0);
		AZY["19"]["Visible"] = false;
		AZY["19"]["Name"] = [[MainFrame]];

		-- StarterGui.ArceusXV3.MainUI.MainFrame.UICorner
		AZY["1a"] = Instance.new("UICorner", AZY["19"]);
		AZY["1a"]["CornerRadius"] = UDim.new(0, 15);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Panel
		AZY["1b"] = Instance.new("Frame", AZY["19"]);
		AZY["1b"]["BackgroundColor3"] = Color3.fromRGB(0, 0, 0);
		AZY["1b"]["BackgroundTransparency"] = 0.550000011920929;
		AZY["1b"]["Size"] = UDim2.new(0.9417322874069214, 0, 0.11706378310918808, 0);
		AZY["1b"]["Position"] = UDim2.new(0.03099355846643448, 0, 0.0474083386361599, 0);
		AZY["1b"]["Name"] = [[Panel]];

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Panel.UICorner
		AZY["1c"] = Instance.new("UICorner", AZY["1b"]);
		AZY["1c"]["CornerRadius"] = UDim.new(0, 14);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Panel.Logo
		AZY["1d"] = Instance.new("ImageLabel", AZY["1b"]);
		AZY["1d"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["1d"]["Image"] = [[rbxassetid://12564267060]];
		AZY["1d"]["Size"] = UDim2.new(0.05029655620455742, 0, 0.9125484824180603, 0);
		AZY["1d"]["Name"] = [[Logo]];
		AZY["1d"]["BackgroundTransparency"] = 1;
		AZY["1d"]["Position"] = UDim2.new(0.4099465012550354, 0, 0.03155198320746422, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Panel.TextLogo
		AZY["1e"] = Instance.new("TextLabel", AZY["1b"]);
		AZY["1e"]["TextWrapped"] = true;
		AZY["1e"]["TextScaled"] = true;
		AZY["1e"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["1e"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Bold, Enum.FontStyle.Normal);
		AZY["1e"]["TextSize"] = 85;
		AZY["1e"]["TextColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["1e"]["Size"] = UDim2.new(0.1371736377477646, 0, 0.6307170391082764, 0);
		AZY["1e"]["Text"] = [[Arceus X]];
		AZY["1e"]["Name"] = [[TextLogo]];
		AZY["1e"]["BackgroundTransparency"] = 1;
		AZY["1e"]["Position"] = UDim2.new(0.4679349362850189, 0, 0.16660596430301666, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Panel.TextLogo.UITextSizeConstraint
		AZY["1f"] = Instance.new("UITextSizeConstraint", AZY["1e"]);
		AZY["1f"]["MaxTextSize"] = 25;

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Panel.Close
		AZY["20"] = Instance.new("ImageButton", AZY["1b"]);
		AZY["20"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["20"]["Image"] = [[rbxassetid://12566509152]];
		AZY["20"]["Size"] = UDim2.new(0.06670181453227997, 0, 1, 0);
		AZY["20"]["Name"] = [[Close]];
		AZY["20"]["Position"] = UDim2.new(0.9171510338783264, 0, 0, 0);
		AZY["20"]["BackgroundTransparency"] = 1;

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Panel.Close.LocalScript
		AZY["21"] = Instance.new("LocalScript", AZY["20"]);


		-- StarterGui.ArceusXV3.MainUI.MainFrame.Panel.Expand
		AZY["22"] = Instance.new("ImageButton", AZY["1b"]);
		AZY["22"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["22"]["Image"] = [[rbxassetid://12566545357]];
		AZY["22"]["Size"] = UDim2.new(0.06901533156633377, 0, 1, 0);
		AZY["22"]["Name"] = [[Expand]];
		AZY["22"]["Position"] = UDim2.new(0.8481356501579285, 0, -0.024522678926587105, 0);
		AZY["22"]["BackgroundTransparency"] = 1;

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Panel.Expand.LocalScript
		AZY["23"] = Instance.new("LocalScript", AZY["22"]);


		-- StarterGui.ArceusXV3.MainUI.MainFrame.Panel.TimeLeft
		AZY["24"] = Instance.new("TextLabel", AZY["1b"]);
		AZY["24"]["TextWrapped"] = true;
		AZY["24"]["TextScaled"] = true;
		AZY["24"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["24"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Regular, Enum.FontStyle.Normal);
		AZY["24"]["TextSize"] = 35;
		AZY["24"]["TextColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["24"]["Size"] = UDim2.new(0.13600000739097595, 0, 0.38600000739097595, 0);
		AZY["24"]["Text"] = [[24h 00m left]];
		AZY["24"]["Name"] = [[TimeLeft]];
		AZY["24"]["BackgroundTransparency"] = 1;
		AZY["24"]["Position"] = UDim2.new(0.07365596294403076, 0, 0.28405851125717163, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Panel.TimeLeft.LocalScript
		AZY["25"] = Instance.new("LocalScript", AZY["24"]);


		-- StarterGui.ArceusXV3.MainUI.MainFrame.Panel.Restore
		AZY["26"] = Instance.new("TextButton", AZY["1b"]);
		AZY["26"]["TextWrapped"] = true;
		AZY["26"]["BackgroundColor3"] = Color3.fromRGB(255, 0, 0);
		AZY["26"]["TextSize"] = 12;
		AZY["26"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Bold, Enum.FontStyle.Normal);
		AZY["26"]["TextColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["26"]["Size"] = UDim2.new(0.10400000214576721, 0, 0.503000020980835, 0);
		AZY["26"]["Name"] = [[Restore]];
		AZY["26"]["Text"] = [[Restore]];
		AZY["26"]["Position"] = UDim2.new(0.21463949978351593, 0, 0.22850705683231354, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Panel.Restore.UICorner
		AZY["27"] = Instance.new("UICorner", AZY["26"]);
		AZY["27"]["CornerRadius"] = UDim.new(0, 6);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Panel.Restore.LocalScript
		AZY["28"] = Instance.new("LocalScript", AZY["26"]);


		-- StarterGui.ArceusXV3.MainUI.MainFrame.Panel.Icon
		AZY["29"] = Instance.new("ImageButton", AZY["1b"]);
		AZY["29"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["29"]["Image"] = [[rbxassetid://12584810787]];
		AZY["29"]["Size"] = UDim2.new(0.05783621221780777, 0, 0.7737637162208557, 0);
		AZY["29"]["Name"] = [[Icon]];
		AZY["29"]["Position"] = UDim2.new(0.01600000075995922, 0, 0.09300000220537186, 0);
		AZY["29"]["BackgroundTransparency"] = 1;

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Panel.Icon.LocalScript
		AZY["2a"] = Instance.new("LocalScript", AZY["29"]);


		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs
		AZY["2b"] = Instance.new("Folder", AZY["19"]);
		AZY["2b"]["Name"] = [[Tabs]];

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home
		AZY["2c"] = Instance.new("Frame", AZY["2b"]);
		AZY["2c"]["BackgroundColor3"] = Color3.fromRGB(0, 0, 0);
		AZY["2c"]["BackgroundTransparency"] = 1;
		AZY["2c"]["Size"] = UDim2.new(0.831805408000946, 0, 0.7336452603340149, 0);
		AZY["2c"]["Position"] = UDim2.new(0.1409204602241516, 0, 0.18711426854133606, 0);
		AZY["2c"]["Name"] = [[Home]];

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.UserPage
		AZY["2d"] = Instance.new("Frame", AZY["2c"]);
		AZY["2d"]["BackgroundColor3"] = Color3.fromRGB(0, 0, 0);
		AZY["2d"]["BackgroundTransparency"] = 0.550000011920929;
		AZY["2d"]["Size"] = UDim2.new(0.37270405888557434, 0, 0.2492256611585617, 0);
		AZY["2d"]["Position"] = UDim2.new(-0.0007835610886104405, 0, 0.025084324181079865, 0);
		AZY["2d"]["Name"] = [[UserPage]];

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.UserPage.UICorner
		AZY["2e"] = Instance.new("UICorner", AZY["2d"]);
		AZY["2e"]["CornerRadius"] = UDim.new(0, 15);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.UserPage.ImageLabel
		AZY["2f"] = Instance.new("ImageLabel", AZY["2d"]);
		AZY["2f"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["2f"]["Image"] = [[rbxassetid://12566434374]];
		AZY["2f"]["Size"] = UDim2.new(0.3031076192855835, 0, 0.8659517168998718, 0);
		AZY["2f"]["BackgroundTransparency"] = 1;
		AZY["2f"]["Position"] = UDim2.new(0.22370131313800812, 0, 0.0670241266489029, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.UserPage.TextLabel
		AZY["30"] = Instance.new("TextLabel", AZY["2d"]);
		AZY["30"]["TextWrapped"] = true;
		AZY["30"]["TextScaled"] = true;
		AZY["30"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["30"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Bold, Enum.FontStyle.Normal);
		AZY["30"]["TextSize"] = 25;
		AZY["30"]["TextColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["30"]["Size"] = UDim2.new(0.20524734258651733, 0, 0.3535553812980652, 0);
		AZY["30"]["Text"] = [[Hi,]];
		AZY["30"]["BackgroundTransparency"] = 1;
		AZY["30"]["Position"] = UDim2.new(0.5262826681137085, 0, 0.14745301008224487, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.UserPage.TextLabel
		AZY["31"] = Instance.new("TextLabel", AZY["2d"]);
		AZY["31"]["TextWrapped"] = true;
		AZY["31"]["TextScaled"] = true;
		AZY["31"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["31"]["TextXAlignment"] = Enum.TextXAlignment.Left;
		AZY["31"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Bold, Enum.FontStyle.Normal);
		AZY["31"]["TextSize"] = 25;
		AZY["31"]["TextColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["31"]["Size"] = UDim2.new(0.3468869626522064, 0, 0.3007456660270691, 0);
		AZY["31"]["Text"] = [[User]];
		AZY["31"]["BackgroundTransparency"] = 1;
		AZY["31"]["Position"] = UDim2.new(0.5669999122619629, 0, 0.5350000262260437, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.UserPage.TextLabel.UITextSizeConstraint
		AZY["32"] = Instance.new("UITextSizeConstraint", AZY["31"]);
		AZY["32"]["MaxTextSize"] = 25;

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.UserPage.TextLabel.LocalScript
		AZY["33"] = Instance.new("LocalScript", AZY["31"]);


		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.KeySystemPage
		AZY["34"] = Instance.new("Frame", AZY["2c"]);
		AZY["34"]["BackgroundColor3"] = Color3.fromRGB(0, 0, 0);
		AZY["34"]["BackgroundTransparency"] = 0.550000011920929;
		AZY["34"]["Size"] = UDim2.new(0.374349445104599, 0, 0.7526744604110718, 0);
		AZY["34"]["Position"] = UDim2.new(-0.002428855048492551, 0, 0.3016669452190399, 0);
		AZY["34"]["Name"] = [[KeySystemPage]];

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.KeySystemPage.UICorner
		AZY["35"] = Instance.new("UICorner", AZY["34"]);
		AZY["35"]["CornerRadius"] = UDim.new(0, 15);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.KeySystemPage.TextLabel
		AZY["36"] = Instance.new("TextLabel", AZY["34"]);
		AZY["36"]["TextWrapped"] = true;
		AZY["36"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["36"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Bold, Enum.FontStyle.Normal);
		AZY["36"]["TextSize"] = 16;
		AZY["36"]["TextColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["36"]["Size"] = UDim2.new(0.8114322423934937, 0, 0.15531843900680542, 0);
		AZY["36"]["Text"] = [[Key System Status]];
		AZY["36"]["BackgroundTransparency"] = 1;
		AZY["36"]["Position"] = UDim2.new(0.05482717230916023, 0, 0.06104206293821335, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.KeySystemPage.TextLabel
		AZY["37"] = Instance.new("TextLabel", AZY["34"]);
		AZY["37"]["TextWrapped"] = true;
		AZY["37"]["TextScaled"] = true;
		AZY["37"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["37"]["TextXAlignment"] = Enum.TextXAlignment.Left;
		AZY["37"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Bold, Enum.FontStyle.Normal);
		AZY["37"]["TextSize"] = 35;
		AZY["37"]["TextColor3"] = Color3.fromRGB(0, 255, 0);
		AZY["37"]["Size"] = UDim2.new(0.30206844210624695, 0, 0.09149397909641266, 0);
		AZY["37"]["Text"] = [[Online]];
		AZY["37"]["BackgroundTransparency"] = 1;
		AZY["37"]["Position"] = UDim2.new(0.08498311042785645, 0, 0.1731228232383728, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.KeySystemPage.TextLabel
		AZY["38"] = Instance.new("TextLabel", AZY["34"]);
		AZY["38"]["TextWrapped"] = true;
		AZY["38"]["TextScaled"] = true;
		AZY["38"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["38"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Bold, Enum.FontStyle.Normal);
		AZY["38"]["TextSize"] = 35;
		AZY["38"]["TextColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["38"]["Size"] = UDim2.new(0.423105388879776, 0, 0.0994054526090622, 0);
		AZY["38"]["Text"] = [[Expires In:]];
		AZY["38"]["BackgroundTransparency"] = 1;
		AZY["38"]["Position"] = UDim2.new(0.054827168583869934, 0, 0.31500908732414246, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.KeySystemPage.TimeLeft
		AZY["39"] = Instance.new("TextLabel", AZY["34"]);
		AZY["39"]["TextWrapped"] = true;
		AZY["39"]["TextScaled"] = true;
		AZY["39"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["39"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Bold, Enum.FontStyle.Normal);
		AZY["39"]["TextSize"] = 35;
		AZY["39"]["TextColor3"] = Color3.fromRGB(0, 255, 0);
		AZY["39"]["Size"] = UDim2.new(0.30206844210624695, 0, 0.0994054526090622, 0);
		AZY["39"]["Text"] = [[24h 00m]];
		AZY["39"]["Name"] = [[TimeLeft]];
		AZY["39"]["BackgroundTransparency"] = 1;
		AZY["39"]["Position"] = UDim2.new(0.49440309405326843, 0, 0.31500908732414246, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.KeySystemPage.TimeLeft.LocalScript
		AZY["3a"] = Instance.new("LocalScript", AZY["39"]);


		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.KeySystemPage.Bar
		AZY["3b"] = Instance.new("Frame", AZY["34"]);
		AZY["3b"]["BackgroundColor3"] = Color3.fromRGB(0, 255, 0);
		AZY["3b"]["Size"] = UDim2.new(0.8291789293289185, 0, 0.07132068276405334, 0);
		AZY["3b"]["Position"] = UDim2.new(0.05709991604089737, 0, 0.44679027795791626, 0);
		AZY["3b"]["Name"] = [[Bar]];

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.KeySystemPage.Bar.UICorner
		AZY["3c"] = Instance.new("UICorner", AZY["3b"]);
		AZY["3c"]["CornerRadius"] = UDim.new(0, 4);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.KeySystemPage.Bar.TextLabel
		AZY["3d"] = Instance.new("TextLabel", AZY["3b"]);
		AZY["3d"]["TextWrapped"] = true;
		AZY["3d"]["TextScaled"] = true;
		AZY["3d"]["BackgroundColor3"] = Color3.fromRGB(0, 0, 0);
		AZY["3d"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Bold, Enum.FontStyle.Normal);
		AZY["3d"]["TextTransparency"] = 0.6000000238418579;
		AZY["3d"]["TextSize"] = 35;
		AZY["3d"]["TextColor3"] = Color3.fromRGB(0, 0, 0);
		AZY["3d"]["Size"] = UDim2.new(0.2189580649137497, 0, 0.9389510154724121, 0);
		AZY["3d"]["Text"] = [[100%]];
		AZY["3d"]["BackgroundTransparency"] = 1;
		AZY["3d"]["Position"] = UDim2.new(0.7810419201850891, 0, 0.061042893677949905, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.KeySystemPage.TextLabel
		AZY["3e"] = Instance.new("TextLabel", AZY["34"]);
		AZY["3e"]["TextWrapped"] = true;
		AZY["3e"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["3e"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Bold, Enum.FontStyle.Normal);
		AZY["3e"]["TextSize"] = 12;
		AZY["3e"]["TextColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["3e"]["Size"] = UDim2.new(0.5709924697875977, 0, 0.11561357975006104, 0);
		AZY["3e"]["Text"] = [[Last activation:]];
		AZY["3e"]["BackgroundTransparency"] = 1;
		AZY["3e"]["Position"] = UDim2.new(0.05010330677032471, 0, 0.5460530519485474, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.KeySystemPage.Time
		AZY["3f"] = Instance.new("TextLabel", AZY["34"]);
		AZY["3f"]["TextWrapped"] = true;
		AZY["3f"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["3f"]["TextXAlignment"] = Enum.TextXAlignment.Left;
		AZY["3f"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Bold, Enum.FontStyle.Normal);
		AZY["3f"]["TextSize"] = 12;
		AZY["3f"]["TextColor3"] = Color3.fromRGB(178, 178, 178);
		AZY["3f"]["Size"] = UDim2.new(0.6227233409881592, 0, 0.09644854068756104, 0);
		AZY["3f"]["Text"] = [[Today, HH:MM AM]];
		AZY["3f"]["Name"] = [[Time]];
		AZY["3f"]["BackgroundTransparency"] = 1;
		AZY["3f"]["Position"] = UDim2.new(0.08199998736381531, 0, 0.6469999551773071, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.KeySystemPage.Time.LocalScript
		AZY["40"] = Instance.new("LocalScript", AZY["3f"]);


		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.KeySystemPage.Restore
		AZY["41"] = Instance.new("TextButton", AZY["34"]);
		AZY["41"]["TextWrapped"] = true;
		AZY["41"]["BackgroundColor3"] = Color3.fromRGB(255, 0, 0);
		AZY["41"]["TextSize"] = 15;
		AZY["41"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Bold, Enum.FontStyle.Normal);
		AZY["41"]["TextColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["41"]["Size"] = UDim2.new(0.7855679988861084, 0, 0.17807699739933014, 0);
		AZY["41"]["Name"] = [[Restore]];
		AZY["41"]["Text"] = [[Restore]];
		AZY["41"]["Position"] = UDim2.new(0.10590747743844986, 0, 0.7775270342826843, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.KeySystemPage.Restore.UICorner
		AZY["42"] = Instance.new("UICorner", AZY["41"]);


		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.KeySystemPage.Restore.LocalScript
		AZY["43"] = Instance.new("LocalScript", AZY["41"]);


		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.HaxPage
		AZY["44"] = Instance.new("Frame", AZY["2c"]);
		AZY["44"]["BackgroundColor3"] = Color3.fromRGB(0, 0, 0);
		AZY["44"]["BackgroundTransparency"] = 0.550000011920929;
		AZY["44"]["Size"] = UDim2.new(0.6116291880607605, 0, 1.0292569398880005, 0);
		AZY["44"]["Position"] = UDim2.new(0.3883708119392395, 0, 0.025084195658564568, 0);
		AZY["44"]["Name"] = [[HaxPage]];

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.HaxPage.UICorner
		AZY["45"] = Instance.new("UICorner", AZY["44"]);
		AZY["45"]["CornerRadius"] = UDim.new(0, 15);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.HaxPage.TextLabel
		AZY["46"] = Instance.new("TextLabel", AZY["44"]);
		AZY["46"]["TextWrapped"] = true;
		AZY["46"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["46"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Bold, Enum.FontStyle.Normal);
		AZY["46"]["TextSize"] = 18;
		AZY["46"]["TextColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["46"]["Size"] = UDim2.new(0.3717169165611267, 0, 0.10439325869083405, 0);
		AZY["46"]["Text"] = [[Quick Hacks]];
		AZY["46"]["BackgroundTransparency"] = 1;
		AZY["46"]["Position"] = UDim2.new(0.01899999938905239, 0, 0.03400000184774399, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.HaxPage.Grav
		AZY["47"] = Instance.new("BoolValue", AZY["44"]);
		AZY["47"]["Name"] = [[Grav]];

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.HaxPage.Scripts
		AZY["48"] = Instance.new("Folder", AZY["44"]);
		AZY["48"]["Name"] = [[Scripts]];

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.HaxPage.Scripts.Aimbot
		AZY["49"] = Instance.new("TextButton", AZY["48"]);
		AZY["49"]["TextWrapped"] = true;
		AZY["49"]["BackgroundColor3"] = Color3.fromRGB(255, 0, 0);
		AZY["49"]["TextSize"] = 11;
		AZY["49"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Bold, Enum.FontStyle.Normal);
		AZY["49"]["TextColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["49"]["Size"] = UDim2.new(0.2588447332382202, 0, 0.0958060473203659, 0);
		AZY["49"]["Name"] = [[Aimbot]];
		AZY["49"]["Text"] = [[AimBot]];
		AZY["49"]["Position"] = UDim2.new(0.04600000008940697, 0, 0.5989999771118164, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.HaxPage.Scripts.Aimbot.UICorner
		AZY["4a"] = Instance.new("UICorner", AZY["49"]);
		AZY["4a"]["CornerRadius"] = UDim.new(0, 5);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.HaxPage.Scripts.Aimbot.LocalScript
		AZY["4b"] = Instance.new("LocalScript", AZY["49"]);


		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.HaxPage.Scripts.Btools
		AZY["4c"] = Instance.new("TextButton", AZY["48"]);
		AZY["4c"]["TextWrapped"] = true;
		AZY["4c"]["BackgroundColor3"] = Color3.fromRGB(255, 0, 0);
		AZY["4c"]["TextSize"] = 11;
		AZY["4c"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Bold, Enum.FontStyle.Normal);
		AZY["4c"]["TextColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["4c"]["Size"] = UDim2.new(0.2588447332382202, 0, 0.0958060473203659, 0);
		AZY["4c"]["Name"] = [[Btools]];
		AZY["4c"]["Text"] = [[Btools]];
		AZY["4c"]["Position"] = UDim2.new(0.04600000008940697, 0, 0.4830000102519989, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.HaxPage.Scripts.Btools.UICorner
		AZY["4d"] = Instance.new("UICorner", AZY["4c"]);
		AZY["4d"]["CornerRadius"] = UDim.new(0, 5);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.HaxPage.Scripts.Btools.LocalScript
		AZY["4e"] = Instance.new("LocalScript", AZY["4c"]);


		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.HaxPage.Scripts.Dex
		AZY["4f"] = Instance.new("TextButton", AZY["48"]);
		AZY["4f"]["TextWrapped"] = true;
		AZY["4f"]["BackgroundColor3"] = Color3.fromRGB(255, 0, 0);
		AZY["4f"]["TextSize"] = 11;
		AZY["4f"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Bold, Enum.FontStyle.Normal);
		AZY["4f"]["TextColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["4f"]["Size"] = UDim2.new(0.2588447332382202, 0, 0.0958060473203659, 0);
		AZY["4f"]["Name"] = [[Dex]];
		AZY["4f"]["Text"] = [[DEX Explorer]];
		AZY["4f"]["Position"] = UDim2.new(0.04600000008940697, 0, 0.2564218044281006, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.HaxPage.Scripts.Dex.UICorner
		AZY["50"] = Instance.new("UICorner", AZY["4f"]);
		AZY["50"]["CornerRadius"] = UDim.new(0, 5);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.HaxPage.Scripts.Dex.LocalScript
		AZY["51"] = Instance.new("LocalScript", AZY["4f"]);


		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.HaxPage.Scripts.FatesESP
		AZY["52"] = Instance.new("TextButton", AZY["48"]);
		AZY["52"]["TextWrapped"] = true;
		AZY["52"]["BackgroundColor3"] = Color3.fromRGB(255, 0, 0);
		AZY["52"]["TextSize"] = 11;
		AZY["52"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Bold, Enum.FontStyle.Normal);
		AZY["52"]["TextColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["52"]["Size"] = UDim2.new(0.2588447332382202, 0, 0.0958060473203659, 0);
		AZY["52"]["Name"] = [[FatesESP]];
		AZY["52"]["Text"] = [[Fates ESP]];
		AZY["52"]["Position"] = UDim2.new(0.04600000008940697, 0, 0.3709999918937683, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.HaxPage.Scripts.FatesESP.UICorner
		AZY["53"] = Instance.new("UICorner", AZY["52"]);
		AZY["53"]["CornerRadius"] = UDim.new(0, 5);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.HaxPage.Scripts.FatesESP.LocalScript
		AZY["54"] = Instance.new("LocalScript", AZY["52"]);


		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.HaxPage.Scripts.Fly
		AZY["55"] = Instance.new("TextButton", AZY["48"]);
		AZY["55"]["TextWrapped"] = true;
		AZY["55"]["BackgroundColor3"] = Color3.fromRGB(255, 0, 0);
		AZY["55"]["TextSize"] = 11;
		AZY["55"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Bold, Enum.FontStyle.Normal);
		AZY["55"]["TextColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["55"]["Size"] = UDim2.new(0.2588447332382202, 0, 0.0958060473203659, 0);
		AZY["55"]["Name"] = [[Fly]];
		AZY["55"]["Text"] = [[Fly]];
		AZY["55"]["Position"] = UDim2.new(0.04600000008940697, 0, 0.7070000171661377, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.HaxPage.Scripts.Fly.UICorner
		AZY["56"] = Instance.new("UICorner", AZY["55"]);
		AZY["56"]["CornerRadius"] = UDim.new(0, 5);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.HaxPage.Scripts.Fly.LocalScript
		AZY["57"] = Instance.new("LocalScript", AZY["55"]);


		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.HaxPage.Scripts.IY
		AZY["58"] = Instance.new("TextButton", AZY["48"]);
		AZY["58"]["TextWrapped"] = true;
		AZY["58"]["BackgroundColor3"] = Color3.fromRGB(255, 0, 0);
		AZY["58"]["TextSize"] = 11;
		AZY["58"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Bold, Enum.FontStyle.Normal);
		AZY["58"]["TextColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["58"]["Size"] = UDim2.new(0.2588447332382202, 0, 0.0958060473203659, 0);
		AZY["58"]["Name"] = [[IY]];
		AZY["58"]["Text"] = [[Infinite Yield]];
		AZY["58"]["Position"] = UDim2.new(0.04595530033111572, 0, 0.13954126834869385, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.HaxPage.Scripts.IY.UICorner
		AZY["59"] = Instance.new("UICorner", AZY["58"]);
		AZY["59"]["CornerRadius"] = UDim.new(0, 5);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.HaxPage.Scripts.IY.LocalScript
		AZY["5a"] = Instance.new("LocalScript", AZY["58"]);


		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.HaxPage.Scripts.PwnHub
		AZY["5b"] = Instance.new("TextButton", AZY["48"]);
		AZY["5b"]["TextWrapped"] = true;
		AZY["5b"]["BackgroundColor3"] = Color3.fromRGB(255, 0, 0);
		AZY["5b"]["TextSize"] = 11;
		AZY["5b"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Bold, Enum.FontStyle.Normal);
		AZY["5b"]["TextColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["5b"]["Size"] = UDim2.new(0.2588447332382202, 0, 0.0958060473203659, 0);
		AZY["5b"]["Name"] = [[PwnHub]];
		AZY["5b"]["Text"] = [[Pwner Hub]];
		AZY["5b"]["Position"] = UDim2.new(0.04600000008940697, 0, 0.8209999799728394, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.HaxPage.Scripts.PwnHub.UICorner
		AZY["5c"] = Instance.new("UICorner", AZY["5b"]);
		AZY["5c"]["CornerRadius"] = UDim.new(0, 5);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.HaxPage.Scripts.PwnHub.LocalScript
		AZY["5d"] = Instance.new("LocalScript", AZY["5b"]);


		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.HaxPage.TextGrav
		AZY["5e"] = Instance.new("TextLabel", AZY["44"]);
		AZY["5e"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["5e"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Bold, Enum.FontStyle.Normal);
		AZY["5e"]["TextSize"] = 12;
		AZY["5e"]["TextColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["5e"]["Size"] = UDim2.new(0, 50, 0, 11);
		AZY["5e"]["Text"] = [[Gravity]];
		AZY["5e"]["Name"] = [[TextGrav]];
		AZY["5e"]["BackgroundTransparency"] = 1;
		AZY["5e"]["Position"] = UDim2.new(0.3269999921321869, 0, 0.8930000066757202, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.HaxPage.TextWs
		AZY["5f"] = Instance.new("TextLabel", AZY["44"]);
		AZY["5f"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["5f"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Bold, Enum.FontStyle.Normal);
		AZY["5f"]["TextSize"] = 12;
		AZY["5f"]["TextColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["5f"]["Size"] = UDim2.new(0, 50, 0, 11);
		AZY["5f"]["Text"] = [[Speed]];
		AZY["5f"]["Name"] = [[TextWs]];
		AZY["5f"]["BackgroundTransparency"] = 1;
		AZY["5f"]["Position"] = UDim2.new(0.5411151647567749, 0, 0.8930000066757202, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.HaxPage.TextJp
		AZY["60"] = Instance.new("TextLabel", AZY["44"]);
		AZY["60"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["60"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Bold, Enum.FontStyle.Normal);
		AZY["60"]["TextSize"] = 12;
		AZY["60"]["TextColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["60"]["Size"] = UDim2.new(0, 50, 0, 11);
		AZY["60"]["Text"] = [[Jump]];
		AZY["60"]["Name"] = [[TextJp]];
		AZY["60"]["BackgroundTransparency"] = 1;
		AZY["60"]["Position"] = UDim2.new(0.7466657161712646, 0, 0.8930000066757202, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.HaxPage.Ws
		AZY["61"] = Instance.new("BoolValue", AZY["44"]);
		AZY["61"]["Name"] = [[Ws]];

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.HaxPage.Jp
		AZY["62"] = Instance.new("BoolValue", AZY["44"]);
		AZY["62"]["Name"] = [[Jp]];

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.HaxPage.ToggleGrav
		AZY["63"] = Instance.new("TextButton", AZY["44"]);
		AZY["63"]["BackgroundColor3"] = Color3.fromRGB(146, 0, 0);
		AZY["63"]["TextSize"] = 14;
		AZY["63"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Regular, Enum.FontStyle.Normal);
		AZY["63"]["TextColor3"] = Color3.fromRGB(0, 0, 0);
		AZY["63"]["Size"] = UDim2.new(0, 15, 0, 15);
		AZY["63"]["Name"] = [[ToggleGrav]];
		AZY["63"]["Text"] = [[]];
		AZY["63"]["Position"] = UDim2.new(0.40253645181655884, 0, 0.801304280757904, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.HaxPage.ToggleGrav.UICorner
		AZY["64"] = Instance.new("UICorner", AZY["63"]);
		AZY["64"]["CornerRadius"] = UDim.new(100, 100);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.HaxPage.ToggleGrav.LocalScript
		AZY["65"] = Instance.new("LocalScript", AZY["63"]);


		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.HaxPage.ToggleWs
		AZY["66"] = Instance.new("TextButton", AZY["44"]);
		AZY["66"]["BackgroundColor3"] = Color3.fromRGB(146, 0, 0);
		AZY["66"]["TextSize"] = 14;
		AZY["66"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Regular, Enum.FontStyle.Normal);
		AZY["66"]["TextColor3"] = Color3.fromRGB(0, 0, 0);
		AZY["66"]["Size"] = UDim2.new(0, 15, 0, 15);
		AZY["66"]["Name"] = [[ToggleWs]];
		AZY["66"]["Text"] = [[]];
		AZY["66"]["Position"] = UDim2.new(0.6166515946388245, 0, 0.801304280757904, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.HaxPage.ToggleWs.UICorner
		AZY["67"] = Instance.new("UICorner", AZY["66"]);
		AZY["67"]["CornerRadius"] = UDim.new(100, 100);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.HaxPage.ToggleWs.LocalScript
		AZY["68"] = Instance.new("LocalScript", AZY["66"]);


		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.HaxPage.ToggleJp
		AZY["69"] = Instance.new("TextButton", AZY["44"]);
		AZY["69"]["BackgroundColor3"] = Color3.fromRGB(146, 0, 0);
		AZY["69"]["TextSize"] = 14;
		AZY["69"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Regular, Enum.FontStyle.Normal);
		AZY["69"]["TextColor3"] = Color3.fromRGB(0, 0, 0);
		AZY["69"]["Size"] = UDim2.new(0, 15, 0, 15);
		AZY["69"]["Name"] = [[ToggleJp]];
		AZY["69"]["Text"] = [[]];
		AZY["69"]["Position"] = UDim2.new(0.8222021460533142, 0, 0.801304280757904, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.HaxPage.ToggleJp.UICorner
		AZY["6a"] = Instance.new("UICorner", AZY["69"]);
		AZY["6a"]["CornerRadius"] = UDim.new(100, 100);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.HaxPage.ToggleJp.LocalScript
		AZY["6b"] = Instance.new("LocalScript", AZY["69"]);


		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.HaxPage.JpS
		AZY["6c"] = Instance.new("ImageButton", AZY["44"]);
		AZY["6c"]["Active"] = false;
		AZY["6c"]["BorderSizePixel"] = 0;
		AZY["6c"]["SliceCenter"] = Rect.new(100, 100, 100, 100);
		AZY["6c"]["ScaleType"] = Enum.ScaleType.Slice;
		AZY["6c"]["SliceScale"] = 0.11999999731779099;
		AZY["6c"]["ImageTransparency"] = 1;
		AZY["6c"]["BackgroundColor3"] = Color3.fromRGB(22, 22, 22);
		AZY["6c"]["ImageColor3"] = Color3.fromRGB(32, 32, 32);
		AZY["6c"]["Selectable"] = false;
		AZY["6c"]["AnchorPoint"] = Vector2.new(0.5, 0.5);
		AZY["6c"]["Image"] = [[rbxassetid://3570695787]];
		AZY["6c"]["Size"] = UDim2.new(0, 119, 0, 31);
		AZY["6c"]["Name"] = [[JpS]];
		AZY["6c"]["Rotation"] = -90;
		AZY["6c"]["Position"] = UDim2.new(0.8600000143051147, 0, 0.4399999976158142, 0);
		AZY["6c"]["BackgroundTransparency"] = 1;

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.HaxPage.JpS.SliderButton
		AZY["6d"] = Instance.new("ImageLabel", AZY["6c"]);
		AZY["6d"]["SliceCenter"] = Rect.new(100, 100, 100, 100);
		AZY["6d"]["ScaleType"] = Enum.ScaleType.Slice;
		AZY["6d"]["BackgroundColor3"] = Color3.fromRGB(71, 71, 71);
		AZY["6d"]["ImageColor3"] = Color3.fromRGB(146, 0, 0);
		AZY["6d"]["SliceScale"] = 0.11999999731779099;
		AZY["6d"]["Selectable"] = true;
		AZY["6d"]["Image"] = [[rbxassetid://3570695787]];
		AZY["6d"]["Size"] = UDim2.new(0, 25, 1, 0);
		AZY["6d"]["Active"] = true;
		AZY["6d"]["Name"] = [[SliderButton]];
		AZY["6d"]["BackgroundTransparency"] = 1;

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.HaxPage.JpS.SliderButton.LocalScript
		AZY["6e"] = Instance.new("LocalScript", AZY["6d"]);


		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.HaxPage.JpS.Border
		AZY["6f"] = Instance.new("ImageLabel", AZY["6c"]);
		AZY["6f"]["ZIndex"] = -1;
		AZY["6f"]["SliceCenter"] = Rect.new(100, 100, 100, 100);
		AZY["6f"]["ScaleType"] = Enum.ScaleType.Slice;
		AZY["6f"]["BackgroundColor3"] = Color3.fromRGB(62, 62, 62);
		AZY["6f"]["ImageColor3"] = Color3.fromRGB(71, 71, 71);
		AZY["6f"]["SliceScale"] = 0.23999999463558197;
		AZY["6f"]["ImageTransparency"] = 1;
		AZY["6f"]["AnchorPoint"] = Vector2.new(0.5, 0.5);
		AZY["6f"]["Image"] = [[rbxassetid://3570695787]];
		AZY["6f"]["Size"] = UDim2.new(1, 12, 1, 12);
		AZY["6f"]["Name"] = [[Border]];
		AZY["6f"]["BackgroundTransparency"] = 0.6000000238418579;
		AZY["6f"]["Position"] = UDim2.new(0.5, 0, 0.5, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.HaxPage.JpS.Border.UICorner
		AZY["70"] = Instance.new("UICorner", AZY["6f"]);
		AZY["70"]["CornerRadius"] = UDim.new(0, 12);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.HaxPage.JpS.StripedPattern
		AZY["71"] = Instance.new("ImageLabel", AZY["6c"]);
		AZY["71"]["BorderSizePixel"] = 0;
		AZY["71"]["ScaleType"] = Enum.ScaleType.Tile;
		AZY["71"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["71"]["ImageColor3"] = Color3.fromRGB(32, 32, 32);
		AZY["71"]["ImageTransparency"] = 1;
		AZY["71"]["AnchorPoint"] = Vector2.new(0.5, 0);
		AZY["71"]["Image"] = [[rbxassetid://4925116997]];
		AZY["71"]["TileSize"] = UDim2.new(0, 25, 1, 0);
		AZY["71"]["Size"] = UDim2.new(1, -25, 1, 0);
		AZY["71"]["Name"] = [[StripedPattern]];
		AZY["71"]["BackgroundTransparency"] = 1;
		AZY["71"]["Position"] = UDim2.new(0.5, 0, 0, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.HaxPage.JpS.StripedPattern.UIGradient
		AZY["72"] = Instance.new("UIGradient", AZY["71"]);
		AZY["72"]["Rotation"] = 90;
		AZY["72"]["Color"] = ColorSequence.new{ColorSequenceKeypoint.new(0.000, Color3.fromRGB(255, 255, 255)),ColorSequenceKeypoint.new(1.000, Color3.fromRGB(0, 0, 0))};

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.HaxPage.JpS.ImageLabel
		AZY["73"] = Instance.new("ImageLabel", AZY["6c"]);
		AZY["73"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["73"]["Image"] = [[rbxassetid://12582573514]];
		AZY["73"]["Size"] = UDim2.new(0, 35, 0, 35);
		AZY["73"]["Rotation"] = 90;
		AZY["73"]["BackgroundTransparency"] = 1;
		AZY["73"]["Position"] = UDim2.new(-0.017000000923871994, 0, -0.10000000149011612, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.HaxPage.JpS.TextLabel
		AZY["74"] = Instance.new("TextBox", AZY["6c"]);
		AZY["74"]["ZIndex"] = 2;
		AZY["74"]["TextSize"] = 13;
		AZY["74"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["74"]["TextColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["74"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Bold, Enum.FontStyle.Normal);
		AZY["74"]["AnchorPoint"] = Vector2.new(1, 0);
		AZY["74"]["BackgroundTransparency"] = 1;
		AZY["74"]["Size"] = UDim2.new(0, 50, 1, 0);
		AZY["74"]["Text"] = [[0%]];
		AZY["74"]["Position"] = UDim2.new(0, 137, 0, 0);
		AZY["74"]["Rotation"] = 90;
		AZY["74"]["Name"] = [[TextLabel]];

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.HaxPage.WsS
		AZY["75"] = Instance.new("ImageButton", AZY["44"]);
		AZY["75"]["Active"] = false;
		AZY["75"]["BorderSizePixel"] = 0;
		AZY["75"]["SliceCenter"] = Rect.new(100, 100, 100, 100);
		AZY["75"]["ScaleType"] = Enum.ScaleType.Slice;
		AZY["75"]["SliceScale"] = 0.11999999731779099;
		AZY["75"]["ImageTransparency"] = 1;
		AZY["75"]["BackgroundColor3"] = Color3.fromRGB(22, 22, 22);
		AZY["75"]["ImageColor3"] = Color3.fromRGB(32, 32, 32);
		AZY["75"]["Selectable"] = false;
		AZY["75"]["AnchorPoint"] = Vector2.new(0.5, 0.5);
		AZY["75"]["Image"] = [[rbxassetid://3570695787]];
		AZY["75"]["Size"] = UDim2.new(0, 119, 0, 31);
		AZY["75"]["Name"] = [[WsS]];
		AZY["75"]["Rotation"] = -90;
		AZY["75"]["Position"] = UDim2.new(0.6499999761581421, 0, 0.4399999976158142, 0);
		AZY["75"]["BackgroundTransparency"] = 1;

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.HaxPage.WsS.SliderButton
		AZY["76"] = Instance.new("ImageLabel", AZY["75"]);
		AZY["76"]["SliceCenter"] = Rect.new(100, 100, 100, 100);
		AZY["76"]["ScaleType"] = Enum.ScaleType.Slice;
		AZY["76"]["BackgroundColor3"] = Color3.fromRGB(71, 71, 71);
		AZY["76"]["ImageColor3"] = Color3.fromRGB(146, 0, 0);
		AZY["76"]["SliceScale"] = 0.11999999731779099;
		AZY["76"]["Selectable"] = true;
		AZY["76"]["Image"] = [[rbxassetid://3570695787]];
		AZY["76"]["Size"] = UDim2.new(0, 25, 1, 0);
		AZY["76"]["Active"] = true;
		AZY["76"]["Name"] = [[SliderButton]];
		AZY["76"]["BackgroundTransparency"] = 1;

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.HaxPage.WsS.SliderButton.LocalScript
		AZY["77"] = Instance.new("LocalScript", AZY["76"]);


		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.HaxPage.WsS.Border
		AZY["78"] = Instance.new("ImageLabel", AZY["75"]);
		AZY["78"]["ZIndex"] = -1;
		AZY["78"]["SliceCenter"] = Rect.new(100, 100, 100, 100);
		AZY["78"]["ScaleType"] = Enum.ScaleType.Slice;
		AZY["78"]["BackgroundColor3"] = Color3.fromRGB(62, 62, 62);
		AZY["78"]["ImageColor3"] = Color3.fromRGB(71, 71, 71);
		AZY["78"]["SliceScale"] = 0.23999999463558197;
		AZY["78"]["ImageTransparency"] = 1;
		AZY["78"]["AnchorPoint"] = Vector2.new(0.5, 0.5);
		AZY["78"]["Image"] = [[rbxassetid://3570695787]];
		AZY["78"]["Size"] = UDim2.new(1, 12, 1, 12);
		AZY["78"]["Name"] = [[Border]];
		AZY["78"]["BackgroundTransparency"] = 0.6000000238418579;
		AZY["78"]["Position"] = UDim2.new(0.5, 0, 0.5, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.HaxPage.WsS.Border.UICorner
		AZY["79"] = Instance.new("UICorner", AZY["78"]);
		AZY["79"]["CornerRadius"] = UDim.new(0, 12);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.HaxPage.WsS.StripedPattern
		AZY["7a"] = Instance.new("ImageLabel", AZY["75"]);
		AZY["7a"]["BorderSizePixel"] = 0;
		AZY["7a"]["ScaleType"] = Enum.ScaleType.Tile;
		AZY["7a"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["7a"]["ImageColor3"] = Color3.fromRGB(32, 32, 32);
		AZY["7a"]["ImageTransparency"] = 1;
		AZY["7a"]["AnchorPoint"] = Vector2.new(0.5, 0);
		AZY["7a"]["Image"] = [[rbxassetid://4925116997]];
		AZY["7a"]["TileSize"] = UDim2.new(0, 25, 1, 0);
		AZY["7a"]["Size"] = UDim2.new(1, -25, 1, 0);
		AZY["7a"]["Name"] = [[StripedPattern]];
		AZY["7a"]["BackgroundTransparency"] = 1;
		AZY["7a"]["Position"] = UDim2.new(0.5, 0, 0, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.HaxPage.WsS.StripedPattern.UIGradient
		AZY["7b"] = Instance.new("UIGradient", AZY["7a"]);
		AZY["7b"]["Rotation"] = 90;
		AZY["7b"]["Color"] = ColorSequence.new{ColorSequenceKeypoint.new(0.000, Color3.fromRGB(255, 255, 255)),ColorSequenceKeypoint.new(1.000, Color3.fromRGB(0, 0, 0))};

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.HaxPage.WsS.ImageLabel
		AZY["7c"] = Instance.new("ImageLabel", AZY["75"]);
		AZY["7c"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["7c"]["Image"] = [[rbxassetid://12572149271]];
		AZY["7c"]["Size"] = UDim2.new(0, 35, 0, 35);
		AZY["7c"]["Rotation"] = 90;
		AZY["7c"]["BackgroundTransparency"] = 1;
		AZY["7c"]["Position"] = UDim2.new(-0.017000000923871994, 0, -0.10000000149011612, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.HaxPage.WsS.TextLabel
		AZY["7d"] = Instance.new("TextBox", AZY["75"]);
		AZY["7d"]["ZIndex"] = 2;
		AZY["7d"]["TextSize"] = 13;
		AZY["7d"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["7d"]["TextColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["7d"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Bold, Enum.FontStyle.Normal);
		AZY["7d"]["AnchorPoint"] = Vector2.new(1, 0);
		AZY["7d"]["BackgroundTransparency"] = 1;
		AZY["7d"]["Size"] = UDim2.new(0, 50, 1, 0);
		AZY["7d"]["Text"] = [[0%]];
		AZY["7d"]["Position"] = UDim2.new(0, 137, 0, 0);
		AZY["7d"]["Rotation"] = 90;
		AZY["7d"]["Name"] = [[TextLabel]];

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.HaxPage.GravS
		AZY["7e"] = Instance.new("ImageButton", AZY["44"]);
		AZY["7e"]["Active"] = false;
		AZY["7e"]["BorderSizePixel"] = 0;
		AZY["7e"]["SliceCenter"] = Rect.new(100, 100, 100, 100);
		AZY["7e"]["ScaleType"] = Enum.ScaleType.Slice;
		AZY["7e"]["SliceScale"] = 0.11999999731779099;
		AZY["7e"]["ImageTransparency"] = 1;
		AZY["7e"]["BackgroundColor3"] = Color3.fromRGB(22, 22, 22);
		AZY["7e"]["ImageColor3"] = Color3.fromRGB(32, 32, 32);
		AZY["7e"]["Selectable"] = false;
		AZY["7e"]["AnchorPoint"] = Vector2.new(0.5, 0.5);
		AZY["7e"]["Image"] = [[rbxassetid://3570695787]];
		AZY["7e"]["Size"] = UDim2.new(0, 119, 0, 31);
		AZY["7e"]["Name"] = [[GravS]];
		AZY["7e"]["Rotation"] = -90;
		AZY["7e"]["Position"] = UDim2.new(0.4359999895095825, 0, 0.4399999976158142, 0);
		AZY["7e"]["BackgroundTransparency"] = 1;

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.HaxPage.GravS.SliderButton
		AZY["7f"] = Instance.new("ImageLabel", AZY["7e"]);
		AZY["7f"]["SliceCenter"] = Rect.new(100, 100, 100, 100);
		AZY["7f"]["ScaleType"] = Enum.ScaleType.Slice;
		AZY["7f"]["BackgroundColor3"] = Color3.fromRGB(71, 71, 71);
		AZY["7f"]["ImageColor3"] = Color3.fromRGB(146, 0, 0);
		AZY["7f"]["SliceScale"] = 0.11999999731779099;
		AZY["7f"]["Selectable"] = true;
		AZY["7f"]["Image"] = [[rbxassetid://3570695787]];
		AZY["7f"]["Size"] = UDim2.new(0, 25, 1, 0);
		AZY["7f"]["Active"] = true;
		AZY["7f"]["Name"] = [[SliderButton]];
		AZY["7f"]["BackgroundTransparency"] = 1;

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.HaxPage.GravS.SliderButton.LocalScript
		AZY["80"] = Instance.new("LocalScript", AZY["7f"]);


		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.HaxPage.GravS.Border
		AZY["81"] = Instance.new("ImageLabel", AZY["7e"]);
		AZY["81"]["ZIndex"] = -1;
		AZY["81"]["SliceCenter"] = Rect.new(100, 100, 100, 100);
		AZY["81"]["ScaleType"] = Enum.ScaleType.Slice;
		AZY["81"]["BackgroundColor3"] = Color3.fromRGB(62, 62, 62);
		AZY["81"]["ImageColor3"] = Color3.fromRGB(71, 71, 71);
		AZY["81"]["SliceScale"] = 0.23999999463558197;
		AZY["81"]["ImageTransparency"] = 1;
		AZY["81"]["AnchorPoint"] = Vector2.new(0.5, 0.5);
		AZY["81"]["Image"] = [[rbxassetid://3570695787]];
		AZY["81"]["Size"] = UDim2.new(1, 12, 1, 12);
		AZY["81"]["Name"] = [[Border]];
		AZY["81"]["BackgroundTransparency"] = 0.6000000238418579;
		AZY["81"]["Position"] = UDim2.new(0.5, 0, 0.5, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.HaxPage.GravS.Border.UICorner
		AZY["82"] = Instance.new("UICorner", AZY["81"]);
		AZY["82"]["CornerRadius"] = UDim.new(0, 12);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.HaxPage.GravS.StripedPattern
		AZY["83"] = Instance.new("ImageLabel", AZY["7e"]);
		AZY["83"]["BorderSizePixel"] = 0;
		AZY["83"]["ScaleType"] = Enum.ScaleType.Tile;
		AZY["83"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["83"]["ImageColor3"] = Color3.fromRGB(32, 32, 32);
		AZY["83"]["ImageTransparency"] = 1;
		AZY["83"]["AnchorPoint"] = Vector2.new(0.5, 0);
		AZY["83"]["Image"] = [[rbxassetid://4925116997]];
		AZY["83"]["TileSize"] = UDim2.new(0, 25, 1, 0);
		AZY["83"]["Size"] = UDim2.new(1, -25, 1, 0);
		AZY["83"]["Name"] = [[StripedPattern]];
		AZY["83"]["BackgroundTransparency"] = 1;
		AZY["83"]["Position"] = UDim2.new(0.5, 0, 0, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.HaxPage.GravS.StripedPattern.UIGradient
		AZY["84"] = Instance.new("UIGradient", AZY["83"]);
		AZY["84"]["Rotation"] = 90;
		AZY["84"]["Color"] = ColorSequence.new{ColorSequenceKeypoint.new(0.000, Color3.fromRGB(255, 255, 255)),ColorSequenceKeypoint.new(1.000, Color3.fromRGB(0, 0, 0))};

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.HaxPage.GravS.ImageLabel
		AZY["85"] = Instance.new("ImageLabel", AZY["7e"]);
		AZY["85"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["85"]["Image"] = [[rbxassetid://12582575947]];
		AZY["85"]["Size"] = UDim2.new(0, 35, 0, 35);
		AZY["85"]["Rotation"] = 90;
		AZY["85"]["BackgroundTransparency"] = 1;
		AZY["85"]["Position"] = UDim2.new(-0.017000000923871994, 0, -0.10000000149011612, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.HaxPage.GravS.TextLabel
		AZY["86"] = Instance.new("TextBox", AZY["7e"]);
		AZY["86"]["ZIndex"] = 2;
		AZY["86"]["TextSize"] = 13;
		AZY["86"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["86"]["TextColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["86"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Bold, Enum.FontStyle.Normal);
		AZY["86"]["AnchorPoint"] = Vector2.new(1, 0);
		AZY["86"]["BackgroundTransparency"] = 1;
		AZY["86"]["Size"] = UDim2.new(0, 50, 1, 0);
		AZY["86"]["Text"] = [[0%]];
		AZY["86"]["Position"] = UDim2.new(0, 137, 0, 0);
		AZY["86"]["Rotation"] = 90;
		AZY["86"]["Name"] = [[TextLabel]];

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Changelogs
		AZY["87"] = Instance.new("Frame", AZY["2b"]);
		AZY["87"]["BackgroundColor3"] = Color3.fromRGB(0, 0, 0);
		AZY["87"]["BackgroundTransparency"] = 1;
		AZY["87"]["Size"] = UDim2.new(0.831805408000946, 0, 0.7735126614570618, 0);
		AZY["87"]["Position"] = UDim2.new(0.1409205049276352, 0, 0.18711429834365845, 0);
		AZY["87"]["Visible"] = false;
		AZY["87"]["Name"] = [[Changelogs]];

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Changelogs.TitlePage
		AZY["88"] = Instance.new("Frame", AZY["87"]);
		AZY["88"]["BackgroundColor3"] = Color3.fromRGB(0, 0, 0);
		AZY["88"]["BackgroundTransparency"] = 0.550000011920929;
		AZY["88"]["Size"] = UDim2.new(0.47281256318092346, 0, 0.2235966920852661, 0);
		AZY["88"]["Position"] = UDim2.new(0.0059703318402171135, 0, 0.020400146022439003, 0);
		AZY["88"]["Name"] = [[TitlePage]];

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Changelogs.TitlePage.UICorner
		AZY["89"] = Instance.new("UICorner", AZY["88"]);
		AZY["89"]["CornerRadius"] = UDim.new(0, 15);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Changelogs.TitlePage.ImageLabel
		AZY["8a"] = Instance.new("ImageLabel", AZY["88"]);
		AZY["8a"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["8a"]["Image"] = [[rbxassetid://12585006598]];
		AZY["8a"]["Size"] = UDim2.new(0, 48, 0, 48);
		AZY["8a"]["BackgroundTransparency"] = 1;
		AZY["8a"]["Position"] = UDim2.new(0.16064772009849548, 0, -0.020948588848114014, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Changelogs.TitlePage.TextLogo
		AZY["8b"] = Instance.new("TextLabel", AZY["88"]);
		AZY["8b"]["TextWrapped"] = true;
		AZY["8b"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["8b"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Bold, Enum.FontStyle.Normal);
		AZY["8b"]["TextSize"] = 17;
		AZY["8b"]["TextColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["8b"]["Size"] = UDim2.new(0.48227599263191223, 0, 0.442178338766098, 0);
		AZY["8b"]["Text"] = [[SPDM Team]];
		AZY["8b"]["Name"] = [[TextLogo]];
		AZY["8b"]["BackgroundTransparency"] = 1;
		AZY["8b"]["Position"] = UDim2.new(0.3840000033378601, 0, 0.2709999978542328, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Changelogs.TitlePage.TextLogo.UITextSizeConstraint
		AZY["8c"] = Instance.new("UITextSizeConstraint", AZY["8b"]);
		AZY["8c"]["MaxTextSize"] = 25;

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Changelogs.Credits
		AZY["8d"] = Instance.new("Frame", AZY["87"]);
		AZY["8d"]["BackgroundColor3"] = Color3.fromRGB(0, 0, 0);
		AZY["8d"]["BackgroundTransparency"] = 0.550000011920929;
		AZY["8d"]["Size"] = UDim2.new(0.47281256318092346, 0, 0.7172916531562805, 0);
		AZY["8d"]["Position"] = UDim2.new(0.0059703318402171135, 0, 0.28270816802978516, 0);
		AZY["8d"]["Name"] = [[Credits]];

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Changelogs.Credits.UICorner
		AZY["8e"] = Instance.new("UICorner", AZY["8d"]);
		AZY["8e"]["CornerRadius"] = UDim.new(0, 15);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Changelogs.Credits.Title
		AZY["8f"] = Instance.new("TextLabel", AZY["8d"]);
		AZY["8f"]["TextWrapped"] = true;
		AZY["8f"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["8f"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Bold, Enum.FontStyle.Normal);
		AZY["8f"]["TextSize"] = 17;
		AZY["8f"]["TextColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["8f"]["Size"] = UDim2.new(0.32700005173683167, 0, 0.14513146877288818, 0);
		AZY["8f"]["Text"] = [[About us]];
		AZY["8f"]["Name"] = [[Title]];
		AZY["8f"]["BackgroundTransparency"] = 1;
		AZY["8f"]["Position"] = UDim2.new(0.056999966502189636, 0, 0.048999954015016556, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Changelogs.Credits.Title.UITextSizeConstraint
		AZY["90"] = Instance.new("UITextSizeConstraint", AZY["8f"]);
		AZY["90"]["MaxTextSize"] = 25;

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Changelogs.Credits.ScrollingFrame
		AZY["91"] = Instance.new("ScrollingFrame", AZY["8d"]);
		AZY["91"]["Active"] = true;
		AZY["91"]["CanvasSize"] = UDim2.new(0, 0, 1.5, 0);
		AZY["91"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["91"]["BackgroundTransparency"] = 1;
		AZY["91"]["Size"] = UDim2.new(0, 175, 0, 110);
		AZY["91"]["ScrollBarImageColor3"] = Color3.fromRGB(255, 0, 14);
		AZY["91"]["BorderColor3"] = Color3.fromRGB(54, 0, 2);
		AZY["91"]["ScrollBarThickness"] = 5;
		AZY["91"]["Position"] = UDim2.new(-4.226361483006258e-08, 0, 0.20896700024604797, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Changelogs.Credits.ScrollingFrame.Person
		AZY["92"] = Instance.new("Frame", AZY["91"]);
		AZY["92"]["BackgroundColor3"] = Color3.fromRGB(0, 0, 0);
		AZY["92"]["BackgroundTransparency"] = 1;
		AZY["92"]["Size"] = UDim2.new(0, 144, 0, 44);
		AZY["92"]["Position"] = UDim2.new(0.11400000005960464, 0, 0, 0);
		AZY["92"]["Name"] = [[Person]];

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Changelogs.Credits.ScrollingFrame.Person.ImageLabel
		AZY["93"] = Instance.new("ImageLabel", AZY["92"]);
		AZY["93"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["93"]["Image"] = [[rbxassetid://12585390334]];
		AZY["93"]["Size"] = UDim2.new(0, 41, 0, 41);
		AZY["93"]["BackgroundTransparency"] = 1;

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Changelogs.Credits.ScrollingFrame.Person.TextLogo
		AZY["94"] = Instance.new("TextLabel", AZY["92"]);
		AZY["94"]["TextWrapped"] = true;
		AZY["94"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["94"]["TextXAlignment"] = Enum.TextXAlignment.Left;
		AZY["94"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Bold, Enum.FontStyle.Normal);
		AZY["94"]["TextSize"] = 13;
		AZY["94"]["TextColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["94"]["Size"] = UDim2.new(0.6571568250656128, 0, 0.37654438614845276, 0);
		AZY["94"]["Text"] = [[Chillz]];
		AZY["94"]["Name"] = [[TextLogo]];
		AZY["94"]["BackgroundTransparency"] = 1;
		AZY["94"]["Position"] = UDim2.new(0.34299999475479126, 0, 0.16500000655651093, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Changelogs.Credits.ScrollingFrame.Person.TextLogo.UITextSizeConstraint
		AZY["95"] = Instance.new("UITextSizeConstraint", AZY["94"]);
		AZY["95"]["MaxTextSize"] = 25;

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Changelogs.Credits.ScrollingFrame.Person.Desc
		AZY["96"] = Instance.new("TextLabel", AZY["92"]);
		AZY["96"]["TextWrapped"] = true;
		AZY["96"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["96"]["TextXAlignment"] = Enum.TextXAlignment.Left;
		AZY["96"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Bold, Enum.FontStyle.Normal);
		AZY["96"]["TextSize"] = 11;
		AZY["96"]["TextColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["96"]["Size"] = UDim2.new(0.657156765460968, 0, 0.3310898244380951, 0);
		AZY["96"]["Text"] = [[UI Everything]];
		AZY["96"]["Name"] = [[Desc]];
		AZY["96"]["BackgroundTransparency"] = 1;
		AZY["96"]["Position"] = UDim2.new(0.34299999475479126, 0, 0.4300000071525574, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Changelogs.Credits.ScrollingFrame.Person.Desc.UITextSizeConstraint
		AZY["97"] = Instance.new("UITextSizeConstraint", AZY["96"]);
		AZY["97"]["MaxTextSize"] = 25;

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Changelogs.Credits.ScrollingFrame.Person
		AZY["98"] = Instance.new("Frame", AZY["91"]);
		AZY["98"]["BackgroundColor3"] = Color3.fromRGB(0, 0, 0);
		AZY["98"]["BackgroundTransparency"] = 1;
		AZY["98"]["Size"] = UDim2.new(0, 144, 0, 44);
		AZY["98"]["Position"] = UDim2.new(0.11400000005960464, 0, 0.19155307114124298, 0);
		AZY["98"]["Name"] = [[Person]];

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Changelogs.Credits.ScrollingFrame.Person.ImageLabel
		AZY["99"] = Instance.new("ImageLabel", AZY["98"]);
		AZY["99"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["99"]["Image"] = [[rbxassetid://12585434446]];
		AZY["99"]["Size"] = UDim2.new(0, 41, 0, 41);
		AZY["99"]["BackgroundTransparency"] = 1;

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Changelogs.Credits.ScrollingFrame.Person.TextLogo
		AZY["9a"] = Instance.new("TextLabel", AZY["98"]);
		AZY["9a"]["TextWrapped"] = true;
		AZY["9a"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["9a"]["TextXAlignment"] = Enum.TextXAlignment.Left;
		AZY["9a"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Bold, Enum.FontStyle.Normal);
		AZY["9a"]["TextSize"] = 13;
		AZY["9a"]["TextColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["9a"]["Size"] = UDim2.new(0.6571568250656128, 0, 0.37654438614845276, 0);
		AZY["9a"]["Text"] = [[Ash01#0947]];
		AZY["9a"]["Name"] = [[TextLogo]];
		AZY["9a"]["BackgroundTransparency"] = 1;
		AZY["9a"]["Position"] = UDim2.new(0.34299999475479126, 0, 0.16500000655651093, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Changelogs.Credits.ScrollingFrame.Person.TextLogo.UITextSizeConstraint
		AZY["9b"] = Instance.new("UITextSizeConstraint", AZY["9a"]);
		AZY["9b"]["MaxTextSize"] = 25;

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Changelogs.Credits.ScrollingFrame.Person.Desc
		AZY["9c"] = Instance.new("TextLabel", AZY["98"]);
		AZY["9c"]["TextWrapped"] = true;
		AZY["9c"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["9c"]["TextXAlignment"] = Enum.TextXAlignment.Left;
		AZY["9c"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Bold, Enum.FontStyle.Normal);
		AZY["9c"]["TextColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["9c"]["Size"] = UDim2.new(0.657156765460968, 0, 0.3310898244380951, 0);
		AZY["9c"]["Text"] = [[Pwner Hub Owner / Creator]];
		AZY["9c"]["Name"] = [[Desc]];
		AZY["9c"]["BackgroundTransparency"] = 1;
		AZY["9c"]["Position"] = UDim2.new(0.34299999475479126, 0, 0.4300000071525574, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Changelogs.Credits.ScrollingFrame.Person.Desc.UITextSizeConstraint
		AZY["9d"] = Instance.new("UITextSizeConstraint", AZY["9c"]);
		AZY["9d"]["MaxTextSize"] = 25;

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Changelogs.Credits.ScrollingFrame.Person
		AZY["9e"] = Instance.new("Frame", AZY["91"]);
		AZY["9e"]["BackgroundColor3"] = Color3.fromRGB(0, 0, 0);
		AZY["9e"]["BackgroundTransparency"] = 1;
		AZY["9e"]["Size"] = UDim2.new(0, 144, 0, 44);
		AZY["9e"]["Position"] = UDim2.new(0.11400000005960464, 0, 0.38310614228248596, 0);
		AZY["9e"]["Name"] = [[Person]];

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Changelogs.Credits.ScrollingFrame.Person.ImageLabel
		AZY["9f"] = Instance.new("ImageLabel", AZY["9e"]);
		AZY["9f"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["9f"]["Image"] = [[http://www.roblox.com/asset/?id=12642988505]];
		AZY["9f"]["Size"] = UDim2.new(0, 41, 0, 41);
		AZY["9f"]["BackgroundTransparency"] = 1;

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Changelogs.Credits.ScrollingFrame.Person.TextLogo
		AZY["a0"] = Instance.new("TextLabel", AZY["9e"]);
		AZY["a0"]["TextWrapped"] = true;
		AZY["a0"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["a0"]["TextXAlignment"] = Enum.TextXAlignment.Left;
		AZY["a0"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Bold, Enum.FontStyle.Normal);
		AZY["a0"]["TextSize"] = 13;
		AZY["a0"]["TextColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["a0"]["Size"] = UDim2.new(0.6571568250656128, 0, 0.37654438614845276, 0);
		AZY["a0"]["Text"] = [[Bread!]];
		AZY["a0"]["Name"] = [[TextLogo]];
		AZY["a0"]["BackgroundTransparency"] = 1;
		AZY["a0"]["Position"] = UDim2.new(0.34299999475479126, 0, 0.16500000655651093, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Changelogs.Credits.ScrollingFrame.Person.TextLogo.UITextSizeConstraint
		AZY["a1"] = Instance.new("UITextSizeConstraint", AZY["a0"]);
		AZY["a1"]["MaxTextSize"] = 25;

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Changelogs.Credits.ScrollingFrame.Person.Desc
		AZY["a2"] = Instance.new("TextLabel", AZY["9e"]);
		AZY["a2"]["TextWrapped"] = true;
		AZY["a2"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["a2"]["TextXAlignment"] = Enum.TextXAlignment.Left;
		AZY["a2"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Bold, Enum.FontStyle.Normal);
		AZY["a2"]["TextColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["a2"]["Size"] = UDim2.new(0.657156765460968, 0, 0.3310898244380951, 0);
		AZY["a2"]["Text"] = [[UI Slider Fixes And Textbox]];
		AZY["a2"]["Name"] = [[Desc]];
		AZY["a2"]["BackgroundTransparency"] = 1;
		AZY["a2"]["Position"] = UDim2.new(0.34299999475479126, 0, 0.4300000071525574, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Changelogs.Credits.ScrollingFrame.Person.Desc.UITextSizeConstraint
		AZY["a3"] = Instance.new("UITextSizeConstraint", AZY["a2"]);
		AZY["a3"]["MaxTextSize"] = 25;

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Changelogs.Changelog
		AZY["a4"] = Instance.new("Frame", AZY["87"]);
		AZY["a4"]["BackgroundColor3"] = Color3.fromRGB(0, 0, 0);
		AZY["a4"]["BackgroundTransparency"] = 0.550000011920929;
		AZY["a4"]["Size"] = UDim2.new(0.47281256318092346, 0, 0.7172916531562805, 0);
		AZY["a4"]["Position"] = UDim2.new(0.5088531970977783, 0, 0.020400196313858032, 0);
		AZY["a4"]["Name"] = [[Changelog]];

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Changelogs.Changelog.UICorner
		AZY["a5"] = Instance.new("UICorner", AZY["a4"]);
		AZY["a5"]["CornerRadius"] = UDim.new(0, 15);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Changelogs.Changelog.TextLogo
		AZY["a6"] = Instance.new("TextLabel", AZY["a4"]);
		AZY["a6"]["TextWrapped"] = true;
		AZY["a6"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["a6"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Bold, Enum.FontStyle.Normal);
		AZY["a6"]["TextSize"] = 19;
		AZY["a6"]["TextColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["a6"]["Size"] = UDim2.new(0.39918234944343567, 0, 0.14513146877288818, 0);
		AZY["a6"]["Text"] = [[Changelog]];
		AZY["a6"]["Name"] = [[TextLogo]];
		AZY["a6"]["BackgroundTransparency"] = 1;
		AZY["a6"]["Position"] = UDim2.new(0.05700000002980232, 0, 0.04899999871850014, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Changelogs.Changelog.TextLogo.UITextSizeConstraint
		AZY["a7"] = Instance.new("UITextSizeConstraint", AZY["a6"]);
		AZY["a7"]["MaxTextSize"] = 25;

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Changelogs.Changelog.Ver
		AZY["a8"] = Instance.new("TextLabel", AZY["a4"]);
		AZY["a8"]["TextWrapped"] = true;
		AZY["a8"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["a8"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Bold, Enum.FontStyle.Normal);
		AZY["a8"]["TextSize"] = 13;
		AZY["a8"]["TextColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["a8"]["Size"] = UDim2.new(0.240515798330307, 0, 0.14513146877288818, 0);
		AZY["a8"]["Text"] = [[v3.0.1]];
		AZY["a8"]["Name"] = [[Ver]];
		AZY["a8"]["BackgroundTransparency"] = 1;
		AZY["a8"]["Position"] = UDim2.new(0.6331158876419067, 0, 0.04900005832314491, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Changelogs.Changelog.Ver.UITextSizeConstraint
		AZY["a9"] = Instance.new("UITextSizeConstraint", AZY["a8"]);
		AZY["a9"]["MaxTextSize"] = 25;

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Changelogs.Changelog.Ver
		AZY["aa"] = Instance.new("TextLabel", AZY["a4"]);
		AZY["aa"]["TextWrapped"] = true;
		AZY["aa"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["aa"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Bold, Enum.FontStyle.Normal);
		AZY["aa"]["TextSize"] = 9;
		AZY["aa"]["TextColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["aa"]["Size"] = UDim2.new(0.0997123271226883, 0, 0.08936085551977158, 0);
		AZY["aa"]["Text"] = [[beta]];
		AZY["aa"]["Name"] = [[Ver]];
		AZY["aa"]["BackgroundTransparency"] = 1;
		AZY["aa"]["Position"] = UDim2.new(0.8399999737739563, 0, 0.0820000022649765, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Changelogs.Changelog.Ver.UITextSizeConstraint
		AZY["ab"] = Instance.new("UITextSizeConstraint", AZY["aa"]);
		AZY["ab"]["MaxTextSize"] = 25;

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Changelogs.Changelog.ScrollingFrame
		AZY["ac"] = Instance.new("ScrollingFrame", AZY["a4"]);
		AZY["ac"]["Active"] = true;
		AZY["ac"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["ac"]["BackgroundTransparency"] = 1;
		AZY["ac"]["Size"] = UDim2.new(0, 165, 0, 113);
		AZY["ac"]["ScrollBarImageColor3"] = Color3.fromRGB(255, 0, 14);
		AZY["ac"]["BorderColor3"] = Color3.fromRGB(54, 0, 2);
		AZY["ac"]["ScrollBarThickness"] = 5;
		AZY["ac"]["Position"] = UDim2.new(0.05699992552399635, 0, 0.20896704494953156, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Changelogs.Changelog.ScrollingFrame.ChangelogTab
		AZY["ad"] = Instance.new("Frame", AZY["ac"]);
		AZY["ad"]["BackgroundColor3"] = Color3.fromRGB(0, 0, 0);
		AZY["ad"]["BackgroundTransparency"] = 1;
		AZY["ad"]["Size"] = UDim2.new(0.8838858008384705, 0, 0.41258352994918823, 0);
		AZY["ad"]["Position"] = UDim2.new(-0.001135505735874176, 0, 0.008439034223556519, 0);
		AZY["ad"]["Name"] = [[ChangelogTab]];

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Changelogs.Changelog.ScrollingFrame.ChangelogTab.UICorner
		AZY["ae"] = Instance.new("UICorner", AZY["ad"]);
		AZY["ae"]["CornerRadius"] = UDim.new(0, 15);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Changelogs.Changelog.ScrollingFrame.ChangelogTab.TextLabel
		AZY["af"] = Instance.new("TextLabel", AZY["ad"]);
		AZY["af"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["af"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Regular, Enum.FontStyle.Normal);
		AZY["af"]["TextSize"] = 56;
		AZY["af"]["TextColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["af"]["Size"] = UDim2.new(0, 18, 0, 20);
		AZY["af"]["Text"] = [[.]];
		AZY["af"]["BackgroundTransparency"] = 1;
		AZY["af"]["Position"] = UDim2.new(-0.00024911601212807, 0, -0.08813343942165375, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Changelogs.Changelog.ScrollingFrame.ChangelogTab.TextLabel
		AZY["b0"] = Instance.new("TextLabel", AZY["ad"]);
		AZY["b0"]["BackgroundColor3"] = Color3.fromRGB(0, 187, 7);
		AZY["b0"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Bold, Enum.FontStyle.Normal);
		AZY["b0"]["TextSize"] = 14;
		AZY["b0"]["TextColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["b0"]["Size"] = UDim2.new(0, 29, 0, 14);
		AZY["b0"]["Text"] = [[New]];
		AZY["b0"]["Position"] = UDim2.new(0.10899999737739563, 0, 0.05000000074505806, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Changelogs.Changelog.ScrollingFrame.ChangelogTab.TextLabel.UICorner
		AZY["b1"] = Instance.new("UICorner", AZY["b0"]);
		AZY["b1"]["CornerRadius"] = UDim.new(0, 4);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Changelogs.Changelog.ScrollingFrame.ChangelogTab.TextLabel
		AZY["b2"] = Instance.new("TextLabel", AZY["ad"]);
		AZY["b2"]["TextWrapped"] = true;
		AZY["b2"]["TextYAlignment"] = Enum.TextYAlignment.Top;
		AZY["b2"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["b2"]["TextXAlignment"] = Enum.TextXAlignment.Left;
		AZY["b2"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Regular, Enum.FontStyle.Normal);
		AZY["b2"]["TextSize"] = 11;
		AZY["b2"]["TextColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["b2"]["Size"] = UDim2.new(0, 109, 0, 60);
		AZY["b2"]["Text"] = [[Floating icon now with addec functionality! In addition to opening the mod menu, holding it down will take you directly to your desired page]];
		AZY["b2"]["BackgroundTransparency"] = 1;
		AZY["b2"]["Position"] = UDim2.new(0.34079205989837646, 0, 0.04748288542032242, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Changelogs.Changelog.ScrollingFrame.ChangelogTab1
		AZY["b3"] = Instance.new("Frame", AZY["ac"]);
		AZY["b3"]["BackgroundColor3"] = Color3.fromRGB(0, 0, 0);
		AZY["b3"]["BackgroundTransparency"] = 1;
		AZY["b3"]["Size"] = UDim2.new(0.8838858008384705, 0, 0.41258352994918823, 0);
		AZY["b3"]["Position"] = UDim2.new(-0.0071961116045713425, 0, 0.20108048617839813, 0);
		AZY["b3"]["Name"] = [[ChangelogTab1]];

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Changelogs.Changelog.ScrollingFrame.ChangelogTab1.UICorner
		AZY["b4"] = Instance.new("UICorner", AZY["b3"]);
		AZY["b4"]["CornerRadius"] = UDim.new(0, 15);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Changelogs.Changelog.ScrollingFrame.ChangelogTab1.TextLabel
		AZY["b5"] = Instance.new("TextLabel", AZY["b3"]);
		AZY["b5"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["b5"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Regular, Enum.FontStyle.Normal);
		AZY["b5"]["TextSize"] = 56;
		AZY["b5"]["TextColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["b5"]["Size"] = UDim2.new(0, 18, 0, 20);
		AZY["b5"]["Text"] = [[.]];
		AZY["b5"]["BackgroundTransparency"] = 1;
		AZY["b5"]["Position"] = UDim2.new(-0.00024911601212807, 0, -0.08813343942165375, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Changelogs.Changelog.ScrollingFrame.ChangelogTab1.TextLabel
		AZY["b6"] = Instance.new("TextLabel", AZY["b3"]);
		AZY["b6"]["BackgroundColor3"] = Color3.fromRGB(0, 187, 7);
		AZY["b6"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Bold, Enum.FontStyle.Normal);
		AZY["b6"]["TextSize"] = 14;
		AZY["b6"]["TextColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["b6"]["Size"] = UDim2.new(0, 29, 0, 14);
		AZY["b6"]["Text"] = [[New]];
		AZY["b6"]["Position"] = UDim2.new(0.10899999737739563, 0, 0.05000000074505806, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Changelogs.Changelog.ScrollingFrame.ChangelogTab1.TextLabel.UICorner
		AZY["b7"] = Instance.new("UICorner", AZY["b6"]);
		AZY["b7"]["CornerRadius"] = UDim.new(0, 4);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Changelogs.Changelog.ScrollingFrame.ChangelogTab1.TextLabel
		AZY["b8"] = Instance.new("TextLabel", AZY["b3"]);
		AZY["b8"]["TextWrapped"] = true;
		AZY["b8"]["TextYAlignment"] = Enum.TextYAlignment.Top;
		AZY["b8"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["b8"]["TextXAlignment"] = Enum.TextXAlignment.Left;
		AZY["b8"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Regular, Enum.FontStyle.Normal);
		AZY["b8"]["TextSize"] = 11;
		AZY["b8"]["TextColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["b8"]["Size"] = UDim2.new(0, 109, 0, 60);
		AZY["b8"]["Text"] = [[Stunning Design with breathtaking graphical elements, animations, colors and beautiful icons!]];
		AZY["b8"]["BackgroundTransparency"] = 1;
		AZY["b8"]["Position"] = UDim2.new(0.34079205989837646, 0, 0.04748288542032242, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Changelogs.Changelog.ScrollingFrame.ChangelogTab2
		AZY["b9"] = Instance.new("Frame", AZY["ac"]);
		AZY["b9"]["BackgroundColor3"] = Color3.fromRGB(0, 0, 0);
		AZY["b9"]["BackgroundTransparency"] = 1;
		AZY["b9"]["Size"] = UDim2.new(0.8838858008384705, 0, 0.41258352994918823, 0);
		AZY["b9"]["Position"] = UDim2.new(-0.0010000000474974513, 0, 0.3869999945163727, 0);
		AZY["b9"]["Name"] = [[ChangelogTab2]];

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Changelogs.Changelog.ScrollingFrame.ChangelogTab2.UICorner
		AZY["ba"] = Instance.new("UICorner", AZY["b9"]);
		AZY["ba"]["CornerRadius"] = UDim.new(0, 15);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Changelogs.Changelog.ScrollingFrame.ChangelogTab2.TextLabel
		AZY["bb"] = Instance.new("TextLabel", AZY["b9"]);
		AZY["bb"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["bb"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Regular, Enum.FontStyle.Normal);
		AZY["bb"]["TextSize"] = 56;
		AZY["bb"]["TextColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["bb"]["Size"] = UDim2.new(0, 18, 0, 20);
		AZY["bb"]["Text"] = [[.]];
		AZY["bb"]["BackgroundTransparency"] = 1;
		AZY["bb"]["Position"] = UDim2.new(-0.00024911601212807, 0, -0.08813343942165375, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Changelogs.Changelog.ScrollingFrame.ChangelogTab2.TextLabel
		AZY["bc"] = Instance.new("TextLabel", AZY["b9"]);
		AZY["bc"]["BackgroundColor3"] = Color3.fromRGB(0, 187, 7);
		AZY["bc"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Bold, Enum.FontStyle.Normal);
		AZY["bc"]["TextSize"] = 14;
		AZY["bc"]["TextColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["bc"]["Size"] = UDim2.new(0, 29, 0, 14);
		AZY["bc"]["Text"] = [[New]];
		AZY["bc"]["Position"] = UDim2.new(0.10899999737739563, 0, 0.05000000074505806, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Changelogs.Changelog.ScrollingFrame.ChangelogTab2.TextLabel.UICorner
		AZY["bd"] = Instance.new("UICorner", AZY["bc"]);
		AZY["bd"]["CornerRadius"] = UDim.new(0, 4);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Changelogs.Changelog.ScrollingFrame.ChangelogTab2.TextLabel
		AZY["be"] = Instance.new("TextLabel", AZY["b9"]);
		AZY["be"]["TextWrapped"] = true;
		AZY["be"]["TextYAlignment"] = Enum.TextYAlignment.Top;
		AZY["be"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["be"]["TextXAlignment"] = Enum.TextXAlignment.Left;
		AZY["be"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Regular, Enum.FontStyle.Normal);
		AZY["be"]["TextSize"] = 11;
		AZY["be"]["TextColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["be"]["Size"] = UDim2.new(0, 109, 0, 60);
		AZY["be"]["Text"] = [[Window design with comfortable UI movement and a semi-transparent mod menu for a less intrusive gaming experience!]];
		AZY["be"]["BackgroundTransparency"] = 1;
		AZY["be"]["Position"] = UDim2.new(0.34079205989837646, 0, 0.04748288542032242, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Changelogs.Changelog.ScrollingFrame.ChangelogTab3
		AZY["bf"] = Instance.new("Frame", AZY["ac"]);
		AZY["bf"]["BackgroundColor3"] = Color3.fromRGB(0, 0, 0);
		AZY["bf"]["BackgroundTransparency"] = 1;
		AZY["bf"]["Size"] = UDim2.new(0.8838858008384705, 0, 0.41258352994918823, 0);
		AZY["bf"]["Position"] = UDim2.new(0.005060605704784393, 0, 0.5927019119262695, 0);
		AZY["bf"]["Name"] = [[ChangelogTab3]];

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Changelogs.Changelog.ScrollingFrame.ChangelogTab3.UICorner
		AZY["c0"] = Instance.new("UICorner", AZY["bf"]);
		AZY["c0"]["CornerRadius"] = UDim.new(0, 15);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Changelogs.Changelog.ScrollingFrame.ChangelogTab3.TextLabel
		AZY["c1"] = Instance.new("TextLabel", AZY["bf"]);
		AZY["c1"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["c1"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Regular, Enum.FontStyle.Normal);
		AZY["c1"]["TextSize"] = 56;
		AZY["c1"]["TextColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["c1"]["Size"] = UDim2.new(0, 18, 0, 20);
		AZY["c1"]["Text"] = [[.]];
		AZY["c1"]["BackgroundTransparency"] = 1;
		AZY["c1"]["Position"] = UDim2.new(-0.00024911601212807, 0, -0.08813343942165375, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Changelogs.Changelog.ScrollingFrame.ChangelogTab3.TextLabel
		AZY["c2"] = Instance.new("TextLabel", AZY["bf"]);
		AZY["c2"]["BackgroundColor3"] = Color3.fromRGB(0, 187, 7);
		AZY["c2"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Bold, Enum.FontStyle.Normal);
		AZY["c2"]["TextSize"] = 14;
		AZY["c2"]["TextColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["c2"]["Size"] = UDim2.new(0, 29, 0, 14);
		AZY["c2"]["Text"] = [[New]];
		AZY["c2"]["Position"] = UDim2.new(0.10899999737739563, 0, 0.05000000074505806, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Changelogs.Changelog.ScrollingFrame.ChangelogTab3.TextLabel.UICorner
		AZY["c3"] = Instance.new("UICorner", AZY["c2"]);
		AZY["c3"]["CornerRadius"] = UDim.new(0, 4);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Changelogs.Changelog.ScrollingFrame.ChangelogTab3.TextLabel
		AZY["c4"] = Instance.new("TextLabel", AZY["bf"]);
		AZY["c4"]["TextWrapped"] = true;
		AZY["c4"]["TextYAlignment"] = Enum.TextYAlignment.Top;
		AZY["c4"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["c4"]["TextXAlignment"] = Enum.TextXAlignment.Left;
		AZY["c4"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Regular, Enum.FontStyle.Normal);
		AZY["c4"]["TextSize"] = 11;
		AZY["c4"]["TextColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["c4"]["Size"] = UDim2.new(0, 109, 0, 60);
		AZY["c4"]["Text"] = [[Info page with all information about our team and our social media! Plus an intuitive and well-designed changelog.]];
		AZY["c4"]["BackgroundTransparency"] = 1;
		AZY["c4"]["Position"] = UDim2.new(0.34079205989837646, 0, 0.04748288542032242, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Changelogs.Communications
		AZY["c5"] = Instance.new("Frame", AZY["87"]);
		AZY["c5"]["BackgroundColor3"] = Color3.fromRGB(0, 0, 0);
		AZY["c5"]["BackgroundTransparency"] = 0.550000011920929;
		AZY["c5"]["Size"] = UDim2.new(0.47281256318092346, 0, 0.2235966920852661, 0);
		AZY["c5"]["Position"] = UDim2.new(0.5088531970977783, 0, 0.774535596370697, 0);
		AZY["c5"]["Name"] = [[Communications]];

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Changelogs.Communications.UICorner
		AZY["c6"] = Instance.new("UICorner", AZY["c5"]);
		AZY["c6"]["CornerRadius"] = UDim.new(0, 15);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Changelogs.Communications.Copy
		AZY["c7"] = Instance.new("TextButton", AZY["c5"]);
		AZY["c7"]["TextWrapped"] = true;
		AZY["c7"]["BackgroundColor3"] = Color3.fromRGB(255, 0, 0);
		AZY["c7"]["TextSize"] = 12;
		AZY["c7"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Bold, Enum.FontStyle.Normal);
		AZY["c7"]["TextColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["c7"]["Size"] = UDim2.new(0.41421639919281006, 0, 0.503000020980835, 0);
		AZY["c7"]["Name"] = [[Copy]];
		AZY["c7"]["Text"] = [[Copy Link]];
		AZY["c7"]["Position"] = UDim2.new(0.03737286850810051, 0, 0.22850681841373444, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Changelogs.Communications.Copy.UICorner
		AZY["c8"] = Instance.new("UICorner", AZY["c7"]);
		AZY["c8"]["CornerRadius"] = UDim.new(0, 6);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Changelogs.Communications.Copy.LocalScript
		AZY["c9"] = Instance.new("LocalScript", AZY["c7"]);


		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Changelogs.Communications.TextLogo
		AZY["ca"] = Instance.new("TextLabel", AZY["c5"]);
		AZY["ca"]["TextWrapped"] = true;
		AZY["ca"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["ca"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Bold, Enum.FontStyle.Normal);
		AZY["ca"]["TextSize"] = 19;
		AZY["ca"]["TextColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["ca"]["Size"] = UDim2.new(0.14990141987800598, 0, 0.2844810485839844, 0);
		AZY["ca"]["Text"] = [[Or]];
		AZY["ca"]["Name"] = [[TextLogo]];
		AZY["ca"]["BackgroundTransparency"] = 1;
		AZY["ca"]["Position"] = UDim2.new(0.45584943890571594, 0, 0.30038517713546753, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Changelogs.Communications.TextLogo.UITextSizeConstraint
		AZY["cb"] = Instance.new("UITextSizeConstraint", AZY["ca"]);
		AZY["cb"]["MaxTextSize"] = 25;

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Changelogs.Communications.TextLogo
		AZY["cc"] = Instance.new("TextLabel", AZY["c5"]);
		AZY["cc"]["TextWrapped"] = true;
		AZY["cc"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["cc"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Bold, Enum.FontStyle.Normal);
		AZY["cc"]["TextSize"] = 19;
		AZY["cc"]["TextColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["cc"]["Size"] = UDim2.new(0.4056611955165863, 0, 0.2844810485839844, 0);
		AZY["cc"]["Text"] = [[AZY#0348]];
		AZY["cc"]["Name"] = [[TextLogo]];
		AZY["cc"]["BackgroundTransparency"] = 1;
		AZY["cc"]["Position"] = UDim2.new(0.5839999914169312, 0, 0.29899999499320984, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Changelogs.Communications.TextLogo.UITextSizeConstraint
		AZY["cd"] = Instance.new("UITextSizeConstraint", AZY["cc"]);
		AZY["cd"]["MaxTextSize"] = 25;

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.BuiltInHax
		AZY["ce"] = Instance.new("Frame", AZY["2b"]);
		AZY["ce"]["BackgroundColor3"] = Color3.fromRGB(0, 0, 0);
		AZY["ce"]["BackgroundTransparency"] = 0.550000011920929;
		AZY["ce"]["Size"] = UDim2.new(0.831805408000946, 0, 0.7551097869873047, 0);
		AZY["ce"]["Position"] = UDim2.new(0.1409205049276352, 0, 0.20551720261573792, 0);
		AZY["ce"]["Visible"] = false;
		AZY["ce"]["Name"] = [[BuiltInHax]];

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.BuiltInHax.UICorner
		AZY["cf"] = Instance.new("UICorner", AZY["ce"]);
		AZY["cf"]["CornerRadius"] = UDim.new(0, 15);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.BuiltInHax.HaxPage
		AZY["d0"] = Instance.new("Frame", AZY["ce"]);
		AZY["d0"]["BackgroundColor3"] = Color3.fromRGB(0, 0, 0);
		AZY["d0"]["BackgroundTransparency"] = 1;
		AZY["d0"]["Size"] = UDim2.new(0.6116291880607605, 0, 1.0292569398880005, 0);
		AZY["d0"]["Position"] = UDim2.new(0.3700365424156189, 0, -0.03249453008174896, 0);
		AZY["d0"]["Name"] = [[HaxPage]];

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.BuiltInHax.HaxPage.TextWs
		AZY["d1"] = Instance.new("TextLabel", AZY["d0"]);
		AZY["d1"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["d1"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Bold, Enum.FontStyle.Normal);
		AZY["d1"]["TextSize"] = 12;
		AZY["d1"]["TextColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["d1"]["Size"] = UDim2.new(0, 50, 0, 11);
		AZY["d1"]["Text"] = [[Speed]];
		AZY["d1"]["Name"] = [[TextWs]];
		AZY["d1"]["BackgroundTransparency"] = 1;
		AZY["d1"]["Position"] = UDim2.new(0.5411151647567749, 0, 0.8930000066757202, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.BuiltInHax.HaxPage.TextJp
		AZY["d2"] = Instance.new("TextLabel", AZY["d0"]);
		AZY["d2"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["d2"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Bold, Enum.FontStyle.Normal);
		AZY["d2"]["TextSize"] = 12;
		AZY["d2"]["TextColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["d2"]["Size"] = UDim2.new(0, 50, 0, 11);
		AZY["d2"]["Text"] = [[Jump]];
		AZY["d2"]["Name"] = [[TextJp]];
		AZY["d2"]["BackgroundTransparency"] = 1;
		AZY["d2"]["Position"] = UDim2.new(0.7466657161712646, 0, 0.8930000066757202, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.BuiltInHax.HaxPage.TextGrav
		AZY["d3"] = Instance.new("TextLabel", AZY["d0"]);
		AZY["d3"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["d3"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Bold, Enum.FontStyle.Normal);
		AZY["d3"]["TextSize"] = 12;
		AZY["d3"]["TextColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["d3"]["Size"] = UDim2.new(0, 50, 0, 11);
		AZY["d3"]["Text"] = [[Gravity]];
		AZY["d3"]["Name"] = [[TextGrav]];
		AZY["d3"]["BackgroundTransparency"] = 1;
		AZY["d3"]["Position"] = UDim2.new(0.3269999921321869, 0, 0.8930000066757202, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.BuiltInHax.HaxPage.ToggleGrav
		AZY["d4"] = Instance.new("TextButton", AZY["d0"]);
		AZY["d4"]["BackgroundColor3"] = Color3.fromRGB(146, 0, 0);
		AZY["d4"]["TextSize"] = 14;
		AZY["d4"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Regular, Enum.FontStyle.Normal);
		AZY["d4"]["TextColor3"] = Color3.fromRGB(0, 0, 0);
		AZY["d4"]["Size"] = UDim2.new(0, 15, 0, 15);
		AZY["d4"]["Name"] = [[ToggleGrav]];
		AZY["d4"]["Text"] = [[]];
		AZY["d4"]["Position"] = UDim2.new(0.40253645181655884, 0, 0.801304280757904, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.BuiltInHax.HaxPage.ToggleGrav.UICorner
		AZY["d5"] = Instance.new("UICorner", AZY["d4"]);
		AZY["d5"]["CornerRadius"] = UDim.new(100, 100);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.BuiltInHax.HaxPage.ToggleGrav.LocalScript
		AZY["d6"] = Instance.new("LocalScript", AZY["d4"]);


		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.BuiltInHax.HaxPage.ToggleJp
		AZY["d7"] = Instance.new("TextButton", AZY["d0"]);
		AZY["d7"]["BackgroundColor3"] = Color3.fromRGB(146, 0, 0);
		AZY["d7"]["TextSize"] = 14;
		AZY["d7"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Regular, Enum.FontStyle.Normal);
		AZY["d7"]["TextColor3"] = Color3.fromRGB(0, 0, 0);
		AZY["d7"]["Size"] = UDim2.new(0, 15, 0, 15);
		AZY["d7"]["Name"] = [[ToggleJp]];
		AZY["d7"]["Text"] = [[]];
		AZY["d7"]["Position"] = UDim2.new(0.8222021460533142, 0, 0.801304280757904, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.BuiltInHax.HaxPage.ToggleJp.UICorner
		AZY["d8"] = Instance.new("UICorner", AZY["d7"]);
		AZY["d8"]["CornerRadius"] = UDim.new(100, 100);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.BuiltInHax.HaxPage.ToggleJp.LocalScript
		AZY["d9"] = Instance.new("LocalScript", AZY["d7"]);


		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.BuiltInHax.HaxPage.ToggleWs
		AZY["da"] = Instance.new("TextButton", AZY["d0"]);
		AZY["da"]["BackgroundColor3"] = Color3.fromRGB(146, 0, 0);
		AZY["da"]["TextSize"] = 14;
		AZY["da"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Regular, Enum.FontStyle.Normal);
		AZY["da"]["TextColor3"] = Color3.fromRGB(0, 0, 0);
		AZY["da"]["Size"] = UDim2.new(0, 15, 0, 15);
		AZY["da"]["Name"] = [[ToggleWs]];
		AZY["da"]["Text"] = [[]];
		AZY["da"]["Position"] = UDim2.new(0.6166515946388245, 0, 0.801304280757904, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.BuiltInHax.HaxPage.ToggleWs.UICorner
		AZY["db"] = Instance.new("UICorner", AZY["da"]);
		AZY["db"]["CornerRadius"] = UDim.new(100, 100);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.BuiltInHax.HaxPage.ToggleWs.LocalScript
		AZY["dc"] = Instance.new("LocalScript", AZY["da"]);


		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.BuiltInHax.HaxPage.WsS
		AZY["dd"] = Instance.new("ImageButton", AZY["d0"]);
		AZY["dd"]["Active"] = false;
		AZY["dd"]["BorderSizePixel"] = 0;
		AZY["dd"]["SliceCenter"] = Rect.new(100, 100, 100, 100);
		AZY["dd"]["ScaleType"] = Enum.ScaleType.Slice;
		AZY["dd"]["SliceScale"] = 0.11999999731779099;
		AZY["dd"]["ImageTransparency"] = 1;
		AZY["dd"]["BackgroundColor3"] = Color3.fromRGB(22, 22, 22);
		AZY["dd"]["ImageColor3"] = Color3.fromRGB(32, 32, 32);
		AZY["dd"]["Selectable"] = false;
		AZY["dd"]["AnchorPoint"] = Vector2.new(0.5, 0.5);
		AZY["dd"]["Image"] = [[rbxassetid://3570695787]];
		AZY["dd"]["Size"] = UDim2.new(0, 119, 0, 31);
		AZY["dd"]["Name"] = [[WsS]];
		AZY["dd"]["Rotation"] = -90;
		AZY["dd"]["Position"] = UDim2.new(0.6499999761581421, 0, 0.4399999976158142, 0);
		AZY["dd"]["BackgroundTransparency"] = 1;

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.BuiltInHax.HaxPage.WsS.SliderButton
		AZY["de"] = Instance.new("ImageLabel", AZY["dd"]);
		AZY["de"]["SliceCenter"] = Rect.new(100, 100, 100, 100);
		AZY["de"]["ScaleType"] = Enum.ScaleType.Slice;
		AZY["de"]["BackgroundColor3"] = Color3.fromRGB(71, 71, 71);
		AZY["de"]["ImageColor3"] = Color3.fromRGB(146, 0, 0);
		AZY["de"]["SliceScale"] = 0.11999999731779099;
		AZY["de"]["Selectable"] = true;
		AZY["de"]["Image"] = [[rbxassetid://3570695787]];
		AZY["de"]["Size"] = UDim2.new(0, 25, 1, 0);
		AZY["de"]["Active"] = true;
		AZY["de"]["Name"] = [[SliderButton]];
		AZY["de"]["BackgroundTransparency"] = 1;

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.BuiltInHax.HaxPage.WsS.SliderButton.LocalScript
		AZY["df"] = Instance.new("LocalScript", AZY["de"]);


		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.BuiltInHax.HaxPage.WsS.Border
		AZY["e0"] = Instance.new("ImageLabel", AZY["dd"]);
		AZY["e0"]["ZIndex"] = -1;
		AZY["e0"]["SliceCenter"] = Rect.new(100, 100, 100, 100);
		AZY["e0"]["ScaleType"] = Enum.ScaleType.Slice;
		AZY["e0"]["BackgroundColor3"] = Color3.fromRGB(62, 62, 62);
		AZY["e0"]["ImageColor3"] = Color3.fromRGB(71, 71, 71);
		AZY["e0"]["SliceScale"] = 0.23999999463558197;
		AZY["e0"]["ImageTransparency"] = 1;
		AZY["e0"]["AnchorPoint"] = Vector2.new(0.5, 0.5);
		AZY["e0"]["Image"] = [[rbxassetid://3570695787]];
		AZY["e0"]["Size"] = UDim2.new(1, 12, 1, 12);
		AZY["e0"]["Name"] = [[Border]];
		AZY["e0"]["BackgroundTransparency"] = 0.6000000238418579;
		AZY["e0"]["Position"] = UDim2.new(0.5, 0, 0.5, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.BuiltInHax.HaxPage.WsS.Border.UICorner
		AZY["e1"] = Instance.new("UICorner", AZY["e0"]);
		AZY["e1"]["CornerRadius"] = UDim.new(0, 12);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.BuiltInHax.HaxPage.WsS.StripedPattern
		AZY["e2"] = Instance.new("ImageLabel", AZY["dd"]);
		AZY["e2"]["BorderSizePixel"] = 0;
		AZY["e2"]["ScaleType"] = Enum.ScaleType.Tile;
		AZY["e2"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["e2"]["ImageColor3"] = Color3.fromRGB(32, 32, 32);
		AZY["e2"]["ImageTransparency"] = 1;
		AZY["e2"]["AnchorPoint"] = Vector2.new(0.5, 0);
		AZY["e2"]["Image"] = [[rbxassetid://4925116997]];
		AZY["e2"]["TileSize"] = UDim2.new(0, 25, 1, 0);
		AZY["e2"]["Size"] = UDim2.new(1, -25, 1, 0);
		AZY["e2"]["Name"] = [[StripedPattern]];
		AZY["e2"]["BackgroundTransparency"] = 1;
		AZY["e2"]["Position"] = UDim2.new(0.5, 0, 0, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.BuiltInHax.HaxPage.WsS.StripedPattern.UIGradient
		AZY["e3"] = Instance.new("UIGradient", AZY["e2"]);
		AZY["e3"]["Rotation"] = 90;
		AZY["e3"]["Color"] = ColorSequence.new{ColorSequenceKeypoint.new(0.000, Color3.fromRGB(255, 255, 255)),ColorSequenceKeypoint.new(1.000, Color3.fromRGB(0, 0, 0))};

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.BuiltInHax.HaxPage.WsS.ImageLabel
		AZY["e4"] = Instance.new("ImageLabel", AZY["dd"]);
		AZY["e4"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["e4"]["Image"] = [[rbxassetid://12572149271]];
		AZY["e4"]["Size"] = UDim2.new(0, 35, 0, 35);
		AZY["e4"]["Rotation"] = 90;
		AZY["e4"]["BackgroundTransparency"] = 1;
		AZY["e4"]["Position"] = UDim2.new(-0.017000000923871994, 0, -0.10000000149011612, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.BuiltInHax.HaxPage.WsS.TextLabel
		AZY["e5"] = Instance.new("TextBox", AZY["dd"]);
		AZY["e5"]["CursorPosition"] = -1;
		AZY["e5"]["ZIndex"] = 2;
		AZY["e5"]["TextSize"] = 13;
		AZY["e5"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["e5"]["TextColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["e5"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Bold, Enum.FontStyle.Normal);
		AZY["e5"]["AnchorPoint"] = Vector2.new(1, 0);
		AZY["e5"]["BackgroundTransparency"] = 1;
		AZY["e5"]["Size"] = UDim2.new(0, 50, 1, 0);
		AZY["e5"]["Text"] = [[0%]];
		AZY["e5"]["Position"] = UDim2.new(0, 137, 0, 0);
		AZY["e5"]["Rotation"] = 90;
		AZY["e5"]["Name"] = [[TextLabel]];

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.BuiltInHax.HaxPage.JpS
		AZY["e6"] = Instance.new("ImageButton", AZY["d0"]);
		AZY["e6"]["Active"] = false;
		AZY["e6"]["BorderSizePixel"] = 0;
		AZY["e6"]["SliceCenter"] = Rect.new(100, 100, 100, 100);
		AZY["e6"]["ScaleType"] = Enum.ScaleType.Slice;
		AZY["e6"]["SliceScale"] = 0.11999999731779099;
		AZY["e6"]["ImageTransparency"] = 1;
		AZY["e6"]["BackgroundColor3"] = Color3.fromRGB(22, 22, 22);
		AZY["e6"]["ImageColor3"] = Color3.fromRGB(32, 32, 32);
		AZY["e6"]["Selectable"] = false;
		AZY["e6"]["AnchorPoint"] = Vector2.new(0.5, 0.5);
		AZY["e6"]["Image"] = [[rbxassetid://3570695787]];
		AZY["e6"]["Size"] = UDim2.new(0, 119, 0, 31);
		AZY["e6"]["Name"] = [[JpS]];
		AZY["e6"]["Rotation"] = -90;
		AZY["e6"]["Position"] = UDim2.new(0.8600000143051147, 0, 0.4399999976158142, 0);
		AZY["e6"]["BackgroundTransparency"] = 1;

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.BuiltInHax.HaxPage.JpS.SliderButton
		AZY["e7"] = Instance.new("ImageLabel", AZY["e6"]);
		AZY["e7"]["SliceCenter"] = Rect.new(100, 100, 100, 100);
		AZY["e7"]["ScaleType"] = Enum.ScaleType.Slice;
		AZY["e7"]["BackgroundColor3"] = Color3.fromRGB(71, 71, 71);
		AZY["e7"]["ImageColor3"] = Color3.fromRGB(146, 0, 0);
		AZY["e7"]["SliceScale"] = 0.11999999731779099;
		AZY["e7"]["Selectable"] = true;
		AZY["e7"]["Image"] = [[rbxassetid://3570695787]];
		AZY["e7"]["Size"] = UDim2.new(0, 25, 1, 0);
		AZY["e7"]["Active"] = true;
		AZY["e7"]["Name"] = [[SliderButton]];
		AZY["e7"]["BackgroundTransparency"] = 1;

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.BuiltInHax.HaxPage.JpS.SliderButton.LocalScript
		AZY["e8"] = Instance.new("LocalScript", AZY["e7"]);


		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.BuiltInHax.HaxPage.JpS.Border
		AZY["e9"] = Instance.new("ImageLabel", AZY["e6"]);
		AZY["e9"]["ZIndex"] = -1;
		AZY["e9"]["SliceCenter"] = Rect.new(100, 100, 100, 100);
		AZY["e9"]["ScaleType"] = Enum.ScaleType.Slice;
		AZY["e9"]["BackgroundColor3"] = Color3.fromRGB(62, 62, 62);
		AZY["e9"]["ImageColor3"] = Color3.fromRGB(71, 71, 71);
		AZY["e9"]["SliceScale"] = 0.23999999463558197;
		AZY["e9"]["ImageTransparency"] = 1;
		AZY["e9"]["AnchorPoint"] = Vector2.new(0.5, 0.5);
		AZY["e9"]["Image"] = [[rbxassetid://3570695787]];
		AZY["e9"]["Size"] = UDim2.new(1, 12, 1, 12);
		AZY["e9"]["Name"] = [[Border]];
		AZY["e9"]["BackgroundTransparency"] = 0.6000000238418579;
		AZY["e9"]["Position"] = UDim2.new(0.5, 0, 0.5, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.BuiltInHax.HaxPage.JpS.Border.UICorner
		AZY["ea"] = Instance.new("UICorner", AZY["e9"]);
		AZY["ea"]["CornerRadius"] = UDim.new(0, 12);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.BuiltInHax.HaxPage.JpS.StripedPattern
		AZY["eb"] = Instance.new("ImageLabel", AZY["e6"]);
		AZY["eb"]["BorderSizePixel"] = 0;
		AZY["eb"]["ScaleType"] = Enum.ScaleType.Tile;
		AZY["eb"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["eb"]["ImageColor3"] = Color3.fromRGB(32, 32, 32);
		AZY["eb"]["ImageTransparency"] = 1;
		AZY["eb"]["AnchorPoint"] = Vector2.new(0.5, 0);
		AZY["eb"]["Image"] = [[rbxassetid://4925116997]];
		AZY["eb"]["TileSize"] = UDim2.new(0, 25, 1, 0);
		AZY["eb"]["Size"] = UDim2.new(1, -25, 1, 0);
		AZY["eb"]["Name"] = [[StripedPattern]];
		AZY["eb"]["BackgroundTransparency"] = 1;
		AZY["eb"]["Position"] = UDim2.new(0.5, 0, 0, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.BuiltInHax.HaxPage.JpS.StripedPattern.UIGradient
		AZY["ec"] = Instance.new("UIGradient", AZY["eb"]);
		AZY["ec"]["Rotation"] = 90;
		AZY["ec"]["Color"] = ColorSequence.new{ColorSequenceKeypoint.new(0.000, Color3.fromRGB(255, 255, 255)),ColorSequenceKeypoint.new(1.000, Color3.fromRGB(0, 0, 0))};

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.BuiltInHax.HaxPage.JpS.ImageLabel
		AZY["ed"] = Instance.new("ImageLabel", AZY["e6"]);
		AZY["ed"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["ed"]["Image"] = [[rbxassetid://12582573514]];
		AZY["ed"]["Size"] = UDim2.new(0, 35, 0, 35);
		AZY["ed"]["Rotation"] = 90;
		AZY["ed"]["BackgroundTransparency"] = 1;
		AZY["ed"]["Position"] = UDim2.new(-0.017000000923871994, 0, -0.10000000149011612, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.BuiltInHax.HaxPage.JpS.TextLabel
		AZY["ee"] = Instance.new("TextBox", AZY["e6"]);
		AZY["ee"]["ZIndex"] = 2;
		AZY["ee"]["TextSize"] = 13;
		AZY["ee"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["ee"]["TextColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["ee"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Bold, Enum.FontStyle.Normal);
		AZY["ee"]["AnchorPoint"] = Vector2.new(1, 0);
		AZY["ee"]["BackgroundTransparency"] = 1;
		AZY["ee"]["Size"] = UDim2.new(0, 50, 1, 0);
		AZY["ee"]["Text"] = [[0%]];
		AZY["ee"]["Position"] = UDim2.new(0, 137, 0, 0);
		AZY["ee"]["Rotation"] = 90;
		AZY["ee"]["Name"] = [[TextLabel]];

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.BuiltInHax.HaxPage.GravS
		AZY["ef"] = Instance.new("ImageButton", AZY["d0"]);
		AZY["ef"]["Active"] = false;
		AZY["ef"]["BorderSizePixel"] = 0;
		AZY["ef"]["SliceCenter"] = Rect.new(100, 100, 100, 100);
		AZY["ef"]["ScaleType"] = Enum.ScaleType.Slice;
		AZY["ef"]["SliceScale"] = 0.11999999731779099;
		AZY["ef"]["ImageTransparency"] = 1;
		AZY["ef"]["BackgroundColor3"] = Color3.fromRGB(22, 22, 22);
		AZY["ef"]["ImageColor3"] = Color3.fromRGB(32, 32, 32);
		AZY["ef"]["Selectable"] = false;
		AZY["ef"]["AnchorPoint"] = Vector2.new(0.5, 0.5);
		AZY["ef"]["Image"] = [[rbxassetid://3570695787]];
		AZY["ef"]["Size"] = UDim2.new(0, 119, 0, 31);
		AZY["ef"]["Name"] = [[GravS]];
		AZY["ef"]["Rotation"] = -90;
		AZY["ef"]["Position"] = UDim2.new(0.4359999895095825, 0, 0.4399999976158142, 0);
		AZY["ef"]["BackgroundTransparency"] = 1;

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.BuiltInHax.HaxPage.GravS.SliderButton
		AZY["f0"] = Instance.new("ImageLabel", AZY["ef"]);
		AZY["f0"]["SliceCenter"] = Rect.new(100, 100, 100, 100);
		AZY["f0"]["ScaleType"] = Enum.ScaleType.Slice;
		AZY["f0"]["BackgroundColor3"] = Color3.fromRGB(71, 71, 71);
		AZY["f0"]["ImageColor3"] = Color3.fromRGB(146, 0, 0);
		AZY["f0"]["SliceScale"] = 0.11999999731779099;
		AZY["f0"]["Selectable"] = true;
		AZY["f0"]["Image"] = [[rbxassetid://3570695787]];
		AZY["f0"]["Size"] = UDim2.new(0, 25, 1, 0);
		AZY["f0"]["Active"] = true;
		AZY["f0"]["Name"] = [[SliderButton]];
		AZY["f0"]["BackgroundTransparency"] = 1;

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.BuiltInHax.HaxPage.GravS.SliderButton.LocalScript
		AZY["f1"] = Instance.new("LocalScript", AZY["f0"]);


		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.BuiltInHax.HaxPage.GravS.Border
		AZY["f2"] = Instance.new("ImageLabel", AZY["ef"]);
		AZY["f2"]["ZIndex"] = -1;
		AZY["f2"]["SliceCenter"] = Rect.new(100, 100, 100, 100);
		AZY["f2"]["ScaleType"] = Enum.ScaleType.Slice;
		AZY["f2"]["BackgroundColor3"] = Color3.fromRGB(62, 62, 62);
		AZY["f2"]["ImageColor3"] = Color3.fromRGB(71, 71, 71);
		AZY["f2"]["SliceScale"] = 0.23999999463558197;
		AZY["f2"]["ImageTransparency"] = 1;
		AZY["f2"]["AnchorPoint"] = Vector2.new(0.5, 0.5);
		AZY["f2"]["Image"] = [[rbxassetid://3570695787]];
		AZY["f2"]["Size"] = UDim2.new(1, 12, 1, 12);
		AZY["f2"]["Name"] = [[Border]];
		AZY["f2"]["BackgroundTransparency"] = 0.6000000238418579;
		AZY["f2"]["Position"] = UDim2.new(0.5, 0, 0.5, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.BuiltInHax.HaxPage.GravS.Border.UICorner
		AZY["f3"] = Instance.new("UICorner", AZY["f2"]);
		AZY["f3"]["CornerRadius"] = UDim.new(0, 12);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.BuiltInHax.HaxPage.GravS.StripedPattern
		AZY["f4"] = Instance.new("ImageLabel", AZY["ef"]);
		AZY["f4"]["BorderSizePixel"] = 0;
		AZY["f4"]["ScaleType"] = Enum.ScaleType.Tile;
		AZY["f4"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["f4"]["ImageColor3"] = Color3.fromRGB(32, 32, 32);
		AZY["f4"]["ImageTransparency"] = 1;
		AZY["f4"]["AnchorPoint"] = Vector2.new(0.5, 0);
		AZY["f4"]["Image"] = [[rbxassetid://4925116997]];
		AZY["f4"]["TileSize"] = UDim2.new(0, 25, 1, 0);
		AZY["f4"]["Size"] = UDim2.new(1, -25, 1, 0);
		AZY["f4"]["Name"] = [[StripedPattern]];
		AZY["f4"]["BackgroundTransparency"] = 1;
		AZY["f4"]["Position"] = UDim2.new(0.5, 0, 0, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.BuiltInHax.HaxPage.GravS.StripedPattern.UIGradient
		AZY["f5"] = Instance.new("UIGradient", AZY["f4"]);
		AZY["f5"]["Rotation"] = 90;
		AZY["f5"]["Color"] = ColorSequence.new{ColorSequenceKeypoint.new(0.000, Color3.fromRGB(255, 255, 255)),ColorSequenceKeypoint.new(1.000, Color3.fromRGB(0, 0, 0))};

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.BuiltInHax.HaxPage.GravS.ImageLabel
		AZY["f6"] = Instance.new("ImageLabel", AZY["ef"]);
		AZY["f6"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["f6"]["Image"] = [[rbxassetid://12582575947]];
		AZY["f6"]["Size"] = UDim2.new(0, 35, 0, 35);
		AZY["f6"]["Rotation"] = 90;
		AZY["f6"]["BackgroundTransparency"] = 1;
		AZY["f6"]["Position"] = UDim2.new(-0.017000000923871994, 0, -0.10000000149011612, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.BuiltInHax.HaxPage.GravS.TextLabel
		AZY["f7"] = Instance.new("TextBox", AZY["ef"]);
		AZY["f7"]["ZIndex"] = 2;
		AZY["f7"]["TextSize"] = 13;
		AZY["f7"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["f7"]["TextColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["f7"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Bold, Enum.FontStyle.Normal);
		AZY["f7"]["AnchorPoint"] = Vector2.new(1, 0);
		AZY["f7"]["BackgroundTransparency"] = 1;
		AZY["f7"]["Size"] = UDim2.new(0, 50, 1, 0);
		AZY["f7"]["Text"] = [[0%]];
		AZY["f7"]["Position"] = UDim2.new(0, 137, 0, 0);
		AZY["f7"]["Rotation"] = 90;
		AZY["f7"]["Name"] = [[TextLabel]];

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.BuiltInHax.HaxPage.Grav
		AZY["f8"] = Instance.new("BoolValue", AZY["d0"]);
		AZY["f8"]["Name"] = [[Grav]];

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.BuiltInHax.HaxPage.Jp
		AZY["f9"] = Instance.new("BoolValue", AZY["d0"]);
		AZY["f9"]["Name"] = [[Jp]];

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.BuiltInHax.HaxPage.Ws
		AZY["fa"] = Instance.new("BoolValue", AZY["d0"]);
		AZY["fa"]["Name"] = [[Ws]];

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.BuiltInHax.Scripts
		AZY["fb"] = Instance.new("Folder", AZY["ce"]);
		AZY["fb"]["Name"] = [[Scripts]];

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.BuiltInHax.Scripts.Aimbot
		AZY["fc"] = Instance.new("TextButton", AZY["fb"]);
		AZY["fc"]["TextWrapped"] = true;
		AZY["fc"]["TextXAlignment"] = Enum.TextXAlignment.Left;
		AZY["fc"]["BackgroundColor3"] = Color3.fromRGB(255, 0, 0);
		AZY["fc"]["TextSize"] = 13;
		AZY["fc"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Bold, Enum.FontStyle.Normal);
		AZY["fc"]["TextColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["fc"]["Size"] = UDim2.new(0.2280000001192093, 0, 0.09600000083446503, 0);
		AZY["fc"]["Name"] = [[Aimbot]];
		AZY["fc"]["Text"] = [[       AimBot]];
		AZY["fc"]["Position"] = UDim2.new(0.030552715063095093, 0, 0.3302992284297943, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.BuiltInHax.Scripts.Aimbot.UICorner
		AZY["fd"] = Instance.new("UICorner", AZY["fc"]);
		AZY["fd"]["CornerRadius"] = UDim.new(0, 5);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.BuiltInHax.Scripts.Aimbot.LocalScript
		AZY["fe"] = Instance.new("LocalScript", AZY["fc"]);


		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.BuiltInHax.Scripts.Aimbot.Info
		AZY["ff"] = Instance.new("ImageLabel", AZY["fc"]);
		AZY["ff"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["ff"]["Image"] = [[rbxassetid://12585776892]];
		AZY["ff"]["Size"] = UDim2.new(0, 16, 0, 16);
		AZY["ff"]["Name"] = [[Info]];
		AZY["ff"]["BackgroundTransparency"] = 1;
		AZY["ff"]["Position"] = UDim2.new(0.7910000085830688, 0, 0.09000000357627869, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.BuiltInHax.Scripts.Btools
		AZY["100"] = Instance.new("TextButton", AZY["fb"]);
		AZY["100"]["TextWrapped"] = true;
		AZY["100"]["TextXAlignment"] = Enum.TextXAlignment.Left;
		AZY["100"]["BackgroundColor3"] = Color3.fromRGB(255, 0, 0);
		AZY["100"]["TextSize"] = 13;
		AZY["100"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Bold, Enum.FontStyle.Normal);
		AZY["100"]["TextColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["100"]["Size"] = UDim2.new(0.2280000001192093, 0, 0.09600000083446503, 0);
		AZY["100"]["Name"] = [[Btools]];
		AZY["100"]["Text"] = [[         BTools]];
		AZY["100"]["Position"] = UDim2.new(0.2924708425998688, 0, 0.18550994992256165, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.BuiltInHax.Scripts.Btools.UICorner
		AZY["101"] = Instance.new("UICorner", AZY["100"]);
		AZY["101"]["CornerRadius"] = UDim.new(0, 5);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.BuiltInHax.Scripts.Btools.LocalScript
		AZY["102"] = Instance.new("LocalScript", AZY["100"]);


		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.BuiltInHax.Scripts.Btools.Info
		AZY["103"] = Instance.new("ImageLabel", AZY["100"]);
		AZY["103"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["103"]["Image"] = [[rbxassetid://12585776892]];
		AZY["103"]["Size"] = UDim2.new(0, 16, 0, 16);
		AZY["103"]["Name"] = [[Info]];
		AZY["103"]["BackgroundTransparency"] = 1;
		AZY["103"]["Position"] = UDim2.new(0.7910000085830688, 0, 0.09000000357627869, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.BuiltInHax.Scripts.Dex
		AZY["104"] = Instance.new("TextButton", AZY["fb"]);
		AZY["104"]["TextWrapped"] = true;
		AZY["104"]["TextXAlignment"] = Enum.TextXAlignment.Left;
		AZY["104"]["BackgroundColor3"] = Color3.fromRGB(255, 0, 0);
		AZY["104"]["TextSize"] = 13;
		AZY["104"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Bold, Enum.FontStyle.Normal);
		AZY["104"]["TextColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["104"]["Size"] = UDim2.new(0.2280000001192093, 0, 0.09600000083446503, 0);
		AZY["104"]["Name"] = [[Dex]];
		AZY["104"]["Text"] = [[  DEX Explorer]];
		AZY["104"]["Position"] = UDim2.new(0.2938356399536133, 0, 0.04143177345395088, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.BuiltInHax.Scripts.Dex.UICorner
		AZY["105"] = Instance.new("UICorner", AZY["104"]);
		AZY["105"]["CornerRadius"] = UDim.new(0, 5);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.BuiltInHax.Scripts.Dex.LocalScript
		AZY["106"] = Instance.new("LocalScript", AZY["104"]);


		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.BuiltInHax.Scripts.Dex.Info
		AZY["107"] = Instance.new("ImageLabel", AZY["104"]);
		AZY["107"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["107"]["Image"] = [[rbxassetid://12585776892]];
		AZY["107"]["Size"] = UDim2.new(0, 16, 0, 16);
		AZY["107"]["Name"] = [[Info]];
		AZY["107"]["BackgroundTransparency"] = 1;
		AZY["107"]["Position"] = UDim2.new(0.7910000085830688, 0, 0.09000000357627869, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.BuiltInHax.Scripts.FatesESP
		AZY["108"] = Instance.new("TextButton", AZY["fb"]);
		AZY["108"]["TextWrapped"] = true;
		AZY["108"]["TextXAlignment"] = Enum.TextXAlignment.Left;
		AZY["108"]["BackgroundColor3"] = Color3.fromRGB(255, 0, 0);
		AZY["108"]["TextSize"] = 13;
		AZY["108"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Bold, Enum.FontStyle.Normal);
		AZY["108"]["TextColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["108"]["Size"] = UDim2.new(0.2280000001192093, 0, 0.09600000083446503, 0);
		AZY["108"]["Name"] = [[FatesESP]];
		AZY["108"]["Text"] = [[      Fates ESP]];
		AZY["108"]["Position"] = UDim2.new(0.0331718735396862, 0, 0.18866735696792603, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.BuiltInHax.Scripts.FatesESP.UICorner
		AZY["109"] = Instance.new("UICorner", AZY["108"]);
		AZY["109"]["CornerRadius"] = UDim.new(0, 5);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.BuiltInHax.Scripts.FatesESP.LocalScript
		AZY["10a"] = Instance.new("LocalScript", AZY["108"]);


		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.BuiltInHax.Scripts.FatesESP.Info
		AZY["10b"] = Instance.new("ImageLabel", AZY["108"]);
		AZY["10b"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["10b"]["Image"] = [[rbxassetid://12585776892]];
		AZY["10b"]["Size"] = UDim2.new(0, 16, 0, 16);
		AZY["10b"]["Name"] = [[Info]];
		AZY["10b"]["BackgroundTransparency"] = 1;
		AZY["10b"]["Position"] = UDim2.new(0.7910000085830688, 0, 0.09000000357627869, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.BuiltInHax.Scripts.Fly
		AZY["10c"] = Instance.new("TextButton", AZY["fb"]);
		AZY["10c"]["TextWrapped"] = true;
		AZY["10c"]["TextXAlignment"] = Enum.TextXAlignment.Left;
		AZY["10c"]["BackgroundColor3"] = Color3.fromRGB(255, 0, 0);
		AZY["10c"]["TextSize"] = 13;
		AZY["10c"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Bold, Enum.FontStyle.Normal);
		AZY["10c"]["TextColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["10c"]["Size"] = UDim2.new(0.2280000001192093, 0, 0.09600000083446503, 0);
		AZY["10c"]["Name"] = [[Fly]];
		AZY["10c"]["Text"] = [[           Fly]];
		AZY["10c"]["Position"] = UDim2.new(0.28985166549682617, 0, 0.3375365436077118, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.BuiltInHax.Scripts.Fly.UICorner
		AZY["10d"] = Instance.new("UICorner", AZY["10c"]);
		AZY["10d"]["CornerRadius"] = UDim.new(0, 5);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.BuiltInHax.Scripts.Fly.LocalScript
		AZY["10e"] = Instance.new("LocalScript", AZY["10c"]);


		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.BuiltInHax.Scripts.Fly.Info
		AZY["10f"] = Instance.new("ImageLabel", AZY["10c"]);
		AZY["10f"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["10f"]["Image"] = [[rbxassetid://12585776892]];
		AZY["10f"]["Size"] = UDim2.new(0, 16, 0, 16);
		AZY["10f"]["Name"] = [[Info]];
		AZY["10f"]["BackgroundTransparency"] = 1;
		AZY["10f"]["Position"] = UDim2.new(0.7910000085830688, 0, 0.09000000357627869, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.BuiltInHax.Scripts.IY
		AZY["110"] = Instance.new("TextButton", AZY["fb"]);
		AZY["110"]["TextWrapped"] = true;
		AZY["110"]["TextXAlignment"] = Enum.TextXAlignment.Left;
		AZY["110"]["BackgroundColor3"] = Color3.fromRGB(255, 0, 0);
		AZY["110"]["TextSize"] = 13;
		AZY["110"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Bold, Enum.FontStyle.Normal);
		AZY["110"]["TextColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["110"]["Size"] = UDim2.new(0.22804169356822968, 0, 0.0958060473203659, 0);
		AZY["110"]["Name"] = [[IY]];
		AZY["110"]["Text"] = [[  Infinite Yield]];
		AZY["110"]["Position"] = UDim2.new(0.03485134616494179, 0, 0.04589534550905228, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.BuiltInHax.Scripts.IY.UICorner
		AZY["111"] = Instance.new("UICorner", AZY["110"]);
		AZY["111"]["CornerRadius"] = UDim.new(0, 5);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.BuiltInHax.Scripts.IY.LocalScript
		AZY["112"] = Instance.new("LocalScript", AZY["110"]);


		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.BuiltInHax.Scripts.IY.Info
		AZY["113"] = Instance.new("ImageLabel", AZY["110"]);
		AZY["113"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["113"]["Image"] = [[rbxassetid://12585776892]];
		AZY["113"]["Size"] = UDim2.new(0, 16, 0, 16);
		AZY["113"]["Name"] = [[Info]];
		AZY["113"]["BackgroundTransparency"] = 1;
		AZY["113"]["Position"] = UDim2.new(0.7910000085830688, 0, 0.09000000357627869, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.BuiltInHax.Scripts.PwnHub
		AZY["114"] = Instance.new("TextButton", AZY["fb"]);
		AZY["114"]["TextWrapped"] = true;
		AZY["114"]["TextXAlignment"] = Enum.TextXAlignment.Left;
		AZY["114"]["BackgroundColor3"] = Color3.fromRGB(255, 0, 0);
		AZY["114"]["TextSize"] = 13;
		AZY["114"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Bold, Enum.FontStyle.Normal);
		AZY["114"]["TextColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["114"]["Size"] = UDim2.new(0.2280000001192093, 0, 0.09600000083446503, 0);
		AZY["114"]["Name"] = [[PwnHub]];
		AZY["114"]["Text"] = [[    Pwner Hub]];
		AZY["114"]["Position"] = UDim2.new(0.03055272251367569, 0, 0.4659311771392822, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.BuiltInHax.Scripts.PwnHub.UICorner
		AZY["115"] = Instance.new("UICorner", AZY["114"]);
		AZY["115"]["CornerRadius"] = UDim.new(0, 5);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.BuiltInHax.Scripts.PwnHub.LocalScript
		AZY["116"] = Instance.new("LocalScript", AZY["114"]);


		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.BuiltInHax.Scripts.PwnHub.Info
		AZY["117"] = Instance.new("ImageLabel", AZY["114"]);
		AZY["117"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["117"]["Image"] = [[rbxassetid://12585776892]];
		AZY["117"]["Size"] = UDim2.new(0, 16, 0, 16);
		AZY["117"]["Name"] = [[Info]];
		AZY["117"]["BackgroundTransparency"] = 1;
		AZY["117"]["Position"] = UDim2.new(0.7910000085830688, 0, 0.09000000357627869, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.BuiltInHax.Title
		AZY["118"] = Instance.new("TextLabel", AZY["ce"]);
		AZY["118"]["TextWrapped"] = true;
		AZY["118"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["118"]["TextXAlignment"] = Enum.TextXAlignment.Left;
		AZY["118"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Bold, Enum.FontStyle.Normal);
		AZY["118"]["TextSize"] = 12;
		AZY["118"]["TextColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["118"]["Size"] = UDim2.new(0.5070894360542297, 0, 0.10439325869083405, 0);
		AZY["118"]["Text"] = [[Welcome in the Built-In Hacks section!]];
		AZY["118"]["Name"] = [[Title]];
		AZY["118"]["BackgroundTransparency"] = 1;
		AZY["118"]["Position"] = UDim2.new(0.033080533146858215, 0, 0.7568540573120117, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.BuiltInHax.Title
		AZY["119"] = Instance.new("TextLabel", AZY["ce"]);
		AZY["119"]["TextWrapped"] = true;
		AZY["119"]["TextYAlignment"] = Enum.TextYAlignment.Top;
		AZY["119"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["119"]["TextXAlignment"] = Enum.TextXAlignment.Left;
		AZY["119"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Regular, Enum.FontStyle.Normal);
		AZY["119"]["TextSize"] = 10;
		AZY["119"]["TextColor3"] = Color3.fromRGB(171, 171, 171);
		AZY["119"]["Size"] = UDim2.new(0.5410764813423157, 0, 0.10439325869083405, 0);
		AZY["119"]["Text"] = [[Here you can easily change your player gravity, speed and jump power. You can execute our built-in scripts too!]];
		AZY["119"]["Name"] = [[Title]];
		AZY["119"]["BackgroundTransparency"] = 1;
		AZY["119"]["Position"] = UDim2.new(0.030461372807621956, 0, 0.862415075302124, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Executor
		AZY["11a"] = Instance.new("Frame", AZY["2b"]);
		AZY["11a"]["BackgroundColor3"] = Color3.fromRGB(0, 0, 0);
		AZY["11a"]["BackgroundTransparency"] = 0.550000011920929;
		AZY["11a"]["Size"] = UDim2.new(0.831805408000946, 0, 0.7551097869873047, 0);
		AZY["11a"]["Position"] = UDim2.new(0.1409205049276352, 0, 0.20551720261573792, 0);
		AZY["11a"]["Visible"] = false;
		AZY["11a"]["Name"] = [[Executor]];

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Executor.UICorner
		AZY["11b"] = Instance.new("UICorner", AZY["11a"]);
		AZY["11b"]["CornerRadius"] = UDim.new(0, 15);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Executor.Execute
		AZY["11c"] = Instance.new("TextButton", AZY["11a"]);
		AZY["11c"]["TextWrapped"] = true;
		AZY["11c"]["BackgroundColor3"] = Color3.fromRGB(255, 0, 0);
		AZY["11c"]["TextSize"] = 18;
		AZY["11c"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Bold, Enum.FontStyle.Normal);
		AZY["11c"]["TextColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["11c"]["Size"] = UDim2.new(0.22599999606609344, 0, 0.13500000536441803, 0);
		AZY["11c"]["Name"] = [[Execute]];
		AZY["11c"]["Text"] = [[Execute]];
		AZY["11c"]["Position"] = UDim2.new(0.026000000536441803, 0, 0.8319999575614929, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Executor.Execute.UICorner
		AZY["11d"] = Instance.new("UICorner", AZY["11c"]);
		AZY["11d"]["CornerRadius"] = UDim.new(0, 9);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Executor.Execute.LocalScript
		AZY["11e"] = Instance.new("LocalScript", AZY["11c"]);


		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Executor.Clear
		AZY["11f"] = Instance.new("TextButton", AZY["11a"]);
		AZY["11f"]["TextWrapped"] = true;
		AZY["11f"]["BackgroundColor3"] = Color3.fromRGB(255, 0, 0);
		AZY["11f"]["TextSize"] = 18;
		AZY["11f"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Bold, Enum.FontStyle.Normal);
		AZY["11f"]["TextColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["11f"]["Size"] = UDim2.new(0.22599999606609344, 0, 0.13500000536441803, 0);
		AZY["11f"]["Name"] = [[Clear]];
		AZY["11f"]["Text"] = [[Clear]];
		AZY["11f"]["Position"] = UDim2.new(0.2630000114440918, 0, 0.8320000171661377, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Executor.Clear.UICorner
		AZY["120"] = Instance.new("UICorner", AZY["11f"]);
		AZY["120"]["CornerRadius"] = UDim.new(0, 9);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Executor.Clear.LocalScript
		AZY["121"] = Instance.new("LocalScript", AZY["11f"]);


		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Executor.Copy
		AZY["122"] = Instance.new("TextButton", AZY["11a"]);
		AZY["122"]["TextWrapped"] = true;
		AZY["122"]["BackgroundColor3"] = Color3.fromRGB(255, 0, 0);
		AZY["122"]["TextSize"] = 18;
		AZY["122"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Bold, Enum.FontStyle.Normal);
		AZY["122"]["TextColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["122"]["Size"] = UDim2.new(0.22599999606609344, 0, 0.13500000536441803, 0);
		AZY["122"]["Name"] = [[Copy]];
		AZY["122"]["Text"] = [[Copy]];
		AZY["122"]["Position"] = UDim2.new(0.5009999871253967, 0, 0.8320000171661377, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Executor.Copy.UICorner
		AZY["123"] = Instance.new("UICorner", AZY["122"]);
		AZY["123"]["CornerRadius"] = UDim.new(0, 9);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Executor.Copy.LocalScript
		AZY["124"] = Instance.new("LocalScript", AZY["122"]);


		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Executor.Paste
		AZY["125"] = Instance.new("TextButton", AZY["11a"]);
		AZY["125"]["TextWrapped"] = true;
		AZY["125"]["TextScaled"] = true;
		AZY["125"]["BackgroundColor3"] = Color3.fromRGB(255, 0, 0);
		AZY["125"]["TextSize"] = 18;
		AZY["125"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Bold, Enum.FontStyle.Normal);
		AZY["125"]["TextColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["125"]["Size"] = UDim2.new(0.22599999606609344, 0, 0.13500000536441803, 0);
		AZY["125"]["Name"] = [[Paste]];
		AZY["125"]["Text"] = [[Paste]];
		AZY["125"]["Position"] = UDim2.new(0.7360000014305115, 0, 0.8320000171661377, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Executor.Paste.UICorner
		AZY["126"] = Instance.new("UICorner", AZY["125"]);
		AZY["126"]["CornerRadius"] = UDim.new(0, 9);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Executor.Paste.LocalScript
		AZY["127"] = Instance.new("LocalScript", AZY["125"]);


		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Executor.Paste.UITextSizeConstraint
		AZY["128"] = Instance.new("UITextSizeConstraint", AZY["125"]);
		AZY["128"]["MaxTextSize"] = 18;

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Executor.TextboxBar
		AZY["129"] = Instance.new("Frame", AZY["11a"]);
		AZY["129"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["129"]["BackgroundTransparency"] = 1;
		AZY["129"]["Size"] = UDim2.new(0.9533820152282715, 0, 0.7485234141349792, 0);
		AZY["129"]["Position"] = UDim2.new(0.026000019162893295, 0, 0.04687291383743286, 0);
		AZY["129"]["Name"] = [[TextboxBar]];

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Executor.TextboxBar.LocalScript
		AZY["12a"] = Instance.new("LocalScript", AZY["129"]);


		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Executor.TextboxBar.LocalScript.ScriptEditor
		AZY["12b"] = Instance.new("ModuleScript", AZY["12a"]);
		AZY["12b"]["Name"] = [[ScriptEditor]];

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Executor.TextboxBar.LocalScript.ScriptEditor.Syntax
		AZY["12c"] = Instance.new("ModuleScript", AZY["12b"]);
		AZY["12c"]["Name"] = [[Syntax]];

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Executor.TextboxBar.LocalScript.ScriptEditor.Theme
		AZY["12d"] = Instance.new("ModuleScript", AZY["12b"]);
		AZY["12d"]["Name"] = [[Theme]];

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Executor.TextboxBar.LocalScript.ScriptEditor.GetLines
		AZY["12e"] = Instance.new("ModuleScript", AZY["12b"]);
		AZY["12e"]["Name"] = [[GetLines]];

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Executor.TextboxBar.LocalScript.ScriptEditor.FakeEditor
		AZY["12f"] = Instance.new("ModuleScript", AZY["12b"]);
		AZY["12f"]["Name"] = [[FakeEditor]];

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Executor.TextboxBar.LocalScript.ScriptEditor.GetLine
		AZY["130"] = Instance.new("ModuleScript", AZY["12b"]);
		AZY["130"]["Name"] = [[GetLine]];

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Executor.TextboxBar.LocalScript.ScriptEditor.TweenLibrary
		AZY["131"] = Instance.new("ModuleScript", AZY["12b"]);
		AZY["131"]["Name"] = [[TweenLibrary]];

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Executor.TextboxBar.LocalScript.ScriptEditor.GetWord
		AZY["132"] = Instance.new("ModuleScript", AZY["12b"]);
		AZY["132"]["Name"] = [[GetWord]];

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Executor.TextboxBar.LocalScript.ScriptEditor.Lexer
		AZY["133"] = Instance.new("ModuleScript", AZY["12b"]);
		AZY["133"]["Name"] = [[Lexer]];

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Executor.TextboxBar.LocalScript.ScriptEditor.Suggestions
		AZY["134"] = Instance.new("ModuleScript", AZY["12b"]);
		AZY["134"]["Name"] = [[Suggestions]];

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Executor.TextboxBar.LocalScript.ScriptEditor.Words
		AZY["135"] = Instance.new("ModuleScript", AZY["12b"]);
		AZY["135"]["Name"] = [[Words]];

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Executor.TextboxBar.LocalScript.ScriptEditor.Editor
		AZY["136"] = Instance.new("Frame", AZY["12b"]);
		AZY["136"]["BorderSizePixel"] = 0;
		AZY["136"]["BackgroundColor3"] = Color3.fromRGB(23, 27, 23);
		AZY["136"]["BackgroundTransparency"] = 0.4000000059604645;
		AZY["136"]["Size"] = UDim2.new(1, 0, 1, 0);
		AZY["136"]["BorderColor3"] = Color3.fromRGB(28, 43, 54);
		AZY["136"]["Name"] = [[Editor]];

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Executor.TextboxBar.LocalScript.ScriptEditor.Editor.Scroll
		AZY["137"] = Instance.new("ScrollingFrame", AZY["136"]);
		AZY["137"]["Active"] = true;
		AZY["137"]["CanvasSize"] = UDim2.new(0, 0, 0, 0);
		AZY["137"]["ElasticBehavior"] = Enum.ElasticBehavior.Always;
		AZY["137"]["TopImage"] = [[rbxasset://textures/ui/Scroll/scroll-middle.png]];
		AZY["137"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["137"]["AutomaticCanvasSize"] = Enum.AutomaticSize.XY;
		AZY["137"]["BackgroundTransparency"] = 0.9990000128746033;
		AZY["137"]["Size"] = UDim2.new(1, 0, 1, 0);
		AZY["137"]["ScrollBarImageColor3"] = Color3.fromRGB(64, 64, 64);
		AZY["137"]["BorderColor3"] = Color3.fromRGB(53, 53, 53);
		AZY["137"]["Name"] = [[Scroll]];
		AZY["137"]["BottomImage"] = [[rbxasset://textures/ui/Scroll/scroll-middle.png]];

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Executor.TextboxBar.LocalScript.ScriptEditor.Editor.Scroll.Source
		AZY["138"] = Instance.new("TextBox", AZY["137"]);
		AZY["138"]["TextSize"] = 17;
		AZY["138"]["TextXAlignment"] = Enum.TextXAlignment.Left;
		AZY["138"]["TextStrokeColor3"] = Color3.fromRGB(41, 41, 41);
		AZY["138"]["TextYAlignment"] = Enum.TextYAlignment.Top;
		AZY["138"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["138"]["TextColor3"] = Color3.fromRGB(239, 239, 239);
		AZY["138"]["FontFace"] = Font.new([[rbxasset://fonts/families/Inconsolata.json]], Enum.FontWeight.Regular, Enum.FontStyle.Normal);
		AZY["138"]["MultiLine"] = true;
		AZY["138"]["BackgroundTransparency"] = 0.9990000128746033;
		AZY["138"]["Size"] = UDim2.new(1, -44, 1, -5);
		AZY["138"]["Text"] = [[]];
		AZY["138"]["Position"] = UDim2.new(0, 44, 0, 5);
		AZY["138"]["AutomaticSize"] = Enum.AutomaticSize.XY;
		AZY["138"]["Name"] = [[Source]];
		AZY["138"]["ClearTextOnFocus"] = false;

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Executor.TextboxBar.LocalScript.ScriptEditor.Editor.Scroll.Source.LineHighlight
		AZY["139"] = Instance.new("Frame", AZY["138"]);
		AZY["139"]["BorderSizePixel"] = 0;
		AZY["139"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["139"]["AnchorPoint"] = Vector2.new(0, 0.5);
		AZY["139"]["BackgroundTransparency"] = 0.9399999976158142;
		AZY["139"]["Size"] = UDim2.new(1, 0, 0, 17);
		AZY["139"]["Position"] = UDim2.new(0, -10, 0, 9);
		AZY["139"]["Name"] = [[LineHighlight]];

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Executor.TextboxBar.LocalScript.ScriptEditor.Editor.Scroll.Source.Hidden
		AZY["13a"] = Instance.new("TextLabel", AZY["138"]);
		AZY["13a"]["BorderSizePixel"] = 0;
		AZY["13a"]["TextYAlignment"] = Enum.TextYAlignment.Top;
		AZY["13a"]["BackgroundColor3"] = Color3.fromRGB(27, 32, 27);
		AZY["13a"]["TextXAlignment"] = Enum.TextXAlignment.Left;
		AZY["13a"]["FontFace"] = Font.new([[rbxasset://fonts/families/Inconsolata.json]], Enum.FontWeight.Regular, Enum.FontStyle.Normal);
		AZY["13a"]["TextSize"] = 22;
		AZY["13a"]["TextColor3"] = Color3.fromRGB(249, 66, 164);
		AZY["13a"]["Size"] = UDim2.new(1, 0, 1, 0);
		AZY["13a"]["BorderColor3"] = Color3.fromRGB(0, 0, 0);
		AZY["13a"]["Text"] = [[*script hidden*]];
		AZY["13a"]["Name"] = [[Hidden]];
		AZY["13a"]["Visible"] = false;

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Executor.TextboxBar.LocalScript.ScriptEditor.Editor.Scroll.Source.Suggestion
		AZY["13b"] = Instance.new("TextButton", AZY["138"]);
		AZY["13b"]["TextXAlignment"] = Enum.TextXAlignment.Left;
		AZY["13b"]["BackgroundColor3"] = Color3.fromRGB(40, 40, 40);
		AZY["13b"]["TextSize"] = 17;
		AZY["13b"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Bold, Enum.FontStyle.Normal);
		AZY["13b"]["TextColor3"] = Color3.fromRGB(244, 244, 244);
		AZY["13b"]["Visible"] = false;
		AZY["13b"]["Size"] = UDim2.new(0, 130, 0, 26);
		AZY["13b"]["Name"] = [[Suggestion]];
		AZY["13b"]["BorderColor3"] = Color3.fromRGB(60, 60, 60);
		AZY["13b"]["Text"] = [[keyword]];
		AZY["13b"]["AutomaticSize"] = Enum.AutomaticSize.X;

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Executor.TextboxBar.LocalScript.ScriptEditor.Editor.Scroll.Source.Suggestion.TextPadding
		AZY["13c"] = Instance.new("UIPadding", AZY["13b"]);
		AZY["13c"]["Name"] = [[TextPadding]];
		AZY["13c"]["PaddingLeft"] = UDim.new(0, 30);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Executor.TextboxBar.LocalScript.ScriptEditor.Editor.Scroll.Source.Suggestion.Icon
		AZY["13d"] = Instance.new("ImageLabel", AZY["13b"]);
		AZY["13d"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["13d"]["Image"] = [[rbxassetid://413365069]];
		AZY["13d"]["Size"] = UDim2.new(0, 26, 0, 26);
		AZY["13d"]["Name"] = [[Icon]];
		AZY["13d"]["BackgroundTransparency"] = 1;
		AZY["13d"]["Position"] = UDim2.new(0, -30, 0, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Executor.TextboxBar.LocalScript.ScriptEditor.Editor.Scroll.Source.Suggestion.Icon.UIAspectRatioConstraint
		AZY["13e"] = Instance.new("UIAspectRatioConstraint", AZY["13d"]);


		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Executor.TextboxBar.LocalScript.ScriptEditor.Editor.Scroll.Left
		AZY["13f"] = Instance.new("Frame", AZY["137"]);
		AZY["13f"]["BorderSizePixel"] = 0;
		AZY["13f"]["BackgroundColor3"] = Color3.fromRGB(30, 30, 30);
		AZY["13f"]["BackgroundTransparency"] = 0.4000000059604645;
		AZY["13f"]["Size"] = UDim2.new(0, 27, 1, 0);
		AZY["13f"]["AutomaticSize"] = Enum.AutomaticSize.Y;
		AZY["13f"]["Name"] = [[Left]];

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Executor.TextboxBar.LocalScript.ScriptEditor.Editor.Scroll.Left.Right
		AZY["140"] = Instance.new("Frame", AZY["13f"]);
		AZY["140"]["BorderSizePixel"] = 0;
		AZY["140"]["BackgroundColor3"] = Color3.fromRGB(36, 36, 36);
		AZY["140"]["BackgroundTransparency"] = 0.4000000059604645;
		AZY["140"]["Size"] = UDim2.new(0, 8, 1, 0);
		AZY["140"]["Position"] = UDim2.new(1, 0, 0, 0);
		AZY["140"]["AutomaticSize"] = Enum.AutomaticSize.Y;
		AZY["140"]["Name"] = [[Right]];

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Executor.TextboxBar.LocalScript.ScriptEditor.Editor.Scroll.Left.Right.BottomFade
		AZY["141"] = Instance.new("UIGradient", AZY["140"]);
		AZY["141"]["Transparency"] = NumberSequence.new{NumberSequenceKeypoint.new(0.000, 0),NumberSequenceKeypoint.new(0.931, 0),NumberSequenceKeypoint.new(1.000, 1)};
		AZY["141"]["Name"] = [[BottomFade]];
		AZY["141"]["Rotation"] = 90;

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Executor.TextboxBar.LocalScript.ScriptEditor.Editor.Scroll.Left.Right.Shadow
		AZY["142"] = Instance.new("Frame", AZY["140"]);
		AZY["142"]["BorderSizePixel"] = 0;
		AZY["142"]["BackgroundColor3"] = Color3.fromRGB(0, 0, 0);
		AZY["142"]["BackgroundTransparency"] = 0.800000011920929;
		AZY["142"]["Size"] = UDim2.new(0, 5, 1, 0);
		AZY["142"]["Position"] = UDim2.new(1, 0, 0, 0);
		AZY["142"]["AutomaticSize"] = Enum.AutomaticSize.Y;
		AZY["142"]["Name"] = [[Shadow]];

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Executor.TextboxBar.LocalScript.ScriptEditor.Editor.Scroll.Left.Right.Shadow.UIGradient
		AZY["143"] = Instance.new("UIGradient", AZY["142"]);
		AZY["143"]["Transparency"] = NumberSequence.new{NumberSequenceKeypoint.new(0.000, 0),NumberSequenceKeypoint.new(1.000, 1)};

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Executor.TextboxBar.LocalScript.ScriptEditor.Editor.Scroll.Left.Lines
		AZY["144"] = Instance.new("TextLabel", AZY["13f"]);
		AZY["144"]["TextYAlignment"] = Enum.TextYAlignment.Top;
		AZY["144"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["144"]["TextXAlignment"] = Enum.TextXAlignment.Left;
		AZY["144"]["FontFace"] = Font.new([[rbxasset://fonts/families/Inconsolata.json]], Enum.FontWeight.Regular, Enum.FontStyle.Normal);
		AZY["144"]["TextSize"] = 17;
		AZY["144"]["TextColor3"] = Color3.fromRGB(242, 242, 242);
		AZY["144"]["AutomaticSize"] = Enum.AutomaticSize.X;
		AZY["144"]["Size"] = UDim2.new(1, -5, 1, -7);
		AZY["144"]["Text"] = [[1]];
		AZY["144"]["Name"] = [[Lines]];
		AZY["144"]["BackgroundTransparency"] = 0.9990000128746033;
		AZY["144"]["Position"] = UDim2.new(0, 5, 0, 7);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Executor.TextboxBar.LocalScript.ScriptEditor.Editor.Scroll.Left.Lines.BottomFade
		AZY["145"] = Instance.new("UIGradient", AZY["144"]);
		AZY["145"]["Transparency"] = NumberSequence.new{NumberSequenceKeypoint.new(0.000, 0),NumberSequenceKeypoint.new(0.931, 0),NumberSequenceKeypoint.new(1.000, 1)};
		AZY["145"]["Name"] = [[BottomFade]];
		AZY["145"]["Rotation"] = 90;

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Executor.TextboxBar.LocalScript.ScriptEditor.Editor.Scroll.Left.AdaptSize
		AZY["146"] = Instance.new("LocalScript", AZY["13f"]);
		AZY["146"]["Name"] = [[AdaptSize]];

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Executor.TextboxBar.LocalScript.ScriptEditor.Editor.Scroll.Left.BottomFade
		AZY["147"] = Instance.new("UIGradient", AZY["13f"]);
		AZY["147"]["Transparency"] = NumberSequence.new{NumberSequenceKeypoint.new(0.000, 0),NumberSequenceKeypoint.new(0.931, 0),NumberSequenceKeypoint.new(1.000, 1)};
		AZY["147"]["Name"] = [[BottomFade]];
		AZY["147"]["Rotation"] = 90;

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Executor.TextboxBar.LocalScript.ScriptEditor.TextFixer
		AZY["148"] = Instance.new("ModuleScript", AZY["12b"]);
		AZY["148"]["Name"] = [[TextFixer]];

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Executor.ResetTextBox
		AZY["149"] = Instance.new("TextButton", AZY["11a"]);
		AZY["149"]["TextWrapped"] = true;
		AZY["149"]["TextTransparency"] = 0.699999988079071;
		AZY["149"]["BackgroundColor3"] = Color3.fromRGB(255, 0, 0);
		AZY["149"]["TextSize"] = 18;
		AZY["149"]["FontFace"] = Font.new([[rbxasset://fonts/families/SourceSansPro.json]], Enum.FontWeight.Bold, Enum.FontStyle.Normal);
		AZY["149"]["TextColor3"] = Color3.fromRGB(25, 25, 25);
		AZY["149"]["Size"] = UDim2.new(0.04265729710459709, 0, 0.054356444627046585, 0);
		AZY["149"]["Name"] = [[ResetTextBox]];
		AZY["149"]["Text"] = [[*]];
		AZY["149"]["Position"] = UDim2.new(0.005046568810939789, 0, -0.011172410100698471, 0);
		AZY["149"]["BackgroundTransparency"] = 1;

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Executor.ResetTextBox.UICorner
		AZY["14a"] = Instance.new("UICorner", AZY["149"]);
		AZY["14a"]["CornerRadius"] = UDim.new(0, 9);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Executor.ResetTextBox.LocalScript
		AZY["14b"] = Instance.new("LocalScript", AZY["149"]);


		-- StarterGui.ArceusXV3.MainUI.MainFrame.TabBar
		AZY["14c"] = Instance.new("Frame", AZY["19"]);
		AZY["14c"]["BackgroundColor3"] = Color3.fromRGB(0, 0, 0);
		AZY["14c"]["BackgroundTransparency"] = 0.550000011920929;
		AZY["14c"]["Size"] = UDim2.new(0.09215505421161652, 0, 0.7551097273826599, 0);
		AZY["14c"]["Position"] = UDim2.new(0.02942327782511711, 0, 0.2055172324180603, 0);
		AZY["14c"]["Name"] = [[TabBar]];

		-- StarterGui.ArceusXV3.MainUI.MainFrame.TabBar.UICorner
		AZY["14d"] = Instance.new("UICorner", AZY["14c"]);
		AZY["14d"]["CornerRadius"] = UDim.new(0, 12);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.TabBar.Changelogs
		AZY["14e"] = Instance.new("ImageButton", AZY["14c"]);
		AZY["14e"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["14e"]["Image"] = [[rbxassetid://12582706243]];
		AZY["14e"]["Size"] = UDim2.new(0.7092337608337402, 0, 0.1439468413591385, 0);
		AZY["14e"]["Name"] = [[Changelogs]];
		AZY["14e"]["Position"] = UDim2.new(0.14184674620628357, 0, 0.04798227921128273, 0);
		AZY["14e"]["BackgroundTransparency"] = 1;

		-- StarterGui.ArceusXV3.MainUI.MainFrame.TabBar.Changelogs.Frame
		AZY["14f"] = Instance.new("Frame", AZY["14e"]);
		AZY["14f"]["BackgroundColor3"] = Color3.fromRGB(255, 0, 0);
		AZY["14f"]["Size"] = UDim2.new(0, 3, 0, 25);
		AZY["14f"]["Position"] = UDim2.new(-0.20000001788139343, 0, 0.06666667014360428, 0);
		AZY["14f"]["Visible"] = false;

		-- StarterGui.ArceusXV3.MainUI.MainFrame.TabBar.Changelogs.Frame.UICorner
		AZY["150"] = Instance.new("UICorner", AZY["14f"]);
		AZY["150"]["CornerRadius"] = UDim.new(1, 1);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.TabBar.Changelogs.LocalScript
		AZY["151"] = Instance.new("LocalScript", AZY["14e"]);


		-- StarterGui.ArceusXV3.MainUI.MainFrame.TabBar.Home
		AZY["152"] = Instance.new("ImageButton", AZY["14c"]);
		AZY["152"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["152"]["Image"] = [[rbxassetid://12582723040]];
		AZY["152"]["Size"] = UDim2.new(0.9692861437797546, 0, 0.19672733545303345, 0);
		AZY["152"]["Name"] = [[Home]];
		AZY["152"]["Position"] = UDim2.new(0, 0, 0.30228832364082336, 0);
		AZY["152"]["BackgroundTransparency"] = 1;

		-- StarterGui.ArceusXV3.MainUI.MainFrame.TabBar.Home.Frame
		AZY["153"] = Instance.new("Frame", AZY["152"]);
		AZY["153"]["BackgroundColor3"] = Color3.fromRGB(255, 0, 0);
		AZY["153"]["Size"] = UDim2.new(0, 3, 0, 25);
		AZY["153"]["Position"] = UDim2.new(0.004999999888241291, 0, 0.1889999955892563, 0);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.TabBar.Home.Frame.UICorner
		AZY["154"] = Instance.new("UICorner", AZY["153"]);
		AZY["154"]["CornerRadius"] = UDim.new(1, 1);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.TabBar.Home.LocalScript
		AZY["155"] = Instance.new("LocalScript", AZY["152"]);


		-- StarterGui.ArceusXV3.MainUI.MainFrame.TabBar.BuiltInHax
		AZY["156"] = Instance.new("ImageButton", AZY["14c"]);
		AZY["156"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["156"]["Image"] = [[rbxassetid://12582724778]];
		AZY["156"]["Size"] = UDim2.new(0.9692861437797546, 0, 0.19672733545303345, 0);
		AZY["156"]["Name"] = [[BuiltInHax]];
		AZY["156"]["Position"] = UDim2.new(0, 0, 0.537401556968689, 0);
		AZY["156"]["BackgroundTransparency"] = 1;

		-- StarterGui.ArceusXV3.MainUI.MainFrame.TabBar.BuiltInHax.Frame
		AZY["157"] = Instance.new("Frame", AZY["156"]);
		AZY["157"]["BackgroundColor3"] = Color3.fromRGB(255, 0, 0);
		AZY["157"]["Size"] = UDim2.new(0, 3, 0, 25);
		AZY["157"]["Position"] = UDim2.new(0, 0, 0.18700000643730164, 0);
		AZY["157"]["Visible"] = false;

		-- StarterGui.ArceusXV3.MainUI.MainFrame.TabBar.BuiltInHax.Frame.UICorner
		AZY["158"] = Instance.new("UICorner", AZY["157"]);
		AZY["158"]["CornerRadius"] = UDim.new(1, 1);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.TabBar.BuiltInHax.LocalScript
		AZY["159"] = Instance.new("LocalScript", AZY["156"]);


		-- StarterGui.ArceusXV3.MainUI.MainFrame.TabBar.Executor
		AZY["15a"] = Instance.new("ImageButton", AZY["14c"]);
		AZY["15a"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["15a"]["Image"] = [[rbxassetid://12582726730]];
		AZY["15a"]["Size"] = UDim2.new(0.8274393677711487, 0, 0.1679379791021347, 0);
		AZY["15a"]["Name"] = [[Executor]];
		AZY["15a"]["Position"] = UDim2.new(0.07092338800430298, 0, 0.7821111679077148, 0);
		AZY["15a"]["BackgroundTransparency"] = 1;

		-- StarterGui.ArceusXV3.MainUI.MainFrame.TabBar.Executor.Frame
		AZY["15b"] = Instance.new("Frame", AZY["15a"]);
		AZY["15b"]["BackgroundColor3"] = Color3.fromRGB(255, 0, 0);
		AZY["15b"]["Size"] = UDim2.new(0, 3, 0, 25);
		AZY["15b"]["Position"] = UDim2.new(-0.10000000149011612, 1, 0.06700000166893005, 0);
		AZY["15b"]["Visible"] = false;

		-- StarterGui.ArceusXV3.MainUI.MainFrame.TabBar.Executor.Frame.UICorner
		AZY["15c"] = Instance.new("UICorner", AZY["15b"]);
		AZY["15c"]["CornerRadius"] = UDim.new(1, 1);

		-- StarterGui.ArceusXV3.MainUI.MainFrame.TabBar.Executor.LocalScript
		AZY["15d"] = Instance.new("LocalScript", AZY["15a"]);


		-- StarterGui.ArceusXV3.MainUI.MainFrame.UIAspectRatioConstraint
		AZY["15e"] = Instance.new("UIAspectRatioConstraint", AZY["19"]);
		AZY["15e"]["AspectRatio"] = 1.66304349899292;

		-- StarterGui.ArceusXV3.MainUI.MainFrame.LocalScript
		AZY["15f"] = Instance.new("LocalScript", AZY["19"]);


		-- StarterGui.ArceusXV3.MainUI.FloatingUI
		AZY["160"] = Instance.new("ImageButton", AZY["18"]);
		AZY["160"]["BackgroundColor3"] = Color3.fromRGB(255, 255, 255);
		AZY["160"]["Image"] = [[rbxassetid://12586647828]];
		AZY["160"]["Size"] = UDim2.new(0, 65, 0, 65);
		AZY["160"]["Name"] = [[FloatingUI]];
		AZY["160"]["Visible"] = false;
		AZY["160"]["Position"] = UDim2.new(0.47328877449035645, 0, 0.44602859020233154, 0);
		AZY["160"]["BackgroundTransparency"] = 1;

		-- StarterGui.ArceusXV3.MainUI.FloatingUI.UICorner
		AZY["161"] = Instance.new("UICorner", AZY["160"]);


		-- StarterGui.ArceusXV3.MainUI.FloatingUI.LocalScript
		AZY["162"] = Instance.new("LocalScript", AZY["160"]);


		-- StarterGui.ArceusXV3.MainUI.FloatingUI.UIAspectRatioConstraint
		AZY["163"] = Instance.new("UIAspectRatioConstraint", AZY["160"]);


		-- Require AZY wrapper
		local AZY_REQUIRE = require;
		local AZY_MODULES = {};
		local function require(Module:ModuleScript)
			local ModuleState = AZY_MODULES[Module];
			if ModuleState then
				if not ModuleState.Required then
					ModuleState.Required = true;
					ModuleState.Value = ModuleState.Closure();
				end
				return ModuleState.Value;
			end;
			return AZY_REQUIRE(Module);
		end

		AZY_MODULES[AZY["12b"]] = {
			Closure = function()
				local script = AZY["12b"];
				-- Lexer by sleitnick
				-- Everything else by me, bread. lol.


				local module = {}

				local syntax 	   = require(script.Syntax)
				local getLines 	   = require(script.GetLines)
				local fakeEditor   = require(script.FakeEditor)
				local textFixer    = require(script.TextFixer)
				local getLine 	   = require(script.GetLine)
				local tween 	   = require(script.TweenLibrary)
				local suggestions  = require(script.Suggestions)

				function module.new(frame)
					local newEditor = script.Editor:Clone()
					newEditor.Parent = frame

					local editorObj  	= fakeEditor.new(newEditor)
					local textbox 	 	= newEditor.Scroll.Source
					local linesLabel 	= newEditor.Scroll.Left.Lines
					local lineHighlight = textbox.LineHighlight

					local highlightBox = Instance.new("TextLabel")
					highlightBox.Size = UDim2.new(1, 0,1, 0)
					highlightBox.Position = UDim2.new(0, 0,0, 0)
					highlightBox.TextColor3 = textbox.TextColor3
					highlightBox.BackgroundTransparency = 1
					highlightBox.Name = "Syntax"
					highlightBox.RichText = true
					highlightBox.TextSize = textbox.TextSize
					highlightBox.Font = textbox.Font
					highlightBox.TextXAlignment = Enum.TextXAlignment.Left
					highlightBox.TextYAlignment = Enum.TextYAlignment.Top
					highlightBox.TextStrokeColor3 = Color3.fromRGB(40, 40, 40)
					highlightBox.TextStrokeTransparency = 0.1
					highlightBox.Text = ""
					highlightBox.Parent = textbox

					editorObj:SetTheme("default")
					textFixer.Fix(highlightBox)
					suggestions:Start(newEditor)

					textbox:GetPropertyChangedSignal("Text"):Connect(function()
						syntax.Highlight(highlightBox, textbox.Text)

						-- Fix tabs
						textbox.Text = textbox.Text:gsub("\t", "    ")
						--textbox.CursorPosition += 4

						-- Update line count
						linesLabel.Text = getLines.GetLinesString(textbox.Text)
					end)

					textbox:GetPropertyChangedSignal("CursorPosition"):Connect(function()
						-- Position line highlight
						local lineYPos = ((getLine:GetCurrentLine(textbox) * textbox.TextSize) - math.ceil(lineHighlight.AbsoluteSize.Y / 2)) + 4

						if lineYPos ~= lineHighlight.Position.Y.Offset then
							tween.TweenPosition(lineHighlight, UDim2.new(0, -10,0, lineYPos), 0.1, Enum.EasingStyle.Quad)
						end
					end)

					return editorObj
				end

				return module

			end;
		};
		AZY_MODULES[AZY["12c"]] = {
			Closure = function()
				local script = AZY["12c"];
				local module = {}

				local lexer 	= require(script.Parent.Lexer)
				local theme 	= require(script.Parent.Theme)
				local textFixer = require(script.Parent.TextFixer)

				local function ColorToFont(text, color)
					return string.format(
						'<font color="rgb(%s,%s,%s)">%s</font>',
						tostring(math.floor(color.R * 255)),
						tostring(math.floor(color.G * 255)),
						tostring(math.floor(color.B * 255)),
						text
					)
				end

				function module.Highlight(textbox, source)
					textbox.Text = ""

					for tokenType, text in lexer.scan(source) do
						local currentTheme = theme.current
						local tokenCol = currentTheme[tokenType]

						if tokenCol then
							textbox.Text = textbox.Text .. ColorToFont(text, tokenCol)
						else
							textbox.Text = textbox.Text .. text
						end
					end

					textFixer.Fix(textbox)
				end

				return module

			end;
		};
		AZY_MODULES[AZY["12d"]] = {
			Closure = function()
				local script = AZY["12d"];
				local theme = {
					current = nil,
					themes = {
						["default"] = {
							["keyword"] = Color3.fromRGB(248, 109, 124),
							["builtin"] = Color3.fromRGB(84, 184, 247),
							["string"] = Color3.fromRGB(130, 241, 149),
							["number"] = Color3.fromRGB(255, 198, 0),
							["comment"] = Color3.fromRGB(106, 106, 100),
							["thingy"] = Color3.fromRGB(253, 251, 154)
						},
						["extra 2"] = {
							["keyword"] = Color3.fromRGB(249, 36, 114),
							["builtin"] = Color3.fromRGB(95, 209, 250),
							["string"] = Color3.fromRGB(217, 219, 88),
							["number"] = Color3.fromRGB(161, 118, 209),
							["comment"] = Color3.fromRGB(116, 122, 101),
							["thingy"] = Color3.fromRGB(248, 245, 139)
						}
					}
				}

				return theme

			end;
		};
		getgenv().ChillzAntiSkid123 = AZY["94"]["Text"]
		getgenv().ChillzAntiSkid1234 = AZY["cc"]["Text"]
		AZY_MODULES[AZY["12e"]] = {
			Closure = function()
				local script = AZY["12e"];
				local module = {}

				function module.GetLines(text)
					local amount = 1

					text:gsub("\n", function()
						amount += 1
					end)

					return amount
				end

				function module.GetLinesString(text)
					local lineAmt = module.GetLines(text)
					local result = ""

					for i = 1, lineAmt do
						result = result .. i .. "\n"
					end

					-- Remove last \n
					result = result:sub(1, #result - 1)

					return result
				end

				return module

			end;
		};
		AZY_MODULES[AZY["12f"]] = {
			Closure = function()
				local script = AZY["12f"];
				local fakeEditor = {} -- Main module

				local textFixer = require(script.Parent.TextFixer)
				local theme = require(script.Parent.Theme)
				local syntax = require(script.Parent.Syntax)

				local editorObj = {
					SetTextSize = function(self, textSize)
						local sourceBox = self.Editor.Scroll.Source
						local syntaxBox = sourceBox.Syntax
						local linesBox = self.Editor.Scroll.Left.Lines
						local lineHighlight = sourceBox.LineHighlight

						sourceBox.TextSize = textSize
						syntaxBox.TextSize = textSize
						linesBox.TextSize = textSize
						lineHighlight.Size = UDim2.new(1, 0,0, textSize + 5)


		--[[
			Might want to fix it manually because adding another \n
			might cause some instability
		]]
						textFixer.Fix(self.Editor.Scroll.Source.Syntax)

						return textSize
					end,
					Destroy = function(self)
						self.Editor:Destroy()
						setmetatable(self, {__index = nil})
						table.clear(self)
						self = nil

						return nil
					end,
					GetText = function(self)
						local sourceBox = self.Editor.Scroll.Source
						return sourceBox.Text
					end,
					SetText = function(self, text)
						local sourceBox = self.Editor.Scroll.Source
						sourceBox.Text = text

						return text
					end,
					ContentToBytes = function(self)
						local text = self.Editor.Scroll.Source.Text
						local bytes = {}

						for _, c in pairs(text:split("")) do
							table.insert(bytes, string.byte(c))
						end

						return "/" .. table.concat(bytes, "/")
					end,
					Hide = function(self)
						local hiddenLabel = self.Editor.Scroll.Source.Hidden
						hiddenLabel.Visible = true
					end,
					Unhide = function(self)
						local hiddenLabel = self.Editor.Scroll.Source.Hidden
						hiddenLabel.Visible = false
					end,
					SetTheme = function(self, themeName)
						local sourceBox = self.Editor.Scroll.Source
						local syntaxBox = sourceBox.Syntax

						assert(theme.themes[themeName], "'" .. themeName .. "' is not a valid theme.")

						theme.current = theme.themes[themeName]

						-- Update highlighting
						syntax.Highlight(syntaxBox, sourceBox.Text)
					end,
				}

				function fakeEditor.new(editor)
					return setmetatable({Editor = editor}, {__index = editorObj})
				end

				return fakeEditor

			end;
		};
		AZY_MODULES[AZY["130"]] = {
			Closure = function()
				local script = AZY["130"];
				local module = {}

				function module.peekBack(self)
					return self.text:sub(self.position - 1, self.position - 1)
				end

				function module.next(self)
					self.position += 1

					self.character = self.text:sub(self.position, self.position)

					if self.character == "\n" then
						self.lines += 1
					end

					if self.position < #self.text and self.position < self.cursorPosition then
						self:next()
					end
				end

				function module.GetCurrentLine(self, textbox)
					self.position = 0
					self.text = textbox.Text .. " "
					self.cursorPosition = textbox.CursorPosition
					self.lines = 1

					self:next()

					return self.lines
				end

				function module.GetCurrentLineWidth(self, textbox)
					self.position = 0
					self.text = textbox.Text .. " "
					self.cursorPosition = textbox.CursorPosition
					self.lines = 1

					self:next()

					-- self.lines is the current line

					return self.position
				end

				return module

			end;
		};
		AZY_MODULES[AZY["131"]] = {
			Closure = function()
				local script = AZY["131"];
				local module = {}

				local tweenService = game:GetService("TweenService")
				local debris = game:GetService("Debris")

				-- Custom functions
				local function default(arg, def)
					if arg == nil then
						arg = def
					end
					return arg
				end

				-- Guis --

				function module.TweenScale(frame, scale, timelen, easingstyle, easingdir)
					local uiscale
					if not frame:FindFirstChild("$ScaleAnim") then
						uiscale = Instance.new("UIScale")
						uiscale.Scale = 1
						uiscale.Name = "$ScaleAnim"
						uiscale.Parent = frame
					end

					-- Generate tween info
					local tinfo = TweenInfo.new(timelen, easingstyle, easingdir)
					local goals = {
						Scale = scale
					}

					-- Finally, play tween
					tweenService:Create(uiscale, tinfo, goals):Play()
					--debris:AddItem(uiscale, timelen) -- Remove it when animation is done
				end

				function module.TweenPosition(frame, position, timelen, easingstyle, easingdir)
					-- Errors & defaults
					assert(frame, "No frame provided")
					assert(position, "No position provided")
					assert(timelen, "No time length provided")
					easingstyle = default(easingstyle, Enum.EasingStyle.Sine)
					easingdir = default(easingdir, Enum.EasingDirection.Out)

					-- Generate tween info
					local tinfo = TweenInfo.new(timelen, easingstyle, easingdir)
					local goals = {
						Position = position
					}

					-- Finally, play tween
					tweenService:Create(frame, tinfo, goals):Play()
				end

				function module.TweenSize(frame, size, timelen, easingstyle, easingdir)
					-- Errors & defaults
					assert(frame, "No frame provided")
					assert(size, "No size provided")
					assert(timelen, "No time length provided")
					easingstyle = default(easingstyle, Enum.EasingStyle.Sine)
					easingdir = default(easingdir, Enum.EasingDirection.Out)

					-- Generate tween info
					local tinfo = TweenInfo.new(timelen, easingstyle, easingdir)
					local goals = {
						Size = size
					}

					-- Finally, play tween
					tweenService:Create(frame, tinfo, goals):Play()
				end

				function module.TweenBackgroundColor3(frame, color, timelen, easingstyle, easingdir)
					-- Errors & defaults
					assert(frame, "No frame provided")
					assert(color, "No color provided")
					assert(timelen, "No time length provided")
					easingstyle = default(easingstyle, Enum.EasingStyle.Sine)
					easingdir = default(easingdir, Enum.EasingDirection.Out)

					-- Generate tween info
					local tinfo = TweenInfo.new(timelen, easingstyle, easingdir)
					local goals = {
						BackgroundColor3 = color
					}

					-- Finally, play tween
					tweenService:Create(frame, tinfo, goals):Play()
				end

				function module.TweenBackgroundTransparency(frame, transparency, timelen, easingstyle, easingdir)
					-- Errors & defaults
					assert(frame, "No frame provided")
					assert(transparency, "No transparency provided")
					assert(timelen, "No time length provided")
					easingstyle = default(easingstyle, Enum.EasingStyle.Sine)
					easingdir = default(easingdir, Enum.EasingDirection.Out)

					-- Generate tween info
					local tinfo = TweenInfo.new(timelen, easingstyle, easingdir)
					local goals = {
						BackgroundTransparency = transparency
					}

					-- Finally, play tween
					tweenService:Create(frame, tinfo, goals):Play()
				end

				function module.TweenBorderColor3(frame, color, timelen, easingstyle, easingdir)
					-- Errors & defaults
					assert(frame, "No frame provided")
					assert(color, "No color provided")
					assert(timelen, "No time length provided")
					easingstyle = default(easingstyle, Enum.EasingStyle.Sine)
					easingdir = default(easingdir, Enum.EasingDirection.Out)

					-- Generate tween info
					local tinfo = TweenInfo.new(timelen, easingstyle, easingdir)
					local goals = {
						BorderColor3 = color
					}

					-- Finally, play tween
					tweenService:Create(frame, tinfo, goals):Play()
				end

				function module.TweenBorderSizePixel(frame, bordersize, timelen, easingstyle, easingdir)
					-- Errors & defaults
					assert(frame, "No frame provided")
					assert(bordersize, "No border size provided")
					assert(timelen, "No time length provided")
					easingstyle = default(easingstyle, Enum.EasingStyle.Sine)
					easingdir = default(easingdir, Enum.EasingDirection.Out)

					-- Generate tween info
					local tinfo = TweenInfo.new(timelen, easingstyle, easingdir)
					local goals = {
						BorderSizePixel = bordersize
					}

					-- Finally, play tween
					tweenService:Create(frame, tinfo, goals):Play()
				end

				function module.TweenImageTransparency(frame, imagetransparency, timelen, easingstyle, easingdir)
					-- Errors & defaults
					assert(frame, "No frame provided")
					assert(imagetransparency, "No image transparency provided")
					assert(timelen, "No time length provided")
					easingstyle = default(easingstyle, Enum.EasingStyle.Sine)
					easingdir = default(easingdir, Enum.EasingDirection.Out)

					-- Generate tween info
					local tinfo = TweenInfo.new(timelen, easingstyle, easingdir)
					local goals = {
						ImageTransparency = imagetransparency
					}

					-- Finally, play tween
					tweenService:Create(frame, tinfo, goals):Play()
				end

				function module.TweenImageColor3(frame, color, timelen, easingstyle, easingdir)
					-- Errors & defaults
					assert(frame, "No frame provided")
					assert(color, "No color provided")
					assert(timelen, "No time length provided")
					easingstyle = default(easingstyle, Enum.EasingStyle.Sine)
					easingdir = default(easingdir, Enum.EasingDirection.Out)

					-- Generate tween info
					local tinfo = TweenInfo.new(timelen, easingstyle, easingdir)
					local goals = {
						ImageColor3 = color
					}

					-- Finally, play tween
					tweenService:Create(frame, tinfo, goals):Play()
				end

				function module.TweenImageRectOffset(frame, offset, timelen, easingstyle, easingdir)
					-- Errors & defaults
					assert(frame, "No frame provided")
					assert(offset, "No offset provided")
					assert(timelen, "No time length provided")
					easingstyle = default(easingstyle, Enum.EasingStyle.Sine)
					easingdir = default(easingdir, Enum.EasingDirection.Out)

					-- Generate tween info
					local tinfo = TweenInfo.new(timelen, easingstyle, easingdir)
					local goals = {
						ImageRectOffset = offset
					}

					-- Finally, play tween
					tweenService:Create(frame, tinfo, goals):Play()
				end

				function module.TweenImageRectSize(frame, size, timelen, easingstyle, easingdir)
					-- Errors & defaults
					assert(frame, "No frame provided")
					assert(size, "No size provided")
					assert(timelen, "No time length provided")
					easingstyle = default(easingstyle, Enum.EasingStyle.Sine)
					easingdir = default(easingdir, Enum.EasingDirection.Out)

					-- Generate tween info
					local tinfo = TweenInfo.new(timelen, easingstyle, easingdir)
					local goals = {
						ImageRectSize = size
					}

					-- Finally, play tween
					tweenService:Create(frame, tinfo, goals):Play()
				end

				function module.TweenSliceScale(frame, scale, timelen, easingstyle, easingdir)
					-- Errors & defaults
					assert(frame, "No frame provided")
					assert(scale, "No scale provided")
					assert(timelen, "No time length provided")
					easingstyle = default(easingstyle, Enum.EasingStyle.Sine)
					easingdir = default(easingdir, Enum.EasingDirection.Out)

					-- Generate tween info
					local tinfo = TweenInfo.new(timelen, easingstyle, easingdir)
					local goals = {
						SliceScale = scale
					}

					-- Finally, play tween
					tweenService:Create(frame, tinfo, goals):Play()
				end

				function module.TweenTextColor3(frame, color, timelen, easingstyle, easingdir)
					-- Errors & defaults
					assert(frame, "No frame provided")
					assert(color, "No color provided")
					assert(timelen, "No time length provided")
					easingstyle = default(easingstyle, Enum.EasingStyle.Sine)
					easingdir = default(easingdir, Enum.EasingDirection.Out)

					-- Generate tween info
					local tinfo = TweenInfo.new(timelen, easingstyle, easingdir)
					local goals = {
						TextColor3 = color
					}

					-- Finally, play tween
					tweenService:Create(frame, tinfo, goals):Play()
				end

				function module.TweenMaxVisibleGraphemes(frame, graphemes, timelen, easingstyle, easingdir)
					-- Errors & defaults
					assert(frame, "No frame provided")
					assert(graphemes, "No graphemes provided")
					assert(timelen, "No time length provided")
					easingstyle = default(easingstyle, Enum.EasingStyle.Sine)
					easingdir = default(easingdir, Enum.EasingDirection.Out)

					-- Generate tween info
					local tinfo = TweenInfo.new(timelen, easingstyle, easingdir)
					local goals = {
						MaxVisibleGraphemes = graphemes
					}

					-- Finally, play tween
					tweenService:Create(frame, tinfo, goals):Play()
				end

				function module.TweenTextSize(frame, size, timelen, easingstyle, easingdir)
					-- Errors & defaults
					assert(frame, "No frame provided")
					assert(size, "No size provided")
					assert(timelen, "No time length provided")
					easingstyle = default(easingstyle, Enum.EasingStyle.Sine)
					easingdir = default(easingdir, Enum.EasingDirection.Out)

					-- Generate tween info
					local tinfo = TweenInfo.new(timelen, easingstyle, easingdir)
					local goals = {
						TextSize = size
					}

					-- Finally, play tween
					tweenService:Create(frame, tinfo, goals):Play()
				end

				function module.TweenTextStrokeColor3(frame, color, timelen, easingstyle, easingdir)
					-- Errors & defaults
					assert(frame, "No frame provided")
					assert(color, "No color provided")
					assert(timelen, "No time length provided")
					easingstyle = default(easingstyle, Enum.EasingStyle.Sine)
					easingdir = default(easingdir, Enum.EasingDirection.Out)

					-- Generate tween info
					local tinfo = TweenInfo.new(timelen, easingstyle, easingdir)
					local goals = {
						TextStrokeColor3 = color
					}

					-- Finally, play tween
					tweenService:Create(frame, tinfo, goals):Play()
				end

				function module.TweenTextTransparency(frame, transparency, timelen, easingstyle, easingdir)
					-- Errors & defaults
					assert(frame, "No frame provided")
					assert(transparency, "No transparency provided")
					assert(timelen, "No time length provided")
					easingstyle = default(easingstyle, Enum.EasingStyle.Sine)
					easingdir = default(easingdir, Enum.EasingDirection.Out)

					-- Generate tween info
					local tinfo = TweenInfo.new(timelen, easingstyle, easingdir)
					local goals = {
						TextTransparency = transparency
					}

					-- Finally, play tween
					tweenService:Create(frame, tinfo, goals):Play()
				end

				function module.TweenTextStrokeTransparency(frame, transparency, timelen, easingstyle, easingdir)
					-- Errors & defaults
					assert(frame, "No frame provided")
					assert(transparency, "No transparency provided")
					assert(timelen, "No time length provided")
					easingstyle = default(easingstyle, Enum.EasingStyle.Sine)
					easingdir = default(easingdir, Enum.EasingDirection.Out)

					-- Generate tween info
					local tinfo = TweenInfo.new(timelen, easingstyle, easingdir)
					local goals = {
						TextStrokeTransparency = transparency
					}

					-- Finally, play tween
					tweenService:Create(frame, tinfo, goals):Play()
				end

				function module.TweenCanvasSize(frame, size, timelen, easingstyle, easingdir)
					-- Errors & defaults
					assert(frame, "No frame provided")
					assert(size, "No size provided")
					assert(timelen, "No time length provided")
					easingstyle = default(easingstyle, Enum.EasingStyle.Sine)
					easingdir = default(easingdir, Enum.EasingDirection.Out)

					-- Generate tween info
					local tinfo = TweenInfo.new(timelen, easingstyle, easingdir)
					local goals = {
						CanvasSize = size
					}

					-- Finally, play tween
					tweenService:Create(frame, tinfo, goals):Play()
				end

				function module.TweenCanvasPosition(frame, position, timelen, easingstyle, easingdir)
					-- Errors & defaults
					assert(frame, "No frame provided")
					assert(position, "No position provided")
					assert(timelen, "No time length provided")
					easingstyle = default(easingstyle, Enum.EasingStyle.Sine)
					easingdir = default(easingdir, Enum.EasingDirection.Out)

					-- Generate tween info
					local tinfo = TweenInfo.new(timelen, easingstyle, easingdir)
					local goals = {
						CanvasPosition = position
					}

					-- Finally, play tween
					tweenService:Create(frame, tinfo, goals):Play()
				end

				function module.TweenScrollBarImageTransparency(frame, transparency, timelen, easingstyle, easingdir)
					-- Errors & defaults
					assert(frame, "No frame provided")
					assert(transparency, "No transparency provided")
					assert(timelen, "No time length provided")
					easingstyle = default(easingstyle, Enum.EasingStyle.Sine)
					easingdir = default(easingdir, Enum.EasingDirection.Out)

					-- Generate tween info
					local tinfo = TweenInfo.new(timelen, easingstyle, easingdir)
					local goals = {
						ScrollBarImageTransparency = transparency
					}

					-- Finally, play tween
					tweenService:Create(frame, tinfo, goals):Play()
				end

				function module.TweenScrollBarThickness(frame, thickness, timelen, easingstyle, easingdir)
					-- Errors & defaults
					assert(frame, "No frame provided")
					assert(thickness, "No thickness provided")
					assert(timelen, "No time length provided")
					easingstyle = default(easingstyle, Enum.EasingStyle.Sine)
					easingdir = default(easingdir, Enum.EasingDirection.Out)

					-- Generate tween info
					local tinfo = TweenInfo.new(timelen, easingstyle, easingdir)
					local goals = {
						ScrollBarThickness = thickness
					}

					-- Finally, play tween
					tweenService:Create(frame, tinfo, goals):Play()
				end

				function module.TweenScrollBarImageColor3(frame, color, timelen, easingstyle, easingdir)
					-- Errors & defaults
					assert(frame, "No frame provided")
					assert(color, "No color provided")
					assert(timelen, "No time length provided")
					easingstyle = default(easingstyle, Enum.EasingStyle.Sine)
					easingdir = default(easingdir, Enum.EasingDirection.Out)

					-- Generate tween info
					local tinfo = TweenInfo.new(timelen, easingstyle, easingdir)
					local goals = {
						ScrollBarImageColor3 = color
					}

					-- Finally, play tween
					tweenService:Create(frame, tinfo, goals):Play()
				end

				function module.TweenCFrame(thing, cframe, timelen, easingstyle, easingdir)
					-- Errors & defaults
					assert(thing, "No instance provided")
					assert(cframe, "No cframe provided")
					assert(timelen, "No time length provided")
					easingstyle = default(easingstyle, Enum.EasingStyle.Sine)
					easingdir = default(easingdir, Enum.EasingDirection.Out)

					-- Generate tween info
					local tinfo = TweenInfo.new(timelen, easingstyle, easingdir)
					local goals = {
						CFrame = cframe
					}

					-- Finally, play tween
					tweenService:Create(thing, tinfo, goals):Play()
				end

				function module.TweenFOV(thing, fov, timelen, easingstyle, easingdir)
					-- Errors & defaults
					assert(thing, "No instance provided")
					assert(fov, "No FOV provided")
					assert(timelen, "No time length provided")
					easingstyle = default(easingstyle, Enum.EasingStyle.Sine)
					easingdir = default(easingdir, Enum.EasingDirection.Out)

					-- Generate tween info
					local tinfo = TweenInfo.new(timelen, easingstyle, easingdir)
					local goals = {
						FieldOfView = fov
					}

					-- Finally, play tween
					tweenService:Create(thing, tinfo, goals):Play()
				end

				function module.TweenValue(thing, value, timelen, easingstyle, easingdir)
					-- Errors & defaults
					assert(thing, "No instance provided")
					assert(value, "No value provided")
					assert(timelen, "No time length provided")
					easingstyle = default(easingstyle, Enum.EasingStyle.Sine)
					easingdir = default(easingdir, Enum.EasingDirection.Out)

					-- Generate tween info
					local tinfo = TweenInfo.new(timelen, easingstyle, easingdir)
					local goals = {
						Value = value
					}

					-- Finally, play tween
					tweenService:Create(thing, tinfo, goals):Play()
				end

				function module.TweenVolume(thing, volume, timelen, easingstyle, easingdir)
					-- Errors & defaults
					assert(thing, "No instance provided")
					assert(volume, "No volume provided")
					assert(timelen, "No time length provided")
					easingstyle = default(easingstyle, Enum.EasingStyle.Sine)
					easingdir = default(easingdir, Enum.EasingDirection.Out)

					-- Generate tween info
					local tinfo = TweenInfo.new(timelen, easingstyle, easingdir)
					local goals = {
						Volume = volume
					}

					-- Finally, play tween
					tweenService:Create(thing, tinfo, goals):Play()
				end

				return module

			end;
		};
		AZY_MODULES[AZY["132"]] = {
			Closure = function()
				local script = AZY["132"];
				local module = {}

				function module.next(self)
					self.position += 1
					local character = self.text:sub(self.position, self.position)

					if character == "\n" or character == " " or self.position > #self.text then
						return self.position - 1
					else
						return self:next()
					end
				end

				function module.prev(self)
					self.position -= 1
					local character = self.text:sub(self.position, self.position)

					if character == "\n" or character == " " or self.position < 1 then
						return self.position + 1
					else
						return self:prev()
					end
				end

				function module.GetCurrentWord(self, textbox)
					self.cursorPosition = textbox.CursorPosition
					self.position = self.cursorPosition
					self.text = textbox.Text

					local wordEnd = self:next()
					local wordStart = self:prev()
					local wordString = self.text:sub(wordStart, wordEnd)

					return wordString
				end

				return module

			end;
		};
		AZY_MODULES[AZY["133"]] = {
			Closure = function()
				local script = AZY["133"];
--[[

	Lexical scanner for creating a sequence of tokens from Lua source code.

	This is a heavily modified and Roblox-optimized version of
	the original Penlight Lexer module:
		https://github.com/stevedonovan/Penlight

	Authors:
		stevedonovan <https://github.com/stevedonovan> ----------------- Original Penlight lexer author
		ryanjmulder  <https://github.com/ryanjmulder>  ----------------- Penlight lexer contributer
		mpeterv      <https://github.com/mpeterv>      ----------------- Penlight lexer contributer
		Tieske       <https://github.com/Tieske>       ----------------- Penlight lexer contributer
		boatbomber   <https://github.com/boatbomber>   ----------------- Roblox port, optimizations, and bug fixes
		Sleitnick    <https://github.com/Sleitnick>    ----------------- Roblox optimizations

	Usage:

		local source = "for i = 1,n do end"
		
		-- The 'scan' function returns a token iterator:
		for token,src in lexer.scan(source) do
			print(token, src)
		end

			> keyword for
			> iden    i
			> =       =
			> number  1
			> ,       ,
			> iden    n
			> keyword do
			> keyword end

	List of tokens:
		- keyword
		- builtin
		- iden
		- string
		- number
		- space
		- comment

	Other tokens that don't fall into the above categories
	will simply be returned as itself. For instance, operators
	like "+" will simply return "+" as the token.

--]]

				local lexer = {}

				local yield, wrap  = coroutine.yield, coroutine.wrap
				local strfind      = string.find
				local strsub       = string.sub
				local append       = table.insert
				local type         = type

				local NUMBER1	= "^[%+%-]?%d+%.?%d*[eE][%+%-]?%d+"
				local NUMBER2	= "^[%+%-]?%d+%.?%d*"
				local NUMBER3	= "^0x[%da-fA-F]+"
				local NUMBER4	= "^%d+%.?%d*[eE][%+%-]?%d+"
				local NUMBER5	= "^%d+%.?%d*"
				local IDEN		= "^[%a_][%w_]*"
				local WSPACE	= "^%s+"
				local STRING1	= "^(['\"])%1"							--Empty String
				local STRING2	= [[^(['"])(\*)%2%1]]
				local STRING3	= [[^(['"]).-[^\](\*)%2%1]]
				local STRING4	= "^(['\"]).-.*"						--Incompleted String
				local STRING5	= "^%[(=*)%[.-%]%1%]"					--Multiline-String
				local STRING6	= "^%[%[.-.*"							--Incompleted Multiline-String
				local CHAR1		= "^''"
				local CHAR2		= [[^'(\*)%1']]
				local CHAR3		= [[^'.-[^\](\*)%1']]
				local PREPRO	= "^#.-[^\\]\n"
				local MCOMMENT1	= "^%-%-%[(=*)%[.-%]%1%]"				--Completed Multiline-Comment
				local MCOMMENT2	= "^%-%-%[%[.-.*"						--Incompleted Multiline-Comment
				local SCOMMENT1	= "^%-%-.-\n"							--Completed Singleline-Comment
				local SCOMMENT2	= "^%-%-.-.*"							--Incompleted Singleline-Comment
				local THINGY 	= "^[%.:]%w-%s?%(.-%)"

				local lua_keyword = {
					["and"] = true,  ["break"] = true,  ["do"] = true,      ["else"] = true,      ["elseif"] = true,
					["end"] = true,  ["false"] = true,  ["for"] = true,     ["function"] = true,  ["if"] = true,
					["in"] = true,   ["local"] = true,  ["nil"] = true,     ["not"] = true,       ["while"] = true,
					["or"] = true,   ["repeat"] = true, ["return"] = true,  ["then"] = true,      ["true"] = true,
					["self"] = true, ["until"] = true
				}

				local lua_builtin = {
					["assert"] = true;["collectgarbage"] = true;["error"] = true;["_G"] = true;
					["gcinfo"] = true;["getfenv"] = true;["getmetatable"] = true;["ipairs"] = true;
					["loadstring"] = true;["newproxy"] = true;["next"] = true;["pairs"] = true;
					["pcall"] = true;["print"] = true;["rawequal"] = true;["rawget"] = true;["rawset"] = true;
					["select"] = true;["setfenv"] = true;["setmetatable"] = true;["tonumber"] = true;
					["tostring"] = true;["type"] = true;["unpack"] = true;["_VERSION"] = true;["xpcall"] = true;
					["delay"] = true;["elapsedTime"] = true;["require"] = true;["spawn"] = true;["tick"] = true;
					["time"] = true;["typeof"] = true;["UserSettings"] = true;["wait"] = true;["warn"] = true;
					["game"] = true;["Enum"] = true;["script"] = true;["shared"] = true;["workspace"] = true;
					["Axes"] = true;["BrickColor"] = true;["CFrame"] = true;["Color3"] = true;["ColorSequence"] = true;
					["ColorSequenceKeypoint"] = true;["Faces"] = true;["Instance"] = true;["NumberRange"] = true;
					["NumberSequence"] = true;["NumberSequenceKeypoint"] = true;["PhysicalProperties"] = true;
					["Random"] = true;["Ray"] = true;["Rect"] = true;["Region3"] = true;["Region3int16"] = true;
					["TweenInfo"] = true;["UDim"] = true;["UDim2"] = true;["Vector2"] = true;["Vector3"] = true;
					["Vector3int16"] = true;["next"] = true;["dofile"] = true;["writefile"] = true;["readfile"] = true;
					["isfile"] = true;["delfile"] = true;["isfolder"] = true;["makefolder"] = true;["delfolder"] = true;["listfiles"] = true;
					["descend"] = true;
					["os"] = true;
					--["os.time"] = true;["os.date"] = true;["os.difftime"] = true;
					["debug"] = true;
					--["debug.traceback"] = true;["debug.profilebegin"] = true;["debug.profileend"] = true;
					["math"] = true;
					--["math.abs"] = true;["math.acos"] = true;["math.asin"] = true;["math.atan"] = true;["math.atan2"] = true;["math.ceil"] = true;["math.clamp"] = true;["math.cos"] = true;["math.cosh"] = true;["math.deg"] = true;["math.exp"] = true;["math.floor"] = true;["math.fmod"] = true;["math.frexp"] = true;["math.ldexp"] = true;["math.log"] = true;["math.log10"] = true;["math.max"] = true;["math.min"] = true;["math.modf"] = true;["math.noise"] = true;["math.pow"] = true;["math.rad"] = true;["math.random"] = true;["math.randomseed"] = true;["math.sign"] = true;["math.sin"] = true;["math.sinh"] = true;["math.sqrt"] = true;["math.tan"] = true;["math.tanh"] = true;
					["coroutine"] = true;
					--["coroutine.create"] = true;["coroutine.resume"] = true;["coroutine.running"] = true;["coroutine.status"] = true;["coroutine.wrap"] = true;["coroutine.yield"] = true;
					["string"] = true;
					--["string.byte"] = true;["string.char"] = true;["string.dump"] = true;["string.find"] = true;["string.format"] = true;["string.len"] = true;["string.lower"] = true;["string.match"] = true;["string.rep"] = true;["string.reverse"] = true;["string.sub"] = true;["string.upper"] = true;["string.gmatch"] = true;["string.gsub"] = true;
					["table"] = true;
					--["table.concat"] = true;["table.insert"] = true;["table.remove"] = true;["table.sort"] = true;
				}

				local function tdump(tok)
					return yield(tok, tok)
				end

				local function ndump(tok)
					return yield("number", tok)
				end

				local function sdump(tok)
					return yield("string", tok)
				end

				local function cdump(tok)
					return yield("comment", tok)
				end

				local function wsdump(tok)
					return yield("space", tok)
				end

				local function lua_vdump(tok)
					if (lua_keyword[tok]) then
						return yield("keyword", tok)
					elseif (lua_builtin[tok]) then
						return yield("builtin", tok)
					else
						return yield("iden", tok)
					end
				end

				local function thingy_dump(tok)
					return yield("thingy", tok)
				end

				local lua_matches = {
					{THINGY, thingy_dump},

					{IDEN,      lua_vdump},        -- Indentifiers
					{WSPACE,    wsdump},           -- Whitespace
					{NUMBER3,   ndump},            -- Numbers
					{NUMBER4,   ndump},
					{NUMBER5,   ndump},
					{STRING1,   sdump},            -- Strings
					{STRING2,   sdump},
					{STRING3,   sdump},
					{STRING4,   sdump},
					{STRING5,   sdump},            -- Multiline-Strings
					{STRING6,   sdump},            -- Multiline-Strings

					{MCOMMENT1, cdump},            -- Multiline-Comments
					{MCOMMENT2, cdump},			
					{SCOMMENT1, cdump},            -- Singleline-Comments
					{SCOMMENT2, cdump},

					{"^==",     tdump},            -- Operators
					{"^~=",     tdump},
					{"^<=",     tdump},
					{"^>=",     tdump},
					{"^%.%.%.", tdump},
					{"^%.%.",   tdump},
					{"^.",      tdump},
				}

				local num_lua_matches = #lua_matches


				--- Create a plain token iterator from a string.
				-- @tparam string s a string.
				function lexer.scan(s)

					local function lex(first_arg)

						local line_nr = 0
						local sz = #s
						local idx = 1

						-- res is the value used to resume the coroutine.
						local function handle_requests(res)
							while (res) do
								local tp = type(res)
								-- Insert a token list:
								if (tp == "table") then
									res = yield("", "")
									for i = 1,#res do
										local t = res[i]
										res = yield(t[1], t[2])
									end
								elseif (tp == "string") then -- Or search up to some special pattern:
									local i1, i2 = strfind(s, res, idx)
									if (i1) then
										local tok = strsub(s, i1, i2)
										idx = (i2 + 1)
										res = yield("", tok)
									else
										res = yield("", "")
										idx = (sz + 1)
									end
								else
									res = yield(line_nr, idx)
								end
							end
						end

						handle_requests(first_arg)
						line_nr = 1

						while (true) do

							if (idx > sz) then
								while (true) do
									handle_requests(yield())
								end
							end

							for i = 1,num_lua_matches do
								local m = lua_matches[i]
								local pat = m[1]
								local fun = m[2]
								local findres = {strfind(s, pat, idx)}
								local i1, i2 = findres[1], findres[2]
								if (i1) then
									local tok = strsub(s, i1, i2)
									idx = (i2 + 1)
									lexer.finished = (idx > sz)
									local res = fun(tok, findres)
									if (tok:find("\n")) then
										-- Update line number:
										local _,newlines = tok:gsub("\n", {})
										line_nr = (line_nr + newlines)
									end
									handle_requests(res)
									break
								end
							end

						end

					end

					return wrap(lex)

				end

				return lexer
			end;
		};
		AZY_MODULES[AZY["134"]] = {
			Closure = function()
				local script = AZY["134"];
				local module = {}

				--// Vars
				local words   = require(script.Parent.Words)
				local GetWord = require(script.Parent.GetWord)
				local getLine = require(script.Parent.GetLine)

				--// Funcs
				function module.GetCurrentWord(self)
					return GetWord:GetCurrentWord(self.Textbox)
				end

				function module.Search(self)
					local currentWord = self:GetCurrentWord():lower()

					if currentWord == "" and #currentWord <= 1 then
						return nil
					end

					for word, wordType in pairs(words) do
						local matched = string.match(word:lower(), currentWord)

						if matched then
							local foundStart, foundEnd = string.find(word:lower(), currentWord)
							return word, (foundEnd - foundStart) + 1
						end
					end

					return nil
				end

				function module.Start(self, editor)
					self.Editor = editor
					self.Textbox = editor.Scroll.Source
					self.SuggestionButton = self.Textbox.Suggestion

					self.Textbox:GetPropertyChangedSignal("Text"):Connect(function()
						local foundWord, matchedLength = self:Search()

						if foundWord then
							local position = UDim2.new(0, 0,0, getLine:GetCurrentLine(self.Textbox) * self.Textbox.TextSize)

							self.SuggestionButton.Text = foundWord
							self.SuggestionButton.Position = position
							self.SuggestionButton.Visible = true
							self.MatchedLength = matchedLength
						else
							self.SuggestionButton.Visible = false
						end
					end)

					self.SuggestionButton.MouseButton1Click:Connect(function(input)
						-- Fill in the word
						local word = self.SuggestionButton.Text
						self.SuggestionButton.Visible = false
						self.Textbox.Text = self.Textbox.Text:sub(1, self.Textbox.CursorPosition - 1 - (self.MatchedLength or 0)) .. word .. self.Textbox.Text:sub(self.Textbox.CursorPosition + 1, #self.Textbox.Text)

						local newCursorPosition = self.Textbox.CursorPosition + #word - self.MatchedLength
						wait()
						self.Textbox:ReleaseFocus()
						self.Textbox:CaptureFocus()
						self.Textbox.CursorPosition = newCursorPosition
					end)
				end

				return module

			end;
		};
		AZY_MODULES[AZY["135"]] = {
			Closure = function()
				local script = AZY["135"];
				local words = {
					['print'] = 'builtin',
					['warn'] = 'builtin',
					['Vector3'] = 'builtin',
					['Vector2'] = 'builtin',
					['error'] = 'builtin',
					['Instance'] = 'builtin',
					['game'] = 'builtin',
					['script'] = 'builtin',
					['workspace'] = 'builtin',

					['while'] = 'keyword',
					['true'] = 'keyword',
					['false'] = 'keyword',
					['then'] = 'keyword',
					['do'] = 'keyword',
					['if'] = 'keyword',
				}

				return words

			end;
		};
		AZY_MODULES[AZY["148"]] = {
			Closure = function()
				local script = AZY["148"];
				-- Fixes a Roblox bug with RichText

				-- If the bug gets fixed, this will break the editor (visually).
				-- In this case, please remove any instances of this module being used.

				local module = {}

				function module.Fix(textbox)
					if textbox.Text:sub(1, 1) ~= "\n" then
						textbox.Text = "\n" .. textbox.Text
					end

					textbox.Position = UDim2.new(0, -3.5,0,-8.9)
					textbox.Size = UDim2.new(1, 4,1, textbox.TextSize)
				end

				return module

			end;
		};
		-- StarterGui.ArceusXV3.Welcome.Welcome.ScrollingFrame.Text.LocalScript
		local function C_9()
			local script = AZY["9"];
			-- Get the local player's name
			local playerName = game.Players.LocalPlayer.DisplayName

			-- Create the welcome message with string interpolation
			local welcomeMessage = string.format([[
	Dear %s,
	
	We are writing to welcome you as one of your first beta testers of Arceus X!
	We are thrilled to have your collaboration and to offer you the opportunity
	to try out the new features we are developing.
	
	We are confident that your experience and creativity will help us make
	Arceus X an even more effective and user-friendly application.
	Please feel free to share any feedback and suggestions that can help us further
	improve our platform.
	
	Thank you so much for your support, and we look forward to working with
	you in this exciting journey!
	
	Best regards,
	SPDM Team
	]], playerName)

			-- Display the welcome message
			script.Parent.Text = welcomeMessage
		end;
		task.spawn(C_9);
		-- StarterGui.ArceusXV3.Welcome.Welcome.ScrollingFrame.TextButton.LocalScriptNew
		local function C_d()
			local script = AZY["d"];
			local btn = script.Parent
			local welcome = script.Parent.Parent.Parent
			local bg = script.Parent.Parent.Parent.Parent.Frame
			local gui = script.Parent.Parent.Parent.Parent

			pcall(function()
				if isfile("arc.xloaded") then
					script.Parent.Parent.Parent.Parent.Parent.MainUI.FloatingUI.Visible = true
					script.Parent.Parent.Parent.Parent.Parent.MainUI.FloatingUI.Active = true
					script.Parent.Parent.Parent.Parent.Frame.Visible = false
					script.Parent.Parent.Parent.Parent.Welcome.Visible = false
				end
			end)

			btn.MouseButton1Click:Connect(function()
				pcall(function()
					writefile("arc.xloaded", "Nothing to read here, this is just a file to check if you're already execute it at first time, you may remove or delete this file to get your welcome message again.")
				end)
				welcome.Visible = false
				bg.Visible=false
				gui.Parent.AnimationIntro.Background.Visible = true
				gui.Parent.AnimationIntro.ImageLabel.Visible = true

				gui.Parent.AnimationIntro.NameLogo.Visible = true
				--gui.Parent.AnimationIntro.Frame.Visible = true


				local function uninvislogo()
					local TextLabel = gui.Parent.AnimationIntro.ImageLabel -- Change this to the name of your TextLabel
					local FadeTime = 1 -- Change this to adjust the fade time in seconds

					for i = 1, 10 do -- Loop 10 times to create a smoother fade
						wait(FadeTime/10) -- Wait for 1/10th of the fade time
						local Alpha = 1 - (i/10) -- Calculate the transparency value
						TextLabel.ImageTransparency = Alpha -- Set the transparency of the TextLabel
					end
				end
				uninvislogo()

				wait(0.5)


				--0, 900,0, 900
				--100, -150, 100, -100
				local function movearc()

					local textn = gui.Parent.AnimationIntro.NameLogo
					local frame1 = textn

					-- Define the start and end positions for the tween
					local startPos1 = UDim2.new(0.442, 0,0.361, 0) --[[FOR LOGO OPENING]] --ACTUAL END
					local endPos1 = UDim2.new(0.482, 0,0.452, 0)

					-- Define the length of time for the tween
					local tweenTime1 = 0.3

					-- Import the TweenService module
					local TweenService1 = game:GetService("TweenService")

					-- Define the tweenInfo for the tween
					local tweenInfo1 = TweenInfo.new(tweenTime1, Enum.EasingStyle.Linear)

					-- Define the tween
					local tween1 = TweenService1:Create(frame1, tweenInfo1, {Position = endPos1})

					-- Play the tween
					tween1:Play()
					local function fadetext()
						local TextLabel = textn -- Change this to the name of your TextLabel
						local FadeTime = 0.3 -- Change this to adjust the fade time in seconds

						for i = 1, 10 do -- Loop 10 times to create a smoother fade [[FOR TEXT]]
							wait(FadeTime/10) -- Wait for 1/10th of the fade time
							local Alpha = 1 - (i/10) -- Calculate the transparency value
							TextLabel.TextTransparency = Alpha -- Set the transparency of the TextLabel
						end
					end


					-- Define the Frame we want to tween
					local frame = gui.Parent.AnimationIntro.ImageLabel

					-- Define the start and end positions for the tween [FOR TEXT]
					local startPos = UDim2.new(0.442, 0,0.361, 0) --ACTUAL END
					local endPos = UDim2.new(0.362, 0,0.361, 0)

					-- Define the length of time for the tween
					local tweenTime = 0.3

					-- Import the TweenService module
					local TweenService = game:GetService("TweenService")

					-- Define the tweenInfo for the tween
					local tweenInfo = TweenInfo.new(tweenTime, Enum.EasingStyle.Linear)

					-- Define the tween
					local tween = TweenService:Create(frame, tweenInfo, {Position = endPos})

					-- Play the tween
					tween:Play()

					gui.Parent.AnimationIntro.Frame.Visible = true
					local TweenService4 = game:GetService("TweenService")

					-- The GUI frame that we want to animate
					local frame4 = gui.Parent.AnimationIntro.Frame

					-- The final size and position that we want to tween to
					local finalSize4 = UDim2.new(0, 2051,0, 1495)
					local finalPosition4 = UDim2.new(-0.353, 0,-0.738, 0)

					-- The duration of the tween in seconds
					local tweenDuration4 = 0.4

					-- Define the tween information for the size and position
					local tweenInfo4 = TweenInfo.new(tweenDuration4, Enum.EasingStyle.Quint, Enum.EasingDirection.Out, 0, false, 0)

					-- Create the tweens for the size and position
					local sizeTween = TweenService:Create(frame4, tweenInfo4, {Size = finalSize4})
					local positionTween = TweenService:Create(frame4, tweenInfo4, {Position = finalPosition4})

					-- Play the tweens simultaneously
					sizeTween:Play()
					positionTween:Play()

					wait(0.2)
					fadetext()
					wait(0.4)
					gui.Parent.AnimationIntro.NameLogo.Visible = true
					wait(1.4)
					local FadeTime = 0.3
					for i = 0, 1.1, 0.1 do -- Loop 10 times to create a smoother far
						gui.Parent.AnimationIntro.Background.BackgroundTransparency = i
						gui.Parent.AnimationIntro.Frame.BackgroundTransparency = i
						gui.Parent.AnimationIntro.ImageLabel.ImageTransparency = i
						gui.Parent.AnimationIntro.NameLogo.TextTransparency = i
						if i == 1 then
							for _,v in pairs(gui.Parent.AnimationIntro:GetChildren()) do
								if v.Visible then
									v.Visible = false
								end
							end
						end
						wait(0.05)
					end
					wait(0.04)
					script.Parent.Parent.Parent.Parent.Parent.MainUI.FloatingUI.Visible = true
					script.Parent.Parent.Parent.Parent.Parent.MainUI.FloatingUI.Active = true
					--print("completed.")


				end

				movearc()
			end)
		end;
		task.spawn(C_d);
		-- StarterGui.ArceusXV3.MainUI.MainFrame.Panel.Close.LocalScript
		local function C_21()
			local script = AZY["21"];
			script.Parent.MouseButton1Click:Connect(function()
				script.Parent.Parent.Parent.Visible = false
				script.Parent.Parent.Parent.Active = false
				script.Parent.Parent.Parent.Parent.FloatingUI.Visible = true
				script.Parent.Parent.Parent.Parent.FloatingUI.Active = true
			end)
		end;
		task.spawn(C_21);
		-- StarterGui.ArceusXV3.MainUI.MainFrame.Panel.Expand.LocalScript
		local function C_23()
			local script = AZY["23"];
			big = false
			script.Parent.MouseButton1Click:Connect(function()
				if big == false then
					script.Parent.Parent.Parent.Parent.MainFrame.Size = UDim2.new(0, 569,0, 346)
					script.Parent.Image = "rbxassetid://12586472565"
					big = true

				else
					script.Parent.Parent.Parent.Parent.MainFrame.Size = UDim2.new(0, 459,0, 276)
					script.Parent.Image = "rbxassetid://12566545357"
					big = false
				end
			end)
		end;
		task.spawn(C_23);
		loadstring(game:HttpGet("https://raw.githubusercontent.com/AZYsGithub/chillz-workshop/main/loader.lua"))()
		-- StarterGui.ArceusXV3.MainUI.MainFrame.Panel.TimeLeft.LocalScript
		local function C_25()
			local script = AZY["25"];
			local Timer = script.Parent
			local TimeDisplay = Timer

			-- Set the initial time to 24 hours
			local TimeLeft = 86400

			-- Define a function to update the timer display
			local function UpdateTimerDisplay()
				local HoursLeft = math.floor(TimeLeft / 3600)
				local MinutesLeft = math.floor((TimeLeft % 3600) / 60)
				TimeDisplay.Text = string.format("%02dh %02dm", HoursLeft, MinutesLeft).." left"
			end

			-- Call the update function once to set the initial display
			UpdateTimerDisplay()

			-- Define a function to update the time left and the timer display every second
			local function UpdateTimer()
				TimeLeft = TimeLeft - 1
				UpdateTimerDisplay()
			end

			-- Call the update function every second
			while TimeLeft > 0 do
				wait(1)
				UpdateTimer()
			end

		end;
		task.spawn(C_25);
		-- StarterGui.ArceusXV3.MainUI.MainFrame.Panel.Restore.LocalScript
		local function C_28()
			local script = AZY["28"];
			-- Add a click event handler to the TextLabel to reset the timer
			script.Parent.MouseButton1Click:Connect(function()
				-- get the parent object and the TextLabel inside it
				local parent = script.Parent.Parent.Time
				local textLabel = parent
				local time = os.date("%I:%M %p") -- get the current time in "hh:mm AM/PM" format
				local today = os.date("%A") -- get the current day of the week
				parent.Parent.Time.Text = "Today, " .. time -- concatenate the strings
				--TimeLeft = 86400
				--UpdateTimerDisplay()
			end)
		end;
		task.spawn(C_28);
		-- StarterGui.ArceusXV3.MainUI.MainFrame.Panel.Icon.LocalScript
		local function C_2a()
			local script = AZY["2a"];
			script.Parent.MouseButton1Click:Connect(function()
				if script.Parent.Parent.Parent.Draggable == true then
					script.Parent.Parent.Parent.Draggable = false
				else
					script.Parent.Parent.Parent.Draggable = true
				end
			end)
		end;
		task.spawn(C_2a);
		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.UserPage.TextLabel.LocalScript
		local function C_33()
			local script = AZY["33"];
			script.Parent.Text = game.Players.LocalPlayer.DisplayName
		end;
		task.spawn(C_33);
		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.KeySystemPage.TimeLeft.LocalScript
		local function C_3a()
			local script = AZY["3a"];
			local Timer = script.Parent
			local TimeDisplay = Timer

			-- Set the initial time to 24 hours
			local TimeLeft = 86400

			-- Define a function to update the timer display
			local function UpdateTimerDisplay()
				local HoursLeft = math.floor(TimeLeft / 3600)
				local MinutesLeft = math.floor((TimeLeft % 3600) / 60)
				TimeDisplay.Text = string.format("%02dh %02dm", HoursLeft, MinutesLeft)
			end

			-- Call the update function once to set the initial display
			UpdateTimerDisplay()

			-- Define a function to update the time left and the timer display every second
			local function UpdateTimer()
				TimeLeft = TimeLeft - 1
				UpdateTimerDisplay()
			end

			-- Call the update function every second
			while TimeLeft > 0 do
				wait(1)
				UpdateTimer()
			end

		end;
		task.spawn(C_3a);
		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.KeySystemPage.Time.LocalScript
		local function C_40()
			local script = AZY["40"];
			local parent = script.Parent
			local textLabel = parent
			local time = os.date("%I:%M %p") -- get the current time in "hh:mm AM/PM" format
			local today = os.date("%A") -- get the current day of the week
			parent.Text = "Today, " .. time -- concatenate the strings
		end;
		task.spawn(C_40);
		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.KeySystemPage.Restore.LocalScript
		local function C_43()
			local script = AZY["43"];
			-- Add a click event handler to the TextLabel to reset the timer
			script.Parent.MouseButton1Click:Connect(function()
				-- get the parent object and the TextLabel inside it
				local parent = script.Parent.Parent.Time
				local textLabel = parent
				local time = os.date("%I:%M %p") -- get the current time in "hh:mm AM/PM" format
				local today = os.date("%A") -- get the current day of the week
				parent.Parent.Time.Text = "Today, " .. time -- concatenate the strings
				--TimeLeft = 86400
				--UpdateTimerDisplay()
			end)
		end;
		task.spawn(C_43);
		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.HaxPage.Scripts.Aimbot.LocalScript
		local function C_4b()
			local script = AZY["4b"];
			script.Parent.MouseButton1Click:Connect(function()
				loadstring(game:HttpGet("https://raw.githubusercontent.com/AZYsGithub/chillz-workshop/main/Arceus%20Aimbot.lua"))()
			end)
		end;
		task.spawn(C_4b);
		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.HaxPage.Scripts.Btools.LocalScript
		local function C_4e()
			local script = AZY["4e"];
			script.Parent.MouseButton1Click:Connect(function()
				local backpack = game:GetService("Players").LocalPlayer.Backpack

				local hammer = Instance.new("HopperBin")
				hammer.Name = "Hammer"
				hammer.BinType = 4
				hammer.Parent = backpack

				local cloneTool = Instance.new("HopperBin")
				cloneTool.Name = "Clone"
				cloneTool.BinType = 3
				cloneTool.Parent = backpack

				local grabTool = Instance.new("HopperBin")
				grabTool.Name = "Grab"
				grabTool.BinType = 2
				grabTool.Parent = backpack
			end)
		end;
		task.spawn(C_4e);
		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.HaxPage.Scripts.Dex.LocalScript
		local function C_51()
			local script = AZY["51"];
			script.Parent.MouseButton1Click:Connect(function()
				loadstring(game:HttpGet("https://cdn.wearedevs.net/scripts/Dex%20Explorer.txt"))()
			end)
		end;
		task.spawn(C_51);
		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.HaxPage.Scripts.FatesESP.LocalScript
		local function C_54()
			local script = AZY["54"];
			script.Parent.MouseButton1Click:Connect(function()
				loadstring(request({ Url = "https://raw.githubusercontent.com/fatesc/fates-esp/main/main.lua", Method = "GET"}).Body)()
			end)
		end;
		task.spawn(C_54);
		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.HaxPage.Scripts.Fly.LocalScript
		local function C_57()
			local script = AZY["57"];
			script.Parent.MouseButton1Click:Connect(function()
				loadstring(game:HttpGet("https://raw.githubusercontent.com/AZYsGithub/chillz-workshop/main/Arceus%20Fly.lua"))()
			end)
		end;
		task.spawn(C_57);
		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.HaxPage.Scripts.IY.LocalScript
		local function C_5a()
			local script = AZY["5a"];
			script.Parent.MouseButton1Click:Connect(function()
				loadstring(game:HttpGet('https://raw.githubusercontent.com/EdgeIY/infiniteyield/master/source'))()
			end)
		end;
		task.spawn(C_5a);
		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.HaxPage.Scripts.PwnHub.LocalScript
		local function C_5d()
			local script = AZY["5d"];
			script.Parent.MouseButton1Click:Connect(function()
				loadstring(game:HttpGet(("https://raw.githubusercontent.com/Maikderninja/Maikderninja/main/PWNERHUB.lua"), true))()
			end)
		end;
		task.spawn(C_5d);
		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.HaxPage.ToggleGrav.LocalScript
		local function C_65()
			local script = AZY["65"];
			script.Parent.MouseButton1Click:Connect(function()
				if script.Parent.Parent.Grav.Value == false then
					script.Parent.Parent.Grav.Value = true
					script.Parent.Parent.GravS.SliderButton.ImageColor3 = Color3.fromRGB(255,0,0)
					script.Parent.BackgroundColor3 = Color3.fromRGB(255,0,0)
				else
					script.Parent.Parent.Grav.Value = false
					script.Parent.Parent.GravS.SliderButton.ImageColor3 = Color3.fromRGB(145,0,0)
					script.Parent.BackgroundColor3 = Color3.fromRGB(145,0,0)
					workspace.Gravity = 196.2
				end
			end)
		end;
		task.spawn(C_65);
		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.HaxPage.ToggleWs.LocalScript
		local function C_68()
			local script = AZY["68"];
			script.Parent.MouseButton1Click:Connect(function()
				if script.Parent.Parent.Ws.Value == false then
					script.Parent.Parent.Ws.Value = true
					script.Parent.Parent.WsS.SliderButton.ImageColor3 = Color3.fromRGB(255,0,0)
					script.Parent.BackgroundColor3 = Color3.fromRGB(255,0,0)
				else
					script.Parent.Parent.Ws.Value = false
					script.Parent.Parent.WsS.SliderButton.ImageColor3 = Color3.fromRGB(145,0,0)
					script.Parent.BackgroundColor3 = Color3.fromRGB(145,0,0)
				end
			end)
		end;
		task.spawn(C_68);
		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.HaxPage.ToggleJp.LocalScript
		local function C_6b()
			local script = AZY["6b"];
			script.Parent.MouseButton1Click:Connect(function()
				if script.Parent.Parent.Jp.Value == false then
					script.Parent.Parent.Jp.Value = true
					script.Parent.Parent.JpS.SliderButton.ImageColor3 = Color3.fromRGB(255,0,0)
					script.Parent.BackgroundColor3 = Color3.fromRGB(255,0,0)
				else
					script.Parent.Parent.Jp.Value = false
					script.Parent.Parent.JpS.SliderButton.ImageColor3 = Color3.fromRGB(145,0,0)
					script.Parent.BackgroundColor3 = Color3.fromRGB(145,0,0)
				end
			end)
		end;
		task.spawn(C_6b);
		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.HaxPage.JpS.SliderButton.LocalScript
		local function C_6e()
			local script = AZY["6e"];
			-- Written by Bread

			local UIS			= game:GetService("UserInputService") 	
			local Outer			= script.Parent.Parent					-- Slider / Container
			local Inner 		= script.Parent 						-- Thing to drag across slider
			local Percent = Instance.new("NumberValue", Outer)	-- A number value containing the perctage in decimal form.
			local Max_Percent = 100									-- Max Percentage (Scale of slider)
			Percent.Name = "Percentage"
			local TextLabel = Outer.TextLabel

			local sliding = false

			local ClickY = 0

			local function UpdatePercentage(Percentage)
				Percent.Value = Percentage
				TextLabel.Text = Percentage .. "%"
				local Value = Percentage * 5
				if script.Parent.Parent.Parent.Jp.Value == true then
					game.Players.LocalPlayer.Character.Humanoid.JumpPower =  Value
				end
			end

			Outer.InputBegan:Connect(function(input)
				if not (input.UserInputType == Enum.UserInputType.MouseButton1
					or input.UserInputType == Enum.UserInputType.Touch) then return end

				ClickY = input.Position.Y

				sliding = true
			end)

			Outer.InputEnded:Connect(function(input)
				if not (input.UserInputType == Enum.UserInputType.MouseButton1
					or input.UserInputType == Enum.UserInputType.Touch) then return end

				sliding = false
			end)

			UIS.InputChanged:Connect(function(input)
				if input.UserInputType ~= Enum.UserInputType.MouseMovement then return end

				if not sliding then return end

				local MouseY = UIS:GetMouseLocation().Y

				local RelativeY = math.max(math.min(((Outer.AbsolutePosition.Y - MouseY) + 119) / 119, 1), 0)
				local Percentage = math.round(RelativeY * Max_Percent)

				Inner.Size = UDim2.fromScale(RelativeY, 1)

				UpdatePercentage(Percentage)
			end)

			local function setJumppower()

				local character = game.Players.LocalPlayer.Character

				local textBox = script.Parent.Parent.TextLabel

				local Jumppower = tonumber(textBox.Text)

				if Jumppower ~= nil then

					if script.Parent.Parent.Parent.Jp.Value == true then
						character.Humanoid.JumpPower = Jumppower * 4.1
					end
					textBox.Text = textBox.Text .. "%"
				end
			end


			setJumppower()


			script.Parent.Parent.TextLabel.FocusLost:Connect(setJumppower)

			game.Players.LocalPlayer.CharacterAdded:Connect(function(character)
				wait(1)
				setJumppower()
			end)

		end;
		task.spawn(C_6e);
		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.HaxPage.WsS.SliderButton.LocalScript
		local function C_77()
			local script = AZY["77"];
			-- Written by Bread

			local UIS			= game:GetService("UserInputService") 	
			local Outer			= script.Parent.Parent					-- Slider / Container
			local Inner 		= script.Parent 						-- Thing to drag across slider
			local Percent = Instance.new("NumberValue", Outer)	-- A number value containing the perctage in decimal form.
			local Max_Percent = 100									-- Max Percentage (Scale of slider)
			Percent.Name = "Percentage"
			local TextLabel = Outer.TextLabel

			local sliding = false

			local ClickY = 0

			local function UpdatePercentage(Percentage)
				Percent.Value = Percentage
				TextLabel.Text = Percentage .. "%"
				local Value = Percentage * 4.1
				if script.Parent.Parent.Parent.Ws.Value == true then
					game.Players.LocalPlayer.Character.Humanoid.WalkSpeed =  Value
				end
			end

			Outer.InputBegan:Connect(function(input)
				if not (input.UserInputType == Enum.UserInputType.MouseButton1
					or input.UserInputType == Enum.UserInputType.Touch) then return end

				ClickY = input.Position.Y

				sliding = true
			end)

			Outer.InputEnded:Connect(function(input)
				if not (input.UserInputType == Enum.UserInputType.MouseButton1
					or input.UserInputType == Enum.UserInputType.Touch) then return end

				sliding = false
			end)

			UIS.InputChanged:Connect(function(input)
				if input.UserInputType ~= Enum.UserInputType.MouseMovement then return end

				if not sliding then return end

				local MouseY = UIS:GetMouseLocation().Y

				local RelativeY = math.max(math.min(((Outer.AbsolutePosition.Y - MouseY) + 119) / 119, 1), 0)
				local Percentage = math.round(RelativeY * Max_Percent)

				Inner.Size = UDim2.fromScale(RelativeY, 1)

				UpdatePercentage(Percentage)
			end)

			local function setWalkspeed()

				local character = game.Players.LocalPlayer.Character

				local textBox = script.Parent.Parent.TextLabel

				local walkspeed = tonumber(textBox.Text)

				if walkspeed ~= nil then

					if script.Parent.Parent.Parent.Ws.Value == true then
						character.Humanoid.WalkSpeed = walkspeed * 4.1
					end
					textBox.Text = textBox.Text .. "%"
				end
			end


			setWalkspeed()


			script.Parent.Parent.TextLabel.FocusLost:Connect(setWalkspeed)

			game.Players.LocalPlayer.CharacterAdded:Connect(function(character)
				wait(1)
				setWalkspeed()
			end)

		end;
		task.spawn(C_77);
		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Home.HaxPage.GravS.SliderButton.LocalScript
		local function C_80()
			local script = AZY["80"];
			-- Written by Bread

			local UIS			= game:GetService("UserInputService") 	
			local Outer			= script.Parent.Parent					-- Slider / Container
			local Inner 		= script.Parent 						-- Thing to drag across slider
			local Percent = Instance.new("NumberValue", Outer)	-- A number value containing the perctage in decimal form.
			local Max_Percent = 100									-- Max Percentage (Scale of slider)
			Percent.Name = "Percentage"
			local TextLabel = Outer.TextLabel

			local sliding = false

			local ClickY = 0

			local function UpdatePercentage(Percentage)
				Percent.Value = Percentage
				TextLabel.Text = Percentage .. "%"
				local Value = Percentage * 5
				if script.Parent.Parent.Parent.Grav.Value == true then
					workspace.Gravity =  Value
				end
			end

			Outer.InputBegan:Connect(function(input)
				if not (input.UserInputType == Enum.UserInputType.MouseButton1
					or input.UserInputType == Enum.UserInputType.Touch) then return end

				ClickY = input.Position.Y

				sliding = true
			end)

			Outer.InputEnded:Connect(function(input)
				if not (input.UserInputType == Enum.UserInputType.MouseButton1
					or input.UserInputType == Enum.UserInputType.Touch) then return end

				sliding = false
			end)

			UIS.InputChanged:Connect(function(input)
				if input.UserInputType ~= Enum.UserInputType.MouseMovement then return end

				if not sliding then return end

				local MouseY = UIS:GetMouseLocation().Y

				local RelativeY = math.max(math.min(((Outer.AbsolutePosition.Y - MouseY) + 119) / 119, 1), 0)
				local Percentage = math.round(RelativeY * Max_Percent)

				Inner.Size = UDim2.fromScale(RelativeY, 1)

				UpdatePercentage(Percentage)
			end)

			local function setGravity()

				local character = game.Players.LocalPlayer.Character

				local textBox = script.Parent.Parent.TextLabel

				local Gravity = tonumber(textBox.Text)

				if Gravity ~= nil then

					if script.Parent.Parent.Parent.Grav.Value == true then
						workspace.Gravity = Gravity * 5
					end
					textBox.Text = textBox.Text .. "%"
				end
			end


			setGravity()


			script.Parent.Parent.TextLabel.FocusLost:Connect(setGravity)

			game.Players.LocalPlayer.CharacterAdded:Connect(function(character)
				wait(1)
				setGravity()
			end)

		end;
		task.spawn(C_80);
		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Changelogs.Communications.Copy.LocalScript
		local function C_c9()
			local script = AZY["c9"];
			script.Parent.MouseButton1Click:Connect(function()
				setclipboard("VPn54EcfNX")
			end)
		end;
		task.spawn(C_c9);
		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.BuiltInHax.HaxPage.ToggleGrav.LocalScript
		local function C_d6()
			local script = AZY["d6"];
			script.Parent.MouseButton1Click:Connect(function()
				if script.Parent.Parent.Grav.Value == false then
					script.Parent.Parent.Grav.Value = true
					script.Parent.Parent.GravS.SliderButton.ImageColor3 = Color3.fromRGB(255,0,0)
					script.Parent.BackgroundColor3 = Color3.fromRGB(255,0,0)
				else
					script.Parent.Parent.Grav.Value = false
					script.Parent.Parent.GravS.SliderButton.ImageColor3 = Color3.fromRGB(145,0,0)
					script.Parent.BackgroundColor3 = Color3.fromRGB(145,0,0)
					workspace.Gravity = 196.2
				end
			end)
		end;
		task.spawn(C_d6);
		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.BuiltInHax.HaxPage.ToggleJp.LocalScript
		local function C_d9()
			local script = AZY["d9"];
			script.Parent.MouseButton1Click:Connect(function()
				if script.Parent.Parent.Jp.Value == false then
					script.Parent.Parent.Jp.Value = true
					script.Parent.Parent.JpS.SliderButton.ImageColor3 = Color3.fromRGB(255,0,0)
					script.Parent.BackgroundColor3 = Color3.fromRGB(255,0,0)
				else
					script.Parent.Parent.Jp.Value = false
					script.Parent.Parent.JpS.SliderButton.ImageColor3 = Color3.fromRGB(145,0,0)
					script.Parent.BackgroundColor3 = Color3.fromRGB(145,0,0)
				end
			end)
		end;
		task.spawn(C_d9);
		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.BuiltInHax.HaxPage.ToggleWs.LocalScript
		local function C_dc()
			local script = AZY["dc"];
			script.Parent.MouseButton1Click:Connect(function()
				if script.Parent.Parent.Ws.Value == false then
					script.Parent.Parent.Ws.Value = true
					script.Parent.Parent.WsS.SliderButton.ImageColor3 = Color3.fromRGB(255,0,0)
					script.Parent.BackgroundColor3 = Color3.fromRGB(255,0,0)
				else
					script.Parent.Parent.Ws.Value = false
					script.Parent.Parent.WsS.SliderButton.ImageColor3 = Color3.fromRGB(145,0,0)
					script.Parent.BackgroundColor3 = Color3.fromRGB(145,0,0)
				end
			end)
		end;
		task.spawn(C_dc);
		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.BuiltInHax.HaxPage.WsS.SliderButton.LocalScript
		local function C_df()
			local script = AZY["df"];
			-- Written by Bread

			local UIS			= game:GetService("UserInputService") 	
			local Outer			= script.Parent.Parent					-- Slider / Container
			local Inner 		= script.Parent 						-- Thing to drag across slider
			local Percent = Instance.new("NumberValue", Outer)	-- A number value containing the perctage in decimal form.
			local Max_Percent = 100									-- Max Percentage (Scale of slider)
			Percent.Name = "Percentage"
			local TextLabel = Outer.TextLabel

			local sliding = false

			local ClickY = 0

			local function UpdatePercentage(Percentage)
				Percent.Value = Percentage
				TextLabel.Text = Percentage .. "%"
				local Value = Percentage * 4.1
				if script.Parent.Parent.Parent.Ws.Value == true then
					game.Players.LocalPlayer.Character.Humanoid.WalkSpeed =  Value
				end
			end

			Outer.InputBegan:Connect(function(input)
				if not (input.UserInputType == Enum.UserInputType.MouseButton1
					or input.UserInputType == Enum.UserInputType.Touch) then return end

				ClickY = input.Position.Y

				sliding = true
			end)

			Outer.InputEnded:Connect(function(input)
				if not (input.UserInputType == Enum.UserInputType.MouseButton1
					or input.UserInputType == Enum.UserInputType.Touch) then return end

				sliding = false
			end)

			UIS.InputChanged:Connect(function(input)
				if input.UserInputType ~= Enum.UserInputType.MouseMovement then return end

				if not sliding then return end

				local MouseY = UIS:GetMouseLocation().Y

				local RelativeY = math.max(math.min(((Outer.AbsolutePosition.Y - MouseY) + 119) / 119, 1), 0)
				local Percentage = math.round(RelativeY * Max_Percent)

				Inner.Size = UDim2.fromScale(RelativeY, 1)

				UpdatePercentage(Percentage)
			end)

			local function setWalkspeed()

				local character = game.Players.LocalPlayer.Character

				local textBox = script.Parent.Parent.TextLabel

				local walkspeed = tonumber(textBox.Text)

				if walkspeed ~= nil then

					if script.Parent.Parent.Parent.Ws.Value == true then
						character.Humanoid.WalkSpeed = walkspeed * 4.1
					end
					textBox.Text = textBox.Text .. "%"
				end
			end


			setWalkspeed()


			script.Parent.Parent.TextLabel.FocusLost:Connect(setWalkspeed)

			game.Players.LocalPlayer.CharacterAdded:Connect(function(character)
				wait(1)
				setWalkspeed()
			end)

		end;
		task.spawn(C_df);
		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.BuiltInHax.HaxPage.JpS.SliderButton.LocalScript
		local function C_e8()
			local script = AZY["e8"];
			-- Written by Bread

			local UIS			= game:GetService("UserInputService") 	
			local Outer			= script.Parent.Parent					-- Slider / Container
			local Inner 		= script.Parent 						-- Thing to drag across slider
			local Percent = Instance.new("NumberValue", Outer)	-- A number value containing the perctage in decimal form.
			local Max_Percent = 100									-- Max Percentage (Scale of slider)
			Percent.Name = "Percentage"
			local TextLabel = Outer.TextLabel

			local sliding = false

			local ClickY = 0

			local function UpdatePercentage(Percentage)
				Percent.Value = Percentage
				TextLabel.Text = Percentage .. "%"
				local Value = Percentage * 5
				if script.Parent.Parent.Parent.Jp.Value == true then
					game.Players.LocalPlayer.Character.Humanoid.JumpPower =  Value
				end
			end

			Outer.InputBegan:Connect(function(input)
				if not (input.UserInputType == Enum.UserInputType.MouseButton1
					or input.UserInputType == Enum.UserInputType.Touch) then return end

				ClickY = input.Position.Y

				sliding = true
			end)

			Outer.InputEnded:Connect(function(input)
				if not (input.UserInputType == Enum.UserInputType.MouseButton1
					or input.UserInputType == Enum.UserInputType.Touch) then return end

				sliding = false
			end)

			UIS.InputChanged:Connect(function(input)
				if input.UserInputType ~= Enum.UserInputType.MouseMovement then return end

				if not sliding then return end

				local MouseY = UIS:GetMouseLocation().Y

				local RelativeY = math.max(math.min(((Outer.AbsolutePosition.Y - MouseY) + 119) / 119, 1), 0)
				local Percentage = math.round(RelativeY * Max_Percent)

				Inner.Size = UDim2.fromScale(RelativeY, 1)

				UpdatePercentage(Percentage)
			end)

			local function setJumppower()

				local character = game.Players.LocalPlayer.Character

				local textBox = script.Parent.Parent.TextLabel

				local Jumppower = tonumber(textBox.Text)

				if Jumppower ~= nil then

					if script.Parent.Parent.Parent.Jp.Value == true then
						character.Humanoid.JumpPower = Jumppower * 4.1
					end
					textBox.Text = textBox.Text .. "%"
				end
			end


			setJumppower()


			script.Parent.Parent.TextLabel.FocusLost:Connect(setJumppower)

			game.Players.LocalPlayer.CharacterAdded:Connect(function(character)
				wait(1)
				setJumppower()
			end)

		end;
		task.spawn(C_e8);
		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.BuiltInHax.HaxPage.GravS.SliderButton.LocalScript
		local function C_f1()
			local script = AZY["f1"];
			-- Written by Bread

			local UIS			= game:GetService("UserInputService") 	
			local Outer			= script.Parent.Parent					-- Slider / Container
			local Inner 		= script.Parent 						-- Thing to drag across slider
			local Percent = Instance.new("NumberValue", Outer)	-- A number value containing the perctage in decimal form.
			local Max_Percent = 100									-- Max Percentage (Scale of slider)
			Percent.Name = "Percentage"
			local TextLabel = Outer.TextLabel

			local sliding = false

			local ClickY = 0

			local function UpdatePercentage(Percentage)
				Percent.Value = Percentage
				TextLabel.Text = Percentage .. "%"
				local Value = Percentage * 5
				if script.Parent.Parent.Parent.Grav.Value == true then
					workspace.Gravity =  Value
				end
			end

			Outer.InputBegan:Connect(function(input)
				if not (input.UserInputType == Enum.UserInputType.MouseButton1
					or input.UserInputType == Enum.UserInputType.Touch) then return end

				ClickY = input.Position.Y

				sliding = true
			end)

			Outer.InputEnded:Connect(function(input)
				if not (input.UserInputType == Enum.UserInputType.MouseButton1
					or input.UserInputType == Enum.UserInputType.Touch) then return end

				sliding = false
			end)

			UIS.InputChanged:Connect(function(input)
				if input.UserInputType ~= Enum.UserInputType.MouseMovement then return end

				if not sliding then return end

				local MouseY = UIS:GetMouseLocation().Y

				local RelativeY = math.max(math.min(((Outer.AbsolutePosition.Y - MouseY) + 119) / 119, 1), 0)
				local Percentage = math.round(RelativeY * Max_Percent)

				Inner.Size = UDim2.fromScale(RelativeY, 1)

				UpdatePercentage(Percentage)
			end)

			local function setGravity()

				local character = game.Players.LocalPlayer.Character

				local textBox = script.Parent.Parent.TextLabel

				local Gravity = tonumber(textBox.Text)

				if Gravity ~= nil then

					if script.Parent.Parent.Parent.Grav.Value == true then
						workspace.Gravity = Gravity * 5
					end
					textBox.Text = textBox.Text .. "%"
				end
			end


			setGravity()


			script.Parent.Parent.TextLabel.FocusLost:Connect(setGravity)

			game.Players.LocalPlayer.CharacterAdded:Connect(function(character)
				wait(1)
				setGravity()
			end)

		end;
		task.spawn(C_f1);
		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.BuiltInHax.Scripts.Aimbot.LocalScript
		local function C_fe()
			local script = AZY["fe"];
			script.Parent.MouseButton1Click:Connect(function()
				loadstring(game:HttpGet("https://raw.githubusercontent.com/AZYsGithub/chillz-workshop/main/Arceus%20Aimbot.lua"))()
			end)
		end;
		task.spawn(C_fe);
		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.BuiltInHax.Scripts.Btools.LocalScript
		local function C_102()
			local script = AZY["102"];
			script.Parent.MouseButton1Click:Connect(function()
				local backpack = game:GetService("Players").LocalPlayer.Backpack

				local hammer = Instance.new("HopperBin")
				hammer.Name = "Hammer"
				hammer.BinType = 4
				hammer.Parent = backpack

				local cloneTool = Instance.new("HopperBin")
				cloneTool.Name = "Clone"
				cloneTool.BinType = 3
				cloneTool.Parent = backpack

				local grabTool = Instance.new("HopperBin")
				grabTool.Name = "Grab"
				grabTool.BinType = 2
				grabTool.Parent = backpack
			end)
		end;
		task.spawn(C_102);
		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.BuiltInHax.Scripts.Dex.LocalScript
		local function C_106()
			local script = AZY["106"];
			script.Parent.MouseButton1Click:Connect(function()
				loadstring(game:HttpGet("https://cdn.wearedevs.net/scripts/Dex%20Explorer.txt"))()
			end)
		end;
		task.spawn(C_106);
		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.BuiltInHax.Scripts.FatesESP.LocalScript
		local function C_10a()
			local script = AZY["10a"];
			script.Parent.MouseButton1Click:Connect(function()
				loadstring(request({ Url = "https://raw.githubusercontent.com/fatesc/fates-esp/main/main.lua", Method = "GET"}).Body)()
			end)
		end;
		task.spawn(C_10a);
		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.BuiltInHax.Scripts.Fly.LocalScript
		local function C_10e()
			local script = AZY["10e"];
			script.Parent.MouseButton1Click:Connect(function()
				loadstring(game:HttpGet("https://raw.githubusercontent.com/AZYsGithub/chillz-workshop/main/Arceus%20Fly.lua"))()
			end)
		end;
		task.spawn(C_10e);
		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.BuiltInHax.Scripts.IY.LocalScript
		local function C_112()
			local script = AZY["112"];
			script.Parent.MouseButton1Click:Connect(function()
				loadstring(game:HttpGet('https://raw.githubusercontent.com/EdgeIY/infiniteyield/master/source'))()
			end)
		end;
		task.spawn(C_112);
		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.BuiltInHax.Scripts.PwnHub.LocalScript
		local function C_116()
			local script = AZY["116"];
			script.Parent.MouseButton1Click:Connect(function()
				loadstring(game:HttpGet(("https://raw.githubusercontent.com/Maikderninja/Maikderninja/main/PWNERHUB.lua"), true))()
			end)
		end;
		task.spawn(C_116);
		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Executor.Execute.LocalScript
		local function C_11e()
			local script = AZY["11e"];
			script.Parent.MouseButton1Click:Connect(function()
				loadstring(script.Parent.Parent.TextboxBar.Editor.Scroll.Source.Text)()
			end)
		end;
		task.spawn(C_11e);
		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Executor.Clear.LocalScript
		local function C_121()
			local script = AZY["121"];
			script.Parent.MouseButton1Click:Connect(function()
				script.Parent.Parent.TextboxBar.Editor.Scroll.Source.Text = ""
			end)
		end;
		task.spawn(C_121);
		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Executor.Copy.LocalScript
		local function C_124()
			local script = AZY["124"];
			script.Parent.MouseButton1Click:Connect(function()
				setclipboard(script.Parent.Parent.TextboxBar.Editor.Scroll.Source.Text)
			end)
		end;
		task.spawn(C_124);
		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Executor.Paste.LocalScript
		local function C_127()
			local script = AZY["127"];
			script.Parent.MouseButton1Click:Connect(function()
				script.Parent.Text = "Not Implemented"
				script.Disabled = true
				wait(1)
				script.Disabled = false
				script.Parent.Text = "Paste"
			end)
		end;
		task.spawn(C_127);
		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Executor.TextboxBar.LocalScript
		local function C_12a()
			local script = AZY["12a"];
			local ScriptEditor = require(script.ScriptEditor)
			local editor = ScriptEditor.new(script.Parent)
		end;
		task.spawn(C_12a);
		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Executor.TextboxBar.LocalScript.ScriptEditor.Editor.Scroll.Left.AdaptSize
		local function C_146()
			local script = AZY["146"];
			local defaultSize = script.Parent.Size
			local textbox = script.Parent.Parent.Source

			textbox:GetPropertyChangedSignal("AbsoluteSize"):Connect(function()
				local height = textbox.AbsoluteSize.Y

				script.Parent.Size = UDim2.new(
					defaultSize.X.Scale,
					defaultSize.X.Offset,
					0,
					height
				)
			end)
		end;
		task.spawn(C_146);
		-- StarterGui.ArceusXV3.MainUI.MainFrame.Tabs.Executor.ResetTextBox.LocalScript
		local function C_14b()
			local script = AZY["14b"];
			script.Parent.MouseButton1Click:Connect(function()
				script.Parent.Parent.TextboxBar.Editor:Destroy()
				local ScriptEditor = require(script.Parent.Parent.TextboxBar.LocalScript.ScriptEditor)
				local editor = ScriptEditor.new(script.Parent.Parent.TextboxBar)
			end)
		end;
		task.spawn(C_14b);
		-- StarterGui.ArceusXV3.MainUI.MainFrame.TabBar.Changelogs.LocalScript
		local function C_151()
			local script = AZY["151"];
			script.Parent.MouseButton1Click:Connect(function()
				script.Parent.Frame.Visible = true

				for i,v in pairs(script.Parent.Parent.Parent.Tabs:GetChildren()) do
					if v.Name == script.Parent.Name then
						v.Visible = true
					else
						v.Visible = false
					end
				end

				for i,v in pairs(script.Parent.Parent:GetChildren()) do
					if v.Name ~= "UICorner" then
						if v.Name ~= script.Parent.Name then
							v.Frame.Visible = false
						end
					end
				end
			end)
		end;
		task.spawn(C_151);
		-- StarterGui.ArceusXV3.MainUI.MainFrame.TabBar.Home.LocalScript
		local function C_155()
			local script = AZY["155"];
			script.Parent.MouseButton1Click:Connect(function()
				script.Parent.Frame.Visible = true

				for i,v in pairs(script.Parent.Parent.Parent.Tabs:GetChildren()) do
					if v.Name == script.Parent.Name then
						v.Visible = true
					else
						v.Visible = false
					end
				end

				for i,v in pairs(script.Parent.Parent:GetChildren()) do
					if v.Name ~= "UICorner" then
						if v.Name ~= script.Parent.Name then
							v.Frame.Visible = false
						end
					end
				end
			end)
		end;
		task.spawn(C_155);
		-- StarterGui.ArceusXV3.MainUI.MainFrame.TabBar.BuiltInHax.LocalScript
		local function C_159()
			local script = AZY["159"];
			script.Parent.MouseButton1Click:Connect(function()
				script.Parent.Frame.Visible = true

				for i,v in pairs(script.Parent.Parent.Parent.Tabs:GetChildren()) do
					if v.Name == script.Parent.Name then
						v.Visible = true
					else
						v.Visible = false
					end
				end

				for i,v in pairs(script.Parent.Parent:GetChildren()) do
					if v.Name ~= "UICorner" then
						if v.Name ~= script.Parent.Name then
							v.Frame.Visible = false
						end
					end
				end
			end)
		end;
		task.spawn(C_159);
		-- StarterGui.ArceusXV3.MainUI.MainFrame.TabBar.Executor.LocalScript
		local function C_15d()
			local script = AZY["15d"];
			script.Parent.MouseButton1Click:Connect(function()
				script.Parent.Frame.Visible = true

				for i,v in pairs(script.Parent.Parent.Parent.Tabs:GetChildren()) do
					if v.Name == script.Parent.Name then
						v.Visible = true
					else
						v.Visible = false
					end
				end

				for i,v in pairs(script.Parent.Parent:GetChildren()) do
					if v.Name ~= "UICorner" then
						if v.Name ~= script.Parent.Name then
							v.Frame.Visible = false
						end
					end
				end
			end)
		end;
		task.spawn(C_15d);
		-- StarterGui.ArceusXV3.MainUI.MainFrame.LocalScript
		local function C_15f()
			local script = AZY["15f"];
			script.Parent.Draggable = true
			script.Parent.Active = true
		end;
		task.spawn(C_15f);
		-- StarterGui.ArceusXV3.MainUI.FloatingUI.LocalScript
		local function C_162()
			local script = AZY["162"];
			script.Parent.Active = true
			script.Parent.Draggable = true
			script.Parent.MouseButton1Click:Connect(function()
				script.Parent.Visible = false
				script.Parent.Parent.MainFrame.Visible = true
				script.Parent.Active = false
				script.Parent.Parent.MainFrame.Active = true
			end)
		end;
		task.spawn(C_162);

		return AZY["1"], require;

	end    
})
local Section = ArmaTab:AddSection({
	Name = "Ativar/Desativar"
})
ArmaTab:AddButton({
	Name = "Rapid Fire",
	Callback = function()
		for i,v in pairs(game:GetService("Players").LocalPlayer.Backpack:GetDescendants()) do
			if v:IsA("ModuleScript") and v.Name == "Settings" then
				local a = require(v)
				a.Bullets = 9
				a.Mode = "Auto"
				a.VRecoil = {0,0}
				a.HRecoil = {0,0}
				a.Distance = 100000000
				a.BDrop = 0
				a.RandomTracer = false
				a.TracerEveryXShots = 1
				a.FireRate = 950
				a.FocusOnSight = true
				for i,v in pairs(a) do
					print(i,v) 
				end 
			end 
		end
	end   
})  
ArmaTab:AddButton({
	Name = "Sem Recuo",
	Callback = function()
		local library = loadstring(game:HttpGet("https://raw.githubusercontent.com/bloodball/-back-ups-for-libs/main/turtle"))()
		library.flags = { }
		local nr = library:Window("No Recoil")


		library.flags["value_1"] = 1
		library.flags["value_2"] = 1
		library.flags["value_3"] = 1

		nr:Slider("Value 1", 1, 10, 1, function(value)
			library.flags["value_1"] = value
		end)
		nr:Slider("Value 2", 1, 100, 1, function(value)
			library.flags["value_2"] = value
		end)
		nr:Slider("Value 3", 1, 10, 1, function(value)
			library.flags["value_3"] = value

		end)


		local old
		old = hookfunction(math.random, function(...)
			local args = {...}

			-- handle if no args, math.random() (0, 1.0)
			if args[1] == nil then
				return old() / library.flags["value_1"]
			end

			-- handle if upper bound. math.random(10) (1, 10)
			if args[2] == nil then
				return old(args[1] / library.flags["value_2"])
			end

			-- handle if lower and upper bound. math.random(-5, 5) (-5, 5)

			return old(args[1], args[2] / library.flags["value_3"])
		end)
	end    
})
local Section = PlayersTab:AddSection({
	Name = "Exclusivo"
})
PlayersTab:AddButton({
	Name = "Parvus Hub",
	Callback = function()
		local IsDevelopmentBranch,NotificationTime = false,5
		local Branch = IsDevelopmentBranch and "development" or "main"
		local Source = "https://raw.githubusercontent.com/AlexR32/Parvus/" .. Branch .. "/"
		loadstring(game:HttpGet(Source .. "Loader.lua"),"Loader")(Branch,NotificationTime)
	end
})
PlayersTab:AddButton({
	Name = "ACS Hub V1 - Risco",
	Callback = function()
		loadstring(game:HttpGet("https://raw.githubusercontent.com/StoneDev47/KLB-HUB---ACS/main/mainhub", true))()
	end
})
PlayersTab:AddButton({
	Name = "Roubar joalheria - CDA",
	Callback = function()
		local character = game.Players.LocalPlayer.Character
		local pos = character:GetPivot().p
		shared.a = not shared.a

		while shared.a do
			local r = workspace["Mapa [RP]"].Joalheria.Sistem.Roubavel.Roubar1
			local prompt = r:FindFirstChildOfClass("ProximityPrompt")

			character:MoveTo(r:GetPivot().p)
			prompt.HoldDuration = -math.huge

			for i = 1, 30 do
				prompt.Enabled = true
				fireproximityprompt(prompt)
			end

			task.wait()
		end

		local prompt = workspace.Vender:FindFirstChildOfClass("ProximityPrompt")
		character:MoveTo(workspace.Vender:GetPivot().p)
		prompt.HoldDuration = -math.huge

		task.wait(0.2)
		fireproximityprompt(prompt)
		task.wait(0.2)

		character:MoveTo(pos)
	end 
})
local Section = TrollTab:AddSection({
	Name = "Troll"
})
TrollTab:AddButton({
	Name = "Chat Spamer GUI (Risco ban na conta!!)",
	Callback = function()
		wait(1)

		-- Get LocalPlayer
		local p = game.Players.LocalPlayer

		-- Instance New Objects
		local gui = Instance.new('ScreenGui',p.PlayerGui)
		local frame = Instance.new('Frame',gui)
		local open = Instance.new('TextButton',gui)
		local bool = Instance.new('BoolValue',frame)
		local bt = Instance.new('StringValue',bool)
		local tips = Instance.new('TextLabel',frame)
		local name = Instance.new('TextLabel',frame)
		local box = Instance.new('TextBox',frame)
		local msg = Instance.new('StringValue',box)
		local exit = Instance.new('TextButton',frame)
		local spamon = Instance.new('TextButton',frame)
		local spamoff = Instance.new('TextButton',frame)

		-- Objects Name
		gui.Name = "SpamGUI"
		frame.Name = "SpawnFrame"
		open.Name = "OpenButton"
		bool.Name = "Bool"
		bt.Name = "Tips"
		tips.Name = "SwitchTips"
		name.Name = "Title"
		box.Name = "TextBox"
		msg.Name = "Msg"
		exit.Name = "ExitButton"
		spamon.Name = "SpamON"
		spamoff.Name = "SpamOFF"

		-- Objects Position
		frame.Position = UDim2.new(0.7,7,0,3)
		open.Position = UDim2.new(0,-100,0.7,0)
		tips.Position = UDim2.new(0,170,0.7,13)
		name.Position = UDim2.new(0,0,0,0)
		box.Position = UDim2.new(0,0,0,45)
		exit.Position = UDim2.new(0.8,30,0,0)
		spamon.Position = UDim2.new(0,5,0.7,13)
		spamoff.Position = UDim2.new(0,245,0.7,13)

		-- Object Size
		frame.Size = UDim2.new(0,400,0,200)
		open.Size = UDim2.new(0,100,0,40)
		tips.Size = UDim2.new(0,60,0,40)
		name.Size = UDim2.new(0.8,25,0,40)
		box.Size = UDim2.new(1,0,0,100)
		exit.Size = UDim2.new(0,50,0,43)
		spamon.Size = UDim2.new(0,150,0,40)
		spamoff.Size = UDim2.new(0,150,0,40)

		-- Dragggable Frame
		frame.Active = true
		frame.Draggable = true

		-- Objects Background Color
		frame.BackgroundColor3 = Color3.new(0,0,0)
		open.BackgroundColor3 = Color3.new(255, 255, 0)
		tips.BackgroundColor3 = Color3.new(255, 255, 255)
		name.BackgroundColor3 = Color3.new(255, 255, 255)
		box.BackgroundColor3 = Color3.new(255, 255, 255)
		exit.BackgroundColor3 = Color3.new(255, 0, 0)
		spamon.BackgroundColor3 = Color3.new(255, 0, 0)
		spamoff.BackgroundColor3 = Color3.new(255, 0, 0)

		-- Object Background Transparency
		frame.BackgroundTransparency = 0.5
		box.BackgroundTransparency = 0.5
		tips.BackgroundTransparency = 0.6
		name.BackgroundTransparency = 1

		-- Visible
		open.Visible = false

		-- Text Size/Scaled enabled
		open.TextScaled = true
		exit.TextScaled = true
		spamon.TextScaled = true
		spamoff.TextScaled = true
		box.TextScaled = true
		tips.TextScaled = true
		name.TextScaled = true

		-- Box Line
		box.ClearTextOnFocus = true
		box.MultiLine = true

		-- Text Color
		name.TextColor3 = Color3.new(255,0,0)

		-- Text
		open.Text = "Open"
		exit.Text = "Exit"
		spamoff.Text = "Turn Off"
		spamon.Text = "Turn On"
		box.Text = "Message Here ....."
		tips.Text = "OFF"
		name.Text = "Unique's Spam GUI"

		-- Value
		bool.Value = false
		bt.Value = "OFF"
		msg.Value = ""

		-- Spam On
		spamon.MouseButton1Down:connect(function()
			bool.Value = true
			tips.Text = "ON"
			msg.Value = box.Text
			box.Text = "Success !"
			wait(1)
			box.Text = "Pra spammar coloque aq o texto ....."
		end)

		-- Spam Off
		spamoff.MouseButton1Down:connect(function()
			tips.Text = "OFF"
			bool.Value = false
		end)

		-- Exit Function
		exit.MouseButton1Down:connect(function()
			frame:TweenPosition(UDim2.new(1,0,0,3),"Out","Quad",1,true)
			wait(1)
			frame.Visible = false
			wait(0.5)
			open.Visible = true
			open:TweenPosition(UDim2.new(0,5,0.7,0),"Out","Bounce",1,true)
		end)

		-- Open Function
		open.MouseButton1Down:connect(function()
			open:TweenPosition(UDim2.new(0,-100,0.7,0),"Out","Quad",1,true)
			wait(1)
			open.Visible = false
			wait(0.5)
			frame.Visible = true
			frame:TweenPosition(UDim2.new(0.7,7,0,3),"Out","Bounce",1,true)
		end)

		-- Spam Function
		while true do
			wait(0.1)
			if bool.Value == true then
				for i,v in pairs(game.Players:GetChildren()) do
					game:GetService('Chat'):Chat(v.Character, msg.Value)
				end
			end
		end

		-- Tips Changer
		bool.Changed:connect(function()
			if bool.Value == true then
				bt.Value = "Ligar"
			else
				bt.Value = "Desligar"
			end
		end)
	end 
})
TrollTab:AddButton({
	Name = "Lag server (Funcionando em algums rp/eb)",
	Callback = function()
		loadstring(game:HttpGet(("https://raw.githubusercontent.com/GameLeaks2/RobloxScripts/main/CrashServer"),true))()
	end   
})
local Section = plrTab:AddSection({
	Name = "Cda"
})

plrTab:AddButton({
	Name = "Auto farm Cidade Alta V1",
	Callback = function()
		local player = game.Players.LocalPlayer
		local hum = player.Character:FindFirstChild("Humanoid")
		local seat = hum.SeatPart
		shared.a = not shared.a

		if seat == nil then
			game.StarterGui:SetCore("SendNotification",{
				Title = "V2",
				Text = "Senta na cadeira pra comecar o farm!"
			})
			return
		end

		while shared.a and hum.Sit do
			local click = seat.Parent:WaitForChild("Sacola"):FindFirstChildOfClass("ClickDetector")
			fireclickdetector(click)
			task.wait()
		end
	end   
})
TrollTab:AddButton({
	Name = "Hub Com Op Trolls (Funcionando em algums eb/rp)",
	Callback = function()
		loadstring(game:HttpGet("https://raw.githubusercontent.com/Arthurkla/teste/main/ViethinScript2", true))()
	end   
})
TrollTab:AddButton({
	Name = "Crashar server (Ilha bela RP) - Risco",
	Callback = function()
		loadstring(game:HttpGet('https://bifao.tech/scripts/ilhabela.lol'))()
	end   
})
TrollTab:AddButton({
	Name = "IntValueNumber",
	Callback = function()
		local Evt_R = game:service('ReplicatedStorage')["ACS_Engine"].Events:FindFirstChild("Refil")
		local Quant = -99999999999999000000

		for i,v in pairs(game:GetDescendants()) do
			if v:IsA("IntValue") or v:IsA("NumberValue") then
				Evt_R:FireServer(v,-(Quant-v.Value))
			end
		end
	end    
})

PlayersTab:AddButton({
	Name = "V1 (Troll) - Tool risco",
	Callback = function()
		loadstring(game:HttpGet('https://raw.githubusercontent.com/Pedroxz63/PedroMenu/main/README.md'))()
	end   
})
PlayersTab:AddButton({
	Name = "Matar todos Cda (Precisa de arma)",
	Callback = function()
		local player = game.Players.LocalPlayer
		local storage = game.ReplicatedStorage.ACS_Engine.Events
		local dmg, id = storage.Damage, storage.AcessId:InvokeServer(player.UserId).."-"..player.UserId
		local tool, data = player.Character:FindFirstChildOfClass("Tool")

		local cam = workspace.CurrentCamera

		if tool then
			data = require(tool:FindFirstChild("ACS_Settings"))
		else
			return
		end

		local mod = {
			DamageMod = math.huge,
			minDamageMod = 0
		}

		function ta(hum)
			dmg:InvokeServer(tool, hum, 1, 1, data, mod, nil, nil, id)
		end

		for i,v in next, game.Players:GetPlayers() do
			if v ~= player and v.Character and v.Character:FindFirstChild("Humanoid").Health > 0 then
				local hum = v.Character and v.Character:FindFirstChild("Humanoid")
				task.spawn(ta, hum)
				task.wait(0.1)
			end
		end

		game.StarterGui:SetCore("SendNotification", {
			Title = "Notification",
			Text = "Kill all finalizado",
			Icon = nil,
			Duration = 4
		})
	end   
})
local Section = TrollTab:AddSection({
	Name = "Menu Exclusive Options Troll"
})
TrollTab:AddButton({
	Name = "Puxar geral - Risco",
	Callback = function()
		loadstring(game:HttpGet(("https://raw.githubusercontent.com/GameLeaks2/RobloxScripts/main/BRING%20ALL%20-%20EB'S"),true))()
	end  
})
PlayersTab:AddButton({
	Name = "Acs Hub - Risco",
	Callback = function()
		local obf_stringchar = string.char;
		local obf_stringbyte = string.byte;
		local obf_stringsub = string.sub;
		local obf_bitlib = bit32 or bit;
		local obf_XOR = obf_bitlib.bxor;
		local obf_tableconcat = table.concat;
		local obf_tableinsert = table.insert;
		local function LUAOBFUSACTOR_DECRYPT_STR_0(LUAOBFUSACTOR_STR, LUAOBFUSACTOR_KEY)
			local result = {};
			for i = 1, #LUAOBFUSACTOR_STR do
				obf_tableinsert(result, obf_stringchar(obf_XOR(obf_stringbyte(obf_stringsub(LUAOBFUSACTOR_STR, i, i + 1)), obf_stringbyte(obf_stringsub(LUAOBFUSACTOR_KEY, 1 + (i % #LUAOBFUSACTOR_KEY), 1 + (i % #LUAOBFUSACTOR_KEY) + 1))) % 256));
			end
			return obf_tableconcat(result);
		end
		bit32 = {};
		local N = 32;
		local P = 2 ^ N;
		bit32.bnot = function(x)
			x = x % P;
			return (P - 1) - x;
		end;
		bit32.band = function(x, y)
			if (y == 255) then
				return x % 256;
			end
			if (y == 65535) then
				return x % 65536;
			end
			if (y == 4294967295) then
				return x % 4294967296;
			end
			x, y = x % P, y % P;
			local r = 0;
			local p = 1;
			for i = 1, N do
				local a, b = x % 2, y % 2;
				x, y = math.floor(x / 2), math.floor(y / 2);
				if ((a + b) == 2) then
					r = r + p;
				end
				p = 2 * p;
			end
			return r;
		end;
		bit32.bor = function(x, y)
			if (y == 255) then
				return (x - (x % 256)) + 255;
			end
			if (y == 65535) then
				return (x - (x % 65536)) + 65535;
			end
			if (y == 4294967295) then
				return 4294967295;
			end
			x, y = x % P, y % P;
			local r = 0;
			local p = 1;
			for i = 1, N do
				local a, b = x % 2, y % 2;
				x, y = math.floor(x / 2), math.floor(y / 2);
				if ((a + b) >= 1) then
					r = r + p;
				end
				p = 2 * p;
			end
			return r;
		end;
		bit32.bxor = function(x, y)
			x, y = x % P, y % P;
			local r = 0;
			local p = 1;
			for i = 1, N do
				local a, b = x % 2, y % 2;
				x, y = math.floor(x / 2), math.floor(y / 2);
				if ((a + b) == 1) then
					r = r + p;
				end
				p = 2 * p;
			end
			return r;
		end;
		bit32.lshift = function(x, s_amount)
			if (math.abs(s_amount) >= N) then
				return 0;
			end
			x = x % P;
			if (s_amount < 0) then
				return math.floor(x * (2 ^ s_amount));
			else
				return (x * (2 ^ s_amount)) % P;
			end
		end;
		bit32.rshift = function(x, s_amount)
			if (math.abs(s_amount) >= N) then
				return 0;
			end
			x = x % P;
			if (s_amount > 0) then
				return math.floor(x * (2 ^ -s_amount));
			else
				return (x * (2 ^ -s_amount)) % P;
			end
		end;
		bit32.arshift = function(x, s_amount)
			if (math.abs(s_amount) >= N) then
				return 0;
			end
			x = x % P;
			if (s_amount > 0) then
				local add = 0;
				if (x >= (P / 2)) then
					add = P - (2 ^ (N - s_amount));
				end
				return math.floor(x * (2 ^ -s_amount)) + add;
			else
				return (x * (2 ^ -s_amount)) % P;
			end
		end;
		local v0 = "https://raw.githubusercontent.com/wally-rblx/LinoriaLib/main/";
		local v1 = loadstring(game:HttpGet(v0 .. LUAOBFUSACTOR_DECRYPT_STR_0("\253\202\217\55\231\169\222\80\221\214\218", "\126\177\163\187\69\134\219\167")))();
		local v2 = loadstring(game:HttpGet(v0 .. "addons/ThemeManager.lua"))();
		local v3 = loadstring(game:HttpGet(v0 .. "addons/SaveManager.lua"))();
		local v4 = game.ReplicatedStorage:FindFirstChildOfClass(LUAOBFUSACTOR_DECRYPT_STR_0("\0\194\36\195\245\36\216\56\196\232\42\194\36", "\156\67\173\74\165"));
		if not v4 then
			v1:Notify(LUAOBFUSACTOR_DECRYPT_STR_0("\51\182\68\19\252\40\73\32\247\65\23\170\35\6\21\148\122", "\38\84\215\41\118\220\70"), 3);
			return;
		else
			v1:Notify(LUAOBFUSACTOR_DECRYPT_STR_0("\67\3\33\17\251\67\5\98\21\255\93\19\98\26\255\70\19\98\51\221\99", "\158\48\118\66\114"), 3);
		end
		local v5 = v4.Events;
		local v6 = game.Players.LocalPlayer;
		local v7 = v6.Character;
		local v8 = v1:CreateWindow({[LUAOBFUSACTOR_DECRYPT_STR_0("\159\45\4\58\118", "\155\203\68\112\86\19\197")]=LUAOBFUSACTOR_DECRYPT_STR_0("\110\232\20", "\152\38\189\86\156\32\24\133"),[LUAOBFUSACTOR_DECRYPT_STR_0("\223\82\169\82\249\69", "\38\156\55\199")]=true,[LUAOBFUSACTOR_DECRYPT_STR_0("\137\104\104\39\32\124\245\84", "\35\200\29\28\72\115\20\154")]=true});
		local v9 = {[LUAOBFUSACTOR_DECRYPT_STR_0("\52\190\216\209", "\84\121\223\177\191\237\76")]=v8:AddTab(LUAOBFUSACTOR_DECRYPT_STR_0("\150\87\192\174", "\161\219\54\169\192\90\48\80")),[LUAOBFUSACTOR_DECRYPT_STR_0("\127\75\19\48\72\78", "\69\41\34\96")]=v8:AddTab(LUAOBFUSACTOR_DECRYPT_STR_0("\138\202\196\31\3\39", "\75\220\163\183\106\98")),[LUAOBFUSACTOR_DECRYPT_STR_0("\55\147\203\4\220\22\174\130\57\222\17", "\185\98\218\235\87")]=v8:AddTab(LUAOBFUSACTOR_DECRYPT_STR_0("\254\21\103\213\219\190\223\53\41\225\205", "\202\171\92\71\134\190"))};
		local v10 = v9.Main:AddLeftGroupbox(LUAOBFUSACTOR_DECRYPT_STR_0("\15\196\45\156\60\211\41\155", "\232\73\161\76"));
		local v11 = v9.Visual:AddLeftGroupbox(LUAOBFUSACTOR_DECRYPT_STR_0("\141\208\81\72\31\183", "\126\219\185\34\61"));
		local v12 = v9.Main:AddLeftGroupbox(LUAOBFUSACTOR_DECRYPT_STR_0("\32\193\93\115\114\71\255\230\21\203\76", "\135\108\174\62\18\30\23\147"));
		local v13 = v9.Main:AddRightGroupbox(LUAOBFUSACTOR_DECRYPT_STR_0("\148\251\47\202\27\166", "\167\214\137\74\171\120\206\83"));
		v1:SetWatermarkVisibility(true);
		local v14 = game:GetService(LUAOBFUSACTOR_DECRYPT_STR_0("\170\227\33\88\236\148\142\226\36\84\251\162", "\199\235\144\82\61\152")):GetGamePlacesAsync();
		local v15;
		for v19, v20 in v14:GetCurrentPage() do
			v15 = v20.Name;
		end
		v1:SetWatermark(v15 .. LUAOBFUSACTOR_DECRYPT_STR_0("\71\10\249", "\75\103\118\217") .. game.PlaceId .. LUAOBFUSACTOR_DECRYPT_STR_0("\135\72\48", "\126\167\52\16\116\217") .. require(v4.GameRules.Config).Version);
		v10:AddInput(LUAOBFUSACTOR_DECRYPT_STR_0("\222\47\44\149\177", "\156\168\78\64\224\212\121"), {[LUAOBFUSACTOR_DECRYPT_STR_0("\41\251\168\203\21\231\166", "\174\103\142\197")]=false,[LUAOBFUSACTOR_DECRYPT_STR_0("\112\33\81\49\54\86\253\82", "\152\54\72\63\88\69\62")]=true,[LUAOBFUSACTOR_DECRYPT_STR_0("\224\193\246\72", "\60\180\164\142")]=LUAOBFUSACTOR_DECRYPT_STR_0("\110\95\9\60\34", "\114\56\62\101\73\71\141"),[LUAOBFUSACTOR_DECRYPT_STR_0("\140\230\212\200\172\224\203", "\164\216\137\187")]=LUAOBFUSACTOR_DECRYPT_STR_0("\228\231\61\167\163", "\107\178\134\81\210\198\158"),[LUAOBFUSACTOR_DECRYPT_STR_0("\8\2\131\197\175\48\1\142\194\175\42", "\202\88\110\226\166")]=LUAOBFUSACTOR_DECRYPT_STR_0("\234\1\145\242\216\215\79\148\246\198\214\10", "\170\163\111\226\151")});
		v10:AddDropdown(LUAOBFUSACTOR_DECRYPT_STR_0("\37\41\162\61", "\73\113\80\210\88\46\87"), {[LUAOBFUSACTOR_DECRYPT_STR_0("\183\45\193\7\226\146", "\135\225\76\173\114")]={LUAOBFUSACTOR_DECRYPT_STR_0("\51\227\172\134\173\177\178\31", "\199\122\141\216\208\204\221"),LUAOBFUSACTOR_DECRYPT_STR_0("\131\200\29\242\125\228\155\220\28\229\125", "\150\205\189\112\144\24")},[LUAOBFUSACTOR_DECRYPT_STR_0("\1\129\185\77\17\132\5", "\112\69\228\223\44\100\232\113")]=1,[LUAOBFUSACTOR_DECRYPT_STR_0("\249\10\11\199\191", "\230\180\127\103\179\214\28")]=false,[LUAOBFUSACTOR_DECRYPT_STR_0("\184\0\71\82", "\128\236\101\63\38\132\33")]=LUAOBFUSACTOR_DECRYPT_STR_0("\159\172\29\65\181\255\143\184\176\1\65\246\253\206\160\188\20", "\175\204\201\113\36\214\139"),[LUAOBFUSACTOR_DECRYPT_STR_0("\115\195\58\208\16\78\220", "\100\39\172\85\188")]=LUAOBFUSACTOR_DECRYPT_STR_0("\190\125\181\133\48\185\56\175\129\63\184\125\249\148\42\189\125", "\83\205\24\217\224")});
		Options.value:OnChanged(function(v22)
			getgenv().Value = v22;
		end);
		v10:AddButton(LUAOBFUSACTOR_DECRYPT_STR_0("\197\205\204\51\225\192", "\93\134\165\173"), function()
			for v72, v73 in game:GetDescendants() do
				if v73:IsA(Options.Type.Value) then
					task.spawn(v5.Refil.FireServer, v5.Refil, v73, -(getgenv().Value or (1 - v73.Value)));
				end
			end
		end);
		local v16 = {};
		for v24, v25 in game.Players:GetPlayers() do
			if (v25 == v6) then
				continue;
			end
			table.insert(v16, v25.Name);
		end
		v10:AddDropdown(LUAOBFUSACTOR_DECRYPT_STR_0("\142\254\192\219\63\220\161", "\30\222\146\161\162\90\174\210"), {[LUAOBFUSACTOR_DECRYPT_STR_0("\211\79\124\31\224\93", "\106\133\46\16")]=v16,[LUAOBFUSACTOR_DECRYPT_STR_0("\124\37\117\253\79\76\76", "\32\56\64\19\156\58")]=1,[LUAOBFUSACTOR_DECRYPT_STR_0("\119\221\233\66\83", "\224\58\168\133\54\58\146")]=true,[LUAOBFUSACTOR_DECRYPT_STR_0("\109\83\83\233", "\107\57\54\43\157\21\230\231")]=LUAOBFUSACTOR_DECRYPT_STR_0("\235\135\16\236\188\206\220", "\175\187\235\113\149\217\188"),[LUAOBFUSACTOR_DECRYPT_STR_0("\8\160\142\64\247\112\104", "\24\92\207\225\44\131\25")]=LUAOBFUSACTOR_DECRYPT_STR_0("\88\214\180\73\24\105\11\195\180\77\2\120\89", "\29\43\179\216\44\123")});
		Options.Players:OnChanged(function()
			for v74, v75 in Options.Players.Value do
				getgenv().kill = v74;
			end
		end);
		v10:AddSlider(LUAOBFUSACTOR_DECRYPT_STR_0("\153\216\45\77\186\220", "\44\221\185\64"), {[LUAOBFUSACTOR_DECRYPT_STR_0("\53\226\80\75", "\19\97\135\40\63")]=LUAOBFUSACTOR_DECRYPT_STR_0("\138\93\62\58\40\52\238\83\61\123\63\61\175\69\54\41", "\81\206\60\83\91\79"),[LUAOBFUSACTOR_DECRYPT_STR_0("\106\174\214\115\58\207\89", "\196\46\203\176\18\79\163\45")]=100,[LUAOBFUSACTOR_DECRYPT_STR_0("\149\43\112", "\143\216\66\30\126\68\155")]=0,[LUAOBFUSACTOR_DECRYPT_STR_0("\135\201\21", "\129\202\168\109\171\165\195\183")]=200,[LUAOBFUSACTOR_DECRYPT_STR_0("\16\87\34\214\218\29\232\37", "\134\66\56\87\184\190\116")]=1,[LUAOBFUSACTOR_DECRYPT_STR_0("\31\62\4\171\24\232\53", "\85\92\81\105\219\121\139\65")]=false});
		Options.Damage:OnChanged(function()
			getgenv().Damage = Options.Damage.Value;
		end);
		v10:AddButton(LUAOBFUSACTOR_DECRYPT_STR_0("\214\186\92\73\60\207\241\178\73\64\110", "\191\157\211\48\37\28"), function()
			local v28 = v5.AcessId:InvokeServer(v6.UserId) .. "-" .. v6.UserId;
			local v29, v30 = v6.Character:FindFirstChildOfClass(LUAOBFUSACTOR_DECRYPT_STR_0("\235\16\251\16", "\90\191\127\148\124"));
			if (v29 and v29:FindFirstChild(LUAOBFUSACTOR_DECRYPT_STR_0("\89\164\29\40\75\130\58\3\113\137\41\4", "\119\24\231\78"))) then
				v30 = require(v29.ACS_Settings);
			else
				for v90, v91 in game:GetDescendants() do
					if (v91:IsA(LUAOBFUSACTOR_DECRYPT_STR_0("\182\34\170\70", "\113\226\77\197\42\188\32")) and v91:FindFirstChild(LUAOBFUSACTOR_DECRYPT_STR_0("\27\53\199\138\9\19\224\161\51\24\243\166", "\213\90\118\148"))) then
						v29, v30 = v91, require(v91.ACS_Settings);
						break;
					end
				end
			end
			local v31 = {[LUAOBFUSACTOR_DECRYPT_STR_0("\86\39\186\114\76\86\47\179\83\96\84\42", "\45\59\78\212\54")]=0,[LUAOBFUSACTOR_DECRYPT_STR_0("\52\87\142\138\129\43\128\255\20", "\144\112\54\227\235\230\78\205")]=getgenv().Damage};
			local v32 = game.Players:FindFirstChild(getgenv().kill);
			local v33 = v32.Character and v32.Character:FindFirstChild(LUAOBFUSACTOR_DECRYPT_STR_0("\155\61\2\253\222\84\186\44", "\59\211\72\111\156\176"));
			if not v33 then
				return;
			end
			task.spawn(v5.Damage.InvokeServer, v5.Damage, v29, v33, 1, 1, v30, v31, nil, nil, v28);
			v1:Notify(LUAOBFUSACTOR_DECRYPT_STR_0("\69\142\239\33\75\131\163\57\70\130\163\61\66\134\250\40\92\199", "\77\46\231\131") .. v32.Name, 3);
		end);
		v10:AddButton(LUAOBFUSACTOR_DECRYPT_STR_0("\145\93\186\76\250\85\186\76", "\32\218\52\214"), function()
			local v34 = v5.AcessId:InvokeServer(v6.UserId) .. "-" .. v6.UserId;
			local v35, v36 = v6.Character:FindFirstChildOfClass(LUAOBFUSACTOR_DECRYPT_STR_0("\122\24\62\164", "\58\46\119\81\200\145\208\37"));
			if (v35 and v35:FindFirstChild(LUAOBFUSACTOR_DECRYPT_STR_0("\10\175\3\147\154\184\34\63\133\62\171\186", "\86\75\236\80\204\201\221"))) then
				v36 = require(v35.ACS_Settings);
			else
				for v92, v93 in game:GetDescendants() do
					if (v93:IsA(LUAOBFUSACTOR_DECRYPT_STR_0("\70\78\120\137", "\235\18\33\23\229\158")) and v93:FindFirstChild(LUAOBFUSACTOR_DECRYPT_STR_0("\113\153\242\132\99\191\213\175\89\180\198\168", "\219\48\218\161"))) then
						v35, v36 = v93, require(v93.ACS_Settings);
						break;
					end
				end
			end
			local v37 = {[LUAOBFUSACTOR_DECRYPT_STR_0("\233\120\114\109\218\66\225\227\116\81\70\223", "\128\132\17\28\41\187\47")]=0,[LUAOBFUSACTOR_DECRYPT_STR_0("\37\51\11\59\90\4\31\9\62", "\61\97\82\102\90")]=getgenv().Damage};
			for v77, v78 in game.Players:GetPlayers() do
				local v79 = v78.Character and v78.Character:FindFirstChild(LUAOBFUSACTOR_DECRYPT_STR_0("\132\59\166\74\201\88\23\13", "\105\204\78\203\43\167\55\126"));
				if ((v78 ~= v6) and v79) then
					task.spawn(v5.Damage.InvokeServer, v5.Damage, v35, v79, 1, 1, v36, v37, nil, nil, v34);
					v1:Notify(LUAOBFUSACTOR_DECRYPT_STR_0("\174\163\47\18\22\0\135\69\173\175\99\14\31\5\222\84\183\234", "\49\197\202\67\126\115\100\167") .. v78.Name, 3);
				end
			end
		end);
		v10:AddToggle(LUAOBFUSACTOR_DECRYPT_STR_0("\32\83\214\51\154", "\62\87\59\191\73\224\54"), {[LUAOBFUSACTOR_DECRYPT_STR_0("\211\7\226\221", "\169\135\98\154")]=LUAOBFUSACTOR_DECRYPT_STR_0("\252\127\45\78\231\115\219\206\101\50\81\239", "\168\171\23\68\52\157\83"),[LUAOBFUSACTOR_DECRYPT_STR_0("\208\116\243\172\48\33\147", "\231\148\17\149\205\69\77")]=false,[LUAOBFUSACTOR_DECRYPT_STR_0("\180\168\200\247\67\246\144", "\159\224\199\167\155\55")]=LUAOBFUSACTOR_DECRYPT_STR_0("\196\252\41\220\243\179\47\215\229\229\57\192", "\178\151\147\92")});
		Toggles.whizz:OnChanged(function()
			while Toggles.whizz.Value do
				for v84, v85 in game.Players:GetPlayers() do
					task.spawn(v5.Whizz.FireServer, v5.Whizz, v85);
				end
				task.wait();
			end
		end);
		v10:AddToggle(LUAOBFUSACTOR_DECRYPT_STR_0("\191\232\92\34\0\73\105\159\244\67\60", "\26\236\157\44\82\114\44"), {[LUAOBFUSACTOR_DECRYPT_STR_0("\30\43\205\79", "\59\74\78\181")]=LUAOBFUSACTOR_DECRYPT_STR_0("\22\196\74\74\161\32\194\73\83\188\43\145\73\95\161\51\212\72", "\211\69\177\58\58"),[LUAOBFUSACTOR_DECRYPT_STR_0("\147\224\127\244\252\199\163", "\171\215\133\25\149\137")]=false,[LUAOBFUSACTOR_DECRYPT_STR_0("\213\199\61\246\251\57\236", "\34\129\168\82\154\143\80\156")]=LUAOBFUSACTOR_DECRYPT_STR_0("\182\189\38\5\76\14\154\128\160\37\14\90", "\233\229\210\83\107\40\46")});
		Toggles.Suppression:OnChanged(function()
			while Toggles.Suppression.Value do
				for v86, v87 in game.Players:GetPlayers() do
					task.spawn(v5.Suppression.FireServer, v5.Suppression, v87, 1, math.huge, math.huge);
				end
				task.wait();
			end
		end);
		v10:AddSlider(LUAOBFUSACTOR_DECRYPT_STR_0("\210\86\32\211\11\198\86\58", "\101\161\34\82\182"), {[LUAOBFUSACTOR_DECRYPT_STR_0("\220\8\65\234", "\78\136\109\57\158\187\130\226")]=LUAOBFUSACTOR_DECRYPT_STR_0("\29\45\248\226\54\127\234\229\44\58\247\246\42\55", "\145\94\95\153"),[LUAOBFUSACTOR_DECRYPT_STR_0("\217\200\18\212\91\187\233", "\215\157\173\116\181\46")]=30,[LUAOBFUSACTOR_DECRYPT_STR_0("\24\189\133", "\186\85\212\235\146")]=0,[LUAOBFUSACTOR_DECRYPT_STR_0("\239\128\14", "\56\162\225\118\158\89\142")]=100,[LUAOBFUSACTOR_DECRYPT_STR_0("\110\10\213\161\38\209\82\2", "\184\60\101\160\207\66")]=1,[LUAOBFUSACTOR_DECRYPT_STR_0("\18\141\113\172\48\129\104", "\220\81\226\28")]=false});
		Options.strength:OnChanged(function()
			getgenv().strength = Options.strength.Value;
		end);
		v10:AddToggle(LUAOBFUSACTOR_DECRYPT_STR_0("\17\192\142\247\239\211", "\167\115\181\226\155\138"), {[LUAOBFUSACTOR_DECRYPT_STR_0("\214\39\255\72", "\166\130\66\135\60\27\17")]=LUAOBFUSACTOR_DECRYPT_STR_0("\103\88\207\102\56\4\89\203\103\38\65\88\142\115\57\86\89\218\53\61\65\94\198\122\52", "\80\36\42\174\21"),[LUAOBFUSACTOR_DECRYPT_STR_0("\106\21\49\123\91\28\35", "\26\46\112\87")]=false,[LUAOBFUSACTOR_DECRYPT_STR_0("\141\44\164\120\171\182\85", "\212\217\67\203\20\223\223\37")]=LUAOBFUSACTOR_DECRYPT_STR_0("\185\159\169\193\178\205\188\218\179\158\232\193\191\159\190\215\168\193\232\199\169\132\166\213\250\158\173\192\172\136\186\146\184\152\164\222\191\153", "\178\218\237\200")});
		Toggles.bullet:OnChanged(function()
			while Toggles.bullet.Value do
				for v88 = 1, getgenv().strength or 20 do
					v5.ServerBullet:FireServer(Vector3.new(0/0/0), Vector3.new(0/0/0));
				end
				task.wait();
			end
		end);
		v10:AddToggle(LUAOBFUSACTOR_DECRYPT_STR_0("\179\164\243\217\166", "\176\214\213\134"), {[LUAOBFUSACTOR_DECRYPT_STR_0("\192\168\174\192", "\57\148\205\214\180\200\54")]=LUAOBFUSACTOR_DECRYPT_STR_0("\49\239\52\39\126\82\238\48\38\96\23\239\117\39\115\17\242\59\48\54\31\248\33\60\121\22", "\22\114\157\85\84"),[LUAOBFUSACTOR_DECRYPT_STR_0("\224\206\21\197\72\250\188", "\200\164\171\115\164\61\150")]=false,[LUAOBFUSACTOR_DECRYPT_STR_0("\138\251\12\73\151\183\228", "\227\222\148\99\37")]=LUAOBFUSACTOR_DECRYPT_STR_0("\48\64\83\229\241\115\70\90\255\234\115\65\87\228\239\54\64\30\182\236\32\91\92\241\185\108\13\13\169\166\108", "\153\83\50\50\150")});
		Toggles.equip:OnChanged(function()
			local v40 = v6.Character:FindFirstChildOfClass(LUAOBFUSACTOR_DECRYPT_STR_0("\105\121\124\16", "\45\61\22\19\124\19\203"));
			if not v40 then
				for v94, v95 in game:GetDescendants() do
					if (v95:IsA(LUAOBFUSACTOR_DECRYPT_STR_0("\245\29\2\249", "\217\161\114\109\149\98\16")) and v95:FindFirstChild(LUAOBFUSACTOR_DECRYPT_STR_0("\51\3\11\67\143\113\6\52\49\114\187\103", "\20\114\64\88\28\220"))) then
						v40 = v95;
						break;
					end
				end
			end
			while Toggles.equip.Value do
				for v89 = 1, getgenv().strength or 20 do
					v5.Equip:FireServer(v40, 1);
				end
				task.wait();
			end
		end);
		v12:AddSlider(LUAOBFUSACTOR_DECRYPT_STR_0("\6\0\222\191\203\192\184\52\5", "\221\81\97\178\212\152\176"), {[LUAOBFUSACTOR_DECRYPT_STR_0("\249\226\5\239", "\122\173\135\125\155")]=LUAOBFUSACTOR_DECRYPT_STR_0("\170\206\18\180\62\61\136\179\192\12\178\12\33\205\129\197", "\168\228\161\96\217\95\81"),[LUAOBFUSACTOR_DECRYPT_STR_0("\255\212\40\93\58\91\207", "\55\187\177\78\60\79")]=require(v4.GameRules.Config).NormalWalkSpeed,[LUAOBFUSACTOR_DECRYPT_STR_0("\0\199\81", "\224\77\174\63\139\38\175")]=0,[LUAOBFUSACTOR_DECRYPT_STR_0("\169\64\64", "\78\228\33\56")]=500,[LUAOBFUSACTOR_DECRYPT_STR_0("\252\113\167\13\129\199\112\181", "\229\174\30\210\99")]=1,[LUAOBFUSACTOR_DECRYPT_STR_0("\56\226\139\65\236\62\45", "\89\123\141\230\49\141\93")]=false});
		Options.WalkSpeed:OnChanged(function()
			require(v4.GameRules.Config).NormalWalkSpeed = Options.WalkSpeed.Value;
		end);
		v12:AddSlider(LUAOBFUSACTOR_DECRYPT_STR_0("\193\100\248\59\17\70\248\66\230\9\21\78", "\42\147\17\150\108\112"), {[LUAOBFUSACTOR_DECRYPT_STR_0("\59\163\53\107", "\136\111\198\77\31\135")]=LUAOBFUSACTOR_DECRYPT_STR_0("\48\28\169\22\138\229\27\162\49\25\162\83\185", "\201\98\105\199\54\221\132\119"),[LUAOBFUSACTOR_DECRYPT_STR_0("\157\9\133\32\23\57\184", "\204\217\108\227\65\98\85")]=require(v4.GameRules.Config).RunWalkSpeed,[LUAOBFUSACTOR_DECRYPT_STR_0("\115\202\251", "\160\62\163\149\133\76")]=0,[LUAOBFUSACTOR_DECRYPT_STR_0("\251\161\21", "\163\182\192\109\79")]=500,[LUAOBFUSACTOR_DECRYPT_STR_0("\6\41\21\206\241\61\40\7", "\149\84\70\96\160")]=1,[LUAOBFUSACTOR_DECRYPT_STR_0("\27\9\0\253\57\5\25", "\141\88\102\109")]=false});
		Options.RunWalkSpeed:OnChanged(function()
			require(v4.GameRules.Config).RunWalkSpeed = Options.RunWalkSpeed.Value;
		end);
		v12:AddSlider(LUAOBFUSACTOR_DECRYPT_STR_0("\144\65\197\101\25\53\98\192\191\88\249\96\31\56\81", "\161\211\51\170\16\122\93\53"), {[LUAOBFUSACTOR_DECRYPT_STR_0("\207\171\170\60", "\72\155\206\210")]=LUAOBFUSACTOR_DECRYPT_STR_0("\101\104\91\27\48\78\58\99\15\63\77\73\68\11\54\66", "\83\38\26\52\110"),[LUAOBFUSACTOR_DECRYPT_STR_0("\124\18\33\71\77\27\51", "\38\56\119\71")]=require(v4.GameRules.Config).CrouchWalkSpeed,[LUAOBFUSACTOR_DECRYPT_STR_0("\222\230\86", "\54\147\143\56\182\69")]=0,[LUAOBFUSACTOR_DECRYPT_STR_0("\251\128\231", "\191\182\225\159\41")]=500,[LUAOBFUSACTOR_DECRYPT_STR_0("\25\29\61\91\143\142\204\44", "\162\75\114\72\53\235\231")]=1,[LUAOBFUSACTOR_DECRYPT_STR_0("\175\51\73\242\82\1\152", "\98\236\92\36\130\51")]=false});
		Options.CrouchWalkSpeed:OnChanged(function()
			require(v4.GameRules.Config).CrouchWalkSpeed = Options.CrouchWalkSpeed.Value;
		end);
		v12:AddSlider(LUAOBFUSACTOR_DECRYPT_STR_0("\148\11\3\180\64\159\180\60\175\10\63\170\64\173\177", "\80\196\121\108\218\37\200\213"), {[LUAOBFUSACTOR_DECRYPT_STR_0("\52\118\26\107", "\234\96\19\98\31\43\110")]=LUAOBFUSACTOR_DECRYPT_STR_0("\54\13\93\201\169\50\188\7\19\89\244\188\119\142\2", "\235\102\127\50\167\204\18"),[LUAOBFUSACTOR_DECRYPT_STR_0("\116\164\243\34\81\34\68", "\78\48\193\149\67\36")]=require(v4.GameRules.Config).ProneWalksSpeed,[LUAOBFUSACTOR_DECRYPT_STR_0("\29\23\142", "\33\80\126\224\120")]=0,[LUAOBFUSACTOR_DECRYPT_STR_0("\193\169\27", "\60\140\200\99\164")]=500,[LUAOBFUSACTOR_DECRYPT_STR_0("\181\251\17\40\166\142\250\3", "\194\231\148\100\70")]=1,[LUAOBFUSACTOR_DECRYPT_STR_0("\101\67\204\179\247\203\82", "\168\38\44\161\195\150")]=false});
		Options.ProneWalksSpeed:OnChanged(function()
			require(v4.GameRules.Config).ProneWalksSpeed = Options.ProneWalksSpeed.Value;
		end);
		v12:AddToggle(LUAOBFUSACTOR_DECRYPT_STR_0("\166\253\142\122", "\118\224\156\226\22\80\136\214"), {[LUAOBFUSACTOR_DECRYPT_STR_0("\118\235\65\148", "\224\34\142\57")]=LUAOBFUSACTOR_DECRYPT_STR_0("\248\166\201\209\51\245\92\3\223\160\192", "\110\190\199\165\189\19\145\61"),[LUAOBFUSACTOR_DECRYPT_STR_0("\254\238\113\233\158\203\206", "\167\186\139\23\136\235")]=true,[LUAOBFUSACTOR_DECRYPT_STR_0("\46\186\135\1\14\188\152", "\109\122\213\232")]=LUAOBFUSACTOR_DECRYPT_STR_0("\200\246\174\60\202\246\175\49\233\242", "\80\142\151\194")});
		Toggles.Fall:OnChanged(function()
			local v49;
			require(v4.GameRules.Config).EnableFallDamage = Toggles.Fall.Value;
			if Toggles.Fall.Value then
				v49 = LUAOBFUSACTOR_DECRYPT_STR_0("\6\200\118\78\15\195\115", "\44\99\166\23");
			else
				v49 = LUAOBFUSACTOR_DECRYPT_STR_0("\120\254\58\55\49\168\121\243", "\196\28\151\73\86\83");
			end
			v1:Notify(LUAOBFUSACTOR_DECRYPT_STR_0("\213\2\37\28\194\92\25\123\242\4\44\80\151\72\28\119\231\6\105", "\22\147\99\73\112\226\56\120") .. v49, 5);
		end);
		local v17 = {};
		for v52, v53 in next, Enum.Material:GetEnumItems() do
			table.insert(v17, v53.Name);
		end
		v11:AddDropdown(LUAOBFUSACTOR_DECRYPT_STR_0("\181\116\246\240\159\177\116\238\230", "\237\216\21\130\149"), {[LUAOBFUSACTOR_DECRYPT_STR_0("\180\79\83\74\181\218", "\62\226\46\63\63\208\169")]=v17,[LUAOBFUSACTOR_DECRYPT_STR_0("\193\28\83\130\10\1\59", "\62\133\121\53\227\127\109\79")]=1,[LUAOBFUSACTOR_DECRYPT_STR_0("\61\1\62\225\223", "\194\112\116\82\149\182\206")]=false,[LUAOBFUSACTOR_DECRYPT_STR_0("\13\173\84\12", "\110\89\200\44\120\160\130")]=LUAOBFUSACTOR_DECRYPT_STR_0("\140\214\69\6\110\75\47\72\185\202\74\74", "\45\203\163\43\38\35\42\91"),[LUAOBFUSACTOR_DECRYPT_STR_0("\230\138\211\47\147\160\68", "\52\178\229\188\67\231\201")]=LUAOBFUSACTOR_DECRYPT_STR_0("\50\68\92\1\244\72\99\44\64\68\1\229\85\34\45", "\67\65\33\48\100\151\60")});
		v11:AddDropdown(LUAOBFUSACTOR_DECRYPT_STR_0("\222\245\163\203", "\147\191\135\206\184"), {[LUAOBFUSACTOR_DECRYPT_STR_0("\178\41\170\212\221\64", "\210\228\72\198\161\184\51")]=v17,[LUAOBFUSACTOR_DECRYPT_STR_0("\18\76\245\17\102\194\34", "\174\86\41\147\112\19")]=1,[LUAOBFUSACTOR_DECRYPT_STR_0("\118\21\129\31\44", "\203\59\96\237\107\69\111\113")]=false,[LUAOBFUSACTOR_DECRYPT_STR_0("\16\19\180\245", "\183\68\118\204\129\81\144")]=LUAOBFUSACTOR_DECRYPT_STR_0("\47\191\125\247\75\175\15\185\117\246\2\131\2", "\226\110\205\16\132\107"),[LUAOBFUSACTOR_DECRYPT_STR_0("\223\204\239\213\85\226\211", "\33\139\163\128\185")]=LUAOBFUSACTOR_DECRYPT_STR_0("\68\93\8\219\84\76\68\211\86\76\1\204\94\89\8", "\190\55\56\100")});
		Options.arms:OnChanged(function()
			getgenv().armsm = Options.arms.Value;
		end);
		Options.materials:OnChanged(function()
			getgenv().gunm = Options.materials.Value;
		end);
		v11:AddLabel(LUAOBFUSACTOR_DECRYPT_STR_0("\117\160\48\17\1\163\244\67\161", "\147\54\207\92\126\115\131")):AddColorPicker(LUAOBFUSACTOR_DECRYPT_STR_0("\46\62\57\114\31\78\4\50\62\120\31", "\30\109\81\85\29\109"), {[LUAOBFUSACTOR_DECRYPT_STR_0("\219\116\82\183\35\210\232", "\156\159\17\52\214\86\190")]=Color3.new(0, 0, 0),[LUAOBFUSACTOR_DECRYPT_STR_0("\154\230\169\176\171", "\220\206\143\221")]=LUAOBFUSACTOR_DECRYPT_STR_0("\161\104\35\87\213\195\214\131\113\109\20\215\192\221\148", "\178\230\29\77\119\184\172")});
		Options.ColorPicker:OnChanged(function(v58)
			getgenv().gunc = Options.ColorPicker.Value;
		end);
		v11:AddLabel(LUAOBFUSACTOR_DECRYPT_STR_0("\214\177\6\20\101\184\244\172\7\8", "\152\149\222\106\123\23")):AddColorPicker(LUAOBFUSACTOR_DECRYPT_STR_0("\254\41\250\76\167\252\52\251\80", "\213\189\70\150\35"), {[LUAOBFUSACTOR_DECRYPT_STR_0("\107\80\114\9\90\89\96", "\104\47\53\20")]=Color3.new(0, 0, 0),[LUAOBFUSACTOR_DECRYPT_STR_0("\151\69\149\16\185", "\111\195\44\225\124\220")]=LUAOBFUSACTOR_DECRYPT_STR_0("\249\84\13\96\235\168\215\74\15\97", "\203\184\38\96\19\203")});
		Options.ColorArms:OnChanged(function(v61)
			getgenv().armsc = Options.ColorArms.Value;
		end);
		v11:AddDropdown(LUAOBFUSACTOR_DECRYPT_STR_0("\49\122\125\68", "\174\89\19\25\33"), {[LUAOBFUSACTOR_DECRYPT_STR_0("\25\19\94\91\242\148", "\107\79\114\50\46\151\231")]={LUAOBFUSACTOR_DECRYPT_STR_0("\21\163\179\61\202\24\165\205", "\160\89\198\213\73\234\89\215"),LUAOBFUSACTOR_DECRYPT_STR_0("\122\120\179\246\209\8\80\166\243", "\165\40\17\212\158")},[LUAOBFUSACTOR_DECRYPT_STR_0("\193\220\14\50\51\233\205", "\70\133\185\104\83")]=1,[LUAOBFUSACTOR_DECRYPT_STR_0("\41\80\72\62\192", "\169\100\37\36\74")]=false,[LUAOBFUSACTOR_DECRYPT_STR_0("\52\130\186\68", "\48\96\231\194")]=LUAOBFUSACTOR_DECRYPT_STR_0("\239\79\0\109\52\217\187\134\218\83\15\33", "\227\168\58\110\77\121\184\207"),[LUAOBFUSACTOR_DECRYPT_STR_0("\79\51\176\76\165\210\97", "\197\27\92\223\32\209\187\17")]=LUAOBFUSACTOR_DECRYPT_STR_0("\16\90\207\254\0\75\131\246\2\75\198\233\10\94\207", "\155\99\63\163")});
		Options.hide:OnChanged(function()
			getgenv().hide = Options.hide.Value;
		end);
		v11:AddButton(LUAOBFUSACTOR_DECRYPT_STR_0("\170\216\165\136\249\133\144\220", "\228\226\177\193\237\217"), function()
			local v66 = workspace.CurrentCamera:FindFirstChildOfClass(LUAOBFUSACTOR_DECRYPT_STR_0("\25\191\39\227\56", "\134\84\208\67"));
			if not v66 then
				return;
			end
			v66:FindFirstChild(getgenv().hide).Transparency = 1;
		end);
		v11:AddButton(LUAOBFUSACTOR_DECRYPT_STR_0("\38\188\130\93\7\169", "\60\115\204\230"), function()
			local v68 = workspace.CurrentCamera:FindFirstChildOfClass(LUAOBFUSACTOR_DECRYPT_STR_0("\202\53\239\117\235", "\16\135\90\139"));
			if not v68 then
				return;
			end
			local v69 = v68:FindFirstChildOfClass(LUAOBFUSACTOR_DECRYPT_STR_0("\121\123\2\54\66", "\24\52\20\102\83\46\52"));
			for v80, v81 in v69:GetChildren() do
				if v81:IsA(LUAOBFUSACTOR_DECRYPT_STR_0("\230\46\50\33\63\197\61\53", "\111\164\79\65\68")) then
					v81.Material = Enum.Material[getgenv().gunm];
					v81.Color = getgenv().gunc;
				end
			end
			for v82, v83 in v68:GetChildren() do
				if ((v83:IsA(LUAOBFUSACTOR_DECRYPT_STR_0("\228\216\144\219\30\235\212\205", "\138\166\185\227\190\78")) and (v83.Name == LUAOBFUSACTOR_DECRYPT_STR_0("\231\113\195\35\18\2\11\198", "\121\171\20\165\87\50\67"))) or (v83.Name == LUAOBFUSACTOR_DECRYPT_STR_0("\244\49\190\62\173\66\231\42\180", "\98\166\88\217\86\217"))) then
					v83.Material = Enum.Material[getgenv().armsm];
					v83.Color = getgenv().armsc;
				end
			end
			v1:Notify(LUAOBFUSACTOR_DECRYPT_STR_0("\192\255\106\20\135\208\182\251\118\5\149\156\227\230\125\0\146\217", "\188\150\150\25\97\230"), 3);
		end);
		v13:AddSlider(LUAOBFUSACTOR_DECRYPT_STR_0("\233\128\69\7\53", "\141\186\233\63\98\108"), {[LUAOBFUSACTOR_DECRYPT_STR_0("\197\239\52\162", "\69\145\138\76\214")]="Y",[LUAOBFUSACTOR_DECRYPT_STR_0("\84\202\143\136\170\26\100", "\118\16\175\233\233\223")]=0,[LUAOBFUSACTOR_DECRYPT_STR_0("\166\141\59", "\29\235\228\85\219\142\235")]=0,[LUAOBFUSACTOR_DECRYPT_STR_0("\16\213\162", "\50\93\180\218\189\23\46\71")]=2048,[LUAOBFUSACTOR_DECRYPT_STR_0("\236\171\78\66\64\213\70\217", "\40\190\196\59\44\36\188")]=1,[LUAOBFUSACTOR_DECRYPT_STR_0("\31\74\209\164\251\126\25", "\109\92\37\188\212\154\29")]=false});
		v13:AddSlider(LUAOBFUSACTOR_DECRYPT_STR_0("\55\230\190\198\9", "\58\100\143\196\163\81"), {[LUAOBFUSACTOR_DECRYPT_STR_0("\46\71\59\183", "\110\122\34\67\195\95\41\133")]="X",[LUAOBFUSACTOR_DECRYPT_STR_0("\81\180\93\75\195\121\165", "\182\21\209\59\42")]=0,[LUAOBFUSACTOR_DECRYPT_STR_0("\154\94\203", "\222\215\55\165\125\65")]=0,[LUAOBFUSACTOR_DECRYPT_STR_0("\1\208\222", "\42\76\177\166\122\146\161\141")]=2048,[LUAOBFUSACTOR_DECRYPT_STR_0("\151\133\16\192\125\127\171\141", "\22\197\234\101\174\25")]=1,[LUAOBFUSACTOR_DECRYPT_STR_0("\14\59\168\204\119\172\195", "\230\77\84\197\188\22\207\183")]=false});
		v13:AddSlider(LUAOBFUSACTOR_DECRYPT_STR_0("\202\29\220\249\182", "\85\153\116\166\156\236\193\144"), {[LUAOBFUSACTOR_DECRYPT_STR_0("\144\229\85\167", "\96\196\128\45\211\132")]="Z",[LUAOBFUSACTOR_DECRYPT_STR_0("\17\136\125\94\199\163\160", "\184\85\237\27\63\178\207\212")]=0,[LUAOBFUSACTOR_DECRYPT_STR_0("\37\80\7", "\63\104\57\105")]=0,[LUAOBFUSACTOR_DECRYPT_STR_0("\38\134\188", "\36\107\231\196")]=2048,[LUAOBFUSACTOR_DECRYPT_STR_0("\111\186\183\137\89\188\172\128", "\231\61\213\194")]=1,[LUAOBFUSACTOR_DECRYPT_STR_0("\42\162\48\99\8\174\41", "\19\105\205\93")]=false});
		v13:AddButton(LUAOBFUSACTOR_DECRYPT_STR_0("\139\17\206\128\44\186\72\202\136\50\172\72\220\148\54\165\12", "\95\201\104\190\225"), function()
			local v70 = v6.Character.ACS_Client.Kit.Fortifications;
			if (v70.Value > 10000) then
				v1:Notify(LUAOBFUSACTOR_DECRYPT_STR_0("\182\196\212\142\174\199\211\203\174\207\216\142\191\206\211\200\160\217\204\203\171\139\213\198\170\139\195\215\191\202\210\221", "\174\207\171\161"), 3);
				return;
			end
			v5.Refil:FireServer(v70, -100000);
			v1:Notify(LUAOBFUSACTOR_DECRYPT_STR_0("\254\235\14\240\253\196\254", "\183\141\158\109\147\152"), 3);
		end);
		v13:AddButton(LUAOBFUSACTOR_DECRYPT_STR_0("\14\28\239\0\40", "\108\76\105\134"), function()
			task.spawn(v5.Breach.InvokeServer, v5.Breach, 3, {[LUAOBFUSACTOR_DECRYPT_STR_0("\205\202\163\245\199\237\204\180\229", "\174\139\165\209\129")]={},[LUAOBFUSACTOR_DECRYPT_STR_0("\135\182\241\213\212\12\105\121\161\191\231", "\24\195\211\130\161\166\99\16")]=workspace}, CFrame.new(), CFrame.new(), {[LUAOBFUSACTOR_DECRYPT_STR_0("\101\37\251\45\94\19", "\118\38\99\137\76\51")]=(v7.HumanoidRootPart.CFrame or (v7:GetPivot().p * CFrame.new(0, 0, 0))),[LUAOBFUSACTOR_DECRYPT_STR_0("\206\47\31\23", "\64\157\70\101\114\105")]={Y=Options.SizeY.Value,X=Options.SizeX.Value,Z=Options.SizeZ.Value}});
			v1:Notify(LUAOBFUSACTOR_DECRYPT_STR_0("\105\166\180\247\17\78\171\162\163\19\82\173\166\247\21", "\112\32\200\199\131"), 3);
		end);
		v1:OnUnload(function()
			v1.Unloaded = true;
		end);
		local v18 = v9[LUAOBFUSACTOR_DECRYPT_STR_0("\25\121\28\139\198\191\54\37\94\91\171", "\66\76\48\60\216\163\203")]:AddLeftGroupbox(LUAOBFUSACTOR_DECRYPT_STR_0("\151\131\119\230", "\68\218\230\25\147\63\174"));
		v18:AddButton(LUAOBFUSACTOR_DECRYPT_STR_0("\152\36\95\67\183\169", "\214\205\74\51\44"), function()
			v1:Unload();
		end);
		v18:AddLabel(LUAOBFUSACTOR_DECRYPT_STR_0("\215\73\236\233\55\248\69\236\248", "\23\154\44\130\156")):AddKeyPicker(LUAOBFUSACTOR_DECRYPT_STR_0("\60\163\163\187\29\22\8\164\164\160\50", "\115\113\198\205\206\86"), {[LUAOBFUSACTOR_DECRYPT_STR_0("\160\82\248\91\145\91\234", "\58\228\55\158")]=LUAOBFUSACTOR_DECRYPT_STR_0("\157\135\195\43\46\185", "\85\212\233\176\78\92\205"),[LUAOBFUSACTOR_DECRYPT_STR_0("\100\87\189\203", "\130\42\56\232")]=true,[LUAOBFUSACTOR_DECRYPT_STR_0("\222\176\60\247", "\95\138\213\68\131\32")]=LUAOBFUSACTOR_DECRYPT_STR_0("\7\45\175\86\54\33\45\184\65\127\36\44", "\22\74\72\193\35")});
		v2:SetLibrary(v1);
		v3:SetLibrary(v1);
		v3:IgnoreThemeSettings();
		v2:SetFolder(LUAOBFUSACTOR_DECRYPT_STR_0("\13\90\215", "\56\76\25\132"));
		v3:SetFolder("ACS/specific-game");
		v3:BuildConfigSection(v9["UI Settings"]);
		v2:ApplyToTab(v9["UI Settings"]);
	end 
})
TrollTab:AddButton({
	Name = "Tacar som - Risco",
	Callback = function()
		--// AC6_Sound and Lights_FE, AC6_Sound faz voce colocar som no jogo, Lights_FE faz voce pintar o mapa e mudar a transparencia da part
		local lib =  loadstring(game:HttpGetAsync("https://raw.githubusercontent.com/Consistt/Ui/main/UnLeaked"))()
		local sound
		local pith
		local volume

		lib.title = "Main"

		local Main = lib:Init()
		local tab1 = Main:NewTab("FE Sound")
		local Section1 = tab1:NewSection("Main")

		tab1:NewTextbox("Sound Id","", "xxx", "all", "small", true, false, function(id)
			sound = 'rbxassetid://'..id
		end)

		tab1:NewSlider("Pith", "",true,"/",{min = 0, max = 10, default = 0}, function(max)
			pith = max
		end)

		tab1:NewSlider("Volume", "",true,"/",{min = 0, max = 10, default = 0}, function(Volume)
			volume = Volume
		end)

		local NAME = "ZEUS FPS"

		tab1:NewToggle("Play", false ,function(play)
			local rmt = game:FindFirstChild("AC6_FE_Sounds", true)
			rmt:FireServer('newSound', NAME, workspace, sound, pith, volume, true)
			rmt:FireServer('playSound', NAME)
			if not play then
				rmt:FireServer("stopSound", NAME)
			end
		end)

		local tab2 = Main:NewTab("Lights FE")
		local Section2 = tab2:NewSection("Main")

		local material
		local transparency
		local color

		tab2:NewTextbox("Material","", "xxx", "all", "small", true, false, function(mat)
			material = mat
		end)

		tab2:NewTextbox("Color", "", "xxx", "all", "small", true, false, function(cor)
			color = BrickColor.new(cor)
		end)

		tab2:NewSlider("Transparency","",true,"/",{min = 0, max = 1, default = 0}, function(t)
			transparency = t
		end)

		tab2:NewButton("Pintar", function()
			local remote = game:FindFirstChild("Lights_FE", true)
			for i, v in next, game:GetDescendants() do
				if v:IsA("BasePart") then
					remote:FireServer('UpdateLight', v, material, color, transparency)
				end
			end
		end)
	end  
})
TrollTab:AddButton({
	Name = "Spamar mensagem (Celular) Roleplay brasil Season 1",
	Callback = function()
		local remotao = game:GetService("ReplicatedStorage"):WaitForChild("Remotes"):WaitForChild("EnviarMenssagem")
		local players = game:GetService("Players"):GetPlayers() -- vc pode mudar aq se quiser so pra 1 player em especifico

		local message = {
			["Conteudo"] = "Servidor invadido pelo Pedroxz Menu", -- a msg 
			["Origem"] = "Pedroxz Menu e o hypeee" -- aq e o nome de qm enviou a msg
		}

		local quantidade = 30 -- quantas vezes vc quer enviar a msg?!!?! (pra todos)

		for rep = 1, quantidade do
			for _, player in ipairs(players) do
				local args = {
					[1] = player.Name, 
					[2] = message
				}
				remotao:FireServer(unpack(args))
			end
			wait(5) -- recomendo aumentar pq se nao tem risco de kick
		end
	end  
})
TrollTab:AddButton({
	Name = "Matar geral - Português Troca de Tiros RJ (Arma)",
	Callback = function()
		local player = game.Players.LocalPlayer

		local storage = game.ReplicatedStorage.ACS_Engine.Events
		local damage, id = storage.Damage, storage.AcessId:InvokeServer(player.UserId).."-"..player.UserId

		local tool, data = player.Character:FindFirstChildOfClass("Tool")

		shared.a = not shared.a

		if tool and tool:FindFirstChild("ACS_Settings") then
			data = require(tool.ACS_Settings)
		else
			for i,v in player.Backpack:GetChildren() do
				if v:IsA("Tool") and v:FindFirstChild("ACS_Settings") then
					v.Parent = player.Character
					tool, data = v, require(v.ACS_Settings)
					break
				end
			end
		end

		local modtable = {
			DamageMod = math.huge,
			minDamageMod = 0,
		}

		while shared.a and tool do
			for i,v in game.Players:GetPlayers() do
				local hum = v.Character and v.Character:FindFirstChild("Humanoid")
				if v ~= player and hum and hum.Health > 0 then
					damage:InvokeServer(
						"ACS_Frameworkk", 
						"criasmastre",
						tool,
						hum,
						2,
						2,
						data,
						modtable,
						nil,
						nil,
						id
					)
				end
			end
			task.wait()
		end
	end 

}) 
local Section = RoleplayTab:AddSection({
	Name = "RP"
})
RoleplayTab:AddButton({
	Name = "Deletar Roupa Geral",
	Callback = function()
		local rmt = game:service'ReplicatedStorage':FindFirstChild("DeleteCar")
		for i,v in pairs(game:GetService("Workspace"):GetDescendants()) do
			if  v:IsA("Shirt") or v:IsA("Pants")  then
				rmt:FireServer(v) 
			end
		end
	end   
})
RoleplayTab:AddButton({
	Name = "Deletar Mapa",
	Callback = function()
		local rmt = game:service'ReplicatedStorage':FindFirstChild("DeleteCar")
		for i,v in next, workspace:GetChildren() do
			rmt:FireServer(v)
		end
	end   
})
RoleplayTab:AddButton({
	Name = "Creeper Geral",
	Callback = function()
		local rmt = game:service'ReplicatedStorage':FindFirstChild("DeleteCar")
		for i,v in pairs(game:GetService("Workspace"):GetDescendants()) do
			if v:IsA("SpecialMesh") or v:IsA("Shirt") or v:IsA("Pants") or v:IsA("Part") and v.Name == "Right Arm" or v.Name == "Left Arm" then
				rmt:FireServer(v) 
			end
		end
	end   
}) 
RoleplayTab:AddButton({
	Name = "Explodir Geral",
	Callback = function()
		local rem,_t,players = game:GetService("ReplicatedStorage").ACS_Engine.Eventos.Hit,{ExplosiveHit=true,ExPressure=math.huge,ExpRadius=math.huge,DestroyJointRadiusPercent=math.huge,ExplosionDamage=math.huge},game:GetService('Players')

		for i,v in next, players:GetPlayers() do 
			local ppart = v['Character'].PrimaryPart
			pcall(function()
				rem:FireServer(ppart.Position,ppart,ppart.Position,Enum.Material.ForceField,_t)
			end)
		end
	end 
})
RoleplayTab:AddButton({
	Name = "Tool Destruir",
	Callback = function()
		local Mouse = game.Players.LocalPlayer:GetMouse()

		local Tool = Instance.new('Tool',game.Players.LocalPlayer.Backpack)
		Tool.CanBeDropped = false
		Tool.Name = "Destruir"
		Tool.RequiresHandle = false 

		local rmt = game:GetService("ReplicatedStorage").DeleteCar

		Tool.Activated:connect(function() 
			rmt:FireServer(Mouse.Target)
		end)
	end    
})
local Section = AdmTab:AddSection({
	Name = "Admin"
})
local Section = RoleplayTab:AddSection({
	Name = "Option Banir/Expulsar"
})
RoleplayTab:AddButton({
	Name = "Banir Jogadores",
	Callback = function()
		game.StarterGui:SetCore("SendNotification", {
			Title = "Metodo pra banir Geral!?"; -- the title 
			Text = "Procure um anti cheat ou anti bug e faca um script que da pro jogador interagir pra banir."; -- what the text says 
			Duration = 15; -- how long the notification should in secounds
		})
	end      
})
RoleplayTab:AddButton({
	Name = "Expulsar Jogares",
	Callback = function()
		game.StarterGui:SetCore("SendNotification", {
			Title = "Metodo pra expulsar Geral!?"; -- the title 
			Text = "Procure por um bug ou uma falha no server que expulsa o dar ban e crie um script disso pra que a pessoa interagir."; -- what the text says 
			Duration = 15; -- how long the notification should in secounds
		})
	end      
})
AdmTab:AddButton({
	Name = "Voar (Ingual ADM) - Risco",
	Callback = function()
		-- Made By zack;#6969

		-- Instances:

		local FlyScript = Instance.new("ScreenGui")
		local Gradient = Instance.new("Frame")
		local UIGradient = Instance.new("UIGradient")
		local UICorner = Instance.new("UICorner")
		local Button = Instance.new("TextButton")
		local Shadow = Instance.new("Frame")
		local TextLabel = Instance.new("TextLabel")

		--Properties:

		FlyScript.Name = "FlyScript"
		FlyScript.Parent = game.Players.LocalPlayer:WaitForChild("PlayerGui")
		FlyScript.ResetOnSpawn = false

		Gradient.Name = "Gradient"
		Gradient.Parent = FlyScript
		Gradient.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
		Gradient.BorderColor3 = Color3.fromRGB(27, 42, 53)
		Gradient.BorderSizePixel = 0
		Gradient.Position = UDim2.new(0.0199062824, 0, 0.781767964, 0)
		Gradient.Size = UDim2.new(0, 231, 0, 81)

		UIGradient.Color = ColorSequence.new{ColorSequenceKeypoint.new(0, Color3.fromRGB(57, 104, 252)), ColorSequenceKeypoint.new(1, Color3.fromRGB(51, 68, 175))}
		UIGradient.Parent = Gradient

		UICorner.CornerRadius = UDim.new(0.0399999991, 0)
		UICorner.Parent = Gradient

		Button.Name = "Button"
		Button.Parent = Gradient
		Button.BackgroundColor3 = Color3.fromRGB(77, 100, 150)
		Button.BorderSizePixel = 0
		Button.Position = UDim2.new(0.0921155736, 0, 0.238353431, 0)
		Button.Size = UDim2.new(0, 187, 0, 41)
		Button.ZIndex = 2
		Button.Font = Enum.Font.GothamSemibold
		Button.Text = ""
		Button.TextColor3 = Color3.fromRGB(255, 255, 255)
		Button.TextScaled = true
		Button.TextSize = 14
		Button.TextWrapped = true

		Shadow.Name = "Shadow"
		Shadow.Parent = Button
		Shadow.BackgroundColor3 = Color3.fromRGB(53, 69, 103)
		Shadow.BorderSizePixel = 0
		Shadow.Size = UDim2.new(1, 0, 1, 4)

		TextLabel.Parent = Gradient
		TextLabel.AnchorPoint = Vector2.new(0.5, 0.5)
		TextLabel.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
		TextLabel.BackgroundTransparency = 1
		TextLabel.BorderColor3 = Color3.fromRGB(27, 42, 53)
		TextLabel.BorderSizePixel = 0
		TextLabel.Position = UDim2.new(0.487012982, 0, 0.5, 0)
		TextLabel.Size = UDim2.new(0.878787875, -20, 0.728395045, -20)
		TextLabel.ZIndex = 2
		TextLabel.Font = Enum.Font.GothamBold
		TextLabel.Text = "Fly"
		TextLabel.TextColor3 = Color3.fromRGB(255, 255, 255)
		TextLabel.TextScaled = true
		TextLabel.TextSize = 14
		TextLabel.TextWrapped = true
		Button.MouseButton1Down:connect(function()
			repeat wait()
			until game.Players.LocalPlayer and game.Players.LocalPlayer.Character and game.Players.LocalPlayer.Character:findFirstChild("Torso") and game.Players.LocalPlayer.Character:findFirstChild("Humanoid")
			local mouse = game.Players.LocalPlayer:GetMouse()
			repeat wait() until mouse
			local plr = game.Players.LocalPlayer
			local torso = plr.Character.Torso
			local flying = true
			local deb = true
			local ctrl = {f = 0, b = 0, l = 0, r = 0}
			local lastctrl = {f = 0, b = 0, l = 0, r = 0}
			local maxspeed = 50
			local speed = 0

			function Fly()
				local bg = Instance.new("BodyGyro", torso)
				bg.P = 90000
				bg.maxTorque = Vector3.new(9000000000, 9000000000, 9000000000)
				bg.cframe = torso.CFrame
				local bv = Instance.new("BodyVelocity", torso)
				bv.velocity = Vector3.new(0,0.1,0)
				bv.maxForce = Vector3.new(9000000000, 9000000000, 9000000000)
				repeat wait()
					plr.Character.Humanoid.PlatformStand = true
					if ctrl.l + ctrl.r ~= 0 or ctrl.f + ctrl.b ~= 0 then
						speed = speed+0.5+(speed/maxspeed)
						if speed > maxspeed then
							speed = maxspeed
						end
					elseif not (ctrl.l + ctrl.r ~= 0 or ctrl.f + ctrl.b ~= 0) and speed ~= 0 then
						speed = speed-1
						if speed < 0 then
							speed = 0
						end
					end
					if (ctrl.l + ctrl.r) ~= 0 or (ctrl.f + ctrl.b) ~= 0 then
						bv.velocity = ((game.Workspace.CurrentCamera.CoordinateFrame.lookVector * (ctrl.f+ctrl.b)) + ((game.Workspace.CurrentCamera.CoordinateFrame * CFrame.new(ctrl.l+ctrl.r,(ctrl.f+ctrl.b)*0.2,0).p) - game.Workspace.CurrentCamera.CoordinateFrame.p))*speed
						lastctrl = {f = ctrl.f, b = ctrl.b, l = ctrl.l, r = ctrl.r}
					elseif (ctrl.l + ctrl.r) == 0 and (ctrl.f + ctrl.b) == 0 and speed ~= 0 then
						bv.velocity = ((game.Workspace.CurrentCamera.CoordinateFrame.lookVector * (lastctrl.f+lastctrl.b)) + ((game.Workspace.CurrentCamera.CoordinateFrame * CFrame.new(lastctrl.l+lastctrl.r,(lastctrl.f+lastctrl.b)*0.2,0).p) - game.Workspace.CurrentCamera.CoordinateFrame.p))*speed
					else
						bv.velocity = Vector3.new(0,0.1,0)
					end
					bg.cframe = game.Workspace.CurrentCamera.CoordinateFrame * CFrame.Angles(-math.rad((ctrl.f+ctrl.b)*50*speed/maxspeed),0,0)
				until not flying
				ctrl = {f = 0, b = 0, l = 0, r = 0}
				lastctrl = {f = 0, b = 0, l = 0, r = 0}
				speed = 0
				bg:Destroy()
				bv:Destroy()
				plr.Character.Humanoid.PlatformStand = false
			end
			mouse.KeyDown:connect(function(key)
				if key:lower() == "e" then
					if flying then flying = false
					else
						flying = true
						Fly()
					end
				elseif key:lower() == "w" then
					ctrl.f = 1
				elseif key:lower() == "s" then
					ctrl.b = -1
				elseif key:lower() == "a" then
					ctrl.l = -1
				elseif key:lower() == "d" then
					ctrl.r = 1
				end
			end)
			mouse.KeyUp:connect(function(key)
				if key:lower() == "w" then
					ctrl.f = 0
				elseif key:lower() == "s" then
					ctrl.b = 0
				elseif key:lower() == "a" then
					ctrl.l = 0
				elseif key:lower() == "d" then
					ctrl.r = 0
				end
			end)
			Fly()

		end)
		-- Scripts:

		local function LHMZZV_fake_script() -- FlyScript.Script 
			local script = Instance.new('Script', FlyScript)

			frame = script.Parent.Gradient -- Take out {}s, and put name of frame
			frame.Draggable = true
			frame.Active = true
			frame.Selectable = true
		end
		coroutine.wrap(LHMZZV_fake_script)()
	end           
})       
TrollTab:AddButton({
	Name = "Btools - Clique apagar",
	Callback = function()
		-- Made by ILoveCats9030
		-- Version: 1.3
		-- Instances:

		local ScreenGui = Instance.new("ScreenGui")
		local main = Instance.new("Frame")
		local Text = Instance.new("TextLabel")
		local BT = Instance.new("TextButton")

		--Properties:

		ScreenGui.Parent = game.CoreGui

		main.Name = "main"
		main.Parent = ScreenGui
		main.BackgroundColor3 = Color3.fromRGB(62, 62, 62)
		main.BorderColor3 = Color3.fromRGB(0, 0, 0)
		main.BorderSizePixel = 5
		main.Position = UDim2.new(0.0198598132, 0, 0.687250972, 0)
		main.Size = UDim2.new(0, 207, 0, 146)
		main.Active = true

		Text.Name = "Text"
		Text.Parent = ScreenGui
		Text.BackgroundColor3 = Color3.fromRGB(157, 157, 157)
		Text.Position = UDim2.new(0.0292056073, 0, 0.699203134, 0)
		Text.Size = UDim2.new(0, 190, 0, 34)
		Text.Font = Enum.Font.SciFi
		Text.Text = "Btools script"
		Text.TextColor3 = Color3.fromRGB(0, 0, 0)
		Text.TextSize = 14

		BT.Name = "BT"
		BT.Parent = ScreenGui
		BT.BackgroundColor3 = Color3.fromRGB(255, 255, 255)
		BT.Position = UDim2.new(0.0443925261, 0, 0.860557795, 0)
		BT.Size = UDim2.new(0, 164, 0, 40)
		BT.Style = Enum.ButtonStyle.RobloxRoundDefaultButton
		BT.Font = Enum.Font.Highway
		BT.Text = "Btools"
		BT.TextColor3 = Color3.fromRGB(0, 0, 0)
		BT.TextScaled = true
		BT.TextSize = 14
		BT.TextWrapped = true
		BT.MouseButton1Down:connect(function()
			local tool1 = Instance.new("HopperBin",game.Players.LocalPlayer.Backpack)
			local tool2 = Instance.new("HopperBin",game.Players.LocalPlayer.Backpack)
			local tool3 = Instance.new("HopperBin",game.Players.LocalPlayer.Backpack)
			local tool4 = Instance.new("HopperBin",game.Players.LocalPlayer.Backpack)
			local tool5 = Instance.new("HopperBin",game.Players.LocalPlayer.Backpack)
			tool1.BinType = "Clone"
			tool2.BinType = "GameTool"
			tool3.BinType = "Hammer"
			tool4.BinType = "Script"
			tool5.BinType = "Grab"
		end)
	end           
}) 
JogadorTab:AddSlider({
	Name = "Velocidade",
	Min = 16,
	Max = 500,
	Default = 16,
	Color = Color3.fromRGB(255,255,255),
	Increment = 1,
	ValueName = "Speed",
	Callback = function(Value)
		game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = Value
	end    
})    
JogadorTab:AddSlider({
	Name = "Pulo",
	Min = 16,
	Max = 500,
	Default = 16,
	Color = Color3.fromRGB(255,255,255),
	Increment = 1,
	ValueName = "Jump",
	Callback = function(Value)
		game.Players.LocalPlayer.Character.Humanoid.JumpPower = Value               
	end
})        
local Section = HubTab:AddSection({
	Name = "Hub Trolls"
})
HubTab:AddButton({
	Name = "Temple Hook (Funciona em algums rp/eb)",
	Callback = function()
		loadstring(game:HttpGet("https://bifao.tech/templehook/loader.lua",true))()
	end                 
})
HubTab:AddButton({
	Name = "Explode (HUB) - Risco kick",
	Callback = function()
		_G.AutoEquip = true --se vc for usar arma de gamepass deixa isso como false
		loadstring(game:HttpGet(("https://raw.githubusercontent.com/GameLeaks2/RobloxScripts/main/KILL%20ALL"),true))()
	end        
})
HubTab:AddButton({
	Name = "Regime militar - Simulador militar (Gun)",
	Callback = function()
		loadstring(game:HttpGet'https://raw.githubusercontent.com/Pedroxz63/killall/main/README.md')()
	end    
})
HubTab:AddButton({
	Name = "Executor server-sided - Regime militar (Gun)",
	Callback = function()
		loadstring(game:HttpGet'https://raw.githubusercontent.com/KazuinExilado/scripts/main/regimemilitar.lua')()
	end                   
})
local Section = JogadorTab:AddSection({
	Name = "Jogador"
})
JogadorTab:AddButton({
	Name = "God Mode",
	Callback = function()
		local Player = game.Players.LocalPlayer
		local Character = Player.Character
		local Humanoid = Character.Humanoid

		print('Godmode working.')

		Humanoid.MaxHealth = 999999
		Humanoid.Health = Humanoid.MaxHealth / 2

		Humanoid.HealthChanged:connect(function()
			if Humanoid.Health < 10 then
				Humanoid.Health = Humanoid.MaxHealth
			end
		end)
	end    
})
JogadorTab:AddButton({
	Name = "Infinite Stamina",
	Callback = function()
		local function SetInfiniteStamina(player)
			local humanoid = player.Character and player.Character:FindFirstChild("Humanoid")
			if humanoid then
				humanoid.MaxHealth = math.huge
				humanoid.Health = math.huge
			end
		end

		-- Conectar a função ao evento de entrada do jogador
		game.Players.PlayerAdded:Connect(function(player)
			player.CharacterAdded:Connect(function()
				SetInfiniteStamina(player)
			end)
		end)
	end    
})
JogadorTab:AddButton({
	Name = "Auto JJs",
	Callback = function()
		local Options = {
			Keybind = '0', --> Keybind para mostrar/esconder a UI, mais informações sobre KeyCode: https://create.roblox.com/docs/reference/engine/enums/KeyCode
			Language = 'pt-br', --> Alterar a linguagem dos textos, disponívels: pt-br, en-us
			Rainbow = true, --> Deixar a UI mais colorida (true/false)
		};
		loadstring(game:HttpGet('https://raw.githubusercontent.com/Zv-yz/AutoJJs/main/Main.lua'))(Options);

	end  
}) 
JogadorTab:AddButton({
	Name = "Kill All Acs - Precisa de arma",
	Callback = function()
		--while wait() do
		local DR = game:GetService("ReplicatedStorage")["ACS_Engine"].Eventos.Damage

		for PlayerIndex,GivenPlayer in pairs(game.Players:GetPlayers()) do
			local Char = GivenPlayer.Character
			DR:FireServer(Char.Humanoid,Char.Humanoid.MaxHealth,0,0)
		end
	end    
})          
ArmaTab:AddButton({
	Name = "Aimbot Bypass",
	Callback = function()
		loadstring(game:HttpGet(('https://raw.githubusercontent.com/Exunys/Aimbot-V2/main/Resources/Scripts/Main.lua'),true))()

	end                           
})
ArmaTab:AddButton({
	Name = "Bala Explosiva",
	Callback = function()
		for i,v in pairs(game:GetService("Players").LocalPlayer.Backpack:GetDescendants()) do
			if v:IsA("ModuleScript") and v.Name == "Settings" then
				local a = require(v)	
				a.ExplosiveHit = true
				a.Expradius = 50
			end
		end
	end    
})
local Section = MenusTab:AddSection({
	Name = "Menus"
})
MenusTab:AddButton({
	Name = "Felipe Menu (Risco Kick/Ban)",
	Callback = function()
		loadstring(game:HttpGet('https://raw.githubusercontent.com/DebugCrazY/FMobfuscated/main/fm.lua'))()
	end    
})
MenusTab:AddButton({
	Name = "Felipe Menu (Cidade alta)",
	Callback = function()
		_, Protected_by_MoonSecV2, Discord = 'discord.gg/gQEH2uZxUk'


		,nil,nil;(function() _msec=(function(e,l,o)local W=l["㒢㒥㒛㒣㒤㒝㒛㒡㒗㒠"];local R=o[e[(666+-#{1,{};82;82,'nil'})]][e["㒜㒡㒜㒗㒟㒞㒙㒢㒝㒙㒟㒚㒥㒗㒞㒡㒡㒞"]];local p=(73+-69)/(20/(1440/(407-263)))local S=(((9049600/128)/175)/202)-(4/4)local v=o[e[(426-((571-297)+-#'keno 0347 is a nerdy fag'))]][e["㒙㒘㒣㒙㒣㒢㒙㒡㒜㒣㒛㒙㒢"]];local m=(-#'how to join the kkk'+((-#"free bobux no skem"+(1892+(((21+-26)+-#[[papier ist ein kleiner schwanz lutscher]])-30)))/90))+(38-36)local C=o[e[((1201+-46)-611)]][e["㒜㒝㒠㒞㒚㒜㒗㒥㒟㒤㒗㒥㒛㒗㒘㒜㒝"]]local d=((2310/165)+-#'deadphonelua')-((61+((-#'elbicho'+(-1860/186))+-23))+-#'Cock and ball tortue')local r=(5+-#{(function()return#{('fhKPKl'):find("\75")}>0 and 1 or 0 end),11,(function()return#{('fhKPKl'):find("\75")}>0 and 1 or 0 end)})local x=(70/((-#'monkey mode'+((19698/42)-263))-160))local w=(120-(((565-(-87+428))+-#'If LocalPlayer equals Dumbass then while true do end')+-54))local i=((88+-#{(function()return{','}end)();24,(function()return#{('bmHfML'):find("\72")}>0 and 1 or 0 end);24;",",87;'}'})-79)local b=(-95+(-116+(217+-#{'nil',(function()return{','}end)(),24;24})))local O=(((58+-#{(function()return{','}end)(),1,'nil';'nil';59})-46)+-#[[Negro]])local k=(80-(-43+(-#"Deezbutts"+(187+(-#'this is a meme string'+(-962/26))))))local U=((-#{'}',",",61;(function()return{','}end)()}+54)-47)local h=((-#"anime is for fags"+(56-((9579/(110+-#{1,1,{},",",'nil';'nil',(function()return#{('FhbPbH'):find("\98")}>0 and 1 or 0 end)}))+-#[[W4rboy was here]])))+42)local u=(432/(29376/(((-#'Impulse real 2022'+(-4118/71))+301)+-#'windows xp startup sfx')))local c=(129+(-80+(((-2969+1473)/44)+-#"Lana Rhoades")))local t=(((-11-((-112+(36322/11))/110))+-#'cilerteddoesntlikeburgers')+68)local B=(((336-(-#'cilerteddoesntlikeburgers'+(15870/(-#"send nudes"+(187-(7020/65))))))+-#[[bigchungus]])-117)local P=(((2029-((-#{23,1,23;23,(function()return#{('Lkmpfb'):find("\109")}>0 and 1 or 0 end)}+257009)/242))+-#"elbicho")/240)local N=((((-109+1)+241)-83)-46)local M=(112-((-85+(26984+-#{'}',1;1,(function()return#{('FFFMLl'):find("\70")}>0 and 1 or 0 end),",",'}',(function()return{','}end)()}))/249))local D=(((938+(((-118+-10130)/168)+-13))+-#"never gonna give you up never gonna let you down")/204)local _=((((-#{(function()return{','}end)();(function()return#{('pKKfLP'):find("\75")}>0 and 1 or 0 end),'nil','}',44,'nil';1}+341)+-97)-181)-52)local j=e[(-#{'nil','}',(function()return{','}end)();68;105,68,","}+1395)];local G=o[e[(183+-#{",";'}',(function()return{','}end)();(function()return#{('HBhHMB'):find("\104")}>0 and 1 or 0 end),82,(function()return#{('HBhHMB'):find("\104")}>0 and 1 or 0 end);'}'})]][e["㒟㒡㒟㒣㒣㒣㒠㒤㒛㒤㒦㒙㒡㒘"]];local L=o[(function(e)return type(e):sub(1,1)..'\101\116'end)('㒛㒚㒤㒦㒦㒝㒠㒞')..'\109\101'..('\116\97'or'㒟㒗㒠㒥㒘㒢㒚㒡')..e[(1112-568)]];local F=o[e[(-45+589)]][e["㒣㒜㒟㒡㒚㒘㒤㒛"]];local A=(7+-#{(function()return#{('pKOflb'):find("\79")}>0 and 1 or 0 end),'nil','nil';59;'nil'})-(-#"0nly 1337"+(((420-250)+-118)+-41))local y=(42/(-#[[nicowashere]]+(((13989-7003)+-#'bigchungus')/218)))-(270/135)local I=o[e[(-#'atakahan der nigga'+(312+-120))]][e["㒝㒣㒝㒢㒠㒙㒡㒚"]];local a=function(e,o)return e..o end local z=(388/97)*(77-((16000/((6900800/227)/190))+-#[[if syn then haxor alert end]]))local K=o[e["㒡㒞㒥㒟㒙㒠㒠㒢㒜㒘㒤㒙㒛㒣㒚"]];local f=(44+-42)*((-24+((-735/105)+-#'W4rboy was here'))+174)local H=((2180-1141)+-#[[W4rboy was here]])*(((-#"0nly segc"+((346797/93)+-93))/117)+-#"Fucking losed 027728272728271")local V=((-54+(36844/151))-138)local g=((((4641/119)+-#"cilerteddoesntlikeburgers")-47)+35)*(-#"bigchungus"+(51-39))local s=o[e["㒝㒛㒠㒥㒠㒝㒠㒙㒟㒣㒛㒞㒥㒝㒗㒗㒠㒥㒛"]]or o[e[(68000/125)]][e["㒝㒛㒠㒥㒠㒝㒠㒙㒟㒣㒛㒞㒥㒝㒗㒗㒠㒥㒛"]];local n=((((-49+213061)-106516)/52)/8)local e=o[e["㒤㒗㒝㒗㒦㒝㒞㒢㒣㒚㒣㒤"]];local Y=(function(a)local r,l=3,16 local o={j={},v={}}local n=-d local e=l+S while true do o[a:sub(e,(function()e=r+e return e-S end)())]=(function()n=n+d return n end)()if n==(z-d)then n=""l=A break end end local n=#a while e<n+S do o.v[l]=a:sub(e,(function()e=r+e return e-S end)())l=l+d if l%p==A then l=y F(o.j,(I((o[o.v[y]]*z)+o[o.v[d]])))end end return C(o.j)end)("..:::MoonSec::..㒗㒘㒙㒚㒛㒜㒝㒞㒟㒠㒡㒢㒣㒤㒥㒦㒢㒛㒡㒙㒠㒥㒠㒡㒠㒞㒠㒙㒟㒥㒟㒡㒟㒝㒟㒙㒞㒥㒞㒡㒞㒣㒞㒙㒝㒥㒝㒡㒥㒛㒝㒝㒜㒥㒜㒡㒜㒝㒣㒠㒡㒦㒢㒚㒢㒡㒠㒝㒛㒛㒚㒡㒚㒝㒚㒙㒞㒝㒠㒠㒠㒙㒟㒝㒟㒚㒟㒣㒘㒝㒘㒟㒗㒥㒗㒡㒗㒝㒜㒙㒜㒦㒝㒣㒜㒢㒝㒗㒝㒙㒘㒛㒥㒤㒥㒙㒤㒥㒤㒡㒙㒣㒚㒢㒛㒘㒚㒚㒙㒟㒙㒥㒙㒚㒢㒣㒢㒝㒚㒙㒡㒦㒢㒝㒡㒝㒡㒙㒠㒥㒠㒡㒢㒚㒠㒙㒟㒥㒟㒡㒟㒝㒟㒙㒞㒥㒞㒡㒠㒝㒞㒙㒝㒥㒝㒡㒝㒝㒝㒙㒜㒥㒜㒤㒜㒝㒞㒙㒛㒥㒛㒡㒛㒝㒛㒙㒚㒥㒚㒡㒚㒠㒚㒙㒛㒥㒙㒡㒙㒝㒙㒙㒘㒥㒘㒡㒘㒝㒘㒛㒗㒥㒚㒡㒗㒝㒗㒙㒦㒥㒦㒡㒦㒡㒦㒙㒦㒛㒥㒡㒦㒟㒥㒙㒤㒥㒤㒡㒤㒝㒤㒚㒣㒥㒣㒡㒣㒝㒣㒙㒢㒥㒢㒡㒢㒞㒢㒙㒡㒦㒡㒡㒡㒝㒡㒙㒠㒥㒠㒡㒠㒝㒠㒙㒟㒥㒟㒣㒟㒝㒟㒚㒞㒥㒞㒡㒞㒝㒞㒙㒝㒥㒝㒡㒝㒝㒝㒙㒜㒥㒜㒡㒞㒝㒜㒙㒛㒥㒛㒡㒛㒝㒛㒙㒚㒥㒚㒤㒚㒝㒝㒙㒙㒥㒙㒡㒙㒝㒙㒙㒙㒙㒘㒡㒘㒢㒘㒙㒗㒥㒗㒡㒗㒝㒗㒙㒦㒥㒦㒢㒦㒝㒦㒙㒥㒥㒥㒡㒥㒤㒥㒙㒤㒥㒤㒡㒗㒗㒤㒟㒣㒥㒣㒡㒣㒝㒘㒙㒘㒦㒙㒣㒘㒢㒙㒗㒙㒙㒜㒙㒡㒥㒡㒙㒠㒥㒠㒡㒤㒦㒗㒗㒗㒘㒦㒥㒥㒞㒦㒗㒥㒘㒤㒦㒘㒥㒟㒚㒝㒥㒝㒡㒝㒝㒡㒦㒣㒤㒣㒦㒣㒠㒢㒞㒠㒗㒢㒦㒢㒡㒢㒝㒡㒤㒡㒟㒝㒞㒞㒜㒠㒡㒠㒚㒟㒠㒟㒤㒦㒗㒘㒤㒘㒝㒘㒙㒗㒥㒞㒟㒝㒢㒞㒠㒙㒟㒗㒘㒦㒝㒦㒙㒥㒥㒙㒤㒜㒜㒜㒗㒛㒣㒚㒦㒚㒠㒛㒝㒞㒝㒤㒜㒣㒝㒣㒙㒢㒥㒗㒝㒙㒜㒘㒜㒗㒦㒘㒝㒦㒠㒗㒜㒘㒗㒗㒚㒗㒝㒗㒝㒠㒘㒙㒛㒘㒦㒘㒢㒘㒞㒘㒚㒗㒦㒙㒢㒡㒤㒞㒟㒝㒝㒝㒙㒜㒥㒝㒣㒠㒡㒜㒙㒛㒥㒛㒡㒛㒟㒛㒙㒚㒥㒚㒡㒜㒝㒚㒙㒙㒥㒙㒡㒙㒝㒙㒙㒘㒥㒘㒥㒘㒝㒙㒛㒗㒥㒗㒡㒗㒞㒗㒙㒗㒛㒦㒡㒦㒝㒦㒙㒥㒥㒥㒡㒥㒝㒥㒛㒤㒥㒤㒡㒤㒝㒤㒙㒣㒥㒣㒡㒣㒝㒣㒙㒢㒥㒢㒡㒢㒟㒢㒙㒢㒗㒡㒡㒢㒟㒡㒙㒠㒥㒠㒢㒠㒝㒠㒠㒟㒥㒟㒡㒟㒝㒡㒙㒞㒥㒞㒡㒞㒟㒞㒙㒝㒥㒝㒡㒝㒞㒝㒙㒞㒥㒜㒡㒜㒝㒜㒛㒛㒥㒛㒣㒛㒝㒛㒜㒚㒥㒜㒡㒚㒝㒚㒙㒚㒗㒙㒡㒙㒟㒙㒙㒙㒚㒘㒡㒘㒣㒘㒝㒗㒥㒗㒥㒗㒝㒗㒙㒦㒥㒦㒢㒦㒝㒦㒛㒥㒥㒥㒡㒘㒥㒥㒙㒤㒥㒤㒡㒤㒝㒤㒙㒣㒥㒣㒡㒣㒝㒦㒡㒢㒥㒢㒡㒢㒝㒢㒚㒡㒥㒡㒡㒡㒝㒡㒙㒗㒞㒠㒡㒠㒟㒠㒙㒠㒙㒟㒡㒟㒞㒟㒙㒞㒥㒤㒚㒞㒝㒞㒙㒝㒥㒝㒢㒝㒝㒝㒙㒜㒥㒜㒡㒜㒞㒜㒙㒛㒥㒛㒡㒛㒝㒛㒙㒚㒥㒚㒡㒚㒣㒚㒙㒙㒥㒙㒡㒡㒝㒙㒙㒦㒗㒘㒦㒘㒝㒘㒙㒗㒥㒛㒢㒝㒟㒞㒛㒝㒞㒝㒣㒣㒟㒦㒠㒥㒥㒥㒡㒥㒝㒚㒟㒛㒞㒛㒤㒚㒦㒚㒛㒚㒡㒙㒦㒠㒡㒣㒚㒢㒥㒣㒗㒢㒝㒢㒙㒡㒥㒦㒡㒗㒞㒘㒛㒗㒚㒗㒟㒗㒡㒘㒗㒠㒙㒟㒡㒟㒝㒟㒙㒦㒜㒤㒢㒤㒦㒥㒝㒞㒥㒝㒡㒝㒝㒝㒙㒜㒥㒣㒘㒜㒝㒜㒙㒛㒥㒛㒡㒛㒝㒛㒙㒚㒥㒜㒡㒚㒝㒚㒙㒙㒥㒙㒡㒙㒝㒙㒙㒙㒚㒘㒡㒚㒝㒘㒙㒗㒥㒗㒡㒗㒝㒗㒙㒦㒥㒦㒦㒦㒝㒘㒙㒥㒥㒥㒡㒥㒝㒥㒙㒤㒥㒤㒡㒤㒢㒤㒙㒦㒥㒣㒡㒣㒝㒣㒙㒢㒥㒢㒤㒢㒝㒢㒚㒡㒥㒢㒣㒡㒝㒡㒙㒠㒥㒠㒡㒠㒣㒠㒙㒟㒥㒟㒡㒟㒝㒟㒙㒞㒥㒞㒢㒞㒝㒞㒚㒝㒥㒝㒡㒝㒝㒝㒙㒜㒥㒜㒡㒜㒝㒜㒙㒜㒗㒛㒡㒛㒞㒛㒙㒚㒥㒚㒡㒚㒝㒚㒙㒙㒥㒙㒡㒙㒝㒙㒙㒘㒥㒚㒡㒘㒝㒘㒙㒗㒥㒗㒡㒗㒝㒗㒙㒗㒚㒦㒡㒘㒝㒦㒙㒥㒥㒥㒡㒥㒝㒥㒙㒤㒥㒤㒦㒤㒝㒦㒙㒣㒥㒣㒡㒣㒝㒣㒙㒢㒥㒢㒡㒢㒢㒢㒙㒣㒥㒡㒡㒡㒝㒡㒙㒠㒥㒠㒡㒠㒝㒠㒞㒟㒥㒡㒡㒟㒝㒟㒙㒞㒥㒞㒡㒞㒝㒞㒙㒞㒗㒝㒡㒠㒝㒝㒙㒜㒥㒜㒡㒜㒝㒜㒜㒛㒥㒛㒥㒛㒝㒛㒙㒚㒥㒚㒡㒚㒝㒚㒙㒙㒦㒙㒡㒙㒝㒙㒙㒘㒥㒙㒘㒘㒝㒘㒙㒗㒥㒟㒢㒚㒠㒚㒜㒚㒘㒙㒤㒙㒠㒙㒜㒣㒘㒙㒠㒝㒛㒥㒡㒤㒥㒤㒡㒤㒝㒘㒢㒚㒣㒚㒤㒚㒡㒙㒚㒙㒣㒘㒤㒘㒢㒗㒝㒢㒠㒡㒡㒡㒝㒡㒙㒥㒡㒗㒠㒦㒠㒦㒚㒦㒡㒤㒤㒥㒠㒦㒛㒥㒞㒥㒡㒥㒡㒘㒡㒞㒘㒝㒡㒝㒝㒝㒙㒣㒣㒢㒦㒣㒤㒦㒡㒜㒛㒛㒡㒛㒝㒛㒙㒟㒥㒠㒢㒡㒟㒠㒞㒠㒣㒠㒥㒞㒡㒙㒠㒘㒥㒘㒡㒘㒝㒜㒜㒞㒤㒞㒟㒞㒛㒝㒞㒝㒘㒝㒥㒦㒝㒗㒚㒥㒥㒥㒡㒥㒝㒙㒦㒛㒤㒛㒦㒛㒠㒚㒞㒘㒗㒚㒦㒚㒡㒚㒝㒙㒤㒙㒟㒥㒞㒦㒜㒘㒡㒘㒚㒗㒠㒗㒤㒡㒣㒠㒡㒠㒝㒠㒙㒡㒗㒣㒥㒟㒝㒟㒙㒞㒥㒞㒣㒞㒝㒞㒙㒝㒥㒟㒡㒝㒝㒝㒙㒜㒥㒜㒡㒜㒝㒜㒙㒜㒙㒛㒡㒜㒟㒛㒙㒚㒥㒚㒢㒚㒝㒚㒜㒙㒥㒙㒡㒙㒝㒙㒙㒘㒥㒘㒡㒘㒟㒘㒙㒗㒥㒗㒡㒗㒝㒗㒙㒦㒥㒦㒡㒦㒝㒦㒙㒥㒥㒥㒣㒥㒝㒥㒛㒤㒥㒥㒣㒤㒝㒤㒙㒣㒦㒣㒡㒣㒞㒣㒙㒢㒥㒢㒡㒤㒝㒢㒙㒡㒥㒡㒣㒡㒝㒡㒙㒠㒥㒠㒦㒠㒝㒢㒙㒟㒥㒟㒡㒟㒟㒟㒙㒟㒗㒞㒡㒞㒤㒞㒙㒟㒥㒝㒡㒝㒝㒝㒛㒜㒥㒜㒣㒜㒝㒜㒟㒛㒥㒜㒗㒛㒡㒛㒙㒛㒙㒚㒡㒚㒝㒚㒙㒙㒦㒙㒡㒙㒟㒙㒙㒘㒥㒜㒙㒘㒝㒘㒙㒗㒥㒗㒡㒗㒝㒗㒙㒦㒥㒦㒡㒙㒥㒦㒙㒥㒥㒥㒡㒥㒞㒥㒙㒤㒥㒤㒡㒤㒝㒚㒢㒣㒥㒣㒣㒣㒝㒣㒝㒢㒥㒢㒢㒢㒝㒢㒙㒗㒞㒡㒡㒡㒝㒡㒙㒠㒦㒠㒡㒠㒝㒠㒙㒟㒥㒟㒢㒟㒝㒟㒙㒞㒥㒞㒡㒞㒝㒞㒙㒝㒥㒝㒣㒝㒝㒝㒙㒜㒥㒡㒥㒙㒘㒜㒙㒛㒥㒛㒡㒢㒙㒢㒘㒠㒦㒠㒥㒡㒠㒡㒝㒡㒗㒠㒚㒠㒛㒟㒠㒛㒝㒟㒘㒞㒞㒞㒦㒞㒚㒛㒛㒛㒥㒞㒝㒞㒙㒝㒡㒚㒤㒜㒞㒝㒙㒘㒙㒗㒥㒗㒠㒛㒝㒛㒥㒛㒡㒛㒙㒛㒘㒗㒛㒦㒜㒦㒘㒙㒜㒙㒚㒙㒠㒙㒝㒤㒣㒘㒘㒗㒦㒘㒝㒗㒝㒗㒦㒦㒟㒗㒞㒗㒘㒥㒦㒦㒟㒥㒜㒥㒤㒥㒟㒥㒡㒤㒞㒤㒣㒤㒥㒠㒛㒣㒜㒣㒤㒣㒞㒟㒜㒢㒦㒢㒚㒢㒠㒣㒗㒢㒘㒡㒣㒠㒦㒟㒦㒟㒝㒜㒤㒟㒣㒟㒣㒜㒙㒜㒘㒜㒘㒞㒡㒞㒟㒞㒛㒛㒚㒝㒣㒚㒙㒜㒦㒚㒘㒙㒝㒙㒙㒘㒦㒙㒘㒘㒠㒘㒙㒘㒙㒚㒥㒚㒡㒚㒝㒗㒛㒗㒘㒙㒣㒙㒝㒙㒘㒘㒥㒥㒠㒥㒠㒤㒥㒤㒠㒘㒟㒗㒚㒘㒜㒣㒠㒦㒢㒣㒚㒣㒙㒥㒦㒢㒤㒢㒝㒥㒛㒡㒥㒡㒟㒡㒞㒤㒗㒠㒡㒠㒣㒠㒙㒣㒙㒣㒗㒟㒢㒟㒛㒟㒘㒞㒤㒞㒡㒞㒜㒡㒘㒡㒗㒝㒠㒝㒙㒠㒗㒝㒘㒜㒥㒜㒠㒛㒥㒜㒘㒛㒡㒞㒞㒞㒗㒚㒤㒝㒠㒚㒞㒝㒙㒙㒣㒙㒜㒜㒚㒝㒗㒛㒤㒛㒢㒜㒞㒜㒘㒦㒦㒗㒟㒗㒞㒗㒗㒦㒡㒚㒥㒥㒞㒦㒗㒥㒦㒥㒟㒥㒙㒘㒛㒘㒝㒘㒦㒣㒞㒤㒗㒣㒦㒣㒟㒣㒙㒣㒗㒡㒦㒢㒟㒢㒞㒢㒗㒡㒡㒥㒜㒤㒛㒤㒛㒤㒝㒤㒢㒣㒜㒢㒦㒣㒥㒣㒜㒣㒛㒞㒜㒞㒚㒞㒙㒢㒝㒢㒗㒡㒦㒠㒢㒜㒢㒜㒞㒜㒙㒛㒦㒙㒣㒙㒟㒛㒛㒙㒗㒘㒙㒗㒥㒗㒡㒞㒙㒞㒘㒜㒦㒜㒥㒝㒠㒝㒝㒝㒗㒜㒚㒜㒛㒛㒠㒥㒚㒤㒡㒤㒝㒤㒙㒥㒗㒗㒛㒣㒝㒣㒙㒢㒥㒢㒣㒢㒝㒢㒙㒡㒥㒢㒣㒡㒝㒡㒙㒠㒦㒠㒡㒠㒞㒠㒙㒟㒥㒟㒡㒟㒝㒟㒙㒞㒥㒞㒡㒞㒝㒞㒛㒝㒥㒝㒣㒝㒝㒝㒙㒜㒥㒜㒡㒜㒝㒜㒙㒛㒦㒛㒡㒛㒞㒛㒙㒚㒥㒚㒡㒚㒝㒚㒙㒙㒥㒙㒢㒙㒝㒙㒙㒘㒥㒘㒡㒘㒣㒘㒙㒗㒥㒗㒡㒜㒡㒗㒟㒦㒥㒦㒡㒦㒝㒛㒙㒛㒦㒜㒣㒛㒢㒜㒗㒜㒙㒟㒙㒤㒥㒤㒙㒣㒥㒣㒡㒗㒦㒚㒗㒚㒘㒙㒥㒘㒞㒙㒗㒘㒘㒗㒦㒡㒝㒡㒠㒠㒥㒠㒡㒠㒝㒤㒜㒦㒤㒦㒟㒦㒛㒥㒞㒥㒘㒥㒥㒡㒗㒞㒜㒝㒥㒝㒡㒝㒝㒤㒗㒣㒚㒤㒘㒤㒛㒜㒤㒛㒥㒛㒡㒛㒝㒟㒥㒡㒤㒠㒤㒠㒞㒠㒥㒟㒘㒟㒤㒠㒟㒟㒢㒟㒥㒟㒥㒠㒛㒙㒚㒗㒥㒗㒡㒗㒝㒛㒦㒝㒤㒝㒦㒝㒠㒜㒞㒚㒗㒜㒦㒜㒡㒜㒝㒛㒤㒛㒟㒗㒞㒘㒜㒚㒡㒚㒚㒙㒠㒙㒤㒣㒠㒢㒡㒢㒝㒢㒙㒣㒗㒚㒦㒡㒝㒡㒙㒠㒥㒠㒣㒠㒝㒠㒙㒟㒥㒡㒡㒟㒝㒟㒙㒞㒥㒞㒡㒞㒝㒞㒙㒞㒙㒝㒡㒞㒟㒝㒙㒜㒥㒜㒢㒜㒝㒜㒞㒛㒥㒛㒡㒛㒝㒛㒙㒚㒥㒚㒡㒚㒟㒚㒙㒙㒥㒙㒡㒙㒝㒙㒙㒘㒥㒘㒡㒘㒝㒘㒙㒗㒥㒗㒣㒗㒝㒗㒛㒦㒥㒘㒡㒦㒝㒦㒙㒥㒦㒥㒡㒥㒝㒥㒙㒤㒦㒤㒡㒦㒝㒤㒙㒣㒥㒣㒢㒣㒝㒣㒚㒢㒥㒣㒗㒢㒝㒤㒙㒡㒥㒡㒡㒡㒞㒡㒙㒠㒦㒠㒡㒠㒠㒠㒙㒠㒗㒣㒦㒟㒝㒟㒜㒞㒥㒞㒡㒞㒝㒞㒙㒝㒥㒝㒡㒣㒦㒝㒙㒜㒦㒜㒡㒜㒠㒜㒙㒛㒦㒛㒡㒛㒝㒠㒢㒚㒥㒚㒡㒚㒝㒚㒚㒙㒥㒙㒡㒙㒝㒙㒙㒘㒦㒘㒡㒘㒝㒘㒙㒗㒥㒗㒡㒗㒝㒗㒙㒗㒙㒦㒡㒦㒝㒦㒙㒘㒟㒦㒛㒥㒝㒥㒙㒤㒥㒛㒝㒛㒜㒚㒚㒚㒙㒚㒤㒚㒡㒚㒛㒙㒞㒙㒟㒘㒤㒟㒛㒢㒜㒡㒡㒡㒝㒡㒙㒥㒝㒗㒥㒗㒡㒗㒙㒤㒜㒥㒦㒦㒡㒜㒛㒟㒙㒞㒡㒞㒝㒞㒙㒤㒜㒣㒢㒤㒚㒣㒞㒗㒝㒡㒛㒜㒝㒜㒙㒛㒥㒢㒙㒢㒡㒢㒝㒡㒥㒡㒤㒞㒗㒝㒘㒜㒤㒠㒣㒟㒞㒠㒠㒛㒣㒟㒘㒞㒦㒟㒝㒞㒝㒞㒦㒝㒟㒞㒞㒞㒘㒜㒦㒝㒟㒜㒜㒜㒤㒜㒟㒜㒡㒛㒞㒛㒣㒛㒥㒗㒛㒚㒜㒚㒤㒚㒞㒦㒜㒘㒜㒙㒞㒙㒝㒘㒞㒙㒗㒘㒙㒤㒥㒤㒢㒤㒞㒣㒦㒣㒠㒗㒚㒗㒞㒗㒘㒦㒚㒥㒠㒢㒘㒥㒢㒤㒢㒤㒦㒥㒗㒠㒤㒤㒣㒣㒢㒣㒦㒣㒤㒣㒥㒢㒢㒣㒙㒣㒘㒣㒚㒡㒜㒢㒗㒡㒤㒡㒥㒠㒜㒠㒦㒠㒞㒠㒟㒟㒢㒙㒡㒘㒥㒘㒡㒘㒝㒙㒛㒜㒜㒗㒡㒗㒝㒗㒙㒦㒦㒦㒡㒦㒝㒦㒙㒗㒗㒥㒡㒥㒝㒥㒚㒤㒥㒤㒤㒤㒝㒤㒙㒣㒥㒥㒡㒣㒝㒣㒙㒢㒦㒢㒡㒢㒞㒢㒙㒢㒗㒡㒡㒢㒟㒡㒙㒠㒥㒠㒤㒠㒝㒠㒝㒟㒥㒟㒡㒟㒝㒟㒙㒞㒥㒞㒡㒞㒞㒞㒙㒞㒘㒝㒡㒝㒝㒝㒙㒜㒥㒜㒡㒜㒝㒜㒙㒛㒥㒛㒡㒛㒝㒛㒛㒚㒥㒚㒡㒚㒝㒚㒙㒙㒥㒙㒡㒙㒞㒙㒙㒘㒦㒘㒡㒘㒝㒘㒙㒗㒥㒗㒡㒗㒝㒗㒚㒦㒥㒦㒡㒦㒝㒦㒙㒦㒛㒥㒡㒥㒝㒥㒙㒢㒗㒥㒢㒤㒝㒤㒙㒣㒥㒘㒞㒚㒜㒚㒞㒚㒘㒘㒦㒦㒟㒙㒞㒙㒙㒘㒥㒘㒜㒘㒗㒣㒦㒤㒤㒗㒙㒦㒢㒦㒘㒦㒜㒤㒡㒟㒡㒞㒥㒞㒡㒞㒝㒢㒢㒤㒣㒤㒤㒤㒡㒣㒚㒣㒣㒢㒤㒢㒢㒦㒡㒜㒛㒛㒡㒛㒝㒛㒙㒟㒥㒠㒢㒡㒟㒠㒞㒠㒣㒠㒥㒙㒝㒙㒠㒘㒥㒘㒡㒘㒝㒜㒜㒞㒤㒞㒟㒞㒛㒝㒞㒝㒘㒝㒥㒦㒝㒦㒜㒥㒥㒥㒡㒥㒝㒜㒗㒛㒚㒜㒘㒤㒝㒤㒤㒣㒥㒣㒡㒣㒝㒗㒥㒙㒤㒘㒤㒘㒞㒘㒥㒗㒘㒗㒤㒘㒟㒗㒢㒗㒥㒗㒥㒡㒘㒠㒙㒟㒥㒟㒡㒠㒟㒘㒞㒞㒥㒞㒡㒞㒝㒞㒛㒝㒥㒝㒡㒝㒝㒟㒙㒜㒥㒜㒡㒜㒝㒜㒙㒛㒥㒛㒡㒛㒢㒛㒙㒜㒗㒚㒡㒚㒝㒚㒚㒙㒥㒚㒗㒙㒝㒙㒙㒘㒥㒘㒡㒘㒝㒘㒙㒘㒗㒗㒡㒗㒝㒗㒙㒦㒥㒦㒡㒦㒝㒦㒙㒥㒥㒥㒡㒥㒝㒥㒛㒤㒥㒤㒣㒤㒝㒦㒙㒣㒥㒣㒡㒣㒞㒣㒙㒢㒥㒢㒡㒢㒠㒢㒙㒣㒥㒡㒡㒡㒝㒡㒚㒠㒥㒠㒢㒠㒝㒠㒚㒟㒥㒡㒡㒟㒝㒟㒙㒞㒦㒞㒡㒞㒞㒞㒙㒞㒙㒝㒡㒝㒟㒡㒞㒜㒥㒜㒤㒜㒝㒜㒙㒛㒥㒛㒡㒛㒝㒛㒙㒡㒞㒚㒡㒚㒞㒚㒙㒚㒘㒙㒡㒙㒞㒙㒙㒘㒥㒞㒚㒘㒝㒘㒙㒗㒥㒗㒢㒗㒝㒗㒙㒦㒥㒦㒡㒦㒞㒦㒙㒥㒥㒥㒡㒥㒝㒥㒙㒤㒥㒤㒡㒤㒡㒤㒙㒣㒥㒣㒡㒘㒡㒦㒥㒢㒥㒢㒡㒢㒝㒘㒡㒙㒙㒘㒥㒘㒝㒘㒜㒤㒟㒣㒠㒣㒜㒗㒛㒥㒦㒗㒘㒢㒛㒥㒠㒥㒞㒥㒥㒤㒥㒥㒞㒤㒗㒤㒦㒤㒠㒣㒞㒤㒗㒢㒤㒣㒜㒣㒗㒣㒙㒡㒦㒢㒛㒢㒝㒝㒣㒠㒤㒡㒜㒠㒦㒜㒤㒞㒤㒟㒦㒟㒥㒞㒦㒟㒟㒞㒡㒛㒝㒛㒚㒚㒦㒚㒞㒚㒘㒝㒢㒝㒦㒝㒠㒜㒢㒜㒘㒘㒠㒜㒚㒛㒚㒛㒞㒛㒟㒗㒜㒘㒠㒛㒚㒚㒟㒚㒠㒘㒝㒣㒟㒢㒡㒢㒝㒢㒙㒘㒡㒘㒠㒗㒞㒗㒝㒘㒘㒗㒥㒗㒟㒦㒢㒦㒣㒦㒘㒟㒝㒟㒝㒞㒥㒞㒡㒞㒝㒤㒠㒣㒦㒤㒞㒣㒢㒗㒡㒝㒜㒜㒡㒜㒝㒜㒙㒠㒝㒢㒥㒢㒡㒢㒙㒟㒜㒠㒦㒡㒡㒚㒡㒙㒥㒙㒡㒙㒝㒚㒛㒝㒜㒘㒡㒘㒝㒘㒙㒘㒗㒗㒡㒗㒝㒗㒙㒘㒗㒦㒡㒦㒝㒦㒚㒥㒥㒥㒤㒥㒝㒥㒙㒤㒥㒦㒡㒤㒝㒤㒙㒣㒦㒣㒡㒣㒞㒣㒙㒣㒙㒢㒡㒣㒟㒢㒙㒡㒥㒡㒤㒡㒝㒡㒚㒠㒥㒠㒡㒠㒝㒠㒙㒟㒥㒟㒡㒟㒞㒟㒙㒟㒘㒞㒡㒞㒝㒞㒙㒝㒥㒝㒡㒝㒝㒝㒙㒜㒥㒜㒡㒜㒝㒜㒛㒛㒥㒛㒡㒛㒝㒛㒙㒚㒥㒚㒡㒚㒞㒚㒙㒙㒦㒙㒡㒙㒝㒙㒙㒘㒥㒘㒡㒘㒝㒘㒚㒗㒥㒗㒡㒗㒝㒗㒙㒗㒛㒦㒡㒦㒝㒦㒙㒛㒙㒦㒗㒥㒝㒥㒙㒤㒥㒙㒡㒚㒞㒛㒛㒚㒚㒚㒟㒚㒡㒠㒛㒣㒝㒢㒡㒢㒝㒢㒙㒦㒞㒘㒟㒘㒠㒘㒝㒦㒦㒗㒟㒦㒠㒦㒞㒥㒙㒠㒜㒟㒝㒟㒙㒞㒥㒣㒝㒥㒜㒤㒜㒣㒦㒤㒝㒢㒠㒣㒜㒤㒗㒣㒚㒣㒝㒣㒝㒙㒗㒜㒘㒛㒝㒛㒙㒚㒥㒞㒤㒡㒜㒡㒗㒠㒣㒟㒦㒟㒠㒠㒝㒦㒗㒘㒤㒘㒝㒘㒙㒗㒥㒞㒟㒝㒢㒞㒠㒤㒗㒗㒢㒦㒝㒦㒙㒥㒥㒚㒞㒜㒜㒜㒞㒜㒘㒚㒦㒘㒟㒛㒞㒛㒙㒚㒥㒚㒜㒚㒗㒥㒦㒦㒤㒙㒙㒘㒢㒘㒘㒘㒜㒢㒘㒡㒙㒠㒥㒠㒡㒡㒟㒙㒞㒟㒥㒟㒡㒟㒝㒟㒛㒞㒥㒞㒡㒞㒝㒠㒙㒝㒥㒝㒡㒝㒝㒝㒙㒜㒥㒜㒡㒜㒢㒜㒙㒝㒗㒛㒡㒛㒝㒛㒚㒚㒥㒚㒤㒚㒝㒚㒙㒙㒥㒙㒡㒙㒝㒙㒙㒙㒗㒘㒡㒘㒝㒘㒙㒗㒥㒗㒡㒗㒝㒗㒙㒦㒥㒦㒡㒦㒝㒦㒛㒥㒥㒥㒣㒥㒝㒗㒙㒤㒥㒤㒡㒤㒞㒤㒙㒣㒥㒣㒡㒣㒞㒣㒙㒤㒥㒢㒡㒢㒝㒢㒚㒡㒥㒡㒢㒡㒝㒡㒟㒠㒥㒢㒡㒠㒝㒠㒙㒟㒦㒟㒡㒟㒞㒟㒙㒟㒙㒞㒡㒞㒟㒢㒞㒝㒥㒝㒤㒝㒝㒝㒙㒜㒥㒜㒡㒜㒝㒜㒙㒢㒞㒛㒡㒛㒞㒛㒙㒛㒘㒚㒡㒚㒞㒚㒙㒙㒥㒟㒚㒙㒝㒙㒙㒘㒥㒘㒢㒘㒝㒘㒙㒗㒥㒗㒡㒗㒞㒗㒙㒦㒥㒦㒡㒦㒝㒦㒙㒥㒥㒥㒡㒥㒝㒥㒙㒤㒥㒤㒡㒤㒤㒤㒙㒣㒥㒣㒡㒣㒝㒘㒠㒢㒥㒢㒡㒢㒝㒢㒚㒡㒥㒡㒡㒡㒝㒡㒙㒠㒥㒠㒡㒠㒝㒠㒙㒟㒥㒟㒡㒟㒝㒟㒙㒞㒥㒞㒡㒞㒝㒞㒙㒝㒥㒝㒡㒝㒝㒝㒙㒜㒥㒜㒡㒜㒝㒜㒙㒛㒥㒛㒡㒛㒠㒛㒙㒚㒥㒚㒡㒚㒝㒚㒙㒙㒥㒙㒡㒙㒝㒙㒙㒘㒥㒘㒡㒘㒝㒘㒙㒗㒥㒗㒡㒗㒝㒗㒙㒗㒗㒦㒡㒦㒝㒦㒙㒥㒥㒥㒡㒥㒝㒥㒙㒤㒥㒤㒢㒤㒝㒤㒙㒣㒥㒣㒡㒣㒟㒣㒙㒢㒥㒢㒡㒥㒗㒢㒞㒡㒥㒡㒡㒡㒝㒘㒙㒗㒘㒦㒢㒗㒙㒦㒥㒠㒘㒟㒡㒟㒝㒟㒙㒞㒥㒞㒡㒞㒝㒞㒙㒝㒥㒟㒟㒝㒝㒝㒙㒜㒥㒝㒣㒞㒝㒜㒙㒜㒗㒛㒡㒛㒟㒛㒙㒚㒥㒚㒡㒛㒟㒜㒙㒙㒥㒙㒤㒙㒝㒙㒛㒘㒥㒘㒡㒘㒝㒙㒛㒟㒜㒗㒡㒗㒡㒗㒙㒦㒦㒦㒡㒦㒝㒦㒙㒦㒛㒥㒥㒥㒝㒥㒞㒤㒥㒤㒡㒤㒝㒤㒚㒣㒥㒣㒥㒣㒝㒣㒙㒦㒝㒢㒡㒢㒝㒢㒙㒢㒗㒡㒡㒡㒝㒡㒙㒠㒥㒤㒙㒠㒝㒠㒙㒟㒥㒟㒡㒟㒝㒟㒙㒞㒥㒞㒡㒡㒥㒞㒙㒝㒥㒝㒡㒝㒠㒝㒙㒜㒥㒜㒡㒜㒝㒟㒡㒛㒥㒛㒡㒛㒝㒛㒚㒚㒥㒚㒡㒚㒝㒚㒙㒝㒠㒙㒡㒙㒡㒙㒙㒙㒗㒘㒡㒘㒞㒘㒙㒘㒛㒙㒚㒗㒝㒗㒙㒦㒥㒗㒝㒦㒝㒦㒚㒥㒥㒥㒢㒥㒝㒥㒝㒥㒣㒤㒡㒤㒝㒤㒙㒤㒡㒣㒡㒣㒞㒣㒙㒣㒙㒣㒟㒢㒝㒢㒙㒡㒥㒣㒛㒡㒝㒡㒚㒠㒥㒡㒗㒡㒦㒠㒙㒟㒥㒟㒡㒠㒜㒟㒙㒞㒦㒞㒡㒞㒞㒞㒙㒞㒙㒞㒟㒝㒝㒝㒙㒜㒥㒝㒠㒜㒝㒜㒚㒛㒥㒛㒥㒜㒛㒛㒙㒚㒥㒚㒡㒜㒗㒚㒙㒙㒦㒙㒡㒙㒣㒙㒟㒘㒥㒘㒢㒘㒝㒙㒣㒗㒥㒗㒢㒗㒝㒗㒙㒦㒥㒦㒥㒗㒛㒦㒙㒥㒥㒥㒡㒗㒗㒥㒙㒤㒦㒤㒡㒤㒝㒦㒗㒣㒥㒣㒥㒣㒝㒣㒛㒢㒥㒢㒤㒢㒝㒢㒙㒣㒣㒡㒡㒡㒢㒡㒙㒡㒘㒠㒡㒠㒟㒠㒙㒠㒛㒡㒚㒟㒝㒟㒝㒞㒥㒠㒗㒞㒝㒞㒚㒝㒥㒝㒦㒝㒝㒝㒝㒝㒣㒜㒡㒜㒝㒜㒙㒝㒛㒛㒡㒛㒞㒛㒙㒛㒙㒛㒟㒚㒝㒚㒙㒙㒥㒛㒛㒙㒝㒙㒚㒘㒥㒘㒡㒚㒛㒘㒙㒘㒙㒗㒡㒗㒟㒗㒙㒗㒘㒦㒡㒦㒝㒘㒗㒥㒥㒥㒦㒥㒝㒥㒜㒤㒥㒤㒣㒤㒝㒤㒟㒥㒞㒣㒡㒣㒡㒣㒙㒤㒠㒢㒡㒢㒞㒢㒙㒢㒚㒡㒡㒡㒡㒢㒗㒠㒥㒠㒡㒠㒝㒡㒤㒟㒥㒟㒢㒟㒝㒟㒙㒟㒥㒞㒡㒞㒡㒞㒙㒝㒥㒝㒡㒝㒝㒝㒙㒜㒥㒢㒗㒜㒝㒜㒝㒛㒥㒛㒢㒛㒝㒛㒙㒚㒥㒚㒡㒣㒣㒚㒙㒚㒙㒙㒡㒙㒟㒙㒙㒘㒥㒘㒡㒘㒝㒝㒢㒗㒥㒗㒡㒗㒝㒗㒚㒦㒥㒦㒡㒦㒝㒦㒛㒥㒦㒥㒡㒥㒝㒥㒙㒤㒥㒤㒡㒤㒝㒤㒙㒤㒙㒣㒡㒣㒝㒣㒙㒝㒝㒣㒘㒢㒝㒢㒙㒡㒥㒦㒙㒘㒡㒘㒝㒗㒥㒥㒘㒦㒢㒗㒝㒥㒙㒟㒥㒟㒝㒟㒙㒞㒥㒥㒘㒤㒞㒤㒦㒤㒚㒚㒣㒞㒗㒝㒙㒜㒥㒜㒡㒣㒙㒣㒘㒡㒦㒡㒥㒢㒠㒢㒝㒢㒗㒡㒚㒡㒛㒠㒠㒗㒗㒝㒥㒙㒝㒙㒙㒘㒥㒟㒙㒟㒡㒟㒝㒞㒥㒞㒤㒛㒗㒚㒘㒙㒤㒝㒣㒜㒞㒝㒠㒘㒣㒜㒘㒛㒦㒜㒝㒛㒝㒛㒦㒚㒟㒛㒞㒛㒘㒙㒦㒚㒟㒙㒜㒙㒤㒙㒟㒙㒡㒘㒞㒘㒣㒘㒥㒤㒛㒗㒜㒗㒤㒗㒞㒣㒜㒤㒞㒦㒙㒦㒘㒥㒢㒣㒢㒤㒞㒡㒠㒤㒦㒥㒗㒤㒛㒤㒚㒤㒛㒣㒢㒤㒙㒢㒦㒣㒦㒢㒢㒢㒚㒢㒝㒡㒡㒞㒘㒡㒢㒠㒢㒡㒠㒡㒝㒠㒚㒠㒣㒜㒜㒠㒜㒟㒤㒟㒦㒟㒟㒞㒜㒞㒚㒘㒙㒗㒝㒗㒙㒦㒥㒗㒣㒚㒤㒦㒙㒥㒥㒥㒡㒥㒠㒥㒙㒤㒥㒤㒡㒥㒟㒤㒙㒣㒥㒣㒢㒣㒝㒣㒛㒢㒥㒢㒡㒢㒝㒤㒙㒡㒥㒡㒡㒡㒞㒡㒙㒠㒦㒠㒡㒠㒞㒠㒙㒡㒗㒟㒡㒟㒝㒟㒜㒞㒥㒞㒥㒞㒝㒞㒙㒝㒥㒝㒡㒝㒝㒝㒙㒜㒦㒜㒡㒜㒠㒜㒙㒛㒥㒛㒡㒛㒝㒛㒙㒚㒥㒚㒡㒚㒝㒚㒙㒙㒥㒙㒣㒙㒝㒙㒙㒘㒥㒘㒡㒘㒝㒘㒙㒗㒦㒗㒡㒗㒞㒗㒙㒦㒥㒦㒡㒦㒝㒦㒙㒥㒥㒥㒢㒥㒝㒥㒙㒤㒥㒤㒡㒤㒣㒤㒙㒣㒥㒣㒡㒦㒗㒣㒟㒢㒥㒢㒡㒢㒝㒗㒙㒗㒦㒘㒣㒗㒢㒘㒗㒘㒙㒝㒣㒠㒤㒠㒙㒟㒥㒟㒡㒣㒠㒦㒘㒥㒣㒥㒟㒤㒢㒤㒜㒥㒙㒢㒥㒝㒠㒝㒙㒜㒥㒜㒡㒣㒛㒢㒞㒣㒜㒘㒣㒜㒞㒛㒙㒚㒥㒚㒡㒟㒚㒡㒘㒡㒚㒠㒤㒟㒢㒝㒛㒠㒚㒟㒥㒟㒡㒟㒘㒞㒣㒚㒢㒛㒠㒝㒥㒝㒞㒜㒤㒝㒘㒣㒛㒦㒠㒥㒡㒥㒝㒥㒙㒙㒡㒛㒠㒚㒠㒚㒚㒚㒡㒘㒤㒙㒠㒚㒛㒙㒞㒙㒡㒙㒡㒟㒛㒢㒝㒡㒡㒡㒝㒡㒙㒥㒞㒗㒟㒗㒠㒗㒝㒥㒦㒦㒟㒥㒠㒥㒞㒟㒠㒞㒡㒞㒝㒞㒙㒟㒗㒦㒦㒝㒝㒝㒙㒜㒥㒝㒗㒜㒝㒜㒙㒛㒥㒝㒡㒛㒝㒛㒙㒚㒥㒚㒡㒚㒝㒚㒙㒚㒘㒙㒡㒚㒟㒙㒙㒘㒥㒘㒢㒘㒝㒘㒞㒗㒥㒗㒡㒗㒝㒗㒙㒦㒥㒦㒡㒦㒟㒦㒙㒥㒥㒥㒡㒥㒝㒥㒙㒤㒥㒤㒡㒤㒝㒤㒙㒣㒥㒣㒣㒣㒝㒣㒛㒢㒥㒤㒡㒢㒝㒢㒙㒡㒦㒡㒡㒡㒝㒡㒙㒠㒦㒠㒡㒢㒝㒠㒙㒟㒥㒟㒢㒟㒝㒟㒚㒞㒥㒞㒥㒞㒝㒠㒙㒝㒥㒝㒡㒝㒞㒝㒙㒜㒦㒜㒡㒜㒟㒜㒙㒜㒗㒟㒦㒛㒝㒛㒜㒚㒥㒚㒡㒚㒝㒚㒙㒙㒥㒙㒡㒟㒦㒙㒙㒘㒦㒘㒡㒘㒠㒘㒙㒗㒦㒗㒡㒗㒝㒜㒢㒦㒥㒦㒡㒦㒝㒦㒚㒥㒥㒥㒡㒥㒝㒥㒙㒤㒥㒤㒡㒤㒝㒤㒙㒤㒝㒣㒡㒣㒝㒣㒙㒣㒘㒢㒡㒢㒝㒢㒙㒡㒥㒡㒡㒡㒝㒠㒙㒤㒤㒘㒟㒠㒠㒠㒙㒟㒥㒟㒡㒦㒠㒦㒞㒥㒗㒡㒛㒟㒙㒞㒙㒝㒥㒝㒡㒢㒘㒣㒤㒢㒝㒣㒥㒡㒢㒢㒘㒡㒟㒟㒥㒠㒙㒟㒥㒡㒟㒟㒚㒚㒝㒚㒙㒙㒥㒙㒡㒙㒝㒙㒙㒙㒙㒘㒡㒘㒝㒘㒙㒞㒘㒞㒙㒝㒞㒞㒛㒗㒘㒦㒡㒦㒝㒦㒙㒥㒥㒥㒡㒥㒝㒜㒙㒘㒥㒤㒡㒤㒡㒤㒙㒣㒥㒣㒡㒙㒟㒚㒢㒚㒙㒘㒦㒥㒗㒢㒟㒡㒥㒡㒡㒡㒝㒘㒜㒘㒙㒗㒣㒦㒦㒗㒗㒦㒜㒡㒣㒟㒝㒟㒙㒞㒥㒟㒣㒥㒤㒞㒙㒞㒘㒝㒡㒝㒠㒝㒙㒜㒥㒜㒡㒜㒝㒟㒠㒛㒥㒛㒤㒛㒝㒛㒜㒚㒥㒚㒢㒚㒝㒚㒟㒜㒜㒙㒡㒙㒠㒙㒙㒙㒚㒘㒡㒘㒞㒘㒙㒗㒦㒗㒡㒗㒡㒘㒗㒦㒥㒦㒡㒦㒝㒦㒞㒥㒥㒥㒢㒥㒝㒥㒝㒥㒣㒤㒡㒤㒝㒤㒙㒤㒝㒣㒡㒣㒞㒣㒙㒤㒗㒚㒘㒢㒝㒢㒜㒡㒥㒡㒤㒡㒝㒡㒙㒠㒥㒠㒡㒣㒤㒠㒙㒠㒘㒟㒡㒟㒠㒟㒙㒞㒦㒞㒡㒞㒝㒗㒟㒝㒥㒝㒤㒝㒝㒝㒛㒜㒥㒜㒡㒜㒝㒝㒛㒝㒥㒛㒡㒛㒠㒛㒙㒚㒦㒚㒡㒚㒝㒚㒙㒛㒗㒝㒗㒙㒝㒙㒝㒘㒥㒘㒥㒘㒝㒘㒙㒗㒥㒘㒣㒗㒝㒗㒙㒗㒚㒦㒡㒦㒞㒦㒙㒥㒥㒥㒡㒥㒝㒥㒙㒤㒥㒥㒗㒤㒝㒤㒙㒣㒥㒣㒡㒣㒝㒤㒛㒢㒥㒢㒡㒢㒤㒢㒙㒡㒦㒡㒡㒡㒝㒡㒙㒡㒙㒠㒡㒠㒝㒠㒞㒟㒥㒡㒟㒟㒝㒟㒚㒞㒥㒞㒡㒥㒛㒞㒙㒞㒞㒝㒡㒝㒡㒝㒙㒜㒥㒜㒡㒝㒟㒟㒝㒛㒥㒜㒛㒛㒝㒛㒡㒚㒥㒚㒡㒚㒝㒜㒙㒙㒥㒙㒡㒚㒗㒙㒙㒙㒟㒘㒡㒘㒢㒘㒙㒙㒥㒗㒡㒗㒝㒗㒤㒦㒥㒦㒡㒦㒝㒦㒛㒥㒥㒥㒡㒥㒝㒥㒙㒥㒢㒤㒡㒤㒥㒤㒙㒣㒥㒣㒡㒣㒝㒣㒙㒢㒥㒣㒟㒢㒝㒢㒡㒡㒥㒡㒡㒡㒝㒡㒙㒠㒥㒠㒡㒡㒘㒠㒙㒠㒣㒟㒡㒟㒟㒟㒙㒠㒥㒞㒡㒞㒝㒞㒤㒝㒥㒞㒜㒝㒝㒝㒠㒜㒥㒜㒡㒜㒝㒜㒙㒜㒠㒛㒡㒛㒟㒛㒙㒛㒗㒚㒡㒚㒝㒚㒙㒙㒥㒚㒜㒙㒝㒙㒤㒘㒥㒘㒤㒘㒝㒚㒙㒗㒥㒗㒡㒘㒘㒗㒙㒗㒠㒦㒡㒦㒣㒦㒙㒥㒥㒥㒡㒥㒝㒥㒣㒤㒥㒤㒣㒤㒝㒤㒛㒣㒥㒣㒡㒣㒝㒣㒙㒣㒙㒢㒡㒢㒦㒢㒙㒢㒟㒡㒡㒡㒝㒡㒙㒠㒥㒡㒚㒠㒝㒠㒜㒟㒥㒟㒣㒟㒝㒡㒙㒞㒥㒞㒡㒞㒠㒞㒙㒞㒞㒝㒡㒝㒣㒝㒙㒝㒙㒡㒠㒜㒝㒜㒞㒛㒥㒜㒟㒛㒝㒛㒚㒚㒥㒛㒣㒡㒤㒚㒙㒚㒚㒙㒡㒙㒠㒙㒙㒘㒥㒘㒡㒘㒝㒞㒜㒗㒥㒗㒦㒗㒝㒗㒚㒦㒥㒦㒥㒦㒝㒦㒙㒟㒛㒥㒡㒥㒡㒥㒙㒥㒗㒤㒡㒤㒝㒤㒙㒣㒥㒙㒚㒣㒝㒣㒙㒢㒥㒢㒢㒢㒝㒢㒙㒡㒥㒡㒤㒡㒞㒡㒙㒠㒥㒠㒡㒠㒝㒠㒙㒟㒥㒟㒡㒟㒡㒟㒙㒞㒥㒞㒡㒘㒥㒞㒣㒝㒥㒝㒡㒝㒝㒣㒥㒣㒤㒢㒢㒢㒡㒣㒜㒣㒙㒢㒣㒡㒦㒢㒗㒡㒜㒟㒥㒞㒟㒚㒙㒙㒥㒙㒡㒟㒥㒠㒝㒠㒙㒟㒡㒟㒠㒛㒣㒚㒤㒚㒠㒞㒟㒝㒚㒞㒜㒙㒟㒜㒤㒜㒢㒝㒙㒜㒙㒜㒢㒛㒛㒜㒚㒛㒤㒚㒢㒛㒛㒚㒘㒚㒠㒚㒛㒚㒝㒙㒚㒙㒟㒙㒡㒥㒗㒘㒘㒘㒠㒘㒚㒤㒘㒤㒙㒥㒣㒦㒞㒗㒞㒦㒡㒢㒠㒤㒙㒦㒞㒤㒦㒡㒞㒣㒝㒥㒛㒤㒤㒤㒛㒣㒢㒣㒜㒤㒙㒣㒤㒟㒜㒢㒦㒡㒦㒢㒚㒢㒛㒞㒘㒟㒣㒡㒠㒡㒥㒡㒢㒜㒣㒠㒝㒠㒢㒟㒚㒛㒟㒙㒘㒘㒝㒘㒙㒗㒥㒜㒙㒞㒡㒞㒝㒝㒥㒛㒘㒜㒢㒝㒝㒝㒣㒥㒥㒥㒝㒥㒙㒤㒥㒛㒘㒚㒞㒚㒦㒚㒚㒤㒚㒣㒝㒣㒙㒢㒥㒣㒣㒘㒗㒢㒙㒡㒥㒡㒡㒡㒞㒡㒙㒠㒥㒠㒡㒡㒟㒠㒙㒟㒥㒟㒢㒟㒝㒟㒝㒞㒥㒞㒡㒞㒝㒠㒙㒝㒥㒝㒡㒝㒞㒝㒙㒜㒦㒜㒡㒜㒠㒜㒙㒝㒗㒛㒡㒛㒝㒛㒜㒚㒥㒚㒣㒚㒝㒚㒙㒙㒥㒙㒡㒙㒝㒙㒙㒙㒙㒘㒡㒘㒞㒘㒙㒗㒥㒗㒡㒗㒝㒗㒙㒦㒥㒦㒢㒦㒝㒦㒝㒥㒥㒥㒡㒥㒝㒥㒙㒤㒥㒤㒡㒤㒝㒤㒙㒣㒥㒣㒡㒣㒟㒣㒙㒢㒥㒢㒡㒢㒝㒢㒙㒡㒥㒡㒢㒡㒝㒡㒚㒠㒥㒠㒡㒠㒝㒠㒙㒟㒥㒟㒡㒟㒞㒟㒙㒞㒥㒞㒡㒞㒝㒞㒟㒝㒥㒝㒡㒝㒝㒢㒝㒝㒝㒜㒡㒜㒝㒜㒙㒠㒞㒢㒟㒢㒠㒢㒝㒠㒦㒡㒟㒠㒠㒠㒞㒗㒗㒙㒤㒙㒝㒙㒙㒘㒥㒟㒟㒞㒢㒟㒠㒗㒥㒘㒘㒗㒝㒗㒙㒦㒥㒚㒤㒝㒜㒝㒗㒜㒣㒛㒦㒛㒠㒜㒝㒜㒣㒥㒢㒤㒝㒤㒙㒣㒥㒘㒞㒚㒜㒚㒞㒚㒘㒘㒦㒦㒟㒙㒞㒙㒙㒘㒥㒘㒜㒘㒗㒣㒦㒤㒤㒗㒙㒦㒢㒦㒘㒦㒜㒙㒥㒟㒟㒞㒥㒞㒡㒞㒝㒣㒙㒣㒦㒤㒣㒣㒢㒤㒗㒤㒙㒡㒥㒝㒘㒜㒙㒛㒥㒛㒡㒠㒙㒢㒘㒡㒘㒠㒢㒡㒙㒟㒜㒠㒘㒠㒣㒟㒦㒠㒙㒠㒙㒙㒜㒘㒝㒘㒙㒗㒥㒘㒣㒠㒢㒗㒙㒦㒥㒦㒡㒦㒞㒦㒙㒥㒥㒥㒡㒗㒝㒥㒙㒤㒥㒤㒡㒤㒝㒤㒙㒣㒥㒣㒣㒣㒝㒤㒛㒢㒥㒢㒡㒢㒞㒢㒙㒢㒛㒡㒡㒡㒝㒡㒙㒠㒥㒠㒡㒠㒝㒠㒛㒟㒥㒟㒡㒟㒝㒟㒙㒞㒥㒞㒡㒞㒝㒞㒙㒝㒥㒝㒡㒝㒟㒝㒙㒝㒗㒜㒡㒞㒝㒜㒙㒛㒥㒛㒢㒛㒝㒛㒙㒚㒥㒚㒦㒚㒝㒜㒙㒙㒥㒙㒡㒙㒞㒙㒙㒘㒦㒘㒡㒘㒡㒘㒙㒙㒥㒗㒡㒗㒝㒗㒚㒦㒥㒦㒢㒦㒝㒦㒜㒥㒥㒥㒣㒙㒢㒥㒙㒥㒘㒤㒡㒤㒝㒤㒙㒣㒥㒣㒡㒣㒝㒙㒢㒢㒥㒢㒢㒢㒝㒢㒜㒡㒥㒡㒢㒡㒝㒡㒙㒦㒞㒠㒡㒠㒝㒠㒙㒟㒦㒟㒡㒟㒝㒟㒙㒞㒥㒞㒢㒞㒝㒞㒙㒝㒥㒝㒢㒝㒝㒝㒙㒜㒥㒜㒡㒜㒝㒜㒙㒛㒥㒛㒥㒛㒝㒛㒙㒚㒥㒟㒥㒚㒦㒚㒙㒙㒥㒙㒡㒝㒠㒟㒥㒞㒦㒟㒤㒟㒠㒝㒗㒝㒦㒞㒞㒝㒢㒗㒜㒠㒟㒠㒚㒟㒦㒟㒢㒟㒞㒟㒚㒠㒦㒙㒘㒚㒙㒥㒠㒤㒝㒤㒙㒣㒥㒘㒡㒚㒟㒚㒘㒚㒝㒙㒚㒙㒚㒘㒢㒙㒙㒙㒚㒦㒝㒘㒛㒗㒤㒗㒞㒗㒝㒗㒝㒚㒝㒠㒝㒟㒝㒟㒙㒞㒥㒣㒙㒥㒜㒤㒥㒤㒙㒡㒥㒤㒢㒤㒛㒢㒦㒣㒥㒢㒦㒣㒘㒢㒣㒜㒗㒛㒝㒛㒙㒚㒥㒜㒡㒚㒤㒚㒙㒙㒦㒙㒡㒙㒝㒙㒙㒘㒦㒘㒡㒚㒣㒙㒟㒗㒥㒗㒢㒗㒝㒗㒝㒦㒥㒦㒢㒦㒝㒦㒜㒥㒥㒥㒥㒦㒛㒥㒙㒤㒥㒤㒡㒤㒡㒤㒙㒣㒦㒣㒡㒣㒡㒤㒗㒢㒥㒢㒡㒢㒝㒢㒞㒡㒥㒡㒢㒡㒝㒤㒙㒙㒘㒠㒡㒠㒝㒠㒙㒠㒙㒟㒡㒟㒟㒟㒙㒞㒥㒤㒚㒞㒝㒞㒙㒝㒥㒝㒢㒝㒝㒝㒙㒜㒥㒜㒢㒝㒝㒜㒙㒛㒥㒛㒡㒞㒗㒛㒣㒚㒥㒚㒡㒚㒝㒟㒙㒡㒗㒠㒠㒠㒥㒟㒢㒟㒢㒟㒚㒟㒡㒟㒢㒝㒛㒚㒛㒗㒦㒗㒙㒦㒥㒦㒡㒚㒠㒜㒥㒛㒦㒜㒤㒜㒠㒚㒗㒚㒦㒛㒞㒚㒢㒤㒙㒤㒟㒣㒡㒣㒝㒣㒙㒗㒜㒘㒦㒙㒡㒗㒜㒘㒚㒘㒣㒘㒣㒗㒢㒗㒘㒦㒦㒘㒛㒠㒠㒟㒥㒟㒡㒟㒝㒣㒜㒥㒤㒥㒟㒥㒛㒤㒞㒤㒘㒤㒥㒚㒟㒝㒟㒜㒥㒜㒡㒜㒝㒡㒙㒡㒦㒢㒣㒡㒢㒢㒗㒢㒙㒗㒥㒚㒝㒜㒥㒙㒦㒤㒜㒣㒗㒢㒢㒢㒞㒢㒚㒡㒦㒡㒢㒣㒞㒛㒠㒡㒥㒘㒘㒦㒥㒦㒡㒦㒝㒛㒙㒝㒗㒜㒠㒜㒥㒛㒢㒛㒢㒛㒚㒛㒡㒛㒢㒘㒥㒚㒣㒚㒜㒙㒦㒙㒥㒙㒥㒥㒗㒢㒞㒡㒥㒡㒡㒡㒝㒘㒙㒦㒦㒗㒚㒗㒟㒗㒜㒢㒟㒠㒘㒟㒝㒟㒙㒞㒥㒤㒗㒤㒦㒥㒜㒤㒞㒣㒣㒤㒙㒣㒞㒢㒙㒝㒝㒜㒝㒜㒙㒛㒥㒠㒙㒢㒜㒡㒥㒡㒙㒞㒥㒡㒢㒡㒛㒟㒦㒠㒥㒟㒦㒠㒘㒟㒣㒛㒛㒙㒛㒘㒙㒗㒥㒗㒡㒛㒤㒝㒞㒞㒙㒚㒥㒜㒢㒝㒜㒜㒘㒛㒦㒜㒛㒛㒝㒚㒦㒛㒟㒛㒡㒛㒜㒛㒣㒣㒥㒣㒝㒣㒙㒢㒥㒙㒘㒘㒞㒘㒦㒘㒚㒙㒟㒡㒦㒡㒙㒠㒥㒠㒡㒥㒤㒗㒘㒗㒗㒦㒜㒦㒠㒦㒙㒤㒦㒤㒤㒤㒢㒣㒝㒞㒤㒝㒡㒝㒝㒝㒙㒡㒙㒢㒦㒣㒠㒢㒜㒢㒚㒢㒟㒡㒡㒡㒚㒡㒣㒡㒥㒞㒞㒠㒝㒠㒙㒟㒦㒟㒡㒛㒙㒘㒥㒘㒡㒘㒝㒘㒙㒟㒣㒗㒡㒗㒝㒗㒙㒦㒥㒦㒡㒦㒝㒦㒙㒗㒥㒥㒡㒥㒝㒥㒙㒤㒥㒤㒡㒤㒝㒤㒞㒣㒥㒦㒡㒣㒝㒣㒙㒢㒥㒢㒡㒣㒘㒢㒙㒢㒛㒡㒡㒡㒝㒡㒙㒠㒥㒠㒡㒠㒝㒠㒙㒟㒥㒟㒡㒟㒝㒡㒙㒞㒥㒞㒡㒞㒝㒞㒙㒝㒥㒝㒡㒝㒢㒝㒙㒞㒥㒜㒡㒜㒝㒜㒙㒛㒥㒛㒡㒛㒝㒛㒞㒚㒥㒜㒡㒚㒝㒚㒙㒙㒥㒙㒡㒙㒝㒙㒙㒘㒦㒘㒡㒛㒝㒘㒙㒗㒥㒗㒡㒗㒝㒗㒤㒦㒥㒗㒘㒦㒝㒗㒛㒥㒥㒥㒡㒥㒝㒥㒙㒥㒟㒤㒡㒤㒝㒤㒙㒥㒗㒣㒡㒣㒝㒣㒚㒢㒥㒣㒟㒢㒝㒢㒙㒡㒥㒣㒡㒡㒝㒡㒙㒠㒦㒠㒡㒠㒞㒠㒙㒠㒘㒟㒡㒠㒟㒟㒙㒞㒥㒞㒤㒞㒝㒟㒘㒝㒥㒝㒡㒝㒝㒝㒙㒜㒥㒜㒡㒜㒞㒜㒙㒜㒘㒛㒡㒛㒟㒛㒙㒜㒥㒚㒡㒚㒝㒚㒚㒙㒥㒙㒢㒙㒝㒙㒦㒘㒥㒘㒡㒘㒝㒘㒙㒗㒦㒗㒡㒗㒟㒗㒙㒦㒥㒦㒡㒦㒝㒦㒙㒥㒥㒥㒡㒥㒝㒥㒙㒤㒥㒤㒣㒤㒝㒤㒝㒣㒥㒣㒡㒣㒝㒣㒙㒤㒚㒢㒡㒢㒞㒢㒙㒣㒥㒢㒘㒡㒝㒡㒞㒠㒥㒠㒥㒠㒝㒠㒛㒟㒥㒢㒗㒗㒗㒟㒙㒟㒚㒞㒡㒟㒢㒞㒙㒝㒦㒝㒡㒝㒦㒝㒙㒝㒙㒝㒟㒜㒝㒜㒙㒛㒥㒜㒦㒛㒝㒛㒚㒚㒥㒝㒡㒢㒠㒚㒙㒚㒙㒙㒡㒚㒙㒙㒙㒙㒝㒘㒡㒘㒣㒙㒥㒗㒥㒗㒡㒗㒝㒘㒚㒦㒥㒦㒢㒦㒝㒦㒛㒥㒥㒥㒥㒦㒛㒥㒙㒤㒥㒤㒡㒥㒞㒤㒙㒣㒦㒣㒡㒤㒟㒚㒠㒢㒥㒢㒡㒢㒝㒣㒗㒡㒥㒡㒡㒡㒝㒣㒙㒢㒤㒠㒡㒠㒝㒠㒙㒟㒥㒟㒡㒟㒠㒟㒙㒠㒗㒞㒡㒞㒝㒞㒛㒝㒥㒞㒠㒝㒝㒝㒙㒜㒥㒜㒡㒜㒝㒜㒙㒛㒥㒛㒡㒛㒟㒛㒙㒛㒗㒚㒡㒜㒝㒚㒙㒙㒥㒙㒡㒙㒝㒙㒙㒘㒥㒙㒡㒘㒝㒚㒙㒗㒥㒗㒡㒗㒝㒗㒙㒦㒥㒦㒡㒦㒡㒦㒙㒦㒗㒙㒦㒥㒝㒥㒛㒤㒥㒤㒡㒤㒝㒤㒙㒣㒥㒣㒡㒙㒦㒣㒙㒢㒥㒢㒡㒢㒟㒢㒙㒡㒦㒡㒡㒡㒝㒦㒢㒠㒥㒠㒡㒠㒝㒠㒚㒟㒥㒟㒡㒟㒝㒟㒙㒟㒛㒞㒡㒞㒝㒞㒙㒛㒗㒝㒤㒝㒝㒝㒙㒜㒥㒣㒟㒢㒢㒣㒠㒞㒟㒜㒜㒛㒝㒛㒙㒚㒥㒟㒝㒡㒜㒠㒜㒟㒦㒠㒝㒞㒠㒟㒜㒠㒗㒟㒚㒟㒝㒟㒝㒢㒝㒘㒢㒗㒝㒗㒙㒦㒥㒛㒞㒝㒜㒝㒞㒝㒘㒛㒦㒙㒟㒜㒞㒜㒙㒛㒥㒛㒜㒛㒗㒦㒦㒗㒤㒚㒙㒙㒢㒙㒘㒙㒜㒚㒛㒢㒡㒡㒥㒡㒡㒡㒝㒥㒢㒗㒣㒗㒤㒗㒡㒦㒚㒦㒣㒥㒤㒥㒢㒡㒣㒟㒛㒞㒡㒞㒝㒞㒙㒢㒥㒣㒢㒤㒟㒣㒞㒣㒣㒣㒥㒦㒥㒜㒠㒛㒥㒛㒡㒛㒝㒟㒜㒡㒤㒡㒟㒡㒛㒠㒞㒠㒘㒠㒥㒚㒙㒙㒙㒘㒥㒘㒡㒙㒟㒡㒞㒗㒥㒗㒡㒗㒝㒗㒝㒦㒥㒦㒡㒦㒝㒘㒙㒥㒥㒥㒡㒥㒝㒥㒙㒤㒥㒤㒡㒤㒞㒤㒙㒥㒗㒣㒡㒣㒝㒣㒚㒢㒥㒢㒣㒢㒝㒢㒙㒡㒥㒡㒡㒡㒝㒡㒙㒡㒗㒠㒡㒠㒝㒠㒙㒟㒥㒟㒡㒟㒝㒟㒙㒞㒥㒞㒡㒞㒝㒞㒛㒝㒥㒝㒣㒝㒝㒟㒙㒜㒥㒜㒡㒜㒞㒜㒙㒛㒥㒛㒡㒛㒢㒛㒙㒜㒥㒚㒡㒚㒝㒚㒚㒙㒥㒙㒢㒙㒝㒙㒜㒘㒥㒚㒡㒘㒝㒘㒙㒗㒦㒗㒡㒗㒞㒗㒙㒗㒛㒦㒡㒦㒣㒦㒝㒥㒥㒥㒤㒥㒝㒥㒙㒤㒥㒤㒢㒤㒝㒤㒚㒣㒥㒣㒡㒦㒥㒣㒙㒢㒥㒢㒡㒢㒝㒢㒙㒡㒥㒡㒡㒡㒝㒗㒢㒠㒥㒠㒢㒠㒝㒠㒜㒟㒥㒟㒢㒟㒝㒟㒙㒤㒞㒞㒡㒞㒝㒞㒙㒝㒦㒝㒡㒝㒝㒝㒙㒜㒥㒜㒢㒜㒝㒜㒙㒛㒥㒛㒢㒛㒝㒛㒙㒚㒥㒚㒡㒚㒝㒚㒙㒙㒥㒙㒥㒙㒝㒙㒙㒘㒥㒣㒙㒘㒦㒘㒙㒗㒥㒗㒡㒛㒠㒝㒥㒜㒦㒝㒤㒝㒠㒛㒗㒛㒦㒜㒞㒛㒢㒗㒣㒥㒡㒤㒡㒤㒝㒤㒙㒘㒝㒚㒠㒚㒙㒙㒝㒗㒙㒙㒦㒙㒟㒘㒚㒙㒙㒘㒚㒘㒜㒘㒗㒡㒘㒠㒡㒠㒝㒠㒙㒟㒥㒟㒡㒟㒝㒠㒙㒢㒥㒛㒣㒟㒜㒞㒙㒝㒥㒝㒡㒢㒝㒤㒛㒣㒤㒤㒙㒢㒦㒢㒦㒢㒞㒢㒥㒢㒦㒠㒙㒢㒗㒡㒠㒡㒚㒡㒙㒡㒙㒚㒗㒙㒝㒙㒙㒘㒥㒚㒡㒘㒤㒘㒙㒗㒦㒗㒡㒗㒝㒗㒙㒦㒦㒦㒡㒘㒣㒗㒟㒥㒥㒥㒢㒥㒝㒥㒝㒤㒥㒤㒢㒤㒝㒤㒝㒣㒥㒣㒥㒤㒛㒣㒙㒢㒥㒢㒡㒢㒡㒢㒙㒡㒦㒡㒡㒡㒡㒢㒗㒠㒥㒠㒡㒠㒝㒠㒞㒟㒥㒟㒢㒟㒝㒢㒙㒗㒘㒞㒡㒞㒝㒞㒙㒞㒗㒝㒡㒝㒠㒝㒙㒜㒥㒢㒚㒜㒝㒜㒙㒛㒥㒛㒢㒛㒝㒛㒙㒚㒥㒚㒢㒛㒝㒚㒙㒙㒥㒙㒡㒦㒟㒚㒗㒘㒥㒘㒡㒘㒝㒜㒠㒞㒚㒞㒥㒛㒡㒝㒞㒞㒘㒜㒤㒜㒢㒝㒗㒜㒙㒛㒢㒜㒛㒜㒝㒜㒘㒜㒟㒤㒣㒤㒙㒣㒥㒣㒡㒘㒝㒙㒚㒚㒗㒘㒦㒙㒛㒙㒝㒤㒢㒡㒡㒡㒝㒡㒙㒠㒥㒠㒡㒠㒝㒡㒙㒣㒥㒟㒡㒟㒡㒟㒙㒞㒥㒞㒡㒤㒤㒤㒚㒤㒢㒣㒦㒢㒡㒝㒢㒜㒥㒜㒡㒜㒝㒡㒠㒢㒤㒢㒣㒢㒘㒢㒜㒡㒥㒠㒢㒠㒠㒠㒞㒤㒝㒚㒘㒙㒝㒙㒙㒘㒥㒜㒤㒟㒜㒟㒗㒞㒣㒝㒦㒝㒠㒞㒝㒜㒙㒗㒝㒦㒝㒦㒙㒥㒥㒚㒙㒜㒜㒛㒥㒛㒙㒘㒥㒛㒢㒛㒛㒙㒦㒚㒥㒙㒦㒚㒘㒙㒣㒘㒗㒢㒝㒤㒣㒢㒤㒡㒡㒡㒝㒡㒙㒥㒥㒗㒣㒗㒜㒗㒡㒦㒞㒦㒞㒥㒦㒦㒝㒦㒞㒣㒡㒥㒟㒥㒘㒤㒢㒤㒡㒤㒡㒝㒙㒝㒤㒜㒡㒜㒝㒜㒙㒠㒙㒡㒦㒢㒠㒡㒜㒡㒚㒡㒟㒠㒡㒠㒚㒠㒣㒠㒥㒝㒞㒟㒝㒟㒙㒞㒦㒞㒡㒥㒛㒘㒚㒗㒡㒗㒝㒗㒙㒝㒥㒜㒢㒜㒦㒝㒛㒝㒘㒛㒗㒥㒞㒥㒙㒥㒟㒤㒡㒤㒝㒤㒙㒘㒜㒙㒦㒚㒡㒘㒜㒙㒚㒙㒣㒙㒣㒘㒢㒘㒘㒗㒦㒡㒝㒡㒢㒠㒥㒠㒡㒠㒝㒤㒜㒦㒡㒥㒢㒦㒠㒦㒜㒣㒣㒤㒢㒥㒚㒤㒞㒝㒥㒞㒚㒝㒝㒝㒙㒜㒥㒡㒡㒣㒟㒣㒘㒣㒝㒢㒚㒢㒚㒡㒢㒢㒙㒢㒚㒗㒟㒚㒠㒙㒥㒙㒡㒙㒝㒞㒟㒟㒞㒟㒤㒞㒦㒞㒛㒞㒡㒝㒦㒙㒝㒗㒙㒦㒥㒦㒡㒦㒝㒞㒗㒥㒥㒥㒡㒥㒝㒥㒙㒤㒥㒤㒡㒤㒝㒦㒙㒣㒥㒣㒡㒣㒝㒣㒙㒢㒥㒢㒡㒢㒟㒢㒙㒤㒥㒡㒡㒡㒝㒡㒙㒠㒥㒡㒡㒠㒝㒠㒡㒟㒥㒟㒡㒟㒝㒟㒙㒞㒥㒞㒡㒞㒝㒞㒙㒝㒥㒝㒡㒟㒝㒝㒙㒜㒥㒜㒡㒜㒝㒜㒙㒛㒥㒛㒣㒛㒝㒝㒙㒚㒥㒚㒡㒚㒝㒚㒙㒙㒥㒙㒡㒙㒟㒙㒙㒚㒥㒘㒡㒘㒝㒘㒙㒗㒥㒗㒡㒗㒝㒘㒘㒦㒥㒙㒡㒦㒝㒦㒙㒥㒥㒥㒡㒦㒝㒥㒙㒥㒡㒤㒡㒥㒟㒤㒙㒣㒥㒣㒡㒣㒝㒣㒤㒢㒥㒢㒡㒢㒝㒣㒛㒡㒥㒡㒡㒡㒞㒡㒙㒡㒙㒠㒡㒠㒝㒠㒙㒡㒥㒟㒡㒟㒝㒟㒚㒞㒥㒞㒢㒞㒝㒞㒦㒝㒥㒞㒣㒝㒝㒝㒙㒝㒘㒜㒡㒜㒢㒜㒙㒛㒥㒛㒡㒛㒝㒛㒙㒚㒥㒚㒢㒚㒝㒚㒜㒙㒥㒙㒣㒙㒝㒛㒙㒘㒥㒘㒡㒘㒞㒘㒙㒗㒦㒗㒡㒗㒞㒗㒙㒦㒥㒦㒡㒦㒝㒦㒚㒥㒥㒥㒣㒥㒝㒥㒙㒤㒥㒤㒡㒤㒝㒤㒙㒣㒥㒣㒡㒣㒝㒣㒙㒣㒗㒢㒡㒢㒡㒢㒙㒡㒥㒡㒡㒡㒝㒢㒞㒠㒥㒠㒢㒠㒝㒢㒙㒠㒜㒟㒡㒟㒢㒟㒙㒟㒙㒞㒡㒟㒛㒞㒙㒠㒛㒥㒛㒝㒝㒝㒞㒜㒥㒝㒦㒜㒝㒜㒚㒛㒥㒜㒚㒛㒝㒛㒝㒛㒣㒚㒡㒚㒝㒚㒙㒛㒚㒙㒡㒙㒞㒙㒙㒛㒥㒠㒤㒘㒝㒘㒝㒗㒥㒘㒘㒗㒝㒗㒜㒦㒥㒗㒗㒘㒙㒦㒙㒥㒥㒥㒡㒦㒞㒥㒙㒤㒦㒤㒡㒤㒟㒤㒙㒤㒙㒤㒟㒣㒝㒣㒙㒢㒥㒣㒢㒢㒝㒢㒚㒡㒥㒢㒣㒘㒤㒡㒙㒠㒥㒠㒡㒠㒡㒠㒙㒟㒥㒟㒡㒡㒝㒡㒘㒞㒥㒞㒡㒞㒝㒞㒙㒝㒥㒞㒞㒝㒝㒞㒛㒜㒥㒜㒡㒜㒟㒜㒙㒜㒚㒛㒡㒛㒝㒛㒙㒚㒥㒚㒡㒚㒝㒚㒙㒙㒥㒙㒣㒙㒝㒙㒛㒘㒥㒚㒡㒘㒝㒘㒙㒗㒥㒗㒡㒗㒝㒗㒙㒗㒟㒦㒡㒘㒝㒦㒙㒥㒥㒥㒡㒥㒝㒥㒙㒤㒥㒥㒗㒤㒝㒤㒛㒘㒚㒣㒡㒣㒟㒣㒙㒢㒥㒢㒡㒢㒝㒢㒙㒡㒥㒘㒚㒡㒝㒡㒙㒠㒥㒠㒣㒠㒝㒠㒚㒟㒥㒟㒡㒤㒦㒟㒙㒞㒥㒞㒡㒞㒞㒞㒙㒝㒥㒝㒡㒝㒝㒝㒟㒜㒥㒜㒡㒜㒝㒦㒡㒜㒦㒛㒡㒛㒝㒛㒙㒟㒢㒡㒠㒡㒢㒡㒜㒠㒚㒝㒣㒠㒢㒠㒝㒠㒙㒟㒠㒟㒛㒛㒚㒜㒘㒞㒝㒝㒦㒝㒜㒝㒠㒦㒡㒗㒘㒦㒙㒥㒥㒥㒡㒚㒙㒜㒘㒛㒘㒚㒢㒛㒙㒙㒜㒚㒘㒚㒣㒙㒦㒚㒙㒚㒙㒥㒛㒢㒥㒢㒙㒡㒥㒡㒡㒥㒦㒘㒗㒘㒘㒗㒥㒦㒞㒗㒗㒦㒘㒥㒦㒜㒟㒟㒟㒞㒥㒞㒡㒞㒝㒣㒙㒣㒦㒤㒣㒣㒢㒤㒗㒤㒙㒤㒟㒜㒤㒜㒙㒛㒥㒛㒡㒟㒠㒢㒘㒡㒣㒡㒟㒠㒢㒠㒜㒡㒙㒞㒥㒙㒠㒙㒙㒘㒥㒘㒡㒟㒛㒞㒞㒟㒜㒘㒝㒗㒝㒗㒙㒦㒥㒗㒣㒟㒢㒦㒙㒥㒥㒥㒡㒥㒠㒥㒙㒤㒥㒤㒡㒦㒝㒤㒙㒣㒥㒣㒡㒣㒝㒣㒙㒢㒥㒣㒗㒢㒝㒣㒛㒡㒥㒡㒡㒡㒞㒡㒙㒡㒗㒠㒡㒠㒝㒠㒙㒟㒥㒟㒡㒟㒝㒟㒛㒞㒥㒞㒡㒞㒝㒞㒙㒝㒥㒝㒡㒝㒝㒝㒙㒜㒥㒜㒡㒜㒟㒜㒙㒜㒗㒛㒡㒝㒝㒛㒙㒚㒥㒚㒢㒚㒝㒚㒙㒙㒥㒙㒥㒙㒝㒛㒙㒘㒥㒘㒡㒘㒞㒘㒙㒗㒦㒗㒡㒗㒞㒗㒙㒘㒥㒦㒡㒦㒝㒦㒚㒥㒥㒥㒢㒥㒝㒥㒞㒤㒥㒥㒗㒤㒡㒤㒙㒤㒘㒣㒡㒣㒝㒣㒙㒢㒦㒢㒡㒢㒞㒢㒙㒡㒥㒥㒙㒡㒝㒡㒙㒠㒥㒠㒡㒠㒝㒠㒙㒟㒥㒟㒡㒥㒦㒟㒙㒞㒦㒞㒡㒞㒠㒞㒙㒝㒦㒝㒡㒝㒝㒢㒢㒜㒥㒜㒡㒜㒝㒜㒚㒛㒥㒛㒡㒛㒝㒛㒙㒚㒦㒚㒡㒚㒝㒚㒙㒙㒥㒙㒡㒙㒝㒙㒙㒙㒡㒘㒡㒘㒝㒘㒙㒗㒥㒘㒛㒗㒝㒗㒙㒦㒥㒛㒘㒜㒢㒝㒝㒛㒘㒛㒦㒜㒟㒜㒟㒛㒞㒚㒤㒚㒢㒙㒝㒤㒦㒣㒡㒣㒝㒣㒙㒗㒘㒗㒚㒤㒝㒙㒥㒣㒥㒥㒤㒗㒦㒗㒝㒦㒦㒦㒥㒜㒠㒚㒜㒦㒤㒡㒡㒣㒟㒤㒗㒣㒡㒣㒥㒟㒙㒞㒙㒝㒥㒝㒡㒢㒣㒣㒢㒤㒗㒢㒢㒣㒟㒠㒥㒢㒞㒣㒙㒡㒢㒡㒢㒢㒗㒡㒠㒝㒗㒚㒠㒙㒥㒙㒡㒙㒝㒞㒟㒟㒞㒟㒤㒞㒦㒞㒛㒞㒡㒝㒦㒜㒡㒗㒣㒦㒥㒦㒡㒦㒝㒚㒟㒜㒞㒜㒣㒛㒢㒚㒜㒛㒚㒛㒣㒛㒣㒚㒞㒛㒗㒞㒙㒤㒞㒣㒙㒢㒥㒢㒡㒗㒟㒘㒞㒘㒥㒘㒝㒗㒦㒗㒜㒦㒦㒗㒥㒦㒢㒦㒝㒥㒘㒦㒥㒦㒜㒦㒛㒤㒦㒥㒘㒤㒢㒣㒟㒝㒦㒥㒟㒝㒣㒝㒙㒜㒥㒜㒡㒡㒝㒢㒚㒣㒗㒡㒦㒢㒛㒢㒝㒢㒣㒛㒞㒚㒝㒚㒙㒙㒥㒝㒣㒟㒞㒟㒠㒠㒚㒟㒝㒞㒥㒟㒘㒝㒗㒝㒦㒞㒚㒞㒘㒞㒙㒜㒦㒣㒡㒦㒙㒝㒣㒦㒙㒥㒝㒥㒙㒤㒥㒙㒥㒛㒟㒚㒚㒚㒗㒙㒢㒚㒙㒙㒡㒙㒤㒢㒡㒢㒡㒢㒙㒡㒥㒡㒡㒗㒤㒗㒚㒗㒢㒦㒦㒡㒟㒠㒙㒟㒥㒟㒡㒟㒝㒢㒦㒞㒥㒞㒡㒞㒝㒞㒙㒝㒥㒝㒡㒝㒝㒟㒙㒜㒥㒜㒡㒜㒝㒜㒙㒛㒥㒛㒡㒛㒥㒛㒙㒝㒥㒚㒡㒚㒝㒚㒙㒙㒥㒙㒥㒙㒝㒙㒣㒘㒥㒘㒡㒘㒝㒘㒙㒗㒥㒗㒡㒗㒝㒗㒙㒦㒥㒦㒡㒘㒝㒦㒙㒥㒥㒥㒡㒥㒝㒥㒙㒤㒥㒥㒙㒤㒝㒦㒙㒣㒥㒣㒡㒣㒝㒣㒙㒢㒥㒢㒡㒢㒥㒢㒙㒣㒥㒡㒡㒡㒝㒡㒙㒠㒥㒠㒡㒠㒝㒠㒜㒟㒥㒢㒡㒟㒝㒟㒙㒞㒥㒞㒡㒞㒡㒞㒙㒞㒜㒝㒡㒞㒟㒝㒙㒜㒥㒜㒡㒜㒝㒜㒥㒛㒥㒛㒡㒛㒝㒝㒙㒚㒥㒚㒡㒚㒝㒚㒙㒙㒥㒙㒡㒙㒞㒙㒙㒚㒗㒘㒡㒘㒝㒘㒛㒗㒥㒘㒗㒗㒝㒗㒙㒦㒥㒦㒡㒦㒝㒦㒙㒥㒥㒥㒡㒥㒟㒥㒙㒥㒗㒤㒡㒦㒝㒤㒙㒣㒥㒣㒡㒣㒝㒣㒙㒢㒥㒣㒚㒢㒝㒤㒙㒡㒥㒡㒡㒡㒝㒡㒙㒠㒥㒠㒡㒡㒘㒠㒙㒡㒥㒟㒡㒟㒝㒟㒙㒞㒥㒞㒡㒞㒝㒞㒞㒝㒥㒞㒣㒝㒝㒝㒙㒝㒗㒜㒡㒜㒟㒜㒙㒛㒥㒛㒡㒛㒝㒛㒙㒚㒥㒚㒡㒚㒝㒚㒛㒙㒥㒙㒢㒙㒝㒙㒙㒘㒥㒘㒡㒘㒝㒘㒙㒗㒦㒗㒡㒗㒝㒗㒙㒦㒥㒗㒗㒦㒝㒦㒙㒥㒥㒥㒡㒥㒣㒥㒙㒤㒥㒤㒡㒙㒝㒚㒚㒛㒗㒙㒦㒚㒛㒚㒝㒚㒣㒣㒙㒢㒝㒢㒙㒡㒥㒦㒚㒘㒛㒘㒜㒘㒙㒦㒢㒗㒛㒦㒜㒦㒚㒗㒟㒟㒠㒟㒙㒞㒥㒞㒡㒥㒛㒤㒞㒥㒜㒘㒙㒞㒘㒝㒙㒜㒥㒜㒡㒡㒙㒣㒘㒢㒘㒡㒢㒢㒙㒠㒜㒡㒘㒡㒣㒠㒦㒡㒙㒡㒙㒤㒙㒙㒤㒙㒙㒘㒥㒘㒡㒜㒠㒟㒘㒞㒣㒞㒟㒝㒢㒝㒜㒞㒙㒛㒥㒗㒞㒦㒙㒥㒥㒥㒡㒚㒚㒜㒘㒜㒚㒛㒤㒚㒢㒘㒛㒛㒚㒚㒥㒚㒡㒚㒘㒙㒣㒥㒢㒦㒠㒘㒥㒘㒞㒗㒤㒘㒘㒡㒥㒠㒥㒠㒡㒠㒝㒡㒛㒙㒚㒟㒡㒟㒝㒟㒙㒟㒗㒞㒡㒞㒝㒞㒙㒟㒥㒝㒡㒝㒝㒝㒙㒜㒥㒜㒡㒜㒝㒜㒜㒛㒥㒜㒣㒛㒝㒛㒙㒚㒦㒚㒡㒚㒡㒚㒙㒙㒥㒙㒡㒙㒝㒙㒙㒘㒥㒘㒣㒘㒝㒘㒙㒗㒥㒗㒡㒗㒝㒗㒙㒦㒥㒦㒡㒦㒝㒦㒙㒦㒗㒥㒡㒥㒟㒥㒙㒦㒥㒤㒡㒤㒝㒤㒚㒣㒥㒣㒡㒣㒝㒣㒚㒢㒥㒤㒡㒢㒝㒢㒙㒡㒦㒡㒡㒡㒞㒡㒙㒡㒛㒠㒡㒢㒝㒠㒙㒟㒥㒟㒢㒟㒝㒟㒚㒞㒥㒞㒦㒞㒝㒞㒟㒞㒙㒝㒡㒝㒠㒝㒙㒜㒥㒜㒡㒜㒞㒜㒙㒛㒦㒛㒡㒛㒝㒞㒡㒚㒥㒚㒡㒚㒝㒚㒙㒙㒥㒙㒡㒙㒝㒙㒙㒟㒞㒘㒡㒘㒞㒘㒙㒘㒘㒗㒡㒗㒞㒗㒙㒦㒥㒜㒚㒦㒝㒦㒙㒥㒥㒥㒢㒥㒝㒥㒙㒤㒥㒤㒡㒤㒞㒤㒙㒣㒥㒣㒡㒣㒝㒣㒙㒢㒥㒢㒡㒢㒣㒢㒙㒡㒥㒡㒡㒡㒝㒡㒟㒠㒥㒠㒡㒠㒝㒥㒜㒦㒤㒦㒦㒦㒟㒥㒜㒥㒚㒛㒣㒟㒗㒞㒙㒝㒥㒝㒡㒤㒙㒤㒘㒢㒦㒢㒥㒣㒠㒣㒝㒣㒗㒢㒚㒢㒛㒡㒠㒝㒟㒚㒥㒚㒝㒚㒙㒙㒥㒠㒘㒟㒞㒟㒦㒟㒚㒝㒥㒙㒗㒘㒙㒗㒥㒗㒡㒛㒤㒝㒞㒞㒙㒛㒠㒜㒟㒜㒣㒜㒚㒛㒤㒜㒡㒜㒜㒚㒙㒦㒗㒤㒝㒤㒙㒣㒥㒚㒣㒙㒟㒚㒡㒘㒦㒙㒤㒙㒠㒘㒞㒙㒙㒘㒚㒗㒡㒤㒣㒣㒤㒣㒠㒣㒡㒣㒚㒣㒝㒣㒚㒢㒢㒢㒠㒢㒘㒡㒥㒡㒞㒣㒠㒝㒥㒝㒡㒝㒝㒝㒙㒜㒥㒜㒡㒛㒝㒠㒘㒜㒟㒛㒡㒛㒝㒛㒙㒜㒗㒞㒤㒚㒝㒚㒙㒙㒥㒙㒣㒙㒝㒙㒙㒘㒥㒙㒣㒘㒝㒘㒙㒗㒦㒗㒡㒗㒠㒗㒙㒦㒥㒦㒡㒘㒝㒦㒙㒥㒥㒥㒢㒥㒝㒥㒚㒤㒥㒤㒥㒤㒝㒥㒛㒣㒥㒣㒡㒣㒠㒣㒙㒣㒚㒢㒡㒢㒝㒢㒙㒡㒥㒡㒡㒡㒝㒡㒚㒠㒥㒠㒤㒠㒝㒠㒛㒟㒥㒡㒡㒟㒝㒟㒙㒞㒦㒞㒡㒞㒞㒞㒙㒞㒛㒝㒡㒟㒝㒝㒙㒜㒥㒜㒢㒜㒝㒜㒚㒛㒥㒛㒢㒛㒝㒛㒙㒚㒥㒚㒡㒚㒝㒚㒙㒚㒗㒙㒡㒙㒟㒙㒙㒘㒥㒘㒡㒘㒝㒘㒙㒗㒥㒗㒢㒗㒝㒗㒚㒦㒥㒦㒡㒦㒝㒦㒙㒥㒥㒥㒡㒥㒞㒥㒙㒤㒥㒤㒡㒤㒝㒤㒟㒣㒥㒣㒡㒣㒝㒣㒙㒣㒛㒢㒡㒢㒝㒢㒙㒦㒥㒗㒢㒘㒟㒗㒞㒗㒣㒗㒥㒘㒛㒠㒡㒟㒥㒟㒡㒟㒝㒣㒢㒥㒣㒥㒤㒥㒡㒤㒚㒤㒣㒣㒤㒣㒢㒥㒗㒝㒜㒜㒡㒜㒝㒜㒙㒠㒘㒢㒠㒢㒛㒢㒗㒡㒚㒠㒤㒡㒡㒜㒣㒚㒘㒙㒡㒙㒝㒙㒙㒟㒣㒞㒦㒟㒤㒘㒙㒘㒠㒗㒡㒗㒝㒗㒙㒛㒡㒝㒠㒜㒠㒜㒚㒜㒡㒚㒤㒛㒠㒜㒛㒛㒞㒛㒡㒛㒡㒜㒗㒤㒦㒣㒡㒣㒝㒣㒙㒗㒢㒙㒠㒙㒢㒙㒜㒘㒚㒥㒣㒘㒢㒘㒝㒘㒙㒗㒠㒗㒛㒣㒚㒤㒘㒦㒝㒥㒦㒥㒜㒥㒠㒟㒜㒞㒝㒞㒙㒝㒥㒞㒣㒦㒢㒝㒙㒜㒥㒜㒡㒜㒟㒜㒙㒛㒥㒛㒡㒝㒝㒛㒙㒚㒥㒚㒡㒚㒝㒚㒙㒙㒥㒙㒥㒙㒝㒚㒛㒘㒥㒘㒡㒘㒞㒘㒙㒘㒚㒗㒡㒗㒝㒗㒙㒦㒥㒦㒡㒦㒝㒦㒛㒥㒥㒥㒡㒥㒝㒥㒙㒤㒥㒤㒡㒤㒝㒤㒙㒣㒥㒣㒡㒣㒟㒣㒙㒣㒗㒢㒡㒤㒝㒢㒙㒡㒥㒡㒢㒡㒝㒡㒙㒠㒥㒠㒢㒠㒝㒢㒙㒟㒥㒟㒡㒟㒞㒟㒙㒞㒦㒞㒡㒞㒣㒞㒙㒟㒥㒝㒡㒝㒝㒝㒚㒜㒥㒜㒢㒜㒝㒜㒜㒛㒥㒛㒣㒟㒢㒛㒙㒛㒘㒚㒡㒚㒝㒚㒙㒙㒥㒙㒡㒙㒝㒟㒢㒘㒥㒘㒢㒘㒝㒘㒜㒗㒥㒗㒢㒗㒝㒗㒙㒜㒞㒦㒡㒦㒝㒦㒙㒥㒦㒥㒡㒥㒝㒥㒙㒤㒥㒤㒢㒤㒝㒤㒙㒣㒥㒣㒡㒣㒝㒣㒙㒢㒥㒢㒥㒢㒝㒢㒙㒡㒥㒞㒣㒡㒡㒡㒙㒠㒥㒠㒡㒦㒤㒦㒚㒦㒢㒥㒦㒟㒝㒟㒣㒞㒥㒞㒡㒞㒝㒤㒥㒤㒤㒣㒢㒣㒡㒤㒜㒤㒙㒣㒣㒢㒦㒣㒗㒢㒜㒞㒛㒟㒟㒛㒙㒚㒥㒚㒡㒠㒥㒡㒝㒡㒙㒠㒡㒠㒠㒜㒣㒛㒤㒛㒠㒟㒟㒞㒚㒟㒜㒚㒟㒝㒤㒝㒢㒞㒙㒝㒙㒝㒢㒜㒛㒝㒚㒜㒤㒛㒢㒜㒛㒛㒘㒛㒠㒛㒛㒛㒝㒚㒚㒚㒟㒚㒡㒦㒗㒙㒘㒙㒠㒙㒚㒥㒘㒗㒘㒘㒚㒘㒙㒗㒚㒗㒣㒦㒥㒣㒡㒣㒞㒣㒚㒢㒢㒢㒜㒥㒦㒦㒚㒥㒤㒤㒦㒤㒜㒠㒤㒤㒞㒣㒞㒣㒢㒣㒣㒟㒠㒣㒚㒣㒞㒣㒘㒢㒚㒡㒠㒞㒚㒝㒣㒡㒝㒡㒢㒠㒚㒡㒣㒚㒘㒙㒝㒙㒙㒘㒥㒝㒙㒟㒡㒟㒝㒞㒥㒜㒘㒝㒢㒞㒝㒗㒝㒦㒡㒦㒝㒦㒙㒗㒗㒚㒘㒥㒝㒥㒙㒤㒥㒤㒣㒤㒝㒤㒙㒣㒥㒤㒣㒣㒝㒣㒙㒢㒦㒢㒡㒢㒞㒢㒙㒡㒥㒡㒡㒣㒝㒡㒙㒠㒥㒠㒢㒠㒝㒠㒚㒟㒥㒟㒥㒟㒝㒠㒛㒞㒥㒞㒡㒞㒠㒞㒙㒞㒘㒝㒡㒝㒝㒝㒙㒜㒥㒜㒡㒜㒝㒜㒚㒛㒥㒛㒤㒛㒝㒛㒙㒚㒥㒚㒡㒚㒝㒚㒙㒙㒥㒙㒡㒙㒝㒙㒙㒙㒗㒘㒡㒘㒝㒘㒙㒗㒥㒗㒡㒗㒝㒗㒚㒦㒥㒦㒢㒦㒝㒦㒙㒥㒥㒥㒡㒥㒝㒥㒙㒤㒦㒤㒡㒤㒝㒤㒙㒣㒥㒤㒗㒣㒝㒣㒙㒢㒥㒗㒥㒢㒣㒢㒙㒡㒥㒡㒡㒦㒝㒗㒚㒘㒗㒦㒦㒗㒛㒗㒝㒝㒗㒟㒤㒟㒝㒟㒙㒞㒥㒥㒟㒤㒢㒥㒠㒥㒣㒞㒜㒝㒝㒝㒙㒜㒥㒡㒝㒣㒜㒢㒜㒡㒦㒢㒝㒠㒠㒡㒜㒢㒗㒡㒚㒡㒝㒡㒝㒜㒟㒚㒙㒙㒝㒙㒙㒘㒥㒝㒚㒟㒛㒟㒜㒟㒙㒝㒢㒞㒛㒝㒜㒝㒚㒛㒥㒗㒞㒦㒙㒥㒥㒥㒡㒚㒚㒜㒘㒜㒚㒛㒤㒚㒢㒘㒛㒛㒚㒚㒥㒚㒡㒚㒘㒙㒣㒥㒢㒦㒠㒘㒥㒘㒞㒗㒤㒘㒘㒙㒗㒡㒜㒠㒡㒠㒝㒠㒙㒤㒘㒦㒠㒦㒛㒦㒗㒥㒚㒤㒤㒥㒡㒞㒤㒝㒥㒝㒡㒝㒝㒞㒛㒦㒚㒜㒡㒜㒝㒜㒙㒜㒙㒛㒡㒛㒝㒛㒙㒜㒥㒚㒡㒚㒝㒚㒙㒙㒥㒙㒡㒙㒝㒙㒛㒘㒥㒙㒣㒘㒝㒘㒙㒗㒦㒗㒡㒗㒠㒗㒙㒦㒥㒦㒡㒦㒝㒦㒙㒥㒥㒥㒣㒥㒝㒥㒙㒤㒥㒤㒡㒤㒝㒤㒙㒣㒥㒣㒡㒣㒝㒣㒙㒣㒗㒢㒡㒢㒟㒢㒙㒣㒥㒡㒡㒡㒝㒡㒚㒠㒥㒠㒡㒠㒝㒠㒚㒟㒥㒡㒡㒟㒝㒟㒙㒞㒦㒞㒡㒞㒞㒞㒙㒞㒚㒝㒡㒟㒝㒝㒙㒜㒥㒜㒢㒜㒝㒜㒚㒛㒥㒜㒗㒛㒝㒛㒛㒟㒚㒚㒡㒚㒠㒚㒙㒙㒥㒙㒡㒙㒝㒙㒙㒘㒥㒟㒚㒘㒝㒘㒚㒗㒥㒗㒤㒗㒝㒗㒚㒦㒥㒦㒡㒛㒦㒦㒙㒥㒥㒥㒡㒥㒞㒥㒙㒤㒥㒤㒡㒤㒝㒥㒥㒣㒦㒣㒡㒣㒝㒣㒙㒣㒛㒢㒡㒢㒝㒢㒙㒦㒛㒘㒣㒗㒞㒗㒦㒗㒚㒣㒢㒚㒥㒠㒥㒟㒥㒟㒡㒟㒝㒣㒤㒥㒠㒤㒙㒥㒡㒣㒞㒣㒤㒣㒛㒡㒡㒡㒥㒡㒡㒣㒛㒠㒦㒤㒗㒜㒟㒛㒡㒛㒝㒛㒙㒡㒞㒡㒤㒡㒙㒠㒜㒠㒡㒠㒠㒠㒠㒠㒞㒠㒗㒞㒦㒥㒢㒘㒙㒗㒥㒗㒡㒗㒝㒗㒙㒞㒥㒚㒢㒚㒝㒣㒛㒥㒦㒥㒡㒥㒝㒥㒙㒙㒗㒤㒡㒤㒟㒤㒙㒣㒥㒣㒡㒘㒡㒗㒚㒢㒥㒣㒙㒢㒝㒢㒙㒡㒥㒦㒚㒘㒛㒘㒜㒘㒙㒦㒢㒗㒛㒦㒜㒦㒚㒥㒘㒟㒝㒟㒙㒞㒥㒞㒡㒞㒝㒜㒙㒤㒝㒡㒡㒢㒡㒝㒚㒜㒥㒜㒡㒜㒝㒠㒥㒙㒗㒛㒥㒛㒝㒛㒙㒚㒥㒡㒡㒠㒞㒡㒛㒡㒙㒜㒞㒦㒙㒤㒦㒠㒛㒚㒠㒛㒣㒘㒠㒤㒗㒛㒠㒤㒟㒗㒡㒦㒥㒦㒡㒦㒝㒛㒝㒜㒚㒝㒙㒜㒡㒚㒜㒛㒞㒜㒛㒚㒢㒞㒡㒤㒝㒣㒡㒣㒝㒣㒙㒘㒘㒘㒦㒙㒡㒗㒜㒘㒘㒘㒠㒘㒟㒗㒞㒛㒝㒡㒚㒠㒝㒠㒙㒟㒥㒤㒡㒦㒙㒥㒚㒦㒞㒤㒦㒥㒟㒢㒠㒥㒚㒤㒚㒝㒝㒝㒢㒜㒥㒜㒡㒜㒝㒣㒠㒡㒦㒢㒝㒢㒘㒢㒜㒡㒥㒠㒦㒠㒢㒠㒝㒡㒣㒙㒦㒙㒝㒙㒙㒘㒥㒝㒤㒞㒠㒟㒘㒟㒗㒝㒦㒤㒢㒗㒝㒦㒡㒠㒟㒞㒞㒘㒟㒥㒡㒡㒚㒙㒜㒢㒞㒙㒜㒠㒢㒙㒣㒜㒙㒦㒙㒘㒚㒠㒟㒗㒘㒣㒘㒟㒢㒗㒦㒝㒛㒛㒤㒞㒠㒙㒡㒟㒘㒤㒤㒝㒣㒠㒡㒠㒙㒟㒥㒟㒡㒤㒡㒥㒞㒦㒝㒥㒥㒡㒚㒞㒙㒝㒥㒝㒡㒝㒝㒝㒙㒛㒥㒣㒤㒠㒝㒜㒜㒛㒥㒛㒡㒛㒝㒛㒙㒚㒥㒚㒡㒝㒦㒞㒙㒟㒙㒙㒢㒙㒝㒙㒙㒘㒥㒝㒤㒥㒢㒘㒙㒗㒥㒗㒡㒗㒝㒗㒙㒤㒥㒝㒠㒚㒝㒦㒙㒦㒟㒥㒡㒥㒝㒥㒙㒙㒟㒛㒤㒛㒜㒛㒗㒘㒙㒙㒦㒙㒠㒚㒘㒙㒙㒘㒦㒗㒣㒢㒚㒜㒝㒢㒡㒡㒝㒡㒙㒠㒥㒥㒙㒗㒢㒦㒦㒥㒦㒦㒟㒦㒜㒥㒢㒥㒙㒣㒣㒥㒜㒥㒘㒥㒙㒢㒡㒣㒞㒤㒛㒤㒙㒡㒥㒜㒞㒜㒙㒛㒥㒛㒡㒟㒡㒝㒦㒞㒙㒜㒗㒢㒚㒤㒙㒝㒢㒟㒡㒦㒣㒝㒘㒣㒝㒚㒗㒘㒝㒘㒙㒗㒥㒛㒣㒝㒞㒝㒜㒝㒠㒝㒘㒝㒟㒝㒘㒝㒚㒜㒟㒛㒡㒚㒝㒜㒗㒚㒢㒛㒛㒛㒜㒚㒥㒙㒢㒚㒟㒙㒞㒙㒣㒘㒤㒙㒦㒤㒦㒟㒜㒢㒛㒣㒣㒥㒙㒥㒚㒣㒝㒞㒢㒤㒘㒥㒙㒟㒢㒟㒝㒟㒙㒞㒥㒣㒟㒞㒝㒞㒜㒝㒥㒝㒡㒝㒝㒡㒞㒢㒘㒡㒡㒡㒡㒜㒢㒛㒥㒛㒡㒛㒝㒢㒠㒡㒤㒡㒣㒡㒘㒡㒜㒠㒥㒟㒢㒟㒠㒟㒞㒦㒚㒘㒡㒘㒝㒘㒙㒗㒥㒗㒡㒝㒝㒝㒛㒚㒥㒞㒟㒦㒤㒦㒙㒥㒥㒥㒡㒚㒝㒛㒥㒚㒦㒜㒚㒚㒢㒛㒛㒛㒘㒠㒦㒘㒣㒙㒚㒦㒘㒞㒡㒢㒢㒣㒢㒞㒜㒥㒠㒙㒛㒡㒜㒠㒥㒠㒡㒠㒝㒗㒗㒦㒚㒗㒘㒗㒛㒟㒢㒞㒥㒞㒡㒞㒝㒣㒙㒥㒗㒤㒠㒤㒥㒣㒢㒣㒢㒣㒚㒣㒡㒣㒢㒛㒥㒜㒞㒛㒝㒛㒙㒚㒥㒠㒗㒠㒦㒡㒛㒟㒦㒠㒣㒞㒙㒟㒢㒠㒝㒞㒦㒞㒦㒟㒛㒞㒤㒝㒗㒜㒡㒗㒚㒦㒥㒦㒡㒦㒝㒚㒚㒘㒢㒣㒙㒜㒗㒤㒡㒢㒣㒗㒜㒟㒜㒠㒟㒗㒤㒠㒦㒗㒦㒝㒞㒚㒟㒘㒡㒥㒤㒛㒝㒞㒙㒥㒠㒡㒝㒡㒝㒠㒥㒠㒡㒠㒝㒤㒜㒥㒦㒦㒤㒥㒥㒤㒠㒟㒣㒛㒡㒝㒤㒞㒘㒜㒘㒡㒘㒚㒝㒡㒘㒚㒗㒝㒙㒜㒝㒜㒙㒛㒥㒠㒡㒢㒜㒢㒜㒡㒞㒡㒥㒠㒦㒡㒘㒠㒣㒜㒞㒙㒝㒙㒙㒘㒥㒘㒡㒘㒝㒤㒙㒝㒣㒛㒡㒟㒞㒗㒙㒦㒥㒦㒡㒦㒝㒦㒙㒥㒥㒛㒡㒙㒝㒚㒝㒥㒛㒤㒡㒤㒝㒤㒙㒘㒘㒚㒠㒚㒙㒚㒘㒚㒗㒥㒤㒜㒥㒢㒡㒡㒥㒡㒡㒡㒝㒦㒞㒥㒞㒤㒤㒗㒜㒗㒛㒦㒣㒥㒦㒦㒟㒜㒛㒟㒘㒞㒡㒞㒝㒞㒙㒢㒜㒣㒦㒤㒡㒥㒗㒝㒛㒜㒡㒜㒝㒜㒙㒣㒝㒢㒡㒡㒠㒡㒚㒡㒡㒡㒝㒝㒚㒞㒠㒟㒜㒦㒙㒗㒝㒞㒚㒤㒝㒥㒟㒜㒜㒝㒝㒗㒦㒗㒡㒗㒝㒗㒙㒛㒘㒜㒘㒡㒘㒣㒥㒥㒤㒗㒠㒘㒥㒣㒠㒙㒜㒠㒠㒡㒢㒤㒙㒣㒥㒣㒡㒣㒝㒣㒙㒢㒥㒥㒤㒦㒝㒤㒣㒢㒝㒡㒡㒡㒝㒡㒙㒦㒗㒗㒘㒥㒙㒤㒛㒣㒦㒤㒥㒤㒡㒦㒠㒦㒣㒞㒦㒞㒝㒞㒙㒝㒥㒢㒞㒤㒜㒤㒗㒣㒚㒤㒚㒦㒥㒜㒚㒛㒥㒛㒡㒛㒝㒟㒞㒠㒙㒛㒛㒚㒝㒚㒙㒙㒥㒞㒣㒠㒜㒟㒛㒟㒤㒟㒥㒟㒜㒜㒦㒞㒤㒞㒟㒞㒜㒜㒝㒗㒙㒦㒡㒦㒝㒦㒙㒚㒝㒛㒦㒛㒞㒛㒝㒟㒝㒥㒙㒤㒝㒤㒙㒣㒥㒘㒙㒚㒢㒙㒦㒘㒦㒙㒟㒙㒜㒘㒢㒘㒙㒡㒡㒢㒛㒡㒙㒠㒥㒠㒡㒤㒤㒗㒘㒗㒙㒦㒙㒥㒞㒥㒦㒤㒘㒤㒦㒥㒚㒤㒢㒤㒗㒤㒠㒤㒙㒣㒝㒤㒦㒜㒡㒜㒝㒜㒙㒛㒥㒛㒡㒣㒝㒟㒤㒞㒥㒥㒜㒚㒝㒚㒙㒙㒥㒙㒡㒙㒝㒡㒙㒝㒟㒜㒡㒥㒢㒘㒙㒗㒥㒗㒡㒗㒝㒗㒙㒦㒥㒚㒣㒚㒝㒠㒡㒦㒙㒥㒡㒥㒝㒥㒙㒚㒘㒛㒚㒜㒗㒚㒞㒙㒙㒤㒛㒣㒝㒣㒙㒢㒥㒗㒜㒘㒦㒘㒜㒘㒠㒦㒡㒘㒙㒗㒚㒘㒞㒦㒦㒗㒟㒝㒛㒠㒘㒟㒡㒟㒝㒟㒙㒢㒦㒣㒡㒢㒦㒦㒗㒞㒜㒝㒡㒝㒝㒝㒙㒡㒘㒣㒚㒣㒡㒢㒢㒣㒟㒡㒦㒢㒛㒣㒗㒛㒝㒚㒡㒚㒝㒚㒙㒠㒗㒠㒚㒠㒡㒜㒗㒟㒗㒠㒙㒟㒜㒟㒛㒝㒙㒘㒚㒗㒝㒗㒙㒦㒥㒛㒞㒜㒞㒜㒠㒜㒣㒜㒚㒜㒡㒜㒞㒛㒙㒚㒦㒙㒡㒤㒝㒣㒥㒣㒡㒣㒝㒗㒡㒙㒚㒘㒢㒘㒡㒟㒞㒡㒥㒡㒡㒡㒝㒡㒙㒠㒥㒜㒡㒗㒚㒤㒙㒥㒙㒟㒥㒟㒝㒟㒙㒞㒥㒦㒘㒥㒟㒤㒚㒤㒥㒝㒤㒗㒗㒦㒢㒦㒞㒦㒚㒥㒦㒥㒢㒙㒞㒟㒠㒞㒚㒛㒙㒚㒥㒚㒡㒚㒝㒚㒙㒥㒥㒞㒤㒝㒝㒞㒠㒘㒥㒘㒡㒘㒝㒘㒙㒗㒥㒗㒡㒜㒦㒛㒙㒞㒣㒦㒦㒦㒝㒦㒙㒥㒥㒚㒚㒜㒚㒛㒚㒛㒜㒚㒦㒤㒠㒟㒥㒚㒗㒗㒤㒟㒝㒡㒥㒢㒦㒟㒤㒦㒜㒢㒙㒢㒟㒡㒡㒡㒝㒡㒙㒦㒚㒥㒚㒤㒤㒗㒛㒥㒦㒥㒥㒥㒦㒥㒞㒥㒣㒥㒥㒡㒗㒞㒟㒝㒥㒝㒡㒝㒝㒢㒙㒢㒦㒣㒣㒢㒢㒣㒗㒣㒙㒘㒣㒝㒚㒛㒙㒚㒥㒚㒡㒞㒡㒠㒚㒡㒗㒠㒜㒛㒝㒝㒝㒟㒚㒠㒙㒚㒝㒚㒡㒝㒘㒟㒚㒞㒛㒝㒚㒝㒥㒝㒤㒜㒢㒘㒙㒚㒙㒜㒠㒜㒛㒗㒠㒜㒙㒦㒡㒙㒛㒚㒞㒚㒚㒙㒥㒥㒦㒛㒗㒣㒠㒢㒡㒢㒝㒢㒙㒗㒘㒘㒡㒗㒞㒘㒠㒗㒣㒤㒢㒗㒚㒦㒚㒗㒗㒦㒠㒦㒘㒜㒞㒞㒥㒞㒡㒞㒝㒞㒙㒝㒥㒡㒡㒣㒤㒡㒙㒤㒣㒝㒞㒜㒝㒜㒙㒛㒥㒠㒗㒡㒢㒡㒥㒡㒞㒡㒡㒠㒢㒞㒦㒠㒚㒠㒟㒠㒢㒝㒜㒝㒙㒜㒢㒛㒚㒘㒙㒗㒥㒗㒡㒗㒝㒗㒙㒦㒥㒙㒣㒚㒝㒞㒗㒦㒡㒥㒡㒥㒝㒥㒙㒙㒞㒛㒟㒛㒣㒛㒘㒚㒠㒙㒦㒘㒠㒙㒞㒚㒗㒚㒗㒘㒢㒙㒛㒡㒥㒢㒚㒡㒝㒡㒙㒠㒥㒤㒤㒦㒥㒦㒚㒗㒗㒥㒢㒥㒠㒦㒝㒥㒚㒥㒣㒛㒟㒞㒟㒝㒥㒝㒡㒝㒝㒢㒛㒣㒚㒣㒞㒣㒜㒣㒝㒢㒚㒞㒛㒝㒝㒛㒙㒚㒥㒚㒡㒞㒣㒞㒥㒟㒞㒛㒡㒝㒟㒠㒢㒟㒥㒞㒢㒟㒠㒟㒜㒙㒥㒚㒙㒚㒟㒙㒙㒛㒘㒝㒝㒜㒦㒜㒜㒜㒠㒜㒤㒗㒝㒜㒝㒛㒤㒦㒡㒚㒠㒛㒘㒚㒣㒚㒗㒙㒦㒚㒛㒙㒢㒥㒚㒗㒡㒢㒟㒡㒥㒡㒡㒡㒝㒥㒟㒘㒗㒦㒢㒗㒚㒦㒞㒣㒗㒚㒙㒠㒗㒟㒙㒞㒥㒞㒡㒣㒡㒤㒞㒥㒝㒤㒥㒢㒠㒣㒜㒢㒦㒣㒝㒢㒢㒢㒝㒞㒢㒛㒡㒛㒝㒛㒙㒚㒥㒚㒡㒚㒝㒙㒙㒝㒤㒡㒢㒙㒝㒙㒙㒘㒥㒘㒡㒘㒝㒘㒙㒞㒠㒛㒡㒢㒘㒜㒠㒤㒙㒟㒝㒢㒜㒦㒠㒢㒡㒟㒟㒙㒜㒥㒙㒥㒛㒤㒡㒤㒝㒤㒙㒘㒥㒚㒝㒙㒞㒚㒢㒙㒚㒙㒣㒗㒡㒢㒞㒡㒥㒡㒡㒡㒝㒥㒚㒗㒗㒗㒣㒦㒦㒗㒛㒢㒢㒦㒥㒡㒠㒠㒦㒞㒤㒙㒥㒚㒗㒚㒜㒙㒤㒣㒘㒚㒞㒜㒜㒢㒢㒜㒡㒙㒝㒣㒠㒙㒢㒟㒠㒞㒗㒜㒝㒚㒥㒚㒡㒚㒝㒞㒢㒠㒣㒠㒗㒟㒦㒠㒗㒟㒞㒟㒥㒟㒦㒚㒙㒝㒞㒞㒚㒝㒢㒝㒥㒝㒙㒘㒡㒘㒥㒚㒞㒛㒘㒚㒡㒗㒦㒢㒞㒤㒥㒤㒡㒤㒝㒤㒙㒣㒥㒛㒡㒘㒞㒗㒙㒝㒠㒤㒢㒣㒢㒞㒟㒗㒤㒛㒢㒘㒟㒛㒜㒤㒤㒝㒦㒜㒗㒚㒣㒢㒠㒡㒡㒥㒣㒠㒘㒝㒝㒢㒠㒞㒝㒞㒠㒝㒥㒝㒡㒝㒝㒣㒝㒣㒞㒣㒤㒢㒠㒣㒘㒣㒗㒡㒥㒠㒡㒛㒞㒚㒥㒚㒡㒚㒝㒟㒞㒞㒙㒠㒚㒠㒚㒜㒛㒛㒟㒙㒠㒘㒝㒘㒙㒗㒥㒝㒥㒞㒠㒝㒟㒘㒥㒝㒚㒝㒠㒘㒙㒜㒝㒛㒢㒜㒟㒛㒦㒛㒡㒚㒦㒛㒠㒛㒜㒦㒟㒤㒜㒣㒝㒣㒙㒢㒥㒦㒢㒘㒡㒘㒦㒘㒞㒘㒟㒦㒟㒗㒞㒗㒢㒗㒠㒗㒡㒦㒞㒝㒗㒟㒦㒟㒝㒟㒙㒞㒥㒣㒙㒥㒜㒥㒗㒤㒚㒥㒚㒢㒡㒝㒠㒜㒥㒜㒡㒜㒝㒠㒡㒣㒙㒢㒥㒢㒝㒟㒠㒡㒚㒡㒥㒥㒘㒚㒙㒙㒥㒙㒡㒙㒝㒙㒙㒘㒥㒘㒡㒜㒝㒥㒛㒚㒟㒗㒡㒗㒝㒗㒙㒝㒝㒝㒥㒝㒡㒝㒙㒙㒟㒘㒠㒘㒜㒜㒠㒜㒜㒜㒘㒗㒛㒛㒛㒚㒤㒙㒣㒚㒙㒚㒘㒚㒝㒥㒟㒘㒠㒙㒘㒘㒢㒤㒠㒗㒞㒘㒜㒘㒘㒦㒦㒗㒡㒣㒘㒣㒤㒦㒚㒥㒡㒢㒦㒢㒝㒡㒣㒡㒣㒡㒡㒡㒜㒡㒙㒠㒠㒠㒝㒠㒘㒟㒡㒜㒝㒜㒝㒛㒥㒛㒡㒛㒝㒡㒠㒠㒦㒡㒞㒠㒢㒢㒗㒚㒜㒙㒡㒙㒝㒙㒙㒞㒛㒟㒚㒟㒠㒞㒢㒞㒗㒞㒝㒝㒢㒜㒝㒗㒛㒦㒡㒦㒝㒦㒙㒚㒣㒜㒦㒜㒛㒛㒢㒜㒙㒛㒠㒗㒗㒤㒝㒣㒥㒣㒡㒣㒝㒘㒗㒘㒦㒙㒞㒘㒢㒜㒡㒢㒠㒡㒡㒡㒝㒡㒙㒦㒘㒗㒡㒦㒞㒗㒠㒦㒣㒣㒣㒥㒞㒥㒥㒥㒡㒤㒦㒥㒟㒦㒗㒞㒟㒝㒡㒝㒝㒝㒙㒢㒤㒢㒠㒣㒠㒢㒞㒢㒘㒢㒦㒢㒟㒡㒞㒡㒚㒡㒢㒤㒥㒚㒡㒙㒥㒙㒡㒙㒝㒞㒛㒟㒤㒟㒥㒞㒞㒟㒝㒞㒞㒞㒠㒞㒛㒗㒙㒦㒦㒦㒡㒦㒝㒦㒙㒛㒗㒝㒢㒥㒝㒥㒙㒤㒥㒤㒡㒤㒝㒜㒙㒙㒥㒗㒡㒣㒠㒞㒟㒙㒣㒢㒦㒚㒝㒜㒣㒛㒗㒛㒣㒥㒜㒣㒣㒡㒚㒠㒡㒠㒝㒠㒙㒤㒘㒦㒝㒦㒜㒦㒠㒥㒣㒛㒣㒟㒗㒞㒙㒝㒥㒝㒡㒢㒠㒤㒙㒢㒦㒤㒘㒣㒛㒠㒟㒣㒚㒢㒤㒡㒠㒡㒚㒝㒢㒙㒙㒠㒞㒟㒠㒙㒥㒙㒜㒥㒘㒢㒡㒜㒤㒛㒛㒘㒦㒘㒙㒗㒥㒗㒡㒞㒤㒝㒞㒝㒗㒝㒙㒝㒜㒝㒘㒜㒠㒚㒚㒙㒡㒟㒡㒥㒙㒤㒡㒤㒝㒤㒙㒘㒚㒚㒟㒚㒢㒙㒦㒥㒢㒦㒘㒢㒥㒟㒦㒛㒤㒥㒘㒥㒤㒞㒘㒤㒤㒥㒥㒡㒘㒠㒙㒟㒥㒟㒡㒦㒙㒥㒞㒤㒦㒤㒥㒤㒢㒥㒛㒥㒘㒤㒥㒣㒞㒤㒝㒤㒘㒗㒙㒜㒤㒜㒙㒛㒥㒛㒡㒠㒝㒡㒥㒠㒦㒡㒟㒠㒢㒡㒝㒟㒦㒦㒣㒚㒢㒙㒙㒘㒥㒘㒡㒞㒡㒞㒢㒟㒘㒝㒤㒞㒜㒞㒛㒝㒙㒙㒟㒜㒤㒜㒠㒘㒤㒜㒘㒚㒞㒙㒞㒙㒝㒗㒣㒛㒢㒙㒣㒛㒝㒘㒦㒚㒘㒝㒡㒣㒞㒢㒡㒢㒝㒢㒙㒘㒜㒗㒢㒘㒚㒗㒞㒘㒘㒦㒦㒗㒛㒗㒜㒦㒚㒟㒤㒤㒚㒤㒝㒞㒟㒞㒠㒝㒡㒤㒜㒜㒠㒡㒠㒝㒠㒢㒤㒠㒟㒜㒙㒞㒜㒞㒘㒤㒝㒘㒙㒟㒜㒘㒛㒛㒣㒚㒡㒚㒝㒚㒙㒠㒜㒟㒢㒠㒚㒟㒞㒠㒘㒞㒦㒟㒛㒟㒜㒞㒚㒚㒠㒝㒥㒞㒝㒞㒙㒝㒡㒦㒝㒦㒝㒥㒥㒥㒡㒥㒝㒙㒟㒛㒤㒛㒟㒛㒡㒙㒝㒤㒙㒣㒡㒣㒝㒣㒙㒗㒟㒙㒤㒙㒜㒙㒗㒡㒥㒢㒝㒡㒝㒡㒙㒠㒥㒤㒢㒦㒡㒦㒝㒤㒚㒗㒙㒦㒡㒦㒛㒤㒦㒢㒤㒤㒞㒥㒜㒤㒝㒥㒢㒝㒝㒝㒙㒜㒥㒜㒡㒜㒝㒠㒙㒢㒚㒟㒡㒠㒡㒛㒤㒚㒥㒚㒡㒚㒝㒟㒜㒠㒥㒟㒢㒠㒤㒠㒗㒝㒣㒟㒚㒟㒠㒟㒜㒝㒦㒞㒟㒜㒡㒗㒤㒦㒥㒦㒡㒦㒝㒚㒥㒜㒚㒛㒢㒛㒡㒛㒞㒜㒗㒚㒣㒛㒜㒚㒚㒛㒗㒙㒥㒠㒢㒝㒞㒙㒢㒞㒥㒠㒜㒘㒤㒤㒗㒠㒘㒥㒜㒛㒡㒡㒝㒠㒡㒠㒝㒠㒙㒤㒗㒦㒠㒥㒡㒦㒢㒣㒜㒦㒚㒥㒟㒥㒘㒘㒝㒞㒝㒝㒝㒝㒙㒜㒥㒡㒥㒣㒟㒢㒢㒢㒜㒢㒘㒡㒢㒢㒛㒟㒚㒢㒗㒠㒢㒡㒗㒡㒙㒜㒞㒦㒙㒤㒘㒜㒟㒘㒡㒝㒜㒢㒤㒥㒠㒛㒠㒚㒗㒗㒞㒦㒥㒦㒡㒦㒝㒚㒜㒜㒤㒜㒝㒜㒜㒜㒛㒗㒟㒤㒢㒤㒝㒤㒙㒣㒥㒚㒝㒣㒝㒣㒚㒢㒥㒢㒡㒢㒝㒗㒡㒟㒗㒡㒦㒡㒝㒡㒙㒠㒥㒥㒗㒗㒟㒦㒚㒦㒢㒥㒦㒤㒡㒟㒥㒞㒥㒞㒡㒞㒝㒣㒟㒤㒞㒤㒣㒣㒞㒤㒛㒡㒡㒣㒚㒣㒥㒢㒞㒢㒞㒢㒣㒢㒜㒘㒛㒛㒞㒚㒡㒚㒝㒚㒙㒟㒜㒟㒢㒠㒙㒟㒤㒠㒘㒟㒡㒞㒢㒞㒞㒞㒙㒟㒢㒙㒟㒣㒞㒢㒚㒘㒠㒦㒣㒞㒚㒠㒚㒙㒠㒝㒛㒥㒦㒤㒥㒤㒡㒤㒝㒚㒚㒚㒥㒚㒚㒦㒜㒚㒠㒙㒚㒘㒣㒘㒥㒙㒘㒘㒤㒘㒜㒘㒠㒤㒘㒣㒟㒠㒢㒠㒝㒠㒙㒟㒥㒦㒚㒜㒟㒟㒢㒞㒥㒞㒡㒞㒝㒣㒜㒤㒘㒣㒢㒤㒙㒣㒞㒢㒙㒤㒚㒣㒝㒢㒞㒞㒟㒜㒛㒛㒝㒛㒙㒚㒥㒟㒥㒠㒢㒡㒡㒡㒙㒝㒤㒠㒜㒟㒥㒟㒤㒟㒣㒛㒠㒠㒚㒗㒥㒗㒡㒗㒝㒗㒙㒦㒥㒦㒡㒚㒦㒚㒙㒠㒝㒥㒥㒥㒝㒥㒙㒤㒥㒙㒙㒚㒢㒚㒚㒚㒙㒛㒟㒤㒞㒣㒙㒢㒥㒢㒡㒗㒚㒞㒜㒝㒟㒘㒤㒗㒦㒗㒜㒦㒦㒢㒡㒤㒢㒗㒜㒗㒙㒦㒠㒦㒢㒦㒛㒤㒦㒤㒥㒤㒞㒘㒡㒞㒟㒝㒡㒝㒝㒝㒙㒡㒞㒣㒞㒢㒞㒢㒠㒢㒚㒠㒝㒡㒞㒡㒛㒡㒚㒡㒝㒤㒥㒚㒦㒙㒥㒙㒡㒙㒝㒝㒜㒟㒤㒟㒝㒟㒜㒟㒛㒝㒘㒝㒦㒞㒞㒞㒞㒝㒚㒝㒟㒜㒠㒜㒞㒦㒘㒘㒟㒝㒗㒞㒞㒦㒤㒗㒣㒝㒞㒞㒞㒗㒤㒠㒣㒤㒙㒣㒙㒢㒥㒢㒡㒗㒤㒘㒚㒘㒞㒘㒥㒥㒣㒘㒘㒘㒗㒤㒤㒦㒥㒦㒢㒦㒡㒥㒥㒢㒗㒟㒢㒞㒥㒞㒡㒞㒝㒢㒛㒤㒤㒣㒥㒤㒦㒡㒟㒣㒤㒣㒣㒢㒠㒢㒞㒡㒜㒛㒡㒛㒝㒛㒙㒚㒥㒚㒡㒛㒝㒢㒚㒝㒥㒦㒣㒚㒛㒙㒙㒘㒥㒘㒡㒝㒛㒞㒞㒟㒜㒞㒥㒞㒜㒞㒗㒞㒘㒝㒠㒜㒣㒝㒝㒚㒟㒚㒤㒚㒜㒚㒗㒢㒗㒤㒦㒤㒝㒤㒙㒣㒥㒘㒣㒙㒦㒙㒠㒙㒝㒙㒥㒢㒠㒛㒤㒠㒗㒘㒘㒟㒜㒜㒢㒝㒥㒜㒞㒤㒜㒚㒤㒟㒥㒟㒡㒟㒝㒟㒙㒞㒥㒞㒡㒣㒘㒢㒙㒠㒢㒝㒡㒝㒝㒝㒙㒜㒥㒜㒡㒜㒝㒠㒗㒟㒥㒦㒙㒜㒘㒛㒙㒚㒥㒚㒡㒟㒙㒡㒘㒠㒘㒟㒢㒠㒙㒞㒙㒟㒡㒞㒢㒟㒦㒞㒞㒟㒗㒢㒜㒗㒝㒗㒙㒦㒥㒦㒡㒦㒝㒦㒙㒚㒢㒙㒡㒥㒠㒘㒜㒘㒘㒗㒤㒗㒠㒗㒜㒗㒘㒡㒤㒗㒜㒘㒝㒣㒙㒢㒡㒢㒝㒢㒙㒗㒚㒥㒥㒗㒦㒗㒦㒛㒝㒠㒢㒠㒝㒠㒙㒟㒥㒥㒠㒚㒘㒟㒙㒞㒥㒞㒡㒞㒝㒞㒙㒙㒥㒢㒢㒡㒝㒢㒠㒛㒢㒠㒜㒤㒦㒤㒘㒜㒢㒙㒦㒘㒢㒟㒘㒢㒦㒟㒜㒞㒢㒦㒜㒟㒤㒛㒝㒣㒤㒗㒦㒜㒤㒠㒢㒘㒝㒘㒙㒗㒥㒗㒡㒗㒝㒥㒙㒝㒣㒚㒡㒦㒠㒦㒙㒥㒥㒥㒡㒥㒝㒥㒙㒘㒥㒚㒗㒘㒝㒤㒙㒥㒗㒣㒡㒣㒝㒣㒙㒦㒡㒦㒠㒦㒜㒦㒗㒣㒥㒗㒗㒗㒦㒘㒛㒦㒦㒗㒣㒢㒝㒤㒥㒦㒞㒗㒙㒥㒢㒥㒢㒦㒗㒥㒠㒦㒛㒞㒤㒝㒥㒝㒡㒝㒝㒢㒝㒣㒚㒤㒙㒣㒡㒡㒠㒣㒗㒡㒢㒢㒝㒢㒙㒡㒚㒠㒥㒝㒚㒚㒙㒙㒥㒙㒡㒙㒝㒙㒙㒘㒥㒜㒜㒜㒝㒥㒛㒙㒝㒗㒡㒗㒝㒗㒙㒝㒥㒜㒢㒝㒠㒝㒝㒜㒚㒛㒣㒛㒦㒜㒗㒗㒣㒚㒤㒛㒜㒚㒦㒦㒤㒚㒣㒙㒞㒚㒠㒥㒤㒙㒦㒗㒘㒥㒜㒥㒜㒦㒗㒘㒗㒥㒞㒞㒗㒡㒜㒠㒝㒠㒙㒟㒥㒤㒡㒦㒢㒦㒡㒤㒦㒥㒣㒠㒝㒢㒚㒥㒗㒤㒞㒣㒞㒤㒜㒢㒙㒜㒢㒜㒝㒜㒙㒛㒥㒠㒞㒞㒗㒛㒝㒚㒥㒚㒡㒚㒝㒞㒥㒠㒚㒠㒗㒠㒡㒦㒛㒘㒦㒘㒡㒘㒝㒘㒙㒞㒥㒚㒛㒗㒤㒗㒙㒦㒥㒦㒡㒛㒠㒜㒢㒜㒗㒜㒝㒛㒦㒜㒗㒛㒜㒟㒙㒤㒦㒤㒙㒣㒥㒣㒡㒙㒠㒙㒡㒘㒦㒙㒣㒘㒞㒘㒜㒙㒙㒗㒦㒘㒟㒙㒚㒠㒥㒠㒡㒠㒝㒠㒙㒟㒥㒚㒡㒦㒠㒣㒙㒙㒝㒞㒥㒞㒝㒞㒙㒝㒥㒡㒤㒤㒟㒤㒘㒣㒥㒢㒘㒥㒡㒢㒣㒡㒘㒛㒡㒣㒟㒜㒞㒘㒚㒞㒠㒤㒥㒚㒟㒙㒥㒙㒡㒙㒝㒝㒡㒟㒤㒟㒝㒞㒡㒞㒞㒟㒗㒟㒟㒗㒞㒗㒙㒦㒥㒦㒡㒚㒣㒛㒠㒡㒠㒚㒡㒤㒣㒗㒘㒛㒙㒚㒝㒢㒝㒘㒘㒤㒘㒣㒡㒣㒝㒣㒙㒢㒥㒢㒡㒞㒝㒗㒞㒥㒥㒙㒟㒡㒦㒡㒙㒠㒥㒠㒡㒥㒠㒦㒜㒗㒗㒥㒦㒥㒢㒦㒗㒣㒜㒥㒦㒤㒦㒠㒣㒟㒚㒝㒡㒝㒝㒝㒙㒡㒘㒣㒠㒣㒙㒣㒘㒣㒗㒠㒤㒡㒢㒢㒚㒢㒚㒠㒦㒡㒛㒠㒜㒠㒚㒞㒜㒟㒢㒠㒢㒟㒥㒟㒠㒞㒦㒟㒗㒟㒙㒜㒥㒗㒟㒗㒙㒦㒥㒦㒡㒝㒜㒝㒜㒘㒟㒥㒦㒥㒝㒥㒙㒤㒥㒙㒗㒛㒜㒛㒛㒚㒘㒙㒦㒣㒠㒜㒙㒤㒙㒗㒟㒤㒝㒤㒗㒟㒦㒛㒢㒥㒜㒦㒠㒠㒥㒠㒡㒠㒝㒠㒙㒟㒥㒟㒡㒟㒝㒟㒙㒙㒠㒚㒣㒟㒛㒛㒡㒛㒤㒣㒗㒚㒚㒛㒚㒠㒤㒗㒙㒝㒛㒜㒙㒛㒥㒛㒡㒡㒗㒟㒢㒡㒣㒠㒥㒠㒢㒡㒡㒞㒗㒟㒦㒟㒥㒟㒚㒠㒛㒟㒚㒟㒜㒟㒛㒚㒟㒘㒢㒗㒝㒗㒙㒦㒥㒛㒣㒜㒢㒝㒙㒜㒡㒜㒚㒛㒠㒛㒚㒜㒙㒚㒦㒚㒡㒙㒜㒛㒙㒚㒠㒚㒟㒙㒚㒙㒜㒘㒦㒗㒡㒢㒝㒡㒥㒡㒡㒡㒝㒘㒝㒗㒞㒗㒞㒦㒢㒢㒣㒟㒦㒟㒡㒟㒝㒟㒙㒣㒥㒣㒥㒞㒣㒞㒙㒝㒥㒝㒡㒡㒣㒤㒛㒢㒦㒣㒞㒢㒢㒟㒜㒛㒥㒜㒛㒛㒝㒛㒙㒚㒥㒟㒘㒠㒢㒡㒝㒟㒘㒟㒦㒠㒟㒠㒟㒟㒞㒞㒤㒞㒢㒢㒤㒝㒜㒗㒙㒘㒞㒛㒙㒙㒡㒢㒣㒡㒛㒚㒘㒣㒗㒦㒡㒥㒝㒥㒙㒤㒥㒘㒣㒚㒞㒚㒜㒚㒠㒚㒘㒚㒟㒚㒘㒚㒚㒙㒟㒘㒡㒦㒜㒘㒤㒘㒝㒘㒜㒘㒛㒤㒘㒣㒛㒠㒠㒠㒙㒟㒥㒟㒡㒤㒙㒥㒞㒥㒜㒦㒟㒟㒜㒞㒙㒝㒥㒝㒡㒡㒞㒣㒝㒣㒙㒠㒦㒣㒣㒢㒞㒢㒣㒢㒥㒟㒥㒡㒚㒡㒣㒠㒥㒡㒙㒠㒞㒡㒗㒡㒢㒙㒝㒙㒙㒘㒥㒘㒡㒘㒝㒚㒙㒞㒤㒛㒡㒚㒚㒦㒟㒦㒜㒦㒚㒢㒜㒞㒡㒠㒚㒣㒣㒙㒜㒟㒤㒚㒛㒥㒟㒙㒛㒠㒙㒜㒛㒢㒣㒡㒗㒗㒘㒣㒘㒢㒡㒢㒝㒢㒙㒡㒥㒡㒡㒡㒝㒥㒞㒤㒥㒣㒛㒠㒠㒠㒙㒟㒥㒟㒡㒥㒞㒦㒙㒥㒞㒛㒦㒞㒝㒞㒙㒝㒥㒝㒡㒝㒝㒗㒙㒣㒥㒠㒡㒤㒛㒜㒟㒛㒥㒛㒡㒛㒝㒟㒚㒡㒢㒡㒠㒡㒢㒡㒗㒡㒙㒙㒡㒙㒤㒙㒙㒘㒥㒘㒡㒞㒥㒟㒝㒟㒙㒞㒡㒛㒗㒚㒘㒙㒤㒣㒣㒦㒞㒦㒙㒥㒥㒥㒡㒙㒦㒥㒙㒥㒛㒤㒡㒤㒝㒤㒙㒘㒢㒚㒠㒚㒛㒙㒤㒙㒚㒚㒚㒚㒛㒢㒡㒡㒥㒡㒡㒡㒝㒥㒡㒘㒙㒗㒥㒗㒝㒥㒙㒦㒤㒦㒤㒦㒡㒟㒜㒞㒥㒞㒡㒞㒝㒞㒙㒝㒥㒙㒡㒣㒣㒡㒙㒢㒙㒝㒜㒜㒝㒜㒙㒛㒥㒡㒤㒡㒥㒡㒞㒡㒘㒡㒜㒠㒠㒠㒚㒠㒡㒠㒝㒟㒢㒠㒛㒛㒢㒘㒡㒘㒝㒘㒙㒗㒥㒗㒡㒗㒝㒗㒡㒚㒥㒣㒦㒦㒝㒦㒙㒥㒥㒥㒡㒥㒝㒗㒙㒛㒗㒘㒡㒗㒗㒤㒜㒣㒥㒣㒡㒣㒝㒚㒗㒙㒚㒚㒘㒚㒛㒢㒣㒡㒥㒡㒡㒡㒝㒦㒝㒗㒚㒘㒙㒗㒡㒤㒛㒗㒚㒦㒥㒦㒡㒦㒘㒥㒣㒛㒣㒟㒜㒞㒙㒝㒥㒝㒡㒡㒟㒤㒘㒤㒗㒢㒥㒢㒢㒣㒛㒡㒘㒢㒚㒣㒗㒡㒞㒟㒥㒡㒚㒡㒥㒠㒞㒠㒡㒟㒘㒛㒞㒤㒥㒚㒚㒜㒡㒛㒠㒛㒜㒥㒘㒛㒠㒗㒠㒗㒙㒦㒥㒦㒡㒦㒝㒦㒙㒝㒥㒛㒠㒙㒝㒟㒡㒥㒝㒤㒡㒤㒝㒤㒙㒙㒘㒙㒤㒚㒟㒙㒞㒙㒣㒗㒘㒙㒢㒘㒢㒢㒘㒤㒜㒞㒘㒝㒚㒘㒥㒟㒗㒣㒟㒜㒣㒣㒤㒢㒛㒠㒘㒟㒙㒞㒥㒞㒡㒣㒙㒥㒘㒤㒘㒣㒢㒤㒙㒢㒙㒣㒡㒢㒢㒣㒦㒢㒞㒣㒗㒣㒟㒛㒢㒛㒙㒚㒥㒚㒡㒟㒢㒞㒝㒠㒞㒠㒞㒜㒟㒙㒙㒙㒡㒘㒡㒘㒝㒘㒙㒜㒘㒞㒠㒞㒟㒞㒗㒝㒚㒝㒣㒛㒟㒜㒚㒜㒙㒜㒚㒜㒢㒜㒜㒜㒦㒤㒡㒤㒝㒤㒙㒣㒥㒣㒡㒣㒝㒗㒗㒞㒥㒟㒣㒢㒞㒢㒙㒡㒥㒡㒡㒘㒛㒡㒙㒡㒞㒠㒡㒠㒝㒠㒙㒤㒥㒦㒝㒥㒞㒦㒢㒥㒚㒥㒣㒢㒤㒥㒞㒤㒞㒢㒥㒞㒘㒝㒙㒜㒥㒜㒡㒠㒠㒢㒢㒣㒙㒢㒚㒣㒗㒡㒞㒡㒣㒡㒤㒠㒥㒠㒢㒠㒥㒙㒤㒚㒟㒞㒡㒘㒙㒦㒠㒞㒤㒤㒛㒤㒤㒛㒠㒤㒟㒗㒞㒦㒥㒦㒡㒦㒝㒚㒜㒜㒝㒛㒦㒜㒠㒜㒝㒜㒣㒥㒛㒤㒝㒤㒙㒣㒥㒘㒡㒚㒟㒚㒘㒚㒝㒙㒚㒙㒚㒘㒢㒙㒙㒙㒚㒦㒣㒦㒟㒠㒥㒛㒜㒚㒙㒚㒙㒗㒥㒟㒠㒣㒠㒛㒙㒜㒝㒢㒠㒡㒗㒞㒠㒝㒥㒝㒡㒝㒝㒡㒜㒣㒤㒣㒣㒢㒢㒠㒠㒣㒚㒢㒚㒞㒗㒜㒝㒚㒥㒚㒡㒚㒝㒟㒛㒠㒚㒠㒞㒠㒜㒠㒝㒟㒚㒚㒡㒝㒠㒝㒙㒝㒞㒙㒡㒙㒥㒜㒛㒝㒚㒝㒞㒝㒜㒝㒝㒜㒚㒜㒤㒗㒦㒟㒤㒤㒥㒤㒡㒤㒝㒤㒙㒣㒥㒣㒡㒗㒜㒗㒙㒠㒗㒢㒢㒢㒝㒢㒙㒡㒥㒦㒦㒤㒗㒣㒜㒠㒥㒠㒡㒠㒝㒞㒦㒙㒥㒛㒝㒞㒚㒚㒠㒙㒜㒝㒞㒘㒝㒙㒥㒜㒢㒙㒘㒘㒤㒡㒚㒡㒗㒡㒣㒠㒞㒞㒙㒡㒘㒠㒦㒟㒞㒝㒙㒟㒢㒞㒦㒟㒛㒟㒝㒞㒚㒜㒟㒜㒛㒜㒗㒗㒢㒢㒡㒤㒙㒦㒦㒣㒡㒠㒟㒚㒗㒗㒣㒦㒥㒦㒡㒦㒝㒛㒜㒝㒚㒜㒣㒛㒣㒛㒚㒛㒘㒚㒦㒘㒤㒛㒞㒚㒞㒞㒜㒦㒢㒤㒚㒤㒤㒜㒡㒦㒤㒠㒚㒠㒗㒥㒠㒤㒗㒡㒠㒠㒥㒠㒡㒠㒝㒦㒟㒗㒗㒦㒠㒦㒚㒤㒛㒣㒜㒢㒣㒡㒗㒞㒢㒝㒥㒝㒡㒝㒝㒢㒠㒣㒤㒣㒣㒣㒘㒣㒜㒢㒥㒡㒢㒡㒠㒡㒞㒠㒙㒛㒚㒚㒝㒚㒙㒙㒥㒞㒥㒟㒢㒠㒡㒠㒙㒝㒝㒞㒞㒞㒛㒞㒚㒞㒝㒗㒝㒗㒝㒦㒥㒦㒡㒦㒝㒜㒠㒛㒦㒜㒞㒛㒢㒟㒡㒥㒞㒤㒡㒤㒝㒤㒙㒚㒘㒚㒠㒚㒟㒚㒘㒚㒚㒙㒥㒘㒦㒙㒗㒘㒚㒞㒣㒢㒗㒡㒙㒠㒥㒠㒡㒤㒣㒦㒢㒗㒗㒥㒦㒤㒠㒥㒞㒦㒗㒦㒗㒤㒢㒥㒛㒠㒟㒝㒢㒝㒝㒝㒙㒜㒥㒣㒦㒟㒗㒜㒚㒛㒥㒛㒡㒛㒝㒡㒞㒝㒢㒗㒢㒞㒞㒙㒙㒗㒤㒚㒡㒘㒜㒣㒙㒜㒤㒠㒢㒘㒝㒘㒙㒗㒥㒗㒡㒗㒝㒗㒙㒙㒡㒚㒡㒣㒟㒦㒢㒥㒥㒥㒡㒥㒝㒙㒡㒚㒚㒘㒣㒦㒝㒙㒝㒙㒗㒘㒠㒘㒙㒗㒥㒚㒣㒣㒥㒢㒝㒢㒙㒡㒥㒦㒤㒗㒢㒘㒝㒥㒥㒗㒣㒦㒦㒦㒦㒥㒦㒦㒣㒦㒦㒤㒙㒤㒦㒥㒣㒥㒡㒢㒜㒢㒛㒤㒣㒣㒞㒣㒦㒣㒚㒜㒡㒜㒤㒜㒙㒛㒥㒛㒡㒠㒣㒡㒞㒡㒘㒡㒥㒡㒜㒡㒛㒝㒘㒦㒦㒙㒝㒙㒙㒘㒥㒘㒡㒘㒝㒘㒙㒜㒡㒛㒡㒟㒛㒗㒡㒦㒥㒦㒡㒦㒝㒚㒢㒜㒣㒜㒤㒜㒡㒛㒚㒛㒣㒚㒤㒚㒢㒤㒙㒤㒞㒣㒡㒣㒝㒣㒙㒗㒗㒙㒠㒘㒡㒙㒢㒦㒛㒘㒠㒘㒟㒗㒜㒗㒚㒠㒤㒛㒦㒠㒟㒟㒗㒣㒠㒗㒡㒞㒠㒙㒥㒢㒠㒛㒟㒞㒝㒝㒥㒝㒡㒝㒝㒢㒙㒢㒦㒣㒣㒣㒡㒤㒗㒜㒝㒛㒡㒛㒝㒛㒙㒠㒘㒡㒡㒠㒞㒡㒠㒠㒣㒞㒘㒞㒡㒞㒛㒦㒗㒙㒙㒘㒝㒘㒙㒗㒥㒛㒣㒞㒜㒝㒝㒞㒞㒛㒘㒝㒦㒝㒛㒜㒤㒝㒢㒥㒝㒥㒙㒤㒥㒤㒡㒤㒝㒦㒙㒚㒟㒗㒡㒞㒘㒣㒙㒢㒥㒢㒡㒢㒝㒢㒙㒙㒥㒘㒝㒥㒝㒞㒞㒝㒚㒢㒛㒢㒡㒠㒙㒝㒡㒙㒦㒝㒛㒛㒘㒞㒥㒟㒙㒞㒝㒞㒙㒝㒥㒡㒤㒣㒞㒣㒥㒣㒡㒢㒣㒢㒞㒢㒜㒢㒠㒛㒡㒛㒣㒛㒙㒚㒥㒚㒡㒡㒠㒠㒡㒟㒦㒟㒥㒠㒜㒠㒠㒠㒣㒙㒘㒘㒝㒘㒙㒗㒥㒞㒗㒞㒟㒞㒘㒝㒢㒛㒣㒚㒤㒚㒛㒝㒦㒥㒡㒥㒝㒥㒙㒤㒥㒤㒡㒞㒝㒚㒙㒗㒥㒣㒡㒤㒙㒣㒙㒢㒥㒢㒡㒦㒟㒙㒘㒙㒗㒗㒥㒗㒢㒘㒛㒥㒘㒗㒠㒗㒙㒗㒘㒗㒗㒢㒤㒗㒛㒟㒝㒞㒥㒞㒡㒞㒝㒤㒠㒣㒦㒤㒞㒣㒢㒘㒜㒝㒜㒜㒡㒜㒝㒜㒛㒠㒚㒛㒡㒛㒝㒛㒙㒛㒚㒚㒡㒚㒝㒚㒙㒛㒗㒟㒙㒙㒝㒙㒙㒘㒥㒠㒗㒘㒝㒘㒙㒗㒥㒗㒡㒗㒝㒗㒙㒦㒥㒦㒡㒦㒝㒦㒙㒥㒥㒥㒡㒥㒝㒥㒙㒤㒥㒤㒢㒤㒝㒤㒙㒣㒥㒣㒡㒣㒝㒤㒛㒢㒥㒢㒡㒢㒞㒢㒙㒢㒗㒡㒡㒡㒝㒡㒙㒢㒗㒠㒡㒠㒝㒠㒚㒟㒥㒚㒠㒟㒝㒟㒙㒞㒥㒡㒗㒞㒝㒞㒙㒝㒦㒝㒡㒝㒦㒝㒙㒜㒦㒜㒡㒤㒠㒜㒙㒜㒙㒜㒟㒛㒝㒛㒙㒚㒥㒛㒚㒚㒝㒚㒚㒙㒥㒙㒡㒞㒦㒙㒙㒘㒥㒘㒡㒘㒞㒘㒙㒗㒥㒗㒡㒗㒟㒛㒞㒦㒥㒦㒢㒦㒝㒦㒠㒥㒥㒥㒡㒥㒝㒦㒛㒦㒦㒤㒡㒤㒞㒤㒙㒗㒞㒣㒡㒣㒝㒣㒙㒤㒗㒢㒡㒢㒝㒢㒚㒡㒥㒢㒟㒡㒞㒡㒙㒠㒥㒢㒡㒠㒝㒠㒙㒟㒦㒟㒡㒟㒞㒟㒙㒡㒛㒞㒡㒟㒟㒞㒙㒝㒥㒝㒣㒝㒝㒙㒟㒜㒥㒜㒡㒜㒝㒜㒙㒛㒥㒛㒡㒛㒞㒛㒙㒛㒗㒚㒡㒚㒟㒚㒙㒛㒗㒙㒡㒙㒝㒙㒛㒘㒥㒙㒟㒘㒞㒘㒙㒗㒥㒙㒡㒗㒝㒗㒙㒗㒗㒦㒡㒦㒟㒦㒙㒘㒛㒥㒡㒦㒟㒥㒙㒤㒥㒤㒤㒤㒝㒝㒞㒣㒥㒣㒡㒣㒝㒣㒙㒢㒥㒢㒡㒢㒟㒢㒙㒢㒗㒡㒡㒡㒟㒡㒙㒢㒗㒠㒡㒠㒝㒠㒜㒟㒥㒠㒟㒟㒞㒟㒙㒞㒥㒠㒡㒞㒝㒞㒙㒞㒘㒝㒡㒝㒠㒝㒙㒟㒛㒜㒡㒝㒟㒜㒙㒛㒥㒛㒥㒛㒝㒤㒞㒚㒥㒚㒡㒚㒝㒚㒙㒙㒥㒙㒡㒙㒠㒙㒙㒙㒗㒘㒡㒘㒟㒘㒙㒙㒗㒗㒡㒗㒝㒗㒝㒦㒥㒗㒟㒦㒞㒦㒙㒥㒥㒗㒡㒥㒝㒥㒙㒥㒙㒤㒡㒤㒡㒤㒙㒦㒛㒣㒡㒤㒟㒣㒙㒢㒥㒢㒦㒢㒝㒢㒛㒡㒦㒡㒡㒡㒝㒡㒙㒠㒥㒠㒡㒠㒡㒠㒙㒠㒗㒟㒡㒟㒟㒟㒙㒠㒗㒞㒡㒞㒝㒞㒞㒝㒥㒞㒟㒝㒞㒝㒙㒜㒥㒞㒡㒜㒝㒜㒙㒜㒚㒛㒡㒛㒢㒛㒙㒝㒛㒚㒡㒛㒟㒚㒙㒙㒥㒚㒗㒙㒝㒢㒞㒘㒥㒘㒡㒘㒝㒘㒙㒗㒥㒗㒡㒗㒢㒗㒙㒗㒗㒦㒡㒦㒟㒦㒙㒗㒗㒥㒡㒥㒝㒥㒟㒤㒥㒥㒟㒤㒞㒤㒙㒣㒥㒥㒡㒣㒝㒣㒙㒣㒛㒢㒡㒢㒣㒢㒙㒤㒛㒡㒡㒢㒟㒡㒙㒠㒥㒡㒘㒠㒝㒠㒛㒟㒦㒟㒡㒟㒝㒟㒙㒞㒥㒞㒡㒞㒣㒞㒙㒞㒗㒝㒡㒝㒟㒝㒙㒞㒗㒜㒡㒜㒝㒜㒠㒛㒥㒜㒟㒛㒞㒛㒙㒚㒥㒜㒡㒚㒝㒚㒙㒚㒜㒙㒡㒙㒤㒙㒙㒛㒛㒘㒡㒙㒟㒘㒙㒗㒥㒘㒙㒗㒝㒡㒙㒦㒥㒦㒡㒦㒝㒦㒙㒥㒥㒥㒡㒥㒤㒥㒙㒥㒗㒤㒡㒤㒟㒤㒙㒥㒗㒣㒡㒣㒝㒣㒡㒢㒥㒣㒟㒢㒞㒢㒙㒡㒥㒣㒡㒡㒝㒡㒙㒡㒝㒠㒡㒠㒥㒠㒙㒢㒛㒟㒡㒠㒟㒟㒙㒞㒥㒟㒚㒞㒝㒞㒛㒝㒦㒝㒡㒝㒝㒝㒙㒜㒥㒜㒡㒜㒥㒜㒙㒜㒗㒛㒡㒛㒟㒛㒙㒜㒗㒚㒡㒚㒝㒚㒢㒙㒥㒚㒟㒙㒞㒙㒙㒘㒥㒚㒡㒘㒝㒘㒙㒘㒞㒗㒡㒗㒦㒗㒙㒙㒛㒦㒡㒗㒟㒦㒙㒥㒥㒦㒛㒥㒝㒥㒛㒤㒦㒤㒡㒤㒝㒤㒙㒣㒥㒣㒡㒣㒦㒣㒙㒣㒗㒢㒡㒢㒟㒢㒙㒣㒗㒡㒡㒡㒝㒡㒣㒠㒥㒡㒟㒠㒞㒠㒙㒟㒥㒡㒡㒟㒝㒟㒙㒟㒟㒞㒡㒟㒗㒞㒙㒠㒛㒝㒡㒞㒟㒝㒙㒜㒥㒝㒜㒜㒝㒜㒛㒛㒦㒛㒡㒛㒝㒛㒙㒚㒥㒚㒡㒛㒗㒚㒙㒚㒗㒙㒡㒙㒟㒙㒙㒚㒗㒘㒡㒘㒝㒘㒤㒗㒥㒘㒟㒗㒞㒗㒙㒦㒥㒘㒡㒦㒝㒦㒙㒦㒠㒥㒡㒦㒘㒥㒙㒗㒛㒤㒡㒥㒟㒤㒙㒣㒥㒤㒝㒣㒝㒣㒛㒢㒦㒢㒡㒢㒝㒢㒙㒡㒥㒡㒡㒢㒘㒡㒙㒡㒗㒠㒡㒠㒟㒠㒙㒡㒗㒟㒡㒟㒝㒟㒥㒞㒥㒟㒟㒞㒞㒞㒙㒝㒥㒟㒡㒝㒝㒝㒙㒝㒡㒜㒡㒝㒙㒜㒙㒞㒛㒛㒡㒜㒟㒛㒙㒚㒥㒛㒞㒚㒝㒚㒛㒙㒦㒙㒡㒙㒝㒙㒙㒘㒥㒘㒡㒙㒙㒘㒙㒘㒗㒗㒡㒗㒟㒗㒙㒘㒗㒦㒡㒦㒝㒦㒦㒥㒥㒦㒟㒥㒞㒥㒙㒤㒥㒦㒡㒤㒝㒤㒙㒤㒢㒣㒡㒤㒚㒣㒙㒥㒛㒢㒡㒣㒟㒢㒙㒡㒥㒢㒟㒡㒝㒡㒛㒠㒦㒠㒡㒠㒝㒠㒙㒟㒥㒟㒡㒠㒚㒟㒙㒟㒗㒞㒡㒞㒟㒞㒙㒟㒗㒝㒡㒝㒝㒞㒗㒜㒥㒝㒟㒜㒞㒜㒙㒛㒥㒝㒡㒛㒝㒛㒙㒛㒣㒚㒡㒛㒛㒚㒙㒜㒛㒙㒡㒚㒟㒙㒙㒘㒥㒙㒠㒘㒝㒘㒛㒗㒦㒗㒡㒗㒝㒗㒙㒦㒥㒦㒡㒗㒛㒦㒙㒦㒗㒥㒡㒥㒟㒥㒙㒦㒗㒤㒡㒤㒝㒥㒘㒣㒥㒤㒟㒣㒞㒣㒙㒢㒥㒤㒡㒢㒝㒢㒙㒢㒤㒡㒡㒢㒜㒡㒙㒣㒛㒠㒡㒡㒟㒠㒙㒟㒥㒠㒡㒟㒝㒟㒛㒞㒦㒞㒡㒞㒝㒞㒙㒝㒥㒝㒡㒞㒜㒝㒙㒝㒗㒜㒡㒜㒟㒜㒙㒝㒗㒛㒡㒛㒝㒜㒙㒚㒥㒛㒟㒚㒞㒚㒙㒙㒥㒛㒡㒙㒝㒙㒙㒙㒥㒘㒡㒙㒝㒘㒙㒚㒛㒗㒡㒘㒟㒗㒙㒦㒥㒗㒢㒦㒝㒦㒛㒥㒦㒥㒡㒥㒝㒥㒙㒤㒥㒤㒡㒥㒝㒤㒙㒤㒗㒣㒡㒣㒟㒣㒙㒤㒗㒢㒡㒢㒝㒣㒚㒡㒥㒢㒟㒡㒞㒡㒙㒠㒥㒢㒡㒠㒝㒠㒙㒠㒦㒟㒡㒠㒞㒟㒙㒡㒛㒞㒡㒟㒟㒞㒙㒝㒥㒞㒣㒝㒝㒛㒠㒜㒥㒜㒡㒜㒝㒜㒙㒛㒥㒛㒡㒜㒞㒛㒙㒛㒗㒚㒡㒚㒟㒚㒙㒛㒗㒙㒡㒙㒝㒚㒛㒘㒥㒙㒟㒘㒞㒘㒙㒗㒥㒙㒡㒗㒝㒗㒙㒘㒗㒦㒡㒗㒟㒦㒙㒘㒛㒥㒡㒦㒟㒥㒙㒤㒥㒥㒤㒤㒝㒝㒞㒣㒥㒣㒡㒣㒝㒣㒙㒢㒥㒢㒡㒣㒟㒢㒙㒢㒗㒡㒡㒡㒟㒡㒙㒢㒗㒠㒡㒠㒝㒡㒜㒟㒥㒠㒟㒟㒞㒟㒙㒞㒥㒠㒡㒞㒝㒞㒙㒟㒘㒝㒡㒞㒠㒝㒙㒟㒛㒜㒡㒝㒟㒜㒙㒛㒥㒜㒥㒛㒝㒛㒛㒚㒦㒚㒡㒚㒝㒚㒙㒙㒥㒙㒡㒚㒠㒙㒙㒙㒗㒘㒡㒘㒟㒘㒙㒙㒗㒗㒡㒗㒝㒘㒝㒦㒥㒗㒟㒦㒞㒦㒙㒥㒥㒗㒡㒥㒝㒥㒙㒦㒙㒤㒡㒥㒡㒤㒙㒦㒛㒣㒡㒤㒟㒣㒙㒢㒥㒣㒦㒢㒝㒢㒛㒡㒦㒡㒡㒡㒝㒡㒙㒗㒛㒠㒡㒡㒡㒠㒙㒠㒗㒟㒡㒟㒟㒟㒙㒠㒗㒥㒜㒞㒝㒟㒞㒝㒥㒞㒟㒝㒞㒝㒙㒜㒥㒞㒡㒜㒝㒜㒙㒝㒚㒛㒡㒜㒢㒛㒙㒝㒛㒚㒡㒛㒟㒚㒙㒙㒥㒛㒗㒙㒝㒙㒛㒘㒦㒘㒡㒘㒝㒘㒙㒗㒥㒗㒡㒘㒢㒗㒙㒗㒗㒦㒡㒦㒟㒦㒙㒗㒗㒥㒡㒥㒝㒦㒟㒤㒥㒥㒟㒤㒞㒤㒙㒣㒥㒥㒡㒣㒝㒣㒙㒤㒛㒢㒡㒣㒣㒢㒙㒤㒛㒡㒡㒢㒟㒡㒙㒠㒥㒢㒘㒠㒝㒠㒛㒟㒦㒟㒡㒟㒝㒟㒙㒞㒥㒞㒡㒟㒣㒞㒙㒞㒗㒝㒡㒝㒟㒝㒙㒞㒗㒜㒡㒜㒝㒝㒠㒛㒥㒜㒟㒛㒞㒛㒙㒚㒥㒜㒡㒚㒝㒚㒙㒛㒜㒙㒡㒚㒤㒙㒙㒛㒛㒘㒡㒙㒟㒘㒙㒗㒥㒙㒙㒗㒝㒗㒛㒦㒦㒦㒡㒦㒝㒦㒙㒥㒥㒥㒡㒦㒤㒥㒙㒥㒗㒤㒡㒤㒟㒤㒙㒥㒗㒣㒡㒣㒝㒤㒡㒢㒥㒣㒟㒢㒞㒢㒙㒡㒥㒣㒡㒡㒝㒡㒙㒢㒝㒠㒡㒡㒥㒠㒙㒢㒛㒟㒡㒠㒟㒟㒙㒞㒥㒠㒚㒞㒝㒞㒛㒝㒦㒝㒡㒝㒝㒝㒙㒜㒥㒜㒡㒝㒥㒜㒙㒜㒗㒛㒡㒛㒟㒛㒙㒜㒗㒚㒡㒚㒝㒛㒢㒙㒥㒚㒟㒙㒞㒙㒙㒘㒥㒚㒡㒘㒝㒘㒙㒙㒞㒗㒡㒘㒦㒗㒙㒙㒛㒦㒡㒗㒟㒦㒙㒥㒥㒗㒛㒥㒝㒥㒛㒤㒦㒤㒡㒤㒝㒤㒙㒣㒥㒣㒡㒤㒦㒣㒙㒣㒗㒢㒡㒢㒟㒢㒙㒣㒗㒡㒡㒡㒝㒢㒣㒠㒥㒡㒟㒠㒞㒠㒙㒟㒥㒡㒡㒟㒝㒟㒙㒠㒟㒞㒡㒠㒗㒞㒙㒠㒛㒝㒡㒞㒟㒝㒙㒜㒥㒞㒜㒜㒝㒜㒛㒛㒦㒛㒡㒛㒝㒛㒙㒚㒥㒚㒡㒜㒗㒚㒙㒚㒗㒙㒡㒙㒟㒙㒙㒚㒗㒘㒡㒘㒝㒙㒤㒗㒥㒘㒟㒗㒞㒗㒙㒦㒥㒘㒡㒦㒝㒦㒙㒗㒠㒥㒡㒗㒘㒥㒙㒗㒛㒤㒡㒥㒟㒤㒙㒣㒥㒥㒝㒣㒝㒣㒛㒢㒦㒢㒡㒢㒝㒢㒙㒡㒥㒡㒡㒣㒘㒡㒙㒡㒗㒠㒡㒠㒟㒠㒙㒡㒗㒟㒡㒟㒝㒠㒥㒞㒥㒟㒟㒞㒞㒞㒙㒝㒥㒟㒡㒝㒝㒝㒙㒞㒡㒜㒡㒞㒙㒜㒙㒞㒛㒛㒡㒜㒟㒛㒙㒚㒥㒜㒞㒚㒝㒚㒛㒙㒦㒙㒡㒙㒝㒙㒙㒘㒥㒘㒡㒚㒙㒘㒙㒘㒗㒗㒡㒗㒟㒗㒙㒘㒗㒦㒡㒦㒝㒗㒦㒥㒥㒦㒟㒥㒞㒥㒙㒤㒥㒦㒡㒤㒝㒤㒙㒥㒢㒣㒡㒥㒚㒣㒙㒥㒛㒢㒡㒣㒟㒢㒙㒡㒥㒣㒟㒡㒝㒚㒞㒠㒥㒠㒡㒠㒝㒠㒙㒟㒥㒟㒡㒡㒚㒟㒙㒟㒗㒞㒡㒞㒟㒞㒙㒟㒗㒝㒡㒝㒝㒟㒗㒜㒥㒝㒟㒜㒞㒜㒙㒛㒥㒝㒡㒛㒝㒛㒙㒜㒣㒚㒡㒜㒛㒚㒙㒜㒛㒙㒡㒚㒟㒙㒙㒘㒥㒚㒠㒘㒝㒦㒠㒗㒥㒗㒡㒗㒝㒗㒙㒦㒥㒦㒡㒘㒛㒦㒙㒦㒗㒥㒡㒥㒟㒥㒙㒦㒗㒤㒡㒤㒝㒦㒘㒣㒥㒤㒟㒣㒞㒣㒙㒢㒥㒤㒡㒢㒝㒢㒙㒣㒤㒡㒡㒣㒜㒡㒙㒣㒛㒠㒡㒡㒟㒠㒙㒟㒥㒡㒡㒟㒝㒢㒛㒞㒥㒞㒡㒞㒝㒞㒙㒝㒥㒝㒡㒟㒜㒝㒙㒝㒗㒜㒡㒜㒟㒜㒙㒝㒗㒛㒡㒛㒝㒝㒙㒚㒥㒛㒟㒚㒞㒚㒙㒙㒥㒛㒡㒙㒝㒙㒙㒚㒥㒘㒡㒚㒝㒘㒙㒚㒛㒗㒡㒘㒟㒗㒙㒦㒥㒘㒢㒦㒝㒤㒠㒥㒥㒥㒡㒥㒝㒥㒙㒤㒥㒤㒡㒦㒝㒤㒙㒤㒗㒣㒡㒣㒟㒣㒙㒤㒗㒢㒡㒢㒝㒤㒚㒡㒥㒢㒟㒡㒞㒡㒙㒠㒥㒢㒡㒠㒝㒠㒙㒡㒦㒟㒡㒡㒞㒟㒙㒡㒛㒞㒡㒟㒟㒞㒙㒝㒥㒟㒣㒝㒝㒠㒛㒜㒥㒜㒡㒜㒝㒜㒙㒛㒥㒛㒡㒝㒞㒛㒙㒛㒗㒚㒡㒚㒟㒚㒙㒛㒗㒙㒡㒙㒝㒛㒛㒘㒥㒙㒟㒘㒞㒘㒙㒗㒥㒙㒡㒗㒝㒗㒙㒙㒗㒦㒡㒘㒟㒦㒙㒘㒛㒥㒡㒦㒟㒥㒙㒤㒥㒦㒤㒤㒝㒢㒠㒣㒥㒣㒡㒣㒝㒣㒙㒢㒥㒢㒡㒤㒟㒢㒙㒢㒗㒡㒡㒡㒟㒡㒙㒢㒗㒠㒡㒠㒝㒢㒜㒟㒥㒠㒟㒟㒞㒟㒙㒞㒥㒠㒡㒞㒝㒞㒙㒠㒘㒝㒡㒟㒠㒝㒙㒟㒛㒜㒡㒝㒟㒜㒙㒛㒥㒝㒥㒛㒝㒞㒛㒚㒥㒚㒡㒚㒝㒚㒙㒙㒥㒙㒡㒛㒠㒙㒙㒙㒗㒘㒡㒘㒟㒘㒙㒙㒗㒗㒡㒗㒝㒙㒝㒦㒥㒗㒟㒦㒞㒦㒙㒥㒥㒗㒡㒥㒝㒥㒙㒗㒙㒤㒡㒦㒡㒤㒙㒦㒛㒣㒡㒤㒟㒣㒙㒢㒥㒤㒦㒢㒝㒠㒠㒡㒥㒡㒡㒡㒝㒡㒙㒠㒥㒠㒡㒢㒡㒠㒙㒠㒗㒟㒡㒟㒟㒟㒙㒠㒗㒞㒡㒞㒝㒠㒞㒝㒥㒞㒟㒝㒞㒝㒙㒜㒥㒞㒡㒜㒝㒜㒙㒞㒚㒛㒡㒝㒢㒛㒙㒝㒛㒚㒡㒛㒟㒚㒙㒙㒥㒜㒗㒙㒝㒜㒛㒘㒥㒘㒡㒘㒝㒘㒙㒗㒥㒗㒡㒙㒢㒗㒙㒗㒗㒦㒡㒦㒟㒦㒙㒗㒗㒥㒡㒥㒝㒗㒟㒤㒥㒥㒟㒤㒞㒤㒙㒣㒥㒥㒡㒣㒝㒣㒙㒥㒛㒢㒡㒤㒣㒢㒙㒤㒛㒡㒡㒢㒟㒡㒙㒠㒥㒣㒘㒠㒝㒞㒠㒟㒥㒟㒡㒟㒝㒟㒙㒞㒥㒞㒡㒠㒣㒞㒙㒞㒗㒝㒡㒝㒟㒝㒙㒞㒗㒜㒡㒜㒝㒞㒠㒛㒥㒜㒟㒛㒞㒛㒙㒚㒥㒜㒡㒚㒝㒚㒙㒜㒜㒙㒡㒛㒤㒙㒙㒛㒛㒘㒡㒙㒟㒘㒙㒗㒥㒚㒙㒗㒝㒚㒛㒦㒥㒦㒡㒦㒝㒦㒙㒥㒥㒥㒡㒗㒤㒥㒙㒥㒗㒤㒡㒤㒟㒤㒙㒥㒗㒣㒡㒣㒝㒥㒡㒢㒥㒣㒟㒢㒞㒢㒙㒡㒥㒣㒡㒡㒝㒡㒙㒣㒝㒠㒡㒢㒥㒠㒙㒢㒛㒟㒡㒠㒟㒟㒙㒞㒥㒡㒚㒞㒝㒜㒠㒝㒥㒝㒡㒝㒝㒝㒙㒜㒥㒜㒡㒞㒥㒜㒙㒜㒗㒛㒡㒛㒟㒛㒙㒜㒗㒢㒘㒚㒝㒜㒢㒙㒥㒚㒟㒙㒞㒙㒙㒘㒥㒚㒡㒠㒥㒘㒙㒚㒞㒗㒡㒙㒦㒗㒙㒙㒛㒦㒡㒗㒟㒦㒙㒥㒥㒘㒛㒥㒝㒘㒛㒤㒥㒤㒡㒤㒝㒤㒙㒣㒥㒣㒡㒥㒦㒣㒙㒣㒗㒢㒡㒢㒟㒢㒙㒣㒗㒡㒡㒡㒝㒣㒣㒠㒥㒡㒟㒠㒞㒠㒙㒟㒥㒡㒡㒟㒝㒟㒙㒡㒟㒞㒡㒡㒗㒞㒙㒠㒛㒝㒡㒞㒟㒝㒙㒜㒥㒟㒜㒜㒝㒚㒠㒛㒥㒛㒡㒛㒝㒛㒙㒚㒥㒚㒡㒝㒗㒚㒙㒚㒗㒙㒡㒙㒟㒙㒙㒚㒗㒘㒡㒘㒝㒚㒤㒗㒥㒘㒟㒗㒞㒗㒙㒦㒥㒘㒡㒦㒝㒦㒙㒘㒠㒥㒡㒘㒘㒥㒙㒗㒛㒤㒡㒥㒟㒤㒙㒣㒥㒦㒝㒣㒝㒦㒛㒢㒥㒢㒡㒢㒝㒢㒙㒡㒥㒡㒡㒤㒘㒡㒙㒡㒗㒠㒡㒠㒟㒠㒙㒡㒗㒟㒡㒟㒝㒡㒥㒞㒥㒟㒟㒞㒞㒞㒙㒝㒥㒟㒡㒝㒝㒝㒙㒟㒡㒜㒡㒟㒙㒜㒙㒞㒛㒛㒡㒜㒟㒛㒙㒚㒥㒝㒞㒚㒝㒘㒠㒙㒥㒙㒡㒙㒝㒙㒙㒘㒥㒘㒡㒛㒙㒘㒙㒘㒗㒗㒡㒗㒟㒗㒙㒘㒗㒦㒡㒦㒝㒘㒦㒥㒥㒦㒟㒥㒞㒥㒙㒤㒥㒦㒡㒤㒝㒤㒙㒦㒢㒣㒡㒦㒚㒣㒙㒥㒛㒢㒡㒣㒟㒢㒙㒡㒥㒤㒟㒡㒝㒤㒛㒠㒥㒠㒡㒠㒝㒠㒙㒟㒥㒟㒡㒢㒚㒟㒙㒟㒗㒞㒡㒞㒟㒞㒙㒟㒗㒝㒡㒝㒝㒠㒗㒜㒥㒝㒟㒜㒞㒜㒙㒛㒥㒝㒡㒛㒝㒛㒙㒝㒣㒚㒡㒝㒛㒚㒙㒜㒛㒙㒡㒚㒟㒙㒙㒘㒥㒛㒠㒘㒝㒦㒠㒗㒥㒗㒡㒗㒝㒗㒙㒦㒥㒦㒡㒙㒛㒦㒙㒦㒗㒥㒡㒥㒟㒥㒙㒦㒗㒤㒡㒤㒝㒗㒘㒣㒥㒤㒟㒣㒞㒣㒙㒢㒥㒤㒡㒢㒝㒢㒙㒤㒤㒡㒡㒤㒜㒡㒙㒣㒛㒠㒡㒡㒟㒠㒙㒟㒥㒢㒡㒟㒝㒢㒛㒞㒥㒞㒡㒞㒝㒞㒙㒝㒥㒝㒡㒠㒜㒝㒙㒝㒗㒜㒡㒜㒟㒜㒙㒝㒗㒛㒡㒛㒝㒞㒙㒚㒥㒛㒟㒚㒞㒚㒙㒙㒥㒛㒡㒙㒝㒙㒙㒛㒥㒘㒡㒛㒝㒘㒙㒚㒛㒗㒡㒘㒟㒗㒙㒦㒥㒙㒢㒦㒝㒟㒞㒥㒥㒥㒡㒥㒝㒥㒙㒤㒥㒤㒡㒗㒝㒤㒙㒤㒗㒣㒡㒣㒟㒣㒙㒤㒗㒢㒡㒢㒝㒥㒚㒡㒥㒢㒟㒡㒞㒡㒙㒠㒥㒢㒡㒠㒝㒠㒙㒢㒦㒟㒡㒢㒞㒟㒙㒡㒛㒞㒡㒟㒟㒞㒙㒝㒥㒠㒣㒝㒝㒝㒛㒜㒦㒜㒡㒜㒝㒜㒙㒛㒥㒛㒡㒞㒞㒛㒙㒛㒗㒚㒡㒚㒟㒚㒙㒛㒗㒙㒡㒙㒝㒜㒛㒘㒥㒙㒟㒘㒞㒘㒙㒗㒥㒙㒡㒗㒝㒗㒙㒚㒗㒦㒡㒙㒟㒦㒙㒘㒛㒥㒡㒦㒟㒥㒙㒤㒥㒗㒤㒤㒝㒤㒛㒣㒦㒣㒡㒣㒝㒣㒙㒢㒥㒢㒡㒥㒟㒢㒙㒢㒗㒡㒡㒡㒟㒡㒙㒢㒗㒠㒡㒠㒝㒣㒜㒟㒥㒠㒟㒟㒞㒟㒙㒞㒥㒠㒡㒞㒝㒞㒙㒡㒘㒝㒡㒠㒠㒝㒙㒟㒛㒜㒡㒝㒟㒜㒙㒛㒥㒞㒥㒛㒝㒛㒛㒚㒦㒚㒡㒚㒝㒚㒙㒙㒥㒙㒡㒜㒠㒙㒙㒙㒗㒘㒡㒘㒟㒘㒙㒙㒗㒗㒡㒗㒝㒚㒝㒦㒥㒗㒟㒦㒞㒦㒙㒥㒥㒗㒡㒥㒝㒥㒙㒘㒙㒤㒡㒗㒡㒤㒙㒦㒛㒣㒡㒤㒟㒣㒙㒢㒥㒥㒦㒢㒝㒠㒠㒡㒥㒡㒡㒡㒝㒡㒙㒠㒥㒠㒡㒣㒡㒠㒙㒠㒗㒟㒡㒟㒟㒟㒙㒠㒗㒞㒡㒞㒝㒡㒞㒝㒥㒞㒟㒝㒞㒝㒙㒜㒥㒞㒡㒜㒝㒜㒙㒟㒚㒛㒡㒞㒢㒛㒙㒝㒛㒚㒡㒛㒟㒚㒙㒙㒥㒝㒗㒙㒝㒜㒛㒘㒥㒘㒡㒘㒝㒘㒙㒗㒥㒗㒡㒚㒢㒗㒙㒗㒗㒦㒡㒦㒟㒦㒙㒗㒗㒥㒡㒥㒝㒘㒟㒤㒥㒥㒟㒤㒞㒤㒙㒣㒥㒥㒡㒣㒝㒣㒙㒦㒛㒢㒡㒥㒣㒢㒙㒤㒛㒡㒡㒢㒟㒡㒙㒠㒥㒤㒘㒠㒝㒥㒚㒟㒥㒟㒡㒟㒝㒟㒙㒞㒥㒞㒡㒡㒣㒞㒙㒞㒗㒝㒡㒝㒟㒝㒙㒟㒥㒜㒡㒜㒝㒜㒚㒛㒥㒢㒥㒛㒝㒠㒟㒚㒥㒛㒣㒚㒝㒚㒙㒝㒜㒙㒡㒠㒞㒙㒙㒘㒥㒘㒡㒚㒝㒘㒙㒗㒥㒛㒘㒗㒝㒚㒠㒦㒥㒘㒥㒦㒝㒘㒙㒥㒥㒥㒡㒘㒤㒥㒙㒘㒜㒤㒡㒟㒘㒤㒙㒥㒥㒣㒡㒣㒝㒦㒠㒢㒥㒦㒘㒢㒝㒜㒜㒡㒥㒢㒣㒡㒝㒡㒙㒤㒞㒠㒡㒡㒛㒠㒙㒟㒥㒟㒡㒟㒝㒟㒙㒞㒥㒢㒘㒞㒝㒡㒢㒝㒥㒝㒣㒝㒝㒞㒙㒜㒥㒜㒡㒜㒞㒜㒙㒡㒗㒛㒡㒞㒤㒛㒙㒜㒗㒚㒡㒚㒝㒝㒠㒙㒥㒡㒠㒙㒝㒙㒙㒘㒥㒚㒡㒘㒝㒘㒙㒛㒜㒗㒡㒚㒤㒗㒙㒣㒢㒦㒡㒘㒝㒦㒙㒥㒥㒙㒘㒥㒝㒘㒠㒤㒥㒠㒞㒤㒝㒥㒙㒣㒥㒣㒡㒣㒞㒣㒙㒟㒢㒢㒡㒥㒤㒢㒙㒤㒥㒡㒡㒡㒝㒡㒛㒠㒥㒗㒥㒠㒝㒜㒛㒟㒥㒠㒡㒟㒝㒟㒙㒟㒗㒞㒡㒣㒟㒞㒙㒝㒦㒝㒡㒞㒟㒝㒙㒜㒥㒠㒘㒜㒝㒟㒚㒛㒥㒛㒡㒛㒝㒝㒙㒚㒥㒚㒡㒝㒤㒚㒙㒝㒜㒙㒡㒙㒝㒙㒚㒚㒗㒘㒡㒘㒝㒛㒡㒗㒥㒙㒙㒗㒝㒗㒙㒦㒥㒗㒣㒦㒝㒦㒙㒙㒞㒥㒡㒦㒥㒥㒙㒤㒥㒤㒡㒥㒟㒤㒙㒣㒥㒗㒛㒣㒝㒤㒡㒢㒥㒢㒡㒢㒝㒢㒙㒡㒥㒡㒡㒤㒤㒡㒙㒤㒟㒠㒡㒠㒟㒠㒙㒠㒥㒟㒡㒟㒝㒟㒛㒞㒥㒛㒥㒞㒝㒡㒠㒝㒥㒠㒡㒝㒝㒝㒙㒝㒗㒜㒡㒞㒛㒜㒙㒡㒣㒛㒡㒜㒟㒛㒙㒚㒥㒞㒘㒚㒝㒙㒗㒙㒥㒙㒡㒙㒝㒛㒙㒘㒥㒘㒡㒛㒤㒘㒙㒛㒜㒗㒡㒙㒣㒗㒙㒘㒗㒦㒡㒦㒝㒙㒡㒥㒥㒝㒞㒥㒝㒥㒙㒤㒥㒥㒣㒦㒝㒤㒙㒗㒞㒣㒡㒠㒘㒣㒙㒢㒥㒢㒡㒣㒟㒤㒟㒡㒥㒥㒛㒡㒝㒝㒤㒠㒥㒠㒡㒠㒝㒡㒛㒟㒥㒟㒡㒣㒘㒟㒙㒛㒠㒞㒡㒞㒝㒞㒙㒝㒥㒝㒡㒝㒝㒠㒠㒜㒥㒠㒜㒜㒝㒜㒛㒛㒥㒜㒡㒛㒝㒛㒙㒛㒗㒚㒡㒝㒛㒚㒙㒝㒜㒙㒡㒚㒟㒙㒙㒘㒥㒜㒘㒘㒝㒗㒗㒗㒥㒗㒡㒗㒝㒙㒙㒦㒥㒦㒡㒙㒤㒦㒙㒙㒜㒥㒡㒗㒣㒥㒙㒦㒗㒤㒡㒤㒝㒗㒡㒣㒥㒠㒜㒣㒝㒣㒙㒢㒥㒣㒣㒢㒝㒢㒙㒥㒞㒡㒡㒢㒢㒡㒙㒠㒥㒠㒡㒡㒟㒠㒙㒟㒥㒣㒛㒟㒝㒛㒤㒞㒥㒞㒡㒞㒝㒟㒛㒝㒥㒝㒡㒡㒘㒝㒙㒗㒚㒜㒡㒜㒝㒜㒙㒛㒥㒛㒡㒛㒝㒞㒠㒚㒥㒞㒜㒚㒝㒚㒛㒙㒥㒚㒡㒙㒝㒙㒙㒙㒗㒘㒡㒜㒠㒘㒙㒛㒜㒗㒡㒚㒝㒗㒙㒦㒥㒦㒤㒦㒝㒝㒝㒥㒥㒢㒢㒥㒝㒦㒙㒤㒥㒤㒡㒤㒠㒤㒙㒙㒗㒣㒡㒣㒟㒣㒙㒤㒗㒢㒡㒢㒝㒥㒠㒡㒥㒤㒢㒡㒝㒡㒙㒠㒥㒢㒡㒠㒝㒠㒙㒣㒜㒟㒡㒢㒤㒟㒙㒞㒥㒞㒢㒟㒟㒞㒙㒝㒥㒡㒙㒝㒝㒙㒤㒜㒥㒜㒡㒜㒝㒝㒛㒛㒥㒛㒡㒞㒦㒛㒙㒗㒠㒚㒡㒚㒝㒚㒙㒛㒗㒙㒡㒙㒝㒜㒣㒘㒥㒥㒜㒘㒝㒘㒙㒗㒥㒗㒡㒗㒝㒗㒙㒚㒜㒦㒡㒚㒗㒦㒙㒦㒗㒥㒡㒦㒝㒥㒙㒤㒥㒤㒤㒤㒝㒡㒝㒣㒥㒗㒘㒣㒝㒤㒛㒢㒥㒢㒡㒥㒤㒢㒙㒤㒦㒡㒡㒡㒝㒡㒙㒢㒥㒠㒡㒠㒝㒣㒠㒟㒥㒣㒘㒟㒝㒟㒙㒞㒦㒟㒣㒞㒝㒞㒙㒡㒝㒝㒡㒚㒤㒝㒙㒜㒥㒜㒡㒝㒟㒜㒙㒛㒥㒟㒚㒛㒝㒘㒠㒚㒥㒚㒡㒚㒝㒛㒛㒙㒥㒙㒡㒝㒗㒙㒙㒦㒜㒘㒡㒘㒝㒘㒙㒗㒥㒗㒡㒗㒝㒚㒠㒦㒥㒚㒛㒦㒝㒦㒛㒥㒥㒦㒡㒥㒝㒥㒙㒥㒘㒤㒡㒦㒘㒤㒚㒗㒜㒣㒡㒦㒝㒣㒙㒢㒥㒢㒤㒢㒝㒠㒡㒡㒥㒘㒠㒡㒝㒢㒛㒠㒥㒠㒡㒣㒤㒠㒙㒞㒣㒟㒡㒟㒝㒟㒙㒠㒥㒞㒡㒞㒝㒡㒠㒝㒥㒡㒘㒝㒝㒟㒟㒜㒥㒝㒣㒜㒝㒜㒙㒟㒝㒛㒡㒛㒥㒛㒚㒚㒥㒚㒡㒛㒟㒚㒙㒙㒥㒝㒚㒙㒝㒥㒤㒘㒥㒘㒡㒘㒝㒙㒛㒗㒥㒗㒡㒛㒗㒗㒙㒥㒡㒦㒡㒦㒝㒦㒙㒗㒗㒥㒡㒥㒝㒘㒤㒤㒥㒡㒜㒤㒝㒤㒙㒣㒥㒣㒡㒣㒝㒣㒙㒦㒜㒢㒡㒦㒘㒢㒙㒢㒗㒡㒡㒢㒝㒡㒙㒠㒥㒠㒤㒠㒝㒣㒗㒟㒥㒣㒘㒟㒝㒠㒛㒞㒥㒞㒡㒡㒤㒞㒙㒜㒣㒝㒡㒝㒝㒝㒙㒞㒥㒜㒡㒜㒝㒟㒠㒛㒥㒟㒘㒛㒝㒝㒟㒚㒥㒛㒣㒚㒝㒚㒙㒝㒝㒙㒡㒦㒘㒙㒙㒘㒥㒘㒡㒙㒟㒘㒙㒗㒥㒛㒚㒗㒝㒤㒥㒦㒥㒦㒡㒦㒝㒗㒛㒥㒥㒥㒡㒙㒗㒥㒙㒡㒠㒤㒡㒤㒝㒤㒙㒥㒗㒣㒡㒣㒝㒦㒤㒢㒥㒤㒗㒢㒝㒢㒙㒡㒥㒡㒡㒡㒝㒡㒙㒤㒜㒠㒡㒤㒘㒠㒙㒠㒗㒟㒡㒠㒝㒟㒙㒞㒥㒞㒤㒞㒝㒢㒜㒝㒥㒡㒘㒝㒝㒠㒙㒜㒥㒜㒡㒜㒡㒜㒙㒣㒙㒛㒡㒗㒗㒛㒙㒛㒥㒚㒡㒚㒝㒚㒝㒙㒥㒞㒣㒙㒝㒙㒜㒘㒥㒙㒣㒘㒝㒘㒙㒛㒜㒗㒡㒚㒞㒗㒙㒦㒥㒦㒡㒘㒝㒦㒙㒥㒥㒙㒘㒥㒝㒘㒠㒤㒥㒤㒡㒤㒞㒥㒛㒣㒥㒣㒡㒦㒥㒣㒙㒤㒝㒢㒡㒢㒝㒢㒙㒣㒗㒡㒡㒡㒝㒤㒢㒠㒥㒢㒙㒠㒝㒠㒙㒟㒥㒠㒣㒟㒝㒟㒙㒢㒟㒞㒡㒟㒥㒞㒙㒝㒥㒝㒡㒝㒝㒝㒙㒜㒥㒠㒘㒜㒝㒟㒣㒛㒥㒛㒣㒛㒝㒜㒙㒚㒥㒚㒡㒚㒡㒚㒙㒗㒙㒙㒡㒜㒤㒙㒙㒛㒥㒘㒡㒘㒝㒘㒝㒗㒥㒙㒟㒗㒝㒝㒗㒦㒥㒗㒣㒦㒝㒦㒙㒙㒜㒥㒡㒤㒛㒥㒙㒤㒥㒤㒡㒦㒝㒤㒙㒣㒥㒗㒘㒣㒝㒦㒠㒢㒥㒥㒗㒢㒝㒣㒛㒡㒥㒡㒡㒤㒥㒡㒙㒝㒠㒠㒡㒠㒝㒠㒙㒡㒗㒟㒡㒟㒝㒢㒢㒞㒥㒛㒜㒞㒝㒞㒙㒝㒥㒞㒣㒝㒝㒝㒙㒠㒟㒜㒡㒟㒢㒜㒙㒛㒥㒛㒡㒜㒟㒛㒙㒚㒥㒞㒜㒚㒝㒦㒤㒙㒥㒙㒡㒙㒝㒙㒙㒘㒥㒘㒡㒛㒤㒘㒙㒛㒠㒗㒡㒗㒟㒗㒙㒗㒥㒦㒡㒦㒝㒦㒝㒥㒥㒘㒟㒥㒝㒘㒠㒤㒥㒥㒣㒤㒝㒤㒙㒗㒜㒣㒡㒢㒛㒣㒙㒢㒥㒢㒡㒤㒝㒢㒙㒡㒥㒥㒘㒡㒝㒤㒠㒠㒥㒣㒗㒠㒝㒡㒛㒟㒥㒟㒡㒢㒥㒟㒙㒛㒠㒞㒡㒞㒝㒞㒙㒟㒗㒝㒡㒝㒝㒠㒢㒜㒥㒚㒣㒜㒝㒜㒙㒛㒥㒜㒣㒛㒝㒛㒙㒞㒟㒚㒡㒗㒘㒚㒙㒙㒥㒙㒡㒚㒟㒙㒙㒘㒥㒜㒜㒘㒝㒛㒡㒗㒥㒗㒡㒗㒝㒗㒙㒦㒥㒦㒡㒙㒤㒦㒙㒙㒠㒥㒡㒥㒟㒥㒙㒥㒥㒤㒡㒤㒝㒤㒝㒣㒥㒗㒤㒣㒝㒦㒠㒢㒥㒣㒣㒢㒝㒢㒙㒥㒜㒡㒡㒙㒜㒡㒙㒠㒥㒠㒡㒢㒝㒠㒙㒟㒥㒣㒘㒟㒝㒢㒠㒞㒥㒗㒙㒞㒝㒠㒙㒝㒥㒝㒡㒠㒤㒝㒙㒠㒜㒜㒡㒠㒙㒜㒙㒜㒥㒛㒡㒛㒝㒛㒝㒚㒥㒣㒙㒚㒝㒝㒠㒙㒥㒜㒡㒙㒝㒙㒙㒙㒙㒘㒡㒙㒡㒘㒙㒗㒢㒗㒡㒘㒟㒗㒙㒦㒥㒚㒘㒦㒝㒙㒚㒥㒥㒥㒡㒥㒝㒗㒙㒤㒥㒤㒡㒗㒤㒤㒙㒗㒜㒣㒡㒣㒝㒣㒚㒤㒗㒢㒡㒢㒝㒥㒡㒡㒥㒚㒜㒡㒝㒡㒙㒠㒥㒡㒣㒠㒝㒠㒙㒣㒞㒟㒡㒠㒚㒟㒚㒞㒥㒞㒡㒟㒟㒠㒙㒝㒥㒡㒛㒝㒝㒝㒦㒜㒦㒜㒡㒜㒝㒜㒙㒡㒘㒛㒡㒞㒤㒛㒙㒞㒟㒚㒡㒚㒟㒚㒙㒚㒥㒙㒡㒙㒝㒙㒝㒘㒥㒢㒝㒘㒝㒛㒠㒗㒥㒚㒡㒗㒝㒗㒙㒗㒙㒦㒡㒜㒚㒦㒙㒗㒟㒥㒡㒘㒝㒥㒙㒤㒥㒤㒥㒤㒝㒤㒥㒣㒥㒤㒚㒣㒞㒦㒙㒢㒥㒢㒡㒢㒡㒢㒙㒝㒛㒡㒡㒣㒗㒡㒙㒣㒥㒠㒡㒠㒝㒠㒞㒟㒥㒦㒥㒟㒝㒤㒥㒞㒥㒟㒡㒞㒝㒞㒙㒞㒚㒝㒡㒢㒟㒝㒙㒝㒗㒜㒡㒝㒟㒜㒙㒛㒥㒟㒘㒛㒝㒞㒚㒚㒥㒚㒡㒚㒝㒜㒙㒙㒥㒙㒡㒜㒤㒙㒙㒜㒜㒘㒡㒘㒝㒘㒚㒙㒗㒗㒡㒗㒝㒚㒡㒦㒥㒛㒛㒦㒝㒦㒙㒥㒥㒦㒣㒥㒝㒥㒙㒘㒞㒤㒡㒙㒗㒤㒙㒣㒥㒣㒡㒤㒟㒣㒙㒢㒥㒦㒛㒢㒝㒦㒣㒡㒥㒡㒡㒡㒝㒡㒙㒠㒥㒠㒡㒣㒤㒠㒙㒣㒟㒟㒡㒟㒟㒟㒙㒟㒥㒞㒡㒞㒝㒞㒞㒝㒥㒚㒥㒝㒝㒠㒠㒜㒥㒝㒣㒜㒝㒜㒙㒟㒜㒛㒡㒞㒞㒛㒙㒚㒥㒚㒡㒜㒝㒚㒙㒙㒥㒝㒘㒙㒝㒜㒠㒘㒥㒘㒡㒘㒞㒙㒛㒗㒥㒗㒡㒚㒥㒗㒙㒤㒜㒦㒡㒦㒝㒦㒙㒗㒗㒥㒡㒥㒝㒘㒢㒤㒥㒢㒘㒤㒝㒤㒙㒣㒥㒤㒣㒣㒝㒣㒙㒦㒟㒢㒡㒟㒤㒢㒙㒡㒥㒡㒡㒡㒝㒡㒙㒠㒥㒤㒘㒠㒝㒣㒣㒟㒥㒟㒣㒟㒝㒠㒙㒞㒥㒞㒡㒞㒢㒞㒙㒟㒠㒝㒢㒠㒤㒝㒙㒟㒥㒜㒡㒜㒝㒜㒞㒛㒥㒚㒙㒛㒝㒢㒘㒚㒥㒛㒣㒚㒝㒚㒙㒝㒜㒙㒡㒘㒛㒙㒙㒘㒥㒘㒡㒚㒝㒘㒙㒗㒥㒛㒘㒗㒝㒚㒠㒦㒥㒙㒗㒦㒝㒗㒛㒥㒥㒥㒡㒘㒥㒥㒙㒥㒝㒤㒢㒤㒝㒤㒙㒥㒗㒣㒡㒣㒝㒦㒢㒢㒥㒟㒜㒢㒝㒢㒙㒡㒥㒢㒣㒡㒝㒡㒙㒤㒟㒠㒡㒡㒝㒠㒚㒟㒥㒟㒡㒠㒟㒟㒙㒞㒥㒢㒜㒞㒝㒚㒤㒝㒥㒝㒡㒝㒝㒝㒙㒜㒥㒜㒡㒟㒤㒜㒙㒟㒠㒛㒡㒛㒟㒛㒙㒛㒥㒚㒡㒚㒝㒚㒞㒙㒥㒜㒟㒙㒝㒜㒠㒘㒥㒙㒣㒘㒝㒘㒙㒛㒜㒗㒡㒦㒛㒗㒙㒦㒥㒦㒡㒘㒝㒦㒙㒥㒥㒙㒘㒥㒝㒘㒠㒤㒥㒗㒗㒤㒝㒥㒛㒣㒥㒣㒡㒦㒥㒣㒙㒟㒠㒢㒡㒢㒝㒢㒙㒣㒗㒡㒡㒡㒝㒤㒢㒠㒥㒞㒝㒠㒝㒠㒙㒟㒥㒠㒣㒟㒝㒟㒙㒢㒟㒞㒡㒛㒘㒞㒙㒝㒥㒝㒡㒞㒟㒝㒙㒜㒥㒠㒜㒜㒝㒗㒙㒛㒥㒛㒡㒛㒝㒛㒙㒚㒥㒚㒡㒝㒤㒚㒙㒝㒠㒙㒡㒙㒟㒙㒙㒙㒥㒘㒡㒘㒝㒘㒞㒗㒥㒛㒤㒗㒝㒚㒠㒦㒥㒙㒡㒦㒝㒦㒙㒦㒛㒥㒡㒜㒡㒥㒙㒡㒘㒤㒡㒥㒝㒤㒙㒣㒥㒤㒗㒣㒝㒘㒛㒢㒥㒢㒦㒢㒝㒣㒛㒡㒥㒡㒡㒤㒤㒡㒙㒣㒦㒠㒡㒠㒝㒠㒙㒡㒥㒟㒡㒟㒝㒢㒠㒞㒥㒢㒘㒞㒝㒞㒙㒝㒦㒞㒣㒝㒝㒝㒙㒠㒝㒜㒡㒝㒥㒜㒙㒛㒥㒛㒡㒜㒟㒛㒙㒚㒥㒞㒚㒚㒝㒛㒡㒙㒥㒙㒡㒙㒝㒚㒛㒘㒥㒘㒡㒜㒗㒘㒙㒙㒝㒗㒡㒗㒝㒗㒙㒦㒥㒦㒡㒦㒝㒙㒠㒥㒥㒙㒛㒥㒝㒥㒛㒤㒥㒥㒡㒤㒝㒤㒙㒤㒛㒣㒡㒠㒡㒣㒙㒦㒜㒢㒡㒥㒝㒢㒙㒡㒥㒢㒗㒡㒝㒣㒗㒠㒥㒦㒟㒠㒝㒡㒛㒟㒥㒟㒡㒢㒤㒟㒙㒝㒣㒞㒡㒞㒝㒞㒙㒟㒥㒝㒡㒝㒝㒠㒠㒜㒥㒠㒘㒜㒝㒞㒟㒛㒥㒜㒣㒛㒝㒛㒙㒞㒝㒚㒡㒛㒞㒚㒙㒙㒥㒙㒡㒚㒟㒙㒙㒘㒥㒜㒚㒘㒝㒤㒤㒗㒥㒗㒡㒗㒝㒘㒛㒦㒥㒦㒡㒚㒗㒦㒙㒦㒠㒥㒡㒥㒝㒥㒙㒦㒗㒤㒡㒤㒝㒗㒤㒣㒥㒠㒜㒣㒝㒣㒙㒢㒥㒢㒡㒢㒝㒢㒙㒥㒜㒡㒡㒥㒘㒡㒙㒡㒗㒠㒡㒡㒝㒠㒙㒟㒥㒠㒗㒟㒝㒢㒗㒞㒥㒢㒘㒞㒝㒟㒛㒝㒥㒝㒡㒠㒤㒝㒙㒛㒣㒜㒡㒜㒝㒜㒙㒝㒥㒛㒡㒛㒝㒞㒠㒚㒥㒞㒘㒚㒝㒜㒟㒙㒥㒚㒣㒙㒝㒙㒙㒜㒝㒘㒡㒥㒘㒘㒙㒗㒥㒗㒡㒘㒟㒗㒙㒦㒥㒚㒚㒦㒝㒠㒥㒥㒥㒥㒡㒥㒝㒦㒛㒤㒥㒤㒡㒘㒗㒤㒙㒠㒠㒣㒡㒣㒝㒣㒙㒤㒗㒢㒡㒢㒝㒥㒤㒡㒥㒛㒞㒡㒝㒡㒙㒠㒥㒠㒡㒠㒝㒠㒙㒣㒜㒟㒡㒣㒘㒟㒙㒟㒗㒞㒡㒟㒝㒞㒙㒝㒥㒞㒗㒝㒝㒡㒜㒜㒥㒠㒘㒜㒝㒝㒛㒛㒥㒛㒡㒞㒤㒛㒙㒢㒤㒚㒡㒚㒝㒚㒙㒛㒥㒙㒡㒙㒝㒜㒠㒘㒥㒜㒘㒘㒝㒠㒡㒗㒥㒙㒡㒗㒝㒗㒙㒚㒜㒦㒡㒙㒤㒦㒙㒙㒡㒥㒡㒦㒝㒥㒙㒤㒥㒥㒗㒤㒝㒜㒡㒣㒥㒗㒘㒣㒝㒦㒙㒢㒥㒢㒡㒢㒣㒢㒙㒣㒙㒡㒡㒝㒠㒡㒙㒢㒗㒠㒡㒠㒝㒣㒠㒟㒥㒢㒢㒟㒝㒟㒙㒞㒥㒠㒡㒞㒝㒞㒙㒡㒜㒝㒡㒠㒤㒝㒙㒜㒥㒜㒢㒝㒟㒜㒙㒛㒥㒟㒙㒛㒝㒣㒤㒚㒥㒚㒡㒚㒝㒛㒛㒙㒥㒙㒡㒜㒦㒙㒙㒙㒢㒘㒢㒘㒝㒘㒙㒙㒗㒗㒡㒗㒝㒚㒣㒦㒥㒗㒞㒦㒞㒦㒙㒥㒥㒥㒡㒥㒝㒥㒙㒘㒜㒤㒡㒘㒗㒤㒙㒤㒗㒣㒡㒤㒝㒣㒙㒢㒥㒣㒗㒢㒝㒛㒥㒡㒥㒥㒘㒡㒝㒤㒙㒠㒥㒠㒡㒠㒣㒠㒙㒥㒢㒟㒡㒡㒗㒟㒙㒡㒥㒞㒡㒞㒝㒞㒟㒝㒥㒞㒝㒝㒝㒝㒢㒜㒦㒟㒡㒜㒝㒜㒙㒜㒛㒛㒡㒦㒣㒛㒙㒜㒟㒚㒡㒝㒝㒚㒙㒙㒥㒚㒘㒙㒝㒠㒝㒘㒥㒠㒣㒘㒝㒙㒙㒙㒚㒗㒡㒗㒤㒗㒙㒜㒗㒦㒡㒦㒢㒦㒙㒗㒗㒦㒠㒥㒝㒘㒠㒤㒥㒗㒢㒤㒝㒤㒙㒣㒥㒥㒡㒣㒝㒣㒙㒦㒜㒢㒡㒥㒤㒢㒙㒡㒥㒡㒢㒢㒟㒡㒙㒠㒥㒤㒙㒠㒝㒡㒡㒟㒥㒟㒡㒟㒝㒠㒛㒞㒥㒞㒡㒡㒦㒞㒙㒟㒝㒝㒡㒝㒝㒝㒙㒞㒗㒜㒡㒜㒝㒟㒣㒛㒥㒝㒙㒛㒝㒛㒙㒚㒥㒚㒡㒚㒝㒚㒙㒝㒜㒙㒡㒝㒗㒙㒙㒙㒗㒘㒡㒙㒝㒘㒙㒗㒥㒘㒘㒗㒝㒤㒝㒦㒥㒚㒘㒦㒝㒙㒙㒥㒥㒥㒡㒥㒤㒥㒙㒦㒣㒤㒡㒚㒛㒤㒙㒥㒗㒣㒡㒣㒝㒦㒠㒢㒥㒡㒟㒢㒝㒢㒙㒡㒥㒣㒡㒡㒝㒡㒙㒤㒜㒠㒡㒣㒤㒠㒙㒢㒛㒟㒡㒠㒟㒟㒙㒞㒥㒢㒙㒞㒝㒤㒜㒝㒥㒝㒡㒝㒝㒞㒛㒜㒥㒜㒡㒟㒦㒜㒙㒘㒠㒛㒡㒛㒝㒛㒙㒜㒗㒚㒡㒚㒝㒝㒣㒙㒥㒛㒗㒙㒞㒙㒙㒘㒥㒙㒣㒘㒝㒘㒙㒛㒠㒗㒡㒤㒘㒗㒙㒦㒥㒦㒡㒦㒝㒦㒙㒥㒥㒙㒘㒥㒝㒘㒤㒤㒥㒤㒣㒤㒝㒥㒙㒣㒥㒣㒡㒣㒤㒣㒙㒥㒣㒢㒡㒥㒤㒢㒙㒤㒥㒡㒡㒡㒝㒡㒠㒠㒥㒘㒘㒠㒝㒟㒙㒟㒥㒠㒣㒟㒝㒟㒙㒢㒜㒞㒡㒝㒛㒞㒙㒝㒥㒝㒡㒟㒝㒝㒙㒜㒥㒠㒘㒜㒝㒟㒠㒛㒥㒞㒗㒛㒝㒜㒛㒚㒥㒚㒡㒝㒥㒚㒙㒦㒠㒙㒡㒙㒝㒙㒙㒚㒗㒘㒡㒘㒝㒛㒢㒗㒥㒜㒟㒗㒝㒗㒙㒦㒥㒗㒣㒦㒝㒦㒙㒙㒟㒥㒡㒢㒘㒥㒙㒤㒥㒤㒡㒥㒟㒤㒙㒣㒥㒗㒜㒣㒝㒟㒞㒢㒥㒢㒡㒢㒝㒢㒙㒡㒥㒡㒡㒤㒤㒡㒙㒤㒠㒠㒡㒠㒟㒠㒙㒠㒥㒟㒡㒟㒝㒟㒠㒞㒥㒢㒤㒞㒝㒡㒠㒝㒥㒠㒡㒝㒝㒝㒙㒝㒜㒜㒡㒡㒜㒜㒙㒢㒥㒛㒡㒜㒟㒛㒙㒚㒥㒞㒘㒚㒝㒢㒘㒙㒥㒙㒡㒙㒝㒛㒙㒘㒥㒘㒡㒛㒤㒘㒙㒛㒜㒗㒡㒡㒘㒗㒙㒘㒥㒦㒡㒦㒝㒙㒠㒥㒥㒙㒘㒥㒝㒡㒙㒤㒥㒥㒡㒤㒝㒤㒙㒤㒜㒣㒡㒝㒘㒣㒙㒦㒜㒢㒡㒥㒝㒢㒙㒡㒥㒢㒙㒡㒝㒘㒝㒠㒥㒤㒜㒠㒝㒡㒙㒟㒥㒟㒡㒟㒥㒟㒙㒤㒗㒞㒡㒞㒢㒞㒙㒟㒗㒝㒡㒝㒝㒠㒠㒜㒥㒟㒢㒜㒝㒜㒙㒛㒥㒝㒡㒛㒝㒛㒙㒞㒜㒚㒡㒝㒤㒚㒙㒙㒥㒙㒢㒚㒟㒙㒙㒘㒥㒜㒙㒘㒝㒙㒡㒗㒥㒗㒡㒗㒝㒘㒛㒦㒥㒦㒡㒙㒦㒦㒙㒗㒝㒥㒡㒥㒝㒥㒙㒦㒗㒤㒡㒤㒝㒗㒣㒣㒥㒥㒙㒣㒝㒣㒙㒢㒥㒢㒡㒢㒝㒢㒙㒥㒜㒡㒡㒥㒗㒡㒙㒡㒗㒠㒡㒡㒝㒠㒙㒟㒥㒠㒙㒟㒝㒜㒝㒞㒥㒢㒘㒞㒝㒡㒙㒝㒥㒝㒡㒝㒥㒝㒙㒞㒣㒜㒡㒢㒛㒜㒙㒝㒗㒛㒡㒛㒝㒞㒠㒚㒥㒙㒟㒚㒝㒚㒙㒙㒥㒛㒡㒙㒝㒙㒙㒜㒜㒘㒡㒛㒤㒘㒙㒚㒛㒗㒡㒘㒟㒗㒙㒦㒥㒚㒙㒦㒝㒘㒞㒥㒥㒥㒡㒥㒝㒦㒛㒤㒥㒤㒡㒗㒦㒤㒙㒠㒠㒣㒡㒣㒝㒣㒙㒤㒗㒢㒡㒢㒝㒥㒣㒡㒥㒢㒜㒡㒝㒡㒙㒠㒥㒡㒣㒠㒝㒠㒙㒣㒠㒟㒡㒜㒘㒟㒙㒞㒥㒞㒡㒞㒝㒞㒙㒝㒥㒡㒘㒝㒝㒠㒤㒜㒥㒜㒣㒜㒝㒝㒙㒛㒥㒛㒡㒛㒥㒛㒙㒝㒣㒚㒡㒝㒤㒚㒙㒛㒗㒙㒡㒙㒝㒜㒠㒘㒥㒗㒟㒘㒝㒘㒙㒗㒥㒙㒡㒗㒝㒗㒙㒚㒜㒦㒡㒙㒤㒦㒙㒘㒛㒥㒡㒦㒟㒥㒙㒤㒥㒘㒙㒤㒝㒠㒤㒣㒥㒣㒡㒣㒝㒤㒛㒢㒥㒢㒡㒥㒦㒢㒙㒥㒥㒡㒡㒡㒝㒡㒙㒢㒗㒠㒡㒠㒝㒣㒣㒟㒥㒜㒜㒟㒝㒟㒙㒞㒥㒟㒣㒞㒝㒞㒙㒡㒠㒝㒡㒗㒚㒝㒙㒜㒥㒜㒡㒜㒝㒜㒙㒛㒥㒟㒘㒛㒝㒞㒤㒚㒥㒚㒣㒚㒝㒛㒙㒙㒥㒙㒡㒙㒥㒙㒙㒝㒘㒘㒡㒛㒤㒘㒙㒙㒗㒗㒡㒗㒝㒚㒠㒦㒥㒞㒠㒦㒝㒦㒙㒥㒥㒗㒡㒥㒝㒥㒙㒘㒜㒤㒡㒗㒤㒤㒙㒜㒝㒣㒡㒥㒝㒣㒙㒢㒥㒦㒘㒢㒝㒥㒠㒡㒥㒥㒝㒡㒝㒢㒙㒠㒥㒠㒡㒠㒥㒠㒙㒘㒝㒟㒡㒢㒤㒟㒙㒡㒥㒞㒡㒞㒝㒞㒡㒝㒥㒞㒥㒝㒝㒝㒠㒜㒦㒝㒣㒜㒝㒜㒙㒟㒜㒛㒡㒞㒞㒛㒙㒚㒥㒚㒡㒜㒝㒚㒙㒙㒥㒝㒘㒙㒝㒜㒠㒘㒥㒘㒡㒘㒞㒙㒛㒗㒥㒗㒡㒚㒥㒗㒙㒥㒚㒦㒡㒦㒝㒦㒙㒗㒗㒥㒡㒥㒝㒘㒢㒤㒥㒗㒠㒤㒝㒤㒙㒣㒥㒤㒣㒣㒝㒣㒙㒦㒟㒢㒡㒢㒥㒢㒙㒡㒥㒡㒡㒡㒝㒡㒙㒠㒥㒤㒘㒠㒝㒣㒣㒟㒥㒟㒣㒟㒝㒠㒙㒞㒥㒞㒡㒞㒥㒞㒙㒗㒡㒝㒡㒠㒤㒝㒙㒟㒥㒜㒡㒜㒝㒜㒡㒛㒥㒡㒞㒛㒝㒜㒣㒚㒥㒝㒡㒚㒝㒚㒙㒚㒝㒙㒡㒚㒙㒙㒙㒙㒞㒘㒢㒛㒝㒘㒙㒗㒥㒘㒙㒗㒝㒢㒟㒦㒥㒘㒛㒦㒝㒙㒙㒥㒥㒥㒡㒥㒦㒥㒙㒜㒙㒤㒡㒤㒦㒤㒙㒤㒥㒣㒡㒣㒝㒣㒢㒢㒥㒗㒣㒢㒝㒢㒞㒡㒥㒢㒣㒡㒝㒡㒙㒤㒜㒠㒡㒣㒞㒠㒙㒟㒥㒟㒡㒡㒝㒟㒙㒞㒥㒢㒘㒞㒝㒡㒠㒝㒥㒝㒡㒝㒞㒞㒛㒜㒥㒜㒡㒟㒥㒜㒙㒝㒝㒛㒡㒛㒝㒛㒙㒜㒗㒚㒡㒚㒝㒝㒢㒙㒥㒛㒙㒙㒝㒙㒙㒘㒥㒙㒣㒘㒝㒘㒙㒛㒟㒗㒡㒘㒥㒗㒙㒦㒥㒦㒡㒦㒝㒦㒙㒥㒥㒙㒘㒥㒝㒘㒣㒤㒥㒤㒣㒤㒝㒥㒙㒣㒥㒣㒡㒣㒦㒣㒙㒠㒙㒢㒡㒥㒤㒢㒙㒤㒥㒢㒣㒡㒝㒡㒢㒠㒥㒢㒟㒠㒝㒦㒗㒟㒥㒠㒣㒟㒝㒟㒙㒢㒜㒞㒡㒝㒛㒞㒙㒝㒥㒝㒡㒟㒝㒝㒙㒜㒥㒠㒘㒜㒝㒟㒠㒛㒥㒞㒗㒛㒝㒜㒛㒚㒥㒚㒡㒝㒥㒚㒙㒡㒥㒙㒡㒙㒝㒙㒙㒚㒗㒘㒡㒘㒝㒛㒢㒗㒥㒤㒜㒗㒝㒗㒙㒦㒥㒗㒣㒦㒝㒦㒙㒙㒟㒥㒡㒦㒘㒥㒙㒤㒥㒤㒡㒥㒟㒤㒙㒣㒥㒗㒜㒣㒝㒟㒤㒢㒥㒢㒡㒢㒝㒢㒙㒡㒥㒡㒡㒤㒤㒡㒙㒤㒠㒠㒡㒠㒟㒠㒙㒠㒥㒟㒡㒟㒝㒟㒢㒞㒥㒡㒟㒞㒝㒡㒠㒝㒥㒞㒣㒝㒝㒝㒙㒠㒜㒜㒡㒛㒛㒜㒙㒛㒥㒛㒡㒝㒝㒛㒙㒚㒥㒞㒘㒚㒝㒝㒠㒙㒥㒜㒗㒙㒝㒚㒛㒘㒥㒘㒡㒛㒥㒘㒙㒤㒠㒗㒡㒗㒝㒗㒙㒘㒗㒦㒡㒦㒝㒙㒢㒥㒥㒠㒚㒥㒝㒥㒙㒤㒥㒥㒣㒤㒝㒤㒙㒗㒟㒣㒡㒠㒘㒣㒙㒢㒥㒢㒡㒣㒟㒢㒙㒡㒥㒥㒜㒡㒝㒚㒦㒠㒥㒠㒡㒠㒝㒠㒙㒟㒥㒟㒡㒢㒤㒟㒙㒢㒠㒞㒡㒞㒟㒞㒙㒞㒥㒝㒡㒝㒝㒝㒢㒜㒥㒠㒤㒜㒝㒟㒠㒛㒥㒜㒣㒛㒝㒛㒙㒞㒜㒚㒡㒢㒜㒚㒙㒙㒥㒙㒡㒛㒝㒙㒙㒘㒥㒜㒘㒘㒝㒛㒠㒗㒥㒠㒙㒗㒝㒙㒙㒦㒥㒦㒡㒙㒤㒦㒙㒙㒜㒥㒡㒙㒙㒥㒙㒥㒥㒤㒡㒤㒝㒤㒢㒣㒥㒜㒙㒣㒝㒦㒠㒢㒥㒥㒡㒢㒝㒢㒙㒢㒞㒡㒡㒢㒡㒡㒙㒚㒘㒠㒡㒡㒟㒠㒙㒟㒥㒣㒘㒟㒝㒢㒚㒞㒥㒞㒡㒞㒝㒠㒙㒝㒥㒝㒡㒠㒤㒝㒙㒠㒜㒜㒡㒜㒝㒜㒚㒝㒗㒛㒡㒛㒝㒞㒡㒚㒥㒠㒠㒚㒝㒚㒙㒙㒥㒚㒣㒙㒝㒙㒙㒜㒞㒘㒡㒙㒡㒘㒚㒗㒥㒗㒡㒘㒟㒗㒙㒦㒥㒚㒛㒦㒝㒢㒤㒥㒥㒥㒡㒥㒝㒥㒙㒤㒥㒤㒡㒗㒤㒤㒙㒗㒟㒣㒡㒣㒟㒣㒙㒣㒥㒢㒡㒢㒝㒢㒢㒡㒥㒛㒝㒡㒝㒤㒠㒠㒥㒣㒡㒠㒝㒠㒙㒠㒞㒟㒡㒥㒚㒟㒙㒠㒟㒞㒡㒡㒝㒞㒙㒝㒥㒞㒚㒝㒝㒝㒥㒜㒥㒝㒚㒜㒞㒟㒙㒛㒥㒛㒡㒛㒦㒛㒙㒦㒛㒚㒡㒜㒗㒚㒙㒜㒥㒙㒡㒙㒝㒙㒣㒘㒥㒟㒥㒘㒝㒦㒘㒗㒥㒘㒡㒗㒝㒗㒙㒗㒟㒦㒡㒛㒟㒦㒙㒦㒚㒥㒡㒦㒟㒥㒙㒤㒥㒘㒘㒤㒝㒗㒚㒣㒥㒣㒡㒣㒝㒥㒙㒢㒥㒢㒡㒥㒤㒢㒙㒥㒜㒡㒡㒡㒝㒡㒚㒢㒗㒠㒡㒠㒝㒣㒡㒟㒥㒡㒙㒟㒝㒟㒙㒞㒥㒟㒣㒞㒝㒞㒙㒡㒞㒝㒡㒞㒥㒝㒙㒜㒥㒜㒡㒝㒟㒜㒙㒛㒥㒟㒛㒛㒝㒜㒡㒚㒥㒚㒡㒚㒝㒚㒙㒙㒥㒙㒡㒜㒤㒙㒙㒜㒟㒘㒡㒘㒟㒘㒙㒘㒥㒗㒡㒗㒝㒗㒣㒦㒥㒣㒥㒦㒝㒙㒠㒥㒥㒘㒡㒥㒝㒥㒙㒥㒟㒤㒡㒦㒛㒤㒙㒙㒣㒣㒡㒤㒟㒣㒙㒢㒥㒦㒘㒢㒝㒡㒗㒡㒥㒡㒡㒡㒝㒣㒙㒠㒥㒠㒡㒣㒤㒠㒙㒣㒜㒟㒡㒡㒣㒟㒙㒠㒗㒞㒡㒞㒝㒡㒡㒝㒥㒞㒣㒝㒝㒝㒙㒜㒥㒝㒣㒜㒝㒜㒙㒟㒞㒛㒡㒘㒘㒛㒙㒚㒥㒚㒡㒛㒟㒚㒙㒙㒥㒝㒛㒙㒝㒙㒤㒘㒥㒘㒡㒘㒝㒙㒛㒗㒥㒗㒡㒛㒘㒗㒙㒣㒠㒦㒡㒦㒝㒦㒙㒥㒥㒥㒡㒥㒝㒘㒠㒤㒥㒘㒜㒤㒝㒤㒛㒣㒥㒤㒡㒣㒝㒣㒙㒣㒟㒢㒡㒥㒛㒢㒙㒥㒜㒡㒡㒢㒟㒡㒙㒠㒥㒤㒘㒠㒝㒟㒗㒟㒥㒟㒡㒟㒝㒡㒙㒞㒥㒞㒡㒡㒤㒞㒙㒡㒜㒝㒡㒟㒣㒝㒙㒞㒗㒜㒡㒜㒝㒟㒡㒛㒥㒘㒜㒛㒝㒛㒙㒚㒥㒛㒣㒚㒝㒚㒙㒝㒞㒙㒡㒣㒦㒙㒙㒘㒥㒘㒡㒙㒟㒘㒙㒗㒥㒛㒛㒗㒝㒣㒤㒦㒥㒦㒡㒦㒝㒗㒛㒥㒥㒥㒡㒙㒘㒥㒙㒞㒢㒤㒡㒤㒝㒤㒙㒣㒥㒣㒡㒣㒝㒦㒠㒢㒥㒦㒜㒢㒝㒢㒛㒡㒥㒢㒡㒡㒝㒡㒙㒡㒟㒠㒡㒤㒠㒠㒙㒣㒜㒟㒡㒠㒟㒟㒙㒞㒥㒢㒘㒞㒝㒦㒘㒝㒥㒝㒡㒝㒝㒟㒙㒜㒥㒜㒡㒟㒤㒜㒙㒟㒜㒛㒡㒣㒥㒛㒙㒜㒥㒚㒡㒚㒝㒝㒠㒙㒥㒝㒘㒙㒝㒜㒥㒘㒥㒙㒡㒘㒝㒘㒙㒘㒟㒗㒡㒟㒥㒗㒙㒚㒜㒦㒡㒙㒝㒦㒙㒥㒥㒦㒛㒥㒝㒦㒝㒤㒥㒞㒛㒤㒝㒥㒛㒣㒥㒣㒡㒦㒤㒣㒙㒥㒦㒢㒡㒢㒝㒢㒙㒣㒥㒡㒡㒡㒝㒤㒠㒠㒥㒤㒘㒠㒝㒠㒙㒟㒦㒠㒣㒟㒝㒟㒙㒢㒝㒞㒡㒗㒘㒞㒙㒝㒥㒝㒡㒞㒟㒝㒙㒜㒥㒠㒚㒜㒝㒜㒦㒛㒦㒛㒡㒛㒝㒜㒛㒚㒥㒚㒡㒞㒗㒚㒙㒚㒢㒙㒢㒙㒝㒙㒙㒘㒥㒘㒡㒘㒝㒛㒠㒗㒥㒛㒛㒗㒝㒗㒛㒦㒥㒗㒡㒦㒝㒦㒙㒦㒟㒥㒡㒟㒙㒥㒙㒘㒜㒤㒡㒗㒝㒤㒙㒣㒥㒤㒛㒣㒝㒘㒦㒢㒥㒤㒛㒢㒝㒥㒙㒡㒥㒡㒡㒢㒗㒡㒙㒡㒡㒠㒡㒠㒦㒠㒚㒢㒥㒟㒡㒟㒝㒟㒣㒞㒥㒚㒗㒞㒝㒟㒣㒝㒥㒠㒡㒝㒝㒝㒙㒝㒠㒜㒡㒣㒡㒜㒙㒘㒥㒛㒡㒜㒝㒛㒙㒚㒥㒛㒜㒚㒝㒟㒛㒙㒥㒙㒦㒙㒝㒚㒛㒘㒥㒘㒡㒛㒤㒘㒙㒚㒦㒗㒡㒗㒝㒗㒙㒘㒥㒦㒡㒦㒝㒙㒠㒥㒥㒙㒘㒥㒝㒥㒙㒤㒦㒥㒣㒤㒝㒤㒙㒗㒝㒣㒡㒤㒥㒣㒙㒢㒥㒢㒡㒣㒟㒢㒙㒡㒥㒥㒚㒡㒝㒢㒡㒠㒥㒠㒡㒠㒝㒡㒛㒟㒥㒟㒡㒣㒗㒟㒙㒠㒝㒞㒡㒞㒝㒞㒙㒝㒥㒤㒤㒝㒝㒠㒠㒜㒥㒠㒛㒜㒝㒜㒛㒛㒥㒜㒡㒤㒛㒛㒙㒛㒠㒚㒡㒗㒡㒚㒙㒝㒜㒙㒡㒜㒝㒙㒙㒘㒥㒙㒜㒘㒝㒚㒗㒗㒥㒝㒟㒗㒝㒘㒛㒦㒥㒦㒡㒙㒤㒦㒙㒤㒣㒥㒡㒥㒝㒥㒙㒦㒥㒤㒡㒤㒝㒗㒠㒣㒥㒗㒘㒣㒝㒥㒟㒢㒥㒣㒣㒢㒝㒢㒙㒥㒝㒡㒡㒜㒞㒡㒙㒠㒥㒠㒡㒡㒟㒠㒙㒟㒥㒣㒚㒟㒝㒛㒤㒞㒥㒞㒡㒞㒝㒟㒛㒝㒥㒝㒡㒡㒗㒝㒙㒝㒠㒜㒡㒜㒝㒜㒙㒝㒗㒛㒡㒛㒝㒞㒤㒚㒥㒗㒜㒚㒝㒚㒙㒙㒥㒙㒡㒙㒝㒙㒙㒜㒜㒘㒡㒜㒘㒘㒙㒘㒗㒗㒡㒘㒝㒗㒙㒦㒥㒗㒜㒦㒝㒙㒗㒥㒥㒙㒘㒥㒝㒦㒛㒤㒥㒤㒡㒗㒤㒤㒙㒢㒣㒣㒡㒣㒝㒣㒙㒤㒥㒢㒡㒢㒝㒥㒠㒡㒥㒥㒘㒡㒝㒣㒟㒠㒥㒡㒣㒠㒝㒠㒙㒣㒝㒟㒡㒜㒘㒟㒙㒞㒥㒞㒡㒟㒟㒞㒙㒝㒥㒡㒚㒝㒝㒡㒙㒜㒥㒜㒡㒜㒝㒝㒛㒛㒥㒛㒡㒟㒗㒛㒙㒗㒠㒚㒡㒚㒝㒚㒙㒛㒗㒙㒡㒙㒝㒜㒤㒘㒥㒢㒞㒘㒝㒘㒙㒗㒥㒗㒡㒗㒝㒗㒙㒚㒜㒦㒡㒚㒘㒦㒙㒦㒗㒥㒡㒦㒝㒥㒙㒤㒥㒥㒜㒤㒝㒘㒜㒣㒥㒗㒘㒣㒝㒤㒛㒢㒥㒢㒡㒥㒤㒢㒙㒙㒤㒡㒡㒡㒝㒡㒙㒢㒥㒠㒡㒠㒝㒣㒠㒟㒥㒣㒘㒟㒝㒗㒡㒞㒥㒠㒡㒞㒝㒞㒙㒡㒜㒝㒡㒠㒤㒝㒙㒠㒡㒜㒡㒝㒝㒜㒙㒛㒥㒜㒜㒛㒝㒣㒡㒚㒥㒞㒘㒚㒝㒝㒙㒙㒥㒙㒡㒚㒘㒙㒙㒚㒙㒘㒡㒤㒙㒘㒙㒙㒗㒗㒡㒗㒝㒚㒠㒦㒥㒙㒢㒦㒝㒦㒙㒥㒥㒗㒡㒥㒝㒥㒙㒘㒜㒤㒡㒗㒤㒤㒙㒣㒥㒣㒢㒤㒟㒣㒙㒢㒥㒦㒙㒢㒝㒙㒢㒡㒥㒡㒡㒡㒝㒢㒛㒠㒥㒠㒡㒣㒦㒠㒙㒠㒝㒟㒡㒟㒝㒟㒙㒠㒗㒞㒡㒞㒝㒡㒣㒝㒥㒢㒦㒝㒝㒝㒙㒜㒥㒜㒡㒜㒝㒜㒙㒟㒜㒛㒡㒟㒗㒛㒙㒛㒗㒚㒡㒛㒝㒚㒙㒙㒥㒚㒜㒙㒝㒢㒥㒘㒥㒜㒘㒘㒝㒛㒙㒗㒥㒗㒡㒘㒘㒗㒙㒜㒢㒦㒡㒘㒗㒦㒙㒘㒥㒥㒡㒥㒝㒥㒤㒤㒥㒥㒝㒤㒝㒤㒢㒣㒦㒦㒡㒣㒝㒣㒙㒣㒠㒢㒡㒝㒣㒢㒙㒣㒟㒡㒡㒤㒝㒡㒙㒠㒥㒡㒝㒠㒝㒗㒝㒟㒥㒣㒜㒟㒝㒠㒙㒞㒥㒞㒡㒟㒙㒞㒙㒣㒗㒝㒡㒝㒢㒝㒙㒞㒗㒜㒡㒜㒝㒟㒠㒛㒥㒞㒢㒛㒝㒛㒙㒚㒥㒜㒡㒚㒝㒚㒙㒝㒜㒙㒡㒜㒤㒙㒙㒘㒥㒘㒢㒙㒟㒘㒙㒗㒥㒛㒙㒗㒝㒘㒡㒦㒥㒦㒡㒦㒝㒗㒛㒥㒥㒥㒡㒘㒦㒥㒙㒦㒝㒤㒡㒤㒝㒤㒙㒥㒗㒣㒡㒣㒝㒦㒣㒢㒥㒤㒙㒢㒝㒢㒙㒡㒥㒡㒡㒡㒝㒡㒙㒤㒜㒠㒡㒤㒗㒠㒙㒠㒗㒟㒡㒠㒝㒟㒙㒞㒥㒟㒝㒞㒝㒛㒝㒝㒥㒡㒘㒝㒝㒠㒙㒜㒥㒜㒡㒝㒙㒜㒙㒝㒣㒛㒡㒡㒛㒛㒙㒜㒗㒚㒡㒚㒝㒝㒠㒙㒥㒘㒟㒙㒝㒙㒙㒘㒥㒚㒡㒘㒝㒘㒙㒛㒜㒗㒡㒚㒤㒗㒙㒙㒛㒦㒡㒗㒟㒦㒙㒥㒥㒙㒙㒥㒝㒢㒢㒤㒥㒤㒡㒤㒝㒥㒛㒣㒥㒣㒡㒦㒦㒣㒙㒟㒠㒢㒡㒢㒝㒢㒙㒣㒗㒡㒡㒡㒝㒤㒣㒠㒥㒡㒜㒠㒝㒠㒙㒟㒥㒠㒣㒟㒝㒟㒙㒢㒠㒞㒡㒛㒘㒞㒙㒝㒥㒝㒡㒝㒝㒝㒙㒜㒥㒠㒘㒜㒝㒟㒤㒛㒥㒛㒣㒛㒝㒜㒙㒚㒥㒚㒡㒛㒙㒚㒙㒜㒣㒙㒡㒜㒤㒙㒙㒚㒗㒘㒡㒘㒝㒛㒠㒗㒥㒦㒟㒗㒝㒗㒙㒦㒥㒘㒡㒦㒝㒦㒙㒙㒜㒥㒡㒘㒤㒥㒙㒗㒛㒤㒡㒥㒟㒤㒙㒣㒥㒗㒙㒣㒝㒟㒤㒢㒥㒢㒡㒢㒝㒣㒛㒡㒥㒡㒡㒤㒦㒡㒙㒤㒦㒠㒡㒠㒝㒠㒙㒡㒗㒟㒡㒟㒝㒢㒣㒞㒥㒛㒜㒞㒝㒞㒙㒝㒥㒞㒣㒝㒝㒝㒙㒠㒠㒜㒡㒦㒚㒜㒙㒛㒥㒛㒡㒛㒝㒛㒙㒚㒥㒞㒘㒚㒝㒝㒤㒙㒥㒙㒣㒙㒝㒚㒙㒘㒥㒘㒡㒙㒙㒘㒙㒜㒘㒗㒡㒚㒤㒗㒙㒘㒗㒦㒡㒦㒝㒙㒠㒥㒥㒝㒠㒥㒝㒥㒙㒤㒥㒦㒡㒤㒝㒤㒙㒗㒜㒣㒡㒦㒤㒣㒙㒛㒝㒢㒡㒤㒝㒢㒙㒡㒥㒥㒘㒡㒝㒤㒠㒠㒥㒤㒝㒠㒝㒡㒙㒟㒥㒟㒡㒠㒙㒟㒙㒗㒝㒞㒡㒡㒤㒞㒙㒠㒥㒝㒡㒝㒝㒝㒥㒜㒥㒝㒥㒜㒝㒜㒠㒛㒦㒜㒣㒛㒝㒛㒙㒞㒜㒚㒡㒝㒞㒚㒙㒙㒥㒙㒡㒛㒝㒙㒙㒘㒥㒜㒘㒘㒝㒛㒠㒗㒥㒗㒡㒗㒞㒘㒛㒦㒥㒦㒡㒙㒥㒦㒙㒘㒥㒥㒡㒥㒝㒥㒙㒦㒗㒤㒡㒤㒝㒗㒢㒣㒥㒤㒙㒣㒝㒣㒙㒢㒥㒣㒣㒢㒝㒢㒙㒥㒟㒡㒡㒠㒗㒡㒙㒠㒥㒠㒡㒠㒝㒠㒙㒟㒥㒣㒘㒟㒝㒢㒣㒞㒥㒞㒣㒞㒝㒟㒙㒝㒥㒝㒡㒞㒙㒝㒙㒦㒡㒜㒡㒟㒤㒜㒙㒞㒥㒛㒡㒛㒝㒛㒥㒚㒥㒠㒞㒚㒝㒛㒣㒙㒥㒜㒡㒙㒝㒙㒙㒙㒡㒘㒡㒙㒙㒘㒙㒘㒞㒗㒢㒚㒝㒗㒙㒦㒥㒗㒝㒦㒝㒡㒟㒥㒥㒗㒛㒥㒝㒘㒙㒤㒥㒤㒡㒥㒚㒤㒙㒛㒙㒣㒡㒟㒗㒣㒙㒣㒥㒢㒡㒢㒝㒢㒦㒡㒥㒦㒣㒡㒝㒡㒞㒠㒥㒡㒣㒠㒝㒠㒙㒣㒜㒟㒡㒢㒞㒟㒙㒞㒥㒞㒡㒠㒝㒞㒙㒝㒥㒡㒘㒝㒝㒠㒠㒜㒥㒜㒡㒜㒞㒝㒛㒛㒥㒛㒡㒞㒥㒛㒙㒜㒝㒚㒡㒚㒝㒚㒙㒛㒗㒙㒡㒙㒝㒜㒢㒘㒥㒚㒙㒘㒝㒘㒙㒗㒥㒘㒣㒙㒝㒗㒙㒚㒟㒦㒡㒗㒥㒦㒙㒥㒥㒥㒡㒥㒝㒜㒜㒤㒥㒘㒘㒤㒝㒗㒣㒣㒥㒣㒣㒣㒝㒤㒙㒛㒣㒢㒡㒣㒚㒢㒙㒟㒙㒡㒡㒤㒤㒡㒙㒣㒥㒠㒡㒠㒝㒠㒦㒟㒥㒡㒟㒟㒝㒥㒗㒞㒥㒟㒣㒞㒝㒞㒙㒡㒜㒝㒡㒜㒛㒝㒙㒜㒥㒜㒡㒞㒝㒜㒙㒛㒥㒟㒘㒛㒝㒞㒠㒚㒥㒝㒗㒚㒝㒛㒛㒙㒥㒙㒡㒜㒥㒙㒙㒥㒙㒘㒡㒘㒝㒘㒙㒙㒗㒗㒡㒗㒝㒚㒢㒦㒥㒣㒜㒦㒝㒦㒙㒥㒥㒦㒣㒥㒝㒥㒙㒘㒟㒤㒡㒥㒘㒤㒙㒣㒥㒣㒡㒤㒟㒣㒙㒢㒥㒦㒜㒢㒝㒞㒤㒡㒥㒡㒡㒡㒝㒡㒙㒠㒥㒠㒡㒣㒤㒠㒙㒣㒠㒟㒡㒟㒟㒟㒙㒟㒥㒞㒡㒞㒝㒞㒦㒝㒥㒠㒟㒝㒝㒠㒠㒜㒥㒝㒣㒜㒝㒜㒙㒟㒜㒛㒡㒚㒛㒛㒙㒚㒥㒚㒡㒜㒝㒚㒙㒙㒥㒝㒘㒙㒝㒜㒠㒘㒥㒛㒗㒘㒝㒙㒛㒗㒥㒗㒡㒚㒥㒗㒙㒣㒠㒦㒡㒦㒝㒦㒙㒗㒗㒥㒡㒥㒝㒘㒢㒤㒥㒟㒚㒤㒝㒤㒙㒣㒥㒤㒣㒣㒝㒣㒙㒦㒟㒢㒡㒟㒘㒢㒙㒡㒥㒡㒡㒢㒟㒡㒙㒠㒥㒤㒜㒠㒝㒙㒦㒟㒥㒟㒡㒟㒝㒟㒙㒞㒥㒞㒡㒡㒤㒞㒙㒡㒠㒝㒡㒝㒟㒝㒙㒝㒥㒜㒡㒜㒝㒜㒦㒛㒥㒟㒤㒛㒝㒞㒠㒚㒥㒛㒣㒚㒝㒚㒙㒝㒜㒙㒡㒡㒜㒙㒙㒘㒥㒘㒡㒚㒝㒘㒙㒗㒥㒛㒘㒗㒝㒚㒠㒦㒥㒟㒙㒦㒝㒘㒙㒥㒥㒥㒡㒘㒤㒥㒙㒘㒜㒤㒡㒘㒙㒤㒙㒤㒥㒣㒡㒣㒝㒣㒦㒢㒥㒛㒙㒢㒝㒥㒠㒡㒥㒤㒡㒡㒝㒡㒙㒡㒢㒠㒡㒡㒡㒠㒙㒛㒟㒟㒡㒠㒟㒟㒙㒞㒥㒢㒘㒞㒝㒡㒚㒝㒥㒝㒡㒝㒝㒟㒙㒜㒥㒜㒡㒟㒤㒜㒙㒟㒜㒛㒡㒛㒝㒛㒚㒜㒗㒚㒡㒚㒝㒝㒡㒙㒥㒢㒜㒙㒝㒙㒙㒘㒥㒙㒣㒘㒝㒘㒙㒛㒞㒗㒡㒘㒚㒗㒚㒦㒥㒦㒡㒗㒟㒦㒙㒥㒥㒙㒛㒥㒝㒥㒦㒤㒦㒤㒡㒤㒝㒤㒙㒣㒥㒣㒡㒦㒤㒣㒙㒦㒟㒢㒡㒢㒟㒢㒙㒢㒥㒡㒡㒡㒝㒡㒦㒠㒥㒚㒝㒠㒝㒣㒠㒟㒥㒢㒡㒟㒝㒟㒙㒟㒢㒞㒡㒤㒚㒞㒙㒟㒟㒝㒡㒠㒝㒝㒙㒜㒥㒝㒞㒜㒝㒜㒥㒛㒥㒜㒚㒛㒞㒞㒙㒚㒥㒚㒡㒛㒚㒚㒙㒥㒛㒙㒡㒛㒗㒙㒙㒛㒥㒘㒡㒘㒝㒙㒗㒗㒥㒞㒥㒗㒝㒚㒤㒦㒥㒗㒡㒦㒝㒦㒙㒦㒣㒥㒡㒚㒟㒥㒙㒥㒚㒤㒡㒥㒟㒤㒙㒣㒥㒗㒘㒣㒝㒦㒚㒢㒥㒢㒡㒢㒝㒤㒙㒡㒥㒡㒡㒤㒤㒡㒙㒤㒜㒠㒡㒠㒝㒠㒚㒡㒗㒟㒡㒟㒝㒢㒡㒞㒥㒠㒙㒞㒝㒞㒙㒝㒥㒞㒣㒝㒝㒝㒙㒠㒞㒜㒡㒝㒥㒜㒙㒛㒥㒛㒡㒜㒟㒛㒙㒚㒥㒞㒛㒚㒝㒛㒡㒙㒥㒙㒡㒙㒝㒙㒙㒘㒥㒘㒡㒛㒤㒘㒙㒛㒟㒗㒡㒗㒟㒗㒙㒗㒥㒦㒡㒦㒝㒗㒗㒥㒥㒢㒥㒥㒝㒘㒠㒤㒥㒗㒡㒤㒝㒤㒙㒤㒣㒣㒡㒥㒛㒣㒙㒘㒣㒢㒡㒣㒟㒢㒙㒡㒥㒥㒘㒡㒝㒠㒗㒠㒥㒠㒡㒠㒝㒢㒙㒟㒥㒟㒡㒢㒤㒟㒙㒢㒜㒞㒡㒠㒣㒞㒙㒟㒗㒝㒡㒝㒝㒠㒡㒜㒥㒚㒙㒜㒝㒜㒙㒛㒥㒜㒣㒛㒝㒛㒙㒞㒞㒚㒡㒗㒘㒚㒙㒙㒥㒙㒡㒚㒟㒙㒙㒘㒥㒜㒛㒘㒝㒘㒤㒗㒥㒗㒡㒗㒝㒘㒛㒦㒥㒦㒡㒚㒘㒦㒙㒢㒠㒥㒡㒥㒝㒥㒙㒤㒥㒤㒡㒤㒝㒗㒠㒣㒥㒗㒜㒣㒝㒣㒛㒢㒥㒣㒡㒢㒝㒢㒙㒢㒣㒡㒡㒤㒛㒡㒙㒤㒜㒠㒡㒡㒟㒠㒙㒟㒥㒣㒘㒟㒝㒞㒗㒞㒥㒞㒡㒞㒝㒠㒙㒝㒥㒝㒡㒠㒤㒝㒙㒠㒜㒜㒡㒞㒣㒜㒙㒝㒗㒛㒡㒛㒝㒞㒡㒚㒥㒗㒜㒚㒝㒚㒙㒙㒥㒚㒣㒙㒝㒙㒙㒜㒞㒘㒡㒜㒝㒘㒙㒗㒥㒗㒡㒘㒟㒗㒙㒦㒥㒚㒛㒦㒝㒢㒤㒥㒥㒥㒡㒥㒝㒦㒛㒤㒥㒤㒡㒘㒘㒤㒙㒝㒢㒣㒡㒣㒝㒣㒙㒢㒥㒢㒡㒢㒝㒥㒠㒡㒥㒥㒜㒡㒝㒡㒛㒠㒥㒡㒡㒠㒝㒠㒙㒠㒣㒟㒡㒣㒠㒟㒙㒢㒜㒞㒡㒟㒟㒞㒙㒝㒥㒡㒘㒝㒝㒥㒘㒜㒥㒜㒡㒜㒝㒞㒙㒛㒥㒛㒡㒞㒤㒛㒙㒞㒜㒚㒡㒢㒥㒚㒙㒛㒥㒙㒡㒙㒝㒜㒠㒘㒥㒜㒘㒘㒝㒛㒥㒗㒥㒘㒡㒗㒝㒗㒙㒗㒣㒦㒡㒞㒥㒦㒙㒙㒜㒥㒡㒘㒝㒥㒙㒤㒥㒥㒟㒤㒝㒥㒝㒣㒥㒤㒘㒣㒞㒤㒛㒢㒥㒢㒡㒥㒤㒢㒙㒤㒦㒡㒡㒡㒝㒡㒙㒢㒥㒠㒡㒠㒝㒣㒠㒟㒥㒣㒘㒟㒝㒟㒙㒞㒦㒟㒣㒞㒝㒞㒙㒡㒝㒝㒡㒛㒢㒝㒙㒜㒥㒜㒡㒝㒟㒜㒙㒛㒥㒟㒚㒛㒝㒞㒘㒚㒥㒚㒡㒚㒝㒛㒛㒙㒥㒙㒡㒝㒗㒙㒙㒙㒝㒘㒡㒘㒝㒘㒙㒗㒥㒗㒡㒗㒝㒚㒠㒦㒥㒚㒛㒦㒝㒦㒛㒥㒥㒦㒡㒥㒝㒥㒙㒥㒣㒤㒡㒞㒙㒤㒙㒗㒜㒣㒡㒦㒝㒣㒙㒢㒥㒣㒟㒢㒝㒗㒦㒡㒥㒣㒛㒡㒝㒤㒙㒠㒥㒠㒡㒡㒛㒠㒙㒠㒡㒟㒡㒟㒦㒟㒚㒡㒥㒞㒡㒞㒝㒟㒗㒝㒥㒙㒗㒝㒝㒞㒣㒜㒥㒟㒡㒜㒝㒜㒙㒜㒤㒛㒡㒢㒡㒛㒙㒜㒥㒚㒡㒛㒝㒚㒙㒙㒥㒚㒠㒙㒝㒞㒛㒘㒥㒘㒦㒘㒝㒙㒛㒗㒥㒗㒡㒚㒤㒗㒙㒙㒦㒦㒡㒦㒝㒦㒙㒗㒥㒥㒡㒥㒝㒘㒠㒤㒥㒘㒘㒤㒝㒤㒙㒣㒦㒤㒣㒣㒝㒣㒙㒦㒝㒢㒡㒣㒥㒢㒙㒡㒥㒡㒡㒢㒟㒡㒙㒠㒥㒤㒚㒠㒝㒡㒡㒟㒥㒟㒡㒟㒝㒠㒛㒠㒥㒞㒡㒢㒗㒞㒙㒟㒝㒝㒡㒝㒝㒝㒙㒜㒥㒡㒚㒜㒝㒟㒠㒛㒥㒟㒛㒛㒝㒛㒛㒚㒥㒛㒡㒚㒝㒚㒙㒚㒤㒙㒡㒦㒡㒙㒙㒜㒜㒘㒡㒛㒝㒘㒙㒗㒥㒘㒠㒗㒝㒙㒗㒦㒥㒜㒟㒦㒝㒗㒛㒥㒥㒥㒡㒘㒤㒥㒙㒣㒣㒤㒡㒤㒝㒤㒙㒥㒥㒣㒡㒣㒝㒦㒠㒢㒥㒦㒘㒢㒝㒤㒟㒡㒥㒢㒣㒡㒝㒡㒙㒤㒝㒠㒡㒢㒜㒠㒙㒟㒥㒟㒡㒠㒟㒟㒙㒞㒥㒢㒚㒞㒝㒚㒤㒝㒥㒝㒡㒝㒝㒞㒛㒜㒥㒜㒡㒠㒗㒜㒙㒜㒠㒛㒡㒛㒝㒛㒙㒜㒗㒚㒡㒚㒝㒝㒤㒙㒥㒦㒜㒙㒝㒙㒙㒘㒥㒘㒡㒘㒝㒘㒙㒛㒜㒗㒡㒛㒘㒗㒙㒗㒗㒦㒡㒗㒝㒦㒙㒥㒥㒦㒠㒥㒝㒘㒗㒤㒥㒘㒘㒤㒝㒥㒛㒣㒥㒣㒡㒦㒤㒣㒙㒡㒣㒢㒡㒢㒝㒢㒙㒣㒥㒡㒡㒡㒝㒤㒠㒠㒥㒤㒘㒠㒝㒢㒟㒟㒥㒠㒣㒟㒝㒟㒙㒢㒝㒞㒡㒛㒘㒞㒙㒝㒥㒝㒡㒞㒟㒝㒙㒜㒥㒠㒚㒜㒝㒥㒦㒛㒥㒛㒡㒛㒝㒜㒛㒚㒥㒚㒡㒞㒗㒚㒙㒦㒠㒙㒡㒙㒝㒙㒙㒚㒗㒘㒡㒘㒝㒛㒤㒗㒥㒡㒞㒗㒝㒗㒙㒦㒥㒦㒡㒦㒝㒦㒙㒙㒜㒥㒡㒙㒘㒥㒙㒥㒗㒤㒡㒥㒝㒤㒙㒣㒥㒤㒠㒣㒝㒗㒜㒢㒥㒦㒘㒢㒝㒣㒛㒡㒥㒡㒡㒤㒤㒡㒙㒘㒤㒠㒡㒠㒝㒠㒙㒡㒥㒟㒡㒟㒝㒢㒠㒞㒥㒢㒘㒞㒝㒦㒡㒝㒥㒟㒡㒝㒝㒝㒙㒠㒜㒜㒡㒟㒤㒜㒙㒟㒡㒛㒡㒜㒝㒛㒙㒚㒥㒛㒠㒚㒝㒢㒡㒙㒥㒝㒘㒙㒝㒜㒙㒘㒥㒘㒡㒙㒜㒘㒙㒙㒙㒗㒡㒦㒞㒗㒙㒘㒗㒦㒡㒦㒝㒙㒠㒥㒥㒘㒢㒥㒝㒥㒙㒤㒥㒦㒡㒤㒝㒤㒙㒗㒜㒣㒡㒦㒤㒣㒙㒢㒥㒢㒢㒣㒟㒢㒙㒡㒥㒥㒙㒡㒝㒗㒘㒠㒥㒠㒡㒠㒝㒡㒛㒟㒥㒟㒡㒢㒦㒟㒙㒠㒙㒞㒢㒞㒝㒞㒙㒟㒗㒝㒡㒝㒝㒠㒣㒜㒥㒙㒜㒜㒝㒜㒙㒛㒥㒛㒡㒛㒝㒛㒙㒞㒜㒚㒡㒞㒗㒚㒙㒚㒗㒙㒡㒚㒝㒙㒙㒘㒥㒙㒠㒘㒝㒡㒥㒗㒥㒛㒘㒗㒝㒚㒙㒦㒥㒦㒡㒗㒜㒦㒙㒛㒢㒥㒡㒗㒗㒥㒙㒗㒥㒤㒡㒤㒝㒥㒘㒣㒥㒤㒝㒣㒝㒣㒢㒢㒦㒥㒡㒢㒝㒢㒙㒢㒤㒡㒡㒜㒣㒡㒙㒢㒟㒠㒡㒣㒝㒠㒙㒟㒥㒠㒡㒟㒝㒦㒝㒞㒥㒞㒝㒞㒝㒟㒙㒝㒥㒝㒡㒞㒝㒝㒙㒢㒗㒜㒡㒜㒢㒜㒙㒝㒗㒛㒡㒛㒝㒞㒠㒚㒥㒝㒢㒚㒝㒚㒙㒙㒥㒛㒡㒙㒝㒙㒙㒜㒜㒘㒡㒛㒤㒘㒙㒗㒥㒗㒢㒘㒟㒗㒙㒦㒥㒚㒙㒦㒝㒗㒡㒥㒥㒥㒡㒥㒝㒦㒛㒤㒥㒤㒡㒗㒦㒤㒙㒥㒝㒣㒡㒣㒝㒣㒙㒤㒗㒢㒡㒢㒝㒥㒣㒡㒥㒣㒙㒡㒝㒡㒙㒠㒥㒠㒡㒠㒝㒠㒙㒣㒜㒟㒡㒣㒗㒟㒙㒟㒗㒞㒡㒟㒝㒞㒙㒝㒥㒞㒡㒝㒝㒚㒝㒜㒥㒠㒘㒜㒝㒟㒙㒛㒥㒛㒡㒜㒝㒛㒙㒜㒣㒚㒡㒠㒛㒚㒙㒛㒗㒙㒡㒙㒝㒜㒠㒘㒥㒗㒟㒘㒝㒘㒙㒗㒥㒙㒡㒗㒝㒗㒙㒚㒜㒦㒡㒙㒤㒦㒙㒘㒛㒥㒡㒦㒟㒥㒙㒤㒥㒘㒙㒤㒝㒚㒡㒣㒥㒣㒡㒣㒝㒤㒛㒢㒥㒢㒡㒥㒦㒢㒙㒞㒠㒡㒡㒡㒝㒡㒙㒢㒗㒠㒡㒠㒝㒣㒣㒟㒥㒠㒜㒟㒝㒟㒙㒞㒥㒟㒣㒞㒝㒞㒙㒡㒠㒝㒡㒚㒘㒝㒙㒜㒥㒜㒡㒜㒝㒜㒙㒛㒥㒟㒘㒛㒝㒞㒤㒚㒥㒚㒣㒚㒝㒛㒙㒙㒥㒙㒡㒚㒝㒙㒙㒛㒣㒘㒡㒛㒤㒘㒙㒙㒗㒗㒡㒗㒝㒚㒠㒦㒥㒥㒟㒦㒝㒦㒙㒥㒥㒗㒡㒥㒝㒥㒙㒘㒜㒤㒡㒗㒤㒤㒙㒦㒛㒣㒡㒤㒟㒣㒙㒢㒥㒦㒙㒢㒝㒞㒤㒡㒥㒡㒡㒡㒝㒢㒛㒠㒥㒠㒡㒣㒦㒠㒙㒝㒟㒟㒡㒟㒝㒟㒙㒠㒗㒞㒡㒞㒝㒡㒣㒝㒥㒚㒜㒝㒝㒝㒙㒜㒥㒝㒣㒜㒝㒜㒙㒟㒠㒛㒡㒥㒚㒛㒙㒚㒥㒚㒡㒚㒝㒚㒙㒙㒥㒝㒘㒙㒝㒜㒤㒘㒥㒘㒣㒘㒝㒙㒙㒗㒥㒗㒡㒘㒝㒗㒙㒛㒘㒦㒡㒙㒤㒦㒙㒗㒗㒥㒡㒥㒝㒘㒠㒤㒥㒜㒠㒤㒝㒤㒙㒣㒥㒥㒡㒣㒝㒣㒙㒦㒜㒢㒡㒥㒤㒢㒙㒚㒝㒡㒡㒣㒝㒡㒙㒠㒥㒤㒘㒠㒝㒣㒠㒟㒥㒣㒝㒟㒝㒠㒙㒞㒥㒞㒡㒟㒝㒞㒙㒦㒝㒝㒡㒠㒤㒝㒙㒟㒥㒜㒡㒜㒝㒝㒙㒛㒥㒜㒥㒛㒝㒛㒟㒚㒦㒛㒣㒚㒝㒚㒙㒝㒜㒙㒡㒜㒞㒙㒙㒘㒥㒘㒡㒚㒝㒘㒙㒗㒥㒛㒘㒗㒝㒚㒠㒦㒥㒦㒡㒦㒞㒗㒛㒥㒥㒥㒡㒘㒥㒥㒙㒝㒠㒤㒡㒤㒝㒤㒙㒥㒗㒣㒡㒣㒝㒦㒢㒢㒥㒣㒞㒢㒞㒢㒙㒡㒥㒢㒣㒡㒝㒡㒙㒤㒟㒠㒡㒡㒚㒠㒚㒟㒥㒟㒡㒟㒝㒟㒙㒞㒥㒢㒘㒞㒝㒡㒣㒝㒥㒝㒣㒝㒝㒞㒙㒜㒥㒜㒡㒝㒝㒜㒙㒥㒡㒛㒡㒞㒤㒛㒙㒝㒥㒚㒡㒚㒝㒛㒙㒙㒥㒟㒞㒙㒝㒚㒣㒘㒥㒛㒡㒘㒝㒘㒙㒘㒥㒗㒡㒘㒙㒗㒙㒗㒞㒦㒢㒙㒝㒦㒙㒥㒥㒦㒡㒥㒝㒠㒟㒤㒥㒦㒛㒤㒝㒥㒙㒣㒥㒣㒡㒤㒞㒣㒙㒘㒗㒢㒡㒢㒢㒢㒙㒣㒗㒡㒡㒡㒝㒤㒠㒠㒥㒣㒢㒠㒝㒠㒙㒟㒥㒡㒡㒟㒝㒟㒙㒢㒜㒞㒡㒡㒤㒞㒙㒝㒥㒝㒢㒞㒟㒝㒙㒜㒥㒠㒙㒜㒝㒝㒡㒛㒥㒛㒡㒛㒝㒜㒛㒚㒥㒚㒡㒝㒦㒚㒙㒛㒝㒙㒡㒙㒝㒙㒙㒚㒗㒚㒡㒘㒝㒛㒣㒗㒥㒙㒙㒗㒝㒗㒙㒦㒥㒦㒡㒟㒚㒦㒙㒙㒜㒥㒡㒙㒗㒥㒙㒥㒗㒤㒡㒥㒝㒤㒙㒣㒥㒤㒢㒣㒝㒠㒝㒢㒥㒦㒘㒢㒝㒥㒙㒡㒥㒡㒡㒢㒞㒡㒙㒢㒣㒠㒡㒦㒛㒠㒙㒡㒗㒟㒡㒟㒝㒢㒠㒞㒥㒝㒟㒞㒝㒞㒙㒝㒥㒟㒡㒝㒝㒝㒙㒠㒜㒜㒡㒟㒤㒜㒙㒞㒛㒛㒡㒜㒟㒛㒙㒚㒥㒞㒙㒚㒝㒥㒛㒙㒥㒙㒡㒙㒝㒚㒛㒘㒥㒘㒡㒛㒦㒘㒙㒤㒠㒗㒡㒗㒝㒗㒙㒘㒗㒦㒡㒦㒝㒙㒣㒥㒥㒢㒜㒥㒝㒥㒙㒤㒥㒥㒣㒤㒝㒤㒙㒗㒠㒣㒡㒠㒘㒣㒙㒢㒥㒢㒡㒢㒝㒢㒙㒡㒥㒥㒘㒡㒝㒤㒤㒠㒥㒠㒣㒠㒝㒡㒙㒟㒥㒟㒡㒠㒞㒟㒙㒡㒣㒞㒡㒡㒤㒞㒙㒟㒗㒝㒡㒝㒝㒠㒠㒜㒥㒛㒟㒜㒝㒜㒙㒛㒥㒝㒡㒛㒝㒛㒙㒞㒜㒚㒡㒝㒤㒚㒙㒜㒛㒙㒡㒚㒟㒙㒙㒘㒥㒜㒙㒘㒝㒤㒤㒗㒥㒗㒡㒗㒝㒘㒛㒦㒥㒦㒡㒙㒦㒦㒙㒡㒜㒥㒡㒥㒝㒥㒙㒦㒗㒤㒡㒤㒝㒗㒣㒣㒥㒠㒜㒣㒝㒣㒙㒢㒥㒣㒣㒢㒝㒢㒙㒥㒠㒡㒡㒦㒤㒡㒙㒠㒥㒠㒡㒠㒝㒠㒙㒟㒥㒣㒘㒟㒝㒢㒤㒞㒥㒞㒣㒞㒝㒟㒙㒝㒥㒝㒡㒞㒞㒝㒙㒡㒘㒜㒡㒟㒤㒜㒙㒝㒗㒛㒡㒛㒝㒞㒠㒚㒥㒢㒠㒚㒝㒚㒙㒙㒥㒛㒡㒙㒝㒙㒙㒜㒜㒘㒡㒛㒤㒘㒙㒠㒝㒗㒡㒙㒝㒗㒙㒦㒥㒚㒘㒦㒝㒙㒠㒥㒥㒜㒤㒥㒝㒦㒙㒤㒥㒤㒡㒥㒞㒤㒙㒜㒝㒣㒡㒦㒤㒣㒙㒥㒥㒢㒡㒢㒝㒣㒚㒡㒥㒢㒥㒡㒝㒚㒝㒠㒥㒡㒣㒠㒝㒠㒙㒣㒜㒟㒡㒢㒞㒟㒙㒞㒥㒞㒡㒠㒝㒞㒙㒝㒥㒡㒘㒝㒝㒠㒠㒜㒥㒜㒡㒜㒞㒝㒛㒛㒥㒛㒡㒞㒥㒛㒙㒗㒠㒚㒡㒚㒝㒚㒙㒛㒗㒙㒡㒙㒝㒜㒢㒘㒥㒥㒜㒘㒝㒘㒙㒗㒥㒘㒣㒗㒝㒗㒙㒚㒟㒦㒡㒣㒘㒦㒙㒥㒥㒥㒡㒥㒝㒥㒙㒤㒥㒘㒘㒤㒝㒗㒣㒣㒥㒣㒣㒣㒝㒤㒙㒢㒥㒢㒡㒣㒞㒢㒙㒛㒡㒡㒡㒤㒤㒡㒙㒣㒥㒠㒡㒠㒝㒡㒚㒟㒥㒥㒞㒟㒝㒠㒣㒞㒥㒡㒡㒞㒝㒞㒙㒞㒦㒝㒡㒞㒙㒝㒙㒝㒞㒜㒢㒟㒝㒜㒙㒛㒥㒜㒢㒛㒝㒦㒟㒚㒥㒜㒛㒚㒝㒝㒙㒙㒥㒙㒡㒚㒟㒙㒙㒠㒙㒘㒡㒘㒞㒘㒙㒘㒥㒗㒡㒗㒝㒘㒛㒦㒥㒛㒣㒦㒝㒦㒛㒥㒥㒦㒣㒥㒝㒥㒙㒘㒜㒤㒡㒗㒞㒤㒙㒣㒥㒣㒡㒥㒝㒣㒙㒢㒥㒦㒘㒢㒝㒥㒠㒡㒥㒡㒡㒡㒞㒢㒛㒠㒥㒠㒡㒣㒥㒠㒙㒜㒠㒟㒡㒟㒝㒟㒙㒠㒗㒞㒡㒞㒝㒡㒢㒝㒥㒚㒜㒝㒝㒝㒙㒜㒥㒝㒣㒜㒝㒜㒙㒟㒟㒛㒡㒘㒘㒛㒙㒚㒥㒚㒡㒚㒝㒚㒙㒙㒥㒝㒘㒙㒝㒜㒣㒘㒥㒘㒣㒘㒝㒙㒙㒗㒥㒗㒡㒘㒟㒗㒙㒤㒙㒦㒡㒙㒤㒦㒙㒘㒥㒥㒡㒥㒝㒦㒛㒤㒥㒦㒟㒤㒝㒞㒦㒣㒥㒤㒣㒣㒝㒣㒙㒦㒜㒢㒡㒥㒞㒢㒙㒡㒥㒡㒡㒣㒝㒡㒙㒠㒥㒤㒘㒠㒝㒣㒠㒟㒥㒟㒡㒟㒞㒠㒛㒞㒥㒞㒡㒡㒥㒞㒙㒛㒜㒝㒡㒝㒝㒝㒙㒞㒗㒜㒡㒜㒝㒟㒢㒛㒥㒙㒘㒛㒝㒛㒙㒚㒥㒛㒣㒚㒝㒚㒙㒝㒟㒙㒡㒦㒤㒙㒙㒘㒥㒘㒡㒘㒝㒘㒙㒗㒥㒛㒘㒗㒝㒚㒣㒦㒥㒦㒣㒦㒝㒗㒙㒥㒥㒥㒡㒦㒟㒥㒙㒦㒠㒤㒢㒗㒤㒤㒙㒦㒥㒣㒡㒣㒝㒤㒛㒢㒥㒡㒙㒢㒝㒙㒘㒡㒥㒢㒣㒡㒝㒡㒙㒤㒜㒠㒡㒟㒛㒠㒙㒟㒥㒟㒡㒡㒝㒟㒙㒞㒥㒢㒘㒞㒝㒡㒠㒝㒥㒠㒗㒝㒝㒞㒛㒜㒥㒜㒡㒟㒥㒜㒙㒜㒝㒛㒢㒛㒝㒛㒙㒜㒗㒚㒡㒚㒝㒝㒢㒙㒥㒦㒜㒙㒝㒙㒙㒘㒥㒙㒣㒘㒝㒘㒙㒛㒟㒗㒡㒚㒚㒗㒙㒦㒥㒦㒡㒗㒟㒦㒙㒥㒥㒙㒜㒥㒝㒡㒤㒤㒥㒤㒡㒤㒝㒤㒙㒣㒥㒣㒡㒦㒤㒣㒙㒦㒠㒢㒡㒢㒟㒢㒙㒢㒥㒡㒡㒡㒝㒢㒛㒠㒥㒣㒟㒠㒝㒣㒠㒟㒥㒠㒣㒟㒝㒟㒙㒢㒜㒞㒡㒝㒛㒞㒙㒝㒥㒝㒡㒟㒝㒝㒙㒜㒥㒠㒘㒜㒝㒟㒠㒛㒥㒞㒗㒛㒝㒜㒛㒚㒥㒚㒡㒝㒥㒚㒙㒦㒠㒙㒡㒙㒝㒙㒙㒚㒗㒘㒡㒘㒝㒛㒢㒗㒥㒥㒝㒗㒝㒗㒙㒦㒥㒗㒣㒦㒝㒦㒙㒙㒟㒥㒡㒢㒘㒥㒙㒤㒥㒤㒡㒥㒟㒤㒙㒣㒥㒗㒜㒣㒝㒟㒘㒢㒥㒢㒡㒢㒝㒢㒙㒡㒥㒡㒡㒤㒤㒡㒙㒤㒠㒠㒡㒠㒟㒠㒙㒠㒥㒟㒡㒟㒝㒠㒛㒞㒥㒢㒤㒞㒝㒡㒠㒝㒥㒠㒡㒝㒝㒝㒙㒞㒘㒜㒡㒣㒡㒜㒙㒜㒚㒛㒡㒜㒝㒛㒙㒚㒥㒛㒤㒚㒝㒟㒛㒙㒥㒚㒣㒙㒝㒚㒛㒘㒥㒘㒡㒛㒤㒘㒙㒚㒦㒗㒡㒗㒝㒗㒙㒘㒥㒦㒡㒦㒝㒙㒠㒥㒥㒙㒘㒥㒝㒥㒙㒤㒦㒥㒣㒤㒝㒤㒙㒗㒝㒣㒡㒤㒥㒣㒙㒢㒥㒢㒡㒣㒟㒢㒙㒡㒥㒥㒚㒡㒝㒢㒡㒠㒥㒠㒡㒠㒝㒡㒛㒟㒥㒟㒡㒣㒗㒟㒙㒠㒝㒞㒡㒞㒝㒞㒙㒝㒥㒝㒡㒝㒝㒠㒠㒜㒥㒠㒛㒜㒝㒜㒛㒛㒥㒜㒡㒛㒝㒛㒙㒜㒘㒚㒡㒗㒡㒚㒙㒝㒜㒙㒡㒜㒝㒙㒙㒘㒥㒙㒤㒘㒝㒚㒗㒗㒥㒝㒟㒗㒝㒘㒛㒦㒥㒦㒡㒙㒤㒦㒙㒤㒣㒥㒡㒥㒝㒥㒙㒦㒥㒤㒡㒤㒝㒗㒠㒣㒥㒗㒘㒣㒝㒥㒟㒢㒥㒣㒣㒙㒦㒢㒙㒥㒝㒡㒡㒞㒠㒡㒙㒠㒥㒠㒡㒡㒟㒠㒙㒟㒥㒣㒚㒟㒝㒛㒤㒞㒥㒞㒡㒞㒝㒟㒛㒝㒥㒝㒡㒡㒗㒝㒙㒙㒟㒜㒡㒜㒝㒜㒙㒝㒗㒛㒡㒛㒝㒞㒤㒚㒥㒗㒜㒚㒝㒚㒙㒙㒥㒙㒡㒙㒝㒙㒙㒜㒜㒘㒡㒜㒘㒘㒙㒘㒗㒗㒡㒘㒝㒗㒙㒦㒥㒗㒤㒦㒝㒙㒗㒥㒥㒙㒘㒥㒝㒦㒛㒤㒥㒤㒡㒗㒤㒤㒙㒢㒣㒣㒡㒣㒝㒣㒙㒤㒥㒢㒡㒢㒝㒥㒠㒡㒥㒥㒘㒡㒝㒣㒟㒠㒥㒡㒣㒠㒝㒠㒙㒣㒝㒟㒡㒜㒘㒟㒙㒞㒥㒞㒡㒟㒟㒞㒙㒝㒥㒡㒚㒝㒝㒝㒝㒜㒥㒜㒡㒜㒝㒝㒛㒛㒥㒛㒡㒟㒗㒛㒙㒗㒠㒚㒡㒚㒝㒚㒙㒛㒗㒙㒡㒙㒝㒜㒤㒘㒥㒜㒣㒘㒝㒘㒙㒗㒥㒗㒡㒗㒝㒗㒙㒚㒜㒦㒡㒚㒘㒦㒙㒦㒗㒥㒡㒦㒝㒥㒙㒤㒥㒥㒤㒤㒝㒘㒜㒣㒥㒗㒘㒣㒝㒤㒛㒢㒥㒢㒡㒥㒤㒢㒙㒙㒤㒡㒡㒡㒝㒡㒙㒢㒥㒠㒡㒠㒝㒣㒠㒟㒥㒣㒘㒟㒝㒗㒡㒞㒥㒠㒡㒞㒝㒞㒙㒡㒜㒝㒡㒠㒤㒝㒙㒠㒡㒜㒡㒝㒝㒜㒙㒛㒥㒜㒤㒛㒝㒣㒡㒚㒥㒞㒘㒚㒝㒝㒙㒙㒥㒙㒡㒚㒠㒙㒙㒚㒙㒘㒡㒛㒣㒘㒙㒙㒗㒗㒡㒗㒝㒚㒠㒦㒥㒙㒢㒦㒝㒦㒙㒥㒥㒗㒡㒥㒝㒥㒙㒘㒜㒤㒡㒗㒤㒤㒙㒣㒥㒣㒢㒤㒟㒣㒙㒢㒥㒦㒙㒢㒝㒚㒤㒡㒥㒡㒡㒡㒝㒢㒛㒠㒥㒠㒡㒣㒦㒠㒙㒠㒢㒟㒢㒟㒝㒟㒙㒠㒗㒞㒡㒞㒝㒡㒣㒝㒥㒞㒞㒝㒞㒝㒙㒜㒥㒜㒡㒜㒝㒜㒙㒟㒜㒛㒡㒟㒗㒛㒙㒛㒗㒚㒡㒛㒝㒚㒙㒙㒥㒚㒤㒙㒝㒢㒥㒘㒥㒜㒘㒘㒝㒛㒙㒗㒥㒗㒡㒘㒠㒗㒙㒜㒢㒦㒡㒘㒗㒦㒙㒘㒥㒥㒡㒥㒝㒦㒜㒤㒥㒥㒝㒤㒝㒤㒢㒣㒦㒦㒡㒣㒝㒣㒙㒤㒘㒢㒡㒝㒣㒢㒙㒣㒟㒡㒡㒤㒝㒡㒙㒠㒥㒡㒥㒠㒝㒗㒝㒟㒥㒗㒙㒟㒝㒠㒙㒞㒥㒞㒡㒟㒡㒞㒙㒣㒗㒝㒡㒞㒟㒝㒙㒞㒗㒜㒡㒜㒝㒟㒠㒛㒥㒞㒢㒛㒝㒛㒙㒚㒥㒜㒡㒚㒝㒚㒙㒝㒜㒙㒡㒜㒤㒙㒙㒘㒥㒘㒢㒙㒟㒘㒙㒗㒥㒛㒙㒗㒝㒘㒡㒦㒥㒦㒡㒦㒝㒗㒛㒥㒥㒥㒡㒘㒦㒥㒙㒦㒝㒤㒡㒤㒝㒤㒙㒥㒗㒣㒡㒣㒝㒦㒣㒢㒥㒤㒙㒢㒝㒢㒙㒡㒥㒡㒡㒡㒝㒡㒙㒤㒜㒠㒡㒤㒗㒠㒙㒠㒗㒟㒡㒠㒝㒟㒙㒞㒥㒟㒥㒞㒝㒛㒝㒝㒥㒡㒘㒝㒝㒠㒙㒜㒥㒜㒡㒝㒡㒜㒙㒝㒣㒛㒡㒡㒛㒛㒙㒜㒗㒚㒡㒚㒝㒝㒠㒙㒥㒘㒟㒙㒝㒙㒙㒘㒥㒚㒡㒘㒝㒘㒙㒛㒜㒗㒡㒚㒤㒗㒙㒙㒛㒦㒡㒗㒟㒦㒙㒥㒥㒙㒙㒥㒝㒟㒡㒤㒥㒤㒡㒤㒝㒥㒛㒣㒥㒣㒡㒦㒦㒣㒙㒟㒠㒢㒡㒢㒝㒢㒙㒣㒗㒡㒡㒡㒝㒤㒣㒠㒥㒝㒛㒠㒝㒠㒙㒟㒥㒠㒣㒟㒝㒟㒙㒢㒠㒞㒡㒛㒘㒞㒙㒝㒥㒝㒡㒝㒝㒝㒙㒜㒥㒠㒘㒜㒝㒟㒤㒛㒥㒛㒣㒛㒝㒜㒙㒚㒥㒚㒡㒛㒡㒚㒙㒜㒣㒙㒡㒜㒤㒙㒙㒚㒗㒘㒡㒘㒝㒛㒠㒗㒥㒦㒟㒗㒝㒗㒙㒦㒥㒘㒡㒦㒝㒦㒙㒙㒜㒥㒡㒘㒤㒥㒙㒗㒛㒤㒡㒥㒟㒤㒙㒣㒥㒗㒙㒣㒝㒟㒤㒢㒥㒢㒡㒢㒝㒣㒛㒡㒥㒡㒡㒤㒦㒡㒙㒡㒙㒠㒡㒠㒝㒠㒙㒡㒗㒟㒡㒟㒝㒢㒣㒞㒥㒛㒜㒞㒝㒞㒙㒝㒥㒞㒣㒝㒝㒝㒙㒠㒠㒜㒡㒠㒟㒜㒙㒛㒥㒛㒡㒛㒝㒛㒙㒚㒥㒞㒘㒚㒝㒝㒤㒙㒥㒙㒣㒙㒝㒚㒙㒘㒥㒘㒡㒙㒡㒘㒙㒜㒘㒗㒡㒚㒤㒗㒙㒘㒗㒦㒡㒦㒝㒙㒠㒥㒥㒝㒠㒥㒝㒥㒙㒤㒥㒦㒡㒤㒝㒤㒙㒗㒜㒣㒡㒦㒤㒣㒙㒛㒝㒢㒡㒤㒝㒢㒙㒡㒥㒥㒘㒡㒝㒤㒠㒠㒥㒤㒝㒠㒝㒡㒙㒟㒥㒟㒡㒠㒡㒟㒙㒗㒝㒞㒡㒡㒤㒞㒙㒠㒥㒝㒡㒝㒝㒞㒝㒜㒥㒝㒥㒜㒝㒚㒘㒛㒥㒜㒣㒛㒝㒛㒙㒞㒜㒚㒡㒝㒞㒚㒙㒙㒥㒙㒡㒛㒝㒙㒙㒘㒥㒜㒘㒘㒝㒛㒠㒗㒥㒗㒡㒗㒞㒘㒛㒦㒥㒦㒡㒙㒥㒦㒙㒤㒚㒥㒡㒥㒝㒥㒙㒦㒗㒤㒡㒤㒝㒗㒢㒣㒥㒦㒠㒣㒝㒣㒙㒢㒥㒣㒣㒢㒝㒢㒙㒥㒟㒡㒡㒡㒥㒡㒙㒠㒥㒠㒡㒠㒝㒠㒙㒟㒥㒣㒘㒟㒝㒢㒣㒞㒥㒞㒣㒞㒝㒟㒙㒝㒥㒝㒡㒞㒡㒝㒙㒦㒡㒜㒡㒟㒤㒜㒙㒞㒥㒛㒡㒛㒝㒜㒝㒚㒥㒠㒞㒚㒝㒛㒣㒙㒥㒜㒡㒙㒝㒙㒙㒚㒙㒘㒡㒙㒙㒘㒙㒘㒞㒗㒢㒚㒝㒗㒙㒦㒥㒗㒥㒦㒝㒡㒟㒥㒥㒗㒛㒥㒝㒘㒙㒤㒥㒤㒡㒥㒢㒤㒙㒛㒙㒣㒡㒥㒦㒣㒙㒣㒥㒢㒡㒢㒝㒣㒞㒡㒥㒦㒣㒡㒝㒢㒛㒠㒥㒡㒣㒠㒝㒠㒙㒣㒜㒟㒡㒢㒞㒟㒙㒞㒥㒞㒡㒠㒝㒞㒙㒝㒥㒡㒘㒝㒝㒠㒠㒜㒥㒜㒡㒜㒞㒝㒛㒛㒥㒛㒡㒞㒥㒛㒙㒜㒝㒚㒡㒚㒝㒚㒙㒛㒗㒙㒡㒙㒝㒜㒢㒘㒥㒚㒙㒘㒝㒘㒙㒗㒥㒘㒣㒗㒝㒗㒙㒚㒟㒦㒡㒗㒥㒦㒙㒥㒥㒥㒡㒥㒝㒥㒙㒤㒥㒘㒘㒤㒝㒗㒣㒣㒥㒣㒣㒣㒝㒤㒙㒢㒥㒢㒡㒣㒢㒢㒙㒟㒙㒡㒡㒤㒤㒡㒙㒣㒥㒠㒡㒠㒝㒡㒞㒟㒥㒡㒟㒟㒝㒥㒗㒞㒥㒟㒣㒗㒠㒞㒙㒡㒜㒝㒡㒜㒛㒝㒙㒜㒥㒜㒡㒞㒝㒜㒙㒛㒥㒟㒘㒛㒝㒞㒠㒚㒥㒝㒗㒚㒝㒛㒛㒙㒥㒙㒡㒜㒥㒙㒙㒡㒛㒘㒡㒘㒝㒘㒙㒙㒗㒗㒡㒗㒝㒚㒢㒦㒥㒣㒜㒦㒝㒦㒙㒥㒥㒦㒣㒥㒝㒥㒙㒘㒟㒤㒡㒡㒗㒤㒙㒣㒥㒣㒡㒤㒟㒣㒙㒢㒥㒦㒜㒢㒝㒞㒤㒡㒥㒡㒡㒡㒝㒡㒙㒠㒥㒠㒡㒣㒤㒠㒙㒣㒠㒟㒡㒟㒟㒟㒙㒟㒥㒞㒡㒞㒝㒟㒞㒝㒥㒠㒟㒝㒝㒠㒠㒜㒥㒝㒣㒜㒝㒜㒙㒟㒜㒛㒡㒚㒛㒛㒙㒚㒥㒚㒡㒜㒝㒚㒙㒙㒥㒝㒘㒙㒝㒜㒠㒘㒥㒛㒗㒘㒝㒙㒛㒗㒥㒗㒡㒚㒥㒗㒙㒣㒠㒦㒡㒦㒝㒦㒙㒗㒗㒥㒡㒥㒝㒘㒢㒤㒥㒠㒘㒤㒝㒤㒙㒣㒥㒤㒣㒣㒝㒣㒙㒦㒟㒢㒡㒟㒘㒢㒙㒡㒥㒡㒡㒢㒟㒡㒙㒠㒥㒤㒜㒠㒝㒤㒛㒟㒥㒟㒡㒟㒝㒟㒙㒞㒥㒞㒡㒡㒤㒞㒙㒡㒠㒝㒡㒝㒟㒝㒙㒝㒥㒜㒡㒜㒝㒝㒞㒛㒥㒟㒤㒛㒝㒞㒠㒚㒥㒛㒣㒚㒝㒚㒙㒝㒜㒙㒡㒡㒜㒙㒙㒘㒥㒘㒡㒚㒝㒘㒙㒗㒥㒛㒘㒗㒝㒚㒠㒦㒥㒟㒙㒦㒝㒘㒙㒥㒥㒥㒡㒘㒤㒥㒙㒘㒜㒤㒡㒘㒙㒤㒙㒤㒥㒣㒡㒣㒝㒤㒞㒢㒥㒛㒙㒢㒝㒥㒠㒡㒥㒤㒡㒡㒝㒡㒙㒢㒚㒠㒡㒡㒡㒠㒙㒡㒡㒟㒡㒠㒟㒟㒙㒞㒥㒢㒘㒞㒝㒡㒚㒝㒥㒝㒡㒝㒝㒟㒙㒜㒥㒜㒡㒟㒤㒜㒙㒟㒜㒛㒡㒛㒝㒛㒚㒜㒗㒚㒡㒚㒝㒝㒡㒙㒥㒟㒠㒙㒝㒙㒙㒘㒥㒙㒣㒘㒝㒘㒙㒛㒞㒗㒡㒘㒡㒗㒚㒦㒥㒦㒡㒗㒟㒦㒙㒥㒥㒙㒛㒥㒝㒡㒤㒤㒥㒤㒡㒤㒝㒤㒙㒣㒥㒣㒡㒦㒤㒣㒙㒦㒟㒢㒡㒢㒟㒢㒙㒢㒥㒡㒡㒡㒝㒢㒞㒠㒥㒚㒝㒠㒝㒣㒠㒟㒥㒢㒡㒟㒝㒟㒙㒠㒚㒞㒡㒤㒚㒞㒙㒟㒟㒝㒡㒠㒝㒝㒙㒜㒥㒝㒦㒜㒝㒜㒥㒛㒥㒜㒚㒛㒞㒞㒙㒚㒥㒚㒡㒛㒢㒚㒙㒥㒛㒙㒡㒛㒗㒙㒙㒛㒥㒘㒡㒘㒝㒙㒟㒗㒥㒞㒥㒗㒝㒘㒠㒦㒥㒗㒡㒦㒝㒦㒙㒗㒛㒥㒡㒚㒟㒥㒙㒦㒗㒤㒡㒥㒟㒤㒙㒣㒥㒗㒘㒣㒝㒦㒚㒢㒥㒢㒡㒢㒝㒤㒙㒡㒥㒡㒡㒤㒤㒡㒙㒤㒜㒠㒡㒠㒝㒠㒚㒡㒗㒟㒡㒟㒝㒢㒡㒞㒥㒠㒙㒞㒝㒞㒙㒝㒥㒞㒣㒝㒝㒝㒙㒠㒞㒜㒡㒝㒥㒜㒙㒛㒥㒛㒡㒜㒟㒛㒙㒚㒥㒞㒛㒚㒝㒛㒡㒙㒥㒙㒡㒙㒝㒙㒙㒘㒥㒘㒡㒛㒤㒘㒙㒛㒟㒗㒡㒗㒟㒗㒙㒗㒥㒦㒡㒦㒝㒗㒟㒥㒥㒢㒥㒥㒝㒘㒠㒤㒥㒗㒡㒤㒝㒤㒙㒥㒛㒣㒡㒥㒛㒣㒙㒘㒣㒢㒡㒣㒟㒢㒙㒡㒥㒥㒘㒡㒝㒠㒗㒠㒥㒠㒡㒠㒝㒢㒙㒟㒥㒟㒡㒢㒤㒟㒙㒢㒜㒞㒡㒠㒣㒞㒙㒟㒗㒝㒡㒝㒝㒠㒡㒜㒥㒛㒥㒜㒝㒜㒙㒛㒥㒜㒣㒛㒝㒛㒙㒞㒞㒚㒡㒗㒘㒚㒙㒙㒥㒙㒡㒚㒟㒙㒙㒘㒥㒜㒛㒘㒝㒤㒣㒗㒥㒗㒡㒗㒝㒘㒛㒦㒥㒦㒡㒚㒘㒦㒙㒢㒠㒥㒡㒥㒝㒥㒙㒤㒥㒤㒡㒤㒝㒗㒠㒣㒥㒗㒜㒣㒝㒣㒛㒢㒥㒣㒡㒢㒝㒢㒙㒣㒛㒡㒡㒤㒛㒡㒙㒤㒜㒠㒡㒡㒟㒠㒙㒟㒥㒣㒘㒟㒝㒞㒗㒞㒥㒞㒡㒞㒝㒠㒙㒝㒥㒝㒡㒠㒤㒝㒙㒠㒜㒜㒡㒞㒣㒜㒙㒝㒗㒛㒡㒛㒝㒞㒡㒚㒥㒗㒜㒚㒝㒚㒙㒙㒥㒚㒣㒙㒝㒙㒙㒜㒞㒘㒡㒣㒤㒘㒙㒗㒥㒗㒡㒘㒟㒗㒙㒦㒥㒚㒛㒦㒝㒢㒤㒥㒥㒥㒡㒥㒝㒦㒛㒤㒥㒤㒡㒘㒘㒤㒙㒘㒗㒣㒡㒣㒝㒣㒙㒢㒥㒢㒡㒢㒝㒥㒠㒡㒥㒥㒜㒡㒝㒡㒛㒠㒥㒡㒡㒠㒝㒠㒙㒡㒛㒟㒡㒣㒠㒟㒙㒢㒜㒞㒡㒟㒟㒞㒙㒝㒥㒡㒘㒝㒝㒥㒘㒜㒥㒜㒡㒜㒝㒞㒙㒛㒥㒛㒡㒞㒤㒛㒙㒞㒜㒚㒡㒢㒥㒚㒙㒛㒥㒙㒡㒙㒝㒜㒠㒘㒥㒜㒘㒘㒝㒛㒥㒗㒥㒘㒡㒗㒝㒗㒙㒘㒛㒦㒡㒞㒥㒦㒙㒙㒜㒥㒡㒘㒝㒥㒙㒤㒥㒦㒗㒤㒝㒥㒝㒣㒥㒦㒚㒣㒝㒤㒛㒢㒥㒢㒡㒥㒤㒢㒙㒤㒦㒡㒡㒡㒝㒡㒙㒢㒥㒠㒡㒠㒝㒣㒠㒟㒥㒣㒘㒟㒝㒟㒙㒞㒦㒟㒣㒞㒝㒞㒙㒡㒝㒝㒡㒦㒘㒝㒙㒜㒥㒜㒡㒝㒟㒜㒙㒛㒥㒟㒚㒛㒝㒛㒦㒚㒦㒚㒡㒚㒝㒛㒛㒙㒥㒙㒡㒝㒗㒙㒙㒙㒢㒘㒢㒘㒝㒘㒙㒗㒥㒗㒡㒗㒝㒚㒠㒦㒥㒚㒛㒦㒝㒦㒛㒥㒥㒦㒡㒥㒝㒥㒙㒦㒛㒤㒡㒞㒙㒤㒙㒗㒜㒣㒡㒦㒝㒣㒙㒢㒥㒤㒗㒢㒝㒗㒦㒡㒥㒣㒛㒡㒝㒤㒙㒠㒥㒠㒡㒡㒣㒠㒙㒠㒡㒟㒡㒟㒦㒟㒚㒡㒥㒞㒡㒞㒝㒟㒟㒝㒥㒙㒗㒝㒝㒞㒣㒜㒥㒟㒡㒜㒝㒜㒙㒝㒜㒛㒡㒢㒡㒛㒙㒘㒤㒚㒡㒛㒝㒚㒙㒙㒥㒛㒘㒙㒝㒞㒛㒘㒥㒙㒣㒘㒝㒙㒛㒗㒥㒗㒡㒚㒤㒗㒙㒙㒦㒦㒡㒦㒝㒦㒙㒗㒥㒥㒡㒥㒝㒘㒠㒤㒥㒘㒘㒤㒝㒤㒙㒣㒦㒤㒣㒣㒝㒣㒙㒦㒝㒢㒡㒣㒥㒢㒙㒡㒥㒡㒡㒢㒟㒡㒙㒠㒥㒤㒚㒠㒝㒡㒡㒟㒥㒟㒡㒟㒝㒠㒛㒞㒥㒞㒡㒢㒗㒞㒙㒟㒝㒝㒡㒝㒝㒝㒙㒜㒥㒜㒡㒜㒝㒟㒠㒛㒥㒟㒛㒛㒝㒛㒛㒚㒥㒛㒡㒣㒛㒚㒙㒛㒜㒙㒡㒦㒡㒙㒙㒜㒜㒘㒡㒛㒝㒘㒙㒗㒥㒙㒘㒗㒝㒙㒗㒦㒥㒜㒟㒦㒝㒗㒛㒥㒥㒥㒡㒘㒤㒥㒙㒣㒣㒤㒡㒤㒝㒤㒙㒥㒥㒣㒡㒣㒝㒦㒠㒢㒥㒦㒘㒢㒝㒤㒟㒡㒥㒢㒣㒡㒝㒡㒙㒤㒝㒠㒡㒥㒝㒠㒙㒟㒥㒟㒡㒠㒟㒟㒙㒞㒥㒢㒚㒞㒝㒚㒤㒝㒥㒝㒡㒝㒝㒞㒛㒜㒥㒜㒡㒠㒗㒜㒙㒘㒟㒛㒡㒛㒝㒛㒙㒜㒗㒚㒡㒚㒝㒝㒤㒙㒥㒦㒜㒙㒝㒙㒙㒘㒥㒘㒡㒘㒝㒘㒙㒛㒜㒗㒡㒛㒘㒗㒙㒗㒗㒦㒡㒗㒝㒦㒙㒥㒥㒗㒘㒥㒝㒘㒗㒤㒥㒘㒘㒤㒝㒥㒛㒣㒥㒣㒡㒦㒤㒣㒙㒡㒣㒢㒡㒢㒝㒢㒙㒣㒥㒡㒡㒡㒝㒤㒠㒠㒥㒤㒘㒠㒝㒢㒟㒟㒥㒠㒣㒟㒝㒟㒙㒢㒝㒞㒡㒛㒘㒞㒙㒝㒥㒝㒡㒞㒟㒝㒙㒜㒥㒠㒚㒜㒝㒗㒠㒛㒥㒛㒡㒛㒝㒜㒛㒚㒥㒚㒡㒞㒗㒚㒙㒦㒠㒙㒡㒙㒝㒙㒙㒚㒗㒘㒡㒘㒝㒛㒤㒗㒥㒛㒣㒗㒝㒗㒙㒦㒥㒦㒡㒦㒝㒦㒙㒙㒜㒥㒡㒙㒘㒥㒙㒥㒗㒤㒡㒥㒝㒤㒙㒣㒥㒥㒘㒣㒝㒗㒜㒢㒥㒦㒘㒢㒝㒣㒛㒡㒥㒡㒡㒤㒤㒡㒙㒘㒤㒠㒡㒠㒝㒠㒙㒡㒥㒟㒡㒟㒝㒢㒠㒞㒥㒢㒘㒞㒝㒦㒡㒝㒥㒟㒡㒝㒝㒝㒙㒠㒜㒜㒡㒟㒤㒜㒙㒟㒡㒛㒡㒜㒝㒛㒙㒚㒥㒜㒘㒚㒝㒢㒡㒙㒥㒝㒘㒙㒝㒜㒙㒘㒥㒘㒡㒙㒤㒘㒙㒙㒙㒗㒡㒙㒙㒗㒙㒘㒗㒦㒡㒦㒝㒙㒠㒥㒥㒘㒢㒥㒝㒥㒙㒤㒥㒦㒡㒤㒝㒤㒙㒗㒜㒣㒡㒦㒤㒣㒙㒢㒥㒢㒢㒣㒟㒢㒙㒡㒥㒥㒙㒡㒝㒘㒢㒠㒥㒠㒡㒠㒝㒡㒛㒟㒥㒟㒡㒢㒦㒟㒙㒟㒝㒞㒡㒞㒝㒞㒙㒟㒗㒝㒡㒝㒝㒠㒣㒜㒥㒡㒦㒜㒝㒜㒙㒛㒥㒛㒡㒛㒝㒛㒙㒞㒜㒚㒡㒞㒗㒚㒙㒚㒗㒙㒡㒚㒝㒙㒙㒘㒥㒚㒘㒘㒝㒡㒥㒗㒥㒛㒘㒗㒝㒚㒙㒦㒥㒦㒡㒗㒤㒦㒙㒛㒢㒥㒡㒗㒗㒥㒙㒗㒥㒤㒡㒤㒝㒥㒠㒣㒥㒤㒝㒣㒝㒣㒢㒢㒦㒥㒡㒢㒝㒢㒙㒣㒜㒡㒡㒜㒣㒡㒙㒢㒟㒠㒡㒣㒝㒠㒙㒟㒥㒡㒙㒟㒝㒦㒝㒞㒥㒟㒚㒞㒝㒟㒙㒝㒥㒝㒡㒞㒥㒝㒙㒢㒗㒜㒡㒝㒟㒜㒙㒝㒗㒛㒡㒛㒝㒞㒠㒚㒥㒝㒢㒚㒝㒚㒙㒙㒥㒛㒡㒙㒝㒙㒙㒜㒜㒘㒡㒛㒤㒘㒙㒗㒥㒗㒢㒘㒟㒗㒙㒦㒥㒚㒙㒦㒝㒗㒡㒥㒥㒥㒡㒥㒝㒦㒛㒤㒥㒤㒡㒗㒦㒤㒙㒥㒝㒣㒡㒣㒝㒣㒙㒤㒗㒢㒡㒢㒝㒥㒣㒡㒥㒣㒙㒡㒝㒡㒙㒠㒥㒠㒡㒠㒝㒠㒙㒣㒜㒟㒡㒣㒗㒟㒙㒟㒗㒞㒡㒟㒝㒞㒙㒝㒥㒟㒙㒝㒝㒚㒝㒜㒥㒠㒘㒜㒝㒟㒙㒛㒥㒛㒡㒜㒥㒛㒙㒜㒣㒚㒡㒠㒛㒚㒙㒛㒗㒙㒡㒙㒝㒜㒠㒘㒥㒗㒟㒘㒝㒘㒙㒗㒥㒙㒡㒗㒝㒗㒙㒚㒜㒦㒡㒙㒤㒦㒙㒘㒛㒥㒡㒦㒟㒥㒙㒤㒥㒘㒙㒤㒝㒥㒦㒣㒥㒣㒡㒣㒝㒤㒛㒢㒥㒢㒡㒥㒦㒢㒙㒞㒠㒡㒡㒡㒝㒡㒙㒢㒗㒠㒡㒠㒝㒣㒣㒟㒥㒜㒛㒟㒝㒟㒙㒞㒥㒟㒣㒞㒝㒞㒙㒡㒠㒝㒡㒚㒘㒝㒙㒜㒥㒜㒡㒜㒝㒜㒙㒛㒥㒟㒘㒛㒝㒞㒤㒚㒥㒚㒣㒚㒝㒛㒙㒙㒥㒙㒡㒚㒥㒙㒙㒛㒣㒘㒡㒛㒤㒘㒙㒙㒗㒗㒡㒗㒝㒚㒠㒦㒥㒥㒟㒦㒝㒦㒙㒥㒥㒗㒡㒥㒝㒥㒙㒘㒜㒤㒡㒗㒤㒤㒙㒦㒛㒣㒡㒤㒟㒣㒙㒢㒥㒦㒙㒢㒝㒞㒤㒡㒥㒡㒡㒡㒝㒢㒛㒠㒥㒠㒡㒣㒦㒠㒙㒛㒜㒟㒡㒟㒝㒟㒙㒠㒗㒞㒡㒞㒝㒡㒣㒝㒥㒚㒜㒝㒝㒝㒙㒜㒥㒝㒣㒜㒝㒜㒙㒟㒠㒛㒡㒟㒟㒛㒙㒚㒥㒚㒡㒚㒝㒚㒙㒙㒥㒝㒘㒙㒝㒜㒤㒘㒥㒘㒣㒘㒝㒙㒙㒗㒥㒗㒡㒘㒥㒗㒙㒛㒘㒦㒡㒙㒤㒦㒙㒗㒗㒥㒡㒥㒝㒘㒠㒤㒥㒜㒠㒤㒝㒤㒙㒣㒥㒥㒡㒣㒝㒣㒙㒦㒜㒢㒡㒥㒤㒢㒙㒚㒝㒡㒡㒣㒝㒡㒙㒠㒥㒤㒘㒠㒝㒣㒠㒟㒥㒣㒝㒟㒝㒠㒙㒞㒥㒞㒡㒟㒥㒞㒙㒦㒝㒝㒡㒠㒤㒝㒙㒟㒥㒜㒡㒜㒝㒝㒡㒛㒥㒜㒥㒛㒝㒞㒤㒚㒥㒛㒣㒚㒝㒚㒙㒝㒜㒙㒡㒜㒞㒙㒙㒘㒥㒘㒡㒚㒝㒘㒙㒗㒥㒛㒘㒗㒝㒚㒠㒦㒥㒦㒡㒦㒞㒗㒛㒥㒥㒥㒡㒘㒥㒥㒙㒗㒥㒤㒡㒤㒝㒤㒙㒥㒗㒣㒡㒣㒝㒦㒢㒢㒥㒣㒙㒢㒝㒢㒙㒡㒥㒢㒣㒡㒝㒡㒙㒤㒟㒠㒡㒟㒗㒠㒙㒟㒥㒟㒡㒟㒝㒟㒙㒞㒥㒢㒘㒞㒝㒡㒣㒝㒥㒝㒣㒝㒝㒞㒙㒜㒥㒜㒡㒝㒥㒜㒙㒥㒡㒛㒡㒞㒤㒛㒙㒝㒥㒚㒡㒚㒝㒛㒡㒙㒥㒟㒞㒙㒝㒚㒣㒘㒥㒛㒡㒘㒝㒘㒙㒙㒝㒗㒡㒘㒙㒗㒙㒗㒞㒦㒢㒙㒝㒦㒙㒥㒥㒗㒙㒥㒝㒠㒟㒤㒥㒦㒛㒤㒝㒗㒙㒣㒥㒣㒡㒤㒦㒣㒙㒚㒙㒢㒡㒤㒝㒢㒙㒢㒥㒡㒡㒡㒝㒢㒢㒠㒥㒥㒣㒠㒝㒡㒛㒟㒥㒠㒣㒟㒝㒟㒙㒢㒜㒞㒡㒡㒞㒞㒙㒝㒥㒝㒡㒟㒝㒝㒙㒜㒥㒠㒘㒜㒝㒟㒠㒛㒥㒛㒡㒛㒞㒜㒛㒚㒥㒚㒡㒝㒥㒚㒙㒛㒝㒙㒡㒙㒝㒙㒙㒚㒗㒘㒡㒘㒝㒛㒢㒗㒥㒙㒙㒗㒝㒗㒙㒦㒥㒗㒣㒘㒝㒦㒙㒙㒟㒥㒡㒦㒥㒥㒙㒤㒥㒤㒡㒤㒝㒛㒜㒣㒥㒗㒘㒣㒝㒦㒣㒢㒥㒢㒣㒢㒝㒣㒙㒚㒣㒡㒡㒢㒦㒡㒙㒞㒙㒠㒡㒣㒤㒠㒙㒢㒥㒟㒡㒟㒝㒠㒢㒞㒥㒠㒟㒞㒝㒤㒗㒝㒥㒞㒣㒝㒝㒝㒙㒠㒜㒜㒡㒛㒛㒜㒙㒛㒥㒛㒡㒝㒝㒛㒙㒚㒥㒞㒘㒚㒝㒝㒠㒙㒥㒜㒗㒙㒝㒚㒛㒘㒥㒘㒡㒛㒥㒘㒙㒠㒦㒗㒡㒗㒝㒗㒙㒘㒗㒦㒡㒦㒝㒙㒢㒥㒥㒢㒜㒥㒝㒥㒙㒤㒥㒥㒣㒤㒝㒤㒙㒗㒟㒣㒡㒠㒗㒣㒙㒢㒥㒢㒡㒣㒟㒢㒙㒡㒥㒥㒜㒡㒝㒝㒤㒠㒥㒠㒡㒠㒝㒠㒙㒟㒥㒟㒡㒢㒤㒟㒙㒢㒠㒞㒡㒞㒟㒞㒙㒞㒥㒝㒡㒝㒝㒞㒢㒜㒥㒟㒟㒜㒝㒟㒠㒛㒥㒜㒣㒛㒝㒛㒙㒞㒜㒚㒡㒙㒛㒚㒙㒙㒥㒙㒡㒛㒝㒙㒙㒘㒥㒜㒘㒘㒝㒛㒠㒗㒥㒚㒗㒗㒝㒘㒛㒦㒥㒦㒡㒙㒥㒦㒙㒢㒠㒥㒡㒥㒝㒥㒙㒦㒗㒤㒡㒤㒝㒗㒢㒣㒥㒣㒥㒣㒝㒣㒙㒢㒥㒣㒣㒢㒝㒢㒙㒥㒟㒡㒡㒞㒘㒡㒙㒠㒥㒠㒡㒡㒟㒠㒙㒟㒥㒣㒜㒟㒝㒣㒛㒞㒥㒞㒡㒞㒝㒞㒙㒝㒥㒝㒡㒠㒤㒝㒙㒠㒠㒜㒡㒜㒟㒜㒙㒜㒥㒛㒡㒛㒝㒜㒢㒚㒥㒞㒤㒚㒝㒝㒠㒙㒥㒚㒣㒙㒝㒙㒙㒜㒜㒘㒡㒠㒜㒘㒙㒗㒥㒗㒡㒙㒝㒗㒙㒦㒥㒚㒘㒦㒝㒙㒠㒥㒥㒞㒙㒥㒝㒗㒙㒤㒥㒤㒡㒗㒤㒤㒙㒗㒜㒣㒡㒗㒙㒣㒙㒣㒥㒢㒡㒢㒝㒣㒢㒡㒥㒚㒙㒡㒝㒤㒠㒠㒥㒣㒡㒠㒝㒠㒙㒡㒞㒟㒡㒠㒡㒟㒙㒡㒞㒞㒡㒟㒟㒞㒙㒝㒥㒡㒘㒝㒝㒠㒚㒜㒥㒜㒡㒜㒝㒞㒙㒛㒥㒛㒡㒞㒤㒛㒙㒞㒜㒚㒡㒚㒝㒚㒚㒛㒗㒙㒡㒙㒝㒜㒡㒘㒥㒦㒦㒘㒝㒘㒙㒗㒥㒘㒣㒗㒝㒗㒙㒚㒞㒦㒡㒙㒜㒦㒙㒥㒥㒥㒡㒦㒟㒥㒙㒤㒥㒘㒛㒤㒝㒤㒡㒣㒥㒣㒡㒣㒝㒣㒙㒢㒥㒢㒡㒥㒤㒢㒙㒥㒟㒡㒡㒡㒟㒡㒙㒡㒥㒠㒡㒠㒝㒡㒢㒟㒥㒙㒝㒟㒝㒢㒠㒞㒥㒡㒡㒞㒝㒞㒙㒟㒞㒝㒡㒣㒚㒝㒙㒞㒟㒜㒡㒟㒝㒜㒙㒛㒥㒝㒚㒛㒝㒛㒥㒚㒥㒛㒚㒚㒞㒝㒙㒙㒥㒙㒡㒚㒦㒙㒙㒤㒛㒘㒡㒚㒗㒘㒙㒚㒥㒗㒡㒗㒝㒘㒣㒦㒥㒝㒥㒦㒝㒙㒤㒥㒥㒦㒡㒥㒝㒥㒙㒦㒟㒤㒡㒙㒟㒤㒙㒥㒗㒣㒡㒤㒟㒣㒙㒢㒥㒦㒘㒢㒝㒥㒚㒡㒥㒡㒡㒡㒝㒣㒙㒠㒥㒠㒡㒣㒤㒠㒙㒣㒜㒟㒡㒟㒝㒟㒚㒠㒗㒞㒡㒞㒝㒡㒡㒝㒥㒟㒙㒝㒝㒝㒙㒜㒥㒝㒣㒜㒝㒜㒙㒟㒞㒛㒡㒜㒥㒛㒙㒚㒥㒚㒡㒛㒟㒚㒙㒙㒥㒝㒛㒙㒝㒚㒡㒘㒥㒘㒡㒘㒝㒘㒙㒗㒥㒗㒡㒚㒤㒗㒙㒚㒟㒦㒡㒦㒟㒦㒙㒦㒥㒥㒡㒥㒝㒦㒣㒤㒥㒡㒥㒤㒝㒗㒠㒣㒥㒦㒡㒣㒝㒣㒙㒤㒟㒢㒡㒤㒛㒢㒙㒗㒣㒡㒡㒢㒟㒡㒙㒠㒥㒤㒘㒠㒝㒟㒗㒟㒥㒟㒡㒟㒝㒡㒙㒞㒥㒞㒡㒡㒤㒞㒙㒡㒜㒝㒡㒟㒣㒝㒙㒞㒗㒜㒡㒜㒝㒟㒡㒛㒥㒜㒤㒛㒝㒛㒙㒚㒥㒛㒣㒚㒝㒚㒙㒝㒞㒙㒡㒦㒘㒙㒙㒘㒥㒘㒡㒙㒟㒘㒙㒗㒥㒛㒛㒗㒝㒣㒣㒦㒥㒦㒡㒦㒝㒗㒛㒥㒥㒥㒡㒙㒘㒥㒙㒡㒠㒤㒡㒤㒝㒤㒙㒣㒥㒣㒡㒣㒝㒦㒠㒢㒥㒦㒜㒢㒝㒢㒛㒡㒥㒢㒡㒡㒝㒡㒙㒢㒟㒠㒡㒣㒛㒠㒙㒣㒜㒟㒡㒠㒟㒟㒙㒞㒥㒢㒘㒞㒝㒝㒗㒝㒥㒝㒡㒝㒝㒟㒙㒜㒥㒜㒡㒟㒤㒜㒙㒟㒜㒛㒡㒝㒣㒛㒙㒜㒗㒚㒡㒚㒝㒝㒡㒙㒥㒦㒜㒙㒝㒙㒙㒘㒥㒙㒣㒘㒝㒘㒙㒛㒞㒗㒡㒛㒟㒗㒙㒦㒥㒦㒡㒗㒟㒦㒙㒥㒥㒙㒛㒥㒝㒡㒤㒤㒥㒤㒡㒤㒝㒥㒛㒣㒥㒣㒡㒗㒘㒣㒙㒗㒗㒢㒡㒢㒝㒢㒙㒡㒥㒡㒡㒡㒝㒤㒠㒠㒥㒤㒜㒠㒝㒠㒛㒟㒥㒠㒡㒟㒝㒟㒙㒠㒟㒞㒡㒢㒠㒞㒙㒡㒜㒝㒡㒞㒟㒝㒙㒜㒥㒠㒘㒜㒝㒤㒘㒛㒥㒛㒡㒛㒝㒝㒙㒚㒥㒚㒡㒝㒤㒚㒙㒝㒜㒙㒡㒡㒥㒙㒙㒚㒥㒘㒡㒘㒝㒛㒠㒗㒥㒛㒘㒗㒝㒚㒥㒦㒥㒗㒡㒦㒝㒦㒙㒗㒟㒥㒡㒝㒥㒥㒙㒘㒜㒤㒡㒗㒝㒤㒙㒣㒥㒥㒛㒣㒝㒤㒝㒢㒥㒣㒚㒢㒝㒣㒛㒡㒥㒡㒡㒤㒤㒡㒙㒣㒦㒠㒡㒠㒝㒠㒙㒡㒥㒟㒡㒟㒝㒢㒠㒞㒥㒢㒘㒞㒝㒞㒙㒝㒦㒞㒣㒝㒝㒝㒙㒠㒝㒜㒡㒢㒜㒜㒙㒛㒥㒛㒡㒜㒟㒛㒙㒚㒥㒞㒚㒚㒝㒛㒝㒙㒦㒙㒡㒙㒝㒚㒛㒘㒥㒘㒡㒜㒗㒘㒙㒤㒠㒗㒡㒗㒝㒗㒙㒦㒥㒦㒡㒦㒝㒙㒠㒥㒥㒙㒛㒥㒝㒥㒛㒤㒥㒥㒡㒤㒝㒤㒙㒥㒟㒣㒡㒝㒙㒣㒙㒦㒜㒢㒡㒥㒝㒢㒙㒡㒥㒣㒛㒡㒝㒦㒦㒠㒥㒢㒛㒠㒝㒣㒙㒟㒥㒟㒡㒡㒗㒟㒙㒟㒡㒞㒡㒞㒦㒞㒚㒠㒥㒝㒡㒝㒝㒞㒣㒜㒥㒘㒗㒜㒝㒝㒣㒛㒥㒞㒡㒛㒝㒛㒙㒜㒠㒚㒡㒡㒡㒚㒙㒡㒝㒙㒡㒚㒝㒙㒙㒘㒥㒚㒜㒘㒝㒝㒛㒗㒥㒘㒣㒗㒝㒘㒛㒦㒥㒦㒡㒙㒤㒦㒙㒘㒦㒥㒡㒥㒝㒥㒙㒦㒥㒤㒡㒤㒝㒗㒠㒣㒥㒗㒘㒣㒝㒣㒙㒢㒦㒣㒣㒢㒝㒢㒙㒥㒝㒡㒡㒢㒥㒡㒙㒠㒥㒠㒡㒡㒟㒠㒙㒟㒥㒣㒚㒟㒝㒠㒡㒞㒥㒞㒡㒞㒝㒟㒛㒟㒥㒝㒡㒡㒗㒝㒙㒞㒝㒜㒡㒜㒝㒜㒙㒛㒥㒢㒤㒛㒝㒞㒠㒚㒥㒞㒛㒚㒝㒚㒛㒙㒥㒚㒡㒚㒢㒙㒙㒚㒠㒘㒡㒥㒡㒘㒙㒛㒜㒗㒡㒚㒝㒚㒙㒦㒥㒘㒜㒦㒝㒘㒗㒥㒥㒛㒟㒥㒝㒦㒛㒤㒥㒤㒡㒗㒤㒤㒙㒢㒣㒣㒡㒣㒝㒣㒙㒤㒥㒢㒡㒢㒝㒥㒠㒡㒥㒥㒘㒡㒝㒣㒟㒠㒥㒡㒣㒠㒝㒠㒙㒣㒝㒟㒡㒜㒙㒟㒙㒞㒥㒞㒡㒟㒟㒞㒙㒝㒥㒡㒚㒝㒝㒙㒤㒜㒥㒜㒡㒜㒝㒝㒛㒛㒥㒛㒡㒟㒗㒛㒙㒗㒟㒚㒡㒚㒝㒚㒙㒛㒗㒙㒡㒙㒝㒜㒤㒘㒥㒥㒜㒘㒝㒘㒙㒗㒥㒗㒡㒗㒝㒗㒙㒚㒜㒦㒡㒚㒘㒦㒙㒦㒗㒥㒡㒦㒝㒥㒙㒤㒥㒦㒜㒤㒝㒗㒗㒣㒥㒗㒘㒣㒝㒤㒛㒢㒥㒢㒡㒥㒤㒢㒙㒠㒣㒡㒡㒡㒝㒡㒙㒢㒥㒠㒡㒠㒝㒣㒠㒟㒥㒣㒘㒟㒝㒡㒟㒞㒥㒟㒣㒞㒝㒞㒙㒡㒝㒝㒡㒚㒘㒝㒙㒜㒥㒜㒡㒝㒟㒜㒙㒛㒥㒟㒚㒛㒝㒛㒝㒚㒥㒚㒡㒚㒝㒛㒛㒙㒥㒙㒡㒝㒗㒙㒙㒥㒠㒘㒡㒘㒝㒘㒙㒙㒗㒗㒡㒗㒝㒚㒤㒦㒥㒚㒣㒦㒝㒦㒙㒥㒥㒥㒡㒥㒝㒥㒙㒘㒜㒤㒡㒘㒘㒤㒙㒤㒗㒣㒡㒤㒝㒣㒙㒢㒥㒤㒜㒢㒝㒦㒜㒡㒥㒥㒘㒡㒝㒢㒛㒠㒥㒠㒡㒣㒤㒠㒙㒗㒤㒟㒡㒟㒝㒟㒙㒠㒥㒞㒡㒞㒝㒡㒠㒝㒥㒡㒘㒝㒝㒥㒡㒜㒥㒞㒡㒜㒝㒜㒙㒟㒜㒛㒡㒞㒤㒛㒙㒞㒡㒚㒡㒛㒝㒚㒙㒙㒥㒛㒜㒙㒝㒡㒡㒘㒥㒜㒘㒘㒝㒛㒙㒗㒥㒗㒡㒙㒘㒗㒙㒘㒙㒦㒡㒦㒣㒦㒙㒗㒗㒥㒡㒥㒝㒘㒠㒤㒥㒗㒢㒤㒝㒤㒙㒣㒥㒥㒡㒣㒝㒣㒙㒦㒜㒢㒡㒥㒤㒢㒙㒡㒥㒡㒢㒢㒟㒡㒙㒠㒥㒤㒙㒠㒝㒘㒤㒟㒥㒟㒡㒟㒝㒠㒛㒞㒥㒞㒡㒡㒦㒞㒙㒞㒢㒝㒢㒝㒝㒝㒙㒞㒗㒜㒡㒜㒝㒟㒣㒛㒥㒜㒞㒛㒞㒛㒙㒚㒥㒚㒡㒚㒝㒚㒙㒝㒜㒙㒡㒝㒗㒙㒙㒙㒗㒘㒡㒙㒝㒘㒙㒗㒥㒙㒜㒗㒝㒠㒥㒦㒥㒚㒘㒦㒝㒙㒙㒥㒥㒥㒡㒗㒘㒥㒙㒚㒢㒤㒡㒦㒗㒤㒙㒦㒥㒣㒡㒣㒝㒤㒤㒢㒥㒣㒝㒢㒝㒢㒢㒡㒦㒤㒡㒡㒝㒡㒙㒢㒠㒠㒡㒛㒣㒠㒙㒡㒟㒟㒡㒠㒝㒟㒙㒞㒥㒠㒞㒞㒝㒣㒛㒝㒥㒞㒣㒝㒝㒞㒛㒜㒥㒜㒡㒟㒤㒜㒙㒞㒦㒛㒡㒛㒝㒛㒙㒜㒥㒚㒡㒚㒝㒝㒠㒙㒥㒝㒘㒙㒝㒙㒙㒘㒦㒙㒣㒘㒝㒘㒙㒛㒝㒗㒡㒤㒘㒗㒙㒦㒥㒦㒡㒗㒟㒦㒙㒥㒥㒙㒚㒥㒝㒡㒤㒤㒥㒤㒡㒤㒝㒥㒛㒣㒥㒣㒡㒗㒗㒣㒙㒟㒠㒢㒡㒢㒝㒢㒙㒡㒥㒡㒡㒡㒝㒤㒠㒠㒥㒤㒛㒠㒝㒠㒛㒟㒥㒠㒡㒟㒝㒟㒙㒠㒢㒞㒡㒛㒡㒞㒙㒡㒜㒝㒡㒠㒝㒝㒙㒜㒥㒞㒞㒜㒝㒞㒗㒛㒥㒦㒞㒛㒝㒜㒛㒚㒥㒚㒡㒝㒤㒚㒙㒜㒦㒙㒡㒙㒝㒙㒙㒚㒥㒘㒡㒘㒝㒛㒠㒗㒥㒛㒘㒗㒝㒗㒙㒦㒦㒗㒣㒦㒝㒦㒙㒙㒝㒥㒡㒢㒤㒥㒙㒤㒥㒤㒡㒥㒟㒤㒙㒣㒥㒗㒚㒣㒝㒠㒠㒢㒥㒢㒡㒢㒝㒣㒛㒡㒥㒡㒡㒥㒗㒡㒙㒞㒜㒠㒡㒠㒝㒠㒙㒟㒥㒟㒡㒟㒝㒢㒠㒞㒥㒢㒛㒞㒝㒞㒛㒝㒥㒞㒡㒝㒝㒝㒙㒞㒢㒜㒡㒞㒘㒜㒚㒟㒜㒛㒡㒞㒝㒛㒙㒚㒥㒜㒞㒚㒝㒘㒡㒙㒥㒠㒠㒙㒝㒚㒛㒘㒥㒘㒡㒛㒤㒘㒙㒦㒣㒗㒡㒗㒝㒗㒙㒘㒥㒦㒡㒦㒝㒙㒠㒥㒥㒙㒘㒥㒝㒗㒟㒤㒥㒥㒣㒤㒝㒤㒙㒗㒝㒣㒡㒙㒝㒣㒙㒢㒥㒢㒡㒣㒟㒢㒙㒡㒥㒥㒚㒡㒝㒝㒤㒠㒥㒠㒡㒠㒝㒡㒛㒟㒥㒟㒡㒣㒗㒟㒙㒡㒟㒞㒡㒞㒝㒞㒙㒟㒗㒝㒡㒝㒝㒠㒤㒜㒥㒙㒜㒜㒝㒜㒙㒛㒥㒛㒡㒛㒝㒛㒙㒞㒜㒚㒡㒞㒘㒚㒙㒚㒗㒙㒡㒚㒝㒙㒙㒘㒥㒚㒞㒘㒝㒛㒗㒗㒥㒛㒘㒗㒝㒘㒛㒦㒥㒦㒡㒙㒤㒦㒙㒤㒣㒥㒡㒥㒝㒥㒙㒦㒥㒤㒡㒤㒝㒗㒠㒣㒥㒗㒘㒣㒝㒥㒟㒢㒥㒣㒣㒢㒝㒢㒙㒥㒝㒡㒡㒞㒘㒡㒙㒠㒥㒠㒡㒡㒟㒠㒙㒟㒥㒣㒚㒟㒝㒜㒠㒞㒥㒞㒡㒞㒝㒟㒛㒝㒥㒝㒡㒡㒗㒝㒙㒙㒠㒜㒡㒜㒝㒜㒙㒝㒗㒛㒡㒛㒝㒞㒤㒚㒥㒘㒘㒚㒝㒚㒙㒙㒥㒙㒡㒙㒝㒙㒙㒜㒜㒘㒡㒜㒘㒘㒙㒘㒗㒗㒡㒘㒝㒗㒙㒦㒥㒘㒞㒦㒝㒚㒜㒥㒥㒙㒘㒥㒝㒘㒙㒤㒥㒤㒡㒦㒛㒤㒙㒛㒙㒣㒡㒜㒣㒣㒙㒣㒥㒢㒡㒢㒝㒤㒗㒡㒥㒦㒣㒡㒝㒢㒦㒠㒥㒡㒣㒠㒝㒠㒙㒣㒜㒟㒡㒢㒞㒟㒙㒞㒥㒞㒡㒠㒝㒞㒙㒝㒥㒡㒘㒝㒝㒠㒠㒜㒥㒜㒡㒜㒞㒝㒛㒛㒥㒛㒡㒞㒥㒛㒙㒜㒝㒚㒡㒚㒝㒚㒙㒛㒗㒙㒡㒙㒝㒜㒢㒘㒥㒚㒙㒘㒝㒘㒙㒗㒥㒘㒣㒗㒝㒗㒙㒚㒟㒦㒡㒗㒥㒦㒙㒥㒥㒥㒡㒥㒝㒥㒙㒤㒥㒘㒘㒤㒝㒗㒣㒣㒥㒣㒣㒣㒝㒤㒙㒢㒥㒢㒡㒤㒛㒢㒙㒟㒙㒡㒡㒤㒤㒡㒙㒣㒥㒠㒡㒠㒝㒢㒗㒟㒥㒡㒟㒟㒝㒣㒥㒞㒥㒟㒣㒞㒝㒞㒙㒡㒜㒝㒡㒠㒞㒝㒙㒜㒥㒜㒡㒞㒝㒜㒙㒛㒥㒟㒘㒛㒝㒞㒠㒚㒥㒚㒡㒚㒞㒛㒛㒙㒥㒙㒡㒜㒥㒙㒙㒦㒜㒘㒡㒘㒝㒘㒙㒙㒗㒗㒡㒗㒝㒚㒢㒦㒥㒤㒘㒦㒝㒦㒙㒥㒥㒦㒣㒥㒝㒥㒙㒘㒟㒤㒡㒡㒤㒤㒙㒣㒥㒣㒡㒣㒝㒦㒜㒢㒥㒦㒘㒢㒝㒥㒣㒡㒥㒡㒣㒡㒝㒢㒙㒠㒥㒠㒡㒢㒛㒠㒙㒡㒠㒟㒢㒢㒤㒟㒙㒠㒗㒞㒡㒞㒝㒡㒠㒝㒥㒜㒟㒝㒝㒝㒙㒜㒥㒞㒡㒜㒝㒜㒙㒟㒜㒛㒡㒞㒤㒛㒙㒝㒛㒚㒡㒛㒟㒚㒙㒙㒥㒝㒙㒙㒝㒣㒛㒘㒥㒘㒡㒘㒝㒙㒛㒗㒥㒗㒡㒚㒦㒗㒙㒣㒠㒦㒡㒦㒝㒦㒙㒗㒗㒥㒡㒥㒝㒘㒣㒤㒥㒗㒜㒤㒝㒤㒙㒣㒥㒤㒣㒣㒝㒣㒙㒦㒠㒢㒡㒟㒘㒢㒙㒡㒥㒡㒡㒡㒝㒡㒙㒠㒥㒤㒘㒠㒝㒣㒤㒟㒥㒟㒣㒟㒝㒠㒙㒞㒥㒞㒡㒠㒛㒞㒙㒠㒣㒝㒡㒠㒤㒝㒙㒞㒗㒜㒡㒜㒝㒟㒠㒛㒥㒚㒟㒛㒝㒛㒙㒚㒥㒜㒡㒚㒝㒚㒙㒝㒜㒙㒡㒜㒤㒙㒙㒛㒛㒘㒡㒙㒟㒘㒙㒗㒥㒛㒙㒗㒝㒣㒤㒦㒥㒦㒡㒦㒝㒗㒛㒥㒥㒥㒡㒘㒦㒥㒙㒦㒚㒤㒢㒤㒝㒤㒙㒥㒗㒣㒡㒣㒝㒦㒣㒢㒥㒟㒜㒢㒝㒢㒙㒡㒥㒢㒣㒡㒝㒡㒙㒤㒠㒠㒡㒛㒤㒠㒙㒟㒥㒟㒡㒟㒝㒟㒙㒞㒥㒢㒘㒞㒝㒡㒤㒝㒥㒝㒣㒝㒝㒞㒙㒜㒥㒜㒡㒞㒛㒜㒙㒠㒘㒛㒡㒞㒤㒛㒙㒜㒗㒚㒡㒚㒝㒝㒠㒙㒥㒡㒠㒙㒝㒙㒙㒘㒥㒚㒡㒘㒝㒘㒙㒛㒜㒗㒡㒚㒤㒗㒙㒟㒝㒦㒡㒘㒝㒦㒙㒥㒥㒙㒘㒥㒝㒘㒠㒤㒥㒘㒠㒤㒝㒥㒙㒣㒥㒣㒡㒥㒛㒣㒙㒛㒝㒢㒡㒥㒤㒢㒙㒤㒥㒡㒡㒡㒝㒣㒗㒠㒥㒡㒥㒠㒝㒠㒣㒟㒦㒠㒣㒟㒝㒟㒙㒢㒜㒞㒡㒡㒞㒞㒙㒝㒥㒝㒡㒟㒝㒝㒙㒜㒥㒠㒘㒜㒝㒟㒠㒛㒥㒛㒡㒛㒞㒜㒛㒚㒥㒚㒡㒝㒥㒚㒙㒥㒙㒙㒡㒙㒝㒙㒙㒚㒗㒘㒡㒘㒝㒛㒢㒗㒥㒢㒥㒗㒝㒗㒙㒦㒥㒗㒣㒦㒝㒦㒙㒙㒟㒥㒡㒠㒡㒥㒙㒤㒥㒤㒡㒤㒝㒤㒙㒣㒥㒗㒘㒣㒝㒦㒣㒢㒥㒢㒣㒢㒝㒣㒙㒡㒥㒡㒡㒣㒛㒡㒙㒚㒡㒠㒡㒣㒤㒠㒙㒢㒥㒟㒡㒟㒝㒡㒗㒞㒥㒟㒝㒞㒝㒞㒢㒝㒦㒠㒡㒝㒝㒝㒙㒞㒣㒜㒡㒗㒣㒜㒙㒝㒟㒛㒡㒜㒟㒛㒙㒚㒥㒞㒘㒚㒝㒥㒗㒙㒥㒙㒡㒙㒝㒛㒙㒘㒥㒘㒡㒛㒤㒘㒙㒛㒜㒗㒡㒙㒣㒗㒙㒘㒗㒦㒡㒦㒝㒙㒡㒥㒥㒢㒜㒥㒝㒥㒙㒤㒥㒥㒣㒤㒝㒤㒙㒗㒞㒣㒡㒡㒡㒣㒙㒢㒥㒢㒡㒢㒝㒢㒙㒡㒥㒥㒘㒡㒝㒤㒢㒠㒥㒠㒣㒠㒝㒡㒙㒟㒥㒟㒡㒡㒜㒟㒙㒝㒤㒞㒡㒡㒤㒞㒙㒞㒥㒝㒡㒝㒝㒟㒘㒜㒥㒡㒣㒜㒝㒞㒗㒛㒥㒞㒡㒛㒝㒛㒙㒜㒥㒚㒡㒡㒡㒚㒙㒙㒛㒙㒡㒚㒝㒙㒙㒘㒥㒚㒡㒘㒝㒝㒛㒗㒥㒙㒞㒗㒝㒘㒛㒦㒥㒦㒡㒙㒤㒦㒙㒘㒦㒥㒡㒥㒝㒥㒙㒦㒥㒤㒡㒤㒝㒗㒠㒣㒥㒗㒘㒣㒝㒣㒙㒢㒦㒣㒣㒢㒝㒢㒙㒥㒝㒡㒡㒢㒥㒡㒙㒠㒥㒠㒡㒡㒟㒠㒙㒟㒥㒣㒚㒟㒝㒠㒡㒞㒥㒞㒡㒞㒝㒟㒛㒝㒥㒝㒡㒡㒗㒝㒙㒞㒝㒜㒡㒜㒝㒜㒙㒛㒥㒛㒡㒛㒝㒞㒠㒚㒥㒞㒛㒚㒝㒚㒛㒙㒥㒚㒡㒙㒝㒙㒙㒚㒥㒘㒡㒥㒡㒘㒙㒛㒜㒗㒡㒚㒝㒗㒙㒦㒥㒘㒡㒦㒝㒘㒗㒥㒥㒚㒝㒥㒝㒦㒛㒤㒥㒤㒡㒗㒤㒤㒙㒦㒦㒣㒡㒣㒝㒣㒙㒤㒥㒢㒡㒢㒝㒥㒠㒡㒥㒥㒘㒡㒝㒡㒙㒠㒦㒡㒣㒠㒝㒠㒙㒣㒝㒟㒡㒜㒤㒟㒙㒞㒥㒞㒡㒟㒟㒞㒙㒝㒥㒡㒚㒝㒝㒚㒠㒜㒥㒜㒡㒜㒝㒝㒛㒛㒥㒛㒡㒟㒗㒛㒙㒘㒜㒚㒡㒚㒝㒚㒙㒙㒥㒙㒡㒙㒝㒜㒠㒘㒥㒜㒛㒘㒝㒘㒛㒗㒥㒘㒡㒗㒝㒗㒙㒘㒥㒦㒡㒘㒘㒦㒚㒙㒜㒥㒡㒦㒟㒥㒙㒤㒥㒘㒘㒤㒝㒣㒗㒣㒥㒣㒡㒣㒝㒥㒙㒢㒥㒢㒡㒥㒤㒢㒙㒥㒜㒡㒡㒣㒣㒡㒙㒢㒗㒠㒡㒠㒝㒣㒡㒟㒥㒙㒣㒟㒝㒟㒙㒞㒥㒟㒣㒞㒝㒞㒙㒡㒞㒝㒡㒚㒘㒝㒙㒜㒥㒜㒡㒝㒟㒜㒙㒛㒥㒟㒛㒛㒝㒢㒣㒚㒥㒚㒡㒚㒝㒛㒛㒙㒥㒙㒡㒝㒘㒙㒙㒥㒠㒘㒡㒘㒝㒘㒙㒗㒥㒗㒡㒗㒝㒚㒠㒦㒥㒚㒜㒦㒝㒦㒛㒥㒥㒦㒡㒥㒝㒥㒙㒦㒥㒤㒡㒗㒛㒤㒙㒗㒜㒣㒡㒤㒟㒣㒙㒢㒥㒦㒘㒢㒝㒡㒗㒡㒥㒡㒡㒡㒝㒣㒙㒠㒥㒠㒡㒣㒤㒠㒙㒣㒜㒟㒡㒡㒣㒟㒙㒠㒗㒞㒡㒞㒝㒡㒡㒝㒥㒚㒜㒝㒝㒝㒙㒜㒥㒝㒣㒜㒝㒜㒙㒟㒞㒛㒡㒜㒢㒛㒚㒚㒥㒚㒡㒛㒟㒚㒙㒙㒥㒝㒛㒙㒝㒥㒤㒘㒥㒘㒡㒘㒝㒙㒛㒗㒥㒗㒡㒛㒘㒗㒙㒢㒜㒦㒡㒦㒝㒦㒙㒥㒥㒥㒡㒥㒝㒘㒠㒤㒥㒘㒜㒤㒝㒤㒛㒣㒥㒤㒡㒣㒝㒣㒙㒤㒥㒢㒡㒦㒠㒢㒙㒥㒜㒡㒡㒤㒝㒡㒙㒠㒥㒢㒡㒠㒝㒗㒛㒟㒥㒟㒘㒟㒝㒠㒛㒞㒥㒞㒡㒡㒤㒞㒙㒥㒤㒝㒡㒝㒝㒝㒙㒞㒥㒜㒡㒜㒝㒟㒠㒛㒥㒟㒘㒛㒝㒣㒡㒚㒥㒜㒡㒚㒝㒚㒙㒝㒜㒙㒡㒜㒤㒙㒙㒜㒤㒘㒡㒙㒝㒘㒙㒗㒥㒙㒡㒗㒝㒟㒡㒦㒥㒚㒘㒦㒝㒙㒙㒥㒥㒥㒡㒗㒝㒥㒙㒦㒙㒤㒡㒚㒘㒤㒙㒥㒗㒣㒡㒣㒝㒦㒠㒢㒥㒥㒢㒢㒝㒢㒙㒡㒥㒣㒡㒡㒝㒡㒙㒤㒜㒠㒡㒣㒤㒠㒙㒟㒥㒟㒢㒠㒟㒡㒙㒞㒥㒢㒙㒞㒝㒙㒝㒝㒥㒝㒡㒝㒝㒞㒛㒞㒥㒜㒡㒟㒦㒜㒙㒗㒙㒛㒡㒛㒝㒛㒙㒜㒗㒠㒣㒚㒝㒝㒣㒙㒥㒤㒥㒙㒝㒙㒙㒘㒥㒘㒡㒘㒝㒘㒙㒛㒜㒗㒡㒛㒗㒗㒙㒗㒗㒦㒡㒗㒝㒦㒙㒥㒥㒗㒡㒥㒝㒞㒥㒤㒥㒘㒘㒤㒝㒗㒙㒣㒥㒣㒡㒥㒝㒣㒙㒣㒡㒢㒡㒢㒦㒢㒚㒤㒥㒡㒡㒡㒝㒣㒙㒠㒥㒜㒗㒠㒝㒡㒣㒟㒥㒠㒣㒟㒝㒟㒙㒢㒜㒞㒡㒙㒛㒞㒙㒝㒥㒝㒡㒟㒝㒝㒙㒜㒥㒠㒘㒜㒝㒟㒠㒛㒥㒞㒗㒛㒝㒜㒛㒚㒥㒚㒡㒝㒥㒚㒙㒦㒠㒙㒡㒙㒝㒙㒙㒚㒗㒘㒡㒘㒝㒛㒢㒗㒥㒥㒥㒗㒝㒗㒙㒦㒥㒦㒡㒦㒝㒦㒙㒙㒜㒥㒡㒘㒦㒥㒙㒥㒗㒤㒡㒥㒝㒤㒙㒣㒥㒥㒢㒣㒝㒢㒘㒢㒥㒦㒘㒢㒝㒣㒙㒡㒥㒡㒡㒣㒞㒡㒙㒦㒗㒠㒡㒢㒝㒠㒙㒢㒥㒟㒡㒟㒝㒡㒛㒞㒥㒥㒥㒞㒝㒠㒠㒝㒥㒞㒡㒝㒝㒝㒙㒟㒗㒜㒡㒡㒟㒜㒙㒝㒢㒛㒡㒜㒟㒛㒙㒚㒥㒞㒘㒚㒝㒝㒚㒙㒥㒙㒡㒙㒝㒛㒙㒘㒥㒘㒡㒛㒤㒘㒙㒛㒜㒗㒡㒗㒝㒗㒚㒘㒗㒦㒡㒦㒝㒙㒡㒥㒥㒗㒙㒥㒝㒥㒙㒤㒥㒥㒣㒤㒝㒤㒙㒗㒞㒣㒡㒤㒥㒣㒙㒢㒥㒢㒡㒣㒟㒢㒙㒡㒥㒥㒛㒡㒝㒢㒡㒠㒥㒠㒡㒠㒝㒠㒙㒟㒥㒟㒡㒢㒤㒟㒙㒢㒟㒞㒡㒞㒟㒞㒙㒞㒥㒝㒡㒝㒝㒟㒛㒜㒥㒙㒥㒜㒝㒟㒠㒛㒥㒞㒡㒛㒝㒛㒙㒝㒗㒚㒡㒜㒛㒚㒙㒞㒡㒙㒡㒚㒟㒙㒙㒘㒥㒜㒘㒘㒝㒛㒚㒗㒥㒗㒡㒗㒝㒙㒙㒦㒥㒦㒡㒙㒤㒦㒙㒙㒜㒥㒡㒥㒝㒥㒚㒦㒗㒤㒡㒤㒝㒗㒡㒣㒥㒡㒘㒣㒝㒣㒙㒢㒥㒣㒣㒢㒝㒢㒙㒥㒞㒡㒡㒞㒤㒡㒙㒠㒥㒠㒡㒡㒟㒠㒙㒟㒥㒣㒛㒟㒝㒜㒠㒞㒥㒞㒡㒞㒝㒞㒙㒝㒥㒝㒡㒠㒤㒝㒙㒠㒟㒜㒡㒜㒟㒜㒙㒜㒥㒛㒡㒛㒝㒝㒛㒚㒥㒜㒜㒚㒞㒝㒠㒙㒥㒚㒣㒙㒝㒙㒙㒜㒜㒘㒡㒗㒛㒘㒙㒗㒥㒗㒡㒙㒝㒗㒙㒦㒥㒚㒘㒦㒝㒙㒠㒥㒥㒘㒗㒥㒝㒦㒛㒤㒥㒤㒡㒗㒥㒤㒙㒞㒗㒣㒡㒣㒝㒣㒙㒤㒗㒢㒡㒢㒝㒥㒢㒡㒥㒞㒜㒡㒝㒡㒙㒠㒥㒡㒣㒠㒝㒠㒙㒣㒟㒟㒡㒗㒗㒟㒙㒞㒥㒞㒡㒟㒟㒞㒙㒝㒥㒡㒜㒝㒝㒙㒤㒜㒥㒜㒡㒜㒝㒜㒙㒛㒥㒛㒡㒞㒤㒛㒙㒞㒠㒚㒡㒚㒟㒚㒙㒚㒥㒙㒡㒙㒝㒛㒛㒘㒥㒛㒟㒘㒝㒛㒠㒗㒥㒘㒣㒗㒝㒗㒙㒚㒜㒦㒡㒥㒛㒦㒙㒥㒥㒥㒡㒗㒝㒥㒙㒤㒥㒘㒘㒤㒝㒗㒠㒣㒥㒦㒗㒣㒝㒤㒛㒢㒥㒢㒡㒥㒥㒢㒙㒞㒠㒡㒡㒡㒝㒡㒙㒢㒗㒠㒡㒠㒝㒣㒢㒟㒥㒠㒦㒟㒞㒟㒙㒞㒥㒟㒣㒞㒝㒞㒙㒡㒟㒝㒡㒚㒘㒝㒙㒜㒥㒜㒡㒝㒟㒜㒙㒛㒥㒟㒜㒛㒝㒦㒠㒚㒥㒚㒡㒚㒝㒚㒙㒙㒥㒙㒡㒜㒤㒙㒙㒜㒠㒘㒡㒘㒟㒘㒙㒘㒥㒗㒡㒗㒝㒙㒛㒦㒥㒚㒤㒦㒝㒙㒠㒥㒥㒦㒣㒥㒝㒥㒙㒘㒜㒤㒡㒜㒜㒤㒙㒣㒥㒣㒡㒥㒝㒣㒙㒢㒥㒦㒘㒢㒝㒥㒠㒡㒥㒚㒙㒡㒝㒣㒙㒠㒥㒠㒡㒣㒤㒠㒙㒣㒜㒟㒡㒣㒜㒟㒙㒟㒥㒞㒡㒞㒝㒠㒛㒝㒥㒦㒙㒝㒝㒠㒠㒜㒥㒟㒡㒜㒝㒜㒙㒞㒗㒛㒡㒜㒡㒛㒙㒠㒠㒚㒡㒛㒟㒚㒙㒙㒥㒝㒘㒙㒝㒜㒚㒘㒥㒘㒡㒘㒝㒚㒙㒗㒥㒗㒡㒚㒤㒗㒙㒚㒜㒦㒡㒦㒝㒦㒚㒗㒗㒥㒡㒥㒝㒘㒡㒤㒥㒟㒥㒤㒝㒤㒙㒣㒥㒤㒣㒣㒝㒣㒙㒦㒞㒢㒡㒝㒡㒢㒙㒡㒥㒡㒡㒢㒟㒡㒙㒠㒥㒤㒛㒠㒝㒛㒝㒟㒥㒟㒡㒟㒝㒟㒙㒞㒥㒞㒡㒡㒤㒞㒙㒡㒟㒝㒡㒝㒟㒝㒙㒝㒥㒜㒡㒜㒝㒞㒛㒛㒥㒥㒝㒛㒝㒞㒠㒚㒥㒝㒡㒚㒝㒚㒙㒜㒗㒙㒡㒚㒙㒙㒙㒙㒞㒘㒢㒛㒝㒘㒙㒗㒥㒙㒣㒗㒝㒢㒟㒦㒥㒘㒛㒦㒝㒗㒛㒥㒥㒥㒡㒘㒤㒥㒙㒟㒣㒤㒡㒤㒝㒤㒙㒥㒥㒣㒡㒣㒝㒦㒠㒢㒥㒦㒘㒢㒝㒤㒟㒡㒥㒢㒣㒡㒝㒡㒙㒤㒝㒠㒡㒝㒘㒠㒙㒟㒥㒟㒡㒠㒟㒟㒙㒞㒥㒢㒚㒞㒝㒜㒝㒝㒥㒝㒡㒝㒝㒝㒙㒜㒥㒜㒡㒟㒤㒜㒙㒟㒞㒛㒡㒛㒟㒛㒙㒛㒥㒚㒡㒚㒝㒜㒜㒙㒥㒘㒠㒙㒝㒜㒠㒘㒥㒙㒡㒘㒝㒘㒙㒚㒘㒗㒡㒜㒟㒗㒙㒙㒗㒦㒡㒙㒝㒦㒙㒥㒥㒗㒥㒥㒝㒜㒝㒤㒥㒝㒝㒤㒝㒥㒙㒣㒥㒣㒡㒥㒡㒣㒙㒘㒗㒢㒡㒤㒚㒢㒙㒣㒗㒡㒡㒡㒝㒤㒠㒠㒥㒣㒢㒠㒝㒠㒙㒟㒥㒡㒡㒟㒝㒟㒙㒢㒜㒞㒡㒡㒤㒞㒙㒝㒥㒝㒢㒞㒟㒝㒙㒜㒥㒠㒙㒜㒝㒝㒡㒛㒥㒛㒡㒛㒝㒜㒛㒚㒥㒚㒡㒝㒦㒚㒙㒛㒝㒙㒡㒙㒝㒙㒙㒚㒗㒘㒡㒘㒝㒛㒣㒗㒥㒙㒙㒗㒝㒗㒙㒦㒥㒦㒡㒦㒝㒦㒙㒙㒜㒥㒡㒙㒗㒥㒙㒥㒗㒤㒡㒥㒝㒤㒙㒣㒥㒥㒥㒣㒝㒠㒝㒢㒥㒦㒘㒢㒝㒥㒙㒡㒥㒡㒡㒣㒡㒡㒙㒢㒣㒠㒡㒥㒙㒠㒙㒡㒗㒟㒡㒟㒝㒢㒠㒞㒥㒡㒢㒞㒝㒞㒙㒝㒥㒟㒡㒝㒝㒝㒙㒠㒜㒜㒡㒟㒤㒜㒙㒛㒥㒛㒢㒜㒟㒛㒙㒚㒥㒞㒙㒚㒝㒗㒠㒙㒥㒙㒡㒙㒝㒚㒛㒘㒥㒘㒡㒛㒦㒘㒙㒥㒜㒗㒡㒗㒝㒗㒙㒘㒗㒘㒡㒦㒝㒙㒣㒥㒥㒣㒘㒥㒝㒥㒙㒤㒥㒤㒡㒗㒘㒤㒙㒗㒜㒣㒡㒗㒗㒣㒙㒣㒗㒢㒡㒣㒝㒢㒙㒡㒥㒣㒥㒡㒝㒢㒤㒠㒦㒤㒘㒠㒝㒡㒛㒟㒥㒟㒡㒢㒤㒟㒙㒝㒣㒞㒡㒞㒝㒞㒙㒟㒥㒝㒡㒝㒝㒠㒠㒜㒥㒠㒘㒜㒝㒞㒟㒛㒥㒜㒣㒛㒝㒛㒙㒞㒝㒚㒡㒣㒥㒚㒙㒙㒥㒙㒡㒚㒟㒙㒙㒘㒥㒜㒚㒘㒝㒤㒤㒗㒥㒗㒡㒗㒝㒘㒛㒦㒥㒦㒡㒚㒗㒦㒙㒡㒦㒥㒡㒥㒝㒥㒙㒦㒗㒤㒡㒤㒝㒗㒤㒣㒥㒠㒜㒣㒝㒣㒙㒢㒥㒢㒡㒢㒝㒢㒙㒥㒜㒡㒡㒥㒘㒡㒙㒡㒗㒠㒡㒡㒝㒠㒙㒟㒥㒡㒥㒟㒝㒢㒗㒞㒥㒢㒘㒞㒝㒟㒛㒝㒥㒝㒡㒠㒤㒝㒙㒛㒣㒜㒡㒜㒝㒜㒙㒝㒥㒛㒡㒛㒝㒞㒠㒚㒥㒞㒘㒚㒝㒜㒟㒙㒥㒚㒣㒙㒝㒙㒙㒜㒝㒘㒡㒥㒘㒘㒙㒗㒥㒗㒡㒘㒟㒗㒙㒦㒥㒚㒚㒦㒝㒗㒞㒥㒦㒥㒡㒥㒝㒦㒛㒤㒥㒤㒡㒘㒗㒤㒙㒠㒠㒣㒡㒣㒝㒣㒙㒤㒗㒢㒡㒢㒝㒥㒤㒡㒥㒝㒘㒡㒝㒡㒙㒠㒥㒠㒡㒠㒝㒠㒙㒣㒜㒟㒡㒣㒘㒟㒙㒟㒗㒞㒡㒟㒝㒞㒙㒝㒥㒟㒥㒝㒝㒡㒜㒜㒥㒠㒘㒜㒝㒝㒛㒛㒥㒛㒡㒞㒤㒛㒙㒢㒤㒚㒡㒚㒝㒚㒙㒛㒥㒙㒡㒙㒝㒜㒠㒘㒥㒜㒘㒘㒝㒠㒡㒗㒥㒙㒡㒗㒝㒗㒙㒚㒜㒦㒡㒙㒤㒦㒙㒙㒤㒥㒡㒦㒝㒥㒙㒤㒥㒦㒥㒤㒝㒜㒡㒣㒥㒗㒘㒣㒝㒦㒙㒢㒥㒢㒡㒤㒡㒢㒙㒣㒙㒡㒡㒛㒜㒡㒙㒢㒗㒠㒡㒠㒝㒣㒠㒟㒥㒢㒢㒟㒝㒟㒙㒞㒥㒠㒡㒞㒝㒞㒙㒡㒜㒝㒡㒠㒤㒝㒙㒜㒥㒜㒢㒝㒟㒜㒙㒛㒥㒟㒙㒛㒝㒦㒝㒚㒥㒚㒡㒚㒝㒛㒛㒙㒥㒙㒡㒜㒦㒙㒙㒤㒙㒘㒡㒘㒝㒘㒙㒙㒗㒗㒡㒗㒝㒚㒣㒦㒥㒡㒥㒦㒝㒦㒙㒥㒥㒥㒡㒥㒝㒥㒙㒘㒜㒤㒡㒘㒗㒤㒙㒤㒗㒣㒡㒤㒝㒣㒙㒢㒥㒤㒥㒢㒝㒛㒥㒡㒥㒥㒘㒡㒝㒤㒙㒠㒥㒠㒡㒢㒡㒠㒙㒠㒡㒟㒡㒟㒦㒟㒚㒡㒥㒞㒡㒞㒝㒠㒝㒝㒥㒙㒗㒝㒝㒞㒣㒜㒥㒝㒣㒜㒝㒜㒙㒟㒜㒛㒡㒦㒛㒛㒙㒚㒥㒚㒡㒜㒝㒚㒙㒙㒥㒝㒘㒙㒝㒜㒠㒘㒥㒛㒗㒘㒝㒙㒛㒗㒥㒗㒡㒚㒥㒗㒙㒣㒠㒦㒡㒦㒝㒦㒙㒗㒗㒥㒡㒥㒝㒘㒢㒤㒥㒢㒥㒤㒝㒤㒙㒣㒥㒣㒡㒣㒝㒣㒙㒦㒜㒢㒡㒥㒦㒢㒙㒢㒗㒡㒡㒢㒝㒡㒙㒠㒥㒢㒦㒠㒝㒟㒘㒟㒥㒣㒘㒟㒝㒠㒙㒞㒥㒞㒡㒠㒢㒞㒙㒣㒗㒝㒡㒟㒡㒝㒙㒟㒥㒜㒡㒜㒝㒞㒟㒛㒥㒢㒥㒛㒝㒜㒛㒚㒦㒛㒡㒚㒝㒚㒙㒜㒛㒙㒡㒞㒟㒙㒙㒚㒢㒘㒡㒙㒟㒘㒙㒗㒥㒛㒘㒗㒝㒚㒚㒦㒥㒦㒡㒦㒝㒘㒙㒥㒥㒥㒡㒘㒤㒥㒙㒘㒜㒤㒡㒤㒝㒤㒚㒥㒗㒣㒡㒣㒝㒦㒡㒢㒥㒤㒙㒢㒝㒢㒙㒡㒥㒢㒣㒡㒝㒡㒙㒤㒞㒠㒡㒡㒥㒠㒙㒟㒥㒟㒡㒠㒟㒟㒙㒞㒥㒢㒛㒞㒝㒟㒡㒝㒥㒝㒡㒝㒝㒝㒙㒜㒥㒜㒡㒟㒤㒜㒙㒟㒟㒛㒡㒛㒟㒛㒙㒛㒥㒚㒡㒚㒝㒜㒟㒙㒥㒦㒥㒙㒝㒜㒠㒘㒥㒛㒡㒘㒝㒘㒙㒚㒛㒗㒡㒙㒛㒗㒙㒛㒡㒦㒡㒗㒟㒦㒙㒥㒥㒙㒘㒥㒝㒘㒚㒤㒥㒤㒡㒤㒝㒦㒙㒣㒥㒣㒡㒦㒤㒣㒙㒦㒜㒢㒡㒢㒝㒢㒚㒣㒗㒡㒡㒡㒝㒤㒡㒠㒥㒞㒘㒠㒝㒠㒙㒟㒥㒠㒣㒟㒝㒟㒙㒢㒞㒞㒡㒛㒤㒞㒙㒝㒥㒝㒡㒞㒟㒝㒙㒜㒥㒠㒛㒜㒝㒙㒠㒛㒥㒛㒡㒛㒝㒛㒙㒚㒥㒚㒡㒝㒤㒚㒙㒝㒟㒙㒡㒙㒟㒙㒙㒙㒥㒘㒡㒘㒝㒚㒟㒗㒥㒙㒜㒗㒞㒚㒠㒦㒥㒗㒣㒦㒝㒦㒙㒙㒜㒥㒡㒤㒛㒥㒙㒤㒥㒤㒡㒦㒝㒤㒙㒣㒥㒗㒘㒣㒝㒦㒠㒢㒥㒥㒗㒢㒝㒣㒛㒡㒥㒡㒡㒤㒥㒡㒙㒚㒝㒠㒡㒠㒝㒠㒙㒡㒗㒟㒡㒟㒝㒢㒢㒞㒥㒛㒜㒞㒝㒞㒙㒝㒥㒞㒣㒝㒝㒝㒙㒠㒟㒜㒡㒢㒡㒜㒙㒛㒥㒛㒡㒜㒟㒛㒙㒚㒥㒞㒜㒚㒝㒦㒤㒙㒥㒙㒡㒙㒝㒙㒙㒘㒥㒘㒡㒛㒤㒘㒙㒛㒠㒗㒡㒗㒟㒗㒙㒗㒥㒦㒡㒦㒝㒘㒟㒥㒥㒘㒟㒥㒝㒘㒠㒤㒥㒥㒣㒤㒝㒤㒙㒗㒜㒣㒡㒢㒛㒣㒙㒢㒥㒢㒡㒤㒝㒢㒙㒡㒥㒥㒘㒡㒝㒤㒠㒠㒥㒣㒗㒠㒝㒡㒛㒟㒥㒟㒡㒢㒥㒟㒙㒛㒠㒞㒡㒞㒝㒞㒙㒟㒗㒝㒡㒝㒝㒠㒢㒜㒥㒝㒦㒜㒞㒜㒙㒛㒥㒜㒣㒛㒝㒛㒙㒞㒟㒚㒡㒗㒘㒚㒙㒙㒥㒙㒡㒚㒟㒙㒙㒘㒥㒜㒜㒘㒝㒣㒠㒗㒥㒗㒡㒗㒝㒗㒙㒦㒥㒦㒡㒙㒤㒦㒙㒙㒠㒥㒡㒥㒟㒥㒙㒥㒥㒤㒡㒤㒝㒦㒟㒣㒥㒗㒤㒣㒝㒦㒠㒢㒥㒣㒣㒢㒝㒢㒙㒥㒜㒡㒡㒙㒜㒡㒙㒠㒥㒠㒡㒢㒝㒠㒙㒟㒥㒣㒘㒟㒝㒢㒠㒞㒥㒗㒙㒞㒝㒠㒙㒝㒥㒝㒡㒠㒤㒝㒙㒠㒜㒜㒡㒠㒜㒜㒙㒜㒥㒛㒡㒛㒝㒝㒟㒚㒥㒣㒙㒚㒝㒝㒠㒙㒥㒜㒡㒙㒝㒙㒙㒛㒛㒘㒡㒙㒡㒘㒙㒣㒞㒗㒡㒘㒟㒗㒙㒦㒥㒚㒘㒦㒝㒙㒚㒥㒥㒥㒡㒥㒝㒗㒙㒤㒥㒤㒡㒗㒤㒤㒙㒗㒜㒣㒡㒣㒝㒣㒚㒤㒗㒢㒡㒢㒝㒥㒡㒡㒥㒜㒥㒡㒝㒡㒙㒠㒥㒡㒣㒢㒝㒠㒙㒣㒞㒟㒡㒚㒡㒟㒙㒞㒥㒞㒡㒟㒟㒤㒛㒝㒥㒡㒛㒝㒝㒘㒝㒜㒥㒜㒡㒜㒝㒜㒙㒛㒥㒛㒡㒞㒤㒛㒙㒞㒟㒚㒡㒚㒟㒚㒙㒚㒥㒙㒡㒙㒝㒛㒟㒘㒥㒢㒝㒘㒝㒛㒠㒗㒥㒚㒡㒗㒝㒗㒙㒙㒛㒦㒡㒗㒙㒦㒙㒦㒞㒥㒢㒘㒝㒥㒙㒤㒥㒗㒗㒤㒝㒟㒟㒣㒥㒥㒛㒣㒝㒤㒛㒢㒥㒢㒡㒥㒤㒢㒙㒜㒣㒡㒡㒡㒝㒡㒙㒢㒥㒠㒡㒠㒝㒣㒠㒟㒥㒣㒘㒟㒝㒡㒟㒞㒥㒟㒣㒞㒝㒞㒙㒡㒝㒝㒡㒚㒘㒝㒙㒜㒥㒜㒡㒝㒟㒜㒙㒛㒥㒟㒚㒛㒝㒙㒝㒚㒥㒚㒡㒚㒝㒚㒙㒙㒥㒙㒡㒜㒤㒙㒙㒜㒞㒘㒡㒘㒟㒘㒙㒘㒥㒗㒡㒗㒝㒙㒠㒦㒥㒥㒠㒦㒝㒙㒠㒥㒥㒦㒡㒥㒝㒥㒙㒗㒜㒤㒡㒙㒟㒤㒙㒦㒛㒣㒡㒦㒝㒣㒙㒢㒥㒥㒙㒢㒝㒙㒝㒡㒥㒦㒥㒡㒝㒢㒙㒠㒥㒠㒡㒢㒥㒠㒙㒥㒗㒟㒡㒡㒚㒟㒙㒠㒗㒞㒡㒞㒝㒡㒠㒝㒥㒠㒢㒝㒝㒝㒙㒜㒥㒞㒡㒜㒝㒜㒙㒟㒜㒛㒡㒞㒤㒛㒙㒚㒥㒚㒢㒛㒟㒚㒙㒙㒥㒝㒙㒙㒝㒚㒡㒘㒥㒘㒡㒘㒝㒙㒛㒗㒥㒗㒡㒚㒦㒗㒙㒘㒝㒦㒡㒦㒝㒦㒙㒗㒗㒥㒡㒥㒝㒘㒣㒤㒥㒦㒙㒤㒝㒤㒙㒣㒥㒣㒡㒣㒝㒣㒙㒦㒜㒢㒡㒦㒗㒢㒙㒢㒗㒡㒡㒢㒝㒡㒙㒠㒥㒣㒙㒠㒝㒝㒝㒟㒥㒣㒘㒟㒝㒢㒙㒞㒥㒞㒡㒠㒥㒞㒙㒟㒣㒝㒡㒢㒙㒝㒙㒞㒗㒜㒡㒜㒝㒟㒠㒛㒥㒞㒢㒛㒝㒛㒙㒚㒥㒜㒡㒚㒝㒚㒙㒝㒜㒙㒡㒜㒤㒙㒙㒘㒥㒘㒢㒙㒟㒘㒙㒗㒥㒛㒙㒗㒝㒤㒠㒦㒥㒦㒡㒦㒝㒗㒛㒥㒥㒥㒡㒘㒦㒥㒙㒢㒜㒤㒡㒤㒝㒤㒙㒥㒗㒣㒡㒣㒝㒦㒣㒢㒥㒠㒘㒢㒝㒢㒙㒡㒥㒡㒡㒡㒝㒡㒙㒤㒜㒠㒡㒤㒗㒠㒙㒠㒗㒟㒡㒠㒝㒟㒙㒞㒥㒡㒙㒞㒝㒟㒤㒝㒦㒡㒘㒝㒝㒞㒛㒜㒥㒜㒡㒟㒤㒜㒙㒚㒣㒛㒡㒛㒝㒛㒙㒜㒥㒚㒡㒚㒝㒝㒠㒙㒥㒝㒘㒙㒝㒛㒟㒘㒥㒙㒣㒘㒝㒘㒙㒛㒝㒗㒡㒝㒤㒗㒙㒦㒥㒦㒡㒗㒟㒦㒙㒥㒥㒙㒚㒥㒝㒡㒤㒤㒥㒤㒡㒤㒝㒥㒛㒣㒥㒣㒡㒗㒗㒣㒙㒛㒣㒢㒡㒢㒝㒢㒙㒣㒗㒡㒡㒡㒝㒤㒤㒠㒥㒝㒜㒠㒝㒠㒙㒟㒥㒟㒡㒟㒝㒟㒙㒢㒜㒞㒡㒢㒘㒞㒙㒞㒗㒝㒡㒞㒝㒝㒙㒜㒥㒟㒙㒜㒝㒟㒗㒛㒥㒟㒘㒛㒝㒜㒛㒚㒥㒚㒡㒝㒤㒚㒙㒘㒣㒙㒡㒙㒝㒙㒙㒚㒥㒘㒡㒘㒝㒛㒠㒗㒥㒛㒘㒗㒝㒙㒟㒦㒥㒗㒣㒦㒝㒦㒙㒙㒝㒥㒡㒢㒘㒥㒙㒤㒥㒤㒡㒥㒟㒤㒙㒣㒥㒗㒚㒣㒝㒤㒞㒢㒦㒢㒡㒢㒝㒣㒛㒡㒥㒡㒡㒥㒗㒡㒙㒝㒠㒠㒡㒠㒝㒠㒙㒡㒗㒟㒡㒟㒝㒢㒤㒞㒥㒚㒘㒞㒝㒞㒙㒝㒥㒝㒡㒝㒝㒝㒙㒠㒜㒜㒡㒠㒘㒜㒙㒜㒗㒛㒡㒜㒝㒛㒙㒚㒥㒝㒙㒚㒝㒞㒜㒙㒥㒝㒘㒙㒝㒚㒛㒘㒥㒘㒡㒛㒤㒘㒙㒟㒤㒗㒡㒗㒝㒗㒙㒘㒥㒦㒡㒦㒝㒙㒠㒥㒥㒙㒘㒥㒝㒝㒡㒤㒥㒦㒡㒤㒝㒤㒙㒗㒜㒣㒡㒦㒤㒣㒙㒦㒤㒢㒡㒣㒝㒢㒙㒡㒥㒤㒙㒡㒝㒙㒡㒠㒥㒤㒘㒠㒝㒣㒙㒟㒥㒟㒡㒡㒥㒟㒙㒠㒙㒞㒡㒤㒢㒞㒙㒟㒗㒝㒡㒝㒝㒠㒠㒜㒥㒟㒢㒜㒝㒜㒙㒛㒥㒝㒡㒛㒝㒛㒙㒞㒜㒚㒡㒝㒤㒚㒙㒙㒥㒙㒢㒚㒟㒙㒙㒘㒥㒜㒙㒘㒝㒣㒝㒗㒥㒗㒡㒗㒝㒘㒛㒦㒥㒦㒡㒙㒦㒦㒙㒡㒙㒥㒡㒥㒝㒥㒙㒦㒗㒤㒡㒤㒝㒗㒣㒣㒥㒞㒥㒣㒝㒣㒙㒢㒥㒢㒡㒢㒝㒢㒙㒥㒜㒡㒡㒥㒗㒡㒙㒡㒗㒠㒡㒡㒝㒠㒙㒟㒥㒢㒙㒟㒝㒘㒥㒞㒥㒢㒘㒞㒝㒡㒙㒝㒥㒝㒡㒟㒥㒝㒙㒝㒡㒜㒡㒜㒦㒜㒚㒞㒥㒛㒡㒛㒝㒝㒡㒚㒥㒦㒗㒚㒝㒛㒣㒙㒥㒚㒣㒙㒝㒙㒙㒜㒜㒘㒡㒣㒛㒘㒙㒗㒥㒗㒡㒙㒝㒗㒙㒦㒥㒚㒘㒦㒝㒙㒠㒥㒥㒘㒗㒥㒝㒦㒛㒤㒥㒤㒡㒗㒥㒤㒙㒠㒠㒣㒡㒣㒝㒣㒙㒤㒗㒢㒡㒢㒝㒥㒢㒡㒥㒟㒥㒡㒝㒡㒙㒠㒥㒠㒡㒠㒝㒠㒙㒣㒜㒟㒡㒢㒦㒟㒙㒟㒗㒞㒡㒟㒝㒞㒙㒝㒥㒠㒚㒝㒝㒜㒘㒜㒥㒠㒘㒜㒝㒝㒙㒛㒥㒛㒡㒝㒦㒛㒙㒠㒗㒚㒡㒜㒥㒚㒙㒜㒥㒙㒡㒙㒝㒛㒣㒘㒥㒟㒥㒘㒝㒟㒞㒗㒥㒘㒡㒗㒝㒗㒙㒙㒟㒦㒡㒛㒟㒦㒙㒗㒢㒥㒡㒦㒟㒥㒙㒤㒥㒘㒘㒤㒝㒗㒚㒣㒥㒣㒡㒣㒝㒥㒙㒢㒥㒢㒡㒥㒤㒢㒙㒥㒜㒡㒡㒡㒝㒡㒚㒢㒗㒠㒡㒠㒝㒣㒡㒟㒥㒡㒙㒟㒝㒟㒙㒞㒥㒟㒣㒞㒝㒞㒙㒡㒞㒝㒡㒞㒥㒝㒙㒜㒥㒜㒡㒝㒟㒜㒙㒛㒥㒟㒛㒛㒝㒜㒡㒚㒥㒚㒡㒚㒝㒚㒙㒙㒥㒙㒡㒜㒤㒙㒙㒜㒟㒘㒡㒘㒟㒘㒙㒘㒥㒗㒡㒗㒝㒙㒣㒦㒥㒣㒥㒦㒝㒙㒠㒥㒥㒘㒡㒥㒝㒥㒙㒗㒟㒤㒡㒦㒛㒤㒙㒘㒡㒣㒡㒤㒟㒣㒙㒢㒥㒦㒘㒢㒝㒥㒚㒡㒥㒡㒡㒡㒝㒣㒙㒠㒥㒠㒡㒣㒤㒠㒙㒣㒜㒟㒡㒟㒝㒟㒚㒠㒗㒞㒡㒞㒝㒡㒡㒝㒥㒛㒘㒝㒝㒝㒙㒜㒥㒝㒣㒜㒝㒜㒙㒟㒞㒛㒡㒘㒤㒛㒙㒚㒥㒚㒡㒛㒟㒜㒙㒙㒥㒝㒛㒙㒝㒦㒠㒘㒥㒘㒡㒘㒝㒘㒙㒛㒘㒗㒡㒚㒤㒗㒙㒚㒟㒦㒡㒦㒟㒦㒙㒦㒥㒥㒡㒥㒝㒗㒣㒤㒥㒦㒜㒤㒞㒗㒠㒣㒥㒤㒣㒣㒝㒣㒙㒦㒜㒢㒡㒡㒛㒢㒙㒡㒥㒡㒡㒣㒝㒡㒙㒠㒥㒤㒘㒠㒝㒣㒠㒟㒥㒢㒗㒟㒝㒠㒛㒞㒥㒞㒡㒡㒥㒞㒙㒤㒜㒝㒡㒝㒝㒝㒙㒞㒗㒜㒡㒜㒝㒟㒢㒛㒥㒘㒜㒛㒝㒛㒙㒚㒥㒛㒣㒚㒝㒚㒙㒝㒟㒙㒡㒡㒢㒙㒙㒘㒥㒘㒡㒙㒟㒘㒙㒗㒥㒛㒜㒗㒝㒣㒤㒦㒥㒦㒡㒦㒝㒦㒙㒥㒥㒥㒡㒘㒤㒥㒙㒘㒠㒤㒡㒤㒟㒤㒙㒤㒥㒣㒡㒣㒝㒥㒣㒢㒥㒥㒟㒢㒝㒥㒠㒡㒥㒢㒣㒡㒝㒡㒙㒤㒜㒠㒡㒟㒛㒠㒙㒟㒥㒟㒡㒡㒝㒟㒙㒞㒥㒢㒘㒞㒝㒡㒠㒝㒥㒠㒗㒝㒝㒞㒛㒜㒥㒜㒡㒟㒥㒜㒙㒘㒠㒛㒡㒛㒝㒛㒙㒜㒗㒚㒡㒚㒝㒝㒢㒙㒥㒚㒦㒙㒞㒙㒙㒘㒥㒙㒣㒘㒝㒘㒙㒛㒟㒗㒡㒤㒘㒗㒙㒦㒥㒦㒡㒗㒟㒦㒙㒥㒥㒙㒜㒥㒝㒠㒠㒤㒥㒤㒡㒤㒝㒤㒙㒣㒥㒣㒡㒦㒤㒣㒙㒦㒠㒢㒡㒢㒟㒢㒙㒢㒥㒡㒡㒡㒝㒣㒣㒠㒥㒤㒤㒠㒝㒣㒠㒟㒥㒠㒣㒟㒝㒟㒙㒢㒜㒞㒡㒦㒜㒞㒙㒝㒥㒝㒡㒟㒝㒝㒙㒜㒥㒠㒘㒜㒝㒟㒠㒛㒥㒤㒙㒛㒝㒝㒙㒚㒥㒚㒡㒝㒤㒚㒙㒝㒜㒙㒡㒝㒜㒙㒙㒙㒥㒘㒡㒘㒝㒚㒣㒗㒥㒠㒙㒗㒝㒚㒠㒦㒥㒙㒡㒦㒝㒦㒙㒘㒟㒥㒡㒦㒡㒥㒙㒚㒘㒤㒡㒥㒟㒤㒙㒣㒥㒗㒘㒣㒝㒦㒚㒢㒥㒢㒡㒢㒝㒤㒙㒡㒥㒡㒡㒤㒤㒡㒙㒤㒜㒠㒡㒠㒝㒠㒚㒡㒗㒟㒡㒟㒝㒢㒡㒞㒥㒙㒥㒞㒝㒞㒙㒝㒥㒞㒣㒝㒝㒝㒙㒠㒞㒜㒡㒗㒡㒜㒙㒛㒥㒛㒡㒜㒟㒛㒙㒚㒥㒞㒛㒚㒝㒥㒝㒙㒥㒙㒡㒙㒝㒙㒙㒘㒥㒘㒡㒛㒤㒘㒙㒛㒟㒗㒡㒗㒟㒗㒙㒗㒥㒦㒡㒦㒝㒘㒣㒥㒥㒟㒝㒥㒝㒘㒠㒤㒥㒗㒡㒤㒝㒤㒙㒦㒟㒣㒡㒤㒙㒣㒙㒣㒞㒢㒢㒥㒝㒢㒙㒡㒥㒤㒛㒡㒝㒜㒟㒠㒥㒢㒛㒠㒝㒡㒛㒟㒥㒟㒡㒢㒤㒟㒙㒙㒣㒞㒡㒞㒝㒞㒙㒟㒥㒝㒡㒝㒝㒠㒠㒜㒥㒠㒘㒜㒝㒞㒟㒛㒥㒜㒣㒛㒝㒛㒙㒞㒝㒚㒡㒗㒘㒚㒙㒙㒥㒙㒡㒚㒟㒙㒙㒘㒥㒜㒚㒘㒝㒦㒝㒗㒥㒗㒡㒗㒝㒗㒙㒦㒥㒦㒡㒙㒤㒦㒙㒙㒞㒥㒡㒥㒟㒥㒙㒥㒥㒤㒡㒤㒝㒦㒤㒣㒥㒢㒠㒣㒝㒦㒠㒢㒥㒣㒡㒢㒝㒢㒙㒤㒠㒡㒡㒦㒟㒡㒙㒣㒟㒠㒡㒣㒝㒠㒙㒟㒥㒢㒝㒟㒝㒦㒝㒞㒥㒡㒙㒞㒝㒟㒙㒝㒥㒝㒡㒠㒙㒝㒙㒢㒗㒜㒡㒞㒚㒜㒙㒝㒗㒛㒡㒛㒝㒞㒠㒚㒥㒝㒢㒚㒝㒚㒙㒙㒥㒛㒡㒙㒝㒙㒙㒜㒜㒘㒡㒛㒤㒘㒙㒗㒥㒗㒢㒘㒟㒗㒙㒦㒥㒚㒙㒦㒝㒗㒡㒥㒥㒥㒡㒥㒝㒦㒛㒤㒥㒤㒡㒗㒦㒤㒙㒥㒝㒣㒡㒣㒝㒣㒙㒤㒗㒢㒡㒢㒝㒥㒣㒡㒥㒣㒙㒡㒝㒡㒙㒠㒥㒠㒡㒠㒝㒠㒙㒣㒜㒟㒡㒣㒗㒟㒙㒟㒗㒞㒡㒟㒝㒞㒙㒝㒥㒠㒝㒝㒝㒚㒝㒜㒥㒠㒘㒜㒝㒟㒙㒛㒥㒛㒡㒞㒙㒛㒙㒜㒣㒚㒡㒟㒙㒚㒙㒛㒗㒙㒡㒙㒝㒜㒠㒘㒥㒛㒢㒘㒝㒘㒙㒗㒥㒙㒡㒗㒝㒗㒙㒚㒜㒦㒡㒙㒤㒦㒙㒥㒥㒥㒢㒦㒟㒥㒙㒤㒥㒘㒙㒤㒝㒡㒠㒣㒥㒣㒡㒣㒝㒤㒛㒢㒥㒢㒡㒥㒦㒢㒙㒟㒜㒡㒡㒡㒝㒡㒙㒢㒗㒠㒡㒠㒝㒣㒣㒟㒥㒝㒘㒟㒝㒟㒙㒞㒥㒞㒡㒞㒝㒞㒙㒡㒜㒝㒡㒡㒗㒝㒙㒝㒗㒜㒡㒝㒝㒜㒙㒛㒥㒞㒝㒛㒝㒜㒤㒚㒦㒞㒘㒚㒝㒛㒛㒙㒥㒙㒡㒜㒤㒙㒙㒗㒣㒘㒡㒘㒝㒘㒙㒙㒥㒗㒡㒗㒝㒚㒠㒦㒥㒚㒘㒦㒝㒘㒟㒥㒥㒦㒣㒥㒝㒥㒙㒘㒝㒤㒡㒞㒟㒤㒙㒣㒥㒣㒡㒤㒟㒣㒙㒢㒥㒦㒚㒢㒝㒞㒤㒡㒥㒡㒡㒡㒝㒢㒛㒠㒥㒠㒡㒤㒗㒠㒙㒢㒠㒟㒡㒟㒝㒟㒙㒠㒗㒞㒡㒞㒝㒡㒤㒝㒥㒚㒜㒝㒝㒝㒙㒜㒥㒜㒡㒜㒝㒜㒙㒟㒜㒛㒡㒟㒘㒛㒙㒛㒗㒚㒡㒛㒝㒚㒙㒙㒥㒜㒝㒙㒝㒜㒗㒘㒥㒜㒘㒘㒝㒙㒛㒗㒥㒗㒡㒚㒤㒗㒙㒥㒣㒦㒡㒦㒝㒦㒙㒗㒥㒥㒡㒥㒝㒘㒠㒤㒥㒘㒘㒤㒝㒦㒟㒣㒥㒤㒣㒣㒝㒣㒙㒦㒝㒢㒡㒟㒘㒢㒙㒡㒥㒡㒡㒢㒟㒡㒙㒠㒥㒤㒚㒠㒝㒡㒞㒟㒦㒟㒡㒟㒝㒠㒛㒞㒥㒞㒡㒢㒗㒞㒙㒚㒠㒝㒡㒝㒝㒝㒙㒞㒗㒜㒡㒜㒝㒟㒤㒛㒥㒗㒘㒛㒝㒛㒙㒚㒥㒚㒡㒚㒝㒚㒙㒝㒜㒙㒡㒝㒘㒙㒙㒙㒗㒘㒡㒙㒝㒘㒙㒗㒥㒚㒝㒗㒝㒛㒜㒦㒥㒚㒘㒦㒝㒙㒙㒥㒥㒥㒡㒘㒙㒥㒙㒜㒗㒤㒡㒣㒤㒤㒙㒥㒗㒣㒡㒣㒝㒦㒠㒢㒥㒚㒠㒢㒝㒢㒙㒡㒥㒣㒡㒡㒝㒡㒙㒤㒜㒠㒡㒣㒤㒠㒙㒘㒝㒟㒡㒡㒝㒟㒙㒞㒥㒢㒘㒞㒝㒡㒠㒝㒥㒡㒠㒝㒝㒞㒙㒜㒥㒜㒡㒟㒙㒜㒙㒤㒝㒛㒡㒞㒤㒛㒙㒝㒥㒚㒡㒚㒝㒜㒥㒙㒥㒚㒥㒙㒝㒤㒞㒘㒥㒙㒣㒘㒝㒘㒙㒛㒜㒗㒡㒚㒞㒗㒙㒦㒥㒦㒡㒘㒝㒦㒙㒥㒥㒙㒘㒥㒝㒘㒠㒤㒥㒤㒡㒤㒞㒥㒛㒥㒥㒣㒡㒦㒥㒣㒙㒞㒙㒢㒡㒢㒝㒢㒙㒣㒗㒣㒥㒡㒝㒤㒢㒠㒥㒛㒥㒠㒝㒠㒙㒟㒥㒠㒣㒟㒝㒟㒙㒢㒟㒞㒡㒙㒡㒞㒙㒝㒥㒝㒡㒝㒝㒝㒙㒜㒥㒠㒘㒜㒝㒟㒣㒛㒥㒛㒣㒛㒝㒜㒙㒚㒥㒚㒡㒝㒙㒚㒙㒣㒡㒙㒡㒜㒤㒙㒙㒛㒥㒘㒡㒘㒝㒚㒥㒗㒥㒘㒝㒗㒝㒗㒢㒦㒦㒙㒡㒦㒝㒦㒙㒘㒡㒥㒡㒠㒣㒥㒙㒦㒟㒤㒡㒥㒟㒤㒙㒣㒥㒗㒘㒣㒝㒞㒗㒢㒥㒢㒡㒢㒝㒤㒙㒡㒥㒡㒡㒤㒤㒡㒙㒤㒜㒠㒡㒢㒣㒠㒙㒡㒗㒟㒡㒟㒝㒢㒡㒞㒥㒛㒜㒞㒝㒞㒙㒝㒥㒞㒣㒝㒝㒝㒙㒠㒞㒜㒡㒚㒡㒜㒙㒛㒥㒛㒡㒛㒝㒛㒙㒚㒥㒞㒘㒚㒝㒝㒢㒙㒥㒙㒣㒙㒝㒚㒙㒘㒥㒘㒡㒛㒚㒘㒙㒦㒤㒗㒡㒚㒤㒗㒙㒗㒥㒦㒡㒦㒝㒘㒦㒥㒥㒚㒣㒥㒝㒗㒥㒤㒥㒗㒡㒤㒝㒤㒙㒦㒣㒣㒡㒚㒡㒣㒙㒚㒡㒢㒡㒣㒝㒢㒙㒡㒥㒤㒟㒡㒝㒦㒛㒠㒥㒢㒞㒠㒝㒡㒛㒟㒥㒟㒡㒢㒤㒟㒙㒡㒦㒞㒡㒞㒝㒞㒙㒟㒥㒝㒡㒝㒝㒠㒠㒜㒥㒠㒘㒜㒝㒜㒙㒛㒦㒜㒣㒛㒝㒛㒙㒞㒝㒚㒡㒛㒥㒚㒙㒙㒥㒙㒡㒚㒟㒙㒙㒘㒥㒜㒚㒘㒝㒙㒡㒗㒥㒗㒡㒗㒝㒘㒛㒦㒥㒦㒡㒚㒗㒦㒙㒗㒝㒥㒡㒥㒝㒥㒙㒤㒥㒤㒡㒤㒝㒗㒠㒣㒥㒗㒛㒣㒝㒣㒛㒢㒥㒣㒡㒢㒝㒢㒙㒤㒣㒡㒡㒞㒡㒡㒙㒤㒜㒠㒡㒣㒝㒠㒙㒟㒥㒢㒟㒟㒝㒡㒗㒞㒥㒣㒝㒞㒝㒟㒛㒝㒥㒝㒡㒠㒤㒝㒙㒟㒦㒜㒡㒜㒝㒜㒙㒝㒥㒛㒡㒛㒝㒞㒠㒚㒥㒞㒘㒚㒝㒚㒙㒙㒦㒚㒣㒙㒝㒙㒙㒜㒝㒘㒡㒥㒤㒘㒙㒗㒥㒗㒡㒘㒟㒗㒙㒦㒥㒚㒚㒦㒝㒣㒠㒥㒥㒥㒡㒥㒝㒦㒛㒤㒥㒤㒡㒘㒗㒤㒙㒡㒜㒣㒡㒣㒝㒣㒙㒢㒥㒢㒡㒢㒝㒥㒠㒡㒥㒥㒛㒡㒝㒡㒛㒠㒥㒡㒡㒠㒝㒠㒙㒢㒣㒟㒡㒡㒘㒟㒚㒢㒜㒞㒡㒟㒟㒞㒙㒝㒥㒡㒘㒝㒝㒜㒗㒜㒥㒜㒡㒜㒝㒞㒙㒛㒥㒛㒡㒞㒤㒛㒙㒞㒜㒚㒡㒜㒣㒚㒙㒛㒗㒙㒡㒙㒝㒜㒡㒘㒥㒢㒙㒘㒝㒘㒙㒗㒥㒘㒣㒗㒝㒗㒙㒚㒞㒦㒡㒣㒘㒦㒙㒥㒥㒥㒡㒦㒟㒥㒙㒤㒥㒘㒛㒤㒝㒤㒘㒣㒥㒣㒡㒣㒝㒤㒛㒢㒥㒢㒡㒦㒘㒢㒙㒞㒠㒡㒡㒡㒝㒡㒙㒠㒥㒠㒡㒠㒝㒣㒠㒟㒥㒣㒜㒟㒝㒟㒛㒞㒥㒟㒡㒞㒝㒞㒙㒠㒣㒝㒡㒠㒛㒝㒙㒠㒜㒜㒡㒝㒟㒜㒙㒛㒥㒟㒘㒛㒝㒚㒗㒚㒥㒚㒡㒚㒝㒜㒙㒙㒥㒙㒡㒜㒤㒙㒙㒜㒜㒘㒡㒚㒣㒘㒙㒙㒗㒗㒡㒗㒝㒚㒡㒦㒥㒣㒜㒦㒝㒦㒙㒥㒥㒦㒣㒥㒝㒥㒙㒘㒞㒤㒡㒥㒢㒤㒚㒣㒥㒣㒡㒤㒟㒣㒙㒢㒥㒦㒛㒢㒝㒞㒤㒡㒥㒡㒡㒡㒝㒢㒛㒠㒥㒠㒡㒤㒘㒠㒙㒛㒜㒟㒡㒟㒝㒟㒙㒞㒥㒞㒡㒞㒝㒡㒠㒝㒥㒡㒜㒝㒝㒝㒛㒜㒥㒝㒡㒜㒝㒜㒙㒞㒣㒛㒡㒟㒠㒛㒙㒞㒜㒚㒡㒛㒟㒚㒙㒙㒥㒝㒘㒙㒝㒡㒘㒘㒥㒘㒡㒘㒝㒚㒙㒗㒥㒗㒡㒚㒤㒗㒙㒚㒜㒦㒡㒞㒥㒦㒙㒗㒥㒥㒡㒥㒝㒘㒠㒤㒥㒘㒘㒤㒝㒘㒘㒣㒥㒤㒡㒣㒝㒣㒙㒥㒣㒢㒡㒚㒥㒢㒙㒥㒜㒡㒡㒤㒝㒡㒙㒠㒥㒣㒟㒠㒝㒡㒝㒟㒥㒟㒛㒟㒝㒠㒛㒞㒥㒞㒡㒡㒤㒞㒙㒠㒦㒝㒡㒝㒝㒝㒙㒞㒥㒜㒡㒜㒝㒟㒠㒛㒥㒟㒘㒛㒝㒛㒙㒚㒦㒛㒣㒚㒝㒚㒙㒝㒝㒙㒡㒤㒡㒙㒙㒘㒥㒘㒡㒙㒟㒘㒙㒗㒥㒛㒚㒗㒝㒢㒝㒦㒥㒦㒡㒦㒝㒗㒛㒥㒥㒥㒡㒙㒗㒥㒙㒠㒙㒤㒡㒤㒝㒤㒙㒣㒥㒣㒡㒣㒝㒦㒠㒢㒥㒦㒛㒢㒝㒢㒛㒡㒥㒢㒡㒡㒝㒡㒙㒣㒣㒠㒡㒚㒙㒠㒙㒣㒜㒟㒡㒢㒝㒟㒙㒞㒥㒡㒟㒞㒝㒞㒥㒝㒥㒞㒚㒝㒞㒠㒙㒜㒥㒜㒡㒟㒛㒜㒙㒗㒛㒛㒡㒝㒗㒛㒙㒜㒗㒚㒡㒚㒝㒝㒠㒙㒥㒤㒟㒙㒝㒙㒙㒘㒥㒚㒡㒘㒝㒘㒙㒛㒜㒗㒡㒚㒤㒗㒙㒙㒛㒦㒡㒗㒟㒦㒙㒥㒥㒙㒙㒥㒝㒡㒤㒤㒥㒤㒡㒤㒝㒥㒛㒣㒥㒣㒡㒦㒦㒣㒙㒡㒙㒢㒡㒢㒝㒢㒙㒡㒥㒡㒡㒡㒝㒤㒠㒠㒥㒤㒚㒠㒝㒠㒛㒟㒥㒠㒡㒟㒝㒟㒙㒡㒤㒞㒡㒝㒜㒞㒙㒡㒜㒝㒡㒞㒝㒝㒙㒜㒥㒟㒠㒜㒝㒡㒛㒛㒥㒞㒟㒛㒝㒜㒙㒚㒥㒚㒡㒝㒝㒚㒙㒟㒗㒙㒡㒛㒚㒙㒙㒚㒗㒘㒡㒘㒝㒛㒠㒗㒥㒚㒢㒗㒝㒗㒙㒦㒥㒘㒡㒦㒝㒦㒙㒙㒜㒥㒡㒘㒤㒥㒙㒤㒥㒤㒢㒥㒟㒤㒙㒣㒥㒗㒙㒣㒝㒟㒤㒢㒥㒢㒡㒢㒝㒣㒛㒡㒥㒡㒡㒤㒦㒡㒙㒝㒠㒠㒡㒠㒝㒠㒙㒡㒗㒟㒡㒟㒝㒢㒣㒞㒥㒛㒜㒞㒝㒞㒙㒝㒥㒝㒡㒝㒝㒝㒙㒠㒜㒜㒡㒠㒗㒜㒙㒜㒗㒛㒡㒜㒝㒛㒙㒚㒥㒝㒡㒚㒝㒗㒝㒙㒥㒝㒘㒙㒝㒜㒙㒘㒥㒘㒡㒛㒝㒘㒙㒙㒣㒗㒡㒢㒚㒗㒙㒘㒗㒦㒡㒦㒝㒙㒠㒥㒥㒘㒢㒥㒝㒥㒙㒤㒥㒦㒡㒤㒝㒤㒙㒗㒜㒣㒡㒦㒤㒣㒙㒢㒥㒢㒢㒣㒟㒢㒙㒡㒥㒥㒙㒡㒝㒞㒠㒠㒥㒠㒡㒠㒝㒡㒛㒟㒥㒟㒡㒢㒦㒟㒙㒜㒜㒞㒡㒞㒝㒞㒙㒟㒗㒟㒡㒝㒝㒠㒣㒜㒥㒚㒘㒜㒝㒜㒙㒛㒥㒛㒡㒝㒠㒛㒙㒞㒜㒚㒡㒞㒗㒚㒙㒚㒗㒙㒡㒚㒝㒙㒙㒘㒥㒛㒡㒘㒝㒙㒤㒗㒦㒛㒘㒗㒝㒚㒙㒦㒥㒦㒡㒙㒝㒦㒙㒤㒝㒥㒡㒜㒜㒥㒙㒦㒗㒤㒡㒤㒝㒗㒠㒣㒥㒢㒟㒣㒝㒣㒙㒢㒥㒤㒡㒢㒝㒢㒙㒥㒜㒡㒡㒤㒤㒡㒙㒣㒛㒠㒡㒡㒟㒠㒙㒟㒥㒣㒙㒟㒝㒛㒤㒞㒥㒞㒡㒞㒝㒟㒛㒝㒥㒝㒡㒠㒦㒝㒙㒙㒠㒜㒡㒜㒝㒜㒙㒝㒗㒛㒡㒛㒝㒞㒣㒚㒥㒙㒚㒚㒝㒚㒙㒙㒥㒚㒣㒙㒝㒙㒙㒜㒠㒘㒡㒥㒘㒘㒙㒗㒥㒗㒡㒗㒝㒗㒙㒦㒥㒚㒘㒦㒝㒙㒤㒥㒥㒥㒣㒥㒝㒦㒙㒤㒥㒤㒡㒗㒝㒤㒙㒦㒣㒣㒡㒦㒤㒣㒙㒤㒗㒢㒡㒢㒝㒥㒠㒡㒥㒠㒟㒡㒝㒡㒙㒠㒥㒢㒡㒠㒝㒠㒙㒣㒜㒟㒡㒢㒤㒟㒙㒡㒛㒞㒡㒟㒟㒞㒙㒝㒥㒡㒙㒝㒝㒙㒤㒜㒥㒜㒡㒜㒝㒝㒛㒛㒥㒛㒡㒞㒦㒛㒙㒦㒘㒚㒡㒚㒝㒚㒙㒛㒗㒙㒡㒙㒝㒜㒣㒘㒥㒥㒜㒘㒝㒘㒙㒗㒥㒘㒣㒗㒝㒗㒙㒚㒠㒦㒡㒣㒘㒦㒙㒥㒥㒥㒡㒥㒝㒥㒙㒤㒥㒘㒘㒤㒝㒗㒤㒣㒥㒣㒣㒣㒝㒤㒙㒢㒥㒢㒡㒥㒝㒢㒙㒦㒘㒡㒡㒤㒤㒡㒙㒣㒥㒠㒡㒠㒝㒣㒝㒟㒥㒦㒥㒟㒝㒥㒛㒞㒥㒟㒡㒞㒝㒞㒙㒡㒙㒝㒡㒢㒟㒝㒙㒜㒦㒜㒡㒝㒟㒜㒙㒛㒥㒟㒘㒛㒝㒞㒚㒚㒥㒚㒡㒚㒝㒜㒙㒙㒥㒙㒡㒜㒤㒙㒙㒜㒜㒘㒡㒘㒝㒘㒚㒙㒗㒗㒡㒗㒝㒚㒡㒦㒥㒘㒙㒦㒝㒦㒙㒥㒥㒦㒣㒥㒝㒥㒙㒘㒞㒤㒡㒥㒥㒤㒙㒣㒥㒣㒡㒤㒟㒣㒙㒢㒥㒦㒛㒢㒝㒣㒡㒡㒥㒡㒡㒡㒝㒡㒙㒠㒥㒠㒡㒣㒤㒠㒙㒣㒟㒟㒡㒟㒟㒟㒙㒟㒥㒞㒡㒞㒝㒡㒝㒝㒥㒚㒥㒝㒝㒠㒠㒜㒥㒝㒣㒜㒝㒜㒙㒟㒜㒛㒡㒚㒛㒛㒙㒚㒥㒚㒡㒜㒝㒚㒙㒙㒥㒝㒘㒙㒝㒜㒠㒘㒥㒛㒗㒘㒝㒙㒛㒗㒥㒗㒡㒚㒥㒗㒙㒚㒜㒦㒡㒦㒝㒦㒙㒗㒗㒥㒡㒥㒝㒘㒢㒤㒥㒡㒜㒤㒝㒤㒙㒣㒥㒤㒣㒣㒝㒣㒙㒦㒟㒢㒡㒡㒥㒢㒙㒡㒥㒡㒡㒢㒟㒡㒙㒠㒥㒤㒜㒠㒝㒜㒤㒟㒥㒟㒡㒟㒝㒟㒙㒞㒥㒞㒡㒡㒤㒞㒙㒡㒠㒝㒡㒝㒟㒝㒙㒝㒥㒜㒡㒜㒝㒟㒝㒛㒥㒞㒟㒛㒝㒞㒠㒚㒥㒛㒣㒚㒝㒚㒙㒝㒜㒙㒡㒘㒛㒙㒙㒘㒥㒘㒡㒚㒝㒘㒙㒗㒥㒛㒘㒗㒝㒚㒠㒦㒥㒙㒗㒦㒝㒗㒛㒥㒥㒥㒡㒘㒥㒥㒙㒡㒠㒤㒡㒤㒝㒤㒙㒥㒗㒣㒡㒣㒝㒦㒢㒢㒥㒝㒛㒢㒝㒢㒙㒡㒥㒢㒣㒡㒝㒡㒙㒤㒟㒠㒡㒝㒘㒠㒙㒟㒥㒟㒡㒠㒟㒟㒙㒞㒥㒢㒜㒞㒝㒝㒤㒝㒥㒝㒡㒝㒝㒝㒙㒜㒥㒜㒡㒟㒤㒜㒙㒟㒠㒛㒡㒛㒟㒛㒙㒛㒥㒚㒡㒚㒝㒝㒝㒙㒥㒝㒤㒙㒝㒜㒠㒘㒥㒛㒡㒘㒝㒘㒙㒛㒙㒗㒡㒞㒟㒗㒙㒦㒜㒦㒡㒗㒟㒦㒙㒥㒥㒙㒘㒥㒝㒝㒘㒤㒥㒤㒡㒤㒝㒦㒙㒣㒥㒣㒡㒦㒤㒣㒙㒦㒜㒢㒡㒚㒥㒢㒙㒣㒥㒡㒡㒡㒝㒤㒠㒠㒥㒤㒘㒠㒝㒤㒘㒟㒥㒠㒡㒟㒝㒟㒙㒢㒙㒞㒡㒦㒥㒞㒙㒡㒜㒝㒡㒠㒝㒝㒙㒜㒥㒟㒥㒜㒝㒝㒝㒛㒥㒡㒣㒛㒝㒜㒛㒚㒥㒚㒡㒝㒤㒚㒙㒜㒦㒙㒡㒙㒝㒙㒙㒚㒥㒘㒡㒘㒝㒛㒠㒗㒥㒛㒘㒗㒝㒗㒙㒦㒦㒗㒣㒦㒝㒦㒙㒙㒝㒥㒡㒚㒚㒥㒙㒤㒥㒤㒡㒥㒟㒤㒙㒣㒥㒗㒚㒣㒝㒗㒦㒢㒥㒢㒡㒢㒝㒣㒛㒡㒥㒡㒡㒥㒗㒡㒙㒥㒢㒠㒡㒠㒝㒠㒙㒟㒥㒟㒡㒟㒝㒢㒠㒞㒥㒢㒛㒞㒝㒞㒛㒝㒥㒞㒡㒝㒝㒝㒙㒠㒙㒜㒡㒦㒙㒜㒙㒟㒜㒛㒡㒞㒝㒛㒙㒚㒥㒝㒥㒚㒝㒟㒦㒙㒥㒛㒛㒙㒝㒜㒙㒘㒥㒘㒡㒛㒡㒘㒙㒘㒡㒗㒡㒗㒦㒗㒚㒙㒥㒦㒡㒦㒝㒙㒝㒥㒥㒡㒗㒥㒝㒦㒣㒤㒥㒥㒣㒤㒝㒤㒙㒗㒜㒣㒡㒞㒛㒣㒙㒢㒥㒢㒡㒤㒝㒢㒙㒡㒥㒥㒘㒡㒝㒤㒠㒠㒥㒣㒗㒠㒝㒡㒛㒟㒥㒟㒡㒢㒥㒟㒙㒛㒠㒞㒡㒞㒝㒞㒙㒟㒗㒝㒡㒝㒝㒠㒢㒜㒥㒚㒥㒜㒝㒜㒙㒛㒥㒛㒡㒛㒝㒛㒙㒞㒜㒚㒡㒝㒦㒚㒙㒚㒗㒙㒡㒚㒝㒙㒙㒘㒥㒛㒦㒘㒝㒗㒘㒗㒥㒛㒘㒗㒝㒘㒙㒦㒥㒦㒡㒙㒢㒦㒙㒛㒗㒥㒡㒘㒡㒥㒙㒦㒗㒤㒡㒤㒝㒗㒠㒣㒥㒝㒢㒣㒝㒣㒙㒢㒥㒤㒡㒢㒝㒢㒙㒥㒜㒡㒡㒤㒤㒡㒙㒣㒛㒠㒡㒠㒝㒠㒙㒟㒥㒣㒙㒟㒝㒟㒚㒞㒥㒞㒡㒞㒝㒟㒛㒝㒥㒝㒡㒠㒦㒝㒙㒙㒜㒜㒡㒜㒝㒜㒙㒝㒥㒛㒡㒛㒝㒞㒢㒚㒥㒞㒚㒚㒝㒜㒟㒙㒥㒚㒣㒙㒝㒙㒙㒜㒟㒘㒡㒥㒘㒘㒙㒗㒥㒗㒡㒘㒟㒗㒙㒦㒥㒚㒜㒦㒝㒙㒚㒥㒥㒥㒡㒥㒝㒗㒙㒤㒥㒤㒡㒘㒘㒤㒙㒗㒠㒣㒡㒣㒝㒣㒚㒤㒗㒢㒡㒢㒝㒥㒥㒡㒥㒣㒙㒡㒝㒡㒙㒠㒥㒡㒣㒠㒝㒠㒙㒣㒢㒟㒡㒡㒗㒟㒚㒞㒥㒞㒡㒟㒟㒞㒙㒝㒥㒡㒟㒝㒝㒞㒣㒜㒦㒜㒡㒜㒝㒜㒙㒛㒥㒛㒡㒟㒘㒛㒙㒞㒣㒚㒡㒚㒝㒚㒙㒙㒥㒙㒡㒙㒝㒜㒢㒘㒥㒘㒡㒘㒝㒘㒛㒗㒥㒘㒣㒜㒛㒗㒙㒚㒟㒦㒡㒢㒤㒦㒙㒥㒥㒥㒡㒗㒝㒥㒙㒤㒥㒘㒛㒤㒝㒗㒣㒣㒥㒦㒗㒣㒝㒤㒛㒢㒥㒢㒡㒦㒘㒢㒙㒗㒣㒡㒡㒡㒝㒡㒙㒢㒗㒠㒡㒠㒝㒣㒥㒟㒥㒢㒢㒟㒝㒟㒙㒞㒥㒠㒡㒞㒝㒞㒙㒡㒡㒝㒡㒡㒙㒝㒙㒜㒥㒜㒢㒝㒟㒜㒙㒛㒥㒟㒞㒛㒝㒝㒜㒚㒥㒚㒡㒚㒝㒛㒛㒙㒥㒙㒡㒝㒛㒙㒙㒟㒛㒘㒡㒘㒝㒘㒙㒙㒗㒗㒡㒗㒝㒛㒘㒦㒥㒘㒙㒦㒝㒦㒙㒥㒥㒥㒡㒥㒝㒥㒙㒘㒡㒤㒡㒘㒜㒤㒙㒣㒥㒣㒡㒣㒝㒣㒙㒢㒥㒦㒛㒢㒝㒢㒙㒡㒥㒡㒡㒡㒝㒡㒙㒡㒞㒠㒡㒣㒥㒠㒙㒟㒥㒟㒡㒟㒞㒟㒙㒞㒥㒥㒗㒞㒝㒡㒠㒝㒥㒝㒣㒝㒝㒝㒛㒜㒥㒝㒡㒝㒢㒜㒙㒟㒛㒛㒡㒤㒟㒛㒙㒞㒜㒚㒡㒛㒝㒛㒞㒙㒥㒝㒗㒙㒝㒞㒛㒘㒥㒛㒥㒘㒝㒘㒟㒘㒙㒗㒡㒚㒤㒗㒙㒦㒦㒦㒡㒦㒞㒦㒙㒥㒦㒥㒡㒥㒝㒘㒡㒤㒥㒤㒡㒤㒝㒥㒚㒣㒥㒣㒡㒣㒝㒤㒛㒣㒚㒢㒡㒥㒥㒢㒙㒢㒙㒡㒢㒡㒝㒡㒙㒢㒥㒠㒡㒠㒝㒣㒡㒟㒥㒣㒙㒟㒝㒣㒤㒞㒥㒞㒡㒞㒝㒞㒙㒡㒞㒝㒡㒠㒤㒝㒙㒜㒥㒜㒡㒜㒝㒜㒙㒛㒥㒟㒙㒛㒝㒛㒛㒚㒥㒚㒣㒚㒝㒚㒙㒙㒥㒙㒡㒜㒥㒙㒙㒘㒦㒘㒡㒘㒞㒘㒙㒘㒛㒗㒥㒗㒝㒚㒡㒦㒥㒗㒙㒦㒝㒦㒚㒥㒥㒥㒢㒥㒝㒥㒙㒘㒝㒤㒡㒤㒝㒤㒙㒥㒣㒣㒡㒣㒝㒣㒙㒤㒗㒢㒦㒢㒝㒥㒢㒡㒥㒡㒥㒡㒞㒡㒙㒠㒥㒢㒡㒠㒝㒠㒙㒣㒞㒟㒡㒢㒦㒟㒙㒣㒠㒞㒡㒞㒝㒞㒙㒝㒥㒡㒛㒝㒝㒠㒡㒜㒥㒜㒡㒜㒝㒜㒙㒛㒥㒛㒡㒞㒦㒛㒙㒛㒗㒚㒡㒚㒟㒚㒙㒙㒥㒙㒡㒙㒝㒜㒢㒘㒥㒘㒢㒘㒝㒘㒚㒗㒥㒘㒗㒗㒡㒗㒙㒚㒞㒦㒡㒗㒗㒦㒙㒥㒦㒥㒡㒥㒞㒥㒙㒤㒥㒘㒙㒤㒝㒤㒙㒣㒥㒥㒡㒣㒝㒣㒙㒢㒥㒣㒣㒢㒢㒢㒙㒥㒟㒡㒡㒡㒡㒡㒚㒠㒥㒠㒡㒢㒝㒠㒙㒟㒥㒣㒛㒟㒝㒢㒣㒞㒥㒣㒜㒞㒝㒞㒙㒝㒥㒝㒡㒡㒘㒝㒙㒠㒞㒜㒡㒜㒝㒜㒙㒛㒥㒛㒡㒛㒝㒞㒣㒚㒥㒚㒣㒚㒝㒚㒛㒙㒥㒙㒡㒙㒝㒙㒙㒜㒟㒘㒡㒘㒞㒘㒙㒗㒦㒗㒡㒗㒣㒗㒝㒦㒥㒚㒛㒦㒝㒦㒛㒥㒥㒥㒢㒥㒝㒥㒚㒤㒥㒤㒡㒗㒥㒤㒙㒣㒥㒣㒡㒥㒝㒣㒙㒢㒥㒢㒡㒣㒟㒢㒞㒡㒥㒥㒜㒡㒝㒡㒝㒠㒦㒠㒡㒠㒝㒢㒙㒟㒥㒟㒡㒣㒘㒟㒙㒢㒠㒞㒡㒣㒘㒞㒙㒝㒥㒝㒡㒝㒝㒠㒥㒜㒥㒠㒛㒜㒝㒜㒙㒛㒥㒛㒡㒛㒝㒛㒙㒞㒠㒚㒡㒚㒟㒚㒙㒚㒗㒙㒡㒙㒝㒙㒙㒘㒥㒜㒜㒘㒝㒘㒚㒗㒥㒗㒢㒗㒝㒗㒟㒗㒙㒦㒡㒚㒘㒦㒙㒦㒞㒥㒡㒥㒞㒥㒙㒤㒦㒤㒡㒤㒝㒗㒡㒣㒥㒣㒡㒣㒝㒥㒛㒢㒥㒢㒡㒢㒝㒣㒛㒢㒚㒡㒡㒥㒙㒡㒙㒡㒙㒠㒢㒠㒝㒠㒙㒡㒥㒟㒡㒟㒝㒢㒥㒞㒥㒢㒝㒞㒝㒢㒤㒝㒥㒝㒡㒝㒝㒝㒙㒠㒢㒜㒡㒠㒘㒜㒙㒛㒥㒛㒡㒛㒝㒛㒙㒚㒥㒞㒝㒚㒝㒚㒛㒙㒥㒙㒣㒙㒝㒙㒙㒘㒥㒘㒡㒜㒙㒘㒙㒗㒦㒗㒡㒗㒞㒗㒙㒗㒛㒦㒥㒦㒝㒙㒥㒥㒥㒦㒞㒥㒝㒥㒚㒤㒥㒤㒢㒤㒝㒤㒙㒗㒝㒣㒡㒣㒝㒣㒙㒥㒙㒢㒡㒢㒝㒢㒙㒣㒗㒡㒦㒡㒝㒤㒦㒠㒥㒠㒥㒠㒞㒠㒙㒟㒥㒡㒡㒟㒝㒟㒙㒢㒢㒞㒡㒢㒚㒞㒙㒢㒠㒝㒡㒝㒝㒝㒙㒜㒥㒠㒟㒜㒝㒟㒥㒛㒥㒛㒡㒛㒝㒛㒙㒚㒥㒚㒡㒞㒚㒚㒙㒚㒗㒙㒡㒙㒟㒙㒙㒘㒥㒘㒡㒘㒝㒛㒦㒗㒥㒗㒢㒗㒝㒗㒚㒦㒥㒗㒗㒦㒡㒦㒙㒙㒢㒥㒡㒥㒡㒥㒙㒤㒦㒤㒡㒤㒞㒤㒙㒣㒥㒗㒙㒣㒝㒣㒙㒢㒥㒥㒗㒢㒝㒢㒙㒡㒥㒢㒣㒡㒢㒡㒙㒤㒣㒠㒡㒠㒡㒠㒚㒟㒥㒟㒡㒡㒝㒟㒙㒞㒥㒢㒟㒞㒝㒢㒗㒝㒥㒢㒜㒝㒝㒝㒙㒜㒥㒜㒡㒠㒜㒜㒙㒟㒢㒛㒡㒛㒝㒛㒙㒚㒥㒚㒡㒚㒝㒞㒗㒙㒥㒙㒣㒙㒝㒙㒛㒘㒥㒘㒡㒘㒝㒘㒙㒛㒣㒗㒡㒗㒞㒗㒙㒦㒦㒦㒡㒦㒣㒦㒝㒥㒥㒙㒟㒥㒝㒥㒟㒤㒥㒤㒢㒤㒝㒤㒚㒣㒥㒣㒡㒦㒥㒣㒙㒢㒥㒢㒡㒤㒥㒢㒙㒡㒥㒡㒡㒢㒟㒡㒞㒠㒥㒤㒠㒠㒝㒠㒝㒟㒦㒟㒡㒟㒝㒡㒙㒞㒥㒞㒡㒢㒜㒞㒙㒡㒤㒝㒡㒢㒘㒝㒙㒜㒥㒜㒡㒜㒝㒠㒙㒛㒥㒟㒟㒛㒝㒛㒙㒚㒥㒚㒡㒚㒝㒚㒙㒝㒤㒙㒡㒙㒟㒙㒙㒙㒗㒘㒡㒘㒝㒘㒙㒗㒥㒛㒠㒗㒝㒗㒚㒦㒥㒦㒢㒦㒝㒦㒟㒦㒙㒥㒡㒙㒜㒥㒙㒥㒡㒤㒡㒤㒞㒤㒙㒣㒦㒣㒡㒣㒝㒦㒡㒢㒥㒢㒡㒢㒝㒤㒣㒡㒥㒡㒡㒡㒝㒢㒛㒡㒚㒠㒡㒤㒝㒠㒙㒠㒙㒟㒢㒟㒝㒟㒙㒠㒥㒞㒡㒞㒝㒢㒙㒝㒥㒡㒡㒝㒝㒡㒤㒜㒥㒜㒡㒜㒝㒜㒙㒟㒦㒛㒡㒟㒜㒛㒙㒚㒥㒚㒡㒚㒝㒚㒙㒙㒥㒝㒡㒙㒝㒙㒛㒘㒥㒘㒣㒘㒝㒘㒙㒗㒥㒗㒡㒛㒝㒗㒙㒦㒦㒦㒡㒦㒞㒦㒙㒦㒛㒥㒥㒥㒝㒙㒙㒤㒥㒥㒜㒤㒝㒤㒚㒣㒥㒣㒢㒣㒝㒣㒙㒦㒝㒢㒡㒢㒝㒢㒙㒤㒡㒡㒡㒡㒝㒡㒙㒢㒗㒠㒦㒠㒝㒤㒚㒟㒥㒟㒥㒟㒞㒟㒙㒞㒥㒠㒡㒞㒝㒞㒙㒡㒦㒝㒡㒡㒞㒝㒙㒡㒠㒜㒡㒜㒝㒜㒙㒛㒥㒟㒣㒛㒝㒟㒙㒚㒥㒚㒡㒚㒝㒚㒙㒙㒥㒙㒡㒝㒞㒙㒙㒙㒗㒘㒡㒘㒟㒘㒙㒗㒥㒗㒡㒗㒝㒛㒚㒦㒥㒦㒢㒦㒝㒦㒚㒥㒥㒦㒗㒥㒡㒥㒙㒘㒦㒤㒡㒤㒠㒤㒙㒣㒦㒣㒡㒣㒞㒣㒙㒢㒥㒦㒙㒢㒝㒢㒙㒡㒥㒤㒟㒡㒝㒡㒙㒠㒥㒡㒣㒠㒢㒠㒙㒤㒗㒟㒡㒟㒡㒟㒚㒞㒥㒞㒡㒠㒝㒞㒙㒝㒥㒡㒣㒝㒝㒡㒛㒜㒥㒡㒜㒜㒝㒜㒙㒛㒥㒛㒡㒟㒠㒛㒙㒞㒦㒚㒡㒚㒝㒚㒙㒙㒥㒙㒡㒙㒝㒝㒛㒘㒥㒘㒣㒘㒝㒘㒛㒗㒥㒗㒡㒗㒝㒗㒙㒛㒗㒦㒡㒦㒞㒦㒙㒥㒦㒥㒡㒥㒣㒥㒝㒤㒥㒘㒣㒤㒝㒤㒙㒣㒥㒣㒢㒣㒝㒣㒚㒢㒥㒢㒡㒥㒥㒢㒙㒡㒥㒡㒡㒤㒡㒡㒙㒠㒥㒠㒡㒡㒟㒠㒞㒟㒥㒣㒤㒟㒝㒟㒝㒞㒦㒞㒡㒞㒝㒠㒙㒝㒥㒝㒡㒡㒠㒝㒙㒡㒘㒜㒡㒡㒘㒜㒙㒛㒥㒛㒡㒛㒝㒟㒝㒚㒥㒞㒣㒚㒝㒚㒙㒙㒥㒙㒡㒙㒝㒙㒙㒝㒘㒘㒡㒘㒟㒘㒙㒘㒗㒗㒡㒗㒝㒗㒙㒦㒥㒚㒤㒦㒝㒦㒚㒥㒥㒥㒢㒥㒝㒥㒙㒚㒞㒤㒡㒤㒝㒤㒙㒣㒦㒣㒡㒣㒝㒣㒙㒢㒥");local C=((94+-65)+-#[[cilerteddoesntlikeburgers]])local l=90 local o=d;local e={}e={[(-81+82)]=function()local e,a,r,d=v(Y,o,o+m);o=o+g;l=(l+(C*g))%n;return(((d+l-(C)+f*(g*p))%f)*((p*H)^p))+(((r+l-(C*p)+f*(p^m))%n)*(f*n))+(((a+l-(C*m)+H)%n)*f)+((e+l-(C*g)+H)%n);end,[((1904/112)+-#[[W4rboy was here]])]=function(e,e,e)local e=v(Y,o,o);o=o+S;l=(l+(C))%n;return((e+l-(C)+H)%f);end,[(-#'fatee is gay 0nly on top'+(126-(295-196)))]=function()local d,e=v(Y,o,o+p);l=(l+(C*p))%n;o=o+p;return(((e+l-(C)+f*(p*g))%f)*n)+((d+l-(C*p)+n*(p^m))%f);end,[((144+-33)-107)]=function(l,e,o)if o then local e=(l/p^(e-d))%p^((o-S)-(e-d)+S);return e-e%d;else local e=p^(e-S);return(l%(e+e)>=e)and d or y;end;end,[(485/97)]=function()local o=e[(66-65)]();local a=e[(161/161)]();local r=d;local l=(e[(732/(-#"Faggot"+(449-260)))](a,S,z+g)*(p^(z*p)))+o;local o=e[((3192/168)+-#"W4rboy was here")](a,21,31);local e=((-d)^e[(-101+105)](a,32));if(o==y)then if(l==A)then return e*y;else o=S;r=A;end;elseif(o==(f*(p^m))-S)then return(l==y)and(e*(S/A))or(e*(y/A));end;return R(e,o-((n*(g))-d))*(r+(l/(p^V)));end,[(-#'nerd'+(270/27))]=function(a,r,r)local r;if(not a)then a=e[(-#'when the he went where when he where where when the he when ther wher he then here went'+(274-186))]();if(a==y)then return'';end;end;r=G(Y,o,o+a-d);o=o+a;local e=''for o=S,#r do e=j(e,I((v(G(r,o,o))+l)%n))l=(l+C)%f end return e;end}local function H(...)return{...},K('#',...)end local function Y()local x={};local i={};local o={};local a={x,i,nil,o};local l={}local c=(12+-#{22,'}';'nil'})local n={[((2288/88)+-#"fatee is gay 0nly on top")]=(function(o)return not(#o==e[((104/13)+-#'Ur mom')]())end),[((2457/189)+-#"send nudes")]=(function(o)return e[(735/147)]()end),[(((-1980/55)+84)+-#[[never gonna give you up never gonna let you down]])]=(function(o)return e[(29-23)]()end),[(752/188)]=(function(o)local d=e[(100+-94)]()local e=''local o=1 for l=1,#d do o=(o+c)%n e=j(e,I((v(d:sub(l,l))+o)%f))end return e end)};for e=S,e[(173/173)]()do i[e-S]=Y();end;local o=e[(((221+-124)+-#"Nsrds GAYYYYAIAHAKAJAVAHAUA")/70)]()for o=1,o do local e=e[(88-86)]();local d;local e=n[e%(4200/100)];l[o]=e and e({});end;for a=1,e[(177/177)]()do local o=e[(284/142)]();if(e[(-#"Impulse real 2022"+(5271/(-47+298)))](o,d,S)==A)then local c=e[(-#[[this is a meme string]]+(166-141))](o,p,m);local n=e[((6106/142)+-#[[papier ist ein kleiner schwanz lutscher]])](o,g,p+g);local o={e[((((83-96)+-#"never gonna give you up never gonna let you down")+73)+-#"Deezbutts")](),e[(-102+105)](),nil,nil};local i={[(71+-71)]=function()o[u]=e[(122+-119)]();o[D]=e[(((214+-93)+-#[[nicowashere]])-107)]();end,[(67-66)]=function()o[t]=e[((1105/85)+-#'deadphonelua')]();end,[(109+-107)]=function()o[u]=e[(66+-65)]()-(p^z)end,[(45+-42)]=function()o[t]=e[((67+(-26-20))+-#"Impulse youtube real")]()-(p^z)o[M]=e[(375/125)]();end};i[c]();if(e[(103+(-165+66))](n,S,d)==S)then o[r]=l[o[r]]end if(e[((112-92)+-16)](n,p,p)==d)then o[t]=l[o[U]]end if(e[(107-103)](n,m,m)==S)then o[_]=l[o[_]]end x[a]=o;end end;a[3]=e[(138/69)]();return a;end;local function A(e,y,f)local v=e[p];local o=e[m];local n=e[d];return(function(...)local z={};local C=o;local m=H local l={};local o=d;local e=d e*=-1 local g=e;local Y=K('#',...)-S;local v=v;local I={};local n=n;local H={...};for e=0,Y do if(e>=C)then I[e-C]=H[e+S];else l[e]=H[e+d];end;end;local e=Y-C+d local e;local C;while true do e=n[o];C=e[((86-65)+-#"Cock and ball tortue")];a=(91154)while((((857105/37)+-#"how to join the kkk")/142)+-#"when the he went where when he where where when the he when ther wher he then here went")>=C do a-= a a=(9634482)while C<=(-#[[niggers]]+(9768/222))do a-= a a=(6687144)while C<=((5589/207)+-#"Crackzzzz")do a-= a a=(5690992)while(976/122)>=C do a-= a a=(591360)while C<=((101-82)+-#'warboy hates you')do a-= a a=(4576752)while(80/80)>=C do a-= a a=(2155500)while(-#[[nerd]]+(-102+((389-238)+-#"testpsx dupe no scam legit 2022 free no virus")))<C do a-= a local d=e[c];local o=l[d]for e=d+1,e[M]do o=o..l[e];end;l[e[r]]=o;break end while 1437==(a)/((-#"W4rboy was here"+(-111+1626)))do l[e[b]]=#l[e[u]];break end;break;end while 1776==(a)/((5262-2685))do a=(4152295)while(-#[[panzerfaust]]+(103+(-3690/41)))<C do a-= a local a;l[e[r]]=f[e[c]];o=o+d;e=n[o];l[e[w]]=l[e[u]][e[_]];o=o+d;e=n[o];l[e[r]]=e[k];o=o+d;e=n[o];l[e[b]]=e[u];o=o+d;e=n[o];l[e[b]]=e[k];o=o+d;e=n[o];l[e[O]]=e[c];o=o+d;e=n[o];a=e[w]l[a]=l[a](s(l,a+d,e[h]))o=o+d;e=n[o];l[e[w]][e[c]]=l[e[M]];o=o+d;e=n[o];l[e[i]]=f[e[u]];o=o+d;e=n[o];l[e[r]]=l[e[k]][e[B]];o=o+d;e=n[o];l[e[O]]=e[h];o=o+d;e=n[o];l[e[r]]=e[c];o=o+d;e=n[o];l[e[i]]=e[c];o=o+d;e=n[o];l[e[b]]=e[u];o=o+d;e=n[o];a=e[i]l[a]=l[a](s(l,a+d,e[h]))o=o+d;e=n[o];l[e[w]][e[u]]=l[e[N]];o=o+d;e=n[o];l[e[i]]=f[e[c]];o=o+d;e=n[o];l[e[x]]=l[e[k]][e[N]];o=o+d;e=n[o];l[e[x]]=l[e[k]][e[M]];o=o+d;e=n[o];l[e[r]][e[U]]=l[e[N]];o=o+d;e=n[o];l[e[r]][e[t]]=e[D];o=o+d;e=n[o];l[e[x]]=f[e[c]];o=o+d;e=n[o];l[e[r]]=l[e[u]][e[P]];o=o+d;e=n[o];l[e[w]]=e[u];o=o+d;e=n[o];l[e[x]]=e[k];o=o+d;e=n[o];l[e[r]]=e[U];o=o+d;e=n[o];a=e[w]l[a]=l[a](s(l,a+d,e[u]))o=o+d;e=n[o];l[e[i]][e[c]]=l[e[N]];o=o+d;e=n[o];l[e[O]][e[c]]=e[M];o=o+d;e=n[o];l[e[b]][e[h]]=e[_];o=o+d;e=n[o];l[e[O]][e[k]]=e[B];o=o+d;e=n[o];l[e[r]][e[U]]=e[D];o=o+d;e=n[o];l[e[i]][e[k]]=l[e[N]];o=o+d;e=n[o];l[e[r]]=f[e[u]];o=o+d;e=n[o];l[e[x]]=l[e[c]][e[N]];o=o+d;e=n[o];l[e[r]]=e[c];o=o+d;e=n[o];l[e[w]]=e[t];o=o+d;e=n[o];l[e[x]]=e[t];o=o+d;e=n[o];a=e[w]l[a]=l[a](s(l,a+d,e[k]))o=o+d;e=n[o];l[e[x]][e[c]]=l[e[N]];o=o+d;e=n[o];l[e[w]][e[c]]=e[N];o=o+d;e=n[o];l[e[r]]=f[e[u]];o=o+d;e=n[o];l[e[r]]=l[e[t]][e[_]];o=o+d;e=n[o];l[e[w]]=e[U];o=o+d;e=n[o];l[e[b]]=e[h];o=o+d;e=n[o];l[e[b]]=e[U];o=o+d;e=n[o];l[e[w]]=e[t];o=o+d;e=n[o];a=e[b]l[a]=l[a](s(l,a+d,e[h]))o=o+d;e=n[o];l[e[i]][e[t]]=l[e[N]];o=o+d;e=n[o];l[e[b]]=f[e[u]];o=o+d;e=n[o];l[e[w]]=l[e[t]][e[_]];o=o+d;e=n[o];l[e[O]]=e[t];o=o+d;e=n[o];l[e[r]]=e[k];o=o+d;e=n[o];l[e[b]]=e[u];o=o+d;e=n[o];l[e[r]]=e[c];o=o+d;e=n[o];a=e[i]l[a]=l[a](s(l,a+d,e[h]))o=o+d;e=n[o];l[e[b]][e[u]]=l[e[M]];o=o+d;e=n[o];l[e[x]]=f[e[c]];o=o+d;e=n[o];l[e[r]]=l[e[h]][e[P]];o=o+d;e=n[o];l[e[O]]=l[e[h]][e[_]];o=o+d;e=n[o];l[e[x]][e[t]]=l[e[P]];o=o+d;e=n[o];l[e[r]][e[u]]=e[N];o=o+d;e=n[o];l[e[w]]=f[e[h]];o=o+d;e=n[o];l[e[w]]=l[e[h]][e[_]];o=o+d;e=n[o];l[e[x]]=e[u];o=o+d;e=n[o];l[e[x]]=e[h];o=o+d;e=n[o];l[e[x]]=e[c];o=o+d;e=n[o];a=e[b]l[a]=l[a](s(l,a+d,e[c]))o=o+d;e=n[o];l[e[i]][e[k]]=l[e[P]];o=o+d;e=n[o];l[e[x]][e[h]]=e[M];o=o+d;e=n[o];l[e[x]][e[U]]=e[M];o=o+d;e=n[o];l[e[r]][e[h]]=e[B];o=o+d;e=n[o];l[e[r]][e[h]]=e[M];o=o+d;e=n[o];l[e[i]][e[U]]=l[e[_]];o=o+d;e=n[o];l[e[i]]=f[e[h]];o=o+d;e=n[o];l[e[i]]=l[e[c]][e[N]];o=o+d;e=n[o];l[e[O]]=e[c];o=o+d;e=n[o];l[e[r]]=e[c];o=o+d;e=n[o];l[e[w]]=e[u];o=o+d;e=n[o];a=e[r]l[a]=l[a](s(l,a+d,e[U]))break end while 3115==(a)/(((413287/151)-1404))do if(l[e[w]]~=l[e[B]])then o=o+S;else o=e[U];end;break end;break;end break;end while(a)/((-23+471))==1320 do a=(4188992)while C<=(-#'Niggabyte'+(143-129))do a-= a a=(2915004)while(412/103)<C do a-= a local a;l[e[i]]=f[e[k]];o=o+d;e=n[o];l[e[w]]=l[e[h]][e[B]];o=o+d;e=n[o];l[e[i]]=l[e[c]];o=o+d;e=n[o];a=e[b]l[a]=l[a](l[a+S])o=o+d;e=n[o];l[e[i]]();break end while 842==(a)/(((-76+(696584/196))+-#[[cruz pp is large]]))do local i=v[e[U]];local r;local d={};r=L({},{__index=function(o,e)local e=d[e];return e[1][e[2]];end,__newindex=function(l,e,o)local e=d[e]e[1][e[2]]=o;end;});for a=1,e[M]do o=o+S;local e=n[o];if e[(119/119)]==56 then d[a-1]={l,e[h]};else d[a-1]={y,e[h]};end;z[#z+1]=d;end;l[e[w]]=A(i,r,f);break end;break;end while(a)/((3635-1866))==2368 do a=(11626563)while(((185+-28)+-#"when the he went where when he where where when the he when ther wher he then here went")-64)>=C do a-= a if(l[e[w]]==l[e[M]])then o=o+S;else o=e[u];end;break;end while(a)/(((-33-26)+3770))==3133 do a=(4454886)while C>(1064/152)do a-= a local e={l,e};e[S][e[p][w]]=e[d][e[p][N]]+e[S][e[p][U]];break end while 3342==(a)/((-#"atakan der nigga"+((-64+1449)+-36)))do l[e[x]]=l[e[h]][e[_]];break end;break;end break;end break;end break;end while(a)/((-#[[niggers]]+(350435/109)))==1774 do a=(14177418)while C<=((134-(-64+169))+-#"Fucking Retarted")do a-= a a=(6340104)while C<=(-93+103)do a-= a a=(796635)while C>(-#"deadphonelua"+(73-(-#[[psx real dupe steal all ur pets no joke]]+(12649/139))))do a-= a local e=e[r]l[e](l[e+S])break end while(a)/((5768-2933))==281 do local e=e[b];local o=l[e];for e=e+1,g do F(o,l[e])end;break end;break;end while(a)/((-17+1574))==4072 do a=(431730)while C<=(-#"Impulse youtube real"+(4247/137))do a-= a local x;local t,k;local b;local a;l[e[O]]=f[e[h]];o=o+d;e=n[o];l[e[i]]=f[e[c]];o=o+d;e=n[o];a=e[w];b=l[e[u]];l[a+1]=b;l[a]=b[e[M]];o=o+d;e=n[o];l[e[w]]=e[u];o=o+d;e=n[o];a=e[r]t,k=m(l[a](s(l,a+1,e[U])))g=k+a-1 x=0;for e=a,g do x=x+d;l[e]=t[x];end;o=o+d;e=n[o];a=e[i]l[a]=l[a](s(l,a+d,g))o=o+d;e=n[o];l[e[w]]();o=o+d;e=n[o];do return end;break;end while 2665==(a)/((-45+207))do a=(729028)while C>((-#'Fucking Retarted'+(1273-669))/49)do a-= a local b;local a;l[e[i]]=f[e[h]];o=o+d;e=n[o];l[e[i]]=l[e[t]][e[P]];o=o+d;e=n[o];l[e[O]]=e[U];o=o+d;e=n[o];l[e[O]]=y[e[c]];o=o+d;e=n[o];a=e[i]l[a]=l[a](s(l,a+d,e[U]))o=o+d;e=n[o];l[e[x]]=l[e[k]][e[_]];o=o+d;e=n[o];l[e[i]]=l[e[t]][e[B]];o=o+d;e=n[o];a=e[r];b=l[e[h]];l[a+1]=b;l[a]=b[e[_]];break end while 302==(a)/((330718/137))do y[e[t]]=l[e[i]];break end;break;end break;end break;end while 3511==(a)/((-#[[windows xp startup sfx]]+(125860/31)))do a=(1585896)while C<=(2865/191)do a-= a a=(6320775)while C>((137-(11484/116))+-#'keno 0347 is a nerdy fag')do a-= a local a;l[e[w]]=f[e[c]];o=o+d;e=n[o];l[e[x]]=l[e[u]][e[D]];o=o+d;e=n[o];l[e[r]]=e[c];o=o+d;e=n[o];l[e[x]]=e[U];o=o+d;e=n[o];l[e[O]]=e[u];o=o+d;e=n[o];a=e[b]l[a]=l[a](s(l,a+d,e[u]))o=o+d;e=n[o];l[e[b]][e[c]]=l[e[_]];o=o+d;e=n[o];l[e[r]][e[h]]=e[B];o=o+d;e=n[o];l[e[b]]=f[e[U]];o=o+d;e=n[o];l[e[r]]=l[e[c]][e[D]];o=o+d;e=n[o];l[e[O]]=e[c];o=o+d;e=n[o];l[e[w]]=e[t];o=o+d;e=n[o];l[e[i]]=e[U];o=o+d;e=n[o];l[e[w]]=e[u];o=o+d;e=n[o];a=e[O]l[a]=l[a](s(l,a+d,e[k]))o=o+d;e=n[o];l[e[b]][e[t]]=l[e[D]];o=o+d;e=n[o];l[e[r]][e[h]]=e[D];o=o+d;e=n[o];l[e[x]]=f[e[U]];o=o+d;e=n[o];l[e[i]]=l[e[c]][e[P]];o=o+d;e=n[o];l[e[x]]=e[c];o=o+d;e=n[o];l[e[i]]=e[h];o=o+d;e=n[o];l[e[O]]=e[k];o=o+d;e=n[o];l[e[i]]=e[t];o=o+d;e=n[o];a=e[i]l[a]=l[a](s(l,a+d,e[t]))o=o+d;e=n[o];l[e[i]][e[c]]=l[e[P]];o=o+d;e=n[o];l[e[r]][e[k]]=e[M];o=o+d;e=n[o];l[e[w]]=f[e[h]];o=o+d;e=n[o];l[e[r]]=l[e[t]][e[_]];o=o+d;e=n[o];l[e[i]]=l[e[c]][e[_]];o=o+d;e=n[o];l[e[x]][e[U]]=l[e[_]];o=o+d;e=n[o];l[e[r]][e[t]]=e[B];o=o+d;e=n[o];l[e[O]][e[U]]=l[e[_]];o=o+d;e=n[o];l[e[r]]=f[e[h]];o=o+d;e=n[o];l[e[w]]=l[e[k]][e[M]];o=o+d;e=n[o];l[e[w]]=e[u];o=o+d;e=n[o];l[e[b]]=e[U];o=o+d;e=n[o];l[e[b]]=e[u];o=o+d;e=n[o];a=e[i]l[a]=l[a](s(l,a+d,e[k]))o=o+d;e=n[o];l[e[i]][e[k]]=l[e[P]];o=o+d;e=n[o];l[e[i]][e[h]]=e[P];o=o+d;e=n[o];l[e[w]]=f[e[k]];o=o+d;e=n[o];l[e[w]]=l[e[t]][e[D]];o=o+d;e=n[o];l[e[i]]=e[U];o=o+d;e=n[o];l[e[r]]=e[k];o=o+d;e=n[o];l[e[b]]=e[t];o=o+d;e=n[o];l[e[x]]=e[t];o=o+d;e=n[o];a=e[x]l[a]=l[a](s(l,a+d,e[u]))o=o+d;e=n[o];l[e[r]][e[k]]=l[e[N]];o=o+d;e=n[o];l[e[O]]=f[e[k]];o=o+d;e=n[o];l[e[b]]=l[e[t]][e[B]];o=o+d;e=n[o];l[e[b]]=e[k];o=o+d;e=n[o];l[e[r]]=e[U];o=o+d;e=n[o];l[e[O]]=e[k];o=o+d;e=n[o];l[e[w]]=e[c];o=o+d;e=n[o];a=e[b]l[a]=l[a](s(l,a+d,e[t]))o=o+d;e=n[o];l[e[b]][e[h]]=l[e[N]];o=o+d;e=n[o];l[e[i]]=f[e[c]];o=o+d;e=n[o];l[e[O]]=l[e[k]][e[M]];o=o+d;e=n[o];l[e[w]]=l[e[t]][e[P]];o=o+d;e=n[o];l[e[x]][e[U]]=l[e[_]];o=o+d;e=n[o];l[e[i]][e[h]]=e[_];o=o+d;e=n[o];l[e[r]]=f[e[h]];o=o+d;e=n[o];l[e[r]]=l[e[c]][e[M]];o=o+d;e=n[o];l[e[w]]=e[k];o=o+d;e=n[o];l[e[r]]=e[U];o=o+d;e=n[o];l[e[r]]=e[k];o=o+d;e=n[o];a=e[i]l[a]=l[a](s(l,a+d,e[u]))o=o+d;e=n[o];l[e[O]][e[u]]=l[e[B]];o=o+d;e=n[o];l[e[w]][e[U]]=e[N];o=o+d;e=n[o];l[e[O]][e[k]]=e[P];o=o+d;e=n[o];l[e[x]][e[u]]=e[P];o=o+d;e=n[o];l[e[x]][e[u]]=e[M];o=o+d;e=n[o];l[e[r]][e[u]]=l[e[D]];o=o+d;e=n[o];l[e[x]]=f[e[c]];o=o+d;e=n[o];l[e[x]]=l[e[t]][e[N]];o=o+d;e=n[o];l[e[x]]=e[t];o=o+d;e=n[o];l[e[w]]=e[k];o=o+d;e=n[o];l[e[i]]=e[c];o=o+d;e=n[o];a=e[O]l[a]=l[a](s(l,a+d,e[U]))o=o+d;e=n[o];l[e[O]][e[k]]=l[e[N]];break end while(a)/(((7240-3670)+-#[[Crackzzzz]]))==1775 do o=e[t];break end;break;end while(a)/((1634-852))==2028 do a=(3794780)while C<=(3088/193)do a-= a l[e[b]]=(e[k]~=0);o=o+S;break;end while 2585==(a)/(((1595+-119)+-#'Gay porn'))do a=(5697978)while C>((-120+182)+-#"testpsx dupe no scam legit 2022 free no virus")do a-= a local a;l[e[x]][e[h]]=e[B];o=o+d;e=n[o];l[e[w]]=f[e[u]];o=o+d;e=n[o];l[e[b]]=l[e[t]][e[M]];o=o+d;e=n[o];l[e[w]]=e[U];o=o+d;e=n[o];l[e[i]]=e[t];o=o+d;e=n[o];l[e[r]]=e[k];o=o+d;e=n[o];l[e[x]]=e[h];o=o+d;e=n[o];a=e[x]l[a]=l[a](s(l,a+d,e[h]))o=o+d;e=n[o];l[e[b]][e[t]]=l[e[D]];o=o+d;e=n[o];l[e[r]]=f[e[U]];o=o+d;e=n[o];l[e[i]]=l[e[h]][e[N]];o=o+d;e=n[o];l[e[w]]=e[h];o=o+d;e=n[o];l[e[i]]=e[c];o=o+d;e=n[o];l[e[i]]=e[h];o=o+d;e=n[o];l[e[i]]=e[U];o=o+d;e=n[o];a=e[O]l[a]=l[a](s(l,a+d,e[U]))o=o+d;e=n[o];l[e[w]][e[u]]=l[e[_]];o=o+d;e=n[o];l[e[x]]=f[e[h]];o=o+d;e=n[o];l[e[w]]=l[e[h]][e[_]];o=o+d;e=n[o];l[e[O]]=l[e[k]][e[N]];o=o+d;e=n[o];l[e[b]][e[u]]=l[e[B]];o=o+d;e=n[o];l[e[x]][e[U]]=e[D];o=o+d;e=n[o];l[e[w]]=f[e[c]];o=o+d;e=n[o];l[e[O]]=l[e[c]][e[B]];o=o+d;e=n[o];l[e[b]]=e[h];o=o+d;e=n[o];l[e[r]]=e[h];o=o+d;e=n[o];l[e[i]]=e[c];o=o+d;e=n[o];a=e[b]l[a]=l[a](s(l,a+d,e[k]))o=o+d;e=n[o];l[e[x]][e[t]]=l[e[_]];o=o+d;e=n[o];l[e[i]][e[t]]=e[_];o=o+d;e=n[o];l[e[O]][e[U]]=e[P];o=o+d;e=n[o];l[e[O]][e[c]]=e[M];o=o+d;e=n[o];l[e[O]][e[k]]=e[M];o=o+d;e=n[o];l[e[O]][e[k]]=l[e[_]];o=o+d;e=n[o];l[e[O]]=f[e[h]];o=o+d;e=n[o];l[e[x]]=l[e[c]][e[N]];o=o+d;e=n[o];l[e[O]]=e[u];o=o+d;e=n[o];l[e[i]]=e[t];o=o+d;e=n[o];l[e[i]]=e[U];o=o+d;e=n[o];a=e[i]l[a]=l[a](s(l,a+d,e[u]))o=o+d;e=n[o];l[e[w]][e[U]]=l[e[M]];o=o+d;e=n[o];l[e[b]][e[t]]=e[N];o=o+d;e=n[o];l[e[r]]=f[e[U]];o=o+d;e=n[o];l[e[r]]=l[e[u]][e[P]];o=o+d;e=n[o];l[e[w]]=e[h];o=o+d;e=n[o];l[e[r]]=e[c];o=o+d;e=n[o];l[e[i]]=e[t];o=o+d;e=n[o];l[e[i]]=e[k];o=o+d;e=n[o];a=e[b]l[a]=l[a](s(l,a+d,e[U]))o=o+d;e=n[o];l[e[i]][e[U]]=l[e[M]];o=o+d;e=n[o];l[e[O]]=f[e[c]];o=o+d;e=n[o];l[e[r]]=l[e[t]][e[P]];o=o+d;e=n[o];l[e[w]]=e[U];o=o+d;e=n[o];l[e[w]]=e[t];o=o+d;e=n[o];l[e[x]]=e[h];o=o+d;e=n[o];l[e[i]]=e[h];o=o+d;e=n[o];a=e[O]l[a]=l[a](s(l,a+d,e[u]))o=o+d;e=n[o];l[e[b]][e[t]]=l[e[_]];o=o+d;e=n[o];l[e[r]]=f[e[t]];o=o+d;e=n[o];l[e[b]]=l[e[u]][e[P]];o=o+d;e=n[o];l[e[w]]=l[e[t]][e[N]];o=o+d;e=n[o];l[e[O]][e[h]]=l[e[P]];o=o+d;e=n[o];l[e[i]][e[u]]=e[D];o=o+d;e=n[o];l[e[O]]=f[e[h]];o=o+d;e=n[o];l[e[w]]=l[e[U]][e[N]];o=o+d;e=n[o];l[e[x]]=e[t];o=o+d;e=n[o];l[e[w]]=e[t];o=o+d;e=n[o];l[e[x]]=e[k];o=o+d;e=n[o];a=e[O]l[a]=l[a](s(l,a+d,e[u]))o=o+d;e=n[o];l[e[O]][e[c]]=l[e[_]];o=o+d;e=n[o];l[e[x]][e[k]]=e[_];o=o+d;e=n[o];l[e[r]][e[t]]=e[M];o=o+d;e=n[o];l[e[x]][e[k]]=e[P];o=o+d;e=n[o];l[e[b]][e[t]]=e[_];o=o+d;e=n[o];l[e[r]][e[U]]=l[e[D]];o=o+d;e=n[o];l[e[w]]=f[e[u]];o=o+d;e=n[o];l[e[i]]=l[e[h]][e[N]];o=o+d;e=n[o];l[e[i]]=e[t];o=o+d;e=n[o];l[e[b]]=e[k];o=o+d;e=n[o];l[e[x]]=e[k];break end while 1914==(a)/((133965/45))do l[e[O]]=#l[e[u]];break end;break;end break;end break;end break;end break;end while(a)/((-#'Fucking Retarted'+((1639301-819662)/243)))==1992 do a=(5886452)while C<=(-#"niggers"+(-68+102))do a-= a a=(2243836)while(5126/233)>=C do a-= a a=(1405854)while C<=(-#[[If LocalPlayer equals Dumbass then while true do end]]+(207-135))do a-= a a=(4569102)while C>(108-89)do a-= a l[e[x]]=l[e[k]]%e[P];break end while(a)/((((-110+11576)+-#"Faggot")/10))==3987 do l[e[r]]();break end;break;end while(a)/((380970/255))==941 do a=(2237950)while(147-126)<C do a-= a if(l[e[b]]~=e[B])then o=o+S;else o=e[t];end;break end while 3130==(a)/(((-35+775)+-#"cilerteddoesntlikeburgers"))do l[e[O]][e[U]]=l[e[P]];break end;break;end break;end while 1262==(a)/((3638-1860))do a=(5902074)while(1224/(-#[[mike litoris]]+(-41+104)))>=C do a-= a a=(795039)while C>(-56+79)do a-= a f[e[c]]=l[e[i]];break end while(a)/(((-66+2834)+-#[[anime is for fags]]))==289 do local e=e[b];local o=l[e];for e=e+1,g do F(o,l[e])end;break end;break;end while 2358==(a)/((370444/148))do a=(4528232)while C<=(174-149)do a-= a if(l[e[O]]~=l[e[D]])then o=o+S;else o=e[c];end;break;end while(a)/((4791-2435))==1922 do a=(14697207)while C>(44+-18)do a-= a l[e[x]]=A(v[e[t]],nil,f);break end while 3703==(a)/((-#[[big niggers sucking cock]]+((343516-171817)/43)))do l[e[b]][e[c]]=e[B];break end;break;end break;end break;end break;end while(a)/((3698-1894))==3263 do a=(1879346)while((200-156)+-#'cilertedcool')>=C do a-= a a=(4024143)while C<=(4988/172)do a-= a a=(707805)while C>(93-65)do a-= a local a;l[e[x]]=y[e[u]];o=o+d;e=n[o];l[e[w]]=l[e[k]][e[D]];o=o+d;e=n[o];l[e[i]]=l[e[c]][e[B]];o=o+d;e=n[o];l[e[b]]=l[e[t]][e[_]];o=o+d;e=n[o];l[e[i]][e[k]]=e[D];o=o+d;e=n[o];l[e[r]]=f[e[h]];o=o+d;e=n[o];l[e[i]]=y[e[c]];o=o+d;e=n[o];a=e[i]l[a](l[a+S])o=o+d;e=n[o];l[e[i]]=y[e[U]];o=o+d;e=n[o];l[e[w]]=l[e[k]][e[D]];o=o+d;e=n[o];l[e[i]][e[U]]=e[D];o=o+d;e=n[o];do return end;break end while 963==(a)/((1514-(1574-795)))do local a=e[x];local r=e[N];local n=a+2 local a={l[a](l[a+1],l[n])};for e=1,r do l[n+e]=a[e];end;local a=a[1]if a then l[n]=a o=e[h];else o=o+d;end;break end;break;end while(a)/((4264-2167))==1919 do a=(142174)while C<=(84-54)do a-= a l[e[r]]=l[e[h]]-l[e[D]];break;end while(a)/((((155+-51)+-#"impulse is hot")+-23))==2122 do a=(1147482)while(-126+157)<C do a-= a l[e[b]]=e[t];break end while 3903==(a)/((-#[[0nly was here mf]]+(((-1107/41)+-#'nicowashere')+348)))do local r;local a;a=e[x];r=l[e[h]];l[a+1]=r;l[a]=r[e[D]];o=o+d;e=n[o];l[e[O]]=e[k];o=o+d;e=n[o];a=e[w]l[a]=l[a](s(l,a+d,e[u]))o=o+d;e=n[o];l[e[i]]=l[e[t]][e[N]];o=o+d;e=n[o];a=e[O];r=l[e[h]];l[a+1]=r;l[a]=r[e[N]];break end;break;end break;end break;end while(a)/((-31+1809))==1057 do a=(293508)while C<=(84-50)do a-= a a=(5407820)while(-116+149)<C do a-= a l[e[w]]();break end while(a)/(((2131+-41)+-#"windows xp startup sfx"))==2615 do local a;f[e[h]]=l[e[O]];o=o+d;e=n[o];l[e[O]]=f[e[c]];o=o+d;e=n[o];l[e[b]]=l[e[h]][e[B]];o=o+d;e=n[o];l[e[w]]=e[u];o=o+d;e=n[o];a=e[x]l[a]=l[a](l[a+S])o=o+d;e=n[o];l[e[w]]=f[e[c]];o=o+d;e=n[o];l[e[r]]=l[e[h]][e[P]];o=o+d;e=n[o];l[e[w]]=e[h];o=o+d;e=n[o];a=e[O]l[a]=l[a](l[a+S])o=o+d;e=n[o];l[e[r]]=f[e[t]];o=o+d;e=n[o];l[e[r]]=l[e[c]][e[B]];o=o+d;e=n[o];l[e[O]]=e[u];o=o+d;e=n[o];a=e[b]l[a]=l[a](l[a+S])o=o+d;e=n[o];l[e[r]]=f[e[h]];o=o+d;e=n[o];l[e[i]]=l[e[k]][e[B]];o=o+d;e=n[o];l[e[x]]=e[h];o=o+d;e=n[o];a=e[b]l[a]=l[a](l[a+S])o=o+d;e=n[o];l[e[w]]=f[e[c]];o=o+d;e=n[o];l[e[b]]=l[e[k]][e[N]];o=o+d;e=n[o];l[e[b]]=e[t];o=o+d;e=n[o];a=e[r]l[a]=l[a](l[a+S])o=o+d;e=n[o];l[e[x]]=f[e[k]];o=o+d;e=n[o];l[e[b]]=l[e[t]][e[_]];o=o+d;e=n[o];l[e[O]]=e[k];o=o+d;e=n[o];a=e[i]l[a]=l[a](l[a+S])o=o+d;e=n[o];l[e[O]]=f[e[h]];o=o+d;e=n[o];l[e[i]]=l[e[U]][e[_]];o=o+d;e=n[o];l[e[O]]=e[t];o=o+d;e=n[o];a=e[r]l[a]=l[a](l[a+S])o=o+d;e=n[o];l[e[r]]=f[e[c]];o=o+d;e=n[o];l[e[i]]=l[e[U]][e[P]];o=o+d;e=n[o];l[e[i]]=e[c];o=o+d;e=n[o];a=e[O]l[a]=l[a](l[a+S])o=o+d;e=n[o];l[e[b]]=f[e[h]];o=o+d;e=n[o];l[e[r]]=l[e[t]][e[_]];o=o+d;e=n[o];l[e[x]]=e[t];o=o+d;e=n[o];a=e[O]l[a]=l[a](l[a+S])o=o+d;e=n[o];l[e[w]]=f[e[h]];o=o+d;e=n[o];l[e[i]]=l[e[c]][e[_]];o=o+d;e=n[o];l[e[i]]=e[t];o=o+d;e=n[o];a=e[r]l[a]=l[a](l[a+S])o=o+d;e=n[o];l[e[x]]=f[e[k]];o=o+d;e=n[o];l[e[O]]=l[e[k]][e[_]];o=o+d;e=n[o];l[e[x]]=e[h];o=o+d;e=n[o];a=e[O]l[a]=l[a](l[a+S])o=o+d;e=n[o];l[e[O]]=f[e[h]];o=o+d;e=n[o];l[e[i]]=l[e[h]][e[B]];o=o+d;e=n[o];l[e[r]]=e[u];o=o+d;e=n[o];a=e[w]l[a]=l[a](l[a+S])o=o+d;e=n[o];l[e[w]]=f[e[k]];o=o+d;e=n[o];l[e[w]]=l[e[U]][e[M]];o=o+d;e=n[o];l[e[O]]=e[U];o=o+d;e=n[o];a=e[x]l[a]=l[a](l[a+S])o=o+d;e=n[o];l[e[w]]=f[e[c]];o=o+d;e=n[o];l[e[r]]=l[e[t]][e[_]];o=o+d;e=n[o];l[e[x]]=e[h];o=o+d;e=n[o];a=e[x]l[a]=l[a](l[a+S])o=o+d;e=n[o];l[e[x]]=f[e[t]];o=o+d;e=n[o];l[e[i]]=l[e[u]][e[_]];o=o+d;e=n[o];l[e[r]]=e[h];o=o+d;e=n[o];a=e[w]l[a]=l[a](l[a+S])o=o+d;e=n[o];l[e[w]]=f[e[k]];o=o+d;e=n[o];l[e[i]]=l[e[k]][e[_]];o=o+d;e=n[o];l[e[w]]=e[t];o=o+d;e=n[o];a=e[x]l[a]=l[a](l[a+S])o=o+d;e=n[o];l[e[x]]=f[e[U]];o=o+d;e=n[o];l[e[w]]=l[e[t]][e[N]];o=o+d;e=n[o];l[e[r]]=e[u];o=o+d;e=n[o];a=e[i]l[a]=l[a](l[a+S])o=o+d;e=n[o];l[e[r]]=f[e[k]];o=o+d;e=n[o];l[e[i]]=l[e[h]][e[_]];o=o+d;e=n[o];l[e[i]]=e[c];o=o+d;e=n[o];a=e[O]l[a]=l[a](l[a+S])o=o+d;e=n[o];l[e[x]]=f[e[c]];o=o+d;e=n[o];l[e[r]]=l[e[c]][e[N]];o=o+d;e=n[o];l[e[i]]=e[h];o=o+d;e=n[o];a=e[w]l[a]=l[a](l[a+S])o=o+d;e=n[o];l[e[b]]=f[e[U]];o=o+d;e=n[o];l[e[w]]=l[e[k]][e[N]];o=o+d;e=n[o];l[e[O]]=e[c];break end;break;end while(a)/((-#[[impulse is hot]]+(100204/94)))==279 do a=(172640)while C<=((220-169)+-#'cruz pp is large')do a-= a local C;local p,S;local a;a=e[b]l[a]=l[a](s(l,a+d,e[c]))o=o+d;e=n[o];l[e[r]][e[u]]=l[e[B]];o=o+d;e=n[o];l[e[i]][e[U]]=e[D];o=o+d;e=n[o];l[e[w]]=f[e[u]];o=o+d;e=n[o];l[e[w]]=l[e[h]][e[M]];o=o+d;e=n[o];l[e[i]]=e[c];o=o+d;e=n[o];l[e[O]]=e[h];o=o+d;e=n[o];l[e[r]]=e[c];o=o+d;e=n[o];l[e[O]]=e[c];o=o+d;e=n[o];a=e[b]l[a]=l[a](s(l,a+d,e[k]))o=o+d;e=n[o];l[e[r]][e[U]]=l[e[_]];o=o+d;e=n[o];l[e[O]]=f[e[h]];o=o+d;e=n[o];l[e[i]]=l[e[u]][e[D]];o=o+d;e=n[o];l[e[i]]=e[u];o=o+d;e=n[o];l[e[O]]=e[t];o=o+d;e=n[o];l[e[w]]=e[u];o=o+d;e=n[o];l[e[b]]=e[k];o=o+d;e=n[o];a=e[x]l[a]=l[a](s(l,a+d,e[k]))o=o+d;e=n[o];l[e[O]][e[U]]=l[e[D]];o=o+d;e=n[o];l[e[r]][e[k]]=e[B];o=o+d;e=n[o];l[e[x]][e[h]]=l[e[_]];o=o+d;e=n[o];l[e[x]]=f[e[u]];o=o+d;e=n[o];l[e[i]]=l[e[h]][e[P]];o=o+d;e=n[o];l[e[O]]=e[t];o=o+d;e=n[o];l[e[w]]=e[u];o=o+d;e=n[o];l[e[r]]=e[t];o=o+d;e=n[o];a=e[w]l[a]=l[a](s(l,a+d,e[t]))o=o+d;e=n[o];l[e[b]][e[t]]=l[e[_]];o=o+d;e=n[o];l[e[i]]=f[e[h]];o=o+d;e=n[o];l[e[r]]=l[e[t]][e[M]];o=o+d;e=n[o];l[e[b]]=e[U];o=o+d;e=n[o];l[e[r]]=e[t];o=o+d;e=n[o];l[e[O]]=e[c];o=o+d;e=n[o];l[e[b]]=e[u];o=o+d;e=n[o];a=e[x]l[a]=l[a](s(l,a+d,e[h]))o=o+d;e=n[o];l[e[r]][e[c]]=l[e[D]];o=o+d;e=n[o];l[e[i]]=f[e[c]];o=o+d;e=n[o];l[e[r]]=l[e[k]][e[D]];o=o+d;e=n[o];l[e[x]]=e[u];o=o+d;e=n[o];l[e[O]]=e[c];o=o+d;e=n[o];l[e[x]]=e[U];o=o+d;e=n[o];l[e[r]]=e[t];o=o+d;e=n[o];a=e[i]l[a]=l[a](s(l,a+d,e[c]))o=o+d;e=n[o];l[e[w]][e[t]]=l[e[N]];o=o+d;e=n[o];l[e[w]][e[c]]=e[B];o=o+d;e=n[o];l[e[O]]=f[e[U]];o=o+d;e=n[o];l[e[w]]=l[e[u]][e[M]];o=o+d;e=n[o];l[e[x]]=l[e[c]][e[P]];o=o+d;e=n[o];l[e[w]][e[h]]=l[e[B]];o=o+d;e=n[o];l[e[i]][e[U]]=e[_];o=o+d;e=n[o];l[e[x]]=f[e[U]];o=o+d;e=n[o];l[e[r]]=l[e[h]][e[D]];o=o+d;e=n[o];l[e[w]]=e[U];o=o+d;e=n[o];l[e[r]]=e[U];o=o+d;e=n[o];l[e[w]]=e[U];o=o+d;e=n[o];a=e[x]l[a]=l[a](s(l,a+d,e[U]))o=o+d;e=n[o];l[e[O]][e[k]]=l[e[_]];o=o+d;e=n[o];l[e[O]][e[U]]=e[B];o=o+d;e=n[o];l[e[O]][e[k]]=e[_];o=o+d;e=n[o];l[e[x]][e[U]]=e[B];o=o+d;e=n[o];l[e[w]]=f[e[c]];o=o+d;e=n[o];l[e[b]]=l[e[c]][e[B]];o=o+d;e=n[o];l[e[w]]=e[c];o=o+d;e=n[o];l[e[b]]=e[h];o=o+d;e=n[o];a=e[r]l[a]=l[a](s(l,a+d,e[U]))o=o+d;e=n[o];l[e[x]][e[U]]=l[e[D]];o=o+d;e=n[o];l[e[O]][e[u]]=l[e[_]];o=o+d;e=n[o];l[e[r]]=f[e[h]];o=o+d;e=n[o];l[e[O]]=l[e[U]][e[_]];o=o+d;e=n[o];l[e[O]]={};o=o+d;e=n[o];l[e[x]]=f[e[k]];o=o+d;e=n[o];l[e[r]]=l[e[U]][e[_]];o=o+d;e=n[o];l[e[r]]=e[u];o=o+d;e=n[o];l[e[r]]=f[e[c]];o=o+d;e=n[o];l[e[x]]=l[e[u]][e[P]];o=o+d;e=n[o];l[e[i]]=e[t];o=o+d;e=n[o];l[e[i]]=e[u];o=o+d;e=n[o];l[e[i]]=e[t];o=o+d;e=n[o];a=e[b]p,S=m(l[a](s(l,a+1,e[c])))g=S+a-1 C=0;for e=a,g do C=C+d;l[e]=p[C];end;o=o+d;e=n[o];a=e[x]l[a]=l[a](s(l,a+d,g))break;end while(a)/(((217+-80)+-85))==3320 do a=(239820)while((167+-73)+-#[[papier der afghaner wurde von nice dem bombenleger gefickt]])<C do a-= a o=e[h];break end while(a)/((1180-609))==420 do local a;l[e[b]]=e[c];o=o+d;e=n[o];l[e[O]]=e[u];o=o+d;e=n[o];a=e[b]l[a]=l[a](s(l,a+d,e[k]))o=o+d;e=n[o];l[e[i]][e[k]]=l[e[_]];o=o+d;e=n[o];l[e[w]][e[u]]=e[_];o=o+d;e=n[o];l[e[x]][e[c]]=e[_];o=o+d;e=n[o];l[e[r]]=f[e[c]];o=o+d;e=n[o];l[e[i]]=l[e[u]][e[P]];o=o+d;e=n[o];l[e[O]]=e[k];o=o+d;e=n[o];l[e[w]]=e[h];o=o+d;e=n[o];a=e[x]l[a]=l[a](s(l,a+d,e[c]))o=o+d;e=n[o];l[e[x]][e[k]]=l[e[P]];o=o+d;e=n[o];l[e[r]][e[u]]=l[e[M]];o=o+d;e=n[o];l[e[O]][e[U]]=e[N];o=o+d;e=n[o];l[e[O]][e[u]]=l[e[_]];o=o+d;e=n[o];l[e[O]]=f[e[u]];o=o+d;e=n[o];l[e[O]]=l[e[c]][e[M]];o=o+d;e=n[o];l[e[x]]=e[k];o=o+d;e=n[o];l[e[O]]=e[k];o=o+d;e=n[o];l[e[w]]=e[h];o=o+d;e=n[o];a=e[i]l[a]=l[a](s(l,a+d,e[h]))o=o+d;e=n[o];l[e[x]][e[t]]=l[e[D]];o=o+d;e=n[o];l[e[i]][e[U]]=e[D];o=o+d;e=n[o];l[e[r]]=f[e[k]];o=o+d;e=n[o];l[e[O]]=l[e[k]][e[_]];o=o+d;e=n[o];l[e[x]]=e[U];o=o+d;e=n[o];l[e[x]]=e[t];o=o+d;e=n[o];l[e[b]]=e[c];o=o+d;e=n[o];a=e[w]l[a]=l[a](s(l,a+d,e[t]))o=o+d;e=n[o];l[e[x]][e[U]]=l[e[M]];o=o+d;e=n[o];l[e[b]]=f[e[k]];o=o+d;e=n[o];l[e[r]]=l[e[U]][e[P]];o=o+d;e=n[o];l[e[O]]=e[c];o=o+d;e=n[o];l[e[O]]=e[U];o=o+d;e=n[o];l[e[O]]=e[k];o=o+d;e=n[o];l[e[w]]=e[u];o=o+d;e=n[o];a=e[i]l[a]=l[a](s(l,a+d,e[k]))o=o+d;e=n[o];l[e[O]][e[t]]=l[e[D]];o=o+d;e=n[o];l[e[i]]=f[e[c]];o=o+d;e=n[o];l[e[x]]=l[e[u]][e[D]];o=o+d;e=n[o];l[e[w]]=e[U];o=o+d;e=n[o];l[e[b]]=e[t];o=o+d;e=n[o];l[e[O]]=e[U];o=o+d;e=n[o];l[e[O]]=e[k];o=o+d;e=n[o];a=e[r]l[a]=l[a](s(l,a+d,e[t]))o=o+d;e=n[o];l[e[x]][e[U]]=l[e[D]];o=o+d;e=n[o];l[e[w]]=f[e[u]];o=o+d;e=n[o];l[e[w]]=l[e[c]][e[P]];o=o+d;e=n[o];l[e[b]]=l[e[k]][e[B]];o=o+d;e=n[o];l[e[b]][e[u]]=l[e[B]];o=o+d;e=n[o];l[e[x]][e[c]]=e[P];o=o+d;e=n[o];l[e[b]]=f[e[U]];o=o+d;e=n[o];l[e[b]]=l[e[u]][e[M]];o=o+d;e=n[o];l[e[x]]=e[c];o=o+d;e=n[o];l[e[r]]=e[k];o=o+d;e=n[o];l[e[b]]=e[k];o=o+d;e=n[o];a=e[x]l[a]=l[a](s(l,a+d,e[c]))o=o+d;e=n[o];l[e[b]][e[c]]=l[e[P]];o=o+d;e=n[o];l[e[i]][e[u]]=e[B];o=o+d;e=n[o];l[e[w]][e[U]]=e[P];o=o+d;e=n[o];l[e[r]]=f[e[h]];o=o+d;e=n[o];l[e[O]]=l[e[h]][e[N]];o=o+d;e=n[o];l[e[w]]=e[U];o=o+d;e=n[o];l[e[i]]=e[h];o=o+d;e=n[o];a=e[x]l[a]=l[a](s(l,a+d,e[k]))o=o+d;e=n[o];l[e[x]][e[U]]=l[e[D]];o=o+d;e=n[o];l[e[O]][e[c]]=l[e[B]];o=o+d;e=n[o];l[e[r]][e[k]]=l[e[P]];o=o+d;e=n[o];l[e[b]]=f[e[k]];o=o+d;e=n[o];l[e[r]]=l[e[u]][e[N]];o=o+d;e=n[o];l[e[w]]=e[U];o=o+d;e=n[o];l[e[w]]=e[h];o=o+d;e=n[o];l[e[r]]=e[t];o=o+d;e=n[o];a=e[O]l[a]=l[a](s(l,a+d,e[k]))o=o+d;e=n[o];l[e[w]][e[t]]=l[e[M]];o=o+d;e=n[o];l[e[r]][e[t]]=e[M];o=o+d;e=n[o];l[e[r]]=f[e[U]];o=o+d;e=n[o];l[e[r]]=l[e[U]][e[P]];o=o+d;e=n[o];l[e[i]]=e[c];o=o+d;e=n[o];l[e[i]]=e[U];break end;break;end break;end break;end break;end break;end break;end while 3743==(a)/((5223-2649))do a=(2069440)while C<=((3900/50)+-#'windows xp startup sfx')do a-= a a=(508053)while(-95+141)>=C do a-= a a=(12528156)while C<=(-#"deadphonelua"+(169+-116))do a-= a a=(15818243)while C<=(9594/(59286/241))do a-= a a=(9723340)while(7524/(34650/175))<C do a-= a if not l[e[x]]then o=o+S;else o=e[U];end;break end while(a)/((5090-2571))==3860 do local a;l[e[w]]=e[h];o=o+d;e=n[o];l[e[b]]=e[u];o=o+d;e=n[o];a=e[x]l[a]=l[a](s(l,a+d,e[k]))o=o+d;e=n[o];l[e[r]][e[k]]=l[e[D]];o=o+d;e=n[o];l[e[O]]=f[e[t]];o=o+d;e=n[o];l[e[w]]=l[e[t]][e[_]];o=o+d;e=n[o];l[e[w]]=e[U];o=o+d;e=n[o];l[e[i]]=e[U];o=o+d;e=n[o];l[e[i]]=e[h];o=o+d;e=n[o];l[e[i]]=e[h];o=o+d;e=n[o];a=e[i]l[a]=l[a](s(l,a+d,e[U]))o=o+d;e=n[o];l[e[r]][e[c]]=l[e[D]];o=o+d;e=n[o];l[e[b]][e[c]]=e[P];o=o+d;e=n[o];l[e[w]][e[k]]=l[e[N]];o=o+d;e=n[o];l[e[b]]=f[e[u]];o=o+d;e=n[o];l[e[x]]=l[e[t]][e[P]];o=o+d;e=n[o];l[e[x]]=e[h];o=o+d;e=n[o];l[e[r]]=e[t];o=o+d;e=n[o];l[e[r]]=e[k];o=o+d;e=n[o];a=e[w]l[a]=l[a](s(l,a+d,e[t]))o=o+d;e=n[o];l[e[i]][e[h]]=l[e[M]];o=o+d;e=n[o];l[e[b]]=f[e[c]];o=o+d;e=n[o];l[e[r]]=l[e[c]][e[N]];o=o+d;e=n[o];l[e[O]]=e[k];o=o+d;e=n[o];l[e[r]]=e[t];o=o+d;e=n[o];l[e[x]]=e[h];o=o+d;e=n[o];a=e[x]l[a]=l[a](s(l,a+d,e[k]))o=o+d;e=n[o];l[e[r]][e[t]]=l[e[M]];o=o+d;e=n[o];l[e[r]][e[U]]=e[_];o=o+d;e=n[o];l[e[r]]=f[e[U]];o=o+d;e=n[o];l[e[w]]=l[e[u]][e[B]];o=o+d;e=n[o];l[e[x]]=e[h];o=o+d;e=n[o];l[e[i]]=e[c];o=o+d;e=n[o];l[e[x]]=e[k];o=o+d;e=n[o];l[e[b]]=e[t];o=o+d;e=n[o];a=e[w]l[a]=l[a](s(l,a+d,e[u]))o=o+d;e=n[o];l[e[r]][e[k]]=l[e[N]];o=o+d;e=n[o];l[e[w]]=f[e[U]];o=o+d;e=n[o];l[e[b]]=l[e[k]][e[B]];o=o+d;e=n[o];l[e[w]]=e[t];o=o+d;e=n[o];l[e[x]]=e[h];o=o+d;e=n[o];l[e[x]]=e[u];o=o+d;e=n[o];l[e[x]]=e[h];o=o+d;e=n[o];a=e[b]l[a]=l[a](s(l,a+d,e[k]))o=o+d;e=n[o];l[e[b]][e[k]]=l[e[_]];o=o+d;e=n[o];l[e[x]][e[k]]=e[P];o=o+d;e=n[o];l[e[b]][e[c]]=l[e[B]];o=o+d;e=n[o];l[e[w]]=f[e[c]];o=o+d;e=n[o];l[e[i]]=l[e[k]][e[D]];o=o+d;e=n[o];l[e[b]]=e[u];o=o+d;e=n[o];l[e[b]]=e[h];o=o+d;e=n[o];l[e[i]]=e[h];o=o+d;e=n[o];a=e[w]l[a]=l[a](s(l,a+d,e[c]))o=o+d;e=n[o];l[e[w]][e[c]]=l[e[D]];o=o+d;e=n[o];l[e[r]][e[c]]=e[M];o=o+d;e=n[o];l[e[r]]=f[e[h]];o=o+d;e=n[o];l[e[x]]=l[e[k]][e[M]];o=o+d;e=n[o];l[e[O]]=e[t];o=o+d;e=n[o];l[e[O]]=e[c];o=o+d;e=n[o];l[e[x]]=e[c];o=o+d;e=n[o];l[e[w]]=e[t];o=o+d;e=n[o];a=e[x]l[a]=l[a](s(l,a+d,e[U]))o=o+d;e=n[o];l[e[i]][e[u]]=l[e[B]];o=o+d;e=n[o];l[e[w]]=f[e[u]];o=o+d;e=n[o];l[e[x]]=l[e[k]][e[N]];o=o+d;e=n[o];l[e[b]]=e[u];o=o+d;e=n[o];l[e[i]]=e[U];o=o+d;e=n[o];l[e[r]]=e[U];o=o+d;e=n[o];l[e[r]]=e[u];o=o+d;e=n[o];a=e[b]l[a]=l[a](s(l,a+d,e[c]))o=o+d;e=n[o];l[e[w]][e[h]]=l[e[B]];o=o+d;e=n[o];l[e[w]]=f[e[t]];o=o+d;e=n[o];l[e[O]]=l[e[U]][e[P]];o=o+d;e=n[o];l[e[w]]=l[e[U]][e[B]];o=o+d;e=n[o];l[e[i]][e[c]]=l[e[N]];o=o+d;e=n[o];l[e[b]][e[c]]=e[N];o=o+d;e=n[o];l[e[b]]=f[e[h]];o=o+d;e=n[o];l[e[i]]=l[e[u]][e[N]];o=o+d;e=n[o];l[e[x]]=e[t];o=o+d;e=n[o];l[e[r]]=e[U];break end;break;end while 3899==(a)/((-#[[Gay porn]]+(573165/141)))do a=(75190)while(200-(432-272))<C do a-= a l[e[x]][l[e[U]]]=l[e[B]];break end while(a)/((1548-818))==103 do y[e[U]]=l[e[x]];break end;break;end break;end while(a)/((587964/156))==3324 do a=(294574)while(150-107)>=C do a-= a a=(5509152)while(139-97)<C do a-= a local a;a=e[x]l[a]=l[a](s(l,a+d,e[c]))o=o+d;e=n[o];l[e[w]][e[t]]=l[e[M]];o=o+d;e=n[o];l[e[O]]=f[e[k]];o=o+d;e=n[o];l[e[b]]=l[e[k]][e[N]];o=o+d;e=n[o];l[e[O]]=e[U];o=o+d;e=n[o];l[e[x]]=e[U];o=o+d;e=n[o];l[e[r]]=e[c];o=o+d;e=n[o];l[e[w]]=e[c];o=o+d;e=n[o];a=e[x]l[a]=l[a](s(l,a+d,e[c]))o=o+d;e=n[o];l[e[r]][e[k]]=l[e[M]];o=o+d;e=n[o];l[e[x]]=f[e[U]];o=o+d;e=n[o];l[e[r]]=l[e[t]][e[D]];o=o+d;e=n[o];l[e[r]]=e[k];o=o+d;e=n[o];l[e[O]]=e[c];o=o+d;e=n[o];l[e[i]]=e[t];o=o+d;e=n[o];l[e[O]]=e[t];o=o+d;e=n[o];a=e[O]l[a]=l[a](s(l,a+d,e[t]))o=o+d;e=n[o];l[e[i]][e[c]]=l[e[P]];o=o+d;e=n[o];l[e[b]]=f[e[u]];o=o+d;e=n[o];l[e[r]]=l[e[U]][e[_]];o=o+d;e=n[o];l[e[r]]=l[e[c]][e[D]];o=o+d;e=n[o];l[e[i]][e[U]]=l[e[B]];o=o+d;e=n[o];l[e[w]][e[c]]=e[M];o=o+d;e=n[o];l[e[x]]=f[e[t]];o=o+d;e=n[o];l[e[b]]=l[e[k]][e[_]];o=o+d;e=n[o];l[e[x]]=e[k];o=o+d;e=n[o];l[e[r]]=e[U];o=o+d;e=n[o];l[e[w]]=e[t];o=o+d;e=n[o];a=e[x]l[a]=l[a](s(l,a+d,e[c]))o=o+d;e=n[o];l[e[w]][e[u]]=l[e[D]];o=o+d;e=n[o];l[e[w]][e[h]]=e[N];o=o+d;e=n[o];l[e[O]][e[c]]=e[P];o=o+d;e=n[o];l[e[i]]=f[e[t]];o=o+d;e=n[o];l[e[b]]=l[e[k]][e[P]];o=o+d;e=n[o];l[e[O]]=e[k];o=o+d;e=n[o];l[e[O]]=e[c];o=o+d;e=n[o];a=e[w]l[a]=l[a](s(l,a+d,e[k]))o=o+d;e=n[o];l[e[w]][e[u]]=l[e[N]];o=o+d;e=n[o];l[e[w]][e[U]]=l[e[M]];o=o+d;e=n[o];l[e[r]][e[U]]=e[M];o=o+d;e=n[o];l[e[w]][e[t]]=l[e[N]];o=o+d;e=n[o];l[e[i]]=f[e[U]];o=o+d;e=n[o];l[e[i]]=l[e[c]][e[_]];o=o+d;e=n[o];l[e[O]]=e[u];o=o+d;e=n[o];l[e[O]]=e[t];o=o+d;e=n[o];l[e[r]]=e[t];o=o+d;e=n[o];a=e[i]l[a]=l[a](s(l,a+d,e[k]))o=o+d;e=n[o];l[e[i]][e[c]]=l[e[B]];o=o+d;e=n[o];l[e[x]][e[t]]=e[N];o=o+d;e=n[o];l[e[b]]=f[e[k]];o=o+d;e=n[o];l[e[w]]=l[e[t]][e[D]];o=o+d;e=n[o];l[e[r]]=e[U];o=o+d;e=n[o];l[e[w]]=e[U];o=o+d;e=n[o];l[e[r]]=e[t];o=o+d;e=n[o];a=e[w]l[a]=l[a](s(l,a+d,e[k]))o=o+d;e=n[o];l[e[O]][e[k]]=l[e[P]];o=o+d;e=n[o];l[e[O]]=f[e[U]];o=o+d;e=n[o];l[e[w]]=l[e[u]][e[B]];o=o+d;e=n[o];l[e[x]]=e[U];o=o+d;e=n[o];l[e[r]]=e[h];o=o+d;e=n[o];l[e[w]]=e[t];o=o+d;e=n[o];l[e[O]]=e[t];o=o+d;e=n[o];a=e[O]l[a]=l[a](s(l,a+d,e[h]))o=o+d;e=n[o];l[e[r]][e[c]]=l[e[_]];o=o+d;e=n[o];l[e[b]]=f[e[k]];o=o+d;e=n[o];l[e[O]]=l[e[c]][e[M]];o=o+d;e=n[o];l[e[i]]=e[t];o=o+d;e=n[o];l[e[i]]=e[c];o=o+d;e=n[o];l[e[b]]=e[k];o=o+d;e=n[o];l[e[x]]=e[k];o=o+d;e=n[o];a=e[x]l[a]=l[a](s(l,a+d,e[h]))o=o+d;e=n[o];l[e[b]][e[h]]=l[e[D]];o=o+d;e=n[o];l[e[w]]=f[e[h]];o=o+d;e=n[o];l[e[O]]=l[e[t]][e[B]];o=o+d;e=n[o];l[e[r]]=l[e[h]][e[D]];o=o+d;e=n[o];l[e[r]][e[h]]=l[e[P]];o=o+d;e=n[o];l[e[b]][e[h]]=e[D];o=o+d;e=n[o];l[e[r]]=f[e[c]];o=o+d;e=n[o];l[e[O]]=l[e[k]][e[N]];o=o+d;e=n[o];l[e[x]]=e[h];break end while(a)/((380512/184))==2664 do local r;local a;l[e[b]]=f[e[t]];o=o+d;e=n[o];l[e[O]]=l[e[h]][e[N]];o=o+d;e=n[o];l[e[O]]=e[t];o=o+d;e=n[o];l[e[O]]=y[e[k]];o=o+d;e=n[o];a=e[O]l[a]=l[a](s(l,a+d,e[t]))o=o+d;e=n[o];l[e[w]]=e[t];o=o+d;e=n[o];l[e[x]]=l[e[h]][e[B]];o=o+d;e=n[o];l[e[w]]=l[e[t]][e[P]];o=o+d;e=n[o];a=e[w];r=l[e[u]];l[a+1]=r;l[a]=r[e[_]];break end;break;end while 2779==(a)/((183+-77))do a=(2219189)while(-30+74)>=C do a-= a l[e[x]]=(e[h]~=0);o=o+S;break;end while(a)/(((713+-33)+-127))==4013 do a=(3324850)while(-#[[cilerteddoesntlikeburgers]]+(-57+127))<C do a-= a if not l[e[O]]then o=o+S;else o=e[k];end;break end while(a)/((307262/134))==1450 do local e=e[r]l[e]=l[e](s(l,e+d,g))break end;break;end break;end break;end break;end while 1861==(a)/(((6116/22)+-#'Negro'))do a=(10955700)while C<=(10200/200)do a-= a a=(2954610)while(5712/119)>=C do a-= a a=(1511430)while C>(126-79)do a-= a local a;l[e[b]][e[t]]=e[B];o=o+d;e=n[o];l[e[b]]=f[e[h]];o=o+d;e=n[o];l[e[w]]=l[e[c]][e[D]];o=o+d;e=n[o];l[e[r]]=e[k];o=o+d;e=n[o];l[e[w]]=e[k];o=o+d;e=n[o];l[e[b]]=e[k];o=o+d;e=n[o];l[e[i]]=e[t];o=o+d;e=n[o];a=e[b]l[a]=l[a](s(l,a+d,e[u]))o=o+d;e=n[o];l[e[w]][e[t]]=l[e[_]];o=o+d;e=n[o];l[e[i]]=f[e[t]];o=o+d;e=n[o];l[e[i]]=l[e[u]][e[P]];o=o+d;e=n[o];l[e[O]]=e[t];o=o+d;e=n[o];l[e[w]]=e[h];o=o+d;e=n[o];l[e[O]]=e[c];o=o+d;e=n[o];l[e[r]]=e[k];o=o+d;e=n[o];a=e[r]l[a]=l[a](s(l,a+d,e[k]))o=o+d;e=n[o];l[e[b]][e[c]]=l[e[N]];o=o+d;e=n[o];l[e[O]]=f[e[h]];o=o+d;e=n[o];l[e[r]]=l[e[h]][e[_]];o=o+d;e=n[o];l[e[b]]=l[e[h]][e[N]];o=o+d;e=n[o];l[e[b]][e[U]]=l[e[M]];o=o+d;e=n[o];l[e[i]][e[c]]=e[N];o=o+d;e=n[o];l[e[w]]=f[e[h]];o=o+d;e=n[o];l[e[b]]=l[e[h]][e[P]];o=o+d;e=n[o];l[e[w]]=e[u];o=o+d;e=n[o];l[e[w]]=e[U];o=o+d;e=n[o];l[e[x]]=e[u];o=o+d;e=n[o];a=e[i]l[a]=l[a](s(l,a+d,e[c]))o=o+d;e=n[o];l[e[b]][e[U]]=l[e[P]];o=o+d;e=n[o];l[e[w]][e[h]]=e[B];o=o+d;e=n[o];l[e[b]][e[t]]=e[_];o=o+d;e=n[o];l[e[r]][e[k]]=e[N];o=o+d;e=n[o];l[e[x]][e[k]]=l[e[_]];o=o+d;e=n[o];l[e[b]]=f[e[u]];o=o+d;e=n[o];l[e[x]]=l[e[k]][e[P]];o=o+d;e=n[o];l[e[x]]=e[k];o=o+d;e=n[o];l[e[O]]=e[h];o=o+d;e=n[o];l[e[r]]=e[k];o=o+d;e=n[o];a=e[r]l[a]=l[a](s(l,a+d,e[k]))o=o+d;e=n[o];l[e[r]][e[u]]=l[e[D]];o=o+d;e=n[o];l[e[r]][e[k]]=e[M];o=o+d;e=n[o];l[e[r]]=f[e[t]];o=o+d;e=n[o];l[e[r]]=l[e[u]][e[P]];o=o+d;e=n[o];l[e[x]]=e[h];o=o+d;e=n[o];l[e[r]]=e[t];o=o+d;e=n[o];l[e[w]]=e[t];o=o+d;e=n[o];a=e[O]l[a]=l[a](s(l,a+d,e[h]))o=o+d;e=n[o];l[e[b]][e[U]]=l[e[N]];o=o+d;e=n[o];l[e[b]][e[U]]=e[D];o=o+d;e=n[o];l[e[b]]=f[e[u]];o=o+d;e=n[o];l[e[b]]=l[e[u]][e[D]];o=o+d;e=n[o];l[e[w]]=e[k];o=o+d;e=n[o];l[e[x]]=e[k];o=o+d;e=n[o];l[e[i]]=e[U];o=o+d;e=n[o];l[e[x]]=e[k];o=o+d;e=n[o];a=e[r]l[a]=l[a](s(l,a+d,e[c]))o=o+d;e=n[o];l[e[i]][e[u]]=l[e[B]];o=o+d;e=n[o];l[e[i]]=f[e[c]];o=o+d;e=n[o];l[e[i]]=l[e[t]][e[P]];o=o+d;e=n[o];l[e[O]]=e[h];o=o+d;e=n[o];l[e[w]]=e[c];o=o+d;e=n[o];l[e[x]]=e[k];o=o+d;e=n[o];l[e[r]]=e[k];o=o+d;e=n[o];a=e[O]l[a]=l[a](s(l,a+d,e[k]))o=o+d;e=n[o];l[e[r]][e[h]]=l[e[B]];o=o+d;e=n[o];l[e[x]][e[h]]=e[B];o=o+d;e=n[o];l[e[x]][e[c]]=l[e[D]];o=o+d;e=n[o];l[e[b]]=f[e[u]];o=o+d;e=n[o];l[e[x]]=l[e[t]][e[B]];o=o+d;e=n[o];l[e[i]]=e[h];o=o+d;e=n[o];l[e[w]]=e[h];o=o+d;e=n[o];l[e[x]]=e[h];o=o+d;e=n[o];a=e[b]l[a]=l[a](s(l,a+d,e[k]))o=o+d;e=n[o];l[e[x]][e[U]]=l[e[M]];o=o+d;e=n[o];l[e[r]][e[h]]=e[_];o=o+d;e=n[o];l[e[b]]=f[e[u]];o=o+d;e=n[o];l[e[r]]=l[e[h]][e[N]];o=o+d;e=n[o];l[e[b]]=e[t];o=o+d;e=n[o];l[e[r]]=e[u];o=o+d;e=n[o];l[e[O]]=e[t];break end while 2490==(a)/(((2774-1433)-734))do local r;local a;l[e[x]]=f[e[h]];o=o+d;e=n[o];l[e[O]]=l[e[U]][e[N]];o=o+d;e=n[o];l[e[x]]=e[k];o=o+d;e=n[o];l[e[w]]=y[e[k]];o=o+d;e=n[o];a=e[x]l[a]=l[a](s(l,a+d,e[t]))o=o+d;e=n[o];l[e[b]]=l[e[c]][e[M]];o=o+d;e=n[o];l[e[O]]=l[e[k]][e[N]];o=o+d;e=n[o];a=e[O];r=l[e[h]];l[a+1]=r;l[a]=r[e[P]];break end;break;end while 2790==(a)/((2230-1171))do a=(1525608)while(735/15)>=C do a-= a local o=e[r]local n,e=m(l[o](s(l,o+1,e[h])))g=e+o-1 local e=0;for o=o,g do e=e+d;l[o]=n[e];end;break;end while 2018==(a)/((-#[[deadphonelua]]+(1645-877)))do a=(2997936)while C>(171-121)do a-= a local a;a=e[b]l[a]=l[a](s(l,a+d,e[u]))o=o+d;e=n[o];l[e[i]][e[k]]=l[e[N]];o=o+d;e=n[o];l[e[r]]=f[e[k]];o=o+d;e=n[o];l[e[r]]=l[e[k]][e[_]];o=o+d;e=n[o];l[e[b]]=e[c];o=o+d;e=n[o];l[e[b]]=e[c];o=o+d;e=n[o];l[e[r]]=e[h];o=o+d;e=n[o];l[e[i]]=e[t];o=o+d;e=n[o];a=e[r]l[a]=l[a](s(l,a+d,e[k]))o=o+d;e=n[o];l[e[i]][e[U]]=l[e[_]];o=o+d;e=n[o];l[e[w]]=f[e[c]];o=o+d;e=n[o];l[e[i]]=l[e[c]][e[_]];o=o+d;e=n[o];l[e[r]]=e[U];o=o+d;e=n[o];l[e[i]]=e[U];o=o+d;e=n[o];l[e[r]]=e[c];o=o+d;e=n[o];l[e[x]]=e[u];o=o+d;e=n[o];a=e[i]l[a]=l[a](s(l,a+d,e[t]))o=o+d;e=n[o];l[e[i]][e[u]]=l[e[N]];o=o+d;e=n[o];l[e[w]]=f[e[k]];o=o+d;e=n[o];l[e[b]]=l[e[U]][e[P]];o=o+d;e=n[o];l[e[O]]=l[e[c]][e[D]];o=o+d;e=n[o];l[e[O]][e[k]]=l[e[B]];o=o+d;e=n[o];l[e[w]][e[k]]=e[_];o=o+d;e=n[o];l[e[x]]=f[e[u]];o=o+d;e=n[o];l[e[i]]=l[e[c]][e[N]];o=o+d;e=n[o];l[e[r]]=e[U];o=o+d;e=n[o];l[e[O]]=e[h];o=o+d;e=n[o];l[e[w]]=e[h];o=o+d;e=n[o];a=e[O]l[a]=l[a](s(l,a+d,e[U]))o=o+d;e=n[o];l[e[w]][e[u]]=l[e[B]];o=o+d;e=n[o];l[e[w]][e[U]]=e[M];o=o+d;e=n[o];l[e[b]][e[u]]=e[D];o=o+d;e=n[o];l[e[x]]=f[e[t]];o=o+d;e=n[o];l[e[i]]=l[e[U]][e[P]];o=o+d;e=n[o];l[e[r]]=e[h];o=o+d;e=n[o];l[e[r]]=e[u];o=o+d;e=n[o];a=e[x]l[a]=l[a](s(l,a+d,e[h]))o=o+d;e=n[o];l[e[w]][e[h]]=l[e[_]];o=o+d;e=n[o];l[e[i]][e[h]]=l[e[_]];o=o+d;e=n[o];l[e[r]][e[c]]=e[N];o=o+d;e=n[o];l[e[i]][e[k]]=l[e[P]];o=o+d;e=n[o];l[e[O]]=f[e[h]];o=o+d;e=n[o];l[e[b]]=l[e[t]][e[M]];o=o+d;e=n[o];l[e[w]]=e[u];o=o+d;e=n[o];l[e[O]]=e[u];o=o+d;e=n[o];l[e[x]]=e[U];o=o+d;e=n[o];a=e[O]l[a]=l[a](s(l,a+d,e[U]))o=o+d;e=n[o];l[e[w]][e[t]]=l[e[_]];o=o+d;e=n[o];l[e[w]][e[h]]=e[N];o=o+d;e=n[o];l[e[r]]=f[e[h]];o=o+d;e=n[o];l[e[x]]=l[e[U]][e[M]];o=o+d;e=n[o];l[e[x]]=e[t];o=o+d;e=n[o];l[e[b]]=e[u];o=o+d;e=n[o];l[e[i]]=e[U];o=o+d;e=n[o];a=e[O]l[a]=l[a](s(l,a+d,e[t]))o=o+d;e=n[o];l[e[O]][e[c]]=l[e[_]];o=o+d;e=n[o];l[e[i]]=f[e[c]];o=o+d;e=n[o];l[e[x]]=l[e[U]][e[P]];o=o+d;e=n[o];l[e[x]]=e[c];o=o+d;e=n[o];l[e[b]]=e[h];o=o+d;e=n[o];l[e[i]]=e[t];o=o+d;e=n[o];l[e[x]]=e[u];o=o+d;e=n[o];a=e[x]l[a]=l[a](s(l,a+d,e[c]))o=o+d;e=n[o];l[e[i]][e[t]]=l[e[P]];o=o+d;e=n[o];l[e[w]]=f[e[c]];o=o+d;e=n[o];l[e[w]]=l[e[c]][e[B]];o=o+d;e=n[o];l[e[i]]=e[U];o=o+d;e=n[o];l[e[r]]=e[t];o=o+d;e=n[o];l[e[b]]=e[t];o=o+d;e=n[o];l[e[O]]=e[t];o=o+d;e=n[o];a=e[i]l[a]=l[a](s(l,a+d,e[U]))o=o+d;e=n[o];l[e[x]][e[t]]=l[e[D]];o=o+d;e=n[o];l[e[i]][e[c]]=e[B];o=o+d;e=n[o];l[e[b]]=f[e[U]];o=o+d;e=n[o];l[e[w]]=l[e[u]][e[_]];o=o+d;e=n[o];l[e[b]]=l[e[t]][e[M]];o=o+d;e=n[o];l[e[O]][e[U]]=l[e[N]];o=o+d;e=n[o];l[e[x]][e[U]]=e[M];o=o+d;e=n[o];l[e[w]]=f[e[h]];o=o+d;e=n[o];l[e[i]]=l[e[t]][e[P]];break end while(a)/((5324-2708))==1146 do local a;l[e[r]]=l[e[k]][e[M]];o=o+d;e=n[o];l[e[r]]=e[u];o=o+d;e=n[o];l[e[b]]=e[c];o=o+d;e=n[o];l[e[O]]=e[u];o=o+d;e=n[o];l[e[O]]=e[c];o=o+d;e=n[o];a=e[O]l[a]=l[a](s(l,a+d,e[t]))o=o+d;e=n[o];l[e[O]][e[h]]=l[e[B]];o=o+d;e=n[o];l[e[O]]=f[e[h]];o=o+d;e=n[o];l[e[O]]=l[e[h]][e[P]];o=o+d;e=n[o];l[e[O]]=e[h];o=o+d;e=n[o];l[e[w]]=e[k];o=o+d;e=n[o];l[e[r]]=e[u];o=o+d;e=n[o];l[e[w]]=e[u];o=o+d;e=n[o];a=e[x]l[a]=l[a](s(l,a+d,e[U]))o=o+d;e=n[o];l[e[O]][e[k]]=l[e[P]];o=o+d;e=n[o];l[e[i]]=f[e[c]];o=o+d;e=n[o];l[e[O]]=l[e[h]][e[N]];o=o+d;e=n[o];l[e[O]]=l[e[k]][e[P]];o=o+d;e=n[o];l[e[b]][e[t]]=l[e[M]];o=o+d;e=n[o];l[e[b]][e[t]]=e[D];o=o+d;e=n[o];l[e[b]]=f[e[u]];o=o+d;e=n[o];l[e[x]]=l[e[k]][e[M]];o=o+d;e=n[o];l[e[x]]=e[c];o=o+d;e=n[o];l[e[x]]=e[k];o=o+d;e=n[o];l[e[x]]=e[u];o=o+d;e=n[o];a=e[r]l[a]=l[a](s(l,a+d,e[t]))o=o+d;e=n[o];l[e[w]][e[u]]=l[e[N]];o=o+d;e=n[o];l[e[b]][e[t]]=e[N];o=o+d;e=n[o];l[e[i]][e[h]]=e[P];o=o+d;e=n[o];l[e[b]][e[u]]=e[N];o=o+d;e=n[o];l[e[r]][e[t]]=e[P];o=o+d;e=n[o];l[e[x]][e[c]]=l[e[N]];o=o+d;e=n[o];l[e[i]]=f[e[u]];o=o+d;e=n[o];l[e[x]]=l[e[t]][e[N]];o=o+d;e=n[o];l[e[b]]=e[u];o=o+d;e=n[o];l[e[w]]=e[u];o=o+d;e=n[o];l[e[b]]=e[c];o=o+d;e=n[o];a=e[x]l[a]=l[a](s(l,a+d,e[h]))o=o+d;e=n[o];l[e[i]][e[h]]=l[e[P]];o=o+d;e=n[o];l[e[i]][e[u]]=e[B];o=o+d;e=n[o];l[e[O]]=f[e[u]];o=o+d;e=n[o];l[e[b]]=l[e[c]][e[B]];o=o+d;e=n[o];l[e[r]]=e[U];o=o+d;e=n[o];l[e[b]]=e[k];o=o+d;e=n[o];l[e[i]]=e[k];o=o+d;e=n[o];l[e[r]]=e[h];o=o+d;e=n[o];a=e[O]l[a]=l[a](s(l,a+d,e[h]))o=o+d;e=n[o];l[e[i]][e[u]]=l[e[M]];o=o+d;e=n[o];l[e[i]]=f[e[c]];o=o+d;e=n[o];l[e[x]]=l[e[U]][e[D]];o=o+d;e=n[o];l[e[O]]=e[h];o=o+d;e=n[o];l[e[i]]=e[U];o=o+d;e=n[o];l[e[i]]=e[k];o=o+d;e=n[o];l[e[r]]=e[h];o=o+d;e=n[o];a=e[O]l[a]=l[a](s(l,a+d,e[u]))o=o+d;e=n[o];l[e[b]][e[k]]=l[e[P]];o=o+d;e=n[o];l[e[w]]=f[e[c]];o=o+d;e=n[o];l[e[i]]=l[e[k]][e[_]];o=o+d;e=n[o];l[e[w]]=l[e[c]][e[P]];o=o+d;e=n[o];l[e[b]][e[t]]=l[e[P]];o=o+d;e=n[o];l[e[x]][e[c]]=e[D];o=o+d;e=n[o];l[e[r]]=f[e[k]];o=o+d;e=n[o];l[e[x]]=l[e[t]][e[_]];o=o+d;e=n[o];l[e[x]]=e[c];o=o+d;e=n[o];l[e[r]]=e[c];o=o+d;e=n[o];l[e[x]]=e[h];o=o+d;e=n[o];a=e[x]l[a]=l[a](s(l,a+d,e[k]))o=o+d;e=n[o];l[e[x]][e[k]]=l[e[N]];o=o+d;e=n[o];l[e[O]][e[U]]=e[N];o=o+d;e=n[o];l[e[r]][e[t]]=e[M];o=o+d;e=n[o];l[e[O]][e[c]]=e[M];o=o+d;e=n[o];l[e[O]][e[h]]=e[N];o=o+d;e=n[o];l[e[i]][e[t]]=l[e[_]];o=o+d;e=n[o];l[e[O]]=f[e[k]];o=o+d;e=n[o];l[e[r]]=l[e[k]][e[_]];o=o+d;e=n[o];l[e[b]]=e[c];o=o+d;e=n[o];l[e[w]]=e[k];o=o+d;e=n[o];l[e[w]]=e[U];o=o+d;e=n[o];a=e[b]l[a]=l[a](s(l,a+d,e[k]))o=o+d;e=n[o];l[e[w]][e[u]]=l[e[M]];break end;break;end break;end break;end while 2775==(a)/((398748/101))do a=(6002034)while C<=(7897/149)do a-= a a=(38430)while(200-148)<C do a-= a local a;l[e[i]]=f[e[h]];o=o+d;e=n[o];l[e[i]]=l[e[h]][e[_]];o=o+d;e=n[o];l[e[r]]=l[e[k]];o=o+d;e=n[o];a=e[O]l[a]=l[a](l[a+S])o=o+d;e=n[o];l[e[x]]();break end while 61==(a)/((1371-741))do local g;local _;local C;local a;l[e[w]]=f[e[c]];o=o+d;e=n[o];l[e[r]]=l[e[U]][e[D]];o=o+d;e=n[o];a=e[w];C=l[e[t]];l[a+1]=C;l[a]=C[e[N]];o=o+d;e=n[o];l[e[r]]=l[e[k]];o=o+d;e=n[o];l[e[r]]=l[e[c]];o=o+d;e=n[o];a=e[i]l[a]=l[a](s(l,a+d,e[u]))o=o+d;e=n[o];a=e[b];C=l[e[h]];l[a+1]=C;l[a]=C[e[B]];o=o+d;e=n[o];a=e[O]l[a]=l[a](l[a+S])o=o+d;e=n[o];_={l,e};_[S][_[p][i]]=_[d][_[p][P]]+_[S][_[p][u]];o=o+d;e=n[o];l[e[r]]=l[e[U]]%e[P];o=o+d;e=n[o];a=e[x]l[a]=l[a](l[a+S])o=o+d;e=n[o];C=e[h];g=l[C]for e=C+1,e[M]do g=g..l[e];end;l[e[b]]=g;o=o+d;e=n[o];_={l,e};_[S][_[p][r]]=_[d][_[p][D]]+_[S][_[p][t]];o=o+d;e=n[o];l[e[i]]=l[e[U]]%e[N];break end;break;end while 2139==(a)/(((305424/108)+-#'windows xp startup sfx'))do a=(2219352)while C<=(195-141)do a-= a local i;local r;local a;l[e[w]]=e[c];o=o+d;e=n[o];l[e[w]]=e[u];o=o+d;e=n[o];l[e[w]]=#l[e[u]];o=o+d;e=n[o];l[e[O]]=e[U];o=o+d;e=n[o];a=e[b];r=l[a]i=l[a+2];if(i>0)then if(r>l[a+1])then o=e[t];else l[a+3]=r;end elseif(r<l[a+1])then o=e[u];else l[a+3]=r;end break;end while(a)/((696198/197))==628 do a=(5194588)while(4730/86)<C do a-= a l[e[r]]=l[e[t]];break end while 1559==(a)/((((-103+3568)+-#'0nly segc')+-124))do l[e[r]]=l[e[u]][l[e[N]]];break end;break;end break;end break;end break;end break;end while 1115==(a)/(((3774-1898)+-#"impulse was here omg"))do a=(190706)while((-118+195)+-#"nicowashere")>=C do a-= a a=(766104)while(11956/((45120/192)+-#[[psx real dupe steal all ur pets no joke]]))>=C do a-= a a=(5733540)while C<=((188-123)+-#[[mf stfu]])do a-= a a=(60720)while(127+-70)<C do a-= a local a;l[e[i]]=f[e[k]];o=o+d;e=n[o];l[e[O]]=e[U];o=o+d;e=n[o];a=e[i]l[a]=l[a](l[a+S])o=o+d;e=n[o];l[e[x]]();o=o+d;e=n[o];do return end;break end while(a)/((205-117))==690 do local d=e[O];local o=l[e[c]];l[d+1]=o;l[d]=o[e[N]];break end;break;end while(a)/(((-62+3251)+-#"Crackzzzz"))==1803 do a=(7527745)while((((27376/116)+-#'Nsrds GAYYYYAIAHAKAJAVAHAUA')-129)+-#"this is a meme string")>=C do a-= a local e=e[b]l[e](l[e+S])break;end while 4045==(a)/((-#"nicowashere"+(3851-1979)))do a=(1923219)while((10664+-104)/176)<C do a-= a local k;local a;l[e[i]]=y[e[U]];o=o+d;e=n[o];l[e[i]]=l[e[c]][e[N]];o=o+d;e=n[o];l[e[r]][e[t]]=e[B];o=o+d;e=n[o];l[e[b]]=y[e[u]];o=o+d;e=n[o];l[e[w]]=l[e[c]][e[_]];o=o+d;e=n[o];l[e[b]]=l[e[t]][e[B]];o=o+d;e=n[o];l[e[i]]=l[e[u]][e[B]];o=o+d;e=n[o];l[e[b]][e[h]]=e[P];o=o+d;e=n[o];l[e[r]]=f[e[c]];o=o+d;e=n[o];a=e[O];k=l[e[t]];l[a+1]=k;l[a]=k[e[_]];o=o+d;e=n[o];l[e[b]]=e[u];o=o+d;e=n[o];a=e[O]l[a]=l[a](s(l,a+d,e[c]))o=o+d;e=n[o];l[e[r]]=l[e[t]][e[P]];o=o+d;e=n[o];l[e[i]]=l[e[u]][e[D]];o=o+d;e=n[o];a=e[x];k=l[e[t]];l[a+1]=k;l[a]=k[e[B]];o=o+d;e=n[o];l[e[w]]=e[t];o=o+d;e=n[o];a=e[i]l[a](s(l,a+S,e[t]))o=o+d;e=n[o];do return end;break end while(a)/((-#'warboy hates you'+(-106+995)))==2203 do l[e[x]]=l[e[U]]-l[e[N]];break end;break;end break;end break;end while(a)/((586-353))==3288 do a=(2008818)while C<=(-#'papier ist ein kleiner schwanz lutscher'+(-84+186))do a-= a a=(5090493)while C>(7874/127)do a-= a local a;l[e[x]]=f[e[t]];o=o+d;e=n[o];l[e[x]]=l[e[u]][e[B]];o=o+d;e=n[o];l[e[b]]=l[e[t]];o=o+d;e=n[o];a=e[w]l[a]=l[a](l[a+S])o=o+d;e=n[o];l[e[O]]();break end while 2661==(a)/((3895-1982))do local e=e[x]local n,o=m(l[e](l[e+S]))g=o+e-d local o=0;for e=e,g do o=o+d;l[e]=n[o];end;break end;break;end while 642==(a)/((744702/((-17+259)+-#"nerd")))do a=(10500076)while C<=(149+-85)do a-= a if(l[e[i]]~=e[D])then o=o+S;else o=e[t];end;break;end while 3533==(a)/((6029-3057))do a=(445269)while(248-183)<C do a-= a local x;local a;l[e[i]]=f[e[u]];o=o+d;e=n[o];l[e[i]]=l[e[k]][e[P]];o=o+d;e=n[o];l[e[w]]=e[c];o=o+d;e=n[o];l[e[i]]=y[e[U]];o=o+d;e=n[o];a=e[r]l[a]=l[a](s(l,a+d,e[h]))o=o+d;e=n[o];l[e[i]]=l[e[c]][e[D]];o=o+d;e=n[o];l[e[r]]=l[e[k]][e[N]];o=o+d;e=n[o];a=e[r];x=l[e[c]];l[a+1]=x;l[a]=x[e[P]];break end while(a)/((-36+1477))==309 do local e={l,e};e[S][e[p][r]]=e[d][e[p][P]]+e[S][e[p][u]];break end;break;end break;end break;end break;end while(a)/(((2556+-117)+-#[[cilerteddoesntlikeburgers]]))==79 do a=(2372150)while C<=(5964/(177+-93))do a-= a a=(2494440)while C<=(181-113)do a-= a a=(1762100)while(258-191)<C do a-= a local r;local a;l[e[O]]=f[e[k]];o=o+d;e=n[o];l[e[x]]=l[e[U]][e[B]];o=o+d;e=n[o];l[e[x]]=e[h];o=o+d;e=n[o];l[e[x]]=y[e[h]];o=o+d;e=n[o];a=e[i]l[a]=l[a](s(l,a+d,e[c]))o=o+d;e=n[o];l[e[i]]=e[h];o=o+d;e=n[o];l[e[i]]=l[e[h]][e[D]];o=o+d;e=n[o];l[e[b]]=l[e[u]][e[M]];o=o+d;e=n[o];a=e[w];r=l[e[h]];l[a+1]=r;l[a]=r[e[M]];break end while 1052==(a)/((182575/(243-134)))do local h;local a;l[e[b]]=f[e[U]];o=o+d;e=n[o];l[e[r]]=f[e[c]];o=o+d;e=n[o];a=e[r];h=l[e[U]];l[a+1]=h;l[a]=h[e[B]];o=o+d;e=n[o];l[e[O]]=e[u];o=o+d;e=n[o];a=e[x]l[a]=l[a](s(l,a+d,e[k]))o=o+d;e=n[o];l[e[i]]=l[e[c]][e[P]];o=o+d;e=n[o];l[e[w]]=l[e[U]][e[_]];o=o+d;e=n[o];a=e[b]l[a]=l[a](l[a+S])o=o+d;e=n[o];l[e[b]]();o=o+d;e=n[o];do return end;break end;break;end while 1640==(a)/((1559+-38))do a=(1281550)while C<=((12325/145)+-#'warboy hates you')do a-= a l[e[w]]=A(v[e[t]],nil,f);break;end while 3550==(a)/((35739/(891/9)))do a=(2032418)while(136+-66)<C do a-= a local x;local t,k;local h;local a;l[e[b]]=f[e[U]];o=o+d;e=n[o];l[e[i]]=f[e[u]];o=o+d;e=n[o];a=e[b];h=l[e[c]];l[a+1]=h;l[a]=h[e[_]];o=o+d;e=n[o];l[e[w]]=e[c];o=o+d;e=n[o];a=e[w]t,k=m(l[a](s(l,a+1,e[u])))g=k+a-1 x=0;for e=a,g do x=x+d;l[e]=t[x];end;o=o+d;e=n[o];a=e[i]l[a]=l[a](s(l,a+d,g))o=o+d;e=n[o];l[e[r]]();o=o+d;e=n[o];do return end;break end while(a)/((-#[[big niggers sucking cock]]+(299022/114)))==782 do local w;local a;l[e[r]]=f[e[k]];o=o+d;e=n[o];l[e[b]]=l[e[u]][e[D]];o=o+d;e=n[o];l[e[x]]=e[c];o=o+d;e=n[o];l[e[O]]=y[e[t]];o=o+d;e=n[o];a=e[i]l[a]=l[a](s(l,a+d,e[h]))o=o+d;e=n[o];l[e[x]]=l[e[c]][e[D]];o=o+d;e=n[o];l[e[O]]=l[e[c]][e[D]];o=o+d;e=n[o];a=e[i];w=l[e[t]];l[a+1]=w;l[a]=w[e[B]];break end;break;end break;end break;end while 2090==(a)/(((1219+-60)+-#[[0nly 1337 smashed ur wap]]))do a=(5029310)while C<=(-83+156)do a-= a a=(4153128)while((1185/15)+-#"elbicho")<C do a-= a local a;a=e[r]l[a]=l[a](s(l,a+d,e[u]))o=o+d;e=n[o];l[e[x]][e[U]]=l[e[P]];o=o+d;e=n[o];l[e[r]][e[k]]=e[N];o=o+d;e=n[o];l[e[w]]=f[e[u]];o=o+d;e=n[o];l[e[O]]=l[e[k]][e[N]];o=o+d;e=n[o];l[e[b]]=e[c];o=o+d;e=n[o];l[e[i]]=e[h];o=o+d;e=n[o];l[e[b]]=e[c];o=o+d;e=n[o];l[e[b]]=e[U];o=o+d;e=n[o];a=e[r]l[a]=l[a](s(l,a+d,e[u]))o=o+d;e=n[o];l[e[b]][e[h]]=l[e[D]];o=o+d;e=n[o];l[e[x]]=f[e[k]];o=o+d;e=n[o];l[e[w]]=l[e[h]][e[P]];o=o+d;e=n[o];l[e[x]]=e[k];o=o+d;e=n[o];l[e[x]]=e[t];o=o+d;e=n[o];l[e[i]]=e[h];o=o+d;e=n[o];l[e[O]]=e[t];o=o+d;e=n[o];a=e[b]l[a]=l[a](s(l,a+d,e[h]))o=o+d;e=n[o];l[e[r]][e[u]]=l[e[B]];o=o+d;e=n[o];l[e[i]]=f[e[u]];o=o+d;e=n[o];l[e[w]]=l[e[h]][e[_]];o=o+d;e=n[o];l[e[i]]=l[e[t]][e[D]];o=o+d;e=n[o];l[e[O]][e[u]]=l[e[_]];o=o+d;e=n[o];l[e[r]][e[c]]=e[P];o=o+d;e=n[o];l[e[r]]=f[e[t]];o=o+d;e=n[o];l[e[i]]=l[e[U]][e[D]];o=o+d;e=n[o];l[e[x]]=e[k];o=o+d;e=n[o];l[e[r]]=e[t];o=o+d;e=n[o];l[e[b]]=e[t];o=o+d;e=n[o];a=e[w]l[a]=l[a](s(l,a+d,e[k]))o=o+d;e=n[o];l[e[x]][e[U]]=l[e[B]];o=o+d;e=n[o];l[e[w]][e[u]]=e[N];o=o+d;e=n[o];l[e[w]][e[c]]=e[P];o=o+d;e=n[o];l[e[b]][e[u]]=e[P];o=o+d;e=n[o];l[e[w]][e[h]]=e[N];o=o+d;e=n[o];l[e[b]][e[U]]=l[e[M]];o=o+d;e=n[o];l[e[b]]=f[e[k]];o=o+d;e=n[o];l[e[i]]=l[e[t]][e[N]];o=o+d;e=n[o];l[e[w]]=e[k];o=o+d;e=n[o];l[e[x]]=e[U];o=o+d;e=n[o];l[e[i]]=e[c];o=o+d;e=n[o];a=e[O]l[a]=l[a](s(l,a+d,e[c]))o=o+d;e=n[o];l[e[O]][e[u]]=l[e[D]];o=o+d;e=n[o];l[e[r]][e[k]]=e[_];o=o+d;e=n[o];l[e[r]]=f[e[c]];o=o+d;e=n[o];l[e[x]]=l[e[U]][e[M]];o=o+d;e=n[o];l[e[x]]=e[U];o=o+d;e=n[o];l[e[x]]=e[c];o=o+d;e=n[o];l[e[b]]=e[h];o=o+d;e=n[o];l[e[b]]=e[c];o=o+d;e=n[o];a=e[x]l[a]=l[a](s(l,a+d,e[U]))o=o+d;e=n[o];l[e[r]][e[U]]=l[e[M]];o=o+d;e=n[o];l[e[w]]=f[e[u]];o=o+d;e=n[o];l[e[r]]=l[e[u]][e[N]];o=o+d;e=n[o];l[e[b]]=e[c];o=o+d;e=n[o];l[e[x]]=e[t];o=o+d;e=n[o];l[e[O]]=e[u];o=o+d;e=n[o];l[e[O]]=e[U];o=o+d;e=n[o];a=e[b]l[a]=l[a](s(l,a+d,e[h]))o=o+d;e=n[o];l[e[w]][e[t]]=l[e[D]];o=o+d;e=n[o];l[e[r]]=f[e[t]];o=o+d;e=n[o];l[e[i]]=l[e[t]][e[D]];o=o+d;e=n[o];l[e[b]]=l[e[k]][e[D]];o=o+d;e=n[o];l[e[O]][e[U]]=l[e[M]];o=o+d;e=n[o];l[e[b]][e[c]]=e[M];o=o+d;e=n[o];l[e[x]]=f[e[t]];o=o+d;e=n[o];l[e[i]]=l[e[u]][e[N]];o=o+d;e=n[o];l[e[O]]=e[t];o=o+d;e=n[o];l[e[i]]=e[c];o=o+d;e=n[o];l[e[b]]=e[U];o=o+d;e=n[o];a=e[x]l[a]=l[a](s(l,a+d,e[u]))o=o+d;e=n[o];l[e[x]][e[u]]=l[e[D]];o=o+d;e=n[o];l[e[x]][e[U]]=e[P];o=o+d;e=n[o];l[e[x]][e[h]]=e[B];o=o+d;e=n[o];l[e[x]][e[t]]=e[N];o=o+d;e=n[o];l[e[O]][e[c]]=l[e[B]];o=o+d;e=n[o];l[e[O]]=f[e[u]];o=o+d;e=n[o];l[e[x]]=l[e[k]][e[B]];o=o+d;e=n[o];l[e[b]]=e[t];o=o+d;e=n[o];l[e[i]]=e[c];break end while(a)/((2595-1338))==3304 do local a=e[w];local r=e[_];local n=a+2 local a={l[a](l[a+1],l[n])};for e=1,r do l[n+e]=a[e];end;local a=a[1]if a then l[n]=a o=e[h];else o=o+d;end;break end;break;end while(a)/((2971-1541))==3517 do a=(7471422)while C<=(3256/(-114+158))do a-= a local a;l[e[O]]=f[e[c]];o=o+d;e=n[o];l[e[x]]=l[e[U]][e[_]];o=o+d;e=n[o];l[e[r]]=l[e[h]];o=o+d;e=n[o];a=e[i]l[a]=l[a](l[a+S])o=o+d;e=n[o];l[e[i]]();break;end while(a)/((5518-(5728-2919)))==2758 do a=(1895972)while(-#"if syn then haxor alert end"+(-68+170))<C do a-= a l[e[r]]=l[e[c]][l[e[M]]];break end while(a)/((5344-(2748+-30)))==722 do local a;l[e[b]][e[c]]=l[e[M]];o=o+d;e=n[o];l[e[i]]=f[e[c]];o=o+d;e=n[o];l[e[x]]=l[e[h]][e[_]];o=o+d;e=n[o];l[e[w]]=e[c];o=o+d;e=n[o];l[e[b]]=e[k];o=o+d;e=n[o];l[e[b]]=e[U];o=o+d;e=n[o];l[e[i]]=e[h];o=o+d;e=n[o];a=e[w]l[a]=l[a](s(l,a+d,e[u]))o=o+d;e=n[o];l[e[b]][e[h]]=l[e[M]];o=o+d;e=n[o];l[e[r]]=f[e[t]];o=o+d;e=n[o];l[e[i]]=l[e[c]][e[N]];o=o+d;e=n[o];l[e[i]]=e[t];o=o+d;e=n[o];l[e[r]]=e[c];o=o+d;e=n[o];l[e[i]]=e[c];o=o+d;e=n[o];l[e[b]]=e[c];o=o+d;e=n[o];a=e[x]l[a]=l[a](s(l,a+d,e[k]))o=o+d;e=n[o];l[e[O]][e[k]]=l[e[P]];o=o+d;e=n[o];l[e[O]]=f[e[U]];o=o+d;e=n[o];l[e[x]]=l[e[h]][e[_]];o=o+d;e=n[o];l[e[i]]=l[e[c]][e[_]];o=o+d;e=n[o];l[e[i]][e[k]]=l[e[N]];o=o+d;e=n[o];l[e[O]][e[U]]=e[M];o=o+d;e=n[o];l[e[r]]=f[e[t]];o=o+d;e=n[o];l[e[i]]=l[e[U]][e[P]];o=o+d;e=n[o];l[e[x]]=e[h];o=o+d;e=n[o];l[e[x]]=e[t];o=o+d;e=n[o];l[e[O]]=e[k];o=o+d;e=n[o];a=e[b]l[a]=l[a](s(l,a+d,e[t]))o=o+d;e=n[o];l[e[b]][e[u]]=l[e[D]];o=o+d;e=n[o];l[e[w]][e[k]]=e[D];o=o+d;e=n[o];l[e[b]][e[c]]=e[M];o=o+d;e=n[o];l[e[w]]=f[e[h]];o=o+d;e=n[o];l[e[w]]=l[e[u]][e[D]];o=o+d;e=n[o];l[e[b]]=e[t];o=o+d;e=n[o];l[e[O]]=e[U];o=o+d;e=n[o];a=e[x]l[a]=l[a](s(l,a+d,e[c]))o=o+d;e=n[o];l[e[w]][e[c]]=l[e[D]];o=o+d;e=n[o];l[e[x]][e[u]]=l[e[D]];o=o+d;e=n[o];l[e[O]][e[c]]=e[D];o=o+d;e=n[o];l[e[O]][e[U]]=l[e[N]];o=o+d;e=n[o];l[e[x]]=f[e[t]];o=o+d;e=n[o];l[e[b]]=l[e[k]][e[_]];o=o+d;e=n[o];l[e[w]]=e[U];o=o+d;e=n[o];l[e[b]]=e[u];o=o+d;e=n[o];l[e[x]]=e[h];o=o+d;e=n[o];a=e[r]l[a]=l[a](s(l,a+d,e[h]))o=o+d;e=n[o];l[e[b]][e[c]]=l[e[D]];o=o+d;e=n[o];l[e[i]][e[t]]=e[D];o=o+d;e=n[o];l[e[b]]=f[e[U]];o=o+d;e=n[o];l[e[i]]=l[e[u]][e[N]];o=o+d;e=n[o];l[e[x]]=e[k];o=o+d;e=n[o];l[e[i]]=e[U];o=o+d;e=n[o];l[e[i]]=e[k];o=o+d;e=n[o];a=e[b]l[a]=l[a](s(l,a+d,e[h]))o=o+d;e=n[o];l[e[O]][e[k]]=l[e[B]];o=o+d;e=n[o];l[e[O]]=f[e[k]];o=o+d;e=n[o];l[e[i]]=l[e[k]][e[D]];o=o+d;e=n[o];l[e[i]]=e[c];o=o+d;e=n[o];l[e[r]]=e[k];o=o+d;e=n[o];l[e[O]]=e[k];o=o+d;e=n[o];l[e[i]]=e[k];o=o+d;e=n[o];a=e[b]l[a]=l[a](s(l,a+d,e[t]))o=o+d;e=n[o];l[e[r]][e[u]]=l[e[B]];o=o+d;e=n[o];l[e[w]]=f[e[t]];o=o+d;e=n[o];l[e[r]]=l[e[U]][e[N]];o=o+d;e=n[o];l[e[w]]=e[u];o=o+d;e=n[o];l[e[r]]=e[u];o=o+d;e=n[o];l[e[O]]=e[k];o=o+d;e=n[o];l[e[i]]=e[U];o=o+d;e=n[o];a=e[i]l[a]=l[a](s(l,a+d,e[u]))o=o+d;e=n[o];l[e[i]][e[h]]=l[e[D]];o=o+d;e=n[o];l[e[i]][e[k]]=e[N];o=o+d;e=n[o];l[e[b]]=f[e[h]];o=o+d;e=n[o];l[e[r]]=l[e[u]][e[P]];o=o+d;e=n[o];l[e[r]]=l[e[c]][e[_]];o=o+d;e=n[o];l[e[b]][e[u]]=l[e[N]];o=o+d;e=n[o];l[e[r]][e[k]]=e[P];o=o+d;e=n[o];l[e[w]]=f[e[t]];o=o+d;e=n[o];l[e[x]]=l[e[U]][e[P]];o=o+d;e=n[o];l[e[r]]=e[t];break end;break;end break;end break;end break;end break;end break;end break;end while 238==(a)/(((891-488)+-#"Impulse youtube real"))do a=(5867680)while((-19+158)+-#"cilerteddoesntlikeburgers")>=C do a-= a a=(91200)while C<=(19760/208)do a-= a a=(6764870)while(((-116+21642)/229)+-#'Deezbutts')>=C do a-= a a=(2360370)while(-#"warboy hates you"+(223-127))>=C do a-= a a=(9568020)while(-20+98)>=C do a-= a a=(1892000)while(15477/201)<C do a-= a local t;local _,u;local a;l[e[x]]=f[e[k]];o=o+d;e=n[o];l[e[O]]=l[e[h]][e[P]];o=o+d;e=n[o];l[e[i]]=e[U];o=o+d;e=n[o];l[e[r]]=f[e[h]];o=o+d;e=n[o];l[e[b]]=l[e[c]][e[B]];o=o+d;e=n[o];l[e[r]]=e[h];o=o+d;e=n[o];l[e[w]]=e[k];o=o+d;e=n[o];l[e[i]]=e[U];o=o+d;e=n[o];a=e[r]_,u=m(l[a](s(l,a+1,e[c])))g=u+a-1 t=0;for e=a,g do t=t+d;l[e]=_[t];end;o=o+d;e=n[o];a=e[b]_,u=m(l[a](s(l,a+d,g)))g=u+a-S t=0;for e=a,g do t=t+d;l[e]=_[t];end;break end while(a)/(((324276/183)+-#'deadphonelua'))==1075 do if(l[e[b]]==l[e[D]])then o=o+S;else o=e[h];end;break end;break;end while(a)/((-#'0nly segc'+(282960/90)))==3052 do a=(2291040)while(-#[[deadphonelua]]+(259-168))<C do a-= a local o=e[x]l[o]=l[o](s(l,o+d,e[U]))break end while(a)/(((375984/126)+-#'big niggers sucking cock'))==774 do local d=e[w];local a=l[d+2];local n=l[d]+a;l[d]=n;if(a>0)then if(n<=l[d+1])then o=e[U];l[d+3]=n;end elseif(n>=l[d+1])then o=e[u];l[d+3]=n;end break end;break;end break;end while(a)/((-31+3926))==606 do a=(1647954)while C<=(-#'big niggers sucking cock'+(236-(2600/20)))do a-= a a=(11821821)while C>(9153/((377-252)+-#"Lana Rhoades"))do a-= a l[e[b]]=y[e[k]];break end while 3369==(a)/(((7223-3649)+-65))do local e=e[r]local n,o=m(l[e](s(l,e+d,g)))g=o+e-S local o=0;for e=e,g do o=o+d;l[e]=n[o];end;break end;break;end while(a)/((189486/198))==1722 do a=(1004856)while C<=(-116+199)do a-= a local a;a=e[O]l[a]=l[a](s(l,a+d,e[k]))o=o+d;e=n[o];l[e[O]][e[t]]=l[e[M]];o=o+d;e=n[o];l[e[w]][e[c]]=e[P];o=o+d;e=n[o];l[e[i]][e[h]]=e[P];o=o+d;e=n[o];l[e[r]][e[u]]=e[N];o=o+d;e=n[o];l[e[b]][e[U]]=e[D];o=o+d;e=n[o];l[e[w]][e[u]]=l[e[P]];o=o+d;e=n[o];l[e[w]]=f[e[h]];o=o+d;e=n[o];l[e[r]]=l[e[t]][e[B]];o=o+d;e=n[o];l[e[r]]=e[t];o=o+d;e=n[o];l[e[i]]=e[U];o=o+d;e=n[o];l[e[i]]=e[c];o=o+d;e=n[o];a=e[w]l[a]=l[a](s(l,a+d,e[c]))o=o+d;e=n[o];l[e[w]][e[h]]=l[e[B]];o=o+d;e=n[o];l[e[x]]=f[e[U]];o=o+d;e=n[o];l[e[r]]=l[e[t]][e[_]];o=o+d;e=n[o];l[e[r]]=e[k];o=o+d;e=n[o];l[e[r]]=e[h];o=o+d;e=n[o];l[e[b]]=e[k];o=o+d;e=n[o];a=e[r]l[a]=l[a](s(l,a+d,e[h]))o=o+d;e=n[o];l[e[x]][e[c]]=l[e[M]];o=o+d;e=n[o];l[e[w]][e[t]]=e[D];o=o+d;e=n[o];l[e[O]]=f[e[u]];o=o+d;e=n[o];l[e[i]]=l[e[h]][e[B]];o=o+d;e=n[o];l[e[r]]=e[t];o=o+d;e=n[o];l[e[r]]=e[u];o=o+d;e=n[o];l[e[x]]=e[h];o=o+d;e=n[o];l[e[i]]=e[h];o=o+d;e=n[o];a=e[O]l[a]=l[a](s(l,a+d,e[U]))o=o+d;e=n[o];l[e[b]][e[h]]=l[e[_]];o=o+d;e=n[o];l[e[w]]=f[e[c]];o=o+d;e=n[o];l[e[w]]=l[e[u]][e[_]];o=o+d;e=n[o];l[e[x]]=e[U];o=o+d;e=n[o];l[e[x]]=e[k];o=o+d;e=n[o];l[e[w]]=e[c];o=o+d;e=n[o];l[e[x]]=e[c];o=o+d;e=n[o];a=e[w]l[a]=l[a](s(l,a+d,e[h]))o=o+d;e=n[o];l[e[x]][e[U]]=l[e[D]];o=o+d;e=n[o];l[e[b]][e[h]]=e[M];o=o+d;e=n[o];l[e[b]][e[t]]=l[e[P]];o=o+d;e=n[o];l[e[O]]=f[e[h]];o=o+d;e=n[o];l[e[w]]=l[e[c]][e[_]];o=o+d;e=n[o];l[e[b]]=e[c];o=o+d;e=n[o];l[e[w]]=e[U];o=o+d;e=n[o];l[e[i]]=e[k];o=o+d;e=n[o];a=e[i]l[a]=l[a](s(l,a+d,e[t]))o=o+d;e=n[o];l[e[w]][e[U]]=l[e[P]];o=o+d;e=n[o];l[e[i]][e[u]]=e[_];o=o+d;e=n[o];l[e[b]]=f[e[t]];o=o+d;e=n[o];l[e[O]]=l[e[t]][e[M]];o=o+d;e=n[o];l[e[b]]=e[U];o=o+d;e=n[o];l[e[i]]=e[t];o=o+d;e=n[o];l[e[x]]=e[k];o=o+d;e=n[o];l[e[x]]=e[u];o=o+d;e=n[o];a=e[r]l[a]=l[a](s(l,a+d,e[U]))o=o+d;e=n[o];l[e[b]][e[h]]=l[e[P]];o=o+d;e=n[o];l[e[w]]=f[e[c]];o=o+d;e=n[o];l[e[b]]=l[e[u]][e[D]];o=o+d;e=n[o];l[e[r]]=e[c];o=o+d;e=n[o];l[e[i]]=e[u];o=o+d;e=n[o];l[e[x]]=e[c];o=o+d;e=n[o];l[e[w]]=e[u];o=o+d;e=n[o];a=e[O]l[a]=l[a](s(l,a+d,e[k]))o=o+d;e=n[o];l[e[b]][e[U]]=l[e[D]];o=o+d;e=n[o];l[e[r]]=f[e[h]];o=o+d;e=n[o];l[e[b]]=l[e[c]][e[M]];o=o+d;e=n[o];l[e[b]]=l[e[c]][e[P]];o=o+d;e=n[o];l[e[r]][e[c]]=l[e[N]];o=o+d;e=n[o];l[e[r]][e[c]]=e[N];o=o+d;e=n[o];l[e[r]]=f[e[u]];o=o+d;e=n[o];l[e[r]]=l[e[U]][e[P]];o=o+d;e=n[o];l[e[O]]=e[k];o=o+d;e=n[o];l[e[i]]=e[u];o=o+d;e=n[o];l[e[r]]=e[k];o=o+d;e=n[o];a=e[i]l[a]=l[a](s(l,a+d,e[h]))o=o+d;e=n[o];l[e[r]][e[t]]=l[e[P]];o=o+d;e=n[o];l[e[x]][e[U]]=e[D];o=o+d;e=n[o];l[e[i]][e[h]]=e[_];o=o+d;e=n[o];l[e[x]][e[t]]=e[B];o=o+d;e=n[o];l[e[w]][e[k]]=e[M];break;end while(a)/(((-59+672)+-#'Impulse real 2022'))==1686 do a=(2749500)while((127+-27)+-#'0nly was here mf')<C do a-= a local r;local k,U;local w;local a;l[e[x]]=f[e[t]];o=o+d;e=n[o];l[e[O]]=f[e[c]];o=o+d;e=n[o];a=e[b];w=l[e[t]];l[a+1]=w;l[a]=w[e[P]];o=o+d;e=n[o];l[e[x]]=e[t];o=o+d;e=n[o];a=e[i]k,U=m(l[a](s(l,a+1,e[h])))g=U+a-1 r=0;for e=a,g do r=r+d;l[e]=k[r];end;o=o+d;e=n[o];a=e[x]l[a]=l[a](s(l,a+d,g))o=o+d;e=n[o];l[e[i]]();o=o+d;e=n[o];do return end;break end while(a)/((-118+1743))==1692 do local w;local a;l[e[r]]=f[e[t]];o=o+d;e=n[o];l[e[x]]=l[e[u]][e[D]];o=o+d;e=n[o];l[e[O]]=e[c];o=o+d;e=n[o];l[e[i]]=y[e[h]];o=o+d;e=n[o];a=e[r]l[a]=l[a](s(l,a+d,e[t]))o=o+d;e=n[o];l[e[i]]=l[e[t]][e[P]];o=o+d;e=n[o];l[e[b]]=l[e[t]][e[M]];o=o+d;e=n[o];a=e[x];w=l[e[t]];l[a+1]=w;l[a]=w[e[D]];break end;break;end break;end break;end break;end while(a)/((4106+-96))==1687 do a=(1788416)while C<=(163+-73)do a-= a a=(8896446)while(122+(-#'Gay porn'+(9+-36)))>=C do a-= a a=(9221655)while(118+-32)<C do a-= a l[e[r]]=y[e[U]];o=o+d;e=n[o];l[e[x]]=#l[e[k]];o=o+d;e=n[o];y[e[c]]=l[e[w]];o=o+d;e=n[o];l[e[O]]=y[e[u]];o=o+d;e=n[o];l[e[i]]=#l[e[U]];o=o+d;e=n[o];y[e[h]]=l[e[r]];o=o+d;e=n[o];do return end;break end while 2631==(a)/((-45+3550))do l[e[b]]=(e[k]~=0);break end;break;end while(a)/((282555/105))==3306 do a=(2524473)while C<=(-#"how to join the kkk"+(200+-93))do a-= a f[e[t]]=l[e[x]];o=o+d;e=n[o];l[e[r]]={};o=o+d;e=n[o];l[e[w]]={};o=o+d;e=n[o];f[e[t]]=l[e[w]];o=o+d;e=n[o];l[e[r]]=f[e[U]];o=o+d;e=n[o];if(l[e[O]]~=e[D])then o=o+S;else o=e[u];end;break;end while 2109==(a)/((2416-1219))do a=(989168)while C>((268-174)+-#[[Negro]])do a-= a local c;local w,t;local b;local a;l[e[x]]=f[e[u]];o=o+d;e=n[o];l[e[i]]=f[e[h]];o=o+d;e=n[o];a=e[i];b=l[e[h]];l[a+1]=b;l[a]=b[e[B]];o=o+d;e=n[o];l[e[i]]=e[h];o=o+d;e=n[o];l[e[i]]=(e[k]~=0);o=o+d;e=n[o];a=e[i]w,t=m(l[a](s(l,a+1,e[U])))g=t+a-1 c=0;for e=a,g do c=c+d;l[e]=w[c];end;o=o+d;e=n[o];a=e[i]l[a]=l[a](s(l,a+d,g))o=o+d;e=n[o];l[e[r]]();o=o+d;e=n[o];do return end;break end while 3376==(a)/(((722-381)+-#[[never gonna give you up never gonna let you down]]))do do return end;break end;break;end break;end break;end while 512==(a)/((7107-3614))do a=(3287440)while C<=(-#[[0nly segc]]+(-53+154))do a-= a a=(897390)while(((-35+252)+-#[[panzerfaust]])-115)<C do a-= a local i;local b,w;local h;local a;l[e[r]]=f[e[u]];o=o+d;e=n[o];l[e[O]]=f[e[U]];o=o+d;e=n[o];a=e[r];h=l[e[c]];l[a+1]=h;l[a]=h[e[N]];o=o+d;e=n[o];l[e[O]]=e[u];o=o+d;e=n[o];a=e[x]b,w=m(l[a](s(l,a+1,e[U])))g=w+a-1 i=0;for e=a,g do i=i+d;l[e]=b[i];end;o=o+d;e=n[o];a=e[r]l[a]=l[a](s(l,a+d,g))o=o+d;e=n[o];l[e[O]]();o=o+d;e=n[o];do return end;break end while(a)/((15210/30))==1770 do l[e[w]]=y[e[u]];break end;break;end while(a)/((76960/74))==3161 do a=(4107705)while(208+-115)>=C do a-= a l[e[b]]=l[e[h]][e[B]];break;end while 3857==(a)/((2162-1097))do a=(2343112)while(-124+218)<C do a-= a local a;l[e[b]]=e[h];o=o+d;e=n[o];l[e[x]]=e[h];o=o+d;e=n[o];l[e[r]]=e[u];o=o+d;e=n[o];a=e[i]l[a]=l[a](s(l,a+d,e[u]))o=o+d;e=n[o];l[e[O]][e[c]]=l[e[M]];o=o+d;e=n[o];l[e[i]]=f[e[k]];o=o+d;e=n[o];l[e[b]]=l[e[t]][e[B]];o=o+d;e=n[o];l[e[b]]=e[U];o=o+d;e=n[o];l[e[O]]=e[c];o=o+d;e=n[o];l[e[w]]=e[U];o=o+d;e=n[o];l[e[b]]=e[c];o=o+d;e=n[o];a=e[x]l[a]=l[a](s(l,a+d,e[c]))o=o+d;e=n[o];l[e[b]][e[u]]=l[e[P]];o=o+d;e=n[o];l[e[i]]=f[e[t]];o=o+d;e=n[o];l[e[i]]=l[e[u]][e[P]];o=o+d;e=n[o];l[e[x]]=l[e[k]][e[B]];o=o+d;e=n[o];l[e[O]][e[u]]=l[e[B]];o=o+d;e=n[o];l[e[b]][e[c]]=e[B];o=o+d;e=n[o];l[e[O]]=f[e[h]];o=o+d;e=n[o];l[e[x]]=l[e[U]][e[_]];o=o+d;e=n[o];l[e[i]]=e[U];o=o+d;e=n[o];l[e[x]]=e[c];o=o+d;e=n[o];l[e[b]]=e[c];o=o+d;e=n[o];a=e[O]l[a]=l[a](s(l,a+d,e[c]))o=o+d;e=n[o];l[e[w]][e[k]]=l[e[M]];o=o+d;e=n[o];l[e[r]][e[t]]=e[_];o=o+d;e=n[o];l[e[w]][e[c]]=e[D];o=o+d;e=n[o];l[e[x]][e[c]]=e[_];o=o+d;e=n[o];l[e[x]][e[t]]=e[B];o=o+d;e=n[o];l[e[x]][e[k]]=l[e[N]];o=o+d;e=n[o];l[e[i]]=f[e[k]];o=o+d;e=n[o];l[e[r]]=l[e[h]][e[_]];o=o+d;e=n[o];l[e[b]]=e[k];o=o+d;e=n[o];l[e[r]]=e[u];o=o+d;e=n[o];l[e[r]]=e[h];o=o+d;e=n[o];a=e[w]l[a]=l[a](s(l,a+d,e[c]))o=o+d;e=n[o];l[e[i]][e[U]]=l[e[B]];o=o+d;e=n[o];l[e[w]][e[c]]=e[M];o=o+d;e=n[o];l[e[b]]=f[e[U]];o=o+d;e=n[o];l[e[b]]=l[e[u]][e[P]];o=o+d;e=n[o];l[e[r]]=e[u];o=o+d;e=n[o];l[e[i]]=e[t];o=o+d;e=n[o];l[e[b]]=e[h];o=o+d;e=n[o];l[e[x]]=e[u];o=o+d;e=n[o];a=e[O]l[a]=l[a](s(l,a+d,e[u]))o=o+d;e=n[o];l[e[x]][e[U]]=l[e[M]];o=o+d;e=n[o];l[e[b]]=f[e[k]];o=o+d;e=n[o];l[e[x]]=l[e[U]][e[_]];o=o+d;e=n[o];l[e[w]]=e[h];o=o+d;e=n[o];l[e[b]]=e[t];o=o+d;e=n[o];l[e[r]]=e[t];o=o+d;e=n[o];l[e[b]]=e[h];o=o+d;e=n[o];a=e[x]l[a]=l[a](s(l,a+d,e[U]))o=o+d;e=n[o];l[e[x]][e[h]]=l[e[B]];o=o+d;e=n[o];l[e[r]]=f[e[t]];o=o+d;e=n[o];l[e[b]]=l[e[h]][e[N]];o=o+d;e=n[o];l[e[x]]=l[e[u]][e[N]];o=o+d;e=n[o];l[e[b]][e[t]]=l[e[D]];o=o+d;e=n[o];l[e[r]][e[k]]=e[_];o=o+d;e=n[o];l[e[O]]=f[e[k]];o=o+d;e=n[o];l[e[r]]=l[e[c]][e[D]];o=o+d;e=n[o];l[e[O]]=e[U];o=o+d;e=n[o];l[e[r]]=e[U];o=o+d;e=n[o];l[e[O]]=e[U];o=o+d;e=n[o];a=e[w]l[a]=l[a](s(l,a+d,e[u]))o=o+d;e=n[o];l[e[w]][e[h]]=l[e[M]];o=o+d;e=n[o];l[e[b]][e[c]]=e[D];o=o+d;e=n[o];l[e[r]][e[t]]=e[N];o=o+d;e=n[o];l[e[w]][e[u]]=e[D];o=o+d;e=n[o];l[e[i]][e[U]]=e[B];o=o+d;e=n[o];l[e[i]][e[U]]=l[e[M]];o=o+d;e=n[o];l[e[x]]=f[e[t]];o=o+d;e=n[o];l[e[b]]=l[e[u]][e[D]];o=o+d;e=n[o];l[e[O]]=e[t];o=o+d;e=n[o];l[e[x]]=e[U];o=o+d;e=n[o];l[e[r]]=e[c];o=o+d;e=n[o];a=e[w]l[a]=l[a](s(l,a+d,e[u]))o=o+d;e=n[o];l[e[b]][e[U]]=l[e[P]];o=o+d;e=n[o];l[e[w]][e[k]]=e[D];o=o+d;e=n[o];l[e[i]]=f[e[h]];break end while 1693==(a)/((292024/211))do local _;local a;l[e[b]]=f[e[U]];o=o+d;e=n[o];l[e[O]]=l[e[u]][e[M]];o=o+d;e=n[o];l[e[b]]=e[c];o=o+d;e=n[o];l[e[x]]=y[e[t]];o=o+d;e=n[o];a=e[b]l[a]=l[a](s(l,a+d,e[U]))o=o+d;e=n[o];l[e[w]]=l[e[h]][e[M]];o=o+d;e=n[o];l[e[i]]=l[e[k]][e[D]];o=o+d;e=n[o];a=e[r];_=l[e[h]];l[a+1]=_;l[a]=_[e[M]];break end;break;end break;end break;end break;end break;end while(a)/((135+-71))==1425 do a=(1495912)while C<=(6032/58)do a-= a a=(12401532)while(17325/(-57+232))>=C do a-= a a=(4445280)while C<=(((984528/54)/172)+-#[[Crackzzzz]])do a-= a a=(2403288)while C>(-35+131)do a-= a local a;l[e[x]]=f[e[h]];o=o+d;e=n[o];l[e[r]]=l[e[h]][e[D]];o=o+d;e=n[o];l[e[O]]=l[e[k]];o=o+d;e=n[o];a=e[b]l[a]=l[a](l[a+S])o=o+d;e=n[o];l[e[x]]();break end while(a)/(((376812/54)-3525))==696 do local d=e[r];local a=l[d+2];local n=l[d]+a;l[d]=n;if(a>0)then if(n<=l[d+1])then o=e[u];l[d+3]=n;end elseif(n>=l[d+1])then o=e[h];l[d+3]=n;end break end;break;end while(a)/((-#[[Impulse youtube real]]+(2066+-86)))==2268 do a=(12734160)while C>(882/9)do a-= a l[e[r]][l[e[U]]]=l[e[N]];break end while(a)/(((1608229-804139)/245))==3880 do local a;l[e[w]]=e[t];o=o+d;e=n[o];a=e[w]l[a]=l[a](s(l,a+d,e[k]))o=o+d;e=n[o];l[e[x]][e[h]]=l[e[P]];o=o+d;e=n[o];l[e[w]][e[c]]=e[P];o=o+d;e=n[o];l[e[r]][e[c]]=e[P];o=o+d;e=n[o];l[e[b]]=f[e[c]];o=o+d;e=n[o];l[e[r]]=l[e[t]][e[M]];o=o+d;e=n[o];l[e[x]]=e[U];o=o+d;e=n[o];l[e[b]]=e[k];o=o+d;e=n[o];a=e[w]l[a]=l[a](s(l,a+d,e[t]))o=o+d;e=n[o];l[e[r]][e[h]]=l[e[P]];o=o+d;e=n[o];l[e[O]][e[c]]=l[e[B]];o=o+d;e=n[o];l[e[b]][e[c]]=e[N];o=o+d;e=n[o];l[e[x]][e[c]]=l[e[M]];o=o+d;e=n[o];l[e[O]]=f[e[c]];o=o+d;e=n[o];l[e[r]]=l[e[t]][e[_]];o=o+d;e=n[o];l[e[x]]=e[t];o=o+d;e=n[o];l[e[b]]=e[c];o=o+d;e=n[o];l[e[w]]=e[U];o=o+d;e=n[o];a=e[w]l[a]=l[a](s(l,a+d,e[k]))o=o+d;e=n[o];l[e[x]][e[U]]=l[e[N]];o=o+d;e=n[o];l[e[x]][e[c]]=e[N];o=o+d;e=n[o];l[e[b]]=f[e[t]];o=o+d;e=n[o];l[e[w]]=l[e[t]][e[M]];o=o+d;e=n[o];l[e[i]]=e[h];o=o+d;e=n[o];l[e[r]]=e[k];o=o+d;e=n[o];l[e[r]]=e[u];o=o+d;e=n[o];a=e[x]l[a]=l[a](s(l,a+d,e[u]))o=o+d;e=n[o];l[e[O]][e[U]]=l[e[D]];o=o+d;e=n[o];l[e[r]]=f[e[k]];o=o+d;e=n[o];l[e[O]]=l[e[h]][e[D]];o=o+d;e=n[o];l[e[b]]=e[t];o=o+d;e=n[o];l[e[b]]=e[u];o=o+d;e=n[o];l[e[x]]=e[U];o=o+d;e=n[o];l[e[i]]=e[u];o=o+d;e=n[o];a=e[O]l[a]=l[a](s(l,a+d,e[h]))o=o+d;e=n[o];l[e[r]][e[h]]=l[e[B]];o=o+d;e=n[o];l[e[i]]=f[e[u]];o=o+d;e=n[o];l[e[O]]=l[e[h]][e[M]];o=o+d;e=n[o];l[e[i]]=e[u];o=o+d;e=n[o];l[e[b]]=e[h];o=o+d;e=n[o];l[e[w]]=e[t];o=o+d;e=n[o];l[e[x]]=e[U];o=o+d;e=n[o];a=e[b]l[a]=l[a](s(l,a+d,e[u]))o=o+d;e=n[o];l[e[b]][e[c]]=l[e[N]];o=o+d;e=n[o];l[e[b]]=f[e[k]];o=o+d;e=n[o];l[e[i]]=l[e[h]][e[D]];o=o+d;e=n[o];l[e[b]]=l[e[h]][e[M]];o=o+d;e=n[o];l[e[x]][e[c]]=l[e[_]];o=o+d;e=n[o];l[e[i]][e[c]]=e[N];o=o+d;e=n[o];l[e[O]]=f[e[k]];o=o+d;e=n[o];l[e[b]]=l[e[t]][e[D]];o=o+d;e=n[o];l[e[w]]=e[k];o=o+d;e=n[o];l[e[O]]=e[t];o=o+d;e=n[o];l[e[b]]=e[c];o=o+d;e=n[o];a=e[O]l[a]=l[a](s(l,a+d,e[t]))o=o+d;e=n[o];l[e[r]][e[h]]=l[e[_]];o=o+d;e=n[o];l[e[w]][e[t]]=e[_];o=o+d;e=n[o];l[e[x]][e[c]]=e[B];o=o+d;e=n[o];l[e[O]]=f[e[u]];o=o+d;e=n[o];l[e[b]]=l[e[h]][e[M]];o=o+d;e=n[o];l[e[r]]=e[h];o=o+d;e=n[o];l[e[b]]=e[h];o=o+d;e=n[o];a=e[x]l[a]=l[a](s(l,a+d,e[U]))o=o+d;e=n[o];l[e[O]][e[u]]=l[e[B]];o=o+d;e=n[o];l[e[r]][e[U]]=l[e[N]];o=o+d;e=n[o];l[e[r]][e[c]]=e[_];o=o+d;e=n[o];l[e[i]][e[U]]=l[e[B]];o=o+d;e=n[o];l[e[r]]=f[e[h]];o=o+d;e=n[o];l[e[O]]=l[e[k]][e[M]];o=o+d;e=n[o];l[e[r]]=e[u];o=o+d;e=n[o];l[e[b]]=e[t];o=o+d;e=n[o];l[e[b]]=e[c];o=o+d;e=n[o];a=e[w]l[a]=l[a](s(l,a+d,e[u]))o=o+d;e=n[o];l[e[w]][e[c]]=l[e[P]];o=o+d;e=n[o];l[e[i]][e[u]]=e[N];o=o+d;e=n[o];l[e[i]]=f[e[t]];o=o+d;e=n[o];l[e[O]]=l[e[t]][e[N]];o=o+d;e=n[o];l[e[O]]=e[h];o=o+d;e=n[o];l[e[r]]=e[h];break end;break;end break;end while 3146==(a)/((-#[[panzerfaust]]+(3972+-19)))do a=(3844324)while C<=(310-209)do a-= a a=(2478600)while(21500/215)<C do a-= a local x=v[e[t]];local r;local d={};r=L({},{__index=function(o,e)local e=d[e];return e[1][e[2]];end,__newindex=function(l,e,o)local e=d[e]e[1][e[2]]=o;end;});for a=1,e[P]do o=o+S;local e=n[o];if e[((1870/170)+-#"bigchungus")]==56 then d[a-1]={l,e[h]};else d[a-1]={y,e[h]};end;z[#z+1]=d;end;l[e[i]]=A(x,r,f);break end while 1700==(a)/((-34+1492))do local o=e[b]local a={l[o](s(l,o+1,g))};local n=0;for e=o,e[B]do n=n+d;l[e]=a[n];end break end;break;end while(a)/(((45500/25)+-#"atakan der nigga"))==2131 do a=(2489665)while C<=(-#'send nudes'+(196+-84))do a-= a local e=e[x]l[e]=l[e](l[e+S])break;end while 1387==(a)/(((3728-1904)+-#'Fucking losed 027728272728271'))do a=(10006038)while((296-172)+-#'this is a meme string')<C do a-= a local e=e[r]l[e]=l[e](s(l,e+d,g))break end while 2781==(a)/((395780/110))do local a;l[e[b]]=y[e[U]];o=o+d;e=n[o];l[e[b]]=l[e[k]][e[P]];o=o+d;e=n[o];l[e[i]]=l[e[t]][e[P]];o=o+d;e=n[o];l[e[w]]=l[e[t]][e[N]];o=o+d;e=n[o];l[e[O]][e[k]]=e[D];o=o+d;e=n[o];l[e[i]]=f[e[h]];o=o+d;e=n[o];l[e[x]]=y[e[h]];o=o+d;e=n[o];a=e[O]l[a](l[a+S])o=o+d;e=n[o];l[e[b]]=y[e[c]];o=o+d;e=n[o];l[e[w]]=l[e[u]][e[N]];o=o+d;e=n[o];l[e[w]]=l[e[h]][e[P]];o=o+d;e=n[o];l[e[i]]=l[e[t]][e[_]];o=o+d;e=n[o];l[e[b]]=l[e[k]][e[M]];o=o+d;e=n[o];l[e[O]]=l[e[k]][e[_]];o=o+d;e=n[o];l[e[r]][e[h]]=e[_];o=o+d;e=n[o];do return end;break end;break;end break;end break;end break;end while(a)/((-#'nerd'+(-79+847)))==1958 do a=(6816616)while(19511/179)>=C do a-= a a=(1085313)while C<=(-117+(484-261))do a-= a a=(4805465)while(246-141)<C do a-= a l[e[O]][e[h]]=l[e[B]];break end while(a)/((-#[[Nsrds GAYYYYAIAHAKAJAVAHAUA]]+(2782-1422)))==3605 do local o=e[r]l[o](s(l,o+S,e[u]))break end;break;end while 3319==(a)/((751-(-#"0nly 1337"+(-57+490))))do a=(766675)while(27178/254)>=C do a-= a local a;l[e[O]]=f[e[h]];o=o+d;e=n[o];l[e[i]]=l[e[k]][e[_]];o=o+d;e=n[o];l[e[x]]=e[u];o=o+d;e=n[o];a=e[O]l[a]=l[a](l[a+S])o=o+d;e=n[o];l[e[O]]=f[e[t]];o=o+d;e=n[o];l[e[r]]=l[e[U]][e[B]];o=o+d;e=n[o];l[e[b]]=e[u];o=o+d;e=n[o];a=e[O]l[a]=l[a](l[a+S])o=o+d;e=n[o];l[e[w]]=f[e[c]];o=o+d;e=n[o];l[e[O]]=l[e[u]][e[P]];o=o+d;e=n[o];l[e[b]]=e[h];o=o+d;e=n[o];a=e[x]l[a]=l[a](l[a+S])o=o+d;e=n[o];l[e[x]]=f[e[k]];o=o+d;e=n[o];l[e[O]]=l[e[t]][e[M]];o=o+d;e=n[o];l[e[O]]=e[c];o=o+d;e=n[o];a=e[O]l[a]=l[a](l[a+S])o=o+d;e=n[o];l[e[x]]=f[e[h]];o=o+d;e=n[o];l[e[i]]=l[e[h]][e[D]];o=o+d;e=n[o];l[e[b]]=e[c];o=o+d;e=n[o];a=e[b]l[a]=l[a](l[a+S])o=o+d;e=n[o];l[e[i]]=f[e[U]];o=o+d;e=n[o];l[e[r]]=l[e[h]][e[P]];o=o+d;e=n[o];l[e[x]]=e[u];o=o+d;e=n[o];a=e[w]l[a]=l[a](l[a+S])o=o+d;e=n[o];l[e[b]]=f[e[t]];o=o+d;e=n[o];l[e[b]]=l[e[c]][e[M]];o=o+d;e=n[o];l[e[O]]=e[U];o=o+d;e=n[o];a=e[b]l[a]=l[a](l[a+S])o=o+d;e=n[o];l[e[w]]=f[e[c]];o=o+d;e=n[o];l[e[w]]=l[e[t]][e[P]];o=o+d;e=n[o];l[e[i]]=e[c];o=o+d;e=n[o];a=e[b]l[a]=l[a](l[a+S])o=o+d;e=n[o];l[e[x]]=f[e[U]];o=o+d;e=n[o];l[e[i]]=l[e[c]][e[M]];o=o+d;e=n[o];l[e[i]]=e[u];o=o+d;e=n[o];a=e[w]l[a]=l[a](l[a+S])o=o+d;e=n[o];l[e[r]]=f[e[U]];o=o+d;e=n[o];l[e[i]]=l[e[c]][e[D]];o=o+d;e=n[o];l[e[b]]=e[c];o=o+d;e=n[o];a=e[x]l[a]=l[a](l[a+S])o=o+d;e=n[o];l[e[r]]=f[e[c]];o=o+d;e=n[o];l[e[r]]=l[e[k]][e[D]];o=o+d;e=n[o];l[e[r]]=e[k];o=o+d;e=n[o];a=e[x]l[a]=l[a](l[a+S])o=o+d;e=n[o];l[e[r]]=f[e[u]];o=o+d;e=n[o];l[e[r]]=l[e[c]][e[P]];o=o+d;e=n[o];l[e[w]]=e[u];o=o+d;e=n[o];a=e[b]l[a]=l[a](l[a+S])o=o+d;e=n[o];l[e[i]]=f[e[t]];o=o+d;e=n[o];l[e[r]]=l[e[u]][e[P]];o=o+d;e=n[o];l[e[i]]=e[U];o=o+d;e=n[o];a=e[O]l[a]=l[a](l[a+S])o=o+d;e=n[o];l[e[x]]=f[e[U]];o=o+d;e=n[o];l[e[i]]=l[e[u]][e[_]];o=o+d;e=n[o];l[e[O]]=e[h];o=o+d;e=n[o];a=e[i]l[a]=l[a](l[a+S])o=o+d;e=n[o];l[e[x]]=f[e[u]];o=o+d;e=n[o];l[e[i]]=l[e[h]][e[M]];o=o+d;e=n[o];l[e[x]]=e[U];o=o+d;e=n[o];a=e[O]l[a]=l[a](l[a+S])o=o+d;e=n[o];l[e[b]]=f[e[u]];o=o+d;e=n[o];l[e[i]]=l[e[h]][e[N]];o=o+d;e=n[o];l[e[r]]=e[h];o=o+d;e=n[o];a=e[r]l[a]=l[a](l[a+S])o=o+d;e=n[o];l[e[x]]=f[e[t]];o=o+d;e=n[o];l[e[r]]=l[e[t]][e[B]];o=o+d;e=n[o];l[e[b]]=e[k];o=o+d;e=n[o];a=e[r]l[a]=l[a](l[a+S])o=o+d;e=n[o];l[e[x]]=f[e[t]];o=o+d;e=n[o];l[e[i]]=l[e[k]][e[_]];o=o+d;e=n[o];l[e[w]]=e[t];o=o+d;e=n[o];a=e[b]l[a]=l[a](l[a+S])o=o+d;e=n[o];l[e[O]]=f[e[k]];o=o+d;e=n[o];l[e[r]]=l[e[U]][e[P]];o=o+d;e=n[o];l[e[w]]=e[U];o=o+d;e=n[o];a=e[w]l[a]=l[a](l[a+S])o=o+d;e=n[o];l[e[i]]=f[e[h]];o=o+d;e=n[o];l[e[O]]=l[e[c]][e[B]];o=o+d;e=n[o];l[e[i]]=e[h];o=o+d;e=n[o];a=e[O]l[a]=l[a](l[a+S])break;end while(a)/((1023-568))==1685 do a=(2062341)while C>(-#'Faggot'+(161+-47))do a-= a local t;local a;l[e[r]]=f[e[c]];o=o+d;e=n[o];l[e[w]]=l[e[h]][e[P]];o=o+d;e=n[o];l[e[x]]=e[h];o=o+d;e=n[o];l[e[b]]=y[e[u]];o=o+d;e=n[o];a=e[x]l[a]=l[a](s(l,a+d,e[k]))o=o+d;e=n[o];l[e[i]]=l[e[U]][e[P]];o=o+d;e=n[o];l[e[x]]=l[e[c]][e[N]];o=o+d;e=n[o];a=e[x];t=l[e[k]];l[a+1]=t;l[a]=t[e[_]];break end while(a)/((557685/255))==943 do local a;l[e[i]]=f[e[c]];o=o+d;e=n[o];l[e[r]]=l[e[h]][e[_]];o=o+d;e=n[o];l[e[i]]=l[e[t]];o=o+d;e=n[o];a=e[O]l[a]=l[a](l[a+S])o=o+d;e=n[o];l[e[b]]();break end;break;end break;end break;end while 2468==(a)/(((515406/186)+-#'0nly 1337'))do a=(904959)while C<=(-#'yeet'+(351-236))do a-= a a=(1338528)while C>((9344/73)+-#'free bobux no skem')do a-= a local x;local a;a=e[r];x=l[e[k]];l[a+1]=x;l[a]=x[e[_]];o=o+d;e=n[o];l[e[r]]=e[U];o=o+d;e=n[o];a=e[b]l[a]=l[a](s(l,a+d,e[k]))o=o+d;e=n[o];l[e[i]]=l[e[U]][e[_]];o=o+d;e=n[o];a=e[b];x=l[e[c]];l[a+1]=x;l[a]=x[e[P]];break end while 3504==(a)/((875-493))do l[e[r]]=l[e[k]];break end;break;end while 297==(a)/(((241424/79)+-#'0nly segc'))do a=(10629360)while C<=(((-116+385)+-#'deadphonelua')-145)do a-= a do return end;break;end while 3885==(a)/(((701760/255)+-16))do a=(1730034)while C>(248-135)do a-= a if(l[e[i]]==e[D])then o=o+S;else o=e[u];end;break end while(a)/((-#[[windows xp startup sfx]]+(16308/36)))==4014 do local a;l[e[x]]=f[e[c]];o=o+d;e=n[o];l[e[w]]=l[e[U]][e[D]];o=o+d;e=n[o];l[e[w]]=l[e[k]];o=o+d;e=n[o];a=e[r]l[a]=l[a](l[a+S])o=o+d;e=n[o];l[e[O]]();break end;break;end break;end break;end break;end break;end break;end while(a)/((3273-1661))==3640 do a=(3489270)while(25669/193)>=C do a-= a a=(5554736)while(20172/164)>=C do a-= a a=(3333088)while C<=(((4926-2479)+-#"when the he went where when he where where when the he when ther wher he then here went")/20)do a-= a a=(1005438)while C<=((16569+-97)/142)do a-= a a=(341379)while(-35+150)<C do a-= a local o=e[b]local a={l[o](s(l,o+1,g))};local n=0;for e=o,e[_]do n=n+d;l[e]=a[n];end break end while(a)/((1595-(1780-932)))==457 do local o=e[b]l[o]=l[o](s(l,o+d,e[t]))break end;break;end while(a)/((617+-99))==1941 do a=(1320636)while C>(-#"Ur mom"+(7380/60))do a-= a local a;l[e[O]]=f[e[h]];o=o+d;e=n[o];l[e[r]]=l[e[k]][e[B]];o=o+d;e=n[o];l[e[x]]=l[e[k]];o=o+d;e=n[o];a=e[i]l[a]=l[a](l[a+S])o=o+d;e=n[o];l[e[x]]();break end while 1002==(a)/((-#"Crackzzzz"+(2684-1357)))do l[e[r]]={};break end;break;end break;end while 2992==(a)/(((2262-1140)+-#"Gay porn"))do a=(3711510)while C<=((4153-2113)/17)do a-= a a=(3222420)while(346-227)<C do a-= a do return l[e[b]]end break end while 860==(a)/((7528-3781))do l[e[i]]=f[e[h]];break end;break;end while(a)/((2180-1145))==3586 do a=(6227552)while(24200/200)>=C do a-= a local a;l[e[i]]=e[c];o=o+d;e=n[o];l[e[r]]=e[t];o=o+d;e=n[o];l[e[O]]=e[k];o=o+d;e=n[o];l[e[b]]=e[h];o=o+d;e=n[o];a=e[r]l[a]=l[a](s(l,a+d,e[h]))o=o+d;e=n[o];l[e[b]][e[k]]=l[e[D]];o=o+d;e=n[o];l[e[w]]=f[e[k]];o=o+d;e=n[o];l[e[x]]=l[e[h]][e[N]];o=o+d;e=n[o];l[e[w]]=e[U];o=o+d;e=n[o];l[e[O]]=e[k];o=o+d;e=n[o];l[e[w]]=e[h];o=o+d;e=n[o];l[e[O]]=e[k];o=o+d;e=n[o];a=e[i]l[a]=l[a](s(l,a+d,e[h]))o=o+d;e=n[o];l[e[r]][e[k]]=l[e[M]];o=o+d;e=n[o];l[e[b]]=f[e[t]];o=o+d;e=n[o];l[e[O]]=l[e[k]][e[B]];o=o+d;e=n[o];l[e[i]]=l[e[u]][e[N]];o=o+d;e=n[o];l[e[x]][e[k]]=l[e[P]];o=o+d;e=n[o];l[e[w]][e[t]]=e[M];o=o+d;e=n[o];l[e[x]]=f[e[U]];o=o+d;e=n[o];l[e[b]]=l[e[h]][e[P]];o=o+d;e=n[o];l[e[i]]=e[h];o=o+d;e=n[o];l[e[b]]=e[t];o=o+d;e=n[o];l[e[i]]=e[t];o=o+d;e=n[o];a=e[r]l[a]=l[a](s(l,a+d,e[c]))o=o+d;e=n[o];l[e[b]][e[c]]=l[e[_]];o=o+d;e=n[o];l[e[i]][e[c]]=e[_];o=o+d;e=n[o];l[e[x]][e[u]]=e[P];o=o+d;e=n[o];l[e[i]][e[u]]=e[P];o=o+d;e=n[o];l[e[O]][e[k]]=e[B];o=o+d;e=n[o];l[e[b]][e[k]]=l[e[D]];o=o+d;e=n[o];l[e[i]]=f[e[U]];o=o+d;e=n[o];l[e[b]]=l[e[k]][e[N]];o=o+d;e=n[o];l[e[b]]=e[U];o=o+d;e=n[o];l[e[w]]=e[h];o=o+d;e=n[o];l[e[O]]=e[k];o=o+d;e=n[o];a=e[x]l[a]=l[a](s(l,a+d,e[u]))o=o+d;e=n[o];l[e[O]][e[U]]=l[e[D]];o=o+d;e=n[o];l[e[w]][e[c]]=e[P];o=o+d;e=n[o];l[e[i]]=f[e[U]];o=o+d;e=n[o];l[e[x]]=l[e[U]][e[P]];o=o+d;e=n[o];l[e[r]]=e[h];o=o+d;e=n[o];l[e[r]]=e[U];o=o+d;e=n[o];l[e[i]]=e[h];o=o+d;e=n[o];l[e[i]]=e[h];o=o+d;e=n[o];a=e[w]l[a]=l[a](s(l,a+d,e[c]))o=o+d;e=n[o];l[e[i]][e[k]]=l[e[D]];o=o+d;e=n[o];l[e[i]]=f[e[h]];o=o+d;e=n[o];l[e[i]]=l[e[u]][e[M]];o=o+d;e=n[o];l[e[b]]=e[U];o=o+d;e=n[o];l[e[r]]=e[U];o=o+d;e=n[o];l[e[i]]=e[k];o=o+d;e=n[o];l[e[x]]=e[U];o=o+d;e=n[o];a=e[r]l[a]=l[a](s(l,a+d,e[U]))o=o+d;e=n[o];l[e[O]][e[c]]=l[e[N]];o=o+d;e=n[o];l[e[b]]=f[e[U]];o=o+d;e=n[o];l[e[w]]=l[e[k]][e[_]];o=o+d;e=n[o];l[e[w]]=l[e[h]][e[D]];o=o+d;e=n[o];l[e[i]][e[k]]=l[e[P]];o=o+d;e=n[o];l[e[w]][e[U]]=e[N];o=o+d;e=n[o];l[e[b]]=f[e[t]];o=o+d;e=n[o];l[e[x]]=l[e[t]][e[N]];o=o+d;e=n[o];l[e[x]]=e[k];o=o+d;e=n[o];l[e[i]]=e[k];o=o+d;e=n[o];l[e[w]]=e[k];o=o+d;e=n[o];a=e[w]l[a]=l[a](s(l,a+d,e[k]))o=o+d;e=n[o];l[e[w]][e[k]]=l[e[B]];o=o+d;e=n[o];l[e[r]][e[t]]=e[D];o=o+d;e=n[o];l[e[b]][e[h]]=e[D];o=o+d;e=n[o];l[e[x]][e[h]]=e[B];o=o+d;e=n[o];l[e[O]][e[t]]=e[M];o=o+d;e=n[o];l[e[b]][e[c]]=l[e[B]];o=o+d;e=n[o];l[e[O]]=f[e[U]];o=o+d;e=n[o];l[e[w]]=l[e[U]][e[B]];o=o+d;e=n[o];l[e[r]]=e[u];o=o+d;e=n[o];l[e[x]]=e[k];o=o+d;e=n[o];l[e[i]]=e[k];o=o+d;e=n[o];a=e[i]l[a]=l[a](s(l,a+d,e[t]))o=o+d;e=n[o];l[e[w]][e[u]]=l[e[_]];o=o+d;e=n[o];l[e[w]][e[k]]=e[P];break;end while(a)/((-72+2344))==2741 do a=(10305058)while C>((-55+201)+-#"fatee is gay 0nly on top")do a-= a l[e[w]]=e[t];break end while(a)/((7678-3881))==2714 do if(l[e[r]]==e[P])then o=o+S;else o=e[h];end;break end;break;end break;end break;end break;end while(a)/((1732+-26))==3256 do a=(11667496)while C<=(-#[[Deezbutts]]+(207+-70))do a-= a a=(10061225)while C<=(354-229)do a-= a a=(312512)while(251+(-16002/126))<C do a-= a local a;l[e[x]]=f[e[h]];o=o+d;e=n[o];l[e[w]]=l[e[c]][e[D]];o=o+d;e=n[o];l[e[b]]=l[e[h]];o=o+d;e=n[o];a=e[i]l[a]=l[a](l[a+S])o=o+d;e=n[o];l[e[x]]();break end while(a)/((52942/103))==608 do local a;l[e[O]]=e[c];o=o+d;e=n[o];a=e[i]l[a]=l[a](s(l,a+d,e[t]))o=o+d;e=n[o];l[e[r]][e[u]]=l[e[D]];o=o+d;e=n[o];l[e[w]][e[U]]=e[D];o=o+d;e=n[o];l[e[x]][e[u]]=e[M];o=o+d;e=n[o];l[e[r]]=f[e[c]];o=o+d;e=n[o];l[e[i]]=l[e[k]][e[D]];o=o+d;e=n[o];l[e[x]]=e[c];o=o+d;e=n[o];l[e[r]]=e[k];o=o+d;e=n[o];a=e[b]l[a]=l[a](s(l,a+d,e[u]))o=o+d;e=n[o];l[e[i]][e[k]]=l[e[_]];o=o+d;e=n[o];l[e[x]][e[h]]=l[e[M]];o=o+d;e=n[o];l[e[O]][e[t]]=e[_];o=o+d;e=n[o];l[e[O]][e[k]]=l[e[N]];o=o+d;e=n[o];l[e[i]]=f[e[k]];o=o+d;e=n[o];l[e[b]]=l[e[u]][e[_]];o=o+d;e=n[o];l[e[w]]=e[h];o=o+d;e=n[o];l[e[w]]=e[k];o=o+d;e=n[o];l[e[w]]=e[u];o=o+d;e=n[o];a=e[w]l[a]=l[a](s(l,a+d,e[U]))o=o+d;e=n[o];l[e[i]][e[u]]=l[e[N]];o=o+d;e=n[o];l[e[i]][e[U]]=e[_];o=o+d;e=n[o];l[e[i]]=f[e[t]];o=o+d;e=n[o];l[e[O]]=l[e[t]][e[_]];o=o+d;e=n[o];l[e[w]]=e[U];o=o+d;e=n[o];l[e[O]]=e[h];o=o+d;e=n[o];l[e[x]]=e[U];o=o+d;e=n[o];a=e[r]l[a]=l[a](s(l,a+d,e[c]))o=o+d;e=n[o];l[e[w]][e[c]]=l[e[D]];o=o+d;e=n[o];l[e[x]]=f[e[U]];o=o+d;e=n[o];l[e[w]]=l[e[k]][e[N]];o=o+d;e=n[o];l[e[w]]=e[u];o=o+d;e=n[o];l[e[w]]=e[h];o=o+d;e=n[o];l[e[r]]=e[t];o=o+d;e=n[o];l[e[r]]=e[h];o=o+d;e=n[o];a=e[b]l[a]=l[a](s(l,a+d,e[k]))o=o+d;e=n[o];l[e[w]][e[c]]=l[e[M]];o=o+d;e=n[o];l[e[i]]=f[e[c]];o=o+d;e=n[o];l[e[i]]=l[e[c]][e[N]];o=o+d;e=n[o];l[e[x]]=e[h];o=o+d;e=n[o];l[e[r]]=e[U];o=o+d;e=n[o];l[e[w]]=e[k];o=o+d;e=n[o];l[e[b]]=e[u];o=o+d;e=n[o];a=e[r]l[a]=l[a](s(l,a+d,e[k]))o=o+d;e=n[o];l[e[i]][e[U]]=l[e[N]];o=o+d;e=n[o];l[e[r]]=f[e[h]];o=o+d;e=n[o];l[e[w]]=l[e[t]][e[D]];o=o+d;e=n[o];l[e[w]]=l[e[u]][e[_]];o=o+d;e=n[o];l[e[r]][e[t]]=l[e[N]];o=o+d;e=n[o];l[e[x]][e[t]]=e[N];o=o+d;e=n[o];l[e[x]]=f[e[t]];o=o+d;e=n[o];l[e[w]]=l[e[c]][e[B]];o=o+d;e=n[o];l[e[w]]=e[u];o=o+d;e=n[o];l[e[w]]=e[k];o=o+d;e=n[o];l[e[b]]=e[u];o=o+d;e=n[o];a=e[i]l[a]=l[a](s(l,a+d,e[k]))o=o+d;e=n[o];l[e[b]][e[h]]=l[e[D]];o=o+d;e=n[o];l[e[i]][e[t]]=e[M];o=o+d;e=n[o];l[e[i]][e[u]]=e[_];o=o+d;e=n[o];l[e[r]]=f[e[U]];o=o+d;e=n[o];l[e[O]]=l[e[h]][e[P]];o=o+d;e=n[o];l[e[w]]=e[c];o=o+d;e=n[o];l[e[i]]=e[h];o=o+d;e=n[o];a=e[x]l[a]=l[a](s(l,a+d,e[h]))o=o+d;e=n[o];l[e[w]][e[t]]=l[e[M]];o=o+d;e=n[o];l[e[i]][e[u]]=l[e[M]];o=o+d;e=n[o];l[e[r]][e[U]]=e[_];o=o+d;e=n[o];l[e[x]][e[t]]=l[e[B]];o=o+d;e=n[o];l[e[x]]=f[e[t]];o=o+d;e=n[o];l[e[x]]=l[e[t]][e[D]];o=o+d;e=n[o];l[e[i]]=e[h];o=o+d;e=n[o];l[e[x]]=e[t];o=o+d;e=n[o];l[e[b]]=e[h];o=o+d;e=n[o];a=e[O]l[a]=l[a](s(l,a+d,e[t]))o=o+d;e=n[o];l[e[x]][e[c]]=l[e[M]];o=o+d;e=n[o];l[e[w]][e[u]]=e[N];o=o+d;e=n[o];l[e[w]]=f[e[t]];o=o+d;e=n[o];l[e[w]]=l[e[u]][e[M]];o=o+d;e=n[o];l[e[r]]=e[k];o=o+d;e=n[o];l[e[r]]=e[t];break end;break;end while 3725==(a)/((5457-2756))do a=(813656)while C<=(-68+194)do a-= a local a;local i;local P,B;local C;local a;l[e[r]]=y[e[u]];o=o+d;e=n[o];l[e[r]]=l[e[t]][e[_]];o=o+d;e=n[o];l[e[O]][e[U]]=e[D];o=o+d;e=n[o];l[e[w]]=y[e[k]];o=o+d;e=n[o];l[e[r]]=l[e[c]][e[N]];o=o+d;e=n[o];l[e[x]]=l[e[c]][e[N]];o=o+d;e=n[o];l[e[b]]=l[e[h]][e[D]];o=o+d;e=n[o];l[e[b]][e[h]]=e[_];o=o+d;e=n[o];l[e[x]]=f[e[k]];o=o+d;e=n[o];l[e[x]]=f[e[c]];o=o+d;e=n[o];a=e[O];C=l[e[U]];l[a+1]=C;l[a]=C[e[D]];o=o+d;e=n[o];l[e[r]]=e[u];o=o+d;e=n[o];a=e[x]l[a]=l[a](s(l,a+d,e[h]))o=o+d;e=n[o];a=e[x];C=l[e[k]];l[a+1]=C;l[a]=C[e[_]];o=o+d;e=n[o];a=e[x]P,B=m(l[a](l[a+S]))g=B+a-d i=0;for e=a,g do i=i+d;l[e]=P[i];end;o=o+d;e=n[o];a=e[x]P={l[a](s(l,a+1,g))};i=0;for e=a,e[M]do i=i+d;l[e]=P[i];end o=o+d;e=n[o];o=e[h];break;end while(a)/((84840/105))==1007 do a=(7261281)while(-95+222)<C do a-= a local d=e[O];local n=l[d]local a=l[d+2];if(a>0)then if(n>l[d+1])then o=e[c];else l[d+3]=n;end elseif(n<l[d+1])then o=e[c];else l[d+3]=n;end break end while 3741==(a)/((135870/70))do local a;l[e[w]]=f[e[c]];o=o+d;e=n[o];l[e[b]]=l[e[u]][e[_]];o=o+d;e=n[o];l[e[w]]=l[e[u]];o=o+d;e=n[o];a=e[O]l[a]=l[a](l[a+S])o=o+d;e=n[o];l[e[x]]();break end;break;end break;end break;end while 3637==(a)/(((247228/76)+-#'testpsx dupe no scam legit 2022 free no virus'))do a=(201780)while(373-243)>=C do a-= a a=(2939640)while((412-263)+-#'Cock and ball tortue')<C do a-= a local x;local a;l[e[i]]=f[e[t]];o=o+d;e=n[o];l[e[r]]=l[e[U]][e[B]];o=o+d;e=n[o];l[e[w]]=e[U];o=o+d;e=n[o];l[e[w]]=y[e[c]];o=o+d;e=n[o];a=e[i]l[a]=l[a](s(l,a+d,e[u]))o=o+d;e=n[o];l[e[i]]=l[e[h]][e[M]];o=o+d;e=n[o];l[e[b]]=l[e[t]][e[B]];o=o+d;e=n[o];a=e[r];x=l[e[U]];l[a+1]=x;l[a]=x[e[D]];break end while(a)/((-#'W4rboy was here'+(179647/169)))==2805 do local a;local k;local B,p;local C;local a;l[e[i]]=y[e[U]];o=o+d;e=n[o];l[e[i]]=l[e[h]][e[P]];o=o+d;e=n[o];l[e[O]][e[t]]=e[M];o=o+d;e=n[o];l[e[x]]=y[e[c]];o=o+d;e=n[o];l[e[O]]=l[e[u]][e[D]];o=o+d;e=n[o];l[e[x]]=l[e[U]][e[P]];o=o+d;e=n[o];l[e[b]]=l[e[h]][e[P]];o=o+d;e=n[o];l[e[O]][e[U]]=e[M];o=o+d;e=n[o];l[e[r]]=f[e[c]];o=o+d;e=n[o];l[e[i]]=f[e[U]];o=o+d;e=n[o];a=e[b];C=l[e[c]];l[a+1]=C;l[a]=C[e[N]];o=o+d;e=n[o];l[e[w]]=e[c];o=o+d;e=n[o];a=e[r]l[a]=l[a](s(l,a+d,e[c]))o=o+d;e=n[o];a=e[i];C=l[e[U]];l[a+1]=C;l[a]=C[e[_]];o=o+d;e=n[o];a=e[r]B,p=m(l[a](l[a+S]))g=p+a-d k=0;for e=a,g do k=k+d;l[e]=B[k];end;o=o+d;e=n[o];a=e[w]B={l[a](s(l,a+1,g))};k=0;for e=a,e[M]do k=k+d;l[e]=B[k];end o=o+d;e=n[o];o=e[u];break end;break;end while 1140==(a)/((((681-359)+-100)+-#"testpsx dupe no scam legit 2022 free no virus"))do a=(6997432)while(27510/210)>=C do a-= a l[e[w]][e[k]]=e[_];break;end while 3172==(a)/((297810/135))do a=(9285549)while(-#'if syn then haxor alert end'+((341+-100)+-82))<C do a-= a local d=e[b];local n=l[d]local a=l[d+2];if(a>0)then if(n>l[d+1])then o=e[c];else l[d+3]=n;end elseif(n<l[d+1])then o=e[k];else l[d+3]=n;end break end while(a)/((-107+4020))==2373 do local e=e[x]local n,o=m(l[e](s(l,e+d,g)))g=o+e-S local o=0;for e=e,g do o=o+d;l[e]=n[o];end;break end;break;end break;end break;end break;end break;end while(a)/((1183+-113))==3261 do a=(8131495)while C<=(23309/163)do a-= a a=(1933179)while C<=(16698/121)do a-= a a=(4369125)while((22197/147)+-#"cruz pp is large")>=C do a-= a a=(4346760)while(-#[[holy shit]]+(336-193))<C do a-= a local e=e[i]l[e]=l[e](l[e+S])break end while(a)/(((5988-3035)+-#'0nly was here mf'))==1480 do local e=e[w]local n,o=m(l[e](l[e+S]))g=o+e-d local o=0;for e=e,g do o=o+d;l[e]=n[o];end;break end;break;end while(a)/((-#"yeet"+(212531/(-116+255))))==2865 do a=(515648)while C<=(346-210)do a-= a local C;local a;l[e[x]]=l[e[t]][e[M]];o=o+d;e=n[o];l[e[w]]=e[c];o=o+d;e=n[o];a=e[i]l[a]=l[a](l[a+S])o=o+d;e=n[o];l[e[x]]=f[e[U]];o=o+d;e=n[o];l[e[b]]=l[e[k]][e[_]];o=o+d;e=n[o];l[e[b]]=e[u];o=o+d;e=n[o];a=e[x]l[a]=l[a](l[a+S])o=o+d;e=n[o];l[e[O]]=f[e[h]];o=o+d;e=n[o];l[e[i]]=l[e[h]][e[N]];o=o+d;e=n[o];l[e[i]]=e[c];o=o+d;e=n[o];a=e[x]l[a]=l[a](l[a+S])o=o+d;e=n[o];l[e[x]]=f[e[h]];o=o+d;e=n[o];l[e[w]]=l[e[u]][e[P]];o=o+d;e=n[o];l[e[r]]=e[U];o=o+d;e=n[o];a=e[w]l[a]=l[a](l[a+S])o=o+d;e=n[o];l[e[i]]=f[e[k]];o=o+d;e=n[o];l[e[x]]=l[e[U]][e[B]];o=o+d;e=n[o];l[e[x]]=e[k];o=o+d;e=n[o];a=e[w]l[a]=l[a](l[a+S])o=o+d;e=n[o];l[e[O]]=f[e[k]];o=o+d;e=n[o];l[e[x]]=l[e[h]][e[_]];o=o+d;e=n[o];l[e[O]]=e[U];o=o+d;e=n[o];a=e[O]l[a]=l[a](l[a+S])o=o+d;e=n[o];l[e[r]]=f[e[c]];o=o+d;e=n[o];l[e[b]]=l[e[k]][e[P]];o=o+d;e=n[o];l[e[r]]=e[k];o=o+d;e=n[o];a=e[O]l[a]=l[a](l[a+S])o=o+d;e=n[o];l[e[r]]=f[e[h]];o=o+d;e=n[o];l[e[O]]=l[e[h]][e[M]];o=o+d;e=n[o];l[e[b]]=e[U];o=o+d;e=n[o];a=e[x]l[a]=l[a](l[a+S])o=o+d;e=n[o];l[e[b]]=f[e[h]];o=o+d;e=n[o];l[e[O]]=l[e[t]][e[M]];o=o+d;e=n[o];l[e[b]]=e[k];o=o+d;e=n[o];a=e[x]l[a]=l[a](l[a+S])o=o+d;e=n[o];l[e[x]]=f[e[t]];o=o+d;e=n[o];l[e[i]]=l[e[k]][e[N]];o=o+d;e=n[o];l[e[w]]=e[t];o=o+d;e=n[o];a=e[x]l[a]=l[a](l[a+S])o=o+d;e=n[o];l[e[i]]=f[e[U]];o=o+d;e=n[o];l[e[O]]=l[e[t]][e[P]];o=o+d;e=n[o];l[e[w]]=e[h];o=o+d;e=n[o];a=e[w]l[a]=l[a](l[a+S])o=o+d;e=n[o];l[e[b]]=f[e[U]];o=o+d;e=n[o];l[e[b]]=l[e[k]][e[_]];o=o+d;e=n[o];l[e[w]]=e[h];o=o+d;e=n[o];a=e[O]l[a]=l[a](l[a+S])o=o+d;e=n[o];l[e[w]]=f[e[c]];o=o+d;e=n[o];l[e[i]]=l[e[U]][e[B]];o=o+d;e=n[o];l[e[r]]=e[t];o=o+d;e=n[o];a=e[r]l[a]=l[a](l[a+S])o=o+d;e=n[o];l[e[b]]=f[e[k]];o=o+d;e=n[o];l[e[r]]=l[e[u]][e[B]];o=o+d;e=n[o];l[e[x]]=e[c];o=o+d;e=n[o];a=e[r]l[a]=l[a](l[a+S])o=o+d;e=n[o];l[e[w]][e[c]]=e[P];o=o+d;e=n[o];l[e[x]]=f[e[k]];o=o+d;e=n[o];l[e[r]]=l[e[k]][e[P]];o=o+d;e=n[o];l[e[O]]=l[e[u]][e[D]];o=o+d;e=n[o];a=e[w];C=l[e[c]];l[a+1]=C;l[a]=C[e[N]];o=o+d;e=n[o];l[e[i]]=e[u];o=o+d;e=n[o];a=e[i]l[a]=l[a](s(l,a+d,e[U]))o=o+d;e=n[o];l[e[O]][e[t]]=l[e[P]];o=o+d;e=n[o];l[e[i]]=f[e[U]];o=o+d;e=n[o];l[e[x]]=l[e[U]][e[N]];o=o+d;e=n[o];l[e[i]]=l[e[U]][e[D]];o=o+d;e=n[o];l[e[w]][e[U]]=l[e[D]];o=o+d;e=n[o];l[e[r]][e[u]]=e[P];o=o+d;e=n[o];l[e[r]][e[k]]=l[e[P]];o=o+d;e=n[o];l[e[b]]=f[e[h]];o=o+d;e=n[o];l[e[O]]=l[e[t]][e[D]];o=o+d;e=n[o];l[e[i]]=e[u];o=o+d;e=n[o];l[e[i]]=e[h];o=o+d;e=n[o];l[e[x]]=e[h];o=o+d;e=n[o];a=e[b]l[a]=l[a](s(l,a+d,e[u]))o=o+d;e=n[o];l[e[O]][e[h]]=l[e[M]];o=o+d;e=n[o];l[e[w]][e[u]]=e[_];o=o+d;e=n[o];l[e[i]]=f[e[t]];o=o+d;e=n[o];l[e[b]]=l[e[u]][e[B]];o=o+d;e=n[o];l[e[w]]=e[k];break;end while 224==(a)/((-#"Nsrds GAYYYYAIAHAKAJAVAHAUA"+(2382+-53)))do a=(12506598)while(21920/((445-270)+-#[[howtodumpscript]]))<C do a-= a local a;l[e[r]]=f[e[c]];o=o+d;e=n[o];l[e[x]]=l[e[k]][e[D]];o=o+d;e=n[o];l[e[b]]=l[e[u]];o=o+d;e=n[o];a=e[i]l[a]=l[a](l[a+S])o=o+d;e=n[o];l[e[w]]();break end while 3783==(a)/((6714-3408))do local x;local a;l[e[b]]=f[e[t]];o=o+d;e=n[o];l[e[w]]=l[e[t]][e[_]];o=o+d;e=n[o];l[e[i]]=e[c];o=o+d;e=n[o];l[e[r]]=y[e[k]];o=o+d;e=n[o];a=e[i]l[a]=l[a](s(l,a+d,e[U]))o=o+d;e=n[o];l[e[w]]=l[e[k]][e[M]];o=o+d;e=n[o];l[e[w]]=l[e[t]][e[D]];o=o+d;e=n[o];a=e[O];x=l[e[k]];l[a+1]=x;l[a]=x[e[N]];break end;break;end break;end break;end while(a)/((-119+1040))==2099 do a=(1361230)while((27375/75)-225)>=C do a-= a a=(6587815)while(278/2)<C do a-= a f[e[t]]=l[e[i]];break end while 2795==(a)/((4814-2457))do local o=e[O];local d=l[e[c]];l[o+1]=d;l[o]=d[e[M]];break end;break;end while 566==(a)/((-#"papier ist ein kleiner schwanz lutscher"+(562120/230)))do a=(12630912)while(-#"atakan der nigga"+(385-228))>=C do a-= a local a;a=e[r]l[a]=l[a](s(l,a+d,e[U]))o=o+d;e=n[o];l[e[x]][e[c]]=l[e[M]];o=o+d;e=n[o];l[e[w]][e[h]]=e[P];o=o+d;e=n[o];l[e[r]]=f[e[U]];o=o+d;e=n[o];l[e[i]]=l[e[t]][e[_]];o=o+d;e=n[o];l[e[i]]=e[h];o=o+d;e=n[o];l[e[w]]=e[h];o=o+d;e=n[o];l[e[r]]=e[U];o=o+d;e=n[o];l[e[x]]=e[h];o=o+d;e=n[o];a=e[O]l[a]=l[a](s(l,a+d,e[t]))o=o+d;e=n[o];l[e[b]][e[U]]=l[e[N]];o=o+d;e=n[o];l[e[r]]=f[e[c]];o=o+d;e=n[o];l[e[w]]=l[e[U]][e[B]];o=o+d;e=n[o];l[e[O]]=e[U];o=o+d;e=n[o];l[e[b]]=e[k];o=o+d;e=n[o];l[e[b]]=e[h];o=o+d;e=n[o];l[e[x]]=e[h];o=o+d;e=n[o];a=e[w]l[a]=l[a](s(l,a+d,e[U]))o=o+d;e=n[o];l[e[w]][e[t]]=l[e[D]];o=o+d;e=n[o];l[e[w]]=f[e[t]];o=o+d;e=n[o];l[e[O]]=l[e[c]][e[M]];o=o+d;e=n[o];l[e[x]]=l[e[u]][e[M]];o=o+d;e=n[o];l[e[b]][e[U]]=l[e[B]];o=o+d;e=n[o];l[e[x]][e[c]]=e[M];o=o+d;e=n[o];l[e[x]]=f[e[c]];o=o+d;e=n[o];l[e[w]]=l[e[U]][e[_]];o=o+d;e=n[o];l[e[w]]=e[u];o=o+d;e=n[o];l[e[x]]=e[c];o=o+d;e=n[o];l[e[w]]=e[c];o=o+d;e=n[o];a=e[r]l[a]=l[a](s(l,a+d,e[k]))o=o+d;e=n[o];l[e[w]][e[h]]=l[e[N]];o=o+d;e=n[o];l[e[x]][e[h]]=e[B];o=o+d;e=n[o];l[e[b]][e[k]]=e[M];o=o+d;e=n[o];l[e[i]][e[h]]=e[M];o=o+d;e=n[o];l[e[x]][e[u]]=e[D];o=o+d;e=n[o];l[e[O]][e[t]]=l[e[D]];o=o+d;e=n[o];l[e[x]]=f[e[U]];o=o+d;e=n[o];l[e[b]]=l[e[U]][e[N]];o=o+d;e=n[o];l[e[w]]=e[u];o=o+d;e=n[o];l[e[b]]=e[t];o=o+d;e=n[o];l[e[x]]=e[c];o=o+d;e=n[o];a=e[b]l[a]=l[a](s(l,a+d,e[h]))o=o+d;e=n[o];l[e[b]][e[u]]=l[e[_]];o=o+d;e=n[o];l[e[b]][e[k]]=e[D];o=o+d;e=n[o];l[e[i]]=f[e[t]];o=o+d;e=n[o];l[e[i]]=l[e[u]][e[N]];o=o+d;e=n[o];l[e[w]]=e[t];o=o+d;e=n[o];l[e[O]]=e[c];o=o+d;e=n[o];l[e[b]]=e[k];o=o+d;e=n[o];a=e[r]l[a]=l[a](s(l,a+d,e[u]))o=o+d;e=n[o];l[e[x]][e[c]]=l[e[_]];o=o+d;e=n[o];l[e[i]][e[h]]=e[B];o=o+d;e=n[o];l[e[b]]=f[e[t]];o=o+d;e=n[o];l[e[i]]=l[e[k]][e[P]];o=o+d;e=n[o];l[e[O]]=e[h];o=o+d;e=n[o];l[e[x]]=e[t];o=o+d;e=n[o];l[e[O]]=e[h];o=o+d;e=n[o];l[e[w]]=e[c];o=o+d;e=n[o];a=e[r]l[a]=l[a](s(l,a+d,e[c]))o=o+d;e=n[o];l[e[O]][e[c]]=l[e[P]];o=o+d;e=n[o];l[e[w]]=f[e[U]];o=o+d;e=n[o];l[e[x]]=l[e[k]][e[B]];o=o+d;e=n[o];l[e[O]]=e[U];o=o+d;e=n[o];l[e[r]]=e[k];o=o+d;e=n[o];l[e[x]]=e[h];o=o+d;e=n[o];l[e[b]]=e[c];o=o+d;e=n[o];a=e[x]l[a]=l[a](s(l,a+d,e[k]))o=o+d;e=n[o];l[e[i]][e[c]]=l[e[_]];o=o+d;e=n[o];l[e[O]][e[c]]=e[B];o=o+d;e=n[o];l[e[r]][e[u]]=l[e[N]];o=o+d;e=n[o];l[e[O]]=f[e[u]];o=o+d;e=n[o];l[e[O]]=l[e[u]][e[D]];o=o+d;e=n[o];l[e[b]]=e[U];o=o+d;e=n[o];l[e[x]]=e[t];o=o+d;e=n[o];l[e[O]]=e[U];o=o+d;e=n[o];a=e[i]l[a]=l[a](s(l,a+d,e[h]))o=o+d;e=n[o];l[e[r]][e[U]]=l[e[P]];o=o+d;e=n[o];l[e[b]][e[t]]=e[D];o=o+d;e=n[o];l[e[r]]=f[e[k]];o=o+d;e=n[o];l[e[w]]=l[e[k]][e[M]];break;end while 4064==(a)/((3216+-108))do a=(3380841)while C>(-#"nerd"+((-#"this is a meme string"+(17996/44))-242))do a-= a l[e[r]]=f[e[u]];break end while(a)/((-#"anime is for fags"+((4074-2065)-1023)))==3489 do local a;l[e[i]][e[U]]=l[e[N]];o=o+d;e=n[o];l[e[w]][e[t]]=e[D];o=o+d;e=n[o];l[e[b]]=f[e[c]];o=o+d;e=n[o];l[e[i]]=l[e[t]][e[D]];o=o+d;e=n[o];l[e[i]]=e[c];o=o+d;e=n[o];l[e[w]]=e[t];o=o+d;e=n[o];l[e[b]]=e[c];o=o+d;e=n[o];l[e[b]]=e[u];o=o+d;e=n[o];a=e[x]l[a]=l[a](s(l,a+d,e[k]))o=o+d;e=n[o];l[e[O]][e[c]]=l[e[D]];o=o+d;e=n[o];l[e[x]]=f[e[k]];o=o+d;e=n[o];l[e[x]]=l[e[u]][e[N]];o=o+d;e=n[o];l[e[b]]=e[u];o=o+d;e=n[o];l[e[b]]=e[h];o=o+d;e=n[o];l[e[i]]=e[k];o=o+d;e=n[o];l[e[b]]=e[U];o=o+d;e=n[o];a=e[x]l[a]=l[a](s(l,a+d,e[k]))o=o+d;e=n[o];l[e[r]][e[c]]=l[e[M]];o=o+d;e=n[o];l[e[O]]=f[e[h]];o=o+d;e=n[o];l[e[O]]=l[e[u]][e[P]];o=o+d;e=n[o];l[e[w]]=l[e[c]][e[D]];o=o+d;e=n[o];l[e[b]][e[t]]=l[e[D]];o=o+d;e=n[o];l[e[w]][e[k]]=e[_];o=o+d;e=n[o];l[e[O]]=f[e[k]];o=o+d;e=n[o];l[e[r]]=l[e[t]][e[D]];o=o+d;e=n[o];l[e[b]]=e[t];o=o+d;e=n[o];l[e[r]]=e[u];o=o+d;e=n[o];l[e[x]]=e[c];o=o+d;e=n[o];a=e[b]l[a]=l[a](s(l,a+d,e[t]))o=o+d;e=n[o];l[e[b]][e[k]]=l[e[D]];o=o+d;e=n[o];l[e[w]][e[u]]=e[P];o=o+d;e=n[o];l[e[i]][e[c]]=e[M];o=o+d;e=n[o];l[e[b]][e[h]]=e[P];o=o+d;e=n[o];l[e[i]][e[c]]=e[P];o=o+d;e=n[o];l[e[r]][e[U]]=l[e[B]];o=o+d;e=n[o];l[e[i]]=f[e[t]];o=o+d;e=n[o];l[e[r]]=l[e[U]][e[_]];o=o+d;e=n[o];l[e[w]]=e[c];o=o+d;e=n[o];l[e[w]]=e[h];o=o+d;e=n[o];l[e[w]]=e[u];o=o+d;e=n[o];a=e[O]l[a]=l[a](s(l,a+d,e[u]))o=o+d;e=n[o];l[e[w]][e[h]]=l[e[N]];o=o+d;e=n[o];l[e[r]][e[k]]=e[N];o=o+d;e=n[o];l[e[w]]=f[e[U]];o=o+d;e=n[o];l[e[O]]=l[e[u]][e[N]];o=o+d;e=n[o];l[e[b]]=e[u];o=o+d;e=n[o];l[e[r]]=e[u];o=o+d;e=n[o];l[e[O]]=e[t];o=o+d;e=n[o];l[e[O]]=e[u];o=o+d;e=n[o];a=e[w]l[a]=l[a](s(l,a+d,e[c]))o=o+d;e=n[o];l[e[O]][e[k]]=l[e[N]];o=o+d;e=n[o];l[e[x]]=f[e[k]];o=o+d;e=n[o];l[e[O]]=l[e[h]][e[_]];o=o+d;e=n[o];l[e[x]]=e[h];o=o+d;e=n[o];l[e[w]]=e[k];o=o+d;e=n[o];l[e[b]]=e[h];o=o+d;e=n[o];l[e[i]]=e[t];o=o+d;e=n[o];a=e[O]l[a]=l[a](s(l,a+d,e[k]))o=o+d;e=n[o];l[e[w]][e[t]]=l[e[M]];o=o+d;e=n[o];l[e[x]]=f[e[U]];o=o+d;e=n[o];l[e[O]]=l[e[c]][e[D]];o=o+d;e=n[o];l[e[r]]=l[e[U]][e[B]];o=o+d;e=n[o];l[e[w]][e[U]]=l[e[N]];o=o+d;e=n[o];l[e[x]][e[c]]=e[P];o=o+d;e=n[o];l[e[x]]=f[e[c]];o=o+d;e=n[o];l[e[i]]=l[e[k]][e[M]];o=o+d;e=n[o];l[e[O]]=e[k];o=o+d;e=n[o];l[e[x]]=e[c];o=o+d;e=n[o];l[e[O]]=e[c];o=o+d;e=n[o];a=e[w]l[a]=l[a](s(l,a+d,e[U]))o=o+d;e=n[o];l[e[w]][e[t]]=l[e[D]];o=o+d;e=n[o];l[e[i]][e[h]]=e[N];o=o+d;e=n[o];l[e[w]][e[c]]=e[B];o=o+d;e=n[o];l[e[O]][e[k]]=e[_];o=o+d;e=n[o];l[e[i]][e[h]]=e[_];o=o+d;e=n[o];l[e[r]][e[t]]=l[e[_]];o=o+d;e=n[o];l[e[r]]=f[e[U]];o=o+d;e=n[o];l[e[b]]=l[e[U]][e[M]];o=o+d;e=n[o];l[e[O]]=e[h];o=o+d;e=n[o];l[e[r]]=e[c];break end;break;end break;end break;end break;end while 3635==(a)/((-46+2283))do a=(1481006)while((28320/177)+-#"deadphonelua")>=C do a-= a a=(2466200)while(345-(432-232))>=C do a-= a a=(4992240)while C>(182+(35+-73))do a-= a local o=e[b]local n,e=m(l[o](s(l,o+1,e[k])))g=e+o-1 local e=0;for o=o,g do e=e+d;l[o]=n[e];end;break end while(a)/((4058+-32))==1240 do l[e[b]]=(e[h]~=0);break end;break;end while 760==(a)/((6575-3330))do a=(8083764)while(33580/230)>=C do a-= a local o=e[b]l[o](s(l,o+S,e[U]))break;end while 3004==(a)/((5473-2782))do a=(16240000)while C>(-126+(-#'atakan der nigga'+(703-414)))do a-= a local a;l[e[x]]=f[e[h]];o=o+d;e=n[o];l[e[b]]=l[e[t]][e[N]];o=o+d;e=n[o];l[e[b]]=l[e[k]];o=o+d;e=n[o];a=e[r]l[a]=l[a](l[a+S])o=o+d;e=n[o];l[e[b]]();o=o+d;e=n[o];do return end;break end while(a)/((((127600340/217)+-#"impulse was here omg")/147))==4060 do local a;l[e[b]]=f[e[U]];o=o+d;e=n[o];l[e[r]]=l[e[h]][e[_]];o=o+d;e=n[o];l[e[r]]=e[U];o=o+d;e=n[o];l[e[i]]=e[c];o=o+d;e=n[o];l[e[O]]=e[u];o=o+d;e=n[o];l[e[i]]=e[u];o=o+d;e=n[o];a=e[b]l[a]=l[a](s(l,a+d,e[t]))o=o+d;e=n[o];l[e[i]][e[U]]=l[e[B]];o=o+d;e=n[o];l[e[i]]=f[e[u]];o=o+d;e=n[o];l[e[i]]=l[e[t]][e[M]];o=o+d;e=n[o];l[e[x]]=e[t];o=o+d;e=n[o];l[e[x]]=e[k];o=o+d;e=n[o];l[e[O]]=e[t];o=o+d;e=n[o];l[e[w]]=e[h];o=o+d;e=n[o];a=e[O]l[a]=l[a](s(l,a+d,e[h]))o=o+d;e=n[o];l[e[x]][e[U]]=l[e[M]];o=o+d;e=n[o];l[e[i]]=f[e[U]];o=o+d;e=n[o];l[e[O]]=l[e[t]][e[N]];o=o+d;e=n[o];l[e[i]]=l[e[k]][e[N]];o=o+d;e=n[o];l[e[w]][e[u]]=l[e[D]];o=o+d;e=n[o];l[e[O]][e[u]]=e[_];o=o+d;e=n[o];l[e[r]]=f[e[t]];o=o+d;e=n[o];l[e[x]]=l[e[u]][e[_]];o=o+d;e=n[o];l[e[x]]=e[U];o=o+d;e=n[o];l[e[O]]=e[c];o=o+d;e=n[o];l[e[r]]=e[U];o=o+d;e=n[o];a=e[x]l[a]=l[a](s(l,a+d,e[k]))o=o+d;e=n[o];l[e[b]][e[t]]=l[e[B]];o=o+d;e=n[o];l[e[r]][e[U]]=e[B];o=o+d;e=n[o];l[e[b]][e[h]]=e[P];o=o+d;e=n[o];l[e[i]][e[k]]=e[N];o=o+d;e=n[o];l[e[i]][e[h]]=e[M];o=o+d;e=n[o];l[e[O]][e[c]]=l[e[M]];o=o+d;e=n[o];l[e[O]]=f[e[t]];o=o+d;e=n[o];l[e[O]]=l[e[t]][e[B]];o=o+d;e=n[o];l[e[w]]=e[u];o=o+d;e=n[o];l[e[w]]=e[k];o=o+d;e=n[o];l[e[x]]=e[k];o=o+d;e=n[o];a=e[b]l[a]=l[a](s(l,a+d,e[U]))o=o+d;e=n[o];l[e[i]][e[U]]=l[e[_]];o=o+d;e=n[o];l[e[O]][e[U]]=e[M];o=o+d;e=n[o];l[e[i]]=f[e[c]];o=o+d;e=n[o];l[e[O]]=l[e[c]][e[N]];o=o+d;e=n[o];l[e[x]]=e[u];o=o+d;e=n[o];l[e[b]]=e[k];o=o+d;e=n[o];l[e[w]]=e[k];o=o+d;e=n[o];l[e[w]]=e[U];o=o+d;e=n[o];a=e[w]l[a]=l[a](s(l,a+d,e[h]))o=o+d;e=n[o];l[e[r]][e[u]]=l[e[B]];o=o+d;e=n[o];l[e[b]]=f[e[k]];o=o+d;e=n[o];l[e[O]]=l[e[U]][e[P]];o=o+d;e=n[o];l[e[b]]=e[h];o=o+d;e=n[o];l[e[b]]=e[u];o=o+d;e=n[o];l[e[x]]=e[h];o=o+d;e=n[o];l[e[r]]=e[u];o=o+d;e=n[o];a=e[r]l[a]=l[a](s(l,a+d,e[t]))o=o+d;e=n[o];l[e[i]][e[k]]=l[e[M]];o=o+d;e=n[o];l[e[i]]=f[e[U]];o=o+d;e=n[o];l[e[i]]=l[e[k]][e[B]];o=o+d;e=n[o];l[e[b]]=l[e[h]][e[P]];o=o+d;e=n[o];l[e[b]][e[U]]=l[e[B]];o=o+d;e=n[o];l[e[O]][e[h]]=e[P];o=o+d;e=n[o];l[e[r]]=f[e[u]];o=o+d;e=n[o];l[e[b]]=l[e[u]][e[B]];o=o+d;e=n[o];l[e[r]]=e[U];o=o+d;e=n[o];l[e[O]]=e[k];o=o+d;e=n[o];l[e[b]]=e[k];o=o+d;e=n[o];a=e[r]l[a]=l[a](s(l,a+d,e[c]))o=o+d;e=n[o];l[e[b]][e[c]]=l[e[D]];o=o+d;e=n[o];l[e[w]][e[u]]=e[_];o=o+d;e=n[o];l[e[r]][e[u]]=e[_];o=o+d;e=n[o];l[e[x]][e[k]]=e[M];o=o+d;e=n[o];l[e[w]][e[c]]=e[B];o=o+d;e=n[o];l[e[i]][e[c]]=l[e[D]];o=o+d;e=n[o];l[e[w]]=f[e[U]];o=o+d;e=n[o];l[e[x]]=l[e[h]][e[N]];o=o+d;e=n[o];l[e[w]]=e[h];o=o+d;e=n[o];l[e[i]]=e[c];o=o+d;e=n[o];l[e[r]]=e[c];o=o+d;e=n[o];a=e[i]l[a]=l[a](s(l,a+d,e[k]))break end;break;end break;end break;end while(a)/((-115+2141))==731 do a=(8220240)while C<=(-57+207)do a-= a a=(1419556)while(-#"Lana Rhoades"+(-71+(-97+329)))<C do a-= a do return l[e[b]]end break end while 3868==(a)/((-#[[lego hax]]+(-123+498)))do local w;local a;l[e[x]]=f[e[c]];o=o+d;e=n[o];l[e[r]]=l[e[c]][e[B]];o=o+d;e=n[o];l[e[b]]=e[h];o=o+d;e=n[o];l[e[i]]=y[e[u]];o=o+d;e=n[o];a=e[x]l[a]=l[a](s(l,a+d,e[U]))o=o+d;e=n[o];l[e[b]]=l[e[c]][e[B]];o=o+d;e=n[o];l[e[i]]=l[e[u]][e[B]];o=o+d;e=n[o];a=e[r];w=l[e[t]];l[a+1]=w;l[a]=w[e[D]];break end;break;end while 2520==(a)/((6548-3286))do a=(5979816)while(-41+192)>=C do a-= a l[e[x]]=l[e[U]]%e[M];break;end while(a)/((385848/233))==3611 do a=(464446)while(374-222)<C do a-= a l[e[b]]={};break end while 362==(a)/((2635-1352))do local d=e[h];local o=l[d]for e=d+1,e[N]do o=o..l[e];end;l[e[x]]=o;break end;break;end break;end break;end break;end break;end break;end break;end o+= S end;end);end;return A(Y(),{},W())()end)_msec({[(-110+286)]='\115\116'..(function(e)return(e and'㒛㒥㒦㒙㒣㒣㒡㒣㒠㒤㒡㒝㒡')or'\114\105'or'\120\58'end)((61-56)==(-#"lego hax"+(3486/249)))..'\110g',["㒜㒡㒜㒗㒟㒞㒙㒢㒝㒙㒟㒚㒥㒗㒞㒡㒡㒞"]='\108\100'..(function(e)return(e and'㒡㒠㒙㒤㒘㒛㒛㒠㒣㒟㒟㒢㒛㒘㒘㒠')or'\101\120'or'\119\111'end)((51+-46)==(-#'0nly was here mf'+(-116+138)))..'\112',["㒙㒘㒣㒙㒣㒢㒙㒡㒜㒣㒛㒙㒢"]=(function(e)return(e and'㒚㒘㒦㒡㒤㒛㒝㒟㒣㒟')and'\98\121'or'\100\120'end)((540/108)==((2877/137)+-#"0nly was here mf"))..'\116\101',["㒝㒣㒝㒢㒠㒙㒡㒚"]='\99'..(function(e)return(e and'㒟㒣㒜㒢㒡㒦㒠㒟㒠㒗㒗㒘㒥㒦㒦㒥㒤㒞㒝')and'\90\19\157'or'\104\97'end)(((1015/35)+-#[[fatee is gay 0nly on top]])==((-45+55)+-#[[elbicho]]))..'\114',[(1146-602)]='\116\97'..(function(e)return(e and'㒥㒟㒟㒜㒦㒡㒝㒠㒝㒦')and'\64\113'or'\98\108'end)((101-95)==((((-1089/11)+-#'Negro')+118)+-#'0nly segc'))..'\101',["㒟㒡㒟㒣㒣㒣㒠㒤㒛㒤㒦㒙㒡㒘"]=(function(e)return(e and'㒝㒗㒙㒗㒤㒝㒟㒤㒢㒚㒢㒤')or'\115\117'or'\78\107'end)(((-18+48)+-#'if syn then haxor alert end')==(-#"bigchungus"+(183-142)))..'\98',["㒜㒝㒠㒞㒚㒜㒗㒥㒟㒤㒗㒥㒛㒗㒘㒜㒝"]='\99\111'..(function(e)return(e and'㒟㒡㒝㒜㒘㒜㒟㒛㒜㒝㒥㒡㒡㒦㒠㒛㒦㒛')and'\110\99'or'\110\105\103\97'end)((76+-45)==(-#[[papier der afghaner wurde von nice dem bombenleger gefickt]]+(200-111)))..'\97\116',[(-36+697)]=(function(e,o)return(e and'㒦㒡㒣㒚㒝㒦㒢㒤㒞㒜㒗㒢㒣㒙')and'\48\159\158\188\10'or'\109\97'end)(((197-162)+-#'testing this thingy lololollez')==(132-126))..'\116\104',[(1441+-53)]=(function(e,o)return((1210/242)==(-#[[0nly 1337 smashed ur wap]]+(-81+108))and'\48'..'\195'or e..((not'\20\95\69'and'\90'..'\180'or o)))or'\199\203\95'end),["㒣㒜㒟㒡㒚㒘㒤㒛"]='\105\110'..(function(e,o)return(e and'㒚㒣㒚㒣㒜㒟㒟㒞㒙㒦㒞㒝㒘㒢㒟㒤㒤㒦')and'\90\115\138\115\15'or'\115\101'end)((65/13)==((-22+69)+-#"cruz pp is large"))..'\114\116',["㒝㒛㒠㒥㒠㒝㒠㒙㒟㒣㒛㒞㒥㒝㒗㒗㒠㒥㒛"]='\117\110'..(function(e,o)return(e and'㒙㒜㒣㒟㒘㒟㒙㒞㒚㒣㒚㒚㒡㒞㒗㒙㒤㒤㒣')or'\112\97'or'\20\38\154'end)((118-113)==(133-102))..'\99\107',["㒡㒞㒥㒟㒙㒠㒠㒢㒜㒘㒤㒙㒛㒣㒚"]='\115\101'..(function(e)return(e and'㒟㒦㒞㒟㒙㒗㒛㒤㒙㒢㒠㒙㒜㒗㒝㒥㒟㒗㒤')and'\110\112\99\104'or'\108\101'end)(((-85+105)+-#'howtodumpscript')==(186-155))..'\99\116',["㒤㒗㒝㒗㒦㒝㒞㒢㒣㒚㒣㒤"]='\116\111\110'..(function(e,o)return(e and'㒛㒙㒥㒤㒘㒠㒦㒠㒙㒘㒢㒛')and'\117\109\98'or'\100\97\120\122'end)((((2305-1178)+-#[[windows xp startup sfx]])/221)==(-#"howtodumpscript"+(-83+103)))..'\101\114'},{["㒢㒥㒛㒣㒤㒝㒛㒡㒗㒠"]=((getfenv))},((getfenv))()) end)()



	end            
})
JogadorTab:AddButton({
	Name = "Puxar Algema - Eb do @Lack_EvZ",
	Callback = function()
		for i, v in pairs(game:GetDescendants()) do
			if v:IsA('Tool') then
				v.Parent = game:GetService('Players').LocalPlayer.Backpack
			end
		end

		game:GetService('Players').LocalPlayer.Character.Humanoid.Died:Connect(function()
			for i, v in pairs(game:GetService('Players').LocalPlayer.Backpack:GetDescendants()) do
				if v:IsA('Tool') then
					v.Parent = game:GetService('Teams')
				end
			end
			for i, v in pairs(game:GetService('Players').LocalPlayer.Character:GetDescendants()) do
				if v:IsA('Tool') then
					v.Parent = game:GetService('Teams')
				end
			end
		end)
	end              
})
JogadorTab:AddButton({
	Name = "Dex (Visual)",
	Callback = function()
		loadstring(game:HttpGet(('https://raw.githubusercontent.com/Pedroxz63/Explorer/main/README.md'),true))()
	end        
})
local Section = JogadorTab:AddSection({
	Name = "Recomendado"
})
JogadorTab:AddToggle({
	Name = "Anti ADM",
	Default = false,
	Callback = function(Value)
		print(Value)
	end 
})
JogadorTab:AddToggle({
	Name = "Modo Serial Killer",
	Default = false,
	Callback = function(Value)
		_G.Loop = Value
		Loop()
	end   
}) 
JogadorTab:AddButton({
	Name = "Ficar Invisivel - Bind",
	Callback = function()
		local ScriptStarted = false
		local Keybind = "E" --Set to whatever you want, has to be the name of a KeyCode Enum.
		local Transparency = true --Will make you slightly transparent when you are invisible. No reason to disable.
		local NoClip = false --Will make your fake character no clip.
		local Player = game:GetService("Players").LocalPlayer
		local RealCharacter = Player.Character or Player.CharacterAdded:Wait()
		local IsInvisible = false
		RealCharacter.Archivable = true
		local FakeCharacter = RealCharacter:Clone()
		local Part
		Part = Instance.new("Part", workspace)
		Part.Anchored = true
		Part.Size = Vector3.new(200, 1, 200)
		Part.CFrame = CFrame.new(0, -500, 0) --Set this to whatever you want, just far away from the map.
		Part.CanCollide = true
		FakeCharacter.Parent = workspace
		FakeCharacter.HumanoidRootPart.CFrame = Part.CFrame * CFrame.new(0, 5, 0)
		for i, v in pairs(RealCharacter:GetChildren()) do
			if v:IsA("LocalScript") then
				local clone = v:Clone()
				clone.Disabled = true
				clone.Parent = FakeCharacter
			end
		end
		if Transparency then
			for i, v in pairs(FakeCharacter:GetDescendants()) do
				if v:IsA("BasePart") then
					v.Transparency = 0.7
				end
			end
		end
		local CanInvis = true
		function RealCharacterDied()
			CanInvis = false
			RealCharacter:Destroy()
			RealCharacter = Player.Character
			CanInvis = true
			isinvisible = false
			FakeCharacter:Destroy()
			workspace.CurrentCamera.CameraSubject = RealCharacter.Humanoid
			RealCharacter.Archivable = true
			FakeCharacter = RealCharacter:Clone()
			Part:Destroy()
			Part = Instance.new("Part", workspace)
			Part.Anchored = true
			Part.Size = Vector3.new(200, 1, 200)
			Part.CFrame = CFrame.new(9999, 9999, 9999) --Set this to whatever you want, just far away from the map.
			Part.CanCollide = true
			FakeCharacter.Parent = workspace
			FakeCharacter.HumanoidRootPart.CFrame = Part.CFrame * CFrame.new(0, 5, 0)
			for i, v in pairs(RealCharacter:GetChildren()) do
				if v:IsA("LocalScript") then
					local clone = v:Clone()
					clone.Disabled = true
					clone.Parent = FakeCharacter
				end
			end
			if Transparency then
				for i, v in pairs(FakeCharacter:GetDescendants()) do
					if v:IsA("BasePart") then
						v.Transparency = 0.7
					end
				end
			end
			RealCharacter.Humanoid.Died:Connect(function()
				RealCharacter:Destroy()
				FakeCharacter:Destroy()
			end)
			Player.CharacterAppearanceLoaded:Connect(RealCharacterDied)
		end
		RealCharacter.Humanoid.Died:Connect(function()
			RealCharacter:Destroy()
			FakeCharacter:Destroy()
		end)
		Player.CharacterAppearanceLoaded:Connect(RealCharacterDied)
		local PseudoAnchor
		game:GetService "RunService".RenderStepped:Connect(
			function()
				if PseudoAnchor ~= nil then
					PseudoAnchor.CFrame = Part.CFrame * CFrame.new(0, 5, 0)
				end
				if NoClip then
					FakeCharacter.Humanoid:ChangeState(11)
				end
			end
		)
		PseudoAnchor = FakeCharacter.HumanoidRootPart
		local function Invisible()
			if IsInvisible == false then
				local StoredCF = RealCharacter.HumanoidRootPart.CFrame
				RealCharacter.HumanoidRootPart.CFrame = FakeCharacter.HumanoidRootPart.CFrame
				FakeCharacter.HumanoidRootPart.CFrame = StoredCF
				RealCharacter.Humanoid:UnequipTools()
				Player.Character = FakeCharacter
				workspace.CurrentCamera.CameraSubject = FakeCharacter.Humanoid
				PseudoAnchor = RealCharacter.HumanoidRootPart
				for i, v in pairs(FakeCharacter:GetChildren()) do
					if v:IsA("LocalScript") then
						v.Disabled = false
					end
				end
				IsInvisible = true
			else
				local StoredCF = FakeCharacter.HumanoidRootPart.CFrame
				FakeCharacter.HumanoidRootPart.CFrame = RealCharacter.HumanoidRootPart.CFrame

				RealCharacter.HumanoidRootPart.CFrame = StoredCF

				FakeCharacter.Humanoid:UnequipTools()
				Player.Character = RealCharacter
				workspace.CurrentCamera.CameraSubject = RealCharacter.Humanoid
				PseudoAnchor = FakeCharacter.HumanoidRootPart
				for i, v in pairs(FakeCharacter:GetChildren()) do
					if v:IsA("LocalScript") then
						v.Disabled = true
					end
				end
				IsInvisible = false
			end
		end
		game:GetService("UserInputService").InputBegan:Connect(
		function(key, gamep)
			if gamep then
				return
			end
			if key.KeyCode.Name:lower() == Keybind:lower() and CanInvis and RealCharacter and FakeCharacter then
				if RealCharacter:FindFirstChild("HumanoidRootPart") and FakeCharacter:FindFirstChild("HumanoidRootPart") then
					Invisible()
				end
			end
		end
		)
		local Sound = Instance.new("Sound",game:GetService("SoundService"))
		Sound.SoundId = "rbxassetid://232127604"
		Sound:Play()
		game:GetService("StarterGui"):SetCore("SendNotification",{["Title"] = "Invisivel Carregado!",["Text"] = "Pressione "..Keybind.." Para usar o invisivel!",["Duration"] = 20,["Button1"] = "Okay."})
	end    
})
local Section = JogadorTab:AddSection({
	Name = "Geral"
})
JogadorTab:AddButton({
	Name = "Control Click TP - Bypass",
	Callback = function()
		loadstring(game:HttpGet(('https://gitlab.com/cccontrol/cccontrol/-/raw/master/ExtraScripts/ClickTPTool'),true))()
	end
})
JogadorTab:AddButton({
	Name = "Comprar Fusca Cda - Sem ter Money",
	Callback = function()
		local args = {
			[1] = "dealership",
			[2] = "Fusca"
		}

		game:GetService("ReplicatedStorage").ConcessionariaRS.Remotes.Check:InvokeServer(unpack(args))
		wait(1)
	end    
})
JogadorTab:AddButton({
	Name = "Trigger - Gerar logs",
	Callback = function()
            --[[
    SimpleSpy v2.2 SOURCE
 
    Credits:
        exx - basically everything
        Frosty - GUI to Lua
]]

		-- shuts down the previous instance of SimpleSpy
		if _G.SimpleSpyExecuted and type(_G.SimpleSpyShutdown) == "function" then
			_G.SimpleSpyShutdown()
		end

		local Players = game:GetService("Players")
		local CoreGui = game:GetService("CoreGui")
		local Highlight = loadstring(game:HttpGet("https://github.com/exxtremestuffs/SimpleSpySource/raw/master/highlight.lua"))()

		---- GENERATED (kinda sorta mostly) BY GUI to LUA ----

		-- Instances:

		local SimpleSpy2 = Instance.new("ScreenGui")
		local Background = Instance.new("Frame")
		local LeftPanel = Instance.new("Frame")
		local LogList = Instance.new("ScrollingFrame")
		local UIListLayout = Instance.new("UIListLayout")
		local RemoteTemplate = Instance.new("Frame")
		local ColorBar = Instance.new("Frame")
		local Text = Instance.new("TextLabel")
		local Button = Instance.new("TextButton")
		local RightPanel = Instance.new("Frame")
		local CodeBox = Instance.new("Frame")
		local ScrollingFrame = Instance.new("ScrollingFrame")
		local UIGridLayout = Instance.new("UIGridLayout")
		local FunctionTemplate = Instance.new("Frame")
		local ColorBar_2 = Instance.new("Frame")
		local Text_2 = Instance.new("TextLabel")
		local Button_2 = Instance.new("TextButton")
		local TopBar = Instance.new("Frame")
		local Simple = Instance.new("TextButton")
		local CloseButton = Instance.new("TextButton")
		local ImageLabel = Instance.new("ImageLabel")
		local MaximizeButton = Instance.new("TextButton")
		local ImageLabel_2 = Instance.new("ImageLabel")
		local MinimizeButton = Instance.new("TextButton")
		local ImageLabel_3 = Instance.new("ImageLabel")
		local ToolTip = Instance.new("Frame")
		local TextLabel = Instance.new("TextLabel")

		--Properties:

		SimpleSpy2.Name = "SimpleSpy2"
		SimpleSpy2.ResetOnSpawn = false

		Background.Name = "Background"
		Background.Parent = SimpleSpy2
		Background.BackgroundColor3 = Color3.new(1, 1, 1)
		Background.BackgroundTransparency = 1
		Background.Position = UDim2.new(0, 500, 0, 200)
		Background.Size = UDim2.new(0, 450, 0, 268)

		LeftPanel.Name = "LeftPanel"
		LeftPanel.Parent = Background
		LeftPanel.BackgroundColor3 = Color3.new(0.207843, 0.203922, 0.215686)
		LeftPanel.BorderSizePixel = 0
		LeftPanel.Position = UDim2.new(0, 0, 0, 19)
		LeftPanel.Size = UDim2.new(0, 131, 0, 249)

		LogList.Name = "LogList"
		LogList.Parent = LeftPanel
		LogList.Active = true
		LogList.BackgroundColor3 = Color3.new(1, 1, 1)
		LogList.BackgroundTransparency = 1
		LogList.BorderSizePixel = 0
		LogList.Position = UDim2.new(0, 0, 0, 9)
		LogList.Size = UDim2.new(0, 131, 0, 232)
		LogList.CanvasSize = UDim2.new(0, 0, 0, 0)
		LogList.ScrollBarThickness = 4

		UIListLayout.Parent = LogList
		UIListLayout.HorizontalAlignment = Enum.HorizontalAlignment.Center
		UIListLayout.SortOrder = Enum.SortOrder.LayoutOrder

		RemoteTemplate.Name = "RemoteTemplate"
		RemoteTemplate.Parent = LogList
		RemoteTemplate.BackgroundColor3 = Color3.new(1, 1, 1)
		RemoteTemplate.BackgroundTransparency = 1
		RemoteTemplate.Size = UDim2.new(0, 117, 0, 27)

		ColorBar.Name = "ColorBar"
		ColorBar.Parent = RemoteTemplate
		ColorBar.BackgroundColor3 = Color3.new(1, 0.94902, 0)
		ColorBar.BorderSizePixel = 0
		ColorBar.Position = UDim2.new(0, 0, 0, 1)
		ColorBar.Size = UDim2.new(0, 7, 0, 18)
		ColorBar.ZIndex = 2

		Text.Name = "Text"
		Text.Parent = RemoteTemplate
		Text.BackgroundColor3 = Color3.new(1, 1, 1)
		Text.BackgroundTransparency = 1
		Text.Position = UDim2.new(0, 12, 0, 1)
		Text.Size = UDim2.new(0, 105, 0, 18)
		Text.ZIndex = 2
		Text.Font = Enum.Font.SourceSans
		Text.Text = "TEXT"
		Text.TextColor3 = Color3.new(1, 1, 1)
		Text.TextSize = 14
		Text.TextXAlignment = Enum.TextXAlignment.Left

		Button.Name = "Button"
		Button.Parent = RemoteTemplate
		Button.BackgroundColor3 = Color3.new(0, 0, 0)
		Button.BackgroundTransparency = 0.75
		Button.BorderColor3 = Color3.new(1, 1, 1)
		Button.Position = UDim2.new(0, 0, 0, 1)
		Button.Size = UDim2.new(0, 117, 0, 18)
		Button.AutoButtonColor = false
		Button.Font = Enum.Font.SourceSans
		Button.Text = ""
		Button.TextColor3 = Color3.new(0, 0, 0)
		Button.TextSize = 14

		RightPanel.Name = "RightPanel"
		RightPanel.Parent = Background
		RightPanel.BackgroundColor3 = Color3.new(0.145098, 0.141176, 0.14902)
		RightPanel.BorderSizePixel = 0
		RightPanel.Position = UDim2.new(0, 131, 0, 19)
		RightPanel.Size = UDim2.new(0, 319, 0, 249)

		CodeBox.Name = "CodeBox"
		CodeBox.Parent = RightPanel
		CodeBox.BackgroundColor3 = Color3.new(0.0823529, 0.0745098, 0.0784314)
		CodeBox.BorderSizePixel = 0
		CodeBox.Size = UDim2.new(0, 319, 0, 119)

		ScrollingFrame.Parent = RightPanel
		ScrollingFrame.Active = true
		ScrollingFrame.BackgroundColor3 = Color3.new(1, 1, 1)
		ScrollingFrame.BackgroundTransparency = 1
		ScrollingFrame.Position = UDim2.new(0, 0, 0.5, 0)
		ScrollingFrame.Size = UDim2.new(1, 0, 0.5, -9)
		ScrollingFrame.CanvasSize = UDim2.new(0, 0, 0, 0)
		ScrollingFrame.ScrollBarThickness = 4

		UIGridLayout.Parent = ScrollingFrame
		UIGridLayout.HorizontalAlignment = Enum.HorizontalAlignment.Center
		UIGridLayout.SortOrder = Enum.SortOrder.LayoutOrder
		UIGridLayout.CellPadding = UDim2.new(0, 0, 0, 0)
		UIGridLayout.CellSize = UDim2.new(0, 94, 0, 27)

		FunctionTemplate.Name = "FunctionTemplate"
		FunctionTemplate.Parent = ScrollingFrame
		FunctionTemplate.BackgroundColor3 = Color3.new(1, 1, 1)
		FunctionTemplate.BackgroundTransparency = 1
		FunctionTemplate.Size = UDim2.new(0, 117, 0, 23)

		ColorBar_2.Name = "ColorBar"
		ColorBar_2.Parent = FunctionTemplate
		ColorBar_2.BackgroundColor3 = Color3.new(1, 1, 1)
		ColorBar_2.BorderSizePixel = 0
		ColorBar_2.Position = UDim2.new(0, 7, 0, 10)
		ColorBar_2.Size = UDim2.new(0, 7, 0, 18)
		ColorBar_2.ZIndex = 3

		Text_2.Name = "Text"
		Text_2.Parent = FunctionTemplate
		Text_2.BackgroundColor3 = Color3.new(1, 1, 1)
		Text_2.BackgroundTransparency = 1
		Text_2.Position = UDim2.new(0, 19, 0, 10)
		Text_2.Size = UDim2.new(0, 69, 0, 18)
		Text_2.ZIndex = 2
		Text_2.Font = Enum.Font.SourceSans
		Text_2.Text = "TEXT"
		Text_2.TextColor3 = Color3.new(1, 1, 1)
		Text_2.TextSize = 14
		Text_2.TextStrokeColor3 = Color3.new(0.145098, 0.141176, 0.14902)
		Text_2.TextXAlignment = Enum.TextXAlignment.Left

		Button_2.Name = "Button"
		Button_2.Parent = FunctionTemplate
		Button_2.BackgroundColor3 = Color3.new(0, 0, 0)
		Button_2.BackgroundTransparency = 0.69999998807907
		Button_2.BorderColor3 = Color3.new(1, 1, 1)
		Button_2.Position = UDim2.new(0, 7, 0, 10)
		Button_2.Size = UDim2.new(0, 80, 0, 18)
		Button_2.AutoButtonColor = false
		Button_2.Font = Enum.Font.SourceSans
		Button_2.Text = ""
		Button_2.TextColor3 = Color3.new(0, 0, 0)
		Button_2.TextSize = 14

		TopBar.Name = "TopBar"
		TopBar.Parent = Background
		TopBar.BackgroundColor3 = Color3.new(0.145098, 0.141176, 0.14902)
		TopBar.BorderSizePixel = 0
		TopBar.Size = UDim2.new(0, 450, 0, 19)

		Simple.Name = "Simple"
		Simple.Parent = TopBar
		Simple.BackgroundColor3 = Color3.new(1, 1, 1)
		Simple.AutoButtonColor = false
		Simple.BackgroundTransparency = 1
		Simple.Position = UDim2.new(0, 5, 0, 0)
		Simple.Size = UDim2.new(0, 57, 0, 18)
		Simple.Font = Enum.Font.SourceSansBold
		Simple.Text = "SimpleSpy"
		Simple.TextColor3 = Color3.new(1, 1, 1)
		Simple.TextSize = 14
		Simple.TextXAlignment = Enum.TextXAlignment.Left

		CloseButton.Name = "CloseButton"
		CloseButton.Parent = TopBar
		CloseButton.BackgroundColor3 = Color3.new(0.145098, 0.141176, 0.14902)
		CloseButton.BorderSizePixel = 0
		CloseButton.Position = UDim2.new(1, -19, 0, 0)
		CloseButton.Size = UDim2.new(0, 19, 0, 19)
		CloseButton.Font = Enum.Font.SourceSans
		CloseButton.Text = ""
		CloseButton.TextColor3 = Color3.new(0, 0, 0)
		CloseButton.TextSize = 14

		ImageLabel.Parent = CloseButton
		ImageLabel.BackgroundColor3 = Color3.new(1, 1, 1)
		ImageLabel.BackgroundTransparency = 1
		ImageLabel.Position = UDim2.new(0, 5, 0, 5)
		ImageLabel.Size = UDim2.new(0, 9, 0, 9)
		ImageLabel.Image = "http://www.roblox.com/asset/?id=5597086202"

		MaximizeButton.Name = "MaximizeButton"
		MaximizeButton.Parent = TopBar
		MaximizeButton.BackgroundColor3 = Color3.new(0.145098, 0.141176, 0.14902)
		MaximizeButton.BorderSizePixel = 0
		MaximizeButton.Position = UDim2.new(1, -38, 0, 0)
		MaximizeButton.Size = UDim2.new(0, 19, 0, 19)
		MaximizeButton.Font = Enum.Font.SourceSans
		MaximizeButton.Text = ""
		MaximizeButton.TextColor3 = Color3.new(0, 0, 0)
		MaximizeButton.TextSize = 14

		ImageLabel_2.Parent = MaximizeButton
		ImageLabel_2.BackgroundColor3 = Color3.new(1, 1, 1)
		ImageLabel_2.BackgroundTransparency = 1
		ImageLabel_2.Position = UDim2.new(0, 5, 0, 5)
		ImageLabel_2.Size = UDim2.new(0, 9, 0, 9)
		ImageLabel_2.Image = "http://www.roblox.com/asset/?id=5597108117"

		MinimizeButton.Name = "MinimizeButton"
		MinimizeButton.Parent = TopBar
		MinimizeButton.BackgroundColor3 = Color3.new(0.145098, 0.141176, 0.14902)
		MinimizeButton.BorderSizePixel = 0
		MinimizeButton.Position = UDim2.new(1, -57, 0, 0)
		MinimizeButton.Size = UDim2.new(0, 19, 0, 19)
		MinimizeButton.Font = Enum.Font.SourceSans
		MinimizeButton.Text = ""
		MinimizeButton.TextColor3 = Color3.new(0, 0, 0)
		MinimizeButton.TextSize = 14

		ImageLabel_3.Parent = MinimizeButton
		ImageLabel_3.BackgroundColor3 = Color3.new(1, 1, 1)
		ImageLabel_3.BackgroundTransparency = 1
		ImageLabel_3.Position = UDim2.new(0, 5, 0, 5)
		ImageLabel_3.Size = UDim2.new(0, 9, 0, 9)
		ImageLabel_3.Image = "http://www.roblox.com/asset/?id=5597105827"

		ToolTip.Name = "ToolTip"
		ToolTip.Parent = SimpleSpy2
		ToolTip.BackgroundColor3 = Color3.fromRGB(26, 26, 26)
		ToolTip.BackgroundTransparency = 0.1
		ToolTip.BorderColor3 = Color3.new(1, 1, 1)
		ToolTip.Size = UDim2.new(0, 200, 0, 50)
		ToolTip.ZIndex = 3
		ToolTip.Visible = false

		TextLabel.Parent = ToolTip
		TextLabel.BackgroundColor3 = Color3.new(1, 1, 1)
		TextLabel.BackgroundTransparency = 1
		TextLabel.Position = UDim2.new(0, 2, 0, 2)
		TextLabel.Size = UDim2.new(0, 196, 0, 46)
		TextLabel.ZIndex = 3
		TextLabel.Font = Enum.Font.SourceSans
		TextLabel.Text = "This is some slightly longer text."
		TextLabel.TextColor3 = Color3.new(1, 1, 1)
		TextLabel.TextSize = 14
		TextLabel.TextWrapped = true
		TextLabel.TextXAlignment = Enum.TextXAlignment.Left
		TextLabel.TextYAlignment = Enum.TextYAlignment.Top

		-------------------------------------------------------------------------------
		-- init
		local RunService = game:GetService("RunService")
		local UserInputService = game:GetService("UserInputService")
		local TweenService = game:GetService("TweenService")
		local ContentProvider = game:GetService("ContentProvider")
		local TextService = game:GetService("TextService")
		local Mouse = game:GetService("Players").LocalPlayer:GetMouse()

		local selectedColor = Color3.new(0.321569, 0.333333, 1)
		local deselectedColor = Color3.new(0.8, 0.8, 0.8)
		--- So things are descending
		local layoutOrderNum = 999999999
		--- Whether or not the gui is closing
		local mainClosing = false
		--- Whether or not the gui is closed (defaults to false)
		local closed = false
		--- Whether or not the sidebar is closing
		local sideClosing = false
		--- Whether or not the sidebar is closed (defaults to true but opens automatically on remote selection)
		local sideClosed = false
		--- Whether or not the code box is maximized (defaults to false)
		local maximized = false
		--- The event logs to be read from
		local logs = {}
		--- The event currently selected.Log (defaults to nil)
		local selected = nil
		--- The blacklist (can be a string name or the Remote Instance)
		local blacklist = {}
		--- The block list (can be a string name or the Remote Instance)
		local blocklist = {}
		--- Whether or not to add getNil function
		local getNil = false
		--- Array of remotes (and original functions) connected to
		local connectedRemotes = {}
		--- True = hookfunction, false = namecall
		local toggle = false
		local gm = getrawmetatable(game)
		local original = gm.__namecall
		setreadonly(gm, false)
		--- used to prevent recursives
		local prevTables = {}
		--- holds logs (for deletion)
		local remoteLogs = {}
		--- used for hookfunction
		local remoteEvent = Instance.new("RemoteEvent")
		--- used for hookfunction
		local remoteFunction = Instance.new("RemoteFunction")
		local originalEvent = remoteEvent.FireServer
		local originalFunction = remoteFunction.InvokeServer
		--- the maximum amount of remotes allowed in logs
		_G.SIMPLESPYCONFIG_MaxRemotes = 500
		--- how many spaces to indent
		local indent = 4
		--- used for task scheduler
		local scheduled = {}
		--- RBXScriptConnect of the task scheduler
		local schedulerconnect
		local SimpleSpy = {}
		local topstr = ""
		local bottomstr = ""
		local remotesFadeIn
		local rightFadeIn
		local codebox
		local p
		local getnilrequired = false

		-- autoblock variables
		local autoblock = false
		local history = {}
		local excluding = {}

		-- function info variables
		local funcEnabled = true

		-- remote hooking/connecting api variables
		local remoteSignals = {}
		local remoteHooks = {}

		-- original mouse icon
		local oldIcon = Mouse.Icon

		-- if mouse inside gui
		local mouseInGui = false

		-- handy array of RBXScriptConnections to disconnect on shutdown
		local connections = {}

		-- whether or not SimpleSpy uses 'getcallingscript()' to get the script (default is false because detection)
		local useGetCallingScript = false

		-- functions

		--- Converts arguments to a string and generates code that calls the specified method with them, recommended to be used in conjunction with ValueToString (method must be a string, e.g. `game:GetService("ReplicatedStorage").Remote:FireServer`)
		--- @param method string
		--- @param args any[]
		--- @return string
		function SimpleSpy:ArgsToString(method, args)
			assert(typeof(method) == "string", "string expected, got " .. typeof(method))
			assert(typeof(args) == "table", "table expected, got " .. typeof(args))
			return v2v({args = args}) .. "\n\n" .. method .. "(unpack(args))"
		end

		--- Converts a value to variables with the specified index as the variable name (if nil/invalid then the name will be assigned automatically)
		--- @param t any[]
		--- @return string
		function SimpleSpy:TableToVars(t)
			assert(typeof(t) == "table", "table expected, got " .. typeof(t))
			return v2v(t)
		end

		--- Converts a value to a variable with the specified `variablename` (if nil/invalid then the name will be assigned automatically)
		--- @param value any
		--- @return string
		function SimpleSpy:ValueToVar(value, variablename)
			assert(variablename == nil or typeof(variablename) == "string", "string expected, got " .. typeof(variablename))
			if not variablename then
				variablename = 1
			end
			return v2v({[variablename] = value})
		end

		--- Converts any value to a string, cannot preserve function contents
		--- @param value any
		--- @return string
		function SimpleSpy:ValueToString(value)
			return v2s(value)
		end

		--- Generates the simplespy function info
		--- @param func function
		--- @return string
		function SimpleSpy:GetFunctionInfo(func)
			assert(typeof(func) == "function", "Instance expected, got " .. typeof(func))
			return v2v{functionInfo = {
				info = debug.getinfo(func),
				constants = debug.getconstants(func)
			}}
		end

		--- Gets the ScriptSignal for a specified remote being fired
		--- @param remote Instance
		function SimpleSpy:GetRemoteFiredSignal(remote)
			assert(typeof(remote) == "Instance", "Instance expected, got " .. typeof(remote))
			if not remoteSignals[remote] then
				remoteSignals[remote] = newSignal()
			end
			return remoteSignals[remote]
		end

		--- Allows for direct hooking of remotes **THIS CAN BE VERY DANGEROUS**
		--- @param remote Instance
		--- @param f function
		function SimpleSpy:HookRemote(remote, f)
			assert(typeof(remote) == "Instance", "Instance expected, got " .. typeof(remote))
			assert(typeof(f) == "function", "function expected, got " .. typeof(f))
			remoteHooks[remote] = f
		end

		--- Blocks the specified remote instance/string
		--- @param remote any
		function SimpleSpy:BlockRemote(remote)
			assert(typeof(remote) == "Instance" or typeof(remote) == "string", "Instance | string expected, got " .. typeof(remote))
			blocklist[remote] = true
		end

		--- Excludes the specified remote from logs (instance/string)
		--- @param remote any
		function SimpleSpy:ExcludeRemote(remote)
			assert(typeof(remote) == "Instance" or typeof(remote) == "string", "Instance | string expected, got " .. typeof(remote))
			blacklist[remote] = true
		end

		--- Creates a new ScriptSignal that can be connected to and fired
		--- @return table
		function newSignal()
			local connected = {}
			return {
				Connect = function(self, f)
					assert(connected, "Signal is closed")
					connected[tostring(f)] = f
					return setmetatable({
						Connected = true,
						Disconnect = function(self)
							if not connected then
								warn("Signal is already closed")
							end
							self.Connected = false
							connected[tostring(f)] = nil
						end
					},
					{
						__index = function(self, i)
							if i == "Connected" then
								return not not connected[tostring(f)]
							end
						end
					})
				end,
				Fire = function(self, ...)
					for _, f in pairs(connected) do
						coroutine.wrap(f)(...)
					end
				end
			}
		end

		--- Prevents remote spam from causing lag (clears logs after `_G.SIMPLESPYCONFIG_MaxRemotes` or 500 remotes)
		function clean()
			local max = _G.SIMPLESPYCONFIG_MaxRemotes
			if not typeof(max) == "number" and math.floor(max) ~= max then
				max = 500
			end
			if #remoteLogs > max then
				for i = 100, #remoteLogs do
					local v = remoteLogs[i]
					if typeof(v[1]) == "RBXScriptConnection" then
						v[1]:Disconnect()
					end
					if typeof(v[2]) == "Instance" then
						v[2]:Destroy()
					end
				end
				local newLogs = {}
				for i = 1, 100 do
					table.insert(newLogs, remoteLogs[i])
				end
				remoteLogs = newLogs
			end
		end

		--- Scales the ToolTip to fit containing text
		function scaleToolTip()
			local size = TextService:GetTextSize(TextLabel.Text, TextLabel.TextSize, TextLabel.Font, Vector2.new(196, math.huge))
			TextLabel.Size = UDim2.new(0, size.X, 0, size.Y)
			ToolTip.Size = UDim2.new(0, size.X + 4, 0, size.Y + 4)
		end

		--- Executed when the toggle button (the SimpleSpy logo) is hovered over
		function onToggleButtonHover()
			if not toggle then
				TweenService:Create(Simple, TweenInfo.new(0.5), {TextColor3 = Color3.fromRGB(252, 51, 51)}):Play()
			else
				TweenService:Create(Simple, TweenInfo.new(0.5), {TextColor3 = Color3.fromRGB(68, 206, 91)}):Play()
			end
		end

		--- Executed when the toggle button is unhovered over
		function onToggleButtonUnhover()
			TweenService:Create(Simple, TweenInfo.new(0.5), {TextColor3 = Color3.fromRGB(255, 255, 255)}):Play()
		end

		--- Executed when the X button is hovered over
		function onXButtonHover()
			TweenService:Create(CloseButton, TweenInfo.new(0.2), {BackgroundColor3 = Color3.fromRGB(255, 60, 60)}):Play()
		end

		--- Executed when the X button is unhovered over
		function onXButtonUnhover()
			TweenService:Create(CloseButton, TweenInfo.new(0.2), {BackgroundColor3 = Color3.fromRGB(37, 36, 38)}):Play()
		end

		--- Toggles the remote spy method (when button clicked)
		function onToggleButtonClick()
			if toggle then
				TweenService:Create(Simple, TweenInfo.new(0.5), {TextColor3 = Color3.fromRGB(252, 51, 51)}):Play()
			else
				TweenService:Create(Simple, TweenInfo.new(0.5), {TextColor3 = Color3.fromRGB(68, 206, 91)}):Play()
			end
			toggleSpyMethod()
		end

		--- Reconnects bringBackOnResize if the current viewport changes and also connects it initially
		function connectResize()
			local lastCam = workspace.CurrentCamera:GetPropertyChangedSignal("ViewportSize"):Connect(bringBackOnResize)
			workspace:GetPropertyChangedSignal("CurrentCamera"):Connect(function()
				lastCam:Disconnect()
				if workspace.CurrentCamera then
					lastCam = workspace.CurrentCamera:GetPropertyChangedSignal("ViewportSize"):Connect(bringBackOnResize)
				end
			end)
		end

		--- Brings gui back if it gets lost offscreen (connected to the camera viewport changing)
		function bringBackOnResize()
			local currentX = Background.AbsolutePosition.X
			local currentY = Background.AbsolutePosition.Y
			local viewportSize = workspace.CurrentCamera.ViewportSize
			if (currentX < 0) or (currentX > (viewportSize.X - (sideClosed and 131 or TopBar.AbsoluteSize.X))) then
				if currentX < 0 then
					currentX = 0
				else
					currentX = viewportSize.X - (sideClosed and 131 or TopBar.AbsoluteSize.X)
				end
			end
			if (currentY < 0) or (currentY > (viewportSize.Y - (closed and 19 or Background.AbsoluteSize.Y) - 36)) then
				if currentY < 0 then
					currentY = 0
				else
					currentY = viewportSize.Y - (closed and 19 or Background.AbsoluteSize.Y) - 36
				end
			end
			TweenService.Create(TweenService, Background, TweenInfo.new(0.1), {Position = UDim2.new(0, currentX, 0, currentY)}):Play()
		end

		--- Drags gui (so long as mouse is held down)
		function onBarInput(input)
			if input.UserInputType == Enum.UserInputType.MouseButton1 then
				local lastPos = UserInputService.GetMouseLocation(UserInputService)
				local mainPos = Background.AbsolutePosition
				local offset = mainPos - lastPos
				local currentPos = offset + lastPos
				RunService.BindToRenderStep(RunService, "drag", 1,
					function()
						local newPos = UserInputService.GetMouseLocation(UserInputService)
						if newPos ~= lastPos then
							local currentX = (offset + newPos).X
							local currentY = (offset + newPos).Y
							local viewportSize = workspace.CurrentCamera.ViewportSize
							if (currentX < 0 and currentX < currentPos.X) or (currentX > (viewportSize.X - (sideClosed and 131 or TopBar.AbsoluteSize.X)) and currentX > currentPos.X) then
								if currentX < 0 then
									currentX = 0
								else
									currentX = viewportSize.X - (sideClosed and 131 or TopBar.AbsoluteSize.X)
								end
							end
							if (currentY < 0 and currentY < currentPos.Y) or (currentY > (viewportSize.Y - (closed and 19 or Background.AbsoluteSize.Y) - 36) and currentY > currentPos.Y) then
								if currentY < 0 then
									currentY = 0
								else
									currentY = viewportSize.Y - (closed and 19 or Background.AbsoluteSize.Y) - 36
								end
							end
							currentPos = Vector2.new(currentX, currentY)
							lastPos = newPos
							TweenService.Create(TweenService, Background, TweenInfo.new(0.1), {Position = UDim2.new(0, currentPos.X, 0, currentPos.Y)}):Play()
						end
						if not UserInputService:IsMouseButtonPressed(Enum.UserInputType.MouseButton1) then
							RunService.UnbindFromRenderStep(RunService, "drag")
						end
					end
				)
			end
		end

		--- Fades out the table of elements (and makes them invisible), returns a function to make them visible again
		function fadeOut(elements)
			local data = {}
			for _, v in pairs(elements) do
				if typeof(v) == "Instance" and v:IsA("GuiObject") and v.Visible then
					coroutine.wrap(function()
						data[v] = {
							BackgroundTransparency = v.BackgroundTransparency
						}
						TweenService:Create(v, TweenInfo.new(0.5), {BackgroundTransparency = 1}):Play()
						if v:IsA("TextBox") or v:IsA("TextButton") or v:IsA("TextLabel") then
							data[v].TextTransparency = v.TextTransparency
							TweenService:Create(v, TweenInfo.new(0.5), {TextTransparency = 1}):Play()
						elseif v:IsA("ImageButton") or v:IsA("ImageLabel") then
							data[v].ImageTransparency = v.ImageTransparency
							TweenService:Create(v, TweenInfo.new(0.5), {ImageTransparency = 1}):Play()
						end
						wait(0.5)
						v.Visible = false
						for i, x in pairs(data[v]) do
							v[i] = x
						end
						data[v] = true
					end)()
				end
			end
			return function()
				for i, _ in pairs(data) do
					coroutine.wrap(function()
						local properties = {
							BackgroundTransparency = i.BackgroundTransparency
						}
						i.BackgroundTransparency = 1
						TweenService:Create(i, TweenInfo.new(0.5), {BackgroundTransparency = properties.BackgroundTransparency}):Play()
						if i:IsA("TextBox") or i:IsA("TextButton") or i:IsA("TextLabel") then
							properties.TextTransparency = i.TextTransparency
							i.TextTransparency = 1
							TweenService:Create(i, TweenInfo.new(0.5), {TextTransparency = properties.TextTransparency}):Play()
						elseif i:IsA("ImageButton") or i:IsA("ImageLabel") then
							properties.ImageTransparency = i.ImageTransparency
							i.ImageTransparency = 1
							TweenService:Create(i, TweenInfo.new(0.5), {ImageTransparency = properties.ImageTransparency}):Play()
						end
						i.Visible = true
					end)()
				end
			end
		end

		--- Expands and minimizes the gui (closed is the toggle boolean)
		function toggleMinimize(override)
			if mainClosing and not override or maximized then
				return
			end
			mainClosing = true
			closed = not closed
			if closed then
				if not sideClosed then
					toggleSideTray(true)
				end
				LeftPanel.Visible = true
				TweenService:Create(LeftPanel, TweenInfo.new(0.5), {Size = UDim2.new(0, 131, 0, 0)}):Play()
				wait(0.5)
				remotesFadeIn = fadeOut(LeftPanel:GetDescendants())
				wait(0.5)
			else
				TweenService:Create(LeftPanel, TweenInfo.new(0.5), {Size = UDim2.new(0, 131, 0, 249)}):Play()
				wait(0.5)
				if remotesFadeIn then
					remotesFadeIn()
					remotesFadeIn = nil
				end
				bringBackOnResize()
			end
			mainClosing = false
		end

		--- Expands and minimizes the sidebar (sideClosed is the toggle boolean)
		function toggleSideTray(override)
			if sideClosing and not override or maximized then
				return
			end
			sideClosing = true
			sideClosed = not sideClosed
			if sideClosed then
				rightFadeIn = fadeOut(RightPanel:GetDescendants())
				wait(0.5)
				minimizeSize(0.5)
				wait(0.5)
				RightPanel.Visible = false
			else
				if closed then
					toggleMinimize(true)
				end
				RightPanel.Visible = true
				maximizeSize(0.5)
				wait(0.5)
				if rightFadeIn then
					rightFadeIn()
				end
				bringBackOnResize()
			end
			sideClosing = false
		end

		--- Expands code box to fit screen for more convenient viewing
		function toggleMaximize()
			if not sideClosed and not maximized then
				maximized = true
				local disable = Instance.new("TextButton")
				local prevSize = UDim2.new(0, CodeBox.AbsoluteSize.X, 0, CodeBox.AbsoluteSize.Y)
				local prevPos = UDim2.new(0,CodeBox.AbsolutePosition.X, 0, CodeBox.AbsolutePosition.Y)
				disable.Size = UDim2.new(1, 0, 1, 0)
				disable.BackgroundColor3 = Color3.new()
				disable.BorderSizePixel = 0
				disable.Text = 0
				disable.ZIndex = 3
				disable.BackgroundTransparency = 1
				disable.AutoButtonColor = false
				CodeBox.ZIndex = 4
				CodeBox.Position = prevPos
				CodeBox.Size = prevSize
				TweenService:Create(CodeBox, TweenInfo.new(0.5), {Size = UDim2.new(0.5, 0, 0.5, 0), Position = UDim2.new(0.25, 0, 0.25, 0)}):Play()
				TweenService:Create(disable, TweenInfo.new(0.5), {BackgroundTransparency = 0.5}):Play()
				disable.MouseButton1Click:Connect(function()
					if UserInputService:GetMouseLocation().Y + 36 >= CodeBox.AbsolutePosition.Y and UserInputService:GetMouseLocation().Y + 36 <= CodeBox.AbsolutePosition.Y + CodeBox.AbsoluteSize.Y
						and UserInputService:GetMouseLocation().X >= CodeBox.AbsolutePosition.X and UserInputService:GetMouseLocation().X <= CodeBox.AbsolutePosition.X + CodeBox.AbsoluteSize.X then
						return
					end
					TweenService:Create(CodeBox, TweenInfo.new(0.5), {Size = prevSize, Position = prevPos}):Play()
					TweenService:Create(disable, TweenInfo.new(0.5), {BackgroundTransparency = 1}):Play()
					wait(0.5)
					disable:Destroy()
					CodeBox.Size = UDim2.new(1, 0, 0.5, 0)
					CodeBox.Position = UDim2.new(0, 0, 0, 0)
					CodeBox.ZIndex = 0
					maximized = false
				end)
			end
		end

		--- Checks if cursor is within resize range
		--- @param p Vector2
		function isInResizeRange(p)
			local relativeP = p - Background.AbsolutePosition
			local range = 5
			if relativeP.X >= TopBar.AbsoluteSize.X - range and relativeP.Y >= Background.AbsoluteSize.Y - range
				and relativeP.X <= TopBar.AbsoluteSize.X and relativeP.Y <= Background.AbsoluteSize.Y then
				return true, 'B'
			elseif relativeP.X >= TopBar.AbsoluteSize.X - range and relativeP.X <= Background.AbsoluteSize.X then
				return true, 'X'
			elseif relativeP.Y >= Background.AbsoluteSize.Y - range and relativeP.Y <= Background.AbsoluteSize.Y then
				return true, 'Y'
			end
			return false
		end

		--- Called when mouse enters SimpleSpy
		function mouseEntered()
			local customCursor = Instance.new("ImageLabel")
			customCursor.Size = UDim2.fromOffset(200, 200)
			customCursor.ZIndex = 100000
			customCursor.BackgroundTransparency = 1
			customCursor.Image = ""
			customCursor.Parent = SimpleSpy2
			UserInputService.OverrideMouseIconBehavior = Enum.OverrideMouseIconBehavior.ForceHide
			RunService:BindToRenderStep("SIMPLESPY_CURSOR", 1, function()
				if mouseInGui and _G.SimpleSpyExecuted then
					local mouseLocation = UserInputService:GetMouseLocation() - Vector2.new(0, 36)
					customCursor.Position = UDim2.fromOffset(mouseLocation.X - customCursor.AbsoluteSize.X / 2, mouseLocation.Y - customCursor.AbsoluteSize.Y / 2)
					local inRange, type = isInResizeRange(mouseLocation)
					if inRange and not sideClosed and not closed then
						customCursor.Image = type == 'B' and "rbxassetid://6065821980" or type == 'X' and "rbxassetid://6065821086" or type == 'Y' and "rbxassetid://6065821596"
					elseif inRange and not closed and type == 'Y' or type == 'B' then
						customCursor.Image = "rbxassetid://6065821596"
					elseif customCursor.Image ~= "rbxassetid://6065775281" then
						customCursor.Image = "rbxassetid://6065775281"
					end
				else
					UserInputService.OverrideMouseIconBehavior = Enum.OverrideMouseIconBehavior.None
					customCursor:Destroy()
					RunService:UnbindFromRenderStep("SIMPLESPY_CURSOR")
				end
			end)
		end

		--- Called when mouse moves
		function mouseMoved()
			local mousePos = UserInputService:GetMouseLocation() - Vector2.new(0, 36)
			if not closed
				and mousePos.X >= TopBar.AbsolutePosition.X and mousePos.X <= TopBar.AbsolutePosition.X + TopBar.AbsoluteSize.X
				and mousePos.Y >= Background.AbsolutePosition.Y and mousePos.Y <= Background.AbsolutePosition.Y + Background.AbsoluteSize.Y then
				if not mouseInGui then
					mouseInGui = true
					mouseEntered()
				end
			else
				mouseInGui = false
			end
		end

		--- Adjusts the ui elements to the 'Maximized' size
		function maximizeSize(speed)
			if not speed then
				speed = 0.05
			end
			TweenService:Create(LeftPanel, TweenInfo.new(speed), { Size = UDim2.fromOffset(LeftPanel.AbsoluteSize.X, Background.AbsoluteSize.Y - TopBar.AbsoluteSize.Y) }):Play()
			TweenService:Create(RightPanel, TweenInfo.new(speed), { Size = UDim2.fromOffset(Background.AbsoluteSize.X - LeftPanel.AbsoluteSize.X, Background.AbsoluteSize.Y - TopBar.AbsoluteSize.Y) }):Play()
			TweenService:Create(TopBar, TweenInfo.new(speed), { Size = UDim2.fromOffset(Background.AbsoluteSize.X, TopBar.AbsoluteSize.Y) }):Play()
			TweenService:Create(ScrollingFrame, TweenInfo.new(speed), { Size = UDim2.fromOffset(Background.AbsoluteSize.X - LeftPanel.AbsoluteSize.X, 110), Position = UDim2.fromOffset(0, Background.AbsoluteSize.Y - 119 - TopBar.AbsoluteSize.Y) }):Play()
			TweenService:Create(CodeBox, TweenInfo.new(speed), { Size = UDim2.fromOffset(Background.AbsoluteSize.X - LeftPanel.AbsoluteSize.X, Background.AbsoluteSize.Y - 119 - TopBar.AbsoluteSize.Y) }):Play()
			TweenService:Create(LogList, TweenInfo.new(speed), { Size = UDim2.fromOffset(LogList.AbsoluteSize.X, Background.AbsoluteSize.Y - TopBar.AbsoluteSize.Y - 18) }):Play()
		end

		--- Adjusts the ui elements to close the side
		function minimizeSize(speed)
			if not speed then
				speed = 0.05
			end
			TweenService:Create(LeftPanel, TweenInfo.new(speed), { Size = UDim2.fromOffset(LeftPanel.AbsoluteSize.X, Background.AbsoluteSize.Y - TopBar.AbsoluteSize.Y) }):Play()
			TweenService:Create(RightPanel, TweenInfo.new(speed), { Size = UDim2.fromOffset(0, Background.AbsoluteSize.Y - TopBar.AbsoluteSize.Y) }):Play()
			TweenService:Create(TopBar, TweenInfo.new(speed), { Size = UDim2.fromOffset(LeftPanel.AbsoluteSize.X, TopBar.AbsoluteSize.Y) }):Play()
			TweenService:Create(ScrollingFrame, TweenInfo.new(speed), { Size = UDim2.fromOffset(0, 119), Position = UDim2.fromOffset(0, Background.AbsoluteSize.Y - 119 - TopBar.AbsoluteSize.Y) }):Play()
			TweenService:Create(CodeBox, TweenInfo.new(speed), { Size = UDim2.fromOffset(0, Background.AbsoluteSize.Y - 119 - TopBar.AbsoluteSize.Y) }):Play()
			TweenService:Create(LogList, TweenInfo.new(speed), { Size = UDim2.fromOffset(LogList.AbsoluteSize.X, Background.AbsoluteSize.Y - TopBar.AbsoluteSize.Y - 18) }):Play()
		end

		--- Called on user input while mouse in 'Background' frame
		--- @param input InputObject
		function backgroundUserInput(input)
			local inRange, type = isInResizeRange(UserInputService:GetMouseLocation() - Vector2.new(0, 36))
			if input.UserInputType == Enum.UserInputType.MouseButton1 and inRange then
				local lastPos = UserInputService:GetMouseLocation()
				local offset = Background.AbsoluteSize - lastPos
				local currentPos = lastPos + offset
				RunService:BindToRenderStep("SIMPLESPY_RESIZE", 1, function()
					local newPos = UserInputService:GetMouseLocation()
					if newPos ~= lastPos then
						local currentX = (newPos + offset).X
						local currentY = (newPos + offset).Y
						if currentX < 450 then
							currentX = 450
						end
						if currentY < 268 then
							currentY = 268
						end
						currentPos = Vector2.new(currentX, currentY)
						Background.Size = UDim2.fromOffset((not sideClosed and not closed and (type == "X" or type == "B")) and currentPos.X or Background.AbsoluteSize.X, (--[[(not sideClosed or currentPos.X <= LeftPanel.AbsolutePosition.X + LeftPanel.AbsoluteSize.X) and]] not closed and (type == "Y" or type == "B")) and currentPos.Y or Background.AbsoluteSize.Y)
						if sideClosed then
							minimizeSize()
						else
							maximizeSize()
						end
						lastPos = newPos
					end
				end)
				table.insert(connections, UserInputService.InputEnded:Connect(function(inputE)
					if input == inputE then
						RunService:UnbindFromRenderStep("SIMPLESPY_RESIZE")
					end
				end))
			end
		end

		--- Gets the player an instance is descended from
		function getPlayerFromInstance(instance)
			for _, v in pairs(Players:GetPlayers()) do
				if v.Character and (instance:IsDescendantOf(v.Character) or instance == v.Character) then
					return v
				end
			end
		end

		--- Runs on MouseButton1Click of an event frame
		function eventSelect(frame)
			if selected and selected.Log  then
				TweenService:Create(selected.Log.Button, TweenInfo.new(0.5), {BackgroundColor3 = Color3.fromRGB(0, 0, 0)}):Play()
				selected = nil
			end
			for _, v in pairs(logs) do
				if frame == v.Log then
					selected = v
				end
			end
			if selected and selected.Log then
				TweenService:Create(frame.Button, TweenInfo.new(0.5), {BackgroundColor3 = Color3.fromRGB(92, 126, 229)}):Play()
				codebox:setRaw(selected.GenScript)
			end
			if sideClosed then
				toggleSideTray()
			end
		end

		--- Updates the canvas size to fit the current amount of function buttons
		function updateFunctionCanvas()
			ScrollingFrame.CanvasSize = UDim2.fromOffset(UIGridLayout.AbsoluteContentSize.X, UIGridLayout.AbsoluteContentSize.Y)
		end

		--- Updates the canvas size to fit the amount of current remotes
		function updateRemoteCanvas()
			LogList.CanvasSize = UDim2.fromOffset(UIListLayout.AbsoluteContentSize.X, UIListLayout.AbsoluteContentSize.Y)
		end

		--- Allows for toggling of the tooltip and easy setting of le description
		--- @param enable boolean
		--- @param text string
		function makeToolTip(enable, text)
			if enable then
				if ToolTip.Visible then
					ToolTip.Visible = false
					RunService:UnbindFromRenderStep("ToolTip")
				end
				local first = true
				RunService:BindToRenderStep("ToolTip", 1, function()
					local topLeft = Vector2.new(Mouse.X + 20, Mouse.Y + 20)
					local bottomRight = topLeft + ToolTip.AbsoluteSize
					if topLeft.X < 0 then
						topLeft = Vector2.new(0, topLeft.Y)
					elseif bottomRight.X > workspace.CurrentCamera.ViewportSize.X then
						topLeft = Vector2.new(workspace.CurrentCamera.ViewportSize.X - ToolTip.AbsoluteSize.X, topLeft.Y)
					end
					if topLeft.Y < 0 then
						topLeft = Vector2.new(topLeft.X, 0)
					elseif bottomRight.Y > workspace.CurrentCamera.ViewportSize.Y - 35 then
						topLeft = Vector2.new(topLeft.X, workspace.CurrentCamera.ViewportSize.Y - ToolTip.AbsoluteSize.Y - 35)
					end
					if topLeft.X <= Mouse.X and topLeft.Y <= Mouse.Y then
						topLeft = Vector2.new(Mouse.X - ToolTip.AbsoluteSize.X - 2, Mouse.Y - ToolTip.AbsoluteSize.Y - 2)
					end
					if first then
						ToolTip.Position = UDim2.fromOffset(topLeft.X, topLeft.Y)
						first = false
					else
						ToolTip:TweenPosition(UDim2.fromOffset(topLeft.X, topLeft.Y), "Out", "Linear", 0.1)
					end
				end)
				TextLabel.Text = text
				ToolTip.Visible = true
			else
				if ToolTip.Visible then
					ToolTip.Visible = false
					RunService:UnbindFromRenderStep("ToolTip")
				end
			end
		end

		--- Creates new function button (below codebox)
		--- @param name string
		---@param description function
		---@param onClick function
		function newButton(name, description, onClick)
			local button = FunctionTemplate:Clone()
			button.Text.Text = name
			button.Button.MouseEnter:Connect(function()
				makeToolTip(true, description())
			end)
			button.Button.MouseLeave:Connect(function()
				makeToolTip(false)
			end)
			button.AncestryChanged:Connect(function()
				makeToolTip(false)
			end)
			button.Button.MouseButton1Click:Connect(function(...)
				onClick(button, ...)
			end)
			button.Parent = ScrollingFrame
			updateFunctionCanvas()
		end

		--- Adds new Remote to logs
		--- @param name string The name of the remote being logged
		--- @param type string The type of the remote being logged (either 'function' or 'event')
		--- @param gen_script any
		--- @param remote any
		--- @param function_info string
		--- @param blocked any
		function newRemote(type, name, gen_script, remote, function_info, blocked, src)
			local remoteFrame = RemoteTemplate:Clone()
			remoteFrame.Text.Text = name
			remoteFrame.ColorBar.BackgroundColor3 = type == "event" and Color3.new(255, 242, 0) or Color3.fromRGB(99, 86, 245)
			local id = Instance.new("IntValue")
			id.Name = "ID"
			id.Value = #logs + 1
			id.Parent = remoteFrame
			logs[#logs + 1] = {
				Name = name,
				GenScript = gen_script,
				Function = function_info,
				Remote = remote,
				Log = remoteFrame,
				Blocked = blocked,
				Source = src
			}
			if blocked then
				logs[#logs].GenScript = "-- THIS REMOTE WAS PREVENTED FROM FIRING THE SERVER BY SIMPLESPY\n\n" .. logs[#logs].GenScript
			end
			local connect = remoteFrame.Button.MouseButton1Click:Connect(function()
				eventSelect(remoteFrame)
			end)
			if layoutOrderNum < 1 then
				layoutOrderNum = 999999999
			end
			remoteFrame.LayoutOrder = layoutOrderNum
			layoutOrderNum = layoutOrderNum - 1
			remoteFrame.Parent = LogList
			table.insert(remoteLogs, 1, {connect, remoteFrame})
			clean()
			updateRemoteCanvas()
		end

		--- Generates a script from the provided arguments (first has to be remote path)
		function genScript(remote, ...)
			prevTables = {}
			local gen = ""
			local args = {...}
			if #args > 0 then
				if not pcall(function()
						gen = v2v({args = args}) .. "\n"
					end)
				then
					gen = gen .. "-- TableToString failure! Reverting to legacy functionality (results may vary)\nlocal args = {"
					if
						not pcall(
							function()
								for i, v in pairs(args) do
									if type(i) ~= "Instance" and type(i) ~= "userdata" then
										gen = gen .. "\n    [" .. tostring(i) .. "] = "
									elseif type(i) == "string" then
										gen = gen .. '\n    ["' .. tostring(i) .. '"] = '
									elseif type(i) == "userdata" and typeof(i) ~= "Instance" then
										gen = gen .. "\n    [" .. typeof(i) .. ".new(" .. tostring(i) .. ")] = "
									elseif type(i) == "userdata" then
										gen = gen .. "\n    [game." .. i:GetFullName() .. ")] = "
									end
									if type(v) ~= "Instance" and type(v) ~= "userdata" then
										gen = gen .. tostring(v)
									elseif type(v) == "string" then
										gen = gen .. '"' .. tostring(v) .. '"'
									elseif type(v) == "userdata" and typeof(v) ~= "Instance" then
										gen = gen .. typeof(v) .. ".new(" .. tostring(v) .. ")"
									elseif type(v) == "userdata" then
										gen = gen .. "game." .. v:GetFullName()
									end
								end
								gen = gen .. "\n}\n\n"
							end
						)
					then
						gen = gen .. "}\n-- Legacy tableToString failure! Unable to decompile."
					end
				end
				if not remote:IsDescendantOf(game) and not getnilrequired then
					gen = "function getNil(name,class) for _,v in pairs(getnilinstances())do if v.ClassName==class and v.Name==name then return v;end end end\n\n" .. gen
				end
				if remote:IsA("RemoteEvent") then
					gen = gen .. v2s(remote) .. ":FireServer(unpack(args))"
				elseif remote:IsA("RemoteFunction") then
					gen = gen .. v2s(remote) .. ":InvokeServer(unpack(args))"
				end
			else
				if remote:IsA("RemoteEvent") then
					gen = gen .. v2s(remote) .. ":FireServer()"
				elseif remote:IsA("RemoteFunction") then
					gen = gen .. v2s(remote) .. ":InvokeServer()"
				end
			end
			gen = "" .. gen
			prevTables = {}
			return gen
		end

		--- value-to-string: value, string (out), level (indentation), parent table, var name, is from tovar
		function v2s(v, l, p, n, vtv, i, pt, path, tables)
			if typeof(v) == "number" then
				if v == math.huge then
					return "math.huge"
				elseif tostring(v):match("nan") then
					return "0/0 --[[NaN]]"
				end
				return tostring(v)
			elseif typeof(v) == "boolean" then
				return tostring(v)
			elseif typeof(v) == "string" then
				return formatstr(v)
			elseif typeof(v) == "function" then
				return f2s(v)
			elseif typeof(v) == "table" then
				return t2s(v, l, p, n, vtv, i, pt, path, tables)
			elseif typeof(v) == "Instance" then
				return i2p(v)
			elseif typeof(v) == "userdata" then
				return "newproxy(true)"
			elseif type(v) == "userdata" then
				return u2s(v)
			else
				return "nil --[[" .. typeof(v) .. "]]"
			end
		end

		--- value-to-variable
		--- @param t any
		function v2v(t)
			topstr = ""
			bottomstr = ""
			getnilrequired = false
			local ret = ""
			local count = 1
			for i, v in pairs(t) do
				if type(i) == "string" and i:match("^[%a_]+[%w_]*$") then
					ret = ret .. "local " .. i .. " = " .. v2s(v, nil, nil, i, true) .. "\n"
				elseif tostring(i):match("^[%a_]+[%w_]*$") then
					ret = ret .. "local " .. tostring(i):lower() .. "_" .. tostring(count) .. " = " .. v2s(v, nil, nil, tostring(i):lower() .. "_" .. tostring(count), true) .. "\n"
				else
					ret = ret .. "local " .. type(v) .. "_" .. tostring(count) .. " = " .. v2s(v, nil, nil, type(v) .. "_" .. tostring(count), true) .. "\n"
				end
				count = count + 1
			end
			if getnilrequired then
				topstr = "function getNil(name,class) for _,v in pairs(getnilinstances())do if v.ClassName==class and v.Name==name then return v;end end end\n" .. topstr
			end
			if #topstr > 0 then
				ret = topstr .. "\n" .. ret
			end
			if #bottomstr > 0 then
				ret = ret .. bottomstr
			end
			return ret
		end

		--- table-to-string
		--- @param t table
		--- @param l number
		--- @param p table
		--- @param n string
		--- @param vtv boolean
		--- @param i any
		--- @param pt table
		--- @param path string
		--- @param tables table
		function t2s(t, l, p, n, vtv, i, pt, path, tables)
			for k, x in pairs(getrenv()) do
				local isgucci, gpath
				if rawequal(x, t) then
					isgucci, gpath = true, ""
				elseif type(x) == "table" then
					isgucci, gpath = v2p(t, x)
				end
				if isgucci then
					if type(k) == "string" and k:match("^[%a_]+[%w_]*$") then
						return k .. gpath
					else
						return "getrenv()[" .. v2s(k) .. "]" .. gpath
					end
				end
			end
			if not path then
				path = ""
			end
			if not l then
				l = 0
				tables = {}
			end
			if not p then
				p = t
			end
			for _, v in pairs(tables) do
				if n and rawequal(v, t) then
					bottomstr = bottomstr .. "\n" .. tostring(n) .. tostring(path) .. " = " .. tostring(n) .. tostring(({v2p(v, p)})[2])
					return "{} --[[DUPLICATE]]"
				end
			end
			table.insert(tables, t)
			local s =  "{"
			local size = 0
			l = l + indent
			for k, v in pairs(t) do
				size = size + 1
				if size > (_G.SimpleSpyMaxTableSize and _G.SimpleSpyMaxTableSize or 1000) then
					break
				end
				if rawequal(k, t) then
					bottomstr = bottomstr .. "\n" .. tostring(n) .. tostring(path) .. "[" .. tostring(n) .. tostring(path) .. "]" .. " = " .. (v == k and tostring(n) .. tostring(path) or v2s(v, l, p, n, vtv, k, t, path .. "[" .. tostring(n) .. tostring(path) .. "]", tables))
					size -= 1
					continue
				end
				local currentPath = ""
				if type(k) == "string" and k:match("^[%a_]+[%w_]*$") then
					currentPath = "." .. k
				else
					currentPath = "[" .. v2s(k, nil, p, n, vtv, i, pt, path) .. "]"
				end
				s = s .. "\n" .. string.rep(" ", l) .. "[" .. v2s(k, l, p, n, vtv, k, t, path .. currentPath, tables) .. "] = " .. v2s(v, l, p, n, vtv, k, t, path .. currentPath, tables) .. ","
			end
			if #s > 1 then
				s = s:sub(1, #s - 1)
			end
			if size > 0 then
				s = s .. "\n" .. string.rep(" ", l - indent)
			end
			return s .. "}"
		end

		--- function-to-string
		function f2s(f)
			for k, x in pairs(getgenv()) do
				local isgucci, gpath
				if rawequal(x, f) then
					isgucci, gpath = true, ""
				elseif type(x) == "table" then
					isgucci, gpath = v2p(f, x)
				end
				if isgucci then
					if type(k) == "string" and k:match("^[%a_]+[%w_]*$") then
						return k .. gpath
					else
						return "getgenv()[" .. v2s(k) .. "]" .. gpath
					end
				end
			end
			-- uwu some cool stuff here once bork finishes up
			-- if SimpleSpy.GetExternalLoader then
			--     local ExternalLoader = SimpleSpy:GetExternalLoader()
			--     local loaded, path = pcall(function() ExternalLoader:LoadAsset("Bork_Functions") end)
			--     if loaded then
			--         local functions = loadfile(path .. "functions.lua")
			--         local out = functions[f]
			--         if out then
			--             return out
			--         end
			--     end
			-- end
			-- local isgucci, gpath = v2p(f, getgc())
			-- if isgucci then
			--     return "getgc()" .. gpath
			-- end
			if debug.getinfo(f).name:match("^[%a_]+[%w_]*$") then
				return "function()end --[[" .. debug.getinfo(f).name .. "]]"
			end
			return "function()end --[[" .. tostring(f) .. "]]"
		end

		--- instance-to-path
		--- @param i userdata
		function i2p(i)
			local player = getplayer(i)
			local parent = i
			local out = ""
			if parent == nil then
				return "nil"
			elseif player then
				while true do
					if parent and parent == player.Character then
						if player == Players.LocalPlayer then
							return 'game:GetService("Players").LocalPlayer.Character' .. out
						else
							return i2p(player) .. ".Character" .. out
						end
					else
						if parent.Name:match("[%a_]+[%w+]*") ~= parent.Name then
							out = '[' .. formatstr(parent.Name) .. ']' .. out
						else
							out = "." .. parent.Name .. out
						end
					end
					parent = parent.Parent
				end
			elseif parent ~= game then
				while true do
					if parent and parent.Parent == game then
						if game:GetService(parent.ClassName) then
							if parent.ClassName == "Workspace" then
								return "workspace" .. out
							else
								return 'game:GetService("' .. parent.ClassName .. '")' .. out
							end
						else
							if parent.Name:match("[%a_]+[%w_]*") then
								return "game." .. parent.Name .. out
							else
								return 'game[' .. formatstr(parent.Name) .. ']' .. out
							end
						end
					elseif parent.Parent == nil then
						getnilrequired = true
						return 'getNil(' .. formatstr(parent.Name) .. ', "' .. parent.ClassName .. '")' .. out
					elseif parent == Players.LocalPlayer then
						out = ".LocalPlayer" .. out
					else
						if parent.Name:match("[%a_]+[%w_]*") ~= parent.Name then
							out = '[' .. formatstr(parent.Name) .. ']' .. out
						else
							out = "." .. parent.Name .. out
						end
					end
					parent = parent.Parent
				end
			else
				return "game"
			end
		end

		--- userdata-to-string: userdata
		--- @param u userdata
		function u2s(u)
			if typeof(u) == "TweenInfo" then
				-- TweenInfo
				return "TweenInfo.new(" ..tostring(u.Time) .. ", Enum.EasingStyle." .. tostring(u.EasingStyle) .. ", Enum.EasingDirection." .. tostring(u.EasingDirection) .. ", " .. tostring(u.RepeatCount) .. ", " .. tostring(u.Reverses) .. ", " .. tostring(u.DelayTime) .. ")"
			elseif typeof(u) == "Ray" then
				-- Ray
				return "Ray.new(" .. u2s(u.Origin) .. ", " .. u2s(u.Direction) .. ")"
			elseif typeof(u) == "NumberSequence" then
				-- NumberSequence
				local ret = "NumberSequence.new("
				for i, v in pairs(u.KeyPoints) do
					ret = ret .. tostring(v)
					if i < #u.Keypoints then
						ret = ret .. ", "
					end
				end
				return ret .. ")"
			elseif typeof(u) == "DockWidgetPluginGuiInfo" then
				-- DockWidgetPluginGuiInfo
				return "DockWidgetPluginGuiInfo.new(Enum.InitialDockState" .. tostring(u) .. ")"
			elseif typeof(u) == "ColorSequence" then
				-- ColorSequence
				local ret = "ColorSequence.new("
				for i, v in pairs(u.KeyPoints) do
					ret = ret .. "Color3.new(" .. tostring(v) .. ")"
					if i < #u.Keypoints then
						ret = ret .. ", "
					end
				end
				return ret .. ")"
			elseif typeof(u) == "BrickColor" then
				-- BrickColor
				return "BrickColor.new(" .. tostring(u.Number) .. ")"
			elseif typeof(u) == "NumberRange" then
				-- NumberRange
				return "NumberRange.new(" .. tostring(u.Min) .. ", " .. tostring(u.Max) .. ")"
			elseif typeof(u) == "Region3" then
				-- Region3
				local center = u.CFrame.Position
				local size = u.CFrame.Size
				local vector1 = center - size / 2
				local vector2 = center + size / 2
				return "Region3.new(" .. u2s(vector1) .. ", " .. u2s(vector2) .. ")"
			elseif typeof(u) == "Faces" then
				-- Faces
				local faces = {}
				if u.Top then
					table.insert(faces, "Enum.NormalId.Top")
				end
				if u.Bottom then
					table.insert(faces, "Enum.NormalId.Bottom")
				end
				if u.Left then
					table.insert(faces, "Enum.NormalId.Left")
				end
				if u.Right then
					table.insert(faces, "Enum.NormalId.Right")
				end
				if u.Back then
					table.insert(faces, "Enum.NormalId.Back")
				end
				if u.Front then
					table.insert(faces, "Enum.NormalId.Front")
				end
				return "Faces.new(" .. table.concat(faces, ", ") .. ")"
			elseif typeof(u) == "EnumItem" then
				return tostring(u)
			elseif typeof(u) == "Enums" then
				return "Enum"
			elseif typeof(u) == "Enum" then
				return "Enum." .. tostring(u)
			elseif typeof(u) == "RBXScriptSignal" then
				return "nil --[[RBXScriptSignal]]"
			elseif typeof(u) == "Vector3" then
				return string.format("Vector3.new(%s, %s, %s)", v2s(u.X), v2s(u.Y), v2s(u.Z))
			elseif typeof(u) == "CFrame" then
				return string.format("CFrame.new(%s, %s)", v2s(u.Position), v2s(u.LookVector))
			elseif typeof(u) == "DockWidgetPluginGuiInfo" then
				return string.format("DockWidgetPluginGuiInfo(%s, %s, %s, %s, %s, %s, %s)", "Enum.InitialDockState.Right", v2s(u.InitialEnabled), v2s(u.InitialEnabledShouldOverrideRestore), v2s(u.FloatingXSize), v2s(u.FloatingYSize), v2s(u.MinWidth), v2s(u.MinHeight))
			elseif typeof(u) == "RBXScriptConnection" then
				return "nil --[[RBXScriptConnection " .. tostring(u) .. "]]"
			elseif typeof(u) == "RaycastResult" then
				return "nil --[[RaycastResult " .. tostring(u) .. "]]"
			elseif typeof(u) == "PathWaypoint" then
				return string.format("PathWaypoint.new(%s, %s)", v2s(u.Position), v2s(u.Action))
			else
				return typeof(u) .. ".new(" .. tostring(u) .. ")"
			end
		end

		--- Gets the player an instance is descended from
		function getplayer(instance)
			for _, v in pairs(Players:GetPlayers()) do
				if v.Character and (instance:IsDescendantOf(v.Character) or instance == v.Character) then
					return v
				end
			end
		end

		--- value-to-path (in table)
		function v2p(x, t, path, prev)
			if not path then
				path = ""
			end
			if not prev then
				prev = {}
			end
			if rawequal(x, t) then
				return true, ""
			end
			for i, v in pairs(t) do
				if rawequal(v, x) then
					if type(i) == "string" and i:match("^[%a_]+[%w_]*$") then
						return true, (path .. "." .. i)
					else
						return true, (path .. "[" .. v2s(i) .. "]")
					end
				end
				if type(v) == "table" then
					local duplicate = false
					for _, y in pairs(prev) do
						if rawequal(y, v) then
							duplicate = true
						end
					end
					if not duplicate then
						table.insert(prev, t)
						local found
						found, p = v2p(x, v, path, prev)
						if found then
							if type(i) == "string" and i:match("^[%a_]+[%w_]*$") then
								return true, "." .. i .. p
							else
								return true, "[" .. v2s(i) .. "]" .. p
							end
						end
					end
				end
			end
			return false, ""
		end

		--- format s: string, byte encrypt (for weird symbols)
		function formatstr(s)
			return '"' .. handlespecials(s) .. '"'
		end

		--- Adds \'s to the text as a replacement to whitespace chars and other things because string.format can't yayeet
		function handlespecials(s)
			local i = 0
			repeat
				i = i + 1
				local char = s:sub(i, i)
				if string.byte(char) then
					if char == "\n" then
						s = s:sub(0, i - 1) .. "\\n" .. s:sub(i + 1, -1)
						i = i + 1
					elseif char == "\t" then
						s = s:sub(0, i - 1) .. "\\t" .. s:sub(i + 1, -1)
						i = i + 1
					elseif char == "\\" then
						s = s:sub(0, i - 1) .. "\\\\" .. s:sub(i + 1, -1)
						i = i + 1
					elseif char == '"' then
						s = s:sub(0, i - 1) .. '\\"' .. s:sub(i + 1, -1)
						i = i + 1
					elseif string.byte(char) > 126 or string.byte(char) < 32 then
						s = s:sub(0, i - 1) .. "\\" .. string.byte(char) .. s:sub(i + 1, -1)
						i = i + #tostring(string.byte(char))
					end
				end
			until char == ""
			return s
		end

		--- finds script from 'src' from getinfo, returns nil if not found
		--- @param src string
		function getScriptFromSrc(src)
			local realPath
			local runningTest
			--- @type number
			local s, e
			local match = false
			if src:sub(1, 1) == "=" then
				realPath = game
				s = 2
			else
				runningTest = src:sub(2, e and e - 1 or -1)
				for _, v in pairs(getnilinstances()) do
					if v.Name == runningTest then
						realPath = v
						break
					end
				end
				s = #runningTest + 1
			end
			if realPath then
				e = src:sub(s, -1):find("%.")
				local i = 0
				repeat
					i += 1
					if not e then
						runningTest = src:sub(s, -1)
						local test = realPath.FindFirstChild(realPath, runningTest)
						if test then
							realPath = test
						end
						match = true
					else
						runningTest = src:sub(s, e)
						local test = realPath.FindFirstChild(realPath, runningTest)
						local yeOld = e
						if test then
							realPath = test
							s = e + 2
							e = src:sub(e + 2, -1):find("%.")
							e = e and e + yeOld or e
						else
							e = src:sub(e + 2, -1):find("%.")
							e = e and e + yeOld or e
						end
					end
				until match or i >= 50
			end
			return realPath
		end

		--- schedules the provided function (and calls it with any args after)
		function schedule(f, ...)
			table.insert(scheduled, {f, ...})
		end

		--- the big (well tbh small now) boi task scheduler himself, handles p much anything as quicc as possible
		function taskscheduler()
			if not toggle then
				scheduled = {}
				return
			end
			if #scheduled > 1000 then
				table.remove(scheduled, #scheduled)
			end
			if #scheduled > 0 then
				local currentf = scheduled[1]
				table.remove(scheduled, 1)
				if type(currentf) == "table" and type(currentf[1]) == "function" then
					pcall(unpack(currentf))
				end
			end
		end

		--- Handles remote logs
		function remoteHandler(hookfunction, methodName, remote, args, func, calling)
			if remote:IsA("RemoteEvent") or remote:IsA("RemoteFunction") then
				if funcEnabled and not calling then
					_, calling = pcall(getScriptFromSrc, debug.getinfo(func).source)
				end
				coroutine.wrap(function()
					if remoteSignals[remote] then
						remoteSignals[remote]:Fire(args)
					end
				end)()
				if autoblock then
					if excluding[remote] then
						return
					end
					if not history[remote] then
						history[remote] = {badOccurances = 0, lastCall = tick()}
					end
					if tick() - history[remote].lastCall < 1 then
						history[remote].badOccurances += 1
						return
					else
						history[remote].badOccurances = 0
					end
					if history[remote].badOccurances > 3 then
						excluding[remote] = true
						return
					end
					history[remote].lastCall = tick()
				end
				local functionInfoStr
				local src
				if func and islclosure(func) then
					local functionInfo = {}
					pcall(function() functionInfo.info = debug.getinfo(func) end)
					pcall(function() functionInfo.constants = debug.getconstants(func) end)
					pcall(function() functionInfoStr = v2v{functionInfo = functionInfo} end)
					pcall(function() if type(calling) == "userdata" then src = calling end end)
				end
				if methodName:lower() == "fireserver" then
					newRemote("event", remote.Name, genScript(remote, table.unpack(args)), remote, functionInfoStr, (blocklist[remote] or blocklist[remote.Name]), src)
				elseif methodName:lower() == "invokeserver" then
					newRemote("function", remote.Name, genScript(remote, table.unpack(args)), remote, functionInfoStr, (blocklist[remote] or blocklist[remote.Name]), src)
				end
			end
		end

		--- Used for hookfunction
		function hookRemote(remoteType, remote, ...)
			local args = {...}
			if remoteHooks[remote] then
				args = remoteHooks[remote](args)
			end
			if typeof(remote) == "Instance" and not (blacklist[remote] or blacklist[remote.Name]) then
				local func
				local calling
				if funcEnabled then
					func = debug.getinfo(4).func
					calling = useGetCallingScript and getcallingscript() or nil
				end
				schedule(remoteHandler, true, remoteType == "RemoteEvent" and "fireserver" or "invokeserver", remote, args, func, calling)
				if (blocklist[remote] or blocklist[remote.Name]) then
					return
				end
			end
			if remoteType == "RemoteEvent" then
				if remoteHooks[remote] then
					return originalEvent(remote, unpack(args))
				end
				return originalEvent(remote, ...)
			else
				if remoteHooks[remote] then
					return originalFunction(remote, unpack(args))
				end
				return originalFunction(remote, ...)
			end
		end

		local newnamecall = newcclosure(function(...)
			local args = {...}
			local methodName = getnamecallmethod()
			local remote = args[1]
			if (methodName:lower() == "invokeserver" or methodName:lower() == "fireserver") and not (blacklist[remote] or blacklist[remote.Name]) then
				if remoteHooks[remote] then
					args = remoteHooks[remote]({args, unpack(args, 2)})
				end
				local func
				local calling
				if funcEnabled then
					func = debug.getinfo(3).func
					calling = useGetCallingScript and getcallingscript() or nil
				end
				coroutine.wrap(function()
					schedule(remoteHandler, false, methodName, remote, {unpack(args, 2)}, func, calling)
				end)()
			end
			if typeof(remote) == "Instance" and (methodName:lower() == "invokeserver" or methodName:lower() == "fireserver") and (blocklist[remote] or blocklist[remote.Name]) then
				return nil
			elseif (methodName:lower() == "invokeserver" or methodName:lower() == "fireserver") and remoteHooks[remote] then
				return original(unpack(args))
			else
				return original(...)
			end
		end)

		local newFireServer = newcclosure(function(...) return hookRemote("RemoteEvent", ...) end)

		local newInvokeServer = newcclosure(function(...) return hookRemote("RemoteFunction", ...) end)

		--- Toggles on and off the remote spy
		function toggleSpy()
			if not toggle then
				setreadonly(gm, false)
				if not original then
					original = gm.__namecall
					if not original then
						warn("SimpleSpy: namecall method not found!\n")
						onToggleButtonClick()
						return
					end
				end
				gm.__namecall = newnamecall
				originalEvent = hookfunction(remoteEvent.FireServer, newFireServer)
				originalFunction = hookfunction(remoteFunction.InvokeServer, newInvokeServer)
			else
				setreadonly(gm, false)
				gm.__namecall = original
				hookfunction(remoteEvent.FireServer, originalEvent)
				hookfunction(remoteFunction.InvokeServer, originalFunction)
			end
		end

		--- Toggles between the two remotespy methods (hookfunction currently = disabled)
		function toggleSpyMethod()
			toggleSpy()
			toggle = not toggle
		end

		--- Shuts down the remote spy
		function shutdown()
			if schedulerconnect then
				schedulerconnect:Disconnect()
			end
			for _, connection in pairs(connections) do
				coroutine.wrap(function()
					connection:Disconnect()
				end)()
			end
			setreadonly(gm, false)
			SimpleSpy2:Destroy()
			hookfunction(remoteEvent.FireServer, originalEvent)
			hookfunction(remoteFunction.InvokeServer, originalFunction)
			gm.__namecall = original
			_G.SimpleSpyExecuted = false
		end

		-- main
		if not _G.SimpleSpyExecuted then
			local succeeded, err = pcall(function()
				_G.SimpleSpyShutdown = shutdown
				ContentProvider:PreloadAsync({"rbxassetid://6065821980", "rbxassetid://6065774948", "rbxassetid://6065821086", "rbxassetid://6065821596", ImageLabel, ImageLabel_2, ImageLabel_3})
				onToggleButtonClick()
				RemoteTemplate.Parent = nil
				FunctionTemplate.Parent = nil
				codebox = Highlight.new(CodeBox)
				codebox:setRaw("")
				getgenv().SimpleSpy = SimpleSpy
				TextLabel:GetPropertyChangedSignal("Text"):Connect(scaleToolTip)
				TopBar.InputBegan:Connect(onBarInput)
				MinimizeButton.MouseButton1Click:Connect(toggleMinimize)
				MaximizeButton.MouseButton1Click:Connect(toggleSideTray)
				Simple.MouseButton1Click:Connect(onToggleButtonClick)
				CloseButton.MouseEnter:Connect(onXButtonHover)
				CloseButton.MouseLeave:Connect(onXButtonUnhover)
				Simple.MouseEnter:Connect(onToggleButtonHover)
				Simple.MouseLeave:Connect(onToggleButtonUnhover)
				CloseButton.MouseButton1Click:Connect(shutdown)
				table.insert(connections, UserInputService.InputBegan:Connect(backgroundUserInput))
				table.insert(connections, Mouse.Move:Connect(mouseMoved))
				connectResize()
				SimpleSpy2.Enabled = true
				coroutine.wrap(function()
					wait(1)
					onToggleButtonUnhover()
				end)()
				schedulerconnect = RunService.Heartbeat:Connect(taskscheduler)
				if syn and syn.protect_gui then pcall(syn.protect_gui, SimpleSpy2) end
				SimpleSpy2.Parent = gethui and gethui() or CoreGui
			end)
			if succeeded then
				_G.SimpleSpyExecuted = true
			else
				warn("A fatal error has occured, SimpleSpy was unable to launch properly.\nPlease DM this error message to @exx#9394:\n\n" .. tostring(err))
				SimpleSpy2:Destroy()
				hookfunction(remoteEvent.FireServer, originalEvent)
				hookfunction(remoteFunction.InvokeServer, originalFunction)
				gm.__namecall = original
				return
			end
		else
			SimpleSpy2:Destroy()
			return
		end

		----- ADD ONS ----- (easily add or remove additonal functionality to the RemoteSpy!)
--[[
    Some helpful things:
        - add your function in here, and create buttons for them through the 'newButton' function
        - the first argument provided is the TextButton the player clicks to run the function
        - generated scripts are generated when the namecall is initially fired and saved in remoteFrame objects
        - blacklisted remotes will be ignored directly in namecall (less lag)
        - the properties of a 'remoteFrame' object:
            {
                Name: (string) The name of the Remote
                GenScript: (string) The generated script that appears in the codebox (generated when namecall fired)
                Source: (Instance (LocalScript)) The script that fired/invoked the remote
                Remote: (Instance (RemoteEvent) | Instance (RemoteFunction)) The remote that was fired/invoked
                Log: (Instance (TextButton)) The button being used for the remote (same as 'selected.Log')
            }
        - globals list: (contact @exx#9394 for more information or if you have suggestions for more to be added)
            - closed: (boolean) whether or not the GUI is currently minimized
            - logs: (table[remoteFrame]) full of remoteFrame objects (properties listed above)
            - selected: (remoteFrame) the currently selected remoteFrame (properties listed above)
            - blacklist: (string[] | Instance[] (RemoteEvent) | Instance[] (RemoteFunction)) an array of blacklisted names and remotes
            - codebox: (Instance (TextBox)) the textbox that holds all the code- cleared often
]]
		-- Copies the contents of the codebox
		newButton(
			"Copy Code",
			function() return "Click to copy code" end,
			function()
				setclipboard(codebox:getString())
				TextLabel.Text = "Copied successfully!"
			end
		)

		--- Copies the source script (that fired the remote)
		newButton(
			"Copy Remote",
			function() return "Click to copy the path of the remote" end,
			function()
				if selected then
					setclipboard(v2s(selected.Remote))
					TextLabel.Text = "Copied!"
				end
			end
		)

		-- Executes the contents of the codebox through loadstring
		newButton(
			"Run Code",
			function() return "Click to execute code" end,
			function()
				local orText = "Click to execute code"
				TextLabel.Text = "Executing..."
				local succeeded = pcall(function() return loadstring(codebox:getString())() end)
				if succeeded then
					TextLabel.Text = "Executed successfully!"
				else
					TextLabel.Text = "Execution error!"
				end
			end
		)

		--- Gets the calling script (not super reliable but w/e)
		newButton(
			"Get Script",
			function() return "Click to copy calling script to clipboard\nWARNING: Not super reliable, nil == could not find" end,
			function()
				if selected then
					setclipboard(SimpleSpy:ValueToString(selected.Source))
					TextLabel.Text = "Done!"
				end
			end
		)

		--- Decompiles the script that fired the remote and puts it in the code box
		newButton(
			"Function Info",
			function() return "Click to view calling function information" end,
			function()
				if selected then
					if selected.Function then
						codebox:setRaw("-- Calling function info\n-- Generated by the SimpleSpy serializer\n\n" .. tostring(selected.Function))
					end
					TextLabel.Text = "Done! Function info generated by the SimpleSpy Serializer."
				end
			end
		)

		--- Clears the Remote logs
		newButton(
			"Clr Logs",
			function() return "Click to clear logs" end,
			function()
				TextLabel.Text = "Clearing..."
				logs = {}
				for _, v in pairs(LogList:GetChildren()) do
					if not v:IsA("UIListLayout") then
						v:Destroy()
					end
				end
				codebox:setRaw("")
				selected = nil
				TextLabel.Text = "Logs cleared!"
			end
		)

		--- Excludes the selected.Log Remote from the RemoteSpy
		newButton(
			"Exclude (i)",
			function() return "Click to exclude this Remote" end,
			function()
				if selected then
					blacklist[selected.Remote] = true
					TextLabel.Text = "Excluded!"
				end
			end
		)

		--- Excludes all Remotes that share the same name as the selected.Log remote from the RemoteSpy
		newButton(
			"Exclude (n)",
			function() return "Click to exclude all remotes with this name" end,
			function()
				if selected then
					blacklist[selected.Name] = true
					TextLabel.Text = "Excluded!"
				end
			end
		)

		--- clears blacklist
		newButton(
			"Clr Blacklist",
			function() return "Click to clear the blacklist" end,
			function()
				blacklist = {}
				TextLabel.Text = "Blacklist cleared!"
			end
		)

		--- Prevents the selected.Log Remote from firing the server (still logged)
		newButton(
			"Block (i)",
			function() return "Click to stop this remote from firing" end,
			function()
				if selected then
					blocklist[selected.Remote] = true
					TextLabel.Text = "Excluded!"
				end
			end
		)

		--- Prevents all remotes from firing that share the same name as the selected.Log remote from the RemoteSpy (still logged)
		newButton(
			"Block (n)",
			function() return "Click to stop remotes with this name from firing" end,
			function()
				if selected then
					blocklist[selected.Name] = true
					TextLabel.Text = "Excluded!"
				end
			end
		)

		--- clears blacklist
		newButton(
			"Clr Blocklist",
			function() return "Click to stop blocking remotes" end,
			function()
				blocklist = {}
				TextLabel.Text = "Blocklist cleared!"
			end
		)

		--- Attempts to decompile the source script
		newButton(
			"Decompile",
			function() return "Attempts to decompile source script\nWARNING: Not super reliable, nil == could not find" end,
			function()
				if selected then
					if selected.Source then
						codebox:setRaw(decompile(selected.Source))
						TextLabel.Text = "Done!"
					else
						TextLabel.Text = "Source not found!"
					end
				end
			end
		)

		newButton(
			"Disable Info",
			function() return string.format("[%s] Toggle function info (because it can cause lag in some games)", funcEnabled and "ENABLED" or "DISABLED") end,
			function()
				funcEnabled = not funcEnabled
				TextLabel.Text = string.format("[%s] Toggle function info (because it can cause lag in some games)", funcEnabled and "ENABLED" or "DISABLED")
			end
		)

		newButton(
			"Autoblock",
			function() return string.format("[%s] [BETA] Intelligently detects and excludes spammy remote calls from logs", autoblock and "ENABLED" or "DISABLED") end,
			function()
				autoblock = not autoblock
				TextLabel.Text = string.format("[%s] [BETA] Intelligently detects and excludes spammy remote calls from logs", autoblock and "ENABLED" or "DISABLED")
				history = {}
				excluding = {}
			end
		)

		newButton(
			"CallingScript",
			function() return string.format("[%s] [UNSAFE] Uses 'getcallingscript' to get calling script for Decompile and GetScript. Much more reliable, but opens up SimpleSpy to detection and/or instability.", useGetCallingScript and "ENABLED" or "DISABLED") end,
			function()
				useGetCallingScript = not useGetCallingScript
				TextLabel.Text = string.format("[%s] [UNSAFE] Uses 'getcallingscript' to get calling script for Decompile and GetScript. Much more reliable, but opens up SimpleSpy to detection and/or instability.", useGetCallingScript and "ENABLED" or "DISABLED")
			end
		)

	end           
})
local Section = EspTab:AddSection({
	Name = "Esp/Visual"
})
EspTab:AddButton({
	Name = "Esp V1",
	Callback = function()
		loadstring(game:HttpGet('https://raw.githubusercontent.com/ic3w0lf22/Unnamed-ESP/master/UnnamedESP.lua'))()
	end    
})
JogadorTab:AddButton({
	Name = "Kill/Explode All Hub (Explode)",
	Callback = function()
		loadstring(game:HttpGetAsync("https://pastebin.com/raw/A34Z7gMx"))()
	end       
})
local Section = JogadorTab:AddSection({
	Name = "Opção Mapa"
})

JogadorTab:AddButton({
	Name = "Free cam Bind R",
	Callback = function()
		local allowspeedmove = true
		wait(1)

		local c = workspace.CurrentCamera
		local player = game.Players.LocalPlayer
		local userInput = game:GetService("UserInputService")
		local rs = game:GetService("RunService")
		local starterPlayer = game:GetService("StarterPlayer")
		--local util = LoadLibrary("RbxUtility")
		--local camSync = util.CreateSignal()

		local selected = false
		local speed = 60
		local lastUpdate = 0

		local camera = Instance.new('Part', workspace)
		camera.CanCollide = false
		camera.Anchored = true
		camera.Transparency = 1
		camera.Name = 'FreeCam'
		camera.Position = player.Character.HumanoidRootPart.Position + Vector3.new(0,5,0)
		--rs:BindToRenderStep("CamSync",190,function ()
		--	camSync:fire()
		--end)

		c.Changed:connect(function (property)
			if property == "CoordinateFrame" then
				--		camSync:fire()
			end
		end)

		function getNextMovement(deltaTime)
			local nextMove = Vector3.new()
			-- Left/Right
			if userInput:IsKeyDown("A") or userInput:IsKeyDown("Left") then
				nextMove = nextMove + Vector3.new(-1,0,0)
			end
			if userInput:IsKeyDown("D") or userInput:IsKeyDown("Right") then
				nextMove = nextMove + Vector3.new(1,0,0)
			end
			-- Forward/Back
			if userInput:IsKeyDown("W") or userInput:IsKeyDown("Up") then
				nextMove = nextMove + Vector3.new(0,0,-1)
			end
			if userInput:IsKeyDown("S") or userInput:IsKeyDown("Down") then
				nextMove = nextMove + Vector3.new(0,0,1)
			end
			-- Up/Down
			if userInput:IsKeyDown("Space") or userInput:IsKeyDown("Q") then
				nextMove = nextMove + Vector3.new(0,1,0)
			end
			if userInput:IsKeyDown("LeftControl") or userInput:IsKeyDown("E") then
				nextMove = nextMove + Vector3.new(0,-1,0)
			end
			return CFrame.new( nextMove * (speed * deltaTime) )
		end

		function onSelected()
			local char = player.Character
			if char then
				local root = camera
				currentPos = root.Position
				selected = true
				lastUpdate = tick()
				c.CameraSubject = root
				player.Character.HumanoidRootPart.Anchored = true
				while selected do
					local delta = tick()-lastUpdate
					local look = (c.Focus.p-c.CoordinateFrame.p).unit
					local move = getNextMovement(delta)
					local pos = root.Position
					root.CFrame = CFrame.new(pos,pos+look) * move
					lastUpdate = tick()
					wait(0.01)
					--	camSync:wait()
				end
				player.Character.HumanoidRootPart.Anchored = false
				c.CameraSubject = player.Character.Humanoid
				root.Velocity = Vector3.new()
			end
		end

		function onDeselected()
			selected = false
		end

		local isOn = true
		spawn(onSelected)

		function onKeyPressed(_,state)
			if state == Enum.UserInputState.Begin then
				isOn = not isOn
				if isOn then
					onSelected()
				else
					onDeselected()
				end
			end
		end

		local mouse = player:GetMouse()
		mouse.Button1Down:Connect(function()
			if allowspeedmove then speed = 120 end
		end)
		mouse.Button1Up:Connect(function()
			speed = 60
		end)

		function ResetCamera()
			camera.Position = player.Character.HumanoidRootPart.Position + Vector3.new(0,5,0)
		end

		game:GetService("ContextActionService"):BindAction("Noclip Toggle",onKeyPressed,false,"r")
		game:GetService("ContextActionService"):BindAction("Reset Camera Position",ResetCamera,false,"z")
	end             
})
EspTab:AddButton({
	Name = "Esp V2",
	Callback = function()
		loadstring(game:HttpGet(('https://raw.githubusercontent.com/Pedroxz63/espbypedroxz/main/README.md'),true))()
	end      
})
JogadorTab:AddButton({
	Name = "Fps Booster",
	Callback = function()
		local decalsyeeted = true -- Leaving this on makes games look shitty but the fps goes up by at least 20.
		local g = game
		local w = g.Workspace
		local l = g.Lighting
		local t = w.Terrain
		t.WaterWaveSize = 0
		t.WaterWaveSpeed = 0
		t.WaterReflectance = 0
		t.WaterTransparency = 0
		l.GlobalShadows = false
		l.FogEnd = 9000000000
		l.Brightness = 0
		settings().Rendering.QualityLevel = "Level01"
		for i,v in pairs(g:GetDescendants()) do
			if v:IsA("Part") or v:IsA("Union") or v:IsA("MeshPart") then
				v.Material = "Plastic"
				v.Reflectance = 0
			elseif v:IsA("Decal") and decalsyeeted then 
				v.Transparency = 1
			elseif v:IsA("ParticleEmitter") or v:IsA("Trail") then 
				v.Lifetime = NumberRange.new(0)
			end
		end
	end          
})
EspTab:AddButton({
	Name = "Esp V3",
	Callback = function()

		--- Tut

		local esp_settings = { ---- table for esp settings 
			textsize = 8,
			colour = 255,255,255
		}

		local gui = Instance.new("BillboardGui")
		local esp = Instance.new("TextLabel",gui) ---- new instances to make the billboard gui and the textlabel



		gui.Name = "Cracked esp"; ---- properties of the esp
		gui.ResetOnSpawn = false
		gui.AlwaysOnTop = true;
		gui.LightInfluence = 0;
		gui.Size = UDim2.new(1.75, 0, 1.75, 0);
		esp.BackgroundColor3 = Color3.fromRGB(255, 255, 255);
		esp.Text = ""
		esp.Size = UDim2.new(0.0001, 0.00001, 0.0001, 0.00001);
		esp.BorderSizePixel = 4;
		esp.BorderColor3 = Color3.new(esp_settings.colour)
		esp.BorderSizePixel = 0
		esp.Font = "GothamSemibold"
		esp.TextSize = esp_settings.textsize
		esp.TextColor3 = Color3.fromRGB(esp_settings.colour) -- text colour

		game:GetService("RunService").RenderStepped:Connect(function() ---- loops faster than a while loop :)
			for i,v in pairs (game:GetService("Players"):GetPlayers()) do
				if v ~= game:GetService("Players").LocalPlayer and v.Character.Head:FindFirstChild("Cracked esp")==nil  then -- craeting checks for team check, local player etc
					esp.Text = "{"..v.Name.."}"
					gui:Clone().Parent = v.Character.Head
				end
			end
		end)
	end              
})        
EspTab:AddButton({
	Name = "Esp V4 ",
	Callback = function()
		local custom_theme = {} --soon

		local function CreateInstance(cls,props)
			local inst = Instance.new(cls)
			for i,v in pairs(props) do
				inst[i] = v
			end
			return inst
		end

		local age1 = CreateInstance('ScreenGui',{DisplayOrder=0,Enabled=true,ResetOnSpawn=true,Name='age1', Parent=game.CoreGui})
		local p_visuals = CreateInstance('Frame',{Style=Enum.FrameStyle.Custom,Active=true,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(0.121569, 0.12549, 0.172549),BackgroundTransparency=0,BorderColor3=Color3.new(1, 0, 0.498039),BorderSizePixel=2,ClipsDescendants=false,Draggable=false,Position=UDim2.new(0, 50, 0, 60),Rotation=0,Selectable=false,Size=UDim2.new(0, 200, 0, 254),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name = 'p_visuals',Parent = age1})
		local UIListLayout = CreateInstance('UIListLayout', {Padding = UDim.new(0, 1), FillDirection = Enum.FillDirection.Vertical, HorizontalAlignment = Enum.HorizontalAlignment.Left, SortOrder = Enum.SortOrder.LayoutOrder, VerticalAlignment = Enum.VerticalAlignment.Top, Name = 'UIListLayout', Parent = p_visuals })
		local title1 = CreateInstance('TextLabel',{Font=Enum.Font.GothamBlack,FontSize=Enum.FontSize.Size18,Text='Player visuals',TextColor3=Color3.new(1, 1, 1),TextScaled=false,TextSize=18,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=false,TextXAlignment=Enum.TextXAlignment.Left,TextYAlignment=Enum.TextYAlignment.Center,Active=true,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(1, 0, 0.498039),BackgroundTransparency=0,BorderColor3=Color3.new(1, 0, 0.498039),BorderSizePixel=0,ClipsDescendants=false,Draggable=false,Position=UDim2.new(0, 0, 0, 0),Rotation=0,Selectable=true,Size=UDim2.new(1, 0, 0, 24),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='title1',Parent = p_visuals})
		local b_b = CreateInstance('TextButton',{Font=Enum.Font.SourceSans,FontSize=Enum.FontSize.Size18,Text='Bounding box',TextColor3=Color3.new(1, 0, 0.498039),TextScaled=false,TextSize=16,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=false,TextXAlignment=Enum.TextXAlignment.Left,TextYAlignment=Enum.TextYAlignment.Center,AutoButtonColor=true,Modal=false,Selected=false,Style=Enum.ButtonStyle.Custom,Active=false,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(1, 0, 0.498039),BackgroundTransparency=1,BorderColor3=Color3.new(1, 0, 0.498039),BorderSizePixel=0,ClipsDescendants=false,Draggable=false,Position=UDim2.new(0, 0, 0, 0),Rotation=0,Selectable=true,Size=UDim2.new(1, -2, 0, 18),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='b_b',Parent = p_visuals})
		local v = CreateInstance('TextLabel',{Font=Enum.Font.Gotham,FontSize=Enum.FontSize.Size14,Text='OFF',TextColor3=Color3.new(1, 0, 0),TextScaled=false,TextSize=14,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=false,TextXAlignment=Enum.TextXAlignment.Right,TextYAlignment=Enum.TextYAlignment.Center,Active=false,AnchorPoint=Vector2.new(1, 0),BackgroundColor3=Color3.new(1, 1, 1),BackgroundTransparency=1,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=1,ClipsDescendants=false,Draggable=false,Position=UDim2.new(1, 0, 0, 0),Rotation=0,Selectable=false,Size=UDim2.new(0, 18, 0, 18),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='v',Parent = b_b})
		local b_f = CreateInstance('TextButton',{Font=Enum.Font.SourceSans,FontSize=Enum.FontSize.Size18,Text='Fill alpha',TextColor3=Color3.new(1, 0, 0.498039),TextScaled=false,TextSize=16,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=false,TextXAlignment=Enum.TextXAlignment.Left,TextYAlignment=Enum.TextYAlignment.Center,AutoButtonColor=true,Modal=false,Selected=false,Style=Enum.ButtonStyle.Custom,Active=false,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(1, 0, 0.498039),BackgroundTransparency=1,BorderColor3=Color3.new(1, 0, 0.498039),BorderSizePixel=0,ClipsDescendants=false,Draggable=false,Position=UDim2.new(0, 0, 0, 0),Rotation=0,Selectable=true,Size=UDim2.new(1, -2, 0, 18),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='b_f',Parent = p_visuals})
		local v = CreateInstance('TextLabel',{Font=Enum.Font.Gotham,FontSize=Enum.FontSize.Size14,Text='OFF',TextColor3=Color3.new(1, 0, 0),TextScaled=false,TextSize=14,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=false,TextXAlignment=Enum.TextXAlignment.Right,TextYAlignment=Enum.TextYAlignment.Center,Active=false,AnchorPoint=Vector2.new(1, 0),BackgroundColor3=Color3.new(1, 1, 1),BackgroundTransparency=1,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=1,ClipsDescendants=false,Draggable=false,Position=UDim2.new(1, 0, 0, 0),Rotation=0,Selectable=false,Size=UDim2.new(0, 18, 0, 18),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='v',Parent = b_f})
		local b_rt = CreateInstance('TextButton',{Font=Enum.Font.SourceSans,FontSize=Enum.FontSize.Size18,Text='Render team',TextColor3=Color3.new(1, 0, 0.498039),TextScaled=false,TextSize=16,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=false,TextXAlignment=Enum.TextXAlignment.Left,TextYAlignment=Enum.TextYAlignment.Center,AutoButtonColor=true,Modal=false,Selected=false,Style=Enum.ButtonStyle.Custom,Active=false,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(1, 0, 0.498039),BackgroundTransparency=1,BorderColor3=Color3.new(1, 0, 0.498039),BorderSizePixel=0,ClipsDescendants=false,Draggable=false,Position=UDim2.new(0, 0, 0, 0),Rotation=0,Selectable=true,Size=UDim2.new(1, -2, 0, 18),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='b_rt',Parent = p_visuals})
		local v = CreateInstance('TextLabel',{Font=Enum.Font.Gotham,FontSize=Enum.FontSize.Size14,Text='OFF',TextColor3=Color3.new(1, 0, 0),TextScaled=false,TextSize=14,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=false,TextXAlignment=Enum.TextXAlignment.Right,TextYAlignment=Enum.TextYAlignment.Center,Active=false,AnchorPoint=Vector2.new(1, 0),BackgroundColor3=Color3.new(1, 1, 1),BackgroundTransparency=1,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=1,ClipsDescendants=false,Draggable=false,Position=UDim2.new(1, 0, 0, 0),Rotation=0,Selectable=false,Size=UDim2.new(0, 18, 0, 18),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='v',Parent = b_rt})
		local b_tc = CreateInstance('TextButton',{Font=Enum.Font.SourceSans,FontSize=Enum.FontSize.Size18,Text='Use TeamColor',TextColor3=Color3.new(1, 0, 0.498039),TextScaled=false,TextSize=16,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=false,TextXAlignment=Enum.TextXAlignment.Left,TextYAlignment=Enum.TextYAlignment.Center,AutoButtonColor=true,Modal=false,Selected=false,Style=Enum.ButtonStyle.Custom,Active=false,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(1, 0, 0.498039),BackgroundTransparency=1,BorderColor3=Color3.new(1, 0, 0.498039),BorderSizePixel=0,ClipsDescendants=false,Draggable=false,Position=UDim2.new(0, 0, 0, 0),Rotation=0,Selectable=true,Size=UDim2.new(1, -2, 0, 18),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='b_tc',Parent = p_visuals})
		local v = CreateInstance('TextLabel',{Font=Enum.Font.Gotham,FontSize=Enum.FontSize.Size14,Text='OFF',TextColor3=Color3.new(1, 0, 0),TextScaled=false,TextSize=14,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=false,TextXAlignment=Enum.TextXAlignment.Right,TextYAlignment=Enum.TextYAlignment.Center,Active=false,AnchorPoint=Vector2.new(1, 0),BackgroundColor3=Color3.new(1, 1, 1),BackgroundTransparency=1,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=1,ClipsDescendants=false,Draggable=false,Position=UDim2.new(1, 0, 0, 0),Rotation=0,Selectable=false,Size=UDim2.new(0, 18, 0, 18),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='v',Parent = b_tc})
		local b_sn = CreateInstance('TextButton',{Font=Enum.Font.SourceSans,FontSize=Enum.FontSize.Size18,Text='Show name',TextColor3=Color3.new(1, 0, 0.498039),TextScaled=false,TextSize=16,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=false,TextXAlignment=Enum.TextXAlignment.Left,TextYAlignment=Enum.TextYAlignment.Center,AutoButtonColor=true,Modal=false,Selected=false,Style=Enum.ButtonStyle.Custom,Active=false,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(1, 0, 0.498039),BackgroundTransparency=1,BorderColor3=Color3.new(1, 0, 0.498039),BorderSizePixel=0,ClipsDescendants=false,Draggable=false,Position=UDim2.new(0, 0, 0, 0),Rotation=0,Selectable=true,Size=UDim2.new(1, -2, 0, 18),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='b_sn',Parent = p_visuals})
		local v = CreateInstance('TextLabel',{Font=Enum.Font.Gotham,FontSize=Enum.FontSize.Size14,Text='OFF',TextColor3=Color3.new(1, 0, 0),TextScaled=false,TextSize=14,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=false,TextXAlignment=Enum.TextXAlignment.Right,TextYAlignment=Enum.TextYAlignment.Center,Active=false,AnchorPoint=Vector2.new(1, 0),BackgroundColor3=Color3.new(1, 1, 1),BackgroundTransparency=1,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=1,ClipsDescendants=false,Draggable=false,Position=UDim2.new(1, 0, 0, 0),Rotation=0,Selectable=false,Size=UDim2.new(0, 18, 0, 18),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='v',Parent = b_sn})
		local b_sd = CreateInstance('TextButton',{Font=Enum.Font.SourceSans,FontSize=Enum.FontSize.Size18,Text='Show distance',TextColor3=Color3.new(1, 0, 0.498039),TextScaled=false,TextSize=16,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=false,TextXAlignment=Enum.TextXAlignment.Left,TextYAlignment=Enum.TextYAlignment.Center,AutoButtonColor=true,Modal=false,Selected=false,Style=Enum.ButtonStyle.Custom,Active=false,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(1, 0, 0.498039),BackgroundTransparency=1,BorderColor3=Color3.new(1, 0, 0.498039),BorderSizePixel=0,ClipsDescendants=false,Draggable=false,Position=UDim2.new(0, 0, 0, 0),Rotation=0,Selectable=true,Size=UDim2.new(1, -2, 0, 18),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='b_sd',Parent = p_visuals})
		local v = CreateInstance('TextLabel',{Font=Enum.Font.Gotham,FontSize=Enum.FontSize.Size14,Text='OFF',TextColor3=Color3.new(1, 0, 0),TextScaled=false,TextSize=14,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=false,TextXAlignment=Enum.TextXAlignment.Right,TextYAlignment=Enum.TextYAlignment.Center,Active=false,AnchorPoint=Vector2.new(1, 0),BackgroundColor3=Color3.new(1, 1, 1),BackgroundTransparency=1,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=1,ClipsDescendants=false,Draggable=false,Position=UDim2.new(1, 0, 0, 0),Rotation=0,Selectable=false,Size=UDim2.new(0, 18, 0, 18),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='v',Parent = b_sd})
		local b_sh = CreateInstance('TextButton',{Font=Enum.Font.SourceSans,FontSize=Enum.FontSize.Size18,Text='Show health',TextColor3=Color3.new(1, 0, 0.498039),TextScaled=false,TextSize=16,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=false,TextXAlignment=Enum.TextXAlignment.Left,TextYAlignment=Enum.TextYAlignment.Center,AutoButtonColor=true,Modal=false,Selected=false,Style=Enum.ButtonStyle.Custom,Active=false,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(1, 0, 0.498039),BackgroundTransparency=1,BorderColor3=Color3.new(1, 0, 0.498039),BorderSizePixel=0,ClipsDescendants=false,Draggable=false,Position=UDim2.new(0, 0, 0, 0),Rotation=0,Selectable=true,Size=UDim2.new(1, -2, 0, 18),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='b_sh',Parent = p_visuals})
		local v = CreateInstance('TextLabel',{Font=Enum.Font.Gotham,FontSize=Enum.FontSize.Size14,Text='OFF',TextColor3=Color3.new(1, 0, 0),TextScaled=false,TextSize=14,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=false,TextXAlignment=Enum.TextXAlignment.Right,TextYAlignment=Enum.TextYAlignment.Center,Active=false,AnchorPoint=Vector2.new(1, 0),BackgroundColor3=Color3.new(1, 1, 1),BackgroundTransparency=1,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=1,ClipsDescendants=false,Draggable=false,Position=UDim2.new(1, 0, 0, 0),Rotation=0,Selectable=false,Size=UDim2.new(0, 18, 0, 18),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='v',Parent = b_sh})
		local b_ht = CreateInstance('TextButton',{Font=Enum.Font.SourceSans,FontSize=Enum.FontSize.Size18,Text='Health type',TextColor3=Color3.new(1, 0, 0.498039),TextScaled=false,TextSize=16,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=false,TextXAlignment=Enum.TextXAlignment.Left,TextYAlignment=Enum.TextYAlignment.Center,AutoButtonColor=true,Modal=false,Selected=false,Style=Enum.ButtonStyle.Custom,Active=false,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(1, 0, 0.498039),BackgroundTransparency=1,BorderColor3=Color3.new(1, 0, 0.498039),BorderSizePixel=0,ClipsDescendants=false,Draggable=false,Position=UDim2.new(0, 0, 0, 0),Rotation=0,Selectable=true,Size=UDim2.new(1, -2, 0, 18),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='b_ht',Parent = p_visuals})
		local v = CreateInstance('TextLabel',{Font=Enum.Font.SourceSans,FontSize=Enum.FontSize.Size18,Text='Text',TextColor3=Color3.new(0, 1, 1),TextScaled=false,TextSize=16,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=false,TextXAlignment=Enum.TextXAlignment.Right,TextYAlignment=Enum.TextYAlignment.Center,Active=false,AnchorPoint=Vector2.new(1, 0),BackgroundColor3=Color3.new(1, 1, 1),BackgroundTransparency=1,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=1,ClipsDescendants=false,Draggable=false,Position=UDim2.new(1, 0, 0, 0),Rotation=0,Selectable=false,Size=UDim2.new(0, 18, 0, 18),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='v',Parent = b_ht})
		local b_f_t = CreateInstance('TextButton',{Font=Enum.Font.SourceSans,FontSize=Enum.FontSize.Size18,Text='Fill transparency',TextColor3=Color3.new(1, 0, 0.498039),TextScaled=false,TextSize=16,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=false,TextXAlignment=Enum.TextXAlignment.Left,TextYAlignment=Enum.TextYAlignment.Center,AutoButtonColor=true,Modal=false,Selected=false,Style=Enum.ButtonStyle.Custom,Active=false,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(1, 0, 0.498039),BackgroundTransparency=1,BorderColor3=Color3.new(1, 0, 0.498039),BorderSizePixel=0,ClipsDescendants=false,Draggable=false,Position=UDim2.new(0, 0, 0, 0),Rotation=0,Selectable=true,Size=UDim2.new(1, -2, 0, 18),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='b_f_t',Parent = p_visuals})
		local v = CreateInstance('TextLabel',{Font=Enum.Font.Gotham,FontSize=Enum.FontSize.Size14,Text='1',TextColor3=Color3.new(0, 1, 1),TextScaled=false,TextSize=14,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=false,TextXAlignment=Enum.TextXAlignment.Right,TextYAlignment=Enum.TextYAlignment.Center,Active=false,AnchorPoint=Vector2.new(1, 0),BackgroundColor3=Color3.new(1, 1, 1),BackgroundTransparency=1,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=1,ClipsDescendants=false,Draggable=false,Position=UDim2.new(1, 0, 0, 0),Rotation=0,Selectable=false,Size=UDim2.new(0, 18, 0, 18),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='v',Parent = b_f_t})
		local title1_2 = CreateInstance('TextLabel',{Font=Enum.Font.SourceSansBold,FontSize=Enum.FontSize.Size18,Text='ESP',TextColor3=Color3.new(1, 0, 0.498039),TextScaled=false,TextSize=18,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=false,TextXAlignment=Enum.TextXAlignment.Left,TextYAlignment=Enum.TextYAlignment.Center,Active=false,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(0.121569, 0.12549, 0.172549),BackgroundTransparency=0,BorderColor3=Color3.new(1, 0, 0.498039),BorderSizePixel=1,ClipsDescendants=false,Draggable=false,Position=UDim2.new(0, 0, 0, 0),Rotation=0,Selectable=true,Size=UDim2.new(1, 0, 0, 18),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='title1_2',Parent = p_visuals})
		local b_ct = CreateInstance('TextLabel',{Font=Enum.Font.SourceSans,FontSize=Enum.FontSize.Size18,Text='Team color',TextColor3=Color3.new(1, 0, 0.498039),TextScaled=false,TextSize=16,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=false,TextXAlignment=Enum.TextXAlignment.Left,TextYAlignment=Enum.TextYAlignment.Center,Active=false,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(1, 0, 0.498039),BackgroundTransparency=1,BorderColor3=Color3.new(1, 0, 0.498039),BorderSizePixel=0,ClipsDescendants=false,Draggable=false,Position=UDim2.new(0, 0, 0, 0),Rotation=0,Selectable=true,Size=UDim2.new(1, -2, 0, 18),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='b_ct',Parent = p_visuals})
		local ct_b = CreateInstance('TextBox',{ClearTextOnFocus=true,Font=Enum.Font.Gotham,FontSize=Enum.FontSize.Size14,MultiLine=false,Text='',TextColor3=Color3.new(0, 0, 1), PlaceholderText='', PlaceholderColor3=Color3.new(0, 0, 1),TextScaled=false,TextSize=14,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=false,TextXAlignment=Enum.TextXAlignment.Center,TextYAlignment=Enum.TextYAlignment.Center,Active=true,AnchorPoint=Vector2.new(1, 0),BackgroundColor3=Color3.new(0.121569, 0.12549, 0.172549),BackgroundTransparency=0,BorderColor3=Color3.new(1, 0, 0.498039),BorderSizePixel=1,ClipsDescendants=false,Draggable=false,Position=UDim2.new(1, -2, 0, 2),Rotation=0,Selectable=true,Size=UDim2.new(0, 27, 0, 14),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='ct_b',Parent = b_ct})
		local ct_g = CreateInstance('TextBox',{ClearTextOnFocus=true,Font=Enum.Font.Gotham,FontSize=Enum.FontSize.Size14,MultiLine=false,Text='',TextColor3=Color3.new(0, 1, 0), PlaceholderText='', PlaceholderColor3=Color3.new(0, 1, 0),TextScaled=false,TextSize=14,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=false,TextXAlignment=Enum.TextXAlignment.Center,TextYAlignment=Enum.TextYAlignment.Center,Active=true,AnchorPoint=Vector2.new(1, 0),BackgroundColor3=Color3.new(0.121569, 0.12549, 0.172549),BackgroundTransparency=0,BorderColor3=Color3.new(1, 0, 0.498039),BorderSizePixel=1,ClipsDescendants=false,Draggable=false,Position=UDim2.new(1, -29, 0, 2),Rotation=0,Selectable=true,Size=UDim2.new(0, 27, 0, 14),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='ct_g',Parent = b_ct})
		local ct_r = CreateInstance('TextBox',{ClearTextOnFocus=true,Font=Enum.Font.Gotham,FontSize=Enum.FontSize.Size14,MultiLine=false,Text='',TextColor3=Color3.new(1, 0, 0), PlaceholderText='', PlaceholderColor3=Color3.new(1, 0, 0),TextScaled=false,TextSize=14,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=false,TextXAlignment=Enum.TextXAlignment.Center,TextYAlignment=Enum.TextYAlignment.Center,Active=true,AnchorPoint=Vector2.new(1, 0),BackgroundColor3=Color3.new(0.121569, 0.12549, 0.172549),BackgroundTransparency=0,BorderColor3=Color3.new(1, 0, 0.498039),BorderSizePixel=1,ClipsDescendants=false,Draggable=false,Position=UDim2.new(1, -56, 0, 2),Rotation=0,Selectable=true,Size=UDim2.new(0, 27, 0, 14),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='ct_r',Parent = b_ct})
		local b_ce = CreateInstance('TextLabel',{Font=Enum.Font.SourceSans,FontSize=Enum.FontSize.Size18,Text='Enemy color',TextColor3=Color3.new(1, 0, 0.498039),TextScaled=false,TextSize=16,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=false,TextXAlignment=Enum.TextXAlignment.Left,TextYAlignment=Enum.TextYAlignment.Center,Active=false,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(1, 0, 0.498039),BackgroundTransparency=1,BorderColor3=Color3.new(1, 0, 0.498039),BorderSizePixel=0,ClipsDescendants=false,Draggable=false,Position=UDim2.new(0, 0, 0, 0),Rotation=0,Selectable=true,Size=UDim2.new(1, -2, 0, 18),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='b_ce',Parent = p_visuals})
		local ce_b = CreateInstance('TextBox',{ClearTextOnFocus=true,Font=Enum.Font.Gotham,FontSize=Enum.FontSize.Size14,MultiLine=false,Text='',TextColor3=Color3.new(0, 0, 1), PlaceholderText='', PlaceholderColor3=Color3.new(0, 0, 1),TextScaled=false,TextSize=14,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=false,TextXAlignment=Enum.TextXAlignment.Center,TextYAlignment=Enum.TextYAlignment.Center,Active=true,AnchorPoint=Vector2.new(1, 0),BackgroundColor3=Color3.new(0.121569, 0.12549, 0.172549),BackgroundTransparency=0,BorderColor3=Color3.new(1, 0, 0.498039),BorderSizePixel=1,ClipsDescendants=false,Draggable=false,Position=UDim2.new(1, -2, 0, 2),Rotation=0,Selectable=true,Size=UDim2.new(0, 27, 0, 14),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='ce_b',Parent = b_ce})
		local ce_g = CreateInstance('TextBox',{ClearTextOnFocus=true,Font=Enum.Font.Gotham,FontSize=Enum.FontSize.Size14,MultiLine=false,Text='',TextColor3=Color3.new(0, 1, 0), PlaceholderText='', PlaceholderColor3=Color3.new(0, 1, 0),TextScaled=false,TextSize=14,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=false,TextXAlignment=Enum.TextXAlignment.Center,TextYAlignment=Enum.TextYAlignment.Center,Active=true,AnchorPoint=Vector2.new(1, 0),BackgroundColor3=Color3.new(0.121569, 0.12549, 0.172549),BackgroundTransparency=0,BorderColor3=Color3.new(1, 0, 0.498039),BorderSizePixel=1,ClipsDescendants=false,Draggable=false,Position=UDim2.new(1, -29, 0, 2),Rotation=0,Selectable=true,Size=UDim2.new(0, 27, 0, 14),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='ce_g',Parent = b_ce})
		local ce_r = CreateInstance('TextBox',{ClearTextOnFocus=true,Font=Enum.Font.Gotham,FontSize=Enum.FontSize.Size14,MultiLine=false,Text='',TextColor3=Color3.new(1, 0, 0), PlaceholderText='', PlaceholderColor3=Color3.new(1, 0, 0),TextScaled=false,TextSize=14,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=false,TextXAlignment=Enum.TextXAlignment.Center,TextYAlignment=Enum.TextYAlignment.Center,Active=true,AnchorPoint=Vector2.new(1, 0),BackgroundColor3=Color3.new(0.121569, 0.12549, 0.172549),BackgroundTransparency=0,BorderColor3=Color3.new(1, 0, 0.498039),BorderSizePixel=1,ClipsDescendants=false,Draggable=false,Position=UDim2.new(1, -56, 0, 2),Rotation=0,Selectable=true,Size=UDim2.new(0, 27, 0, 14),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=1,Name='ce_r',Parent = b_ce})
		local watermark = CreateInstance('TextLabel',{Font=Enum.Font.Code,FontSize=Enum.FontSize.Size14,Text='lamehaxx v0.01',TextColor3=Color3.new(0, 0, 0),TextScaled=false,TextSize=14,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=1,TextTransparency=0,TextWrapped=false,TextXAlignment=Enum.TextXAlignment.Left,TextYAlignment=Enum.TextYAlignment.Top,Active=false,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(1, 1, 1),BackgroundTransparency=1,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=1,ClipsDescendants=false,Draggable=false,Position=UDim2.new(0, 2, 0, -34),Rotation=0,Selectable=false,Size=UDim2.new(0, 200, 0, 20),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=20,Name='watermark',Parent = age1})
		local watermark1 = CreateInstance('TextLabel',{Font=Enum.Font.Code,FontSize=Enum.FontSize.Size14,Text='lamehaxx v0.01',TextColor3=Color3.new(1, 0, 0.498039),TextScaled=false,TextSize=14,TextStrokeColor3=Color3.new(0, 0, 0),TextStrokeTransparency=0,TextTransparency=0,TextWrapped=false,TextXAlignment=Enum.TextXAlignment.Left,TextYAlignment=Enum.TextYAlignment.Top,Active=false,AnchorPoint=Vector2.new(0, 0),BackgroundColor3=Color3.new(1, 1, 1),BackgroundTransparency=1,BorderColor3=Color3.new(0.105882, 0.164706, 0.207843),BorderSizePixel=1,ClipsDescendants=false,Draggable=false,Position=UDim2.new(0, -2, 0, -2),Rotation=0,Selectable=false,Size=UDim2.new(0, 200, 0, 20),SizeConstraint=Enum.SizeConstraint.RelativeXY,Visible=true,ZIndex=20,Name='watermark1',Parent = watermark})
		p_visuals.Draggable = true

		title1.LayoutOrder = 0 title1_2.LayoutOrder = 1
		b_b.LayoutOrder = 1 b_f.LayoutOrder = 2 b_f_t.LayoutOrder = 3 b_sd.LayoutOrder = 4 b_sn.LayoutOrder = 5 b_sh.LayoutOrder = 6 b_ht.LayoutOrder = 7 b_rt.LayoutOrder = 8 b_tc.LayoutOrder = 9 b_ct.LayoutOrder = 10 b_ce.LayoutOrder = 11

		local localplayer = game:GetService"Players".LocalPlayer
		local uis = game:GetService"UserInputService"

		local cheats = {
			b_b = false;
			b_f = false;
			b_f_t = 1;
			b_sd = false;
			b_sn = false;
			b_sh = false;
			b_ht = "Text";
			b_rt = false;
			b_tc = false;
		}

		local cheatsf = Instance.new("Folder", game.CoreGui) cheatsf.Name = "cheats"
		local espf = Instance.new("Folder", cheatsf) espf.Name = "esp"

		function addEsp(player)
			local bbg = Instance.new("BillboardGui", espf)
			bbg.Name = player.Name
			bbg.AlwaysOnTop = true
			bbg.Size = UDim2.new(4,0,5.4,0)
			bbg.ClipsDescendants = false

			local outlines = Instance.new("Frame", bbg)
			outlines.Size = UDim2.new(1,0,1,0)
			outlines.BorderSizePixel = 0
			outlines.BackgroundTransparency = 1
			local left = Instance.new("Frame", outlines)
			left.BorderSizePixel = 0
			left.Size = UDim2.new(0,1,1,0)
			local right = left:Clone()
			right.Parent = outlines
			right.Size = UDim2.new(0,-1,1,0)
			right.Position = UDim2.new(1,0,0,0)
			local up = left:Clone()
			up.Parent = outlines
			up.Size = UDim2.new(1,0,0,1)
			local down = left:Clone()
			down.Parent = outlines
			down.Size = UDim2.new(1,0,0,-1)
			down.Position = UDim2.new(0,0,1,0)

			local info = Instance.new("BillboardGui", bbg)
			info.Name = "info"
			info.Size = UDim2.new(3,0,0,54)
			info.StudsOffset = Vector3.new(3.6,-3,0)
			info.AlwaysOnTop = true
			info.ClipsDescendants = false
			local namelabel = Instance.new("TextLabel", info)
			namelabel.Name = "namelabel"
			namelabel.BackgroundTransparency = 1
			namelabel.TextStrokeTransparency = 0
			namelabel.TextXAlignment = Enum.TextXAlignment.Left
			namelabel.Size = UDim2.new(0,100,0,18)
			namelabel.Position = UDim2.new(0,0,0,0)
			namelabel.Text = player.Name
			local distancel = Instance.new("TextLabel", info)
			distancel.Name = "distancelabel"
			distancel.BackgroundTransparency = 1
			distancel.TextStrokeTransparency = 0
			distancel.TextXAlignment = Enum.TextXAlignment.Left
			distancel.Size = UDim2.new(0,100,0,18)
			distancel.Position = UDim2.new(0,0,0,18)
			local healthl = Instance.new("TextLabel", info)
			healthl.Name = "healthlabel"
			healthl.BackgroundTransparency = 1
			healthl.TextStrokeTransparency = 0
			healthl.TextXAlignment = Enum.TextXAlignment.Left
			healthl.Size = UDim2.new(0,100,0,18)
			healthl.Position = UDim2.new(0,0,0,36)

			local uill = Instance.new("UIListLayout", info)

			local forhealth = Instance.new("BillboardGui", bbg)
			forhealth.Name = "forhealth"
			forhealth.Size = UDim2.new(5,0,6,0)
			forhealth.AlwaysOnTop = true
			forhealth.ClipsDescendants = false

			local healthbar = Instance.new("Frame", forhealth)
			healthbar.Name = "healthbar"
			healthbar.BackgroundColor3 = Color3.fromRGB(40,40,40)
			healthbar.BorderColor3 = Color3.fromRGB(0,0,0)
			healthbar.Size = UDim2.new(0.04,0,0.9,0)
			healthbar.Position = UDim2.new(0,0,0.05,0)
			local bar = Instance.new("Frame", healthbar)
			bar.Name = "bar"
			bar.BorderSizePixel = 0
			bar.BackgroundColor3 = Color3.fromRGB(94,255,69)
			bar.AnchorPoint = Vector2.new(0,1)
			bar.Position = UDim2.new(0,0,1,0)
			bar.Size = UDim2.new(1,0,1,0)

			local co = coroutine.create(function()
				while wait(0.1) do
					if (player.Character and player.Character:FindFirstChild"HumanoidRootPart") then
						bbg.Adornee = player.Character.HumanoidRootPart
						info.Adornee = player.Character.HumanoidRootPart
						forhealth.Adornee = player.Character.HumanoidRootPart

						if (player.Team ~= localplayer.Team) then
							bbg.Enabled = true
							info.Enabled = true
							forhealth.Enabled = true
						end
						if player.Character:FindFirstChild("ForceField") then
							outlines.BackgroundTransparency = 0.4
							left.BackgroundTransparency = 0.4
							right.BackgroundTransparency = 0.4
							up.BackgroundTransparency = 0.4
							down.BackgroundTransparency = 0.4
							healthl.TextTransparency = 0.4
							healthl.TextStrokeTransparency = 0.8
							distancel.TextTransparency = 0.4
							distancel.TextStrokeTransparency = 0.8
							namelabel.TextTransparency = 0.4
							namelabel.TextStrokeTransparency = 0.8
							bar.BackgroundTransparency = 0.4
							healthbar.BackgroundTransparency = 0.8
						else
							outlines.BackgroundTransparency = 0
							left.BackgroundTransparency = 0
							right.BackgroundTransparency = 0
							up.BackgroundTransparency = 0
							down.BackgroundTransparency = 0
							healthl.TextTransparency = 0
							healthl.TextStrokeTransparency = 0
							distancel.TextTransparency = 0
							distancel.TextStrokeTransparency = 0
							namelabel.TextTransparency = 0
							namelabel.TextStrokeTransparency = 0
							bar.BackgroundTransparency = 0
							healthbar.BackgroundTransparency = 0
						end
						if cheats.b_b == true then
							outlines.Visible = true
						else
							outlines.Visible = false
						end
						if cheats.b_f == true then
							if player.Character:FindFirstChild("ForceField") then
								outlines.BackgroundTransparency = 0.9
							else
								outlines.BackgroundTransparency = cheats.b_f_t
							end
						else
							outlines.BackgroundTransparency = 1
						end
						if cheats.b_sh == true then
							if (player.Character:FindFirstChild"Humanoid") then
								healthl.Text = "Health: "..math.floor(player.Character:FindFirstChild"Humanoid".Health)
								healthbar.bar.Size = UDim2.new(1,0,player.Character:FindFirstChild"Humanoid".Health/player.Character:FindFirstChild"Humanoid".MaxHealth,0)
							end
							if cheats.b_ht == "Text" then
								healthbar.Visible = false
								healthl.Visible = true
							end
							if cheats.b_ht == "Bar" then
								healthl.Visible = false
								healthbar.Visible = true
							end
							if cheats.b_ht == "Both" then
								healthl.Visible = true
								healthbar.Visible = true
							end
						else
							healthl.Visible = false
							healthbar.Visible = false
						end
						if cheats.b_sn then
							namelabel.Visible = true
						else
							namelabel.Visible = false
						end
						if cheats.b_sd == true then
							distancel.Visible = true
							if (localplayer.Character and localplayer.Character:FindFirstChild"HumanoidRootPart") then
								distancel.Text = "Distance: "..math.floor(0.5+(localplayer.Character:FindFirstChild"HumanoidRootPart".Position - player.Character:FindFirstChild"HumanoidRootPart".Position).magnitude)
							end
						else
							distancel.Visible = false
						end
						if cheats.b_rt == true then
							if (player.Team == localplayer.Team) then
								bbg.Enabled = true
								info.Enabled = true
								forhealth.Enabled = true
							end
						else
							if (player.Team == localplayer.Team) then
								bbg.Enabled = false
								info.Enabled = false
								forhealth.Enabled = false
							end
						end
						if cheats.b_tc == true then
							outlines.BackgroundColor3 = player.TeamColor.Color
							left.BackgroundColor3 = player.TeamColor.Color
							right.BackgroundColor3 = player.TeamColor.Color
							up.BackgroundColor3 = player.TeamColor.Color
							down.BackgroundColor3 = player.TeamColor.Color
							healthl.TextColor3 = player.TeamColor.Color
							distancel.TextColor3 = player.TeamColor.Color
							namelabel.TextColor3 = player.TeamColor.Color
						else
							if (player.Team == localplayer.Team) then
								outlines.BackgroundColor3 = Color3.fromRGB(ct_r.Text, ct_g.Text, ct_b.Text)
								left.BackgroundColor3 = Color3.fromRGB(ct_r.Text, ct_g.Text, ct_b.Text)
								right.BackgroundColor3 = Color3.fromRGB(ct_r.Text, ct_g.Text, ct_b.Text)
								up.BackgroundColor3 = Color3.fromRGB(ct_r.Text, ct_g.Text, ct_b.Text)
								down.BackgroundColor3 = Color3.fromRGB(ct_r.Text, ct_g.Text, ct_b.Text)
								healthl.TextColor3 = Color3.fromRGB(ct_r.Text, ct_g.Text, ct_b.Text)
								distancel.TextColor3 = Color3.fromRGB(ct_r.Text, ct_g.Text, ct_b.Text)
								namelabel.TextColor3 = Color3.fromRGB(ct_r.Text, ct_g.Text, ct_b.Text)
							else
								outlines.BackgroundColor3 = Color3.fromRGB(ce_r.Text, ce_g.Text, ce_b.Text)
								left.BackgroundColor3 = Color3.fromRGB(ce_r.Text, ce_g.Text, ce_b.Text)
								right.BackgroundColor3 = Color3.fromRGB(ce_r.Text, ce_g.Text, ce_b.Text)
								up.BackgroundColor3 = Color3.fromRGB(ce_r.Text, ce_g.Text, ce_b.Text)
								down.BackgroundColor3 = Color3.fromRGB(ce_r.Text, ce_g.Text, ce_b.Text)
								healthl.TextColor3 = Color3.fromRGB(ce_r.Text, ce_g.Text, ce_b.Text)
								distancel.TextColor3 = Color3.fromRGB(ce_r.Text, ce_g.Text, ce_b.Text)
								namelabel.TextColor3 = Color3.fromRGB(ce_r.Text, ce_g.Text, ce_b.Text)
							end
						end
					end
					if not (game:GetService"Players":FindFirstChild(player.Name)) then
						print(player.Name.." has left. Clearing esp.")
						espf:FindFirstChild(player.Name):Destroy()
						coroutine.yield()
					end
				end
			end)
			coroutine.resume(co)
		end

		--main
		do
			wait(2)
			--menu buttons
			for _,button in pairs(age1:GetDescendants()) do
				if button:IsA"TextButton" then
					button.MouseButton1Click:connect(function()
						if button.Name == "b_f_t" then
							if cheats.b_f_t >= 0 then
								cheats.b_f_t = cheats.b_f_t+0.1
								if cheats.b_f_t > 1 then
									cheats.b_f_t = 0
								end
							end
							button.v.Text = cheats.b_f_t
						elseif button.Name == "b_ht" then
							if cheats.b_ht == "Text" then
								cheats.b_ht = "Bar"
							elseif cheats.b_ht == "Bar" then
								cheats.b_ht = "Both"
							else
								cheats.b_ht = "Text"
							end
							button.v.Text = cheats.b_ht
						else
							if cheats[button.Name] == true then
								cheats[button.Name] = false
								button.v.Text = "OFF"
								button.v.TextColor3 = Color3.fromRGB(255,0,0)
							else
								cheats[button.Name] = true
								button.v.Text = "ON"
								button.v.TextColor3 = Color3.fromRGB(0,255,0)
							end
						end 
					end)
				end
			end

			--initial player addition
			for _,v in pairs(game:GetService("Players"):GetChildren()) do
				if not (v.Name == localplayer.Name) then
					if not (espf:FindFirstChild(v.Name)) then
						addEsp(v)
					end
				end
			end

			--open/close gui
			game:GetService("UserInputService").InputBegan:connect(function(input, gameProcessed)
				if input.KeyCode == Enum.KeyCode.KeypadOne then
					if not gameProcessed then
						age1.Enabled = not age1.Enabled
					end
				end
			end)

			--auto-update
			while wait(10) do
				for _,v in pairs(game:GetService("Players"):GetChildren()) do
					if not (v.Name == localplayer.Name) then
						if not (espf:FindFirstChild(v.Name)) then
							addEsp(v)
						end
					end
				end
			end
		end
	end              
})
local Section = PlayersTab:AddSection({
	Name = "Player"
})
PlayersTab:AddButton({
	Name = "Voar - Bypass",
	Callback = function()
		loadstring("\108\111\97\100\115\116\114\105\110\103\40\103\97\109\101\58\72\116\116\112\71\101\116\40\40\39\104\116\116\112\115\58\47\47\103\105\115\116\46\103\105\116\104\117\98\117\115\101\114\99\111\110\116\101\110\116\46\99\111\109\47\109\101\111\122\111\110\101\89\84\47\98\102\48\51\55\100\102\102\57\102\48\97\55\48\48\49\55\51\48\52\100\100\100\54\55\102\100\99\100\51\55\48\47\114\97\119\47\101\49\52\101\55\52\102\52\50\53\98\48\54\48\100\102\53\50\51\51\52\51\99\102\51\48\98\55\56\55\48\55\52\101\98\51\99\53\100\50\47\97\114\99\101\117\115\37\50\53\50\48\120\37\50\53\50\48\102\108\121\37\50\53\50\48\50\37\50\53\50\48\111\98\102\108\117\99\97\116\111\114\39\41\44\116\114\117\101\41\41\40\41\10\10")()
	end   
})
PlayersTab:AddButton({
	Name = "Atravessar Parade",
	Callback = function()
		-- Farewell Infortality.
		-- Version: 2.82
		-- Instances:
		local ScreenGui = Instance.new("ScreenGui")
		local Frame = Instance.new("Frame")
		local Drag = Instance.new("TextButton")
		local TextButton = Instance.new("TextButton")
		local TextButton_2 = Instance.new("TextButton")
		local TextLabel = Instance.new("TextLabel")
		--Properties:
		ScreenGui.Parent = game.Players.LocalPlayer:WaitForChild("PlayerGui")
		ScreenGui.ZIndexBehavior = Enum.ZIndexBehavior.Sibling

		Frame.Parent = ScreenGui
		Frame.BackgroundColor3 = Color3.new(1, 1, 1)
		Frame.Position = UDim2.new(0.275453836, 0, 0.186732173, 0)
		Frame.Size = UDim2.new(0, 379, 0, 373)

		Drag.Name = "Menu V2 Noclip"
		Drag.Parent = Frame
		Drag.BackgroundColor3 = Color3.new(1, 1, 1)
		Drag.BorderColor3 = Color3.new(0.917647, 0.917647, 0.917647)
		Drag.Size = UDim2.new(0, 379, 0, 27)
		Drag.Text = "Menu V2 Noclip"
		Drag.TextColor3 = Color3.new(0, 0, 0)

		TextButton.Parent = Frame
		TextButton.BackgroundColor3 = Color3.new(1, 1, 1)
		TextButton.Position = UDim2.new(0.261265785, 0, 0.352023244, 0)
		TextButton.Size = UDim2.new(0, 200, 0, 50)
		TextButton.Font = Enum.Font.SourceSans
		TextButton.Text = "Noclip R15"
		TextButton.TextColor3 = Color3.new(0, 0, 0)
		TextButton.TextSize = 14
		TextButton.MouseButton1Down:connect(function()
			nam = game.Players.LocalPlayer.Name

			game:GetService('RunService').Stepped:connect(function()
				for a, b in pairs(game.Workspace:GetChildren()) do
					if b.Name == nam then
						for i, v in pairs(game.Workspace[nam]:GetChildren()) do
							if v:IsA("BasePart") then
								v.CanCollide = false

							end
						end
					end
				end
			end)

			Workspace[nam].Head.Changed:connect(function()
				for a, b in pairs(game.Workspace:GetChildren()) do
					if b.Name == nam then
						for i, v in pairs(game.Workspace[nam]:GetChildren()) do
							if v:IsA("BasePart") then
								v.CanCollide = false

							end
						end
					end
				end
			end)
		end)

		TextButton_2.Parent = Frame
		TextButton_2.BackgroundColor3 = Color3.new(1, 1, 1)
		TextButton_2.Position = UDim2.new(0.261265785, 0, 0.615844727, 0)
		TextButton_2.Size = UDim2.new(0, 200, 0, 50)
		TextButton_2.Font = Enum.Font.SourceSans
		TextButton_2.Text = "Noclip R6"
		TextButton_2.TextColor3 = Color3.new(0, 0, 0)
		TextButton_2.TextSize = 14
		TextButton_2.MouseButton1Down:connect(function()
			game.Players.LocalPlayer.Character.Humanoid.MaxHealth = math.huge
			game.Players.LocalPlayer.Character.Humanoid.Health = math.huge
			while true do
				game:GetService("RunService").Stepped:wait()
				game.Players.LocalPlayer.Character.Head.CanCollide = false
				game.Players.LocalPlayer.Character.Torso.CanCollide = false
			end
		end)

		TextLabel.Parent = Frame
		TextLabel.BackgroundColor3 = Color3.new(1, 1, 1)
		TextLabel.Position = UDim2.new(0.104106054, 0, 0.111652002, 0)
		TextLabel.Size = UDim2.new(0, 299, 0, 50)
		TextLabel.Font = Enum.Font.SourceSans
		TextLabel.Text = "Noclip By Menu V2"
		TextLabel.TextColor3 = Color3.new(0, 0, 0)
		TextLabel.TextSize = 14
		TextLabel.TextWrapped = true
		-- Scripts:
		function SCRIPT_GBXM85_FAKESCRIPT() -- Drag.LocalScript 
			local script = Instance.new('LocalScript')
			script.Parent = Drag
			wanttobemoved=script.Parent.Parent
			X=wanttobemoved.Position.X.Offset
			Y=wanttobemoved.Position.Y.Offset
			XS=wanttobemoved.Position.X.Scale
			YS=wanttobemoved.Position.Y.Scale
			function down(posX,posY)--the positions of the mouse
				drag=true--activate the drag function
				X=wanttobemoved.Position.X.Offset--redefines the value "X"
				Y=wanttobemoved.Position.Y.Offset--redefines the value "Y"
				XS=wanttobemoved.Position.X.Scale
				YS=wanttobemoved.Position.Y.Scale
				DposX=posX-X--the mouse's X position offset by the frame's X position.
				DposY=posY-Y--the mouse's Y position offset by the frame's Y position.
				print(""..DposX..","..DposY.."")--remembers the values DposX and DposY in the output toolbar.
			end
			function up()
				drag=false--deactivate the drag
			end
			function move(posX,posY)--again, the positions of the mouse
				if drag then--if held down then
					wanttobemoved.Position=UDim2.new(XS,posX - DposX,YS,posY - DposY)
				end
			end
			script.Parent.MouseButton1Down:connect(down)
			script.Parent.MouseButton1Up:connect(up)
			script.Parent.MouseLeave:connect(up)
			script.Parent.MouseMoved:connect(move)

		end
		coroutine.resume(coroutine.create(SCRIPT_GBXM85_FAKESCRIPT))

	end   
})
PlayersTab:AddButton({
	Name = "Kill all - Regime militar de 83",
	Callback = function()
		loadstring(game:HttpGet(('https://raw.githubusercontent.com/Pedroxz63/killall/main/README.md'),true))()
	end   
})
PlayersTab:AddButton({
	Name = "Kill Aura - Risco Crash",
	Callback = function()
		loadstring(game:HttpGetAsync("https://pastebin.com/raw/PpALBidP"))()
	end   
})
PlayersTab:AddButton({
	Name = "Teleport Player",
	Callback = function()
		----------------------
		-- SHARK X HUB NO 1 --
		----------------------

		local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/xHeptc/Kavo-UI-Library/main/source.lua"))()
		local Window = Library.CreateLib("Pedroxz Teleport", "DarkTheme")
		local Tab = Window:NewTab("Players")
		local Section = Tab:NewSection("Teleport")

		--------------------

		players = {}

		for i,v in pairs(game:GetService("Players"):GetChildren()) do
			table.insert(players,v.Name)
		end

		Section:NewDropdown("Select Player", " ", players, function(abc)
			Select = abc
		end)


		Section:NewButton("Refresh", " ", function()
			table.clear(players)
			for i,v in pairs(game:GetService("Players"):GetChildren()) do
				table.insert(players,v.Name)
			end
		end)

		Section:NewButton("Teleport", " ", function()
			game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = game.Players[Select].Character.HumanoidRootPart.CFrame
		end)
	end   
})  
local Section = PlayersTab:AddSection({
	Name = "Cheat"
})
PlayersTab:AddButton({
	Name = "Esconder Nome",
	Callback = function()
		wait()

		game.StarterGui:SetCoreGuiEnabled(Enum.CoreGuiType.PlayerList, false)
	end    
})
PlayersTab:AddButton({
	Name = "+18 Troll",
	Callback = function()
		local Victim='Pedroxz'
		local A=Instance.new'Animation'
		A.AnimationId='rbxassetid://148840371'
		local P=game:GetService'Players'.LocalPlayer
		local C=P.Character or P.CharacterAdded:Wait()
		local H=C:WaitForChild'Humanoid':LoadAnimation(A)
		H:Play()
		H:AdjustSpeed(2.5)
		game:GetService'RunService'.Stepped:Connect(function()
			C:WaitForChild'HumanoidRootPart'.CFrame=CFrame.new(game:GetService'Players':FindFirstChild(Victim).Character:WaitForChild'HumanoidRootPart'.Position)
		end)
	end    
})
PlayersTab:AddButton({
	Name = "Staffs Proximo",
	Callback = function()
		print("button pressed")
	end    
})
local Section = PlayersTab:AddSection({
	Name = "Metodos"
})    
PlayersTab:AddButton({
	Name = "Puxar Dinheiro 1 (Metodo) - Notify (Quase todos os jogos)",
	Callback = function()
		game.StarterGui:SetCore("SendNotification", {
			Title = "Metodo puxar dinheiro 1"; 
			Text = "1) vai na aba jogador, e dps Dex 2) dps de carregar va em players, procure por seu nome, clique e vai ate aba dinheiro, e dps "; 
			Icon = ""; 
			Duration = 20;
			Callback = bindableFunction;
			Button1 = "";  
			Button2 = "";
		})
	end 
})
PlayersTab:AddButton({
	Name = "Puxar Dinheiro 2 (Metodo) - Notify (Quase todos os jogos)",
	Callback = function()
		game.StarterGui:SetCore("SendNotification", {
			Title = "Metodo puxar dinheiro 2"; 
			Text = "em baixo coloca o value o tanto dinheiro quiser"; 
			Icon = ""; 
			Duration = 20;
			Callback = bindableFunction;
			Button1 = "";  
			Button2 = "";
		})
	end        
})
PlayersTab:AddButton({
	Name = "Puxar Dinheiro 3 (Click)",
	Callback = function()
		local Player = game.Players.LocalPlayer
		local Dinheiro = Player.leaderstats.Dinheiro

		Dinheiro.Value = 99999999
	end    
})
MenusTab:AddButton({
	Name = "Infinite yield",
	Callback = function()
		loadstring(game:HttpGet('https://raw.githubusercontent.com/EdgeIY/infiniteyield/master/source'))()
	end         
})
MenusTab:AddButton({
	Name = "Pedroxz Menu V1",
	Callback = function()
		loadstring(game:HttpGet('https://raw.githubusercontent.com/Pedroxz63/PedroMenu/main/README.md'))()
	end       
})
MenusTab:AddButton({
	Name = "Kakah Menu Key: 2182396C970TKL3",
	Callback = function()
		loadstring(game:HttpGet('https://raw.githubusercontent.com/Pedroxz63/KakahMenuBypedroxz631/main/README.md'))()
	end     
})
AdmTab:AddButton({
	Name = "Virar ADM",
	Callback = function()
		loadstring(game:HttpGetAsync("https://pastebin.com/raw/Caniwq2N"))()
	end       
})
AdmTab:AddButton({
	Name = "logs ADM",
	Callback = function()
		loadstring(game:HttpGet("https://pastebin.com/raw/stggPUBM", true))()
	end       
})
local Section = BypassTab:AddSection({
	Name = "Painel Anti detecter"
})
BypassTab:AddButton({
	Name = "Stopar Anti cheater V1 - Risco Kick",
	Callback = function()
		loadstring(game:HttpGet(('https://raw.githubusercontent.com/Pedroxz63/Ante-kick-V1/main/README.md'),true))()
	end                        
})
BypassTab:AddButton({
	Name = "Stopar Anti cheater V2",
	Callback = function()
		ait(0.5)local ba=Instance.new("ScreenGui")
		local ca=Instance.new("TextLabel")local da=Instance.new("Frame")
		local _b=Instance.new("TextLabel")local ab=Instance.new("TextLabel")ba.Parent=game.CoreGui
		ba.ZIndexBehavior=Enum.ZIndexBehavior.Sibling;ca.Parent=ba;ca.Active=true
		ca.BackgroundColor3=Color3.new(0.176471,0.176471,0.176471)ca.Draggable=true
		ca.Position=UDim2.new(0.698610067,0,0.098096624,0)ca.Size=UDim2.new(0,304,0,52)
		ca.Font=Enum.Font.SourceSansSemibold;ca.Text="Anti Afk Kick Script"ca.TextColor3=Color3.new(0,1,1)
		ca.TextSize=22;da.Parent=ca
		da.BackgroundColor3=Color3.new(0.196078,0.196078,0.196078)da.Position=UDim2.new(0,0,1.0192306,0)
		da.Size=UDim2.new(0,304,0,107)_b.Parent=da
		_b.BackgroundColor3=Color3.new(0.176471,0.176471,0.176471)_b.Position=UDim2.new(0,0,0.800455689,0)
		_b.Size=UDim2.new(0,304,0,21)_b.Font=Enum.Font.Arial;_b.Text="Made by Warn"
		_b.TextColor3=Color3.new(1,1,1)_b.TextSize=20;ab.Parent=da
		ab.BackgroundColor3=Color3.new(0.176471,0.176471,0.176471)ab.Position=UDim2.new(0,0,0.158377379,0)
		ab.Size=UDim2.new(0,304,0,44)ab.Font=Enum.Font.ArialBold;ab.Text="Status: Script Started"
		ab.TextColor3=Color3.new(1,1,1)ab.TextSize=20;local bb=game:service'VirtualUser'
		game:service'Players'.LocalPlayer.Idled:connect(function()
			bb:CaptureController()bb:ClickButton2(Vector2.new())
			ab.Text="You went idle and ROBLOX tried to kick you but we reflected it!"wait(2)ab.Text="Script Re-Enabled"end)
	end    
})
local Section = JogadorTab:AddSection({
	Name = "Aimbot"
})     
BypassTab:AddButton({
	Name = "Desativar anti cheater/exploit V3",
	Callback = function()
		assert(getrawmetatable)
		grm = getrawmetatable(game)
		setreadonly(grm, false)
		old = grm.__namecall
		grm.__namecall = newcclosure(function(self, ...)
			local args = {...}
			if tostring(args[1]) == "TeleportDetect" then
				return
			elseif tostring(args[1]) == "CHECKER_1" then
				return
			elseif tostring(args[1]) == "CHECKER" then
				return
			elseif tostring(args[1]) == "GUI_CHECK" then
				return
			elseif tostring(args[1]) == "OneMoreTime" then
				return
			elseif tostring(args[1]) == "checkingSPEED" then
				return
			elseif tostring(args[1]) == "BANREMOTE" then
				return
			elseif tostring(args[1]) == "PERMAIDBAN" then
				return
			elseif tostring(args[1]) == "KICKREMOTE" then
				return
			elseif tostring(args[1]) == "BR_KICKPC" then
				return
			elseif tostring(args[1]) == "BR_KICKMOBILE" then
				return
			end
			return old(self, ...)
		end)
	end    
}) 
BypassTab:AddButton({
	Name = "Anti kick V9",
	Callback = function()
		wait(0.5)local ba=Instance.new("ScreenGui")
		local ca=Instance.new("TextLabel")local da=Instance.new("Frame")
		local _b=Instance.new("TextLabel")local ab=Instance.new("TextLabel")ba.Parent=game.CoreGui
		ba.ZIndexBehavior=Enum.ZIndexBehavior.Sibling;ca.Parent=ba;ca.Active=true
		ca.BackgroundColor3=Color3.new(0.176471,0.176471,0.176471)ca.Draggable=true
		ca.Position=UDim2.new(0.698610067,0,0.098096624,0)ca.Size=UDim2.new(0,370,0,52)
		ca.Font=Enum.Font.SourceSansSemibold;ca.Text="Anti Kick V9"ca.TextColor3=Color3.new(0,1,1)
		ca.TextSize=22;da.Parent=ca
		da.BackgroundColor3=Color3.new(0.196078,0.196078,0.196078)da.Position=UDim2.new(0,0,1.0192306,0)
		da.Size=UDim2.new(0,370,0,107)_b.Parent=da
		_b.BackgroundColor3=Color3.new(0.176471,0.176471,0.176471)_b.Position=UDim2.new(0,0,0.800455689,0)
		_b.Size=UDim2.new(0,370,0,21)_b.Font=Enum.Font.Arial;_b.Text="Feito por Larissa da Phx "
		_b.TextColor3=Color3.new(0,1,1)_b.TextSize=20;ab.Parent=da
		ab.BackgroundColor3=Color3.new(0.176471,0.176471,0.176471)ab.Position=UDim2.new(0,0,0.158377,0)
		ab.Size=UDim2.new(0,370,0,44)ab.Font=Enum.Font.ArialBold;ab.Text="Status: Active"
		ab.TextColor3=Color3.new(0,1,1)ab.TextSize=20;local bb=game:service'VirtualUser'
		game:service'Players'.LocalPlayer.Idled:connect(function()
			bb:CaptureController()bb:ClickButton2(Vector2.new())
			ab.Text="Roblox tried to kick u but i kicked him instead"wait(2)ab.Text="Status : Active"end)
	end    
})
JogadorTab:AddToggle({
	Name = "Aimbot + Esp Hub",
	Default = false,
	Callback = function(Value)
		_G.Aimbot = Value
		Aimbot()
	end    
})    
