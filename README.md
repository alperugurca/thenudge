# thenudge (Nudge)

A small **Windows** desktop app for quick notes and time-based reminders. It runs from the **system tray** and keeps data **on your device**.

## Requirements

- **Windows 10/11** (64-bit)
- **Build `Nudge.exe`:** [MinGW-w64](https://www.mingw-w64.org/) (`gcc` + `windres`) *or* **Visual Studio** with C++ desktop workload
- **Build `Nudge.msix`:** [Python 3](https://www.python.org/) and **Windows SDK** (`makeappx.exe`)

## Build

```bat
build.bat
```

Output: `dist\Nudge.exe`

**MSIX (for Microsoft Store or sideload):**

```bat
build_msix.bat
```

Output: `dist\Nudge.msix` (unsigned; [Partner Center](https://partner.microsoft.com/dashboard) signs Store submissions).

Icons and MSIX tile PNGs are generated with `gen_ico.py` when needed.

## Store / manifest

`msix\AppxManifest.xml` must match your **Partner Center** product identity (`Name`, `Publisher`, `PublisherDisplayName`). Update those values before you ship.

## License

Add a license file if you open-source the repo (e.g. MIT).
