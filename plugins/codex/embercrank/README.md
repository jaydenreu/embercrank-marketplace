# Embercrank connector

This package is the local Embercrank connector for Codex. It contains host integration, protocol validation and bounded local execution protections. The managed routing policy, model catalogue, entitlement logic and learning policy remain on Embercrank's service.

Requirements: Node.js 22.13 or newer, Git, an active Embercrank entitlement, and a separately installed and authenticated official coding provider.

Run `node cli.mjs --help` to inspect local commands. Device activation uses `node cli.mjs activate`; approve only the code shown by your own command. `node cli.mjs doctor --json` checks supported provider discovery without model inference. Provider credentials remain with the official provider tool and must never be pasted into chat or stored in this folder.

Before project tools can run, the host MCP process needs `EMBERCRANK_ALLOWED_ROOTS` as a JSON array of approved absolute Git project roots. Missing roots deny project operations. Do not authorize an entire home folder. Normal host permission prompts and Embercrank execution checks still apply.

Installing the connector does not start or grant a subscription. A routing recommendation does not prove provider execution, validation or savings. Embercrank reports those states separately and cannot intercept unrelated host actions outside Embercrank-managed jobs.

Use is governed by the included `LICENSE.md` and Embercrank's Terms of Service.

Support: contact@embercrank.com
