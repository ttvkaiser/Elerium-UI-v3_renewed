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

## 📄 Preview

![Elerium V3 Banner](https://imgur.com/a/AZLZbJd)

---

## 🚀 Usage

### Loadstring:
```lua
local library = loadstring(game:HttpGet("https://raw.githubusercontent.com/ttvkaiser/Elerium-UI-v3_renewed/refs/heads/main/Library.lua", true))()
```

---

### Adding Window:
```lua
local window = library:AddWindow("Elerium UI Example | Recontinued", { -- You can change the Name!
	main_color = Color3.fromRGB(41, 74, 122), -- Color
	min_size = Vector2.new(500, 500), -- Size of the gui, you can change it. To adjust your size of script
	can_resize = false, -- true or false
})
```

---

### Adding Tabs:
```lua
local main = window:addtab("Main") -- Name of tab
main:Show() -- Shows the tab
```

---

### Adding Labels:
```lua
main:AddLabel("Label Example")
```

---

### Adding Button:
```lua
main:AddButton("Button Example",function()
	-- Code here
end)
```

---

### Adding Switches:
```lua
local switch = main:AddSwitch("Switch Example", function(bool)
	 -- Code can be entered here!
end)
switch:Set(true) -- Turn false if don't want it already turned on
```

---

### Adding Textboxes:
```lua
main:AddTextBox("Text Box Example", function(text) -- You can add anything to "text"
	game:GetService("ReplicatedStorage").Events.FreeGifts.Gift2:FireServer(text,"Clicks",false,false,"Normal")
end)
```

---

### WORKS ON PC, NOT ON MOBILE. I'LL FIX IT LATER!! | Adding Slider:
```lua
local slider = main:AddSlider("Slider Example", function(p)
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
local dropdown = main:AddDropdown("Dropdown Example", function(text)
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
main:AddConsole({ 
	["y"] = 210,
	["readonly"] = false,  
	["source"] = "Lua",
})
```

---

### Adding Folders:
```lua
-- add folder for more space
local folder = main:AddFolder("    Example Folder")
folder:AddSwitch()
folder:AddLabel("Woo! I'm inside a folder!")

local folder2 = folder:AddFolder()
folder2:AddLabel("I'm inside *two* folders :smirk:")
```

---

#### Credits: ttvkaiser and Kuzanu
