-- Gui to Lua
-- Version: 3.2

-- Instances:

local ScreenGui = Instance.new("ScreenGui")
local Frame = Instance.new("Frame")
local name = Instance.new("TextLabel")
local UICorner = Instance.new("UICorner")
local rejoin = Instance.new("TextButton")
local UICorner_2 = Instance.new("UICorner")
local infiniteyield = Instance.new("TextButton")
local UICorner_3 = Instance.new("UICorner")
local credits = Instance.new("TextLabel")
local crash = Instance.new("TextButton")
local UICorner_4 = Instance.new("UICorner")
local close = Instance.new("TextButton")
local TextLabel = Instance.new("TextLabel")
local UICorner_5 = Instance.new("UICorner")

--Properties:

ScreenGui.Parent = game.Players.LocalPlayer:WaitForChild("PlayerGui")

Frame.Parent = ScreenGui
Frame.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
Frame.BorderColor3 = Color3.fromRGB(0, 0, 0)
Frame.Position = UDim2.new(0.407382488, 0, 0.0880503133, 0)
Frame.Size = UDim2.new(0, 300, 0, 185)
Frame.Style = Enum.FrameStyle.RobloxRound

name.Name = "name"
name.Parent = Frame
name.BackgroundColor3 = Color3.fromRGB(193, 1, 68)
name.BorderColor3 = Color3.fromRGB(6, 0, 2)
name.Position = UDim2.new(-0.0299999993, 0, -0.0549999997, 0)
name.Size = UDim2.new(0, 302, 0, 35)
name.Font = Enum.Font.Unknown
name.Text = " Doge Hub "
name.TextColor3 = Color3.fromRGB(0, 0, 0)
name.TextSize = 22.000

UICorner.CornerRadius = UDim.new(0, 5)
UICorner.Parent = name

rejoin.Name = "rejoin"
rejoin.Parent = Frame
rejoin.BackgroundColor3 = Color3.fromRGB(193, 1, 68)
rejoin.BorderColor3 = Color3.fromRGB(240, 2, 53)
rejoin.Position = UDim2.new(0.0599999987, 0, 0.204999998, 0)
rejoin.Size = UDim2.new(0, 250, 0, 25)
rejoin.SizeConstraint = Enum.SizeConstraint.RelativeYY
rejoin.Selected = true
rejoin.Font = Enum.Font.ArialBold
rejoin.Text = "Re Join"
rejoin.TextColor3 = Color3.fromRGB(0, 0, 0)
rejoin.TextSize = 15.000
rejoin.MouseButton1Down:connect(function()
	local ts = game:GetService("TeleportService")

local p = game:GetService("Players").LocalPlayer

 

ts:Teleport(game.PlaceId, p)
end)

UICorner_2.CornerRadius = UDim.new(0, 10)
UICorner_2.Parent = rejoin

infiniteyield.Name = "infiniteyield"
infiniteyield.Parent = Frame
infiniteyield.BackgroundColor3 = Color3.fromRGB(193, 1, 68)
infiniteyield.BorderColor3 = Color3.fromRGB(240, 2, 53)
infiniteyield.Position = UDim2.new(0.0599999987, 0, 0.360000014, 0)
infiniteyield.Size = UDim2.new(0, 250, 0, 25)
infiniteyield.SizeConstraint = Enum.SizeConstraint.RelativeYY
infiniteyield.Font = Enum.Font.ArialBold
infiniteyield.Text = "Infinite Yield"
infiniteyield.TextColor3 = Color3.fromRGB(0, 0, 0)
infiniteyield.TextSize = 15.000
infiniteyield.MouseButton1Down:connect(function()
	loadstring(game:HttpGet('https://raw.githubusercontent.com/EdgeIY/infiniteyield/master/source'))()
end)

UICorner_3.CornerRadius = UDim.new(0, 10)
UICorner_3.Parent = infiniteyield

credits.Name = "credits"
credits.Parent = Frame
credits.BackgroundColor3 = Color3.fromRGB(32, 37, 41)
credits.BorderColor3 = Color3.fromRGB(65, 65, 65)
credits.Position = UDim2.new(0, -8, 0.560000002, 0)
credits.Size = UDim2.new(0, 300, 0, 30)
credits.Font = Enum.Font.Ubuntu
credits.Text = "Created By GRP#0615 | Helped By Lay#7616                                          https://dsc.gg/grphub"
credits.TextColor3 = Color3.fromRGB(255, 255, 255)
credits.TextSize = 13.000
credits.TextWrapped = true

