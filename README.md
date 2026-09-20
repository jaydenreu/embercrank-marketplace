# Embercrank

Embercrank is a local connector for managed coding-task routing. It works with a supported Codex or Claude Code installation while provider credentials and coding execution stay on the customer machine. An Embercrank account and active trial or subscription are required; installing this connector does not grant paid access.

## Install from this release

This repository is released with immutable Git tags. Replace no part of the commands below; the tag is the reviewed connector version.

### Codex

```text
codex plugin marketplace add jaydenreu/embercrank-marketplace --ref v0.1.0-beta.11
codex plugin add embercrank@embercrank --json
```

Start a new Codex session after installation, then ask Embercrank to check its connection and provider availability before starting work.

### Claude Code

```text
claude plugin marketplace add jaydenreu/embercrank-marketplace@v0.1.0-beta.11
claude plugin install embercrank@embercrank
```

Restart Claude Code after installation, then invoke `/embercrank:route` and ask it to check the connection and provider availability before starting work.

## Connect and authorize

The connector guides device activation through Embercrank's website. Approve only the code shown by your own command. Provider login remains in the official Codex or Claude Code tool. Never paste a provider credential, card number, email code, or Embercrank token into chat.

Project access is explicit and bounded. Authorize only the Git project you intend to use. Embercrank cannot intercept work outside an Embercrank-managed job.

## Verify the release

`release.json` identifies the reviewed version and every distributable file. `checksums.sha256` contains SHA-256 hashes for those files and the release manifest. A Git tag alone does not replace checksum verification.

The published repository contains the inspectable local connector, host manifests, setup documentation and notices. It does not contain Embercrank's server routing policy, database migrations, provider credentials, customer credentials or payment secrets.

## Requirements and support

- Node.js 22.13 or newer.
- Git.
- A supported, separately authenticated Codex or Claude Code installation.
- An Embercrank account with an active entitlement.

Security reports: see [SECURITY.md](SECURITY.md).  
Support: contact@embercrank.com  
Website: https://embercrank.com

