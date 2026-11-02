# PROMPT for Claude Code — TV over WiFi

My TV is a [BRAND AND MODEL] running [Android TV / Google TV].
Its IP address is [192.168.x.x] and USB debugging is turned on.

Connect to it with adb over WiFi, confirm the model and Android version, and stop.
Explain every command before you run it. Do not change anything yet.

Once connected:
1. Take a full backup of the current package list and home settings.
2. Identify and disable manufacturer bloat, ad services, telemetry, and unused preloaded apps (use pm disable-user, never uninstall).
3. Offer to install a clean Apple TV-style launcher if appropriate.
4. Show me the plan and wait for confirmation before making changes.
5. After changes, verify Home opens to the new launcher and provide a one-command restore.

Keep everything reversible. Prefer the tools and lists from https://github.com/Gathin23/cleanyourtv if available, otherwise work carefully from first principles.
