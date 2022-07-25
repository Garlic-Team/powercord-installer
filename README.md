<h1 align="center">Powercord Installer</h1>

<p align="center">
  <a href="#overview">Overview</a> |
  <a href="#development">Development</a> |
  <a href="#contributors">Contributors</a>
</p>

<p align="center">
  <img alt="Preview" width="524" alt="Hero image" src="https://user-images.githubusercontent.com/32397453/169029285-b1307d75-b3c1-4764-8849-69cf35fb523f.png"/>
  <br/>
  <i>This is an unofficial project and we are not affiliated with Powercord.<br><br><b>
  Powercord is officially supported on Canary, if you're an average user, please referain from using the Development channel, it may cause confict!</b></i><br/><br>
  A simple standalone program which automates the installation, removal and maintenance of <a href="https://github.com/powercord-org/powercord">Powercord</a>.
  <br/>
  <br/>
  <a href="https://discord.gg/AjKJSBbGm2" target="_blank">
    <img src="https://img.shields.io/badge/discord-join-green?labelColor=242831&color=7289da&style=for-the-badge&logo=data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iNzEiIGhlaWdodD0iNTUiIHZpZXdCb3g9IjAgMCA3MSA1NSIgZmlsbD0ibm9uZSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4NCjxnIGNsaXAtcGF0aD0idXJsKCNjbGlwMCkiPg0KPHBhdGggZD0iTTYwLjEwNDUgNC44OTc4QzU1LjU3OTIgMi44MjE0IDUwLjcyNjUgMS4yOTE2IDQ1LjY1MjcgMC40MTU0MkM0NS41NjAzIDAuMzk4NTEgNDUuNDY4IDAuNDQwNzY5IDQ1LjQyMDQgMC41MjUyODlDNDQuNzk2MyAxLjYzNTMgNDQuMTA1IDMuMDgzNCA0My42MjA5IDQuMjIxNkMzOC4xNjM3IDMuNDA0NiAzMi43MzQ1IDMuNDA0NiAyNy4zODkyIDQuMjIxNkMyNi45MDUgMy4wNTgxIDI2LjE4ODYgMS42MzUzIDI1LjU2MTcgMC41MjUyODlDMjUuNTE0MSAwLjQ0MzU4OSAyNS40MjE4IDAuNDAxMzMgMjUuMzI5NCAwLjQxNTQyQzIwLjI1ODQgMS4yODg4IDE1LjQwNTcgMi44MTg2IDEwLjg3NzYgNC44OTc4QzEwLjgzODQgNC45MTQ3IDEwLjgwNDggNC45NDI5IDEwLjc4MjUgNC45Nzk1QzEuNTc3OTUgMTguNzMwOSAtMC45NDM1NjEgMzIuMTQ0MyAwLjI5MzQwOCA0NS4zOTE0QzAuMjk5MDA1IDQ1LjQ1NjIgMC4zMzUzODYgNDUuNTE4MiAwLjM4NTc2MSA0NS41NTc2QzYuNDU4NjYgNTAuMDE3NCAxMi4zNDEzIDUyLjcyNDkgMTguMTE0NyA1NC41MTk1QzE4LjIwNzEgNTQuNTQ3NyAxOC4zMDUgNTQuNTEzOSAxOC4zNjM4IDU0LjQzNzhDMTkuNzI5NSA1Mi41NzI4IDIwLjk0NjkgNTAuNjA2MyAyMS45OTA3IDQ4LjUzODNDMjIuMDUyMyA0OC40MTcyIDIxLjk5MzUgNDguMjczNSAyMS44Njc2IDQ4LjIyNTZDMTkuOTM2NiA0Ny40OTMxIDE4LjA5NzkgNDYuNiAxNi4zMjkyIDQ1LjU4NThDMTYuMTg5MyA0NS41MDQxIDE2LjE3ODEgNDUuMzA0IDE2LjMwNjggNDUuMjA4MkMxNi42NzkgNDQuOTI5MyAxNy4wNTEzIDQ0LjYzOTEgMTcuNDA2NyA0NC4zNDYxQzE3LjQ3MSA0NC4yOTI2IDE3LjU2MDYgNDQuMjgxMyAxNy42MzYyIDQ0LjMxNTFDMjkuMjU1OCA0OS42MjAyIDQxLjgzNTQgNDkuNjIwMiA1My4zMTc5IDQ0LjMxNTFDNTMuMzkzNSA0NC4yNzg1IDUzLjQ4MzEgNDQuMjg5OCA1My41NTAyIDQ0LjM0MzNDNTMuOTA1NyA0NC42MzYzIDU0LjI3NzkgNDQuOTI5MyA1NC42NTI5IDQ1LjIwODJDNTQuNzgxNiA0NS4zMDQgNTQuNzczMiA0NS41MDQxIDU0LjYzMzMgNDUuNTg1OEM1Mi44NjQ2IDQ2LjYxOTcgNTEuMDI1OSA0Ny40OTMxIDQ5LjA5MjEgNDguMjIyOEM0OC45NjYyIDQ4LjI3MDcgNDguOTEwMiA0OC40MTcyIDQ4Ljk3MTggNDguNTM4M0M1MC4wMzggNTAuNjAzNCA1MS4yNTU0IDUyLjU2OTkgNTIuNTk1OSA1NC40MzVDNTIuNjUxOSA1NC41MTM5IDUyLjc1MjYgNTQuNTQ3NyA1Mi44NDUgNTQuNTE5NUM1OC42NDY0IDUyLjcyNDkgNjQuNTI5IDUwLjAxNzQgNzAuNjAxOSA0NS41NTc2QzcwLjY1NTEgNDUuNTE4MiA3MC42ODg3IDQ1LjQ1OSA3MC42OTQzIDQ1LjM5NDJDNzIuMTc0NyAzMC4wNzkxIDY4LjIxNDcgMTYuNzc1NyA2MC4xOTY4IDQuOTgyM0M2MC4xNzcyIDQuOTQyOSA2MC4xNDM3IDQuOTE0NyA2MC4xMDQ1IDQuODk3OFpNMjMuNzI1OSAzNy4zMjUzQzIwLjIyNzYgMzcuMzI1MyAxNy4zNDUxIDM0LjExMzYgMTcuMzQ1MSAzMC4xNjkzQzE3LjM0NTEgMjYuMjI1IDIwLjE3MTcgMjMuMDEzMyAyMy43MjU5IDIzLjAxMzNDMjcuMzA4IDIzLjAxMzMgMzAuMTYyNiAyNi4yNTMyIDMwLjEwNjYgMzAuMTY5M0MzMC4xMDY2IDM0LjExMzYgMjcuMjggMzcuMzI1MyAyMy43MjU5IDM3LjMyNTNaTTQ3LjMxNzggMzcuMzI1M0M0My44MTk2IDM3LjMyNTMgNDAuOTM3MSAzNC4xMTM2IDQwLjkzNzEgMzAuMTY5M0M0MC45MzcxIDI2LjIyNSA0My43NjM2IDIzLjAxMzMgNDcuMzE3OCAyMy4wMTMzQzUwLjkgMjMuMDEzMyA1My43NTQ1IDI2LjI1MzIgNTMuNjk4NiAzMC4xNjkzQzUzLjY5ODYgMzQuMTEzNiA1MC45IDM3LjMyNTMgNDcuMzE3OCAzNy4zMjUzWiIgZmlsbD0iIzcyODlkYSIvPg0KPC9nPg0KPGRlZnM+DQo8Y2xpcFBhdGggaWQ9ImNsaXAwIj4NCjxyZWN0IHdpZHRoPSI3MSIgaGVpZ2h0PSI1NSIgZmlsbD0id2hpdGUiLz4NCjwvY2xpcFBhdGg+DQo8L2RlZnM+DQo8L3N2Zz4NCg==" alt="Chat"/>
    </a>
   <a href="https://github.com/Garlic-Team/powercord-installer/releases/" target="_blank">
    <img src="https://img.shields.io/github/downloads/Garlic-Team/powercord-installer/total?labelColor=242831&color=7289da&style=for-the-badge&logo=data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iNDgiIGhlaWdodD0iNDgiIHZpZXdCb3g9IjAgMCA0OCA0OCIgZmlsbD0ibm9uZSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4gPHBhdGggZD0iTTEyLjI1IDM4LjVIMzUuNzVDMzYuNzE2NSAzOC41IDM3LjUgMzkuMjgzNSAzNy41IDQwLjI1QzM3LjUgNDEuMTY4MiAzNi43OTI5IDQxLjkyMTIgMzUuODkzNSA0MS45OTQyTDM1Ljc1IDQySDEyLjI1QzExLjI4MzUgNDIgMTAuNSA0MS4yMTY1IDEwLjUgNDAuMjVDMTAuNSAzOS4zMzE4IDExLjIwNzEgMzguNTc4OCAxMi4xMDY1IDM4LjUwNThMMTIuMjUgMzguNUgzNS43NUgxMi4yNVpNMjMuNjA2NSA2LjI1NThMMjMuNzUgNi4yNUMyNC42NjgyIDYuMjUgMjUuNDIxMiA2Ljk1NzExIDI1LjQ5NDIgNy44NTY0N0wyNS41IDhWMjkuMzMzTDMwLjI5MzEgMjQuNTQwN0MzMC45NzY1IDIzLjg1NzMgMzIuMDg0NiAyMy44NTczIDMyLjc2OCAyNC41NDA3QzMzLjQ1MTQgMjUuMjI0MiAzMy40NTE0IDI2LjMzMjIgMzIuNzY4IDI3LjAxNTZMMjQuOTg5OCAzNC43OTM4QzI0LjMwNjQgMzUuNDc3MiAyMy4xOTg0IDM1LjQ3NzIgMjIuNTE1IDM0Ljc5MzhMMTQuNzM2OCAyNy4wMTU2QzE0LjA1MzQgMjYuMzMyMiAxNC4wNTM0IDI1LjIyNDIgMTQuNzM2OCAyNC41NDA3QzE1LjQyMDIgMjMuODU3MyAxNi41MjgyIDIzLjg1NzMgMTcuMjExNyAyNC41NDA3TDIyIDI5LjMyOVY4QzIyIDcuMDgxODMgMjIuNzA3MSA2LjMyODgxIDIzLjYwNjUgNi4yNTU4TDIzLjc1IDYuMjVMMjMuNjA2NSA2LjI1NThaIiBmaWxsPSIjNzI4OWRhIi8+IDwvc3ZnPg==" alt="Downloads"/>
  </a>
  <a href="https://github.com/Garlic-Team/powercord-installer/blob/main/LICENSE" target="_blank">
    <img src="https://img.shields.io/github/license/Garlic-Team/powercord-installer?labelColor=242831&color=7289da&style=for-the-badge&logo=data:image/svg+xml;base64,PHN2ZyB3aWR0aD0iMjQiIGhlaWdodD0iMjQiIHZpZXdCb3g9IjAgMCAyNCAyNCIgZmlsbD0ibm9uZSIgeG1sbnM9Imh0dHA6Ly93d3cudzMub3JnLzIwMDAvc3ZnIj4gPHBhdGggZD0iTTEwLjk2ODQgMi4zMjQ2NUMxMS41ODMgMS44NzYxNiAxMi40MTcgMS44NzYxNiAxMy4wMzE2IDIuMzI0NjVMMjAuNDUzNCA3Ljc0MDZDMjEuNDI5OSA4LjQ1MzE1IDIwLjkyNjggOS45OTgzNSAxOS43MTg5IDEwLjAwMDNINC4yODEwOEMzLjA3MzE4IDkuOTk4MzUgMi41NzAxMSA4LjQ1MzE1IDMuNTQ2NTcgNy43NDA2TDEwLjk2ODQgMi4zMjQ2NVpNMTMgNi4yNTAzNEMxMyA1LjY5ODA1IDEyLjU1MjMgNS4yNTAzNCAxMiA1LjI1MDM0QzExLjQ0NzcgNS4yNTAzNCAxMSA1LjY5ODA1IDExIDYuMjUwMzRDMTEgNi44MDI2MiAxMS40NDc3IDcuMjUwMzQgMTIgNy4yNTAzNEMxMi41NTIzIDcuMjUwMzQgMTMgNi44MDI2MiAxMyA2LjI1MDM0WiIgZmlsbD0iIzcyODlkYSIvPiA8cGF0aCBkPSJNMTEuMjUgMTYuMDAwM0g5LjI1VjExLjAwMDNIMTEuMjVWMTYuMDAwM1oiIGZpbGw9IiM3Mjg5ZGEiLz4gPHBhdGggZD0iTTE0Ljc1IDE2LjAwMDNIMTIuNzVWMTEuMDAwM0gxNC43NVYxNi4wMDAzWiIgZmlsbD0iIzcyODlkYSIvPiA8cGF0aCBkPSJNMTguNSAxNi4wMDAzSDE2LjI1VjExLjAwMDNIMTguNVYxNi4wMDAzWiIgZmlsbD0iIzcyODlkYSIvPiA8cGF0aCBkPSJNMTguNzUgMTcuMDAwM0g1LjI1QzQuMDA3MzYgMTcuMDAwMyAzIDE4LjAwNzcgMyAxOS4yNTAzVjE5Ljc1MDNDMyAyMC4xNjQ1IDMuMzM1NzkgMjAuNTAwMyAzLjc1IDIwLjUwMDNIMjAuMjVDMjAuNjY0MiAyMC41MDAzIDIxIDIwLjE2NDUgMjEgMTkuNzUwM1YxOS4yNTAzQzIxIDE4LjAwNzcgMTkuOTkyNiAxNy4wMDAzIDE4Ljc1IDE3LjAwMDNaIiBmaWxsPSIjNzI4OWRhIi8+IDxwYXRoIGQ9Ik03Ljc1IDE2LjAwMDNINS41VjExLjAwMDNINy43NVYxNi4wMDAzWiIgZmlsbD0iIzcyODlkYSIvPiA8L3N2Zz4=" alt="License"/>
  </a>
