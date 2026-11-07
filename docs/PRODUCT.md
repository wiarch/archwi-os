# ArchWi OS — Product Definition

## Summary

ArchWi OS is the WI Arch initiative to create an Arch Linux-based operating system. Its goal is to provide a coherent desktop experience without hiding the flexibility and transparency of its upstream foundation.

## Problem

A raw Arch Linux installation gives users significant control but requires them to make many decisions about installation, desktop configuration, applications, drivers, maintenance, and recovery. ArchWi OS aims to offer a curated and repeatable starting point while keeping system behavior understandable.

## Target users

- Linux users who want an Arch-based desktop with sensible defaults.
- Developers who value a configurable, current Linux environment.
- Users who want a consistent WI-branded workstation experience.

## Initial product direction

- Arch Linux as upstream base.
- KDE Plasma as the proposed default desktop.
- Curated defaults, applications, themes, fonts, icons, and wallpapers.
- Reproducible ISO build process.
- Documented installation and recovery flows.
- Clear update, package, and maintenance guidance.

## Non-goals for the first milestone

- Claiming compatibility with every device or hardware configuration.
- Replacing Arch Linux upstream repositories or governance.
- Building a custom package ecosystem before it is needed.
- Shipping automatic destructive disk operations without explicit user consent.
- Promising a zero-maintenance rolling-release experience.

## Product principles

1. Upstream-first: prefer official Arch packages and established tools.
2. Reproducibility: build artifacts from versioned definitions.
3. Security: least privilege, signed artifacts where feasible, and transparent update paths.
4. User agency: disclose disk, bootloader, encryption, and partitioning choices.
5. Accessibility: provide readable defaults and keyboard-operable workflows.
6. Honest status: distinguish implemented, experimental, planned, and unsupported features.

## Success criteria

- A clean, documented build can produce the same class of ISO from versioned inputs.
- Installation succeeds in a defined and tested hardware/virtual-machine matrix.
- Updates and recovery have documented, testable procedures.
- Customizations are traceable and do not unnecessarily fork upstream components.
