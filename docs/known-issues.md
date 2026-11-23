# Known issues

**Notus 1.1.0** — last updated 2026-11-22

These are problems we already know about. If you hit something that isn't listed here, please [report it](https://github.com/40solutions/notus-community/issues/new/choose).

## ⚠️ PDF blocks in 1.1.0

- **Every PDF block shows "PDF render failed" in 1.1.0.** Your PDFs are safe and unchanged in your notebooks; they display again once the fix is installed. A quick update is coming ([#10](https://github.com/40solutions/notus-community/issues/10)).

## Installing

- **Notus 1.1 needs macOS 13 (Ventura) or later.** On Linux it needs glibc 2.34 or later (Ubuntu 22.04, Debian 12 or newer). Windows 10 or 11, 64-bit, is unchanged.
- **Once 1.1 opens a notebook, older versions of Notus can't open it.** Nothing is lost; an older Notus just says the notebook needs a newer version. If you sync notebooks between computers, update them all to 1.1. If you might go back to 1.0, copy your notebooks folder before you update.
- **The Windows installer isn't code-signed yet.** SmartScreen may show "Windows protected your PC" — click **More info → Run anyway**. On Windows 11 with **Smart App Control** turned on, Notus is blocked outright. Please don't turn Smart App Control off to get around this: on Windows, turning it off is permanent unless you reinstall. A signed installer is planned.
- **Linux: slow drawing on some Wayland desktops.** 1.1 runs on a much newer engine, which may fix this. If you still see it, launch Notus with `--ozone-platform=x11`, and please tell us in a [new issue](https://github.com/40solutions/notus-community/issues/new/choose).
- **No automatic updates.** Download each new version and install it over the old one. Your notebooks are not affected.

## AI agents and Coding Sessions

- **Typing in a text block while an agent is editing that same block** can cause the agent's edit to be lost. Let the agent finish first.
- **An agent's chat isn't kept after you quit and reopen Notus.** Your pages and anything the agent wrote on them are kept. Keeping the chat is planned.
- **Coding Sessions and running agents stop when you switch to another notebook.** Making them keep running is planned.
- **Coding Sessions on Windows have had less testing** than on macOS and Linux.

## Terminals

- **Cmd+Z (Ctrl+Z on Windows and Linux) typed in a terminal block on the canvas undoes your last canvas change** instead of reaching the terminal. Inside a pop-out it works normally. A fix is planned for 1.1.2.

## Voice notes

- **Mac: recording a meeting's computer audio needs one setting.** Turn Notus on in the **top** list of System Settings → Privacy & Security → Screen & System Audio Recording, then quit and reopen Notus. Without it, the meeting records your microphone only, and Notus tells you what to change.
- **Recording meetings on Linux is untested**, and may capture only your microphone, not the other people on the call.
