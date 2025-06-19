-- Example Easter Shop loader script
local player = game.Players.LocalPlayer
local ReplicatedStorage = game:GetService("ReplicatedStorage")
local EasterShopGui = ReplicatedStorage:WaitForChild("EasterShopGui")

if player and player:FindFirstChild("PlayerGui") then
    if not player.PlayerGui:FindFirstChild("EasterShopGui") then
        EasterShopGui:Clone().Parent = player.PlayerGui
    end
end
