# Empyrion---Dedicated-Server-GUI
this is a fully redeveloped EDS GUI  made to be move user friendly than the generic steam version, and can be run separately from the client side game

# Empyrion Dedicated Server Launcher

A portable, one-folder GUI for running your own **Empyrion - Galactic Survival** dedicated server on Windows.
No Steam account, no command line, no editing batch files. Extract, run, click Start.

**Download:** grab `EmpyrionServerGUI-vX.X.X.zip` from the [latest release](../../releases/latest).

---

## Quick setup (first time)

1. **Make a folder** anywhere with ~20 GB free, e.g. `D:\EmpyrionServer`
   (not inside `Program Files` or your Steam folder).
2. **Extract the whole zip** into that folder.
3. **Run `EmpyrionServerGUI.exe`**
   - Windows SmartScreen may warn about an unknown publisher: click **More info → Run anyway**.
     (The exe is a tiny stub; everything it does is in the readable `EmpyrionServerGUI.ps1` next to it.)
4. **Click Yes** when asked to download the server files. A SteamCMD window appears and downloads
   ~18 GB from Steam. Leave it open until it closes by itself.
5. A **Default** server profile is created. Select it and click **Start**.

That's it - the status bar shows **RUNNING** and your connect address.

## Joining your server

In Empyrion: **Multiplayer → Join Server → Direct Connect** (bottom of the list) and enter the address.

| Who | Address |
|---|---|
| You, on the same PC | `127.0.0.1:30000` |
| Friends on your home network | `<your LAN IP>:30000` |
| Friends via Radmin VPN / Hamachi | `<your VPN IP>:30000` (no port forwarding needed) |
| Friends over the internet | `<your public IP>:30000` (needs port forwarding, UDP 30000-30003) |

Click **Connect Info** in the launcher to see all of these with copy buttons.

**Playing on the same PC:** while the server runs, Steam shows Empyrion as "Running" and greys out Play.
This is normal. Use the **Launch Game** button in the launcher instead - it starts your Steam copy of the game directly.

## Everyday use

- **Config tab** - edit `dedicated.yaml` (server name, password, max players...). Save & Restart applies it.
- **Scenario & Mods tab** - pick a scenario from the dropdown (Steam Workshop scenarios like Reforged Eden 2
  are found automatically if you're subscribed to them in Steam), tick/untick DLL mods.
- **Backup Save** - zips your save game at any time, even while running.
- **New...** - run several servers with their own ports, saves and scenarios (one at a time).
- **Update Server** - run this after every Empyrion patch, otherwise players on the new version can't join.
- The launcher checks for its own updates on start and installs them with one click.

## Requirements

- Windows 10 / 11 (64-bit). Uses the PowerShell that's built into Windows - nothing else to install.
- ~20 GB free disk space, internet for the first download.
- A Steam client is only needed if you want Steam Workshop scenarios/mods or want to play on the same PC.

## Moving / uninstalling

Everything lives in the one folder. Move it anywhere, or delete it to remove the server completely.
Nothing is written anywhere else on the PC.

---

Found it useful? [Buy me a coffee](https://www.paypal.com/paypalme/cowslink)
