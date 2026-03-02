# 🛡️ BetterOnTop

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
