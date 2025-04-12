# ImGui-Keybind
## Works out of the box with Medal.tv & Nvidia Overlays.

## discord: m2n5m35n63b5mbv56m34bm73v4bn3v5v

## Example Usage
```cpp
namespace keybinds { // char mappings
	inline int triggerbot_key = 0x45;
	inline int player_select_key = 0x43;
	inline int visuals_key = 0x4c;
	inline int macro_key = 0x58;
	inline int camlock_key = 0x47;
}

namespace listeners {
	inline bool triggerbot_listener = false;
	inline bool camlock_listener = false;
	inline bool player_select_listener = false;
	inline bool visuals_listener = false;
	inline bool macro_listener = false;
}

Keybind(&cache::keybinds::triggerbot_key, "Triggerbot Key", &cache::listeners::triggerbot_listener, "tb");
Keybind(&cache::keybinds::camlock_key, "Camlock Key", &cache::listeners::camlock_listener, "cl");
Keybind(&cache::keybinds::player_select_key, "Player Select Key", &cache::listeners::player_select_listener, "ps");
Keybind(&cache::keybinds::visuals_key, "Visuals Key", &cache::listeners::visuals_listener, "vs");
Keybind(&cache::keybinds::macro_key, "Macro Key", &cache::listeners::macro_listener, "mc");
```
