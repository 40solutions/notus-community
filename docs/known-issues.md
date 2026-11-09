# Known issues

**Notus 1.0.0** — last updated 2026-11-09

These are problems we already know about. If you hit something that isn't listed here, please [report it](https://github.com/40solutions/notus-community/issues/new/choose).

## Installing

- **The Windows installer isn't code-signed yet.** SmartScreen may show "Windows protected your PC" — click **More info → Run anyway**. On Windows 11 with **Smart App Control** turned on, Notus is blocked outright. Please don't turn Smart App Control off to get around this: on Windows, turning it off is permanent unless you reinstall. A signed installer is planned.
- **Linux: slow drawing on some Wayland desktops.** Launch Notus with `--ozone-platform=x11`.
- **No automatic updates.** Download each new version and install it over the old one. Your notebooks are not affected.

## AI agents and Coding Sessions

- **Typing in a text block while an agent is editing that same block** can cause the agent's edit to be lost. Let the agent finish first.
- **An agent's chat isn't kept after you quit and reopen Notus.** Your pages and anything the agent wrote on them are kept. Keeping the chat is planned.
- **Coding Sessions and running agents stop when you switch to another notebook.** Making them keep running is planned.
- **Coding Sessions on Windows have had less testing** than on macOS and Linux.

## Voice notes

- **Recording meetings on Linux is untested**, and may capture only your microphone, not the other people on the call.
