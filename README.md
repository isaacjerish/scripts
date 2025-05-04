# isaac — Personalized Mac Automation CLI

This Zsh script acts as a custom command-line automation tool designed to streamline Isaac's workflow. It supports launching coding environments, study sessions, message sending, system cleanup, and wallpaper changes all from a single terminal command.

---

## Features

### `isaac code`
- Closes all unnecessary applications
- Opens:
  - GitHub in browser
  - Spotify
  - Visual Studio Code

### `isaac study`
- Closes all apps except terminal-related ones
- Opens:
  - ChatGPT desktop app
  - Spotify
  - Georgia Tech Canvas in browser
  - Plays a custom Spotify playlist

### `isaac text <name> "<message>"`
- Sends an iMessage to a contact (via AppleScript)
- Uses a local `numbers.txt` file to map contact names to phone numbers
- Gracefully handles fallback if name not found

### `isaac clean`
- Closes all GUI applications except a few whitelisted ones
- Force-quits Terminal and Visual Studio Code

### `isaac wallpaper <1|2>`
- Changes the system wallpaper to a preset image

---

##  File Structure

- `isaac` — The main script (make this executable)
- `numbers.txt` — Phone numbers and iMessage service ID (not committed to Git)