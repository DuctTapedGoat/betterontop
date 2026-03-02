# 🛡️ BetterOnTop Project (v1.1)

BetterOnTop is a powerful, lightweight Windows utility built for power users to manage window states with system-wide hotkeys and persistent memory.

---

## ⚡ Key Features (NEW in v1.1)

| Hotkey (Ctrl + Alt +) | Feature | Description |
|:---:|:---|:---|
| **`T`** | **Topmost** | Pins the active window to stay always on top of others. |
| **`W`** | **Window Opacity** | Toggles 75% transparency to see through windows. |
| **`U`** | **Unlock (Ghost)** | Enables **Click-through** mode (interact with windows behind). |
| **`L`** | **Lock Position** | **Continuous Position Memory**: Automatically restores window X/Y on launch. |

---

## � Persistent Window Position (`L`)

Unlike simple snapshots, the **Lock** feature (`Ctrl + Alt + L`) creates a per-app profile:

1. **Dynamic Tracking**: Once locked, BetterOnTop monitors that window's position as you move it.
2. **Auto-Restore**: When you relaunch that program next time (or next session), it **immediately snaps** back to its last known coordinates.
3. **Tray Visibility**: Manage which windows are being remembered through the system tray.

---

## 🛠️ System Tray Control Center

Right-click the **Shield Icon** in your tray for:

- **Status Indicators**: Each active window shows its state: `[T W U L]`.
- **Run at Startup**: Auto-toggle Windows Registry entry for self-launch.
- **Active Filter**: The menu intelligently hides windows that are no longer running.
- **Self-Cleaning**: Use "Forget All" to wipe your position memory database.

---

## 📦 Distribution Formats

### [BetterOnTop-PortableMini.exe]

* ~180KB Single-file executable.
- Zero installation.
- Requires .NET 8 Runtime installed.

### [BetterOnTop-InstallerOnline.exe]

* Self-guided setup UI.
- **Auto-dependency check**: Offers to install .NET 8 via `winget`.
- Registers for clean uninstallation via Windows Apps & Features.

---

## � Note on Permissions

BetterOnTop requires **Administrator Privileges** to:

1. Register system-wide hotkeys securely.
2. Interact with other admin-level windows (Task Manager, Command Prompt, etc.).
3. Manage Registry keys for "Run at Startup."

---

## 🏗️ Project Structure

- **/BetterOnTop-v1.1**: Core development source.
- **/BetterOnTop-v1.1-MiniPortable-Source**: Build source for the portable mini version.
- **/BetterOnTop-v1.1-InstallerOnline-Source**: Build source for the installer and embedded app.

Built with ❤️ for power users.
