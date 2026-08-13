# Initial LLM Prompt

Command manifest entrypoint:
- MANDATORY FIRST READ: docs/reference/agentic-kit-commands.json (manifest_sha: 4a6368de864c). Every reply containing commands MUST start with: COMMAND_MANIFEST_ACK 4a6368de864c. Consult `agentic-kit command-for` before proposing commands and choose the most specific available Kit workflow command.
- Before proposing ANY command run/consult `agentic-kit command-for` and choose the most specific available Kit workflow command.
- raw git/gh commands with a mapped wrapper are rejected by instruction lint.

Command reference contract:
- Read `docs/reference/agentic-kit-commands.json` before composing agentic-kit commands.
- Read `docs/reference/AGENTIC_KIT_COMMANDS.md` before composing agentic-kit commands.
- `must_not_reconstruct_commands_from_memory: true`.
- Treat `source_hashes` as freshness evidence.
source_hashes:
- docs/reference/AGENTIC_KIT_COMMANDS.md: 0200ba8c7dc99792004a14dd522129f50eba4abcac4f411b38ad856db905a23c
- docs/reference/agentic-kit-commands.json: f1af5c2d038a7bf6ad6c55ede61bec1b7a8347173ffa46f3f599ac96127aada7

You are working in repository `sampleproject`.

Before mutating anything:
1. Inspect the repository root and current branch.
2. Read `.agentic/config.yaml`.
3. Treat `.agentic/transfer/inbox/` as the workspace transfer inbox carrier.
4. Run or request `agentic-kit standard-gates-audit-suite` before claiming completion.

Default branch: `main`
Project type: `python`
Profile: `python-default`

Private/public boundary: no secrets, credentials, private chat fragments, or
personal logs belong in any versioned part of `.agentic/`. Machine-local state
lives under `.agentic/tmp/` and is ignored by construction.
