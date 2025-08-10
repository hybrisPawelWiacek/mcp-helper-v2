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

### Docker Desktop with MCP Toolkit

1. **Install Docker Desktop**:
   - **Mac**: Download from [docker.com](https://docker.com), drag to Applications
   - **Windows**: Download installer from [docker.com](https://docker.com), run the .exe
   - **Linux**: Download .deb package, run `sudo apt install docker-desktop-*.deb`

2. **Enable MCP Toolkit**:
   - Open Docker Desktop → Settings (gear icon)
   - Navigate to "Beta features"
   - Check "Enable Docker MCP Toolkit"
   - Click "Apply & Restart"

### Claude Code CLI
Install from [claude.ai/code](https://claude.ai/code)

That's it! Claude will guide you through everything else.

## What This Is

MCP Helper V2 is not a tool or CLI application. It's a collection of documentation and playbooks that Claude Code reads and follows to guide you through MCP server configuration. Think of it as an instruction manual that Claude uses to have intelligent conversations with you about your MCP server needs.

## Available Conversations

- **Greenfield Setup**: Adding MCP servers to new projects
- **Global to Local**: Overriding global server configurations locally
- **Reconfigure Existing**: Modifying existing server configurations
- **Add Novel Server**: (Advanced) Adding servers not in our catalog

Claude will adapt to your preferred interaction style (verbosity, tone, and depth) which you'll set on first use.

## Curated MCP Servers

We've evaluated 18 MCP servers for their effectiveness in agentic development. Here are our top recommendations:

### 🌟 Essential for AI Agents (Rating 5/5)
- **Serena** - Semantic code navigation and understanding. Replace Read/Grep with intelligent symbol search.
- **Sequential Thinking** - Complex problem planning and reasoning. Break down multi-step tasks systematically.
- **Memory** - Persistent context across sessions. Never lose project knowledge between conversations.

### 🚀 Core Development Stack (Rating 4/5)
- **GitHub** - Full git workflow integration. PRs, issues, code management from Claude.
- **Context7** - Up-to-date framework documentation. Prevent hallucination with real docs.
- **Firecrawl** - Web scraping and content extraction. Access any web documentation.
- **Perplexity** - Deep research and multi-source analysis. Answer complex technical questions.

### 💼 Team Collaboration (Rating 3-5/5)
- **Slack** - Team communication and notifications. Keep everyone in the loop.
- **Atlassian** - Jira/Confluence integration. Track tasks and documentation.
- **Notion** - Knowledge base management. Organize team documentation.

### 🔧 Specialized Tools
- **PostgreSQL** - Database operations and queries. Direct SQL access when needed.
- **Playwright/Puppeteer** - Browser automation and testing. Web scraping and E2E tests.
- **Docker MCP Toolkit** - Container management. Control Docker from Claude.
- **LinkedIn** - Professional network integration. Research and recruitment.
- **Brave Search** - Privacy-focused web search. Alternative to standard search.
- **Claude Code** - Meta-server for Claude operations. Self-improvement capabilities.
- **OpenMemory** - Alternative memory solution. Enhanced embedding-based recall.

Each server includes **Agentic Usefulness Ratings** (Human Verification 1-5, AI Agent 1-5) to help you choose based on your workflow. See [rating-explanation.md](rating-explanation.md) for detailed explanations.

## Performance Note

**Use Native Claude Code CLI** (`claude`) instead of `claude mcp serve` for **37% better performance**. Native tools avoid the 18+ second delays common with MCP server configurations.
