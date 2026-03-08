# my-claude-code

ida4213's Claude Code Plugin Marketplace

## Installation

Add the marketplace to your Claude Code settings (`~/.claude/settings.json`):

```json
{
  "extraKnownMarketplaces": {
    "my-tools": {
      "source": {
        "source": "github",
        "repo": "ida4213/my-claude-code"
      }
    }
  }
}
```

Install the plugin:

```bash
claude plugin install my-tools
```

## Directory Structure

```
my-claude-code/
├── .claude-plugin/
│   └── marketplace.json     # Marketplace manifest
├── agents/                  # Agent definitions
│   └── general-purpose.md
├── skills/                  # Skill definitions
│   └── commit-push/
│       └── SKILL.md
├── rules/                   # Rule definitions
│   └── git-workflow.md
└── mcp-configs/             # MCP server configuration samples
```

## Agents

### general-purpose
General-purpose software engineering agent for implementation, debugging, refactoring, and code review.

## Skills

### `/commit-push`
Commits staged changes and pushes to remote.
