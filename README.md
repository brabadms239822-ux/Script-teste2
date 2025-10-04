--dragon
local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/xHeptc/Kavo-UI-Library/main/source.lua"))()

-‐Windows
local Window = Library.CreateLib("dragon", "Ocean")

--tabs
local Tab = Window:NewTab("main")

Section:NewLabel("script")


--comesso

Section:NewButton("tuturiau Butão", "teste para inscritos", function()
    print("drágon")
end)


--tggles usavel
Section:NewToggle("speed", "ToggleInfo", function(state)
    if state then
        print("speed On")
    else
        print("speed Off")
    end
end)

--sloders
Section:NewSlider("SliderText", "SliderInfo", 500, 0, function(s) -- 500 (MaxValue) | 0 (MinValue)
    game.Players.LocalPlayer.Character.Humanoid.WalkSpeed = s
end)
