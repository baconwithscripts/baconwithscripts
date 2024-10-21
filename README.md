local RejoinTime = 900  -- second(s)
local TeleportService = game:GetService("TeleportService")
local Players = game:GetService("Players")

local function rejoinGame()
    local player = Players.LocalPlayer
    print("Rejoining Server, Please Wait...")  -- Simple output to the console
    TeleportService:TeleportToPlaceInstance(game.PlaceId, game.JobId, player)
end

print("Script Loaded Successfully!")  -- Simple output to the console

wait(RejoinTime)
rejoinGame()
