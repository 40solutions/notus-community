# Installing Notus

Notus is a desktop application for **macOS, Windows and Linux**. You install it once per computer. It needs **macOS 13 (Ventura) or later**, **Windows 10 or 11 (64-bit)**, or **Linux with glibc 2.34 or later** (Ubuntu 22.04, Debian 12 or newer). It runs entirely on your machine and needs no account to get started.

Download the installer for your computer from the Notus page at **[40solutions.com/notus](https://www.40solutions.com/notus)**.

## macOS

macOS has a **separate build for each kind of processor**: one for **Apple silicon** (M-series) Macs and one for **Intel** Macs. Download the one that matches your Mac.

1. Open the downloaded disk image.
2. Drag **Notus** into your Applications folder.
3. Open Notus from Applications.

The Mac builds are signed and notarized by Apple, so Notus opens like any other app, with no security warning to get past.

## Windows

Windows has a **64-bit installer only**. There is no build for ARM-based Windows.

1. Run the downloaded installer and follow the prompts. It installs Notus for your user account.
2. **The Windows installer is not code-signed yet**, so Windows SmartScreen may show a **"Windows protected your PC"** message. Click **More info**, then **Run anyway**. You only need to do this once.

**Windows 11 with Smart App Control turned on blocks unsigned apps outright**, with no "Run anyway" option. Notus will not run on such a machine until the Windows build is signed, which is planned for an upcoming update. Turning Smart App Control off is permanent (Windows does not let you turn it back on without reinstalling), so we don't recommend switching it off just to run Notus.

## Linux

Linux has an **AppImage** (64-bit). There is no `.deb` or `.rpm`.

1. Make the file executable: `chmod +x Notus-*.AppImage`
2. Run it: `./Notus-*.AppImage`

On newer distributions you may need to install `libfuse2` first. On some Wayland desktops Notus renders slowly; launching with `--ozone-platform=x11` fixes that.

## Updating

Notus does not update itself. When a new version is posted, download it and install it over the old one (or replace the AppImage on Linux). Your notebooks stay where they are. **One exception, from 1.1:** once 1.1 opens a notebook, older versions can't open it, so update every computer you sync notebooks between, and copy your notebooks folder first if you might go back to 1.0.

## Accepting the license agreement

The first time you launch Notus, before anything else, it shows the Notus End User License Agreement. Click **I Agree** to continue. If you click **Decline**, Notus asks you to confirm and then quits — it can't be used without accepting, and it asks again next time you launch. When a new version of the agreement ships, Notus asks you once more. You can read it again any time under **Help → License Agreement**, or read it online at [40solutions.com/notus-eula](https://www.40solutions.com/notus-eula).

## After installing

The first time you launch Notus, it asks you to choose where your notebooks will be stored. The same screen also explains what a license is for — what it unlocks, and what stays free — and tells you where licenses live: **Settings → License**. There is no key to enter during first run. Beside **Get started** there is a **Set up a license** button, which saves your storage choice and then opens **Settings → License** for you. You do not need a license to continue, and you can add one at any time later; see the Licensing guide (in Notus: Help → Documentation → Licensing) for what a license covers and how to activate one.

Notus then opens to a welcome screen with **Create New Notebook** and **Open Existing Notebook** buttons. Notus does not create a sample or "Getting Started" notebook for you — you begin from an empty workspace.

Continue to [Your first notebook](02-your-first-notebook.md).
