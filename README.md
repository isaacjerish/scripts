# isaac — personal CLI assistant

Tiny Zsh script that flips your Mac into preset modes with a single command.

## Features

| Command | What it does (default behavior) |
|---------|---------------------------------|
| `isaac code` | *Wipes distractions*, launches your coding stack (VS Code, GitHub tab, Spotify coding playlist). |
| `isaac study` | Quits social / entertainment apps, opens Obsidian (notes), your course site, PDF viewer, and sets Do Not Disturb. |
| `isaac text <contact> "<message>"` | Fires an iMessage or SMS via AppleScript. Great for quick “running late” pings from the terminal. |

Everything is just shell + AppleScript, so tweak any app / URL list you like.

---

## Quick install

```bash
# 1. Clone or copy the script
mkdir -p ~/scripts
cp isaac ~/scripts/isaac
chmod +x ~/scripts/isaac

# 2. Add that folder to your PATH (once)
echo 'export PATH="$HOME/scripts:$PATH"' >> ~/.zshrc
source ~/.zshrc