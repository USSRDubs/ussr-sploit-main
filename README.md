local userKey == "f12DF33" -- USSRSploit key required for login (Accessible if your smart)
local hacker = "USSRDubs" -- Change this to your ROBLOX username

local enterButton = Instance.new("TextButton")
local userKeyEnterBox = Instance.new("TextBox")
local newframe = Instance.new("Frame")

local function loadLogin()
  local gui = Instance.new("StarterGui")
  gui.Name = "USSRSploit_LoginID1"
  newframe.Size = UDim2.new(0, 400, 0, 600)
  newframe.AnchorPoint = "0.5, 0.5"
  newframe.Position = UDim2.new(0.5, 0, 0.5, 0)
  userKeyEnterBox.AnchorPoint = "0.5, 0.5"
  userKeyEnterBox.PlaceholderText = "Login key"
  userKeyEnterBox.Parent = newframe
  userKeyEnterBox.Position = UDim2.new("0, 400, 0, 525")
  enterButton.Text = "Log in"
  enterButton.Parent = newframe
  enterButton.Position = UDim2,new("0, 400, 0, 600")
  newframe.Parent = gui
  gui.Parent = hacker.PlayerGui
end)

loadLogin()

enterButton.MouseButton1Click:Connect(function()
   if userKeyEnterBox.Text == userKey then
      print("Logged in as "..hacker)
      enterButton.Text = "Success, logging in"
      wait(2)
   end
end)
