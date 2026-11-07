# Security Policy

## Status

ArchWi OS is currently a documentation-only project. There is no installable image or installer in this repository. This policy describes requirements for future implementation.

## Security objectives

- Preserve Arch package signature verification.
- Prefer official repositories and trusted upstream sources.
- Minimize privileged code and avoid unnecessary root daemons.
- Validate all external inputs, downloads, checksums, and configuration.
- Make partitioning, formatting, bootloader changes, encryption, and other destructive operations explicit.
- Avoid storing secrets in source code, build logs, ISO metadata, or command-line arguments.
- Provide auditable build definitions and release provenance.

## ISO and supply-chain requirements

- Generate images from version-controlled profiles and scripts.
- Record build environment, package versions, and source revisions.
- Publish cryptographic checksums; sign release metadata and artifacts when release infrastructure is established.
- Protect CI credentials with least privilege.
- Pin third-party CI actions to immutable commit SHAs where practical.
- Do not publish experimental images as stable releases.

## Installer requirements

- Clearly identify target disks and planned changes before execution.
- Require explicit confirmation for destructive actions.
- Support encryption through established, reviewed Linux tooling.
- Never silently weaken Secure Boot, package signature, or TLS verification.
- Handle failures without leaving disks in an ambiguous partially modified state where feasible.

## Reporting

Until a dedicated security contact is published, report vulnerabilities privately to the repository maintainers rather than posting exploitable details publicly. Do not include secrets or personal data in reports.
