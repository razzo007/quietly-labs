# Public Repo Boundaries

This repository is public. It contains experiments, generic demos, and learning materials.

It must never contain production Quietly Tools source code, user data, private backend logic, analytics, payments, auth flows, premium brand assets, or sensitive product internals.

## Repo Identity

Quietly Labs is:

> A public lab of small experiments, demos, retired prototypes, and reusable patterns.

Quietly Labs is not:

> The Quietly Tools product codebase.

## Never Include

- Full Quietly Tools application source code.
- MindMark production code.
- Memoir production code.
- Production share-link implementation.
- Production auth logic.
- Payment, donation, subscription, or monetization logic.
- Analytics or tracking logic.
- Production database schemas.
- Production backend functions.
- API keys, tokens, secrets, `.env` files, or private configuration.
- Production URLs unless they are public marketing links.
- User-generated content.
- Real notes, memoirs, names, emails, photos, places, or coordinates.
- Premium Quietly Tools illustrations, brand assets, logos, orb visuals, monk silhouettes, or custom graphics.
- Internal prompts or product strategy documents.
- Exact production UI layouts that would make cloning easy.

## Safe To Include

- Generic standalone utilities.
- Simplified demos.
- Toy implementations.
- Mock-only examples.
- BYO-AI templates where users enter their own API key locally.
- Public API connector demos using open/public APIs only.
- Generic calm UI components.
- Documentation and principles.
- Deprecated prototypes rewritten from scratch as generic examples.
- Small starter apps that teach one concept.

## Transformation Rule

If something is inspired by Quietly Tools, transform it into a generic teaching version.

| Production thing | Public version |
| --- | --- |
| MindMark production editor | Simple markdown preview demo |
| Memoir production feature | Generic memory-card writing demo with mock data |
| Quietly share URLs | Toy local short-link demo with mock storage |
| Desk Reset production ritual system | Simple breathing timer |
| Focus Flow Zen mode | Basic timer ring |
| Premium orb visualizer | Generic CSS breathing orb |
| Production UI cards | Generic calm cards |

The public repo can teach the concept, but must not expose the product implementation.

## File Safety Review

Before creating or modifying files, check for:

- Secrets.
- Private URLs.
- Production identifiers.
- Real user data.
- Proprietary product logic.
- Exact production UI.
- Analytics, payment, or auth code.
- Backend or database details.
- Premium brand assets.

Use placeholders instead:

- `YOUR_API_KEY_HERE`
- `https://example.com`
- `mock-user`
- `sample-note`
- `sample-memory`
- `mock-data.json`

## Commit Safety Checklist

- [ ] No production Quietly Tools code was copied.
- [ ] No MindMark production code was added.
- [ ] No Memoir production code was added.
- [ ] No production share-link logic was added.
- [ ] No auth, payment, donation, subscription, or analytics code was added.
- [ ] No secrets or `.env` files were added.
- [ ] No private URLs or backend endpoints were added.
- [ ] No real user data or memoir/note content was added.
- [ ] No premium brand assets were added.
- [ ] All examples use mock data.
- [ ] README clearly states this is not the main product.
- [ ] Disclaimers are present.
- [ ] License is MIT.

If any item fails, remove the risky content before completing the task.

