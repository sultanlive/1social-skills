# 1Social skills for AI agents

Publish and schedule posts to Instagram, TikTok, X (Twitter), Threads, LinkedIn, Facebook Pages, YouTube Shorts and Bluesky from OpenClaw, Hermes, Claude Code, Codex and other agents that read [Agent Skills](https://agentskills.io).

Each skill teaches the agent one network's rules — length limits, required media, formats — and drives the hosted [1Social](https://1social.dev) MCP server (`https://mcp.1social.dev/mcp`), which publishes to accounts you own and reports what actually reached each network. Sign-in is OAuth in the browser: no API keys.

## Install

- **Any agent, via [skills.sh](https://skills.sh):** `npx skills add sultanlive/1social-skills`
- **OpenClaw, via [ClawHub](https://clawhub.ai):** see the table below.
- **Hermes:** `hermes skills tap add sultanlive/1social-skills`, one skill with `hermes skills install sultanlive/1social-skills/skills/<name>`, or straight from the site: `hermes skills install well-known:https://1social.dev/.well-known/skills/<name>`.

**OpenClaw plugins** (skill plus MCP connection in one install), in [`plugins/`](plugins): `openclaw plugins install clawhub:<name>`, e.g. `clawhub:instagram-by-1social`, then `openclaw mcp login 1social`.

With a bare skill, connect the MCP server once — each skill's *Setup* section has the command for your agent, and [1social.dev/mcp](https://1social.dev/mcp) covers every client.

| Skill | What it is | ClawHub |
|---|---|---|
| `instagram-post` | Instagram: post & schedule posts, Reels and carousels (1Social) | `openclaw skills install @sultanlive/instagram` |
| `tiktok-post` | TikTok: post & schedule videos and photo carousels (1Social) | `openclaw skills install @sultanlive/tiktok` |
| `x-twitter-post` | X (Twitter): post & schedule tweets and threads (1Social) | `openclaw skills install @sultanlive/twitter` |
| `threads-post` | Threads: post & schedule posts (1Social) | `openclaw skills install @sultanlive/threads` |
| `linkedin-post` | LinkedIn: post & schedule posts (1Social) | `openclaw skills install @sultanlive/linkedin` |
| `facebook-page-post` | Facebook: post & schedule Page posts (1Social) | `openclaw skills install @sultanlive/facebook` |
| `youtube-shorts` | YouTube Shorts: post & schedule Shorts (1Social) | `openclaw skills install @sultanlive/youtube-shorts` |
| `bluesky-post` | Bluesky: post & schedule posts and threads (1Social) | `openclaw skills install @sultanlive/bluesky` |
| `social-media-publisher` | Social Media Scheduler: post to Instagram, TikTok, X (Twitter), Threads, LinkedIn, Facebook, YouTube Shorts, Bluesky (1Social) | `openclaw skills install @sultanlive/social-media-scheduler` |
| `1social` | 1Social: post & schedule to every social network | `openclaw skills install @sultanlive/1social` |

## Requirements

A 1Social account with the networks you want to post to connected at [1social.dev/app](https://1social.dev/app). New accounts start with a free trial; publishing after the trial needs a paid plan — see [pricing](https://1social.dev/pricing).

## What data leaves your machine

The skills run no code. The agent sends the text and media of posts you ask it to preview or publish, and their schedule, to the 1Social MCP server; 1Social publishes them to the networks you connected. Details: [privacy policy](https://1social.dev/legal/privacy), [terms](https://1social.dev/legal/terms).

## Support

[1social.dev/support](https://1social.dev/support) · support@1social.dev

Generated from the 1Social monorepo; edit there, not here.

## License

MIT
