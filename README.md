# Elmiral – Releases

Installer and update files for **Elmiral**, a 2D pixel-art fantasy action RPG for Windows (in development, not released).
This repository holds only the installer, the launcher and the game files; the game's source code is not here.

- Installer: `Elmiral-0.19.1-Setup.exe` – installs the **Elmiral Launcher** and the game. Afterwards the launcher shows
  the patch notes and keeps the game up to date: press UPDATE (only changed files are downloaded), then PLAY.
- `launcher.json` is what the launcher reads; the files it downloads live in `game/<version>/` and `launcher/<version>/`
  (gzip-packed, checked with SHA-256). `patch_notes.json` holds the notes shown in the launcher.
- `latest.json` is only for game versions up to 0.19.0: their built-in updater installs 0.19.1, which brings the launcher.
- Installing or updating keeps your characters and settings (they live in `%APPDATA%\Elmiral`).
- Launcher, game and installer are not code-signed; Windows SmartScreen may show a warning.
