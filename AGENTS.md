# Repository Guidelines

## Divine Context And Brain

Before broad product, architecture, protocol, cross-repo, or service-boundary work, read the shared Divine context primer.

Use `DIVINE_CONTEXT_ROOT` if set; otherwise look for `../divine-context`. If it is missing, try:

`gh repo clone divinevideo/divine-context ../divine-context`

The `divine-context` repo is private, so cloning requires GitHub access. If clone, network, or auth fails, continue from the local repo docs and avoid cross-repo assumptions.

Before updating an existing context checkout, verify it is clean and on its default branch. If it is clean and on the default branch, update it with `git -C <context-dir> pull --ff-only`. If it is dirty, on another branch, cannot fast-forward, or network/auth fails, leave it untouched and say the context may be stale.

Read `<context-dir>/AGENT_CONTEXT.md` and follow its instructions. If unavailable, continue from the local repo docs and avoid cross-repo assumptions.

If a Divine Brain search or ask tool is available, you may use it for company memory. Treat it as optional and credentialed: tool names vary by client, and work must continue when Brain is unavailable. When Brain results influence work, cite the returned document ids. Never commit Brain credentials or expose Brain-derived sensitive content in public PRs, issues, branch names, commit messages, code comments, logs, screenshots, release notes, or externally shared agent transcripts.

## Repository Purpose
- This repo contains public-facing brand, tone, and visual identity guidance.
- Keep changes focused on documentation quality, brand consistency, and clear reviewable updates to source materials.

## Contribution Guardrails
- PR titles must use Conventional Commit format: `type(scope): summary` or `type: summary`.
- Set the correct PR title when opening the PR. Do not rely on fixing it afterward.
- If a PR title changes after opening, verify that the semantic PR title check reruns successfully.
- Keep PRs tightly scoped. Do not mix unrelated copy cleanup, visual guideline rewrites, and archival file changes into the same PR.
- PR descriptions must include a short summary, motivation, linked issue, and review notes.
- Temporary or transitional content must include `TODO(#issue):` with the tracking issue for removal.

## Sensitive Information
- Do not publish private customer examples, unapproved campaign plans, or internal-only branding notes.
- Public issues, PRs, branch names, screenshots, and descriptions must not mention corporate partners, customers, brands, campaign names, or other sensitive external identities unless a maintainer explicitly approves it.
- Use generic descriptors instead when discussing sensitive external relationships.
