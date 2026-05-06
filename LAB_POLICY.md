# Quietly Labs Policy

This repo exists to build public proof without leaking or duplicating the current Quietly.tools product.

## Inclusion rule

Add a project only when it matches at least one of these:

- It is a standalone free tool.
- It is an old prototype or failed experiment.
- It is an open-source engine used by or inspired by Quietly.tools.
- It is a public case study, teardown, or build note.
- It can be safely understood without private context.

## Exclusion rule

Do not add:

- Current source from `quietly.tools/quietly-tools/src/pages`.
- Current source from `quietly.tools/quietly-tools/src/lib`, `src/data`, or production config unless it has been deliberately extracted.
- Anything with credentials, keys, private URLs, customer/client data, or real financial records.
- Private strategy docs from the active Quietly.tools repo.
- Paid-only product logic.

## Current Quietly.tools projects to avoid copying

These were found as active routes in the local Quietly.tools app and should stay out of Labs as source code:

- ClearLedger
- Sheet Doctor
- MindMark
- Desk Reset / Posture Break
- Focus Flow
- Dayfall
- Groundwork
- Life Glance
- Clean Share
- JSON Tidy
- Markdown Editor
- Invoice Generator
- Subscription Audit
- Meeting Agenda Builder
- Weekly Review
- Worry Dump / Unburden
- Quietly Ledger

Labs can link to these tools or discuss sanitized lessons from them, but should not duplicate their active implementation.

## Publishing checklist

Before adding any project:

- Remove `.env`, `.DS_Store`, caches, generated outputs, and local virtual environments.
- Remove `node_modules`, build folders, and package artifacts unless the project needs them as source fixtures.
- Replace client/customer names and assets unless they are public and permitted.
- Add a short README with purpose, status, and run instructions.
- Label the status clearly: `stable`, `prototype`, `deprecated`, `case-study`, or `experiment`.
- Add a link back to https://quietly.tools when relevant.

