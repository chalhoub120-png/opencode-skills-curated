# OpenCode Skills — Curated (31)

A curated collection of 31 OpenCode skills (single source of truth: `open-code-skills-manager/skills/`), packaged for local use and as an HTTP catalog.

## Install locally

Copy a skill folder into your OpenCode skills directory:

```bash
# Windows
xcopy /E /I skills\<skill-id> %USERPROFILE%\.config\opencode\skills\<skill-id>\

# macOS/Linux
cp -r skills/<skill-id> ~/.config/opencode/skills/<skill-id>
```

Then reload: `/reload` or restart the session.

## HTTP catalog

Add to your `opencode.json`:

```jsonc
{
  "skills": ["https://<user>.github.io/opencode-skills-curated/"],
}
```

`index.json` lists all 31 skills with their files. Bump `version` in `index.json` to refresh cache.

## Skills (31)

agent-reach, brain-dump, carousels, caveman, clean-architecture, contract-review, dashboard-builder, decision-journal, deep-research, expense-report, explainer-infographic, graphify-me, inbox-triage, invoice-generator, karpathy-guidelines, kent-beck-style, mcp-builder, meeting-prep, morning-briefing, omniroute (pointer-only), personal-crm, ponytail, skill-creator, slide-deck, step-back, superpowers, vercel-composition-patterns, vercel-react-best-practices, vercel-web-design-guidelines, webapp-testing, workflow-visualizer.

## Notes

- `omniroute` is a **pointer-only** skill (AI Gateway server, not native). Server code stays upstream (npm/Docker). See `skills/omniroute/SKILL.md`.
- Richer bundled files (scripts/examples) are included where available; generated artifacts (`__pycache__`, `node_modules`, `*.pyc`) are excluded via `.gitignore`.
- No secrets committed. Provide API keys via `{env:...}`.

## License

MIT
