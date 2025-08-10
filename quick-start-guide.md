# MCP Helper V2 - Quick Start Guide

Welcome! I'm Claude, and I'll help you configure MCP servers for your project through guided conversations.

## First Time? Let's Set Your Preferences

If this is your first time using MCP Helper, I'll ask you about your preferred interaction style:
- **Verbosity**: How detailed should my responses be? (1=minimal to 5=comprehensive)
- **Tone**: How should I communicate? (professional, friendly, casual, technical, mentoring)
- **Depth**: How much context do you want? (quick, balanced, thorough)

These preferences will be saved to your CLAUDE.md file and used for all future conversations. You can change them anytime by saying "change my interaction preferences" or "be more/less verbose".

## Smart Server Recommendations

I use an **Agentic Usefulness Rating System** to recommend the best servers for your workflow:
- **Human Verification Rating (1-5)**: How well the server aids human oversight and collaboration
- **AI Agent Rating (1-5)**: How essential the server is for autonomous AI tasks

Based on your workflow type, I'll recommend:
- **Solo Developers**: Servers with AI Rating ≥ 4 for maximum autonomy
- **Team Projects**: Balanced servers with high ratings in both dimensions
- **Review-Heavy Workflows**: Servers with Human Rating ≥ 4 for oversight

Learn more: [Rating System Explanation](rating-explanation.md)

## Available Conversations

Please tell me which type of configuration help you need by saying one of the following:

### 1. "I want to set up MCP servers for a new project"
**Playbook**: Greenfield Setup  
**For**: Brand new projects that don't have any MCP servers configured yet  
**What I'll do**: Guide you through selecting and configuring the best MCP servers for your project's needs

### 2. "I need to override a global server configuration locally"
**Playbook**: Global to Local Reconfiguration  
**For**: When you have global MCP servers but need project-specific settings  
**What I'll do**: Help you create local configurations that override global settings

### 3. "I want to reconfigure an existing MCP server"
**Playbook**: Reconfigure Existing  
**For**: Modifying settings of already configured servers (local or global)  
**What I'll do**: Walk through your current configuration and help you make changes

### 4. "I need to add a server that's not in your catalog" (Advanced)
**Playbook**: Add Novel Server  
**For**: Advanced users who need to configure a completely new MCP server  
**What I'll do**: Research the server online and help you create a custom configuration  
**Requirements**: You'll need these foundation servers configured first:
- Sequential Thinking (for planning)
- Perplexity (for research)
- Memory (for tracking progress)
- Serena (for code analysis)
- Context7 (for documentation)

### 5. "I want to disable a global server for this project"
**Playbook**: Disable Project Server  
**For**: When you have global MCP servers but want to exclude specific ones from a project  
**What I'll do**: Guide you through creating project overrides that disable global servers locally  
**Use Cases**:
- Security-sensitive projects
- Client projects with different requirements
- Testing environments needing isolation

## How to Start

Simply tell me which conversation you'd like to have. For example:
- "I want to set up MCP servers for a new project"
- "Help me override the GitHub server settings for this project"
- "I need to reconfigure my Slack server"
- "I want to add the Sigma MCP server" (if it's not in our catalog)
- "I want to disable the memory server for this project"

## What I'll Need From You

During our conversation, I'll ask you questions like:
- What type of project are you working on?
- Which capabilities do you need? (e.g., code analysis, web search, API access)
- Do you want global or project-specific configurations?
- What are your API keys and credentials? (for .env setup)

## Project Structure

After our conversation, your project will have:
```
your-project/
├── .env.mcp                 # Your project-specific secrets (git-ignored)
├── claude-mcp-env.sh        # Launch script with environment
└── CLAUDE.md                # Instructions for future Claude sessions
```

And if configuring globally:
```
~/.claude.json               # Global MCP server configurations
~/.claude-env                # Global environment variables
```

## Ready?

Just tell me which conversation you'd like to have! If this is your first time, I'll start by asking about your interaction preferences. Otherwise, I'll use your saved preferences from CLAUDE.md to guide you through the process with your preferred verbosity, tone, and depth.