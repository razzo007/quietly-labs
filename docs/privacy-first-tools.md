# Privacy-First Tools

Privacy-first tools collect less, explain more, and avoid turning small tasks into accounts.

## Default Posture

- Process locally when possible.
- Use mock data in demos.
- Avoid accounts, databases, analytics, and cloud storage in Labs examples.
- Keep imports and exports explicit.
- Do not store personal content unless the demo clearly says where and why.
- Prefer `localStorage` only for toy examples.
- Give users a clear way to clear local data.

## Data Rules

Never commit:

- Real user content.
- Notes, memoirs, emails, names, photos, places, or coordinates.
- Financial records.
- API keys or tokens.
- `.env` files.
- Production URLs or private backend endpoints.

Use placeholders and mock fixtures:

- `mock-user`
- `sample-note`
- `sample-memory`
- `https://example.com`
- `YOUR_API_KEY_HERE`

## BYO-AI Rules

BYO-AI demos should:

- Ask the user for their own provider key locally.
- Avoid shipping a default production key.
- Explain that content may be sent to the user's chosen provider.
- Link users to their provider's privacy and data-retention policies.
- Use mock examples by default.

## Finance And GST Rules

GST and finance utilities in this repo are helpers, not professional advice.

They should:

- Show assumptions.
- Preserve originals where possible.
- Flag uncertain rows.
- Avoid silent deletion.
- Encourage review by a qualified professional for important filings.

