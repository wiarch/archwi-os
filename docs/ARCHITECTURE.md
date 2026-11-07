# Architecture

## Current state

There is no implementation in this repository yet. This document describes a proposed architecture, not existing components.

## Proposed layers

1. **Upstream base:** Arch Linux packages, kernel, systemd, pacman, and official repositories.
2. **Image composition:** versioned profile and package selection, filesystem layout, boot configuration, and ISO assembly.
3. **Desktop experience:** KDE Plasma defaults, display/login configuration, themes, icons, fonts, wallpapers, and selected applications.
4. **Installation:** a validated installer workflow or an established upstream installer configured for ArchWi OS.
5. **System utilities:** optional tools for first-run setup, maintenance, diagnostics, and recovery.
6. **Release engineering:** automated builds, artifact checksums, signatures, release notes, and reproducible build metadata.

## Build strategy

Evaluate Archiso as the initial ISO-generation foundation before introducing custom build infrastructure. Keep profile configuration, package lists, overlays, and scripts in version control. Pin or record relevant toolchain and package snapshot information where practical.

## Installer strategy

Prefer a mature installer with a clear maintenance and security model if it meets product requirements. A custom installer should be considered only after requirements, threat model, supported partition layouts, encryption behavior, boot modes, and recovery paths are specified.

## Update model

Use pacman and upstream Arch repositories by default. Any ArchWi OS-specific repository must have a documented signing model, package ownership, build provenance, mirror strategy, and incident response process. Never instruct users to disable package signature verification as a workaround.

## Compatibility

Define and test a support matrix before making hardware compatibility claims. At minimum, test UEFI virtual machines and document BIOS/legacy boot support separately if pursued.

## Design constraints

- Keep privileged operations small and auditable.
- Avoid shell commands assembled from untrusted input.
- Validate downloaded artifacts and configuration.
- Make destructive storage operations explicit and reviewable.
- Preserve upstream licenses, notices, and trademarks.
