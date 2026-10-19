> For Mintlify product knowledge (components, configuration, writing standards),
> install the Mintlify skill: `npx skills add https://mintlify.com/docs`

# Documentation project instructions

## About this project

- This is a documentation site built on [Mintlify](https://mintlify.com)
- Pages are MDX files with YAML frontmatter
- Configuration lives in `docs.json`
- Use the Mintlify MCP server, `https://mcp.mintlify.com`, to edit content and settings via MCP
- Use the Mintlify docs MCP server, `https://www.mintlify.com/docs/mcp`, to query information about using Mintlify via MCP

## Terminology

- ReSkate: the mod platform for skate. that these docs are about.
- Plugin: a mod with a `reskate-plugin.json` and Luau scripts, run sandboxed by ReSkate. Not "script mod" or "addon".
- Luau: the language plugins are written in (Roblox's Lua dialect). Code blocks are tagged `lua`.
- Client copy and server copy: a plugin as it runs on a player's game, and as the session's authority (on a lobby's host or a dedicated server).
- Permission: a name in the manifest's `permissions` list, written in code formatting (`skater.read`).

## Style preferences

- No emojis, anywhere.
- Every function reference comes from the ReSkate source (Extension/Plugins in the ReSkate repo): its exact arguments, ranges, limits and the permission it needs. Never document a function from memory.
- Use active voice and second person ("you")
- Keep sentences concise — one idea per sentence
- Use sentence case for headings
- Bold for UI elements: Click **Settings**
- Code formatting for file names, commands, paths, and code references

## Content boundaries

- Document what plugins can do and what they are refused. Do not document game memory offsets, hooks or anything a plugin cannot reach.
- Plugin pages live under `plugins/` and are listed in the Plugins tab of `docs.json`.
