# BAT publications - Interchouette ITC / ITCy

Canonical: [Interchouette-ITC/itcy-publications](https://github.com/Interchouette-ITC/itcy-publications)  
Worker fork: [Interchouette/itcy-publications](https://github.com/Interchouette/itcy-publications)

Default branch: **`dev`**. Public LinkedIn publish is gated by **BAT** on this repo.

## BAT merge rule (locked)

| What | Rule |
| --- | --- |
| **BAT** | **gRoussac Approve** on the publications PR (= BON a tirer) |
| **Merge** | Only after Approve. ITCy webhook may rebase-merge on Approve wake. |
| **Comments** | **Babysit only:** fix copy, rework, Q&A. Not BAT. Not a second gate. |

Always open PRs with `--reviewer gRoussac` (CODEOWNERS: `@gRoussac`).

GitHub Free + private: branch protection unavailable until org Pro. Habit + CODEOWNERS + this README enforce BAT until then.

## Content layout

See [`posts/README.md`](posts/README.md). Each draft is `posts/<slug>/body.md` + `meta.toml`.

## Workflow

```text
fork: feat/… from origin/dev
  → draft under posts/<slug>/ + disclosure metadata
  → PR into Interchouette-ITC/itcy-publications **dev**
  → --reviewer gRoussac
  → optional review comments (babysit / rework)
  → gRoussac Approve (BAT)
  → merge → ITCy may publish to LinkedIn company page
```

Never `git push upstream`. Never recreate `main`.

## License

BUSL-1.1 (Interchouette-ITC). See [LICENSE](LICENSE). Post drafts under `posts/` are covered by [posts/NOTICE](posts/NOTICE).
