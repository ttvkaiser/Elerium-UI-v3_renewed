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
features:Show() -- shows the tab
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
	 -- toggle_god_mode(bool)
end)
switch:Set(true)
```
