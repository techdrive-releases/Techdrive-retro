# TechDrive XP Edition

Separate edition for **Windows XP SP2/SP3 and Windows Vista (32-bit and
64-bit) + Python 3.4.4**.

## Official notice

TechDrive XP Edition is owned and published by TechDrive. It is **not**
a community-made or third-party build.

**This is the first and final release of this edition.** No further
updates, bug fixes, feature additions, or technical support will be
provided for it, ever — this build is complete and final as-is.

**If you're on Windows 7, 8, 10, 11, or later, use a modern, actively
maintained TechDrive edition instead.** This legacy edition exists only
to help keep genuinely old XP/Vista hardware useful, not as a general
recommendation.

It was created as a small, free contribution to the retro computing
community. No payment is required, and it never will be.

**Copying, redistributing, or modifying the source code of this
software is not allowed.** See [`EULA_XP.txt`](EULA_XP.txt) for the
full license terms. By using this software, you agree to those terms.

This is **not** a cut-down copy of the modern TechDrive. It is a dedicated
application written for the last official Python that still ran on XP
(Python 3.4.4) and for the commands that actually exist on XP/Vista
(`wmic`, `systeminfo`, `netsh`, `sc`, `reg`, classic Control Panel applets).

## Requirements

| Item | Notes |
|------|--------|
| **OS** | Windows XP SP2/SP3 or Windows Vista — 32-bit or 64-bit |
| **Python** | **3.4.4** (last official build that supported XP) |

| **Extra packages** | **None** – uses only the standard library |

Download Python 3.4.4 from the official archives:  
https://www.python.org/downloads/release/python-344/

## Run

Double-click:

```
Run_TechDrive_XP.bat
```

Or from a command prompt:

```
python techdrive_xp.py
```

The batch file also looks for common install paths (`C:\Python34\`, etc.).

## What you get

- Classic XP-style blue header / Tahoma UI
- Full original-style catalogue (hundreds of entries) with clear status:
  - **[OK] WORKS** – implemented with XP-era commands
  - **[~] LIMITED** – guidance or partial result
  - **[X] NO** – not available on XP (shown so the full scope is visible)
- System inventory, disk space, network config, processes, services, hardware IDs
- Launch of classic applets (Display, Network Connections, etc.)
- App icon (`techdrive_icon.ico`)
- Optional startup sound (bundled WAV, played via `winsound`) - **off by
  default**, toggle it on in File > Settings
- Built-in Settings dialog (File > Settings, or the Settings toolbar
  button): launch reminder popup on/off, startup sound on/off
- Built-in Help and License (EULA) viewers (Help menu) - no need to open
  a separate file, the full text is right there in the app

Open **Utilities → Compatibility Matrix** inside the app for the full
tool-by-tool status list.

## Why many tools are marked [X]

Modern TechDrive relies on:

- Python 3.8+ language features and packages (psutil, WMI, Pillow, …)
- PowerShell modules (Defender, BitLocker, TPM, …)
- DISM, modern CBS logs, cloud APIs, etc.

None of those exist on stock Windows XP. Tools that *can* work use only
commands and COM surfaces that shipped with XP.

For the complete modern experience use:

- **TechDrive Win7 + Python 3.8.10 edition** on Windows 7  
- **Main TechDrive** on Windows 10 / 11

## Files in this package

```
techdrive_xp.py          Main application
py34_compat.py           XP / Python 3.4 helpers
tool_status.py           Full catalogue + WORKS/LIMITED/NO status
original_catalogue.py    Original tool names (display)
gui/theme.py             Classic blue XP-style theme
gui/assets/sounds/       Startup / Shutdown / Error WAVs
techdrive_icon.ico       Application icon
Run_TechDrive_XP.bat     Launcher
docs/LIMITATIONS.md      Detailed limitations
README_XP.md             This file
```

## Support reality

Windows XP reached end of support in April 2014. This edition exists so
technicians who still encounter XP machines can run a useful set of
diagnostics and repair helpers. Full feature parity with modern TechDrive
is impossible and is not claimed.
