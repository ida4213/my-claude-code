# my-claude-code

ida42's Claude Code Plugin Marketplace

## Installation

Add the marketplace to your Claude Code settings (`~/.claude/settings.json`):

```json
{
  "extraKnownMarketplaces": {
    "ida42": {
      "source": {
        "source": "github",
        "repo": "izumida-ryo/my-claude-code"
      }
    }
  }
}
```

Install the plugin:

```bash
claude plugin install ida42
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
