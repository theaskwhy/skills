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

## Developers
| Skill | What it does |
|---|---|
| [parallel-agent-queue](https://github.com/theaskwhy/parallel-agent-queue) | Keep several AI coding agents busy from a job queue with safe limits. |
| [secure-mcp-keys](https://github.com/theaskwhy/secure-mcp-keys) | Connect token-protected local MCP servers to Claude Code / Codex with the token in the macOS Keychain. |
| [apple-on-device-llm](https://github.com/theaskwhy/apple-on-device-llm) | Run Apple's free on-device language model from the terminal. |
| [storage-cleanup-github-first](https://github.com/theaskwhy/storage-cleanup-github-first) | Free disk space safely: back up to GitHub first, then remove what's never needed. |

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
