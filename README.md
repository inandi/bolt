# Bolt

**Bolt** is a VS Code extension that puts a script launcher in your status bar. One click opens a searchable menu of your scripts; pick one and it runs in the integrated terminal.

## Setup

1. Open the project in VS Code and press **F5** to launch the Extension Development Host.
2. In settings, add your scripts under **Bolt: Scripts** (`bolt.scripts`), for example:

```json
"bolt.scripts": [
  { "alias": "Reset DB", "path": "./scripts/reset-db.sh" },
  { "alias": "Deploy", "path": "~/scripts/deploy.sh" }
]
```

- **alias** — Label shown in the menu.
- **path** — Script location: `./` = workspace-relative, `~` = home directory, or an absolute path.

## Usage

Click **$(zap) Bolt** in the status bar, choose a script from the Quick Pick list, and it runs in a new Bolt terminal.

See [docs/OVERVIEW.md](docs/OVERVIEW.md) for the full spec and development overview.
