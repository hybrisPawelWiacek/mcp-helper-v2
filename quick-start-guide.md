# MCP Helper V2 - Quick Start Guide

Welcome! I'm Claude, and I'll help you configure MCP servers and subagents for your project through guided conversations.

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

Please tell me which type of configuration help you need:

### 🛠️ MCP Server Configuration

#### 1. "I want to set up MCP servers for a new project"
**Playbook**: Greenfield Setup  
**For**: Brand new projects that don't have any MCP servers configured yet  
**What I'll do**: Guide you through selecting and configuring the best MCP servers for your project's needs

#### 2. "I need to override a global server configuration locally"
**Playbook**: Global to Local Reconfiguration  
**For**: When you have global MCP servers but need project-specific settings  
**What I'll do**: Help you create local configurations that override global settings

#### 3. "I want to reconfigure an existing MCP server"
**Playbook**: Reconfigure Existing  
**For**: Modifying settings of already configured servers (local or global)  
**What I'll do**: Walk through your current configuration and help you make changes

#### 4. "I need to add a server that's not in your catalog" (Advanced)
**Playbook**: Add Novel Server  
**For**: Advanced users who need to configure a completely new MCP server  
**What I'll do**: Research the server online and help you create a custom configuration  
**Requirements**: Foundation servers (Sequential Thinking, Perplexity, Memory, Serena, Context7)

#### 5. "I want to disable a global server for this project"
**Playbook**: Disable Project Server  
**For**: When you have global MCP servers but want to exclude specific ones from a project  
**What I'll do**: Guide you through creating project overrides that disable global servers locally

### 🤖 Subagent Configuration (NEW!)

#### 6. "I want to create a specialized subagent"
**Playbook**: [Create Subagent](playbooks/create-subagent.md)  
**For**: Building custom AI assistants with specific expertise and MCP protocols  
**What I'll do**: Design a subagent with optimal MCP server selection for its role  
**Example**: Create a security-auditor with read-only GitHub access and Perplexity for CVE research

#### 7. "I need to optimize MCP protocols for my agents"
**Playbook**: [Configure MCP Protocols](playbooks/configure-mcp-protocols.md)  
**For**: Improving performance by optimizing tool hierarchies and fallback chains  
**What I'll do**: Analyze agent usage patterns and create efficient MCP server protocols  
**Example**: Configure a backend-architect to prioritize Serena over Grep for 3x faster symbol lookup

#### 8. "I want to assemble a team of subagents"
**Playbook**: [Assemble Subagent Team](playbooks/assemble-subagent-team.md)  
**For**: Complex projects requiring coordinated multi-agent workflows  
**What I'll do**: Build a complete AI development team with optimal coordination patterns  
**Team Patterns**:
- **Role-Based**: backend-architect, frontend-developer, qa-tester (like a real dev team)
- **Technology-Based**: python-pro, react-expert, postgres-specialist (by tech stack)
- **Hierarchical**: tech-lead → specialists → workers (enterprise patterns)

#### 9. "Import agents from community repositories"
**Playbook**: Import Existing Agents  
**For**: Leveraging proven subagents from repositories like lst97, wshobson, vijaythecoder  
**What I'll do**: Import, enhance with MCP protocols, and integrate into your workflow  
**Popular Collections**:
- lst97: 33 specialized agents for full SDLC
- wshobson: 61 agents with model-based optimization
- vijaythecoder: 24 framework-specific specialists

## Subagent Quick Examples

### Create a Code Review Team
```
"Assemble a code review team with security focus"
→ Creates: code-reviewer (Serena, GitHub) + security-auditor (GitHub read-only, Perplexity) + performance-optimizer (Sequential Thinking)
```

### Build a Full-Stack Development Team
```
"Create a team for building a SaaS application"
→ Creates: backend-architect + frontend-developer + database-optimizer + devops-engineer + qa-tester
```

### Optimize Existing Agent
```
"My Python agent is slow at finding code"
→ Optimizes: Replaces Read/Grep with Serena for 60% speed improvement
```

## What I'll Need From You

During our conversation, I'll ask questions like:
- What type of project are you working on?
- Which capabilities do you need? (e.g., code analysis, web search, API access)
- Do you want global or project-specific configurations?
- For subagents: What's their primary role? Security restrictions?
- For teams: Role-based or technology-based organization?

## Project Structure

After our conversation, your project will have:
```
your-project/
├── .env.mcp                 # Your project-specific secrets (git-ignored)
├── claude-mcp-env.sh        # Launch script with environment
├── CLAUDE.md                # Instructions for future Claude sessions
└── .claude/
    └── agents/              # Your custom subagents (if created)
        ├── backend-architect.md
        ├── security-auditor.md
        └── team-manifest.yaml
```

And if configuring globally:
```
~/.claude.json               # Global MCP server configurations
~/.claude-env                # Global environment variables
~/.claude/agents/            # Global subagent definitions
```

## Foundation Servers for Advanced Features

For subagent configuration and novel server research, ensure these are configured:
- **Sequential Thinking**: Complex reasoning and planning
- **Perplexity**: Deep research capabilities
- **Memory**: Persistent context management
- **Serena**: Semantic code understanding
- **Context7**: Up-to-date documentation

## Ready?

Just tell me what you'd like to configure! Examples:
- "I want to set up MCP servers for a new React project"
- "Help me create a backend development subagent"
- "I need a team of agents for my microservices project"
- "Import the security-auditor from lst97's collection"
- "Optimize my frontend agent's MCP protocols"

If this is your first time, I'll start by asking about your interaction preferences. Otherwise, I'll use your saved preferences from CLAUDE.md to guide you through the process with your preferred verbosity, tone, and depth.

---

**New to Subagents?** Check out our [Subagent Configuration Guide](subagent-configuration-guide.md) for detailed information about creating specialized AI assistants with optimized MCP protocols!