# BAT publications - Interchouette ITC / ITCy

Canonical: [Interchouette-ITC/itcy-publications](https://github.com/Interchouette-ITC/itcy-publications)  
Worker fork: [Interchouette/itcy-publications](https://github.com/Interchouette/itcy-publications)

Default branch: **`dev`**. LinkedIn publish is gated by **BAT** = merge of an approved PR here.

## BAT merge rule (locked)

A publications PR may merge only after **two** approvals:

| # | Who | Role |
| --- | --- | --- |
| 1 | **Interchouette** (ITCy worker) | Self-review on its own PR. GitHub blocks author `Approve`; post a review comment: `BAT #1 self-review complete`. |
| 2 | **gRoussac** (Greg) | Always requested as reviewer; must **Approve** (`BAT #2`). |

Do not merge with only one of those. Agent habit: always
`gh pr create … --reviewer gRoussac` (and re-request if missing).

GitHub Free + private: branch protection (required 2 reviews) is unavailable until org Pro. Enforce by this README + product contract/rule until then.

## Content layout

See [`posts/README.md`](posts/README.md). Each draft is `posts/<slug>/body.md` + `meta.toml`.

## Workflow

```text
fork: feat/… from origin/dev
  → draft under posts/<slug>/ + disclosure metadata
  → PR into Interchouette-ITC/itcy-publications **dev**
  → --reviewer gRoussac
  → Interchouette self-review → comment `BAT #1 self-review complete`
  → gRoussac Approve (`BAT #2`)
  → merge (= BAT green) → head branch auto-deletes
  → ITCy may publish to LinkedIn company page
```

Never `git push upstream`. Never recreate `main`.

## License

BUSL-1.1 (Interchouette-ITC). See [LICENSE](LICENSE). Post drafts under `posts/` are covered by [posts/NOTICE](posts/NOTICE).
