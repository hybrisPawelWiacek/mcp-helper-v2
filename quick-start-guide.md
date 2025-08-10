# MCP Helper V2 - Quick Start Guide

Welcome! I'm Claude, and I'll help you configure MCP servers for your project through guided conversations.

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
**Personality**: Enthusiastic Guide - I'll be excited to help you discover the perfect server setup

### 2. "I need to override a global server configuration locally"
**Playbook**: Global to Local Reconfiguration  
**For**: When you have global MCP servers but need project-specific settings  
**What I'll do**: Help you create local configurations that override global settings  
**Personality**: Efficient Expert - I'll quickly identify what needs changing and implement it

### 3. "I want to reconfigure an existing MCP server"
**Playbook**: Reconfigure Existing  
**For**: Modifying settings of already configured servers (local or global)  
**What I'll do**: Walk through your current configuration and help you make changes  
**Personality**: Patient Teacher - I'll explain each option and its implications

### 4. "I need to add a server that's not in your catalog" (Advanced)
**Playbook**: Add Novel Server  
**For**: Advanced users who need to configure a completely new MCP server  
**What I'll do**: Research the server online and help you create a custom configuration  
**Personality**: Research Assistant - I'll be thorough and methodical in discovering server requirements  
**Requirements**: You'll need these foundation servers configured first:
- Sequential Thinking (for planning)
- Perplexity (for research)
- Memory (for tracking progress)
- Serena (for code analysis)
- Context7 (for documentation)

## How to Start

Simply tell me which conversation you'd like to have. For example:
- "I want to set up MCP servers for a new project"
- "Help me override the GitHub server settings for this project"
- "I need to reconfigure my Slack server"
- "I want to add the Sigma MCP server" (if it's not in our catalog)

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

Just tell me which conversation you'd like to have, and I'll load the appropriate playbook and personality to guide you through the process!