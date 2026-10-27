# LinkedIn by 1Social for OpenClaw

Publish and schedule LinkedIn posts from OpenClaw. This bundle plugin connects OpenClaw to the [1Social](https://1social.dev) MCP server (`https://mcp.1social.dev/mcp`) and adds the `linkedin-post` skill, which carries LinkedIn's rules so the agent drafts posts the network will accept.

## Install

```bash
openclaw plugins install clawhub:linkedin-by-1social
openclaw mcp login 1social
```

The login opens a page where you sign in to 1Social (OAuth — no API key). On a machine with no browser, finish it on another device and pass the code back with `openclaw mcp login 1social --code <code>`.

## Requirements

A 1Social account with your networks connected at [1social.dev/app](https://1social.dev/app). New accounts start with a free trial; publishing after it needs a paid plan — see [pricing](https://1social.dev/pricing).

## What data leaves your machine

The plugin runs no code. The agent sends the text and media of posts you ask it to preview or publish, and their schedule, to the 1Social MCP server. Details: [privacy policy](https://1social.dev/legal/privacy).

## License

MIT
