# QualiVerse App

**[Download QualiVerse.Te.V2 for Windows](https://github.com/QualiVerse/QualiVerse-App/releases/latest/download/QualiVerse.Te.V2.exe)**

[View all releases](https://github.com/QualiVerse/QualiVerse-App/releases)

The frontend repository's GitHub Actions workflow builds each Windows update and publishes the installer and its SHA-256 checksum as Release assets. Installed versions check the latest public Release and verify the checksum before installing an update.

`version.json` and `appcast.xml` remain in this repository for update metadata and are refreshed by the publishing workflow. Installer binaries are stored only in Releases.

The frontend workflow needs an `UPDATE_REPO_TOKEN` secret with Contents: Read and write permission for this repository.
