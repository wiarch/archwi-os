# ArchWi

**ArchWi** is the WI Arch initiative to build an Arch Linux-based operating system and distribution.

> Project status: **concept and documentation foundation**. This repository currently does not contain an installable operating system, ISO image, installer, package repository, or maintained system configuration.

## Vision

Create a polished, reproducible, maintainable Arch Linux-based desktop operating system with a distinct WI identity. The initial direction is a KDE Plasma desktop, with sensible defaults and a carefully curated set of system tools.

## Product principles

- **Arch-based:** build on Arch Linux and its rolling-release ecosystem.
- **Reproducible:** version the configuration and automate image generation.
- **Transparent:** document upstream components, licenses, changes, and known limitations.
- **Secure by default:** minimize privileged components, validate inputs, and provide safe update practices.
- **Maintainable:** keep custom patches small and track upstream changes.
- **User-controlled:** make installation, disk operations, encryption, and destructive actions explicit.

## Initial direction

- Base system: Arch Linux.
- Desktop environment: KDE Plasma (proposed default).
- Delivery: bootable ISO generated through a documented, automated build pipeline.
- Installer: evaluate a supported installer or develop a dedicated workflow after validating requirements.
- Branding: WI wallpapers, themes, icons, artwork, and coherent defaults.
- System tooling: curated setup, update, recovery, and maintenance utilities.

These are product decisions and targets, not claims that the features already exist.

## Repository status

This repository is currently a documentation-only starting point. Implementation, build scripts, installer, package definitions, and release artifacts are not yet present.

See:
- [Product definition](docs/PRODUCT.md)
- [Architecture](docs/ARCHITECTURE.md)
- [Roadmap](docs/ROADMAP.md)
- [Security policy](docs/SECURITY.md)
- [Contribution guide](CONTRIBUTING.md)
- [Claude instructions](CLAUDE.md)
- [Implementation prompt](PROMPT.md)

## Development

No build or installation commands are available yet. Do not use this repository as instructions for installing or replacing an operating system.

## License

A project license has not yet been selected. ArchWi must preserve all applicable Arch Linux trademarks, upstream licenses, notices, and attribution. Do not imply that Arch Linux endorses or maintains ArchWi.
