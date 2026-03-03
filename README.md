# Dodge the Creeps — Your First 2D Game (Godot)

Simple 2D survival demo built while following the official "Your First 2D Game" Godot tutorial.
The player must avoid enemies (creeps) that spawn randomly. Survive as long as possible to increase
your score.

Tutorial reference
: https://docs.godotengine.org/en/latest/getting_started/first_2d_game/index.html

## Table of contents

- Project overview
- Requirements
- Quick start (open & run)
- Controls
- Project structure (what's in this repo)
- Assets & credits
- Contributing
- License / Notes

## Project overview

This is a small educational project showcasing core Godot concepts:

- Scenes and instancing
- GDScript for gameplay logic
- Signals for node communication
- Timers and spawning logic
- Collision detection and simple UI (HUD)

It's intended as a learning/example project rather than a full commercial game.

## Requirements

- Godot Engine (recommended: Godot 3.2+). If you try Godot 4.x you may need to adjust some APIs.
- A desktop OS (Windows, macOS, Linux) with Godot installed.

## Quick start — open and run

1. Install Godot from https://godotengine.org.
2. Open Godot and choose "Import" or "Scan" to open the project folder, or open the folder that contains `project.godot`.
3. In the Godot editor, open `main.tscn` (or set it as the main scene) and press Play (F5) to run.

Optional: clone the repository locally:

```powershell
git clone https://github.com/zmoussam/Your_first_2D_game_with_Godot-.git
cd "Your_first_2D_game_with_Godot-"
# Then open the folder from Godot
```

## Controls

- Move: Arrow keys or WASD
- Objective: avoid enemies; score increases the longer you survive

## Gameplay video

Below is a short gameplay recording. If your platform supports HTML5 video (for example, GitHub will show a playable video for supported file types), use the player; otherwise click the download link.

<video controls width="640">
  <source src="./media/gameplay.mp4" type="video/mp4">
  Your browser does not support the video tag. You can download the video here: [gameplay.mp4](./media/gameplay.mp4)
</video>
 
## Project structure (short)

- `project.godot` — Godot project file
- `scenes/` — game scenes (.tscn)
  - `main.tscn` — main scene / entry point
  - `player.tscn`, `mob.tscn`, `hud.tscn` — core scenes used by the game
- `scripts/` — GDScript files
  - `main.gd`, `player.gd`, `mob.gd`, `hud.gd`
- `art/` — imported sprites and audio (images and sounds used by the game)
- `fonts/` — font files and license notes for fonts
- `media/` — (optional) external media like demo videos

Example listing from this repo:

```
project.godot
scenes/
  ├─ main.tscn
  ├─ player.tscn
  ├─ mob.tscn
  └─ hud.tscn
scripts/
  ├─ main.gd
  ├─ player.gd
  ├─ mob.gd
  └─ hud.gd
art/
fonts/
media/
```

## Assets & credits

- Art and sound assets included in `art/` and `media/` are part of this project's learning materials.
- Fonts: see `fonts/` (license files for fonts may be included there).

If you plan to reuse assets outside this project, verify the original license for each file.

## Contributing

Small contributions are welcome (fixes, readme improvements). Suggested workflow:

1. Fork the repo
2. Create a branch for your change
3. Open a pull request describing the change

## License / Notes

This repository contains example/educational material. There is no project-level license file in
this repo — assume the code and assets are provided for learning and demonstration. Contact the
repository owner if you need permission for other uses.

---