</p>

---

# Overview

This repository contains the source code for the Powercord installer. This installer is written with [electron-webpack](https://webpack.electron.build/) and [Svelte 3](https://svelte.dev/).

## Downloads

These will link you to the latest builds found in the [releases](https://github.com/Garlic-Team/powercord-installer/releases/) tab of this repository.

| [Windows (7+)](https://github.com/Garlic-Team/powercord-installer/releases/latest/download/Powercord-Windows.exe) | [macOS (10.10+)](https://github.com/Garlic-Team/powercord-installer/releases/latest/download/Powercord-Mac.zip) | [Linux](https://github.com/Garlic-Team/powercord-installer/releases/latest/download/Powercord-Linux.AppImage) |
| ------------------------------------------------------------------------------------------------------------ | ---------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------- |



## Codebase

```
.
├──assets                  // Contains static assets (such as images) used by the installer.
|  └──images               // Images (logos, backgrounds, etc...) used by the installer.
├──scripts                 // Scripts needed for development and contributing.
└──src                     // The installer's source code.
    ├──main                // Electron "main" process. Creates and configures the BrowserWindow.
    └──renderer            // Electron "renderer" process. Contains most components and scripts.
        ├──actions         // Scripts performed by the installer such as installing, repairing and uninstalling.
        |  └──utils        // Common utilities used by installer actions (such as killing discord).
        ├──common          // Common UI components such as buttons, checkboxes, radios, etc...
        ├──pages           // Component files for each page in the installer's setup process.
        ├──stores          // Svelte store used for storing global data.
        |  └──types        // Used for defining custom svelte stores.
        └──transitions     // Contains custom Svelte transitions and animations.
```

---

# Development

> This is a tutorial designed for people looking to contribute to, or work directly with the installer's source code. If you are just looking to download and install Powercord, visit the [releases](https://github.com/Garlic-Team/powercord-installer/releases/) page of this repository.

## Prerequisites
- [Git](https://git-scm.com)
- [Node.js](https://nodejs.org/en/)
- [yarn](https://yarnpkg.com)
- Command line of your choice.

## Building

### 1: Clone the repository.
```bash
git clone https://github.com/Garlic-Team/powercord-installer && cd powercord-installer
```
This will create a local copy of this repository and navigate you to the root folder of the repository.

### 2: Install Dependencies
Run this command at the root folder to install dependencies:
```bash
npm install
```

### 3: Run Build Script
To run the installer in development mode, simply run the following command:
```bash
yarn dev
```

## Additional Scripts

### Linting
This project uses [ESLint](https://eslint.org/). Run this command to lint your changes:
```bash
yarn lint
```

### Compiling & Distribution

```bash
yarn dist
```

---

# Contributors

For information on contributing to this project, please see [CONTRIBUTING.md](/CONTRIBUTING.md).

<a href="https://github.com/Garlic-Team/powercord-installer/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=Garlic-Team/powercord-installer" />
</a>

# Credits

The whole installer is forked from [BetterDiscord](https://github.com/BetterDiscord/Installer) and modified for [Powercord](https://powercord.dev)