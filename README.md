# tv-claude-code

Repo for TVs that **Claude Code** connects over WiFi (via ADB) to debloat, change the home screen, and update content.

This is a starter/workspace for the popular CleanYourTV workflow (and similar projects).

## What this is for
- Android TV / Google TV devices
- Connect from your computer (running Claude Code) over the same WiFi network
- Enable USB/Wireless debugging on the TV
- Claude Code uses ADB to:
  - Backup current state
  - Disable bloatware, ads, telemetry packages (`pm disable-user`)
  - Install a clean Apple TV-style launcher
  - Optionally push custom content, themes, or apps

**Nothing is uninstalled** — everything is reversible.

## Quick start

1. **On the TV**
   - Settings → Device Preferences → About → Press OK on "Build" 7 times to enable Developer Options
   - Developer Options → Turn on **USB debugging** (and Wireless debugging if available)
   - Note the TV's local IP address (Settings → Network)

2. **On your computer** (same WiFi)
   ```bash
   git clone https://github.com/albahaj725-pixel/tv-claude-code.git
   cd tv-claude-code
   # Open this folder in Claude Code
   ```

3. **In Claude Code**
   - Paste the contents of `PROMPT.md`
   - Fill in your TV model and IP address
   - Accept the "Allow USB debugging" prompt on the TV

## Recommended upstream project
For full debloat lists, launcher source, and community support for 400+ models:

**https://github.com/Gathin23/cleanyourtv**  
Website: https://cleanyour.tv

Clone that one if you want the complete ready-to-use toolkit. Use this repo as a personal workspace or for custom changes.

## Safety notes
- Only connect on your local network
- Turn debugging off when finished
- Backup first (the prompt does this)
- Fully reversible via restore scripts

## Structure
- `PROMPT.md` — Ready-to-paste prompt for Claude Code
- Add your own model-specific lists, themes, or content here
