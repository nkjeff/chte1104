# chte1104 — Minimal Messenger

An unofficial, minimal Android Telegram client project for realme Neo8 / ColorOS 17.

## Build strategy

- Upstream Android client: [TelegramOrg/Telegram-Android](https://github.com/TelegramOrg/Telegram-Android)
- Upstream revision pinned for the initial build: `3de37c8cfb039452be7398909461da6288babf15`
- Source is fetched with Git submodules by GitHub Actions; the full upstream source is not duplicated in this repository.
- Build runs on GitHub-hosted Linux using the upstream Dockerfile and uploads generated APKs as workflow artifacts.

## Current status

The first workflow is a **baseline build only**. It verifies that the upstream source can be fetched and compiled in CI. The minimal UI and feature removals have not yet been applied.

The upstream repository currently includes placeholder/reproducible-build configuration. Before a usable public client release, configure your own Telegram API ID and API hash from [my.telegram.org](https://my.telegram.org), review push-notification configuration, and replace signing credentials. Never commit private signing keys or passwords.

## Start a build

Open **Actions → Build Android APK → Run workflow**. When it finishes, open the successful run and download the `chte1104-apk` artifact.

## License and attribution

The upstream Telegram Android project is GPL-2.0-or-later. This project must preserve applicable copyright and license notices and publish the corresponding source for distributed modified binaries. See the upstream [LICENSE](https://github.com/TelegramOrg/Telegram-Android/blob/master/LICENSE) and [README/build instructions](https://github.com/TelegramOrg/Telegram-Android#compilation-guide).

This is an unofficial third-party client and is not endorsed by Telegram.
