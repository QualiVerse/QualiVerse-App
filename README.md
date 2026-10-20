# QualiVerse App

**[Download QualiVerse.Te.V2 for Windows](https://github.com/QualiVerse/QualiVerse-App/releases/latest/download/QualiVerse.Te.V2.exe)**

**[Download QualiVerse.Te.V2 for macOS](https://github.com/QualiVerse/QualiVerse-App/releases/latest/download/QualiVerse.Te.V2-macOS.zip)**

[View all releases](https://github.com/QualiVerse/QualiVerse-App/releases)

The frontend repository's GitHub Actions workflow builds Windows and macOS releases and publishes each app with its SHA-256 checksum as Release assets. Installed versions check the latest public Release, download the matching platform asset, and verify its checksum before updating.

`version.json` and `appcast.xml` remain in this repository for Windows update metadata and are refreshed by the publishing workflow. App binaries are stored only in Releases.

The frontend workflow needs an `UPDATE_REPO_TOKEN` secret with Contents: Read and write permission for this repository.
