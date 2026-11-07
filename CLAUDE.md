# Claude Code Instructions — ArchWi OS

## Project context

ArchWi OS is a planned Arch Linux-based operating system under WI Arch. The repository currently contains documentation only. Do not assume an ISO, installer, package profile, or system utility exists.

## Working rules

1. Inspect the repository and current upstream Arch documentation before proposing implementation.
2. Prefer official Arch tooling and packages. Evaluate Archiso before designing a custom image builder.
3. Keep changes modular, reproducible, documented, and easy to audit.
4. Do not claim a feature is implemented unless its code and tests exist.
5. Never disable pacman signature verification, TLS verification, or security controls to make a build pass.
6. Treat installer and disk-management work as security-critical. Require explicit user consent for destructive operations.
7. Do not embed credentials, signing keys, private keys, or tokens in the repository or generated images.
8. Preserve upstream license notices and trademark requirements.
9. Add tests and CI checks for scripts and build definitions as they are introduced.
10. Update README, architecture, security, and roadmap documents when implementation decisions change.

## Engineering expectations

- Shell scripts: use strict error handling where appropriate, quote variables, validate arguments, and avoid unsafe evaluation.
- Downloads: verify source, checksum, and signature when available.
- Privileged operations: minimize scope and explain why elevation is required.
- Build outputs: record versions and provide checksums.
- Documentation: distinguish supported, experimental, planned, and unsupported behavior.

## Before completing a task

Report files changed, commands/tests actually executed, results, unresolved risks, and any manual steps. Never report a build as successful unless it was run and verified.
