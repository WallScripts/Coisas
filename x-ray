XRayVision = Instance.new("Tool")
XRayVision.Name = "X-RayTool"
XRayVision.RequiresHandle = false
XRayVision.Parent = game.Players.LocalPlayer.Backpack

local function enableXRay()
for _, Part in pairs(workspace:GetDescendants()) do
if Part:IsA("BasePart") and not Part:IsDescendantOf(game.Players.LocalPlayer.Character) then
Part.Transparency = 0.5
end
end
end

local function disableXRay()
for _, Part in pairs(workspace:GetDescendants()) do
if Part:IsA("BasePart") and not Part:IsDescendantOf(game.Players.LocalPlayer.Character) then
Part.Transparency = 0
end
end
end

local xRayEnabled = false
XRayVision.Activated:Connect(function()
if xRayEnabled then
disableXRay()
else
enableXRay()
end
xRayEnabled = not xRayEnabled
end)
