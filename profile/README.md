# RenCord
[![ren.gay badge](badge.svg)](https://github.com/rendotgay)

## Prerequisites
- Git
- Node.js
- pnpm

## Installation
1. [Build Vencord from source](https://docs.vencord.dev/installing/)
  ### Windows (cmd)
  ```cmd
  (where git >nul 2>nul || winget install --id Git.Git -e -h --accept-source-agreements --accept-package-agreements) && (where node >nul 2>nul || winget install --id OpenJS.NodeJS.LTS -e -h --accept-source-agreements --accept-package-agreements) && set "PATH=%PATH%;C:\Program Files\Git\cmd;%LOCALAPPDATA%\Programs\Git\cmd;C:\Program Files\nodejs;%APPDATA%\npm;%LOCALAPPDATA%\pnpm" && (where pnpm >nul 2>nul || call npm install -g pnpm) && (if not exist "%USERPROFILE%\Documents\Vencord" git clone https://github.com/Vendicated/Vencord.git "%USERPROFILE%\Documents\Vencord") && cd /d "%USERPROFILE%\Documents\Vencord" && call pnpm install && call pnpm build && call pnpm inject --branch auto
  ```
  ### Linux
  ```bash
  (command -v git >/dev/null 2>&1 && command -v node >/dev/null 2>&1 || (which apt-get >/dev/null 2>&1 && sudo apt-get update && sudo apt-get install -y git nodejs npm || which pacman >/dev/null 2>&1 && sudo pacman -Sy --noconfirm git nodejs npm || which dnf >/dev/null 2>&1 && sudo dnf install -y git nodejs npm || which zypper >/dev/null 2>&1 && sudo zypper install -y git nodejs npm)) && (command -v pnpm >/dev/null 2>&1 || sudo npm install -g pnpm) && ([ -d "$HOME/Documents/Vencord" ] || git clone https://github.com/Vendicated/Vencord.git "$HOME/Documents/Vencord") && cd "$HOME/Documents/Vencord" && pnpm install && pnpm build && pnpm inject --branch auto
  ```
2. Installing a plugin
  From your Vencord directory, run:
  ```bash
  cd src/userplugins
  git clone <repo>
  pnpm build
  ```

---
<sub>RenVencord is not associated with Discord or Vencord.</sub>
