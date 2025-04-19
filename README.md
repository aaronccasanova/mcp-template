# mcp-template

A minimal, unopinionated template to quickly start building an MCP Server.

## Installation

> **Note:** The `npx github:<repo>` syntax is used for convenience and rapid prototyping. To use a specific version, append a branch name or tag (e.g. `npx github:<repo>#<branch-or-tag>`).

### Claude Code

1. Create a local `.mcp.json` file in your project directory or a global `~/.claude.json` file.
2. Add the following configuration:
   ```json
   {
     "mcpServers": {
       "mcp-template": {
         "type": "stdio",
         "command": "npx",
         "args": ["-y", "github:aaronccasanova/mcp-template"]
       }
     }
   }
   ```

### Claude for Desktop

1. Create a global `~/Library/Application Support/Claude/claude_desktop_config.json` file.
2. Add the following configuration:
   ```json
   {
     "mcpServers": {
       "mcp-template": {
         "command": "npx",
         "args": ["-y", "github:aaronccasanova/mcp-template"]
       }
     }
   }
   ```

### Cursor

1. Create a local `.cursor/mcp.json` file in your project directory or a global `~/.cursor/mcp.json` file.
2. Add the following configuration:
   ```json
   {
     "mcpServers": {
       "mcp-template": {
         "command": "npx",
         "args": ["-y", "github:aaronccasanova/mcp-template"]
       }
     }
   }
   ```

### VS Code

1. Create a local `.vscode/mcp.json` file in your project directory.
2. Add the following configuration:
   ```json
   {
     "servers": {
       "mcp-template": {
         "type": "stdio",
         "command": "npx",
         "args": ["-y", "github:aaronccasanova/mcp-template"]
       }
     }
   }
   ```

## Debugging

Use the MCP Inspector to debug your server.

```sh
pnpm build
npx @modelcontextprotocol/inspector node dist/server.js
```
