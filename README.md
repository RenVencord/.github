# RenCord
A collection of Vencord plugins made by [ren](https://github.com/rendotgay)

## Prerequisites
- Git
- Node.js
- pnpm

## Installation
1. [Build Vencord from source](https://docs.vencord.dev/installing/)
  ```bash
  git clone https://github.com/Vendicated/Vencord
  cd Vencord
  pnpm install --frozen-lockfile
  pnpm build
  pnpm inject
  ```
2. Installing a plugin
  From your Vencord directory, run:
  ```bash
  cd src/userplugins
  git clone <repo>
  cd ../..
  pnpm build
  ```
