# Elerium V3 UI Library | SUPPORTS MOBILE AND PC

**Elerium V3** is a sleek and modern Roblox UI library, designed for script developers who want power, polish, and performance. Rewritten from scratch by **Emperor (ttvkaiser)**, Elerium V3 takes everything great about V2 — and evolves it for the next generation.

> ⚡ Fast. 🧠 Modular. 🎨 Stylish.  
> For **Vyntric Hub X** and every elite script out there.

---

## 📦 Features

- 📁 Tabs, Sections, Buttons, Toggles, Sliders, Dropdowns, Textboxes
- 🎨 Fully animated UI with blur, neon glow, and drag support
- 🔒 Key System UI (optional integration with Linkvertise, LootLabs, etc.)
- 💾 Config Save/Load System
- ⚙️ Plugin support (coming soon)
- 🔑 Toggle UI keybind
- 💬 Built-in Notifications
- 📱 Mobile-friendly

---

## 🚀 Usage

### Loadstring:
```lua
loadstring(game:HttpGet("https://raw.githubusercontent.com/ttvkaiser/Elerium-UI-v3_renewed/refs/heads/main/Library.lua"))()
```

---

### Adding Window:
```lua
local window = library:AddWindow("Name GUI", {
	main_color = Color3.fromRGB(41, 74, 122), -- Color
	min_size = Vector2.new(250, 346), -- Size of the gui
	can_resize = false, -- true or false
})
```

---

### Adding Labels:
```lua
features:AddLabel("Hello World!")
```

---

### Adding Tabs:
```lua
local features = window:AddTab("Features") -- Name of tab
features:Show() -- Shows the tab
```

---

### Adding Button:
```lua
features:AddButton("name",function()
	-- Code here
end)
```

---

### Adding Switches:
```lua
local switch = features:AddSwitch("name", function(bool)
	 -- Code can be entered here!
end)
switch:Set(true) -- Turn false if don't want it already turned on
```

---

### Adding Textboxes:
```lua
features:AddTextBox("free click", function(text) -- You can add anything to "text"
	game:GetService("ReplicatedStorage").Events.FreeGifts.Gift2:FireServer(text,"Clicks",false,false,"Normal")
end)
```

---

### WORKS ON PC, NOT ON MOBILE. I'LL FIX IT LATER!! | Adding Slider:
```lua
local slider = features:AddSlider("WalkSpeed", function(p)
	setwalkspeed(p)   
end, {                    

	["min"] = 16,
	["max"] = 100,  
})
slider:Set(16) -- Needed
```

---

### Adding Dropdowns:
```lua
local dropdown = features:AddDropdown("select", function(text)
	if text == "Mars" then  -- Code
		print("o")
	elseif text == "Earth" then
	print("k")
	elseif text == "Iridocyclitis" then
	print("Weeeee")
	end
end)
local mars = dropdown:Add("Mars")  -- Options 
local earth = dropdown:Add("Earth")
local not_a_planet = dropdown:Add("Iridocyclitis")
```

---

### Adding Console:
```lua
-- Add console for ur Script/Gui, Idk if works
features:AddConsole({ 
	["y"] = 210,
	["readonly"] = false,  
	["source"] = "Lua",
})
```

---

### Adding Folders:
```lua
-- add folder for more space
local folder = features:AddFolder()
folder:AddSwitch()
folder:AddLabel("Woo! I'm inside a folder!")

local folder2 = folder:AddFolder()
folder2:AddLabel("I'm inside *two* folders :smirk:")
```

---

#### Credits: ttvkaiser and Kuzanu
