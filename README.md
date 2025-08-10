# MCP Helper V2

A conversational framework for configuring MCP servers with Claude Code.

## Quick Start

1. Clone this repository into your project:
   ```bash
   git clone https://github.com/hybrisPawelWiacek/mcp-helper-v2.git
   ```

2. Start Claude Code:
   ```bash
   claude
   ```

3. Tell Claude:
   > "There is a file quick-start-guide.md in mcp-helper-v2, tell me what options I have"

4. Choose your conversation type and follow the guided process.

## Requirements

- Docker Desktop with MCP Toolkit enabled
- Claude Code CLI

That's it! Claude will guide you through everything else.

## What This Is

MCP Helper V2 is not a tool or CLI application. It's a collection of documentation and playbooks that Claude Code reads and follows to guide you through MCP server configuration. Think of it as an instruction manual that Claude uses to have intelligent conversations with you about your MCP server needs.

## Available Conversations

- **Greenfield Setup**: Adding MCP servers to new projects
- **Global to Local**: Overriding global server configurations locally
- **Reconfigure Existing**: Modifying existing server configurations
- **Add Novel Server**: (Advanced) Adding servers not in our catalog

Each conversation type has its own personality and guided flow to ensure you get exactly what you need.
