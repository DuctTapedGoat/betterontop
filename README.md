# 🛡️ BetterOnTop (v1.2.2)

BetterOnTop is a powerful, lightweight Windows utility built for power users to manage window states with system-wide hotkeys, persistent memory, and a specialized Glass HUD.

---

## ⚡ System Hotkeys (Ctrl + Alt + Key)

| Hotkey | Feature | Description |
|:---:|:---|:---|
| **`T`** | **Topmost** | Pins the active window to stay always on top. |
| **`W`** | **Opacity** | Toggles 70% transparency for better visibility behind windows. |
| **`U`** | **Ghost** | Enables **Click-through** mode (interact with windows behind). |
| **`L`** | **Lock Pos** | **Persistent Memory**: Automatically restores window X/Y on launch. |
| **`M`** | **Mouse Lock** | **New**: Traps the mouse inside the window with an 8px internal safety barrier. |
| **`/`** | **Glass HUD** | Toggles a "Glass" overlay showing live input and window telemetry. |
| **`Bksp`** | **Clear Log** | Instantly wipes the live Glass HUD log history. |
| **`\`** | **Save Log** | Exports all current session logs to a dated `.txt` file. |

---

## 💎 The Glass HUD (`/`)

The Glass HUD provides a non-obtrusive, high-performance telemetry display:

- **Rich Metrics**: See PIDs, Window Handles, Extended Styles, and state flags (`T`, `W`, `U`, `L`, `M`) in real-time.
- **Visual Style**: Fully transparent background with 50% opacity Cyan/Black high-contrast text.
- **Safe Positioning**: Automatically applies a 2px shave in fullscreen to ensure it stays "inside" borderless apps.
- **Hardened**: Includes anti-recursion logic to prevent hooking into itself (Explorer stability fix).

---

## 🖱️ Mouse Lock & Clipping (`M`)

The **Mouse Lock** feature is designed for borderless gaming and multi-monitor productivity:

1. **Dynamic Capture**: Locks the cursor instantly to the application frame.
2. **8px Safety Barrier**: The cursor is trapped 8 pixels inside the edge to prevent "leakage" into other screens or the taskbar.
3. **Smart Focus**: Automatically releases the clip when you Alt+Tab to another app, and re-snags it the millisecond you return.

---

## 🛠️ Control Center (System Tray)

Right-click the **Shield Icon** in your tray for total control:

- **Visual Flags**: Quick-view active states: `[T W U L M]`.
- **Run at Startup**: One-click Registry toggle to keep BetterOnTop active across reboots.
- **Global Reset**: Instantly strip all effects (topmost, transparency, ghost) from any tracked window.
- **Memory Management**: View and wipe specific application position profiles.

---

## 📦 Distribution Formats

### 1. [Standalone Installer (Offline)](file:///BetterOnTop-v1.2.2-Installer.exe)

* **Full Suite**: Includes everything needed in a single installer.
- **Self-Contained**: No external downloads required.
- **Auto-Cleanup**: Registers a clean uninstaller in Windows Settings.

### 2. [Live Setup (Online)](file:///BetterOnTop-v1.2.2-OnlineInstaller.exe)

* **Ultralight**: ~400KB bootstrap.
- **Self-Healing**: Automatically verifies and installs .NET 8 via `winget` if missing.

### 3. [Portable Standalone](file:///BetterOnTop-v1.2.2-Standalone.exe)

* **Single File**: ~67MB, includes the entire .NET runtime. Just run it.

### 4. [Portable Mini](file:///BetterOnTop-v1.2.2-Mini.exe)

* **Tiny**: ~215KB executable. Requires .NET 8 Runtime pre-installed.

---

## 🏗️ Project Organization

- `BetterOnTop-v1.2.2-Source/`: Core Application Source (C# / .NET 8).
- `BetterOnTop-v1.2.2-Installer/`: Installer project source (Offline).
- `BetterOnTop-v1.2.2-OnlineInstaller-Source/`: Bootstrap source (Online).
- `BetterOnTop-v1.2.2-Mini-Source/`: Lightweight build source.

---

Built by **Antigravity** ❤️ For power users who demand perfect window control.





# 🛡️ BetterOnTop Project (v1.1) 

https://github.com/DuctTapedGoat/betterontop/releases/download/Utility/BetterOnTop-v1.1-InstallerOnline.exe
https://github.com/DuctTapedGoat/betterontop/releases/download/Utility/BetterOnTop-v1.1-PortableMini.exe

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



# 🛡️ BetterOnTop v0.7 🫡 (original version)

BetterOnTop is a lightweight Windows utility that gives you instant control over your windows with high-speed hotkeys. Stay organized, stay focused, and keep your most important windows where they belong: **On Top.**

---

## 🔥 Key Features

BetterOnTop lives in your system tray and listens for three global hotkeys:

* **`Ctrl + Alt + T` (Topmost)**: Toggle a window to stay "Always on Top" of every other window.
* **`Ctrl + Alt + W` (Opacity)**: Make any window partially transparent (see-through) so you can peek at what's behind it.
* **`Ctrl + Alt + G` (Ghost Mode)**: Toggle "Click-through" transparency. You'll be able to see the window, but your mouse clicks will pass right through it to whatever is underneath. Ideal for overlays!

---

## 📦 Downloads (4 Ways to Use)

We offer different builds depending on your needs:

| Build | Size | Best For... |
| :--- | :--- | :--- |
| **[Standalone (Mono)](https://github.com/USER/BetterOnTop/releases)** | ~65 MB | People who want a single `.exe` that "just works" on any 64-bit Windows PC without installing anything. |
| **[Portable Mini](https://github.com/USER/BetterOnTop/releases)** | **163 KB** | Power users who already have [.NET 8](https://dotnet.microsoft.com/en-us/download/dotnet/8.0) installed and want the absolute smallest footprint. |
| **[Installer (Offline)](https://github.com/USER/BetterOnTop/releases)** | ~9 MB | A full setup experience that installs the app, adds it to your **Startup List**, and registers for easy **Uninstall** from Windows Settings. |
| **[Installer (Online)](https://github.com/USER/BetterOnTop/releases)** | ~300 KB | Same as the Offline Installer, but transparently uses `winget` to ensure the .NET 8 Runtime is installed for you. |

---

## 🛠️ Installation & Setup

1. Download your preferred version from the **[Releases](https://github.com/USER/BetterOnTop/releases)** page.
2. Run the application.
3. Look for the **Shield Icon** in your system tray (near the clock).
4. Right-click the icon to:
    * See a list of currently modified windows.
    * Reset specific windows to their original state.
    * Reset all windows at once.
    * Exit the application.

---

## 🗑️ Uninstallation

If you used the **Installer** version:

* Open Windows **Settings** > **Apps** > **Installed Apps**.
* Search for **BetterOnTop**.
* Click **Uninstall**.

If you used the **Portable** version:

* Just delete the `.exe`. (Note: you may need to manually remove it from your Startup folder if you put it there).

---

## 📜 Built With

* C# / .NET 8
* Win32 API (User32.dll)
* ❤️ and coffee.

---

*Note: As this tool interacts with system-level window handles and requires registry access for startup/uninstall, some antivirus software may flag the installer. This is normal for window-management utilities.*
