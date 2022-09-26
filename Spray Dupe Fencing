local amounttodupe = 500

local plr = game.Players.LocalPlayer
local backpack = plr.Backpack
local character = plr.Character
local hrp = character.HumanoidRootPart
local tool = backpack.Foil

for i = 1,amounttodupe do
	firetouchinterest(game:GetService("Workspace").Handle,hrp,0)
	firetouchinterest(game:GetService("Workspace").Handle,hrp,1)
	character.ChildAdded:wait()
	task.wait()
	for i,v in pairs(character:GetChildren()) do
		if v:IsA("Tool") then
			v.Parent = backpack
			v.Parent = character
			v.Parent = tool
			v.Parent = backpack
			v.Parent = tool
		end
	end
	task.wait()
end

for i,v in pairs(tool:GetChildren()) do
	if v:IsA("Tool") then
		tool.Parent = character
		v.Parent = character
		v.Parent = backpack
	end
end
