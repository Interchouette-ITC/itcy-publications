# BAT publications - Interchouette ITC / ITCy

Canonical: [Interchouette-ITC/itcy-publications](https://github.com/Interchouette-ITC/itcy-publications)  
Worker fork: [Interchouette/itcy-publications](https://github.com/Interchouette/itcy-publications)

Default branch: **`dev`**. LinkedIn publish is gated by **BAT** = merge of an approved PR here.

## BAT merge rule (locked)

A publications PR may merge only after **two** approvals:

| # | Who | Role |
| --- | --- | --- |
| 1 | **Interchouette** (ITCy worker) | Self-review then **Approve** on its own draft/PR |
| 2 | **gRoussac** (Greg) | Always requested as reviewer; must **Approve** |

Do not merge with only one of those. Agent habit: always
`gh pr create … --reviewer gRoussac` (and re-request if missing).

GitHub Free + private: branch protection (required 2 reviews) is unavailable until org Pro. Enforce by this README + product contract/rule until then.

## Workflow

```text
fork: feat/… from origin/dev
  → draft content + disclosure metadata
  → PR into Interchouette-ITC/itcy-publications **dev**
  → --reviewer gRoussac
  → Interchouette self-review → Approve
  → gRoussac Approve
  → merge (= BAT green) → head branch auto-deletes
  → ITCy may publish to LinkedIn company page
```

Never `git push upstream`. Never recreate `main`.
