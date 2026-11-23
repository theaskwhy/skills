# Skills by The Ask Why Company

The catalogue of practical Agent Skills for creators, app makers and developers. Each skill lives in its own repository — click a name to open it. Works with Claude (Claude Code, Claude.ai) and any tool that reads the open [Agent Skills](https://agentskills.io) `SKILL.md` format.

## Creators and marketing
| Skill | What it does |
|---|---|
| [reel-editor](https://github.com/theaskwhy/reel-editor) | Turn long raw footage into short vertical reels: find the moments, where to cut, montages, rhythm, sound, captions, originality, credit. |
| [launch-reveal-series](https://github.com/theaskwhy/launch-reveal-series) | Plan a "Day N of showing you what we built" launch series with cliffhangers, per-platform posting and free scheduling. |
| [social-account-audit](https://github.com/theaskwhy/social-account-audit) | Read Instagram/Facebook/TikTok/YouTube insights and turn them into a posting plan. |
| [free-video-tools-check](https://github.com/theaskwhy/free-video-tools-check) | Check what free AI video, editing and scheduling tools really allow before relying on them. |
| [ai-council](https://github.com/theaskwhy/ai-council) | Run one brief through several AI models independently and merge the results. |

## App makers
| Skill | What it does |
|---|---|
| [app-store-answer-check](https://github.com/theaskwhy/app-store-answer-check) | Verify App Store / Google Play / Galaxy Store privacy, age-rating and listing answers against the code before submitting. |
| [mobile-launch-readiness](https://github.com/theaskwhy/mobile-launch-readiness) | Review a mobile app for final launch readiness across feature flags, routes, accessibility, offline behavior, store materials, review access, build identity, and… |
| [beginner-persona-gap-review](https://github.com/theaskwhy/beginner-persona-gap-review) | Synthesize independent beginner-focused reviews into a deduplicated, code-checked gap list and a release disposition. |

## Developers
| Skill | What it does |
|---|---|
| [parallel-agent-queue](https://github.com/theaskwhy/parallel-agent-queue) | Keep several AI coding agents busy from a job queue with safe limits. |
| [secure-mcp-keys](https://github.com/theaskwhy/secure-mcp-keys) | Connect token-protected local MCP servers to Claude Code / Codex with the token in the macOS Keychain. |
| [apple-on-device-llm](https://github.com/theaskwhy/apple-on-device-llm) | Run Apple's free on-device language model from the terminal. |
| [storage-cleanup-github-first](https://github.com/theaskwhy/storage-cleanup-github-first) | Free disk space safely: back up to GitHub first, then remove what's never needed. |

## Research and data
| Skill | What it does |
|---|---|
| [claim-verification](https://github.com/theaskwhy/claim-verification) | Verify important factual claims with traceable sources, dates, provenance, corroboration, and explicit uncertainty. |
| [evidence-first-data-analysis](https://github.com/theaskwhy/evidence-first-data-analysis) | Analyze and validate datasets with reproducible, evidence-backed methods. |
| [research-data-qa](https://github.com/theaskwhy/research-data-qa) | Independently audit research datasets for structural integrity, evidence and provenance, coverage, contradictions, and readiness, with explicit fail-closed gates. |
| [research-spreadsheet-architect](https://github.com/theaskwhy/research-spreadsheet-architect) | Design reviewable research tables and spreadsheets with stable schemas, traceable evidence, explicit uncertainty, and reproducible counts. |
| [inventory-reconciler](https://github.com/theaskwhy/inventory-reconciler) | Compare frozen independent records with a separate read-only catalog and prepare conservative match, conflict, duplicate, and unmatched candidate findings for human… |
| [social-research-reader](https://github.com/theaskwhy/social-research-reader) | Read and compare public social content with clear evidence layers, source links, coverage limits, privacy safeguards, and no unauthorized access or unapproved spending. |
| [rights-checked-image-download](https://github.com/theaskwhy/rights-checked-image-download) | Safely retrieve a small, bounded set of images from a specific public URL when official image sources cannot provide them. |

## Teams working with AI agents
| Skill | What it does |
|---|---|
| [agent-permission-boundaries](https://github.com/theaskwhy/agent-permission-boundaries) | Define actions an AI agent may complete independently and actions reserved for explicit human approval, including money, security settings, production, publication,… |
| [risk-based-review-gates](https://github.com/theaskwhy/risk-based-review-gates) | Set review effort from change risk, reviewer independence, and exact commit state. |
| [decision-ledger](https://github.com/theaskwhy/decision-ledger) | Maintain durable owner decisions in one living ledger and one issue thread, including superseded history and a parking lane for future paid work. |
| [project-handoff](https://github.com/theaskwhy/project-handoff) | Close out a substantial project session with a source-backed checkpoint, preserved decisions and gates, concrete blockers, and next steps for a new person or agent. |
| [open-source-privacy-scan](https://github.com/theaskwhy/open-source-privacy-scan) | Scan a project before it becomes public for personal data, confidential names, local paths, credentials, internal tool references, and identifying Git history. |

## Install in Claude — pick only the skills you need
Each skill is separate. Install one, a few, or all.

**Claude Code:** add the catalogue once, then install any skill by name:
```
/plugin marketplace add theaskwhy/skills
/plugin install reel-editor@theaskwhy
```
Swap `reel-editor` for any skill name in the tables above (e.g. `social-account-audit@theaskwhy`).

**Manual (any tool that reads SKILL.md):** open the skill's repository and copy its `skills/<name>/` folder into `~/.claude/skills/` (personal) or `.claude/skills/` (project).

**Claude.ai:** download that skill's `skills/<name>/` folder from its repository, zip it, and upload it under Settings → Capabilities → Skills.

## Use it with any AI agent
These skills use the open **Agent Skills** standard (`SKILL.md`), so the same file works in Claude Code, OpenAI Codex, Cursor, Gemini CLI, GitHub Copilot, Windsurf, Antigravity, OpenCode, Goose and many more.

**Quickest (any supported agent):** the open-source `skills` installer detects your tools and installs for them:
```
npx skills add theaskwhy/<skill-name>
```

**Manual:** copy the skill's `skills/<skill-name>/` folder into your tool's skills folder:

| Tool | Personal (all projects) | One project |
|---|---|---|
| Claude Code | `~/.claude/skills/` | `.claude/skills/` |
| OpenAI Codex | `~/.codex/skills/` | `.agents/skills/` |
| Cursor | `~/.cursor/skills/` | `.cursor/skills/` |
| Gemini CLI / Antigravity | `~/.gemini/skills/` | `.gemini/skills/` |
| GitHub Copilot | `~/.copilot/skills/` | `.github/skills/` |
| Windsurf | — | `.windsurf/skills/` |
| Any spec-compliant agent | — | `.agents/skills/` |

Folder names change between tool versions — if a tool doesn't pick it up, check its current skills documentation. Tools without skills support can still use it: paste `SKILL.md` into the tool's rules/instructions file (e.g. `AGENTS.md`, Cursor rules).

## Credits
Built by [The Ask Why Company](https://github.com/theaskwhy) from hands-on work and independent research. Platform rules and free tiers change — check current guidance before relying on any number here.

MIT licensed. If you use or adapt these skills, a credit to The Ask Why Company is appreciated.
