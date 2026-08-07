# ShootTheBox-2D

**Shoot The Box** is a 2D top-down arcade shooter built with **Godot 4.2+ and GDScript**. Shoot moving boxes inside a room, earn points, clear waves and chase a high score before the 60-second timer expires.

## Features

- Top-down arcade shooting
- 15 targets in the first wave
- +5 targets every new wave
- Moving/rotating RigidBody2D boxes
- One-hit targets with particle break effect
- Score, ammo and 60-second timer
- 10-shot magazine + reload
- WASD movement
- Mobile virtual joystick
- Mouse aiming
- Mobile Shoot button
- Pause and Restart
- 1280x720 viewport
- 60 physics ticks per second
- GL Compatibility renderer
- Android, Windows Desktop and Web export presets

## Controls

### Windows / Web

- **W A S D** — Move
- **Mouse** — Aim
- **Left Mouse Button** — Shoot
- **R** — Reload
- **Pause** — Pause/resume

### Android

- **Left joystick** — Move
- **SHOOT** — Shoot
- **R** — Reload
- **PAUSE** — Pause/resume

## How to Run

1. Install Godot **4.2 or newer**.
2. Import the repository folder into the Godot Project Manager.
3. Open `scenes/Main.tscn`.
4. Press **F6** to run the main scene or **F5** to run the project.

## How to Export Android APK

1. Install the Android export templates from Godot.
2. Configure the Android SDK and JDK in Godot's Editor Settings.
3. Open **Project > Export**.
4. Select the included **Android** preset.
5. Set your final package/keystore values for release distribution.
6. Choose **Export Project** and select an APK destination.

The included `export_presets.cfg` contains a ready Android preset with ARM architectures enabled. SDK/JDK locations and release signing credentials are intentionally machine-specific and should be configured locally.

## Windows Export

Open **Project > Export**, select **Windows Desktop**, and export the executable.

## Web Export

Open **Project > Export**, select **Web**, and export the project. Host the generated files through a web server.

## Screenshots

Place gameplay images in `docs/screenshots/`, then add them here, for example:

```md
![Gameplay](docs/screenshots/gameplay.png)
```

## Repository Structure

```text
ShootTheBox-2D/
├── assets/
│   ├── player.png
│   ├── box.png
│   ├── bullet.png
│   ├── wall.png
│   ├── shoot.wav
│   ├── hit.wav
│   └── break.wav
├── scenes/
│   ├── Main.tscn
│   ├── Player.tscn
│   ├── Box.tscn
│   └── Bullet.tscn
├── scripts/
│   ├── player.gd
│   ├── box.gd
│   ├── bullet.gd
│   ├── game_manager.gd
│   ├── ui.gd
│   └── virtual_joystick.gd
├── docs/screenshots/
├── project.godot
├── export_presets.cfg
├── .gitignore
├── LICENSE
└── README.md
```

## License

MIT License. See `LICENSE`.
