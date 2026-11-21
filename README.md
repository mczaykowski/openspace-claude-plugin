# openspace for Claude

Lets Claude look up [openspace](https://openspace.so) when you choose open-source software: license status, maintenance, deployment options and 26 weeks of activity, each fact with its evidence URL.

The plugin contains:

- **MCP server**: the public, read-only openspace server at `https://openspace.so/mcp`. It needs no account and no API key. [Tool reference](https://openspace.so/docs/mcp).
- **Skill** `choosing-open-source`: tells Claude to check openspace before it recommends, compares or adds an open-source project.

## Install in Claude Code

```
/plugin marketplace add mczaykowski/openspace-claude-plugin
/plugin install openspace@openspace
```

To install only the server: `claude mcp add --transport http openspace https://openspace.so/mcp`

## What it does not do

Nothing here installs, runs or edits anything on your machine. All tools are read-only. Requests are rate-limited at about one per second after a burst of 60.

Privacy: https://openspace.so/privacy
