local Library = loadstring(game:HttpGet("https://raw.githubusercontent.com/NIcoGabrielRealYtr/Aether.lua-Library/refs/heads/main/Source"))()

local MainWindow = Library:CreateWindow({
    Title = "Title",
    SubText = "SubTitle",
    Image = "rbxassetid://95259225424429",
    IsMobile = true
})

local CombatTab = MainWindow:AddTab({
    Text = "Tab",
    Icon = "rbxassetid://108020878442937"
})

local AimSection = CombatTab:AddSection({
    Title = "Left Section",
    Side = "Left"
})

-- Add elements to section
AimSection:AddToggle({
    Text = "Toggle",
    Flag = "aimbot",
    Default = true,
    Callback = function(value)
        print("Aimbot:", value)
    end
})

AimSection:AddSlider({
    Text = "Slider",
    Flag = "aimbot_fov",
    Min = 0,
    Max = 360,
    Default = 120,
    Suffix = "°",
    Callback = function(value)
        print("FOV:", value)
    end
})

AimSection:AddDropdown({
    Text = "Hit Part",
    Flag = "hit_part",
    Options = {"Head", "Chest", "Legs"},
    Default = "Head",
    Callback = function(value)
        print("Target:", value)
    end
})

-- Add another section on the right side
local VisualSection = CombatTab:AddSection({
    Title = "Right Section",
    Side = "Right"
})

VisualSection:AddColorPicker({
    Text = "FOV Color",
    Flag = "fov_color",
    Default = Color3.fromRGB(255, 0, 0),
    Transparency = 0.5,
    Callback = function(color, alpha)
        print("Color set")
    end
})

VisualSection:AddKeyPicker({
    Text = "ESP Key",
    Flag = "esp_key",
    Default = "RightShift",
    Mode = "Toggle",
    Callback = function(value)
        print("Key state:", value)
    end
})

Library:Notify({
    Title = "Script Loaded!",
    Lifetime = 3
})
