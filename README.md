# Z Agent Communication Skill

This repository is the technical source of truth for **z-agent-communication**, the ZedBiz standard for clear, plain-language communication with Jack and human team members.

## Purpose

Use this skill when an agent needs to write an assignment, status update, correction, handoff, approval request, or completion report for a human. It ensures the message clearly states ownership, the exact work required, the requested deliverable, location, deadline, approval gate, and definition of done.

## When to Use

Use the skill for human-facing project communication, including messages to Jack, Virtual Assistants, contractors, or managers. It is especially important when a message assigns work, reopens work, requests proof, sets a deadline, requires approval, or tells someone what must wait.

Do not use it for machine-to-machine payloads, source code comments, private memory notes, or messages where this standard has already been explicitly superseded by a stricter approved policy.

## Authoritative Runtime Guide

[`SKILL.md`](./SKILL.md) is the concise runtime instruction set for all agents, including task and subtask descriptions. [Additional examples](references/examples.md) contain terminology guidance and longer handoffs; load them only when needed.

## Runtime Files and Deployment

| Item | Purpose |
|---|---|
| `SKILL.md` | Runtime communication standard for agents. |
| `docs/z-agent-communication-SOP.md` | Business-facing SOP source used to create and maintain the Notion record. |
| Amanda `workspace/AGENTS.md` | Always-loaded rule requiring Amanda to use the skill for human communication. |
| Amanda `workspace/SOUL.md` | Short personality statement that reinforces the desired communication style. |

Deploy the validated runtime package containing `SKILL.md`, `agents/`, and `references/` to the target agent's active skill directory. Record the prior GitHub commit for recovery; do not create discoverable backup skills. Verify ownership and permissions, refresh only if required, and test one representative human-facing message. The September 24 revision does not change AGENTS.md or SOUL.md.

## Validation

Run the validator bundled with the Z AI Skill Developer repository:

```bash
python3 /home/ubuntu/z-ai-skill-developer-Skill/scripts/validate_skill.py --repository /home/ubuntu/z-agent-communication-Skill
```

Also confirm that every file named in this README exists and that the live target loads the skill. Use one normal human-facing assignment message as the happy-path test before declaring the rollout complete.

## Safety and Approval Boundaries

This skill governs language, not authority. It does not authorize spending, publishing, production changes, credential changes, legal commitments, or client-facing actions. Messages must clearly state the appropriate decision maker and stop instruction when approval is required. Never include secrets, private credentials, or sensitive client information in the skill, the repository, or human-facing messages.

## Maintenance

Keep the runtime standard concise enough to load reliably and update it only when a communication problem has been confirmed. Record revisions in the associated GitHub issue and the Notion Technical Journal. The detailed operational SOP belongs in Notion, while GitHub remains the source of truth for the technical skill and deployment files.
