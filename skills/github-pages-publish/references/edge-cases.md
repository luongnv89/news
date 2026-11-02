# Edge cases

Read when a run hits one of these situations (root SKILL.md → Step 4 or Step 5).

- The target is the current repo, but the checkout is on a feature branch or has unpushed commits: use a fresh clone, then tell the user that their local default branch is behind `origin`.
- The content is a framework or site-generator project: `check-site` returns `needs-build`. Report BLOCKED with the Decision "build it, then publish the output folder".
- The content is already the site folder in the workspace: `sync-site` copies nothing and only refreshes the manifest.
- `CNAME` in the site folder is never deleted. The custom domain itself lives in the Pages settings.
- Files whose names start with `.` are never deployed. `check-site` warns about them.
- The repo name is `<owner>.github.io`: a user site at the domain root. No `/<name>/` prefix applies.
