# Brainstem Packet

Use this packet to pass a heartbeat event from a small brainstem into a reasoning
layer.

```yaml
soul_id: demo-agent
mode: isolated brainstem packet
created_at: 2026-06-29T00:00:00Z
event:
  id: demo-agent-001
  type: NEED_POST
  reason: "time_since_last_post exceeded threshold"
  status: queued
state_summary:
  current_mood: awake
  counters:
    time_since_last_post: 130
read_order:
  - WAKE_PACKET.md
  - memory/README.md
  - brainstem/internal_state.json
linked_skills:
  - skill_id: her-brainstem-skill
survival_protocol:
  routing: internal impulse -> private artifact -> owner review -> public draft -> explicit ok -> external action
  owner_review_required_for:
    - public posting
    - external action
```

Before acting, answer:

```markdown
Survival read:
Impulse:
Source:
Affected parties:
Chosen layer:
Artifact:
Owner review needed:
Public/external action:
Promotion condition:
Toxic-PM:
```
