# Z Agent Communication SOP

**Last updated:** 2026-09-02 | **Author:** Manus | **Status:** Active

## Purpose

Use the Z Agent Communication skill to make every message to Jack or a human team member clear enough to act on without translation, guesswork, or unnecessary follow-up. The standard prevents missed ownership, vague deliverables, unclear approval gates, and premature task closure.

## Scope and Source of Truth

This SOP applies to ZedBiz agents writing assignments, status updates, corrections, handoffs, approval requests, and completion reports for Jack, Virtual Assistants, contractors, or managers. It does not replace a stricter approved legal, security, client, or platform policy.

The runtime source of truth is [`SKILL.md`](../SKILL.md) in the `ZedBiz44/z-agent-communication-Skill` repository. The deployed copy must match the validated GitHub version. The Notion SOP is the operational record, not a competing runtime copy.

## Required Inputs

Before writing, confirm the recipient, the current situation, the exact work required, the expected deliverable, the destination for that deliverable, the deadline if one exists, the approval or decision owner, and the condition for marking the main task done.

If any material input is unknown, state what is unknown and who must decide it. Do not guess.

## Procedure

### Choose the right message size

Use the full assignment format for a new or reopened assignment, several related actions, a problem affecting work, a proof or approval request, a deadline, or a stop condition. Use the short format for a simple correction, reminder, single missing item, wait instruction, or one decision. Use the status-only format when the recipient only needs to know what can continue, what must wait, and who decides next.

### Write for one person

Address one person per comment and name the person responsible for every action, recommendation, approval, or decision. Mention another person only when their work changes what the recipient must do. Put unrelated work in another comment.

### Make the work executable

Use everyday words and short complete sentences at roughly a Grade 8 reading level. Explain an unfamiliar technical term the first time it appears. State the exact file, link, screenshot, list, test, or result the recipient must send back and exactly where it must be uploaded or posted.

State why the work matters when that will help the recipient make a good decision. Clearly state what can happen now, what must wait, what must not happen, who gives the next approval, and when the main task can be marked done.

### State stop conditions

If payment, publication, production changes, legal rights, credentials, or a new material problem is involved, name the decision maker and tell the recipient to stop before taking the affected action. Do not use vague phrases such as “escalate if necessary” or “wait for approval.”

### Check before sending

Use the skill’s before-sending self-check. Rewrite the message if a new team member could reasonably ask what main task is being discussed, who needs to act, what proof is needed, where it belongs, whether work can continue, or who decides next.

### Learn from a correction

When Jack or a team member points out confusing language, correct the message promptly, identify the unclear wording, add a better everyday-language replacement to the skill when it is reusable, and use the clearer wording from then on.

## Responsibilities

| Role | Responsibility |
|---|---|
| Agent writing the message | Apply the skill, confirm all required details, complete the self-check, and correct reusable language problems. |
| Recipient | Complete only the clearly assigned work, return the requested deliverable to the stated location, and raise a specific gap if an instruction remains unclear. |
| Decision owner | Make the named approval, spending, publication, or priority decision. |
| Jack | Approve decisions that the message assigns to him and provide missing authority when needed. |

## Verification and Completion Record

A message passes when its intended recipient can identify the situation, their exact action, the required return item, its location, the deadline or lack of one, what can continue, what must wait, the next decision maker, and the main-task completion condition.

For a rollout, save the validated `SKILL.md` in the GitHub repository, update the target agent’s `AGENTS.md` and `SOUL.md`, create a dated backup before the live edit, and record the file paths, validation result, representative message test, status, and any exception in the associated GitHub issue and daily Technical Journal.

## Failure Handling

If the required skill is missing, malformed, out of date, or unavailable in the target runtime, stop before claiming compliance. Restore the last known-good deployed copy, document the observed problem and attempted fix, and escalate to Jack or the responsible manager for the smallest needed decision. Do not replace or delete unrelated agent instructions.
