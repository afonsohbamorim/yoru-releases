# Yoru

Yoru is a personal, self-hosted companion for anime, TV series, and films. Your Windows PC hosts the library, downloads, and playback services. Use the Windows app or pair another device on your home network.

## Download and install

Open the [latest release](https://github.com/afonsohbamorim/yoru-releases/releases/latest) and download **Yoru-Setup-&lt;version&gt;.exe**. Run Setup, choose **Instalar**, and follow the initial storage and playback setup. Internet access is required to prepare the pinned components on first launch.

To upgrade an existing installation, keep its installation and data folders. Uninstalling first is unnecessary. For versions older than the 1.10 update manager, use the latest Setup to upgrade the recovery and startup components as well.

The ZIP is the update payload. `latest.json`, `SHA256SUMS.txt`, and `package-inventory.json` support signature and file verification. Releases do not contain the author's accounts, credentials, databases, or media.

## Use your collection

- **Descobrir**: search and explore catalogues. Saving a title, marking it watched, and giving it a rating are tracking actions.
- **Biblioteca**: manage followed titles and continue from confirmed playable items.
- **Downloads**: explicitly request a movie or episodes, confirm quality and audio requirements, and follow the actual transfer and import state. A movie can be downloaded without adding it to the tracking library.
- **Disponíveis**: browse confirmed local files, resume playback, and select audio or subtitles. File cleanup previews the exact selected files and preserves tracking and watched history.

The interface is currently Portuguese (Portugal); this guide uses its real menu labels. Yoru preserves the configured audio requirements and keeps a 50 GiB reserve on each media disk. An undeclared language is not confirmed English. Availability and transfer speed depend on the selected sources and peers.

## TV and Mac

For a TV, install a compatible Jellyfin client and use the server address shown in **Definições → Dispositivos**. Use the prepared playback profile or Quick Connect when the client supports it. Client availability depends on the TV model and store.

For a Mac, enable browser access on the PC, generate a pairing code, and open the displayed **Yoru** address in Safari. Do not install another media server on the Mac. `localhost` on the Mac refers to the Mac itself, so use the PC's address.

The PC, Yoru, and the relevant services must remain running, with both devices on the same home network. A native Mac companion is a separate delivery; do not assume a Windows release includes a Mac DMG. Actual device and format testing is still needed for playback, subtitle rendering, and HDR.

## Accounts, updates, and removal

Connect AniList if you want anime tracking integration. Approved pending updates are preserved for reconciliation after temporary failures; a connected account alone does not prove that an external history update succeeded.

Yoru registers in Windows Installed Apps and Control Panel. Closing the window leaves the tray service running; use the tray exit action to stop it. Startup with Windows is optional. Uninstalling preserves application data and videos by default; review any optional removal scope before confirming.

Updates use Ed25519 signatures and file hashes. The installer does not currently have an Authenticode certificate, so Windows may show an unknown-publisher warning. Packaged service components remain pinned until an explicitly supported component update is provided.

The source repository is private. This repository publishes installers, verified update payloads, and English release notes. Historical release notes describe their specific version and its validation limits.
