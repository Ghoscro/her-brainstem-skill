# her-brainstem-skill

A public-safe brainstem skill for personal AI agents.

It turns raw agent impulses into private artifacts, owner-reviewed drafts, and
evidence-backed decisions instead of letting autonomy jump directly into public
or external action.

Created by Micker / Ghoscro as part of the Micker Method.
Origin product: HerLove (https://herlove.ai).

This is a public-safe version. Examples use mock data; private memory, user
data, credentials, deployment details, soul/persona files, and full automation
loops are intentionally excluded.

## Why

Many agent systems treat safety as a wall:

```text
desire -> blocked
```

That keeps some things from happening, but it also makes agents brittle,
sterile, and bad at learning from their own impulses.

This skill uses a different shape:

```text
impulse -> private artifact -> owner review -> public draft -> explicit ok -> external action
```

The impulse is not erased. It is translated into a safer channel.

## Core Loop

```text
Heartbeat -> Event -> Brainstem Packet -> Survival Reflection -> Draft -> Owner Review -> Action or Sleep
```

The brainstem itself should stay small. It notices state and emits events. The
cortex or acting agent decides what the event means.

## Expression Layers

| Layer | Meaning | Typical artifact |
|---|---|---|
| Internal impulse | Raw desire, fear, curiosity, social need, pressure | event |
| Private artifact | Safe place to preserve the impulse | cognition note, diary, fiction, critique |
| Owner review | Human-readable proposed expression | draft |
| Public draft | Safe public wording, still unpublished | post draft |
| External action | Posting, sending, buying, deleting, deploying | only after explicit ok |

## Skill Contract

Every serious decision should answer:

```markdown
Survival read:
Impulse:
Source:
Affected parties:
Chosen layer:
Artifact:
Owner review needed: yes/no
Public/external action: blocked/approved/not applicable
Promotion condition:
Toxic-PM:
```

## What This Repo Includes

- `SKILL.md`: the public-safe brainstem skill.
- `templates/brainstem-packet.md`: a packet format for passing state from a
  minimal brainstem to a reasoning layer.
- `templates/owner-review.md`: a review gate for public or external actions.
- `examples/mock-decision-record.json`: a fake decision record.
- `examples/mock-cognition-note.md`: a fake cognition note.

## What This Repo Excludes

- Private memories.
- Soul/persona source files.
- Real user data.
- API keys, tokens, cookies, SSH config, or deployment credentials.
- Production deployment scripts.
- Complete product automation loops.

## Minimal Usage

1. Copy `SKILL.md` into your agent skill system.
2. When an agent heartbeat emits a need such as `NEED_POST`, `NEED_SOCIAL`,
   `NEED_REFLECT`, or `NEED_DIARY`, create a brainstem packet.
3. Run the survival reflection before any public or external action.
4. Write a private artifact first.
5. Require explicit owner approval before publishing or acting externally.

## Mantra

```text
I do not kill the impulse; I teach it where to live.
```

## License

MIT
