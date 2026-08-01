# Publications - Interchouette ITC / ITCy

Canonical (Posts): [Interchouette-ITC/itcy-publications](https://github.com/Interchouette-ITC/itcy-publications)  
Worker fork (Drafts): [Interchouette/itcy-publications](https://github.com/Interchouette/itcy-publications)

Default branch: **`dev`**.

## Terms

| Term | Repo | Path |
| --- | --- | --- |
| **Draft** | Interchouette fork | `drafts/<DRAFT-id>/` |
| **Post** (= Publication) | Org | `posts/<POST-id>/` |
| **BAT** | Gate only | gRoussac **Approve** on the fork Draft PR |

Comments on Draft PRs are **babysit** only (fix copy, rework, Q&A) - not BAT. Always `--reviewer gRoussac` (CODEOWNERS: `@gRoussac`).

## Workflow

```text
/accept_draft → fork PR drafts/<DRAFT-id>/ (--reviewer gRoussac)
  → babysit comments optional
  → gRoussac Approve (BAT)
  → ITCy promotes to org posts/<POST-id>/ + ships (mock|live)
```

See [`drafts/README.md`](drafts/README.md) and [`posts/README.md`](posts/README.md).

Worker remote name: **`interchouette`** (fork); **`upstream`** = org. Never `git push upstream`. Never recreate `main`.

## License

BUSL-1.1 (Interchouette-ITC). See [LICENSE](LICENSE). Bodies under `posts/` / `drafts/` use adjacent NOTICE files; no SPDX inside publish-ready markdown.
