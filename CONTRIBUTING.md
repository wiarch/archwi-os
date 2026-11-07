# Contributing to ArchWi

ArchWi is an early-stage Arch Linux-based operating system project. Contributions should favor upstream compatibility, reproducibility, security, and maintainability.

## Before contributing

- Read the README, product definition, architecture, roadmap, and security policy.
- Check whether a proposed feature is in scope for the current milestone.
- Prefer official Arch packages and established tooling.
- Discuss major architecture or installer decisions before implementing them.

## Pull requests

- Keep changes focused and explain the motivation.
- Include tests or validation steps for scripts and build profiles.
- Document commands actually executed and their results.
- Never commit secrets, private keys, credentials, or generated ISO files.
- Preserve upstream license and attribution notices.
- Do not weaken signature or TLS verification to bypass failures.

## Status accuracy

Mark features as implemented only when the code is present and validated. Clearly label experimental and planned functionality.
