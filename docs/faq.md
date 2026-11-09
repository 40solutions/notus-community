# Frequently asked questions

Can't find your answer? Check **Help → Documentation** in Notus, the [known issues](known-issues.md), or [ask a question](https://github.com/40solutions/notus-community/issues/new/choose).

### What's free, and what does Notus Annual add?

**Free, forever:** notebooks, sections and pages, the page canvas, writing and formatting, shapes and diagrams, images, PDFs, and search.

**Notus Annual** adds connectors — email, calendar, Slack, databases, MQTT, I3X and MCP servers — plus AI agents, Coding Sessions, terminals and voice notes.

Without a license, your notes are never locked: everything you've written stays readable and editable.

### Where are my notes stored?

On your own computer. Each notebook is an ordinary file in the folder you chose the first time you ran Notus. Back up that folder and you've backed up your notes. Updating Notus never touches your notebooks.

### Can I use Notus on more than one computer?

Yes. One license covers up to three computers, as stated at purchase. To activate it, open **Settings → License** on each computer and enter your key.

### How do I move my license to a new computer?

On the old computer, open **Settings → License** and click **Deactivate this machine**. Then activate on the new computer. If you can't get to the old computer any more, you can release it from the list of machines in **Settings → License** on any computer that uses your license.

### Can I keep my notebooks in iCloud Drive, Dropbox or OneDrive?

Yes — on **one computer at a time**. Quit Notus on one computer and let the sync finish before you open the notebook on another. If a notebook looks like it's still open on another computer, Notus warns you before opening it.

### Do I have to pay for AI separately?

Yes. Notus uses your own API key from **Anthropic, OpenAI, OpenRouter or SpaceXAI**, and your provider bills you directly. Notus is never in the middle of that bill. You can see what you've spent under **View → AI Spend Report**.

### Can I use my Claude Pro or Max plan?

Not inside the AI agent block — it needs an API key. But you can use your plan through a **Coding Session**, which runs your own copy of Claude Code, signed in with your own account, right on the page.

### Does Notus send my data anywhere?

No telemetry. Your notes stay on your computer. Content only goes to services you choose to connect — for example, when you ask an AI agent something, that goes to your AI provider. If you enter a license key, Notus checks it with our licensing provider; free use makes no license check at all.

### Windows says "Windows protected your PC", or won't run Notus at all

The Windows installer isn't code-signed yet (a signed installer is planned).

- **"Windows protected your PC"** is SmartScreen. Click **More info → Run anyway**.
- **No "Run anyway" button** means Windows 11 Smart App Control is blocking it. We don't recommend turning Smart App Control off — on Windows, that can't be undone without reinstalling.

### On Linux, Notus is slow to draw the screen

On some Wayland desktops, launch Notus with `--ozone-platform=x11`:

```
./Notus-*.AppImage --ozone-platform=x11
```

### How do I update Notus?

Notus doesn't update itself yet. Download the new version from [40solutions.com/notus](https://www.40solutions.com/notus) and install it over the old one (on Linux, replace the AppImage). Your notebooks are untouched. To see which version you have, choose **Help → About Notus**.

### How do I report a problem?

Open a [new issue](https://github.com/40solutions/notus-community/issues/new/choose) and choose **Bug report**. You can also start from **Help → Report an Issue…** in Notus, or ask a Notus agent or Claude Code in a Coding Session to draft one for you — you always review it and click **Submit** on GitHub yourself.

**Issues are public.** Never include license keys, API keys, passwords, tokens or notebook contents. Security problems go to **contact@40solutions.com**, not a public issue.
