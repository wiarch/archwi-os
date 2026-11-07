# Roadmap

This roadmap is aspirational. No milestone below should be considered implemented until code, tests, and release evidence exist.

## Phase 0 — Foundation
- [x] Establish repository purpose and product documentation.
- [ ] Select project license after reviewing included assets and upstream obligations.
- [ ] Define supported architectures and initial hardware/VM matrix.
- [ ] Decide naming, visual identity, and trademark review.

## Phase 1 — Minimal bootable image
- [ ] Create an Archiso profile.
- [ ] Define minimal package sets and boot configuration.
- [ ] Build an ISO in CI or a documented clean environment.
- [ ] Verify ISO integrity and boot it in UEFI virtual machines.
- [ ] Publish checksums and build metadata for test artifacts.

## Phase 2 — Desktop experience
- [ ] Add KDE Plasma profile and display manager.
- [ ] Apply WI branding and accessible defaults.
- [ ] Curate a small default application set.
- [ ] Document package selection and customization.

## Phase 3 — Installation
- [ ] Evaluate installer options and maintenance risk.
- [ ] Define partitioning, encryption, bootloader, and recovery requirements.
- [ ] Test installation and failure recovery in virtual machines.
- [ ] Publish installation documentation only after end-to-end validation.

## Phase 4 — Maintenance and releases
- [ ] Establish update and rollback guidance appropriate to a rolling release.
- [ ] Automate build, smoke tests, checksums, and release notes.
- [ ] Define security advisories and release support policy.
- [ ] Establish a process for tracking upstream Arch changes.

## Phase 5 — Wider hardware support
- [ ] Expand testing to physical hardware.
- [ ] Document GPU, Wi-Fi, Bluetooth, audio, and power-management coverage.
- [ ] Evaluate accessibility and localization improvements.
