TechDrive 95 Edition
=====================
Tribute / classic command menu for Windows 95 and higher

This is the oldest edition in the TechDrive family.

---------------------------------------------------------------------
OFFICIAL NOTICE
---------------------------------------------------------------------

TechDrive 95 Edition is owned and published by TechDrive. It is NOT
a community-made, fan-made, or third-party build.

This is the first and final release of this edition. No further
updates, changes, or support are planned or provided for it - what
you have here is the complete, finished package.

It was created simply as a small, goodwill contribution to the
retro computing community. It is completely free to use, no
payment is required, and it always will be.

---------------------------------------------------------------------
REALITY CHECK (read this)
---------------------------------------------------------------------

A full TechDrive-style Python + Tkinter application cannot run on
Windows 95 in any supported or recommended way.

Reasons:

  1. Python 3.x has never supported Windows 95.
  2. The last Python series with any historical Win9x mentions
     (old 2.x) is abandoned, unmaintained, and not safe to install
     from a security standpoint in 2026.
  3. Windows 95 has no PowerShell, no modern WMI/wmic stack like XP,
     no DISM, no SFC /scannow, no BitLocker, no Defender APIs, etc.
  4. Modern packages (psutil, cryptography, Pillow, ...) do not exist
     for that platform.
  5. Plain Windows 95 (pre-OSR2) doesn't even ship TCP/IP networking
     by default - it has to be added via Add/Remove Programs before
     winipcfg, net, or netstat will do anything useful.

Therefore this package is intentionally a **batch-file menu** that
only launches commands and tools that actually shipped with the
Windows 95 era. It is a tribute and a practical cheatsheet, not a
fake port of the modern app.

---------------------------------------------------------------------
What this menu can do
---------------------------------------------------------------------

  [OK]  ver, mem, dir, tree, set, date, time
  [OK]  Scandisk / Defrag (if present on the system)
  [OK]  Basic net commands, winipcfg - only if TCP/IP networking was
        installed (not present on a stock Windows 95 Gold install)
  [OK]  Environment listing and simple status screens

  [X]   Everything that needs Python 3, PowerShell, modern WMI,
        cloud, security modules, live graphs, etc.

---------------------------------------------------------------------
How to run
---------------------------------------------------------------------

1. Copy the whole TechDrive_95 folder to the Windows 95 machine
   (floppy, USB if the box supports it, network share, CD, etc.).

2. Double-click:

      TechDrive95.bat

3. Pick a number from the menu.

No installer. No Python. No extra DLLs.

---------------------------------------------------------------------
Sister editions (for real diagnostic work)
---------------------------------------------------------------------

  Windows XP ........ TechDrive XP Edition    
  Windows 7 ......... TechDrive Win7 Edition  
  Windows 10 / 11 ... Main TechDrive

Use those on supported OS versions. Use this 95 menu only on actual
Windows 95 (or later) boxes when you need a quick classic toolkit.

---------------------------------------------------------------------
Files
---------------------------------------------------------------------

  TechDrive95.bat     Main menu
  README_95.txt       This file
  docs\LIMITATIONS.txt
  assets\             Optional icon (may not display on pure 95)

---------------------------------------------------------------------
Have fun keeping the old hardware alive — safely.
---------------------------------------------------------------------
