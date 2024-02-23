local players = game:GetService("Players")
game:GetService("StarterGui"):SetCore("SendNotification", {
    Title = "Bot";
    Text = "Made By gagghigggg" .. players.LocalPlayer.DisplayName;
    Icon = "rbxthumb://type=AvatarHeadShot&id=" .. players.LocalPlayer.UserId .. "&w=180&h=180 true";
    Duration = 5
})

local gui = Instance.new("ScreenGui")
gui.Name = "WHY Of Gui"
gui.Parent = game.CoreGui

--screengui = gui


-- gui = ScreenGui
local Frame = Instance.new("Frame")
Frame.Size = UDim2.new(0.5, 0, 0.7, 0)
Frame.Position = UDim2.new(0.5, 0, 0.5, 0)
Frame.BackgroundColor3 = Color3.new(0,0,0)
Frame.BorderColor3 = Color3.new(0, 0, 0)
Frame.BorderSizePixel = 1
Frame.Active = true
Frame.Draggable = true
Frame.Parent = gui

local UICorner = Instance.new("UICorner")
UICorner.CornerRadius = UDim.new(0, 5)
UICorner.Parent = Frame


local TextButton = Instance.new("TextButton")
TextButton.Size = UDim2.new(0.3, 0, 0.2, 0)
TextButton.Position = UDim2.new(0.09, 0, 0.4, 0)
TextButton.BackgroundColor3 = Color3.new(0,0,0)
TextButton.BorderColor3 = Color3.new(0, 0, 0)
TextButton.BorderSizePixel = 1
TextButton.Text = "AutoFarm(JustPress2Time)"
TextButton.TextColor3 = Color3.new(255, 255, 255)
TextButton.Font = Enum.Font.Code
TextButton.Parent = Frame
TextButton.TextSize = 14.00


TextButton.MouseButton1Click:Connect(function()
     while true do wait()
workspace:WaitForChild("BladePowerGiver"):WaitForChild("RemoteEvent"):FireServer()

end
end)

local UICorner_2 = Instance.new("UICorner")
UICorner_2.CornerRadius = UDim.new(0, 5)
UICorner_2.Parent = Frame


local TextButton_2 = Instance.new("TextButton")
TextButton_2.Size = UDim2.new(0.3, 0, 0.2, 0)
TextButton_2.Position = UDim2.new(0.6, 0, 0.4, 0)
TextButton_2.BackgroundColor3 = Color3.new(0,0,0)
TextButton_2.BorderColor3 = Color3.new(0, 0, 0)
TextButton_2.BorderSizePixel = 1
TextButton_2.Text = "Hide"
TextButton_2.TextColor3 = Color3.new(255,255,255)
TextButton_2.Font = Enum.Font.Code
TextButton_2.Parent = Frame
TextButton_2.TextSize = 14.00

TextButton_2.MouseButton1Click:Connect(function()
game.Players.LocalPlayer.Character.HumanoidRootPart.CFrame = CFrame.new(-35, -39, -178)


end)



local UICorner_3 = Instance.new("UICorner")
UICorner_3.CornerRadius = UDim.new(0, 5)
UICorner_3.Parent = Frame


local TextButton_3 = Instance.new("TextButton")
TextButton_3.Size = UDim2.new(0.4, 0, 0.2, 0)
TextButton_3.Position = UDim2.new(0.3, 0, 0.7,  0)
TextButton_3.BackgroundColor3 = Color3.new(0,0,0)
TextButton_3.BorderColor3 = Color3.new(0, 0, 0)
TextButton_3.BorderSizePixel = 1
TextButton_3.Text = "AntiAfk"
TextButton_3.TextColor3 = Color3.new(255, 255, 255)
TextButton_3.Font = Enum.Font.Code
TextButton_3.Parent = Frame
TextButton_3.TextSize = 14.00


TextButton_3.MouseButton1Click:Connect(function()
     --[[
	WARNING: Heads up! This script has not been verified by ScriptBlox. Use at your own risk!
]]
loadstring(game:HttpGet("https://raw.githubusercontent.com/evxncodes/mainroblox/main/anti-afk", true))()


end)


local TextLabel = Instance.new("TextLabel")
TextLabel.Size = UDim2.new(0.9, 35, 0.2, 0)
TextLabel.Position = UDim2.new(-0.0, 0, 0.5, -95)
TextLabel.BackgroundColor3 = Color3.new(0,0,0)
TextLabel.BorderColor3 = Color3.new(0, 0, 0)
TextLabel.BorderSizePixel = 1
TextLabel.Text = "Blades World Script"
TextLabel.TextColor3 = Color3.new(255, 255, 255)
TextLabel.Font = Enum.Font.Code
TextLabel.Parent = Frame
TextLabel.TextSize = 20.00
