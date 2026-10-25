<div align="center">

# maxOS tools

**Seven small Mac tools. One app to run them all.**

Menu bar utilities that each do one job well, managed from a single place,
built natively for macOS 26 with Liquid Glass.

[**⬇ Download the latest DMG**](https://github.com/SnapNext-GmbH/maxOS-tools-releases/releases/latest)

Signed with Developer ID · Notarized by Apple · Apple Silicon · macOS 26+

</div>

---

## Why

Most Mac utilities come with their own settings window, their own updater and their own permission dance. maxOS tools turn that around:

- **Small and separate.** Each tool is its own app with its own menu bar icon. A crash or a missing permission in one never touches another.
- **One control room.** **maxOS Control** shows what is installed and running, holds every tool's settings, and tells you which macOS permission is missing and where to grant it.
- **One download.** A single DMG carries every tool. Control installs them and keeps them current.

## The tools

| Tool | What it does |
|---|---|
| **CalBar** | Next meeting countdown, calendar and reminders in the menu bar |
| **DeskPin** | Puts every window back where it was for your display setup |
| **AgeTint** | Colors files and folders by age, so new downloads stand out |
| **Toggles** | Put your Mac into the right mode for the moment, and back |
| **Panes** | Tabbed, split-pane file browser with instant search and previews |
| **Tempo** | See where your Mac time goes, by app, site and window |
| **Depot** | Browse what Homebrew, npm, pipx and cargo installed |

## maxOS Control

The one app you open occasionally: after install, when something looks wrong, or to change a setting.

- See at a glance which tools are installed, running and healthy
- Launch, quit and set launch at login per tool
- Change any setting without hunting through a tool's own menu
- See which permission a tool still needs, and jump straight to it
- Update everything with one button when a new version is out

Control only shows a tool as healthy when the tool reports it itself. If it does not know, it says so.

## Install

1. Download `maxOS-tools-<version>.dmg` from the [latest release](https://github.com/SnapNext-GmbH/maxOS-tools-releases/releases/latest).
2. Open it and drag **maxOS Control** onto **Applications**.
3. Open **maxOS Control** from Applications and install the tools you want.
4. macOS asks for permissions the first time a tool needs them (Accessibility, Files and Folders, Automation). Grant each once.

Control has to live directly in `/Applications`, otherwise it cannot install tools or update itself.

## Updates

Control checks for a new version after launch and then once a day. Nothing installs on its own: you click **Update**.

Before anything is replaced, Control verifies the download:

- HTTPS only
- SHA-256 matches the value in `latest.json`
- Developer ID signature is valid and the Team ID is `N9NHR797R5`
- Only strictly newer versions are installed, never a downgrade

If any check fails, the current version keeps running.

## Requirements

- macOS 26 (Tahoe) or later
- Apple Silicon

## About this repository

This repository holds release assets only: the DMG and `latest.json`. There is no source code here.

Built by SnapNext.
