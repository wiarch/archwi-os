# ArchWi — Project Implementation Brief

You are working in the ArchWi repository, a planned Arch Linux-based operating system under WI Arch.

## Current baseline

The repository currently contains only a minimal README. There is no working OS image, Archiso profile, installer, package repository, or implementation. Treat this as a greenfield project.

## Product direction

Build a polished, maintainable Arch-based desktop distribution. KDE Plasma is the proposed default desktop. The system should have WI branding, a curated package selection, reproducible ISO generation, clear installation and maintenance guidance, and secure defaults.

## Recommended first milestone

Deliver a minimal, reproducible, bootable Archiso image before implementing a custom installer or adding large numbers of applications.

1. Research current official Arch Linux and Archiso documentation.
2. Propose a minimal profile structure and explain each file.
3. Define supported architecture and UEFI test environment.
4. Create a minimal package set and boot configuration using supported Archiso conventions.
5. Add a build script that validates prerequisites, builds in a clean environment, and fails safely.
6. Add automated checks for shell scripts and profile consistency.
7. Document how to build and test the ISO in a disposable virtual machine.
8. Record known limitations and update the roadmap.

## Constraints

- Do not claim ArchWi is production-ready.
- Do not build a custom installer in the first milestone.
- Do not disable package signature checks or TLS verification.
- Do not add unreviewed third-party repositories.
- Do not automate disk formatting or installation.
- Do not include credentials, signing keys, or secrets.
- Preserve Arch Linux license notices and trademark requirements.
- Prefer small, reviewable changes over speculative frameworks.

## Expected deliverables

A proposed implementation plan first, followed by a tested minimal Archiso profile and build pipeline. Include exact commands and actual test results. Ask for clarification only when a decision materially affects safety or architecture.
