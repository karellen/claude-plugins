# Karellen Claude Code Plugins

Claude Code plugin marketplace by [Karellen, Inc.](https://karellen.co)

## Available Plugins

| Plugin | Description |
|--------|-------------|
| [karellen-rr-mcp](https://github.com/karellen/karellen-rr-mcp) | rr reverse debugging via MCP |
| [karellen-jdb-mcp](https://github.com/karellen/karellen-jdb-mcp) | JDB (Java Debugger) via MCP |
| [karellen-lsp-mcp](https://github.com/karellen/karellen-lsp-mcp) | LSP code intelligence via MCP and native LSP |
| [karellen-qbo-mcp](https://github.com/karellen/karellen-qbo-mcp) | QuickBooks Online bookkeeping via MCP |

## Usage

Add this marketplace to Claude Code:

```bash
claude plugin marketplace add karellen/claude-plugins
```

Then install a plugin:

```bash
claude plugin install karellen-rr-mcp@karellen-plugins
```

Claude Code auto-updates only Anthropic's own marketplaces by default. To receive new
plugin releases automatically, turn on **Enable auto-update** for `karellen-plugins` under
`/plugin` → **Marketplaces**, or set `autoUpdate` on the marketplace in your settings:

```json
{
  "extraKnownMarketplaces": {
    "karellen-plugins": {
      "source": { "source": "github", "repo": "karellen/claude-plugins" },
      "autoUpdate": true
    }
  }
}
```

Otherwise update a plugin by hand with `claude plugin update <plugin>@karellen-plugins`.

## Prerequisites

Each plugin has its own prerequisites. See the individual plugin README for details.

## License

Apache-2.0
