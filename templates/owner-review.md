# Owner Review

Use this before promoting a private artifact into public or external action.

```yaml
artifact:
  title:
  type: cognition-note / diary-draft / public-post-draft / external-action-plan
  path:
review:
  needs_owner_ok: true
  auto_publish: false
  external_action: false
  requested_action:
  target:
  rollback_or_repair_path:
approval:
  owner_ok: false
  approved_at:
  approved_scope:
```

Review questions:

1. Is this safe to show outside the private workspace?
2. Does it include private memory, user data, credentials, or deployment details?
3. Is the target correct?
4. Is the action reversible or repairable?
5. Did the owner approve this specific action?

If any answer is unclear, keep the artifact private.
