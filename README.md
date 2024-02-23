local players = game:GetService("Players")
game:GetService("StarterGui"):SetCore("SendNotification", {
    Title = "Bot";
    Text = "Made By WHY" .. players.LocalPlayer.DisplayName;
    Icon = "rbxthumb://type=AvatarHeadShot&id=" .. players.LocalPlayer.UserId .. "&w=180&h=180 true";
    Duration = 5
})

local gui = Instance.new("ScreenGui")
gui.Name = "WHY Of Gui"
gui.Parent = game.CoreGui

local Frame = Instance.new("Frame")
Frame.Size = UDim2.new(0.5, 0, 0.7, 0)
Frame.Position = UDim2.new(0.5, 0, 0.5, 0)
Frame.BackgroundColor3 = Color3.fromRGB(0, 0, 0)
Frame.BorderColor3 = Color3.new(0, 0, 0)
Frame.BorderSizePixel = 1
Frame.Active = true
Frame.Draggable = true
Frame.Parent = gui

local UICorner = Instance.new("UICorner")
UICorner.CornerRadius = UDim.new(0, 5)
UICorner.Parent = Frame

local Bar = Instance.new("TextButton")
Bar.Size = UDim2.new(0.3, 0, 0.2, 0)
Bar.Position = UDim2.new(0.09, 0, 0.4, 0)
Bar.BackgroundColor3 = Color3.fromRGB(255, 247, 0)
Bar.BorderColor3 = Color3.new(0, 0, 0)
Bar.BorderSizePixel = 1
Bar.Text = "AutoFarm(JustPress2Time)"
Bar.TextColor3 = Color3.new(255, 255, 255)
Bar.Font = Enum.Font.Code
Bar.Parent = Frame
Bar.TextSize = 14.00

Bar.MouseButton1Click:Connect(function()
    while true do
        wait()
        workspace:WaitForChild("BladePowerGiver"):WaitForChild("RemoteEvent"):FireServer()
    end
end)

local UICorner_2 = Instance.new("UICorner")
UICorner_2.CornerRadius = UDim.new(0, 5)
UICorner_2.Parent = Frame

local Bar_2 = Instance.new("TextButton")
Bar_2.Size = UDim2.new(0.3, 0, 0.2, 0)
Bar_2.Position = UDim2.new(0.6, 0, 0.4, 0)
Bar_2.BackgroundColor3 = Color3.fromRGB(255, 247, 0)
Bar_2.BorderColor3 = Color3.new(0, 0, 0)
Bar_2.BorderSizePixel = 1
Bar_2.Text = "Hide"
Bar_2.TextColor3 = Color3.new(255, 255, 255)
Bar_2.Font = Enum.Font.Code
Bar_2.Parent = Frame
Bar_2.TextSize = 14.00

Bar_2.MouseButton1Click:Connect(function()
    game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(91, -66, -146)
end)

local UICorner_3 = Instance.new("UICorner")
UICorner_3.CornerRadius = UDim.new(0, 5)
UICorner_3.Parent = Frame

local Bar_3 = Instance.new("TextButton")
Bar_3.Size = UDim2.new(0.3, 0, 0.2, 0)
Bar_3.Position = UDim2.new(0.3, 0, 0.7, 0)
Bar_3.BackgroundColor3 = Color3.fromRGB(255, 247, 0)
Bar_3.BorderColor3 = Color3.new(0, 0, 0)
Bar_3.BorderSizePixel = 1
Bar_3.Text = "AntiAfk"
Bar_3.TextColor3 = Color3.new(255, 255, 255)
Bar_3.Font = Enum.Font.Code
Bar_3.Parent = Frame
Bar_3.TextSize = 14.00

Bar_3.MouseButton1Click:Connect(function()
    loadstring(game:HttpGet("https://raw.githubusercontent.com/evxncodes/mainroblox/main/anti-afk", true))()
end)

local TextLabel = Instance.new("TextLabel")
TextLabel.Size = UDim2.new(0.9, 35, 0.2, 0)
TextLabel.Position = UDim2.new(-0.0, 0, 0.5, -95)
TextLabel.BackgroundColor3 = Color3.fromRGB(255, 0, 0)
TextLabel.BorderColor3 = Color3.new(0, 0, 0)
TextLabel.BorderSizePixel = 1
TextLabel.Text = "Blades World Script"
TextLabel.TextColor3 = Color3.new(255, 255, 255)
TextLabel.Font = Enum.Font.Code
TextLabel.Parent = Frame
TextLabel.TextSize = 20.00