crash.Name = "crash"
crash.Parent = Frame
crash.BackgroundColor3 = Color3.fromRGB(193, 1, 68)
crash.BorderColor3 = Color3.fromRGB(240, 2, 53)
crash.Position = UDim2.new(0.0599999987, 0, 0.779999971, 0)
crash.Size = UDim2.new(0, 250, 0, 35)
crash.SizeConstraint = Enum.SizeConstraint.RelativeYY
crash.Font = Enum.Font.ArialBold
crash.Text = "Crash Trade Box"
crash.TextColor3 = Color3.fromRGB(0, 0, 0)
crash.TextSize = 15.000
crash.MouseButton1Down:connect(function()
		local createRemote = workspace:WaitForChild("__THINGS"):WaitForChild("__REMOTES"):WaitForChild("MAIN")
local remoteTypes = {"a","b","c","e"}
for i = 1, 3, 1 do
    createRemote:FireServer(remoteTypes[math.random(#remoteTypes)],tostring(tick()):rep(100))
end
end)

UICorner_4.CornerRadius = UDim.new(0, 10)
UICorner_4.Parent = crash

close.Name = "close"
close.Parent = Frame
close.BackgroundColor3 = Color3.fromRGB(193, 1, 68)
close.Position = UDim2.new(0, 265, 0, -2)
close.Size = UDim2.new(0, 22, 0, 22)
close.Font = Enum.Font.Unknown
close.Text = "X"
close.TextColor3 = Color3.fromRGB(32, 37, 41)
close.TextSize = 20.000

TextLabel.Parent = ScreenGui
TextLabel.BackgroundColor3 = Color3.fromRGB(193, 1, 68)
TextLabel.Position = UDim2.new(0.75, 0, 0.930000007, 0)
TextLabel.Size = UDim2.new(0, 170, 0, 30)
TextLabel.Font = Enum.Font.Unknown
TextLabel.Text = "Press E To Open GUI"
TextLabel.TextColor3 = Color3.fromRGB(0, 0, 0)
TextLabel.TextSize = 17.000
TextLabel.TextStrokeColor3 = Color3.fromRGB(193, 1, 68)

UICorner_5.CornerRadius = UDim.new(0, 30)
UICorner_5.Parent = TextLabel

-- Scripts:

local function GUNEZPR_fake_script() -- close.LocalScript 
	local script = Instance.new('LocalScript', close)

	local Frame = script.Parent.Parent
	
	script.Parent.MouseButton1Click:Connect(function()
		Frame.Visible = false
	end)
end
coroutine.wrap(GUNEZPR_fake_script)()
local function NLYMZX_fake_script() -- Frame.LocalScript 
	local script = Instance.new('LocalScript', Frame)

	
	script.Parent.Visible = false
	local UIS = game:GetService('UserInputService')
	
	local allowed = {
	
		'GRP_OFFICIAL', --Place username in the: ''
		'Thas_Jayy',
		'ikindalovetycoon'
	
	
	
	}
	
	local function isAllowed(player)
		for i,v in pairs(allowed) do
			if v == player.Name then
	
				if 	script.Parent.Visible == true then
	
					script.Parent.Visible = false 
				elseif 	script.Parent.Visible == false then
	
					script.Parent.Visible = true 
				end
	
			end
		end
		--script.Parent.Enabled = false
	end
	
	
	
	local function onInputBegan(input)
		if input.KeyCode == Enum.KeyCode.E then
	
			isAllowed(game.Players.LocalPlayer)
	
		end
	end
	
	UIS.InputBegan:Connect(onInputBegan)
end
coroutine.wrap(NLYMZX_fake_script)()
local function FLDI_fake_script() -- ScreenGui.Script 
	local script = Instance.new('Script', ScreenGui)

	frame = script.Parent.Frame
	frame.Draggable = true
	frame.Active = true
	frame.Selectable = true
end
coroutine.wrap(FLDI_fake_script)()
