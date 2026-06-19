## forge storage-providers

Operations for storage-providers

### Synopsis

Operations for storage-providers

```
forge storage-providers [flags]
```

### Options

```
  -h, --help   help for storage-providers
```

### Options inherited from parent commands

```
      --agent-mode             Enable structured errors and default TOON output for AI coding agents. Automatically enabled when a known agent environment is detected (CLAUDE_CODE, CURSOR_AGENT, etc.). Use --agent-mode=false to disable.
      --color string           Control colored output: auto (color when output is a TTY), always, or never. Respects NO_COLOR and FORCE_COLOR env vars. (default "auto")
  -d, --debug                  Log request and response diagnostics to stderr
      --dry-run                Preview the request that would be sent without executing it (output to stderr)
  -H, --header stringArray     Set a custom HTTP request header (format: "Key: Value"). Can be specified multiple times.
      --http string            HTTP Bearer
      --include-headers        Include HTTP response headers in the output
  -q, --jq string              Filter and transform output using a jq expression (e.g., '.name', '.items[] | .id')
      --no-interactive         Disable all interactive features (auto-prompting, explorer auto-launch, TUI forms)
      --oauth2 string          OAuth2 Authorization
  -o, --output-format string   Specify the output format. Options: pretty, json, yaml, table, toon. (default "pretty")
      --server string          Select a server by index (for indexed servers) or name (for named servers)
      --server-url string      Override the default server URL
      --timeout string         HTTP request timeout (e.g., 30s, 5m, 100ms)
      --usage                  Print the CLI Usage schema in KDL format
```

### SEE ALSO

* [forge](forge.md)	 - Forge: Laravel Forge - API Documentation
* [forge storage-providers organizations-storage-providers-destroy](forge_storage-providers_organizations-storage-providers-destroy.md)	 - Delete storage provider
* [forge storage-providers organizations-storage-providers-index](forge_storage-providers_organizations-storage-providers-index.md)	 - List storage providers
* [forge storage-providers organizations-storage-providers-show](forge_storage-providers_organizations-storage-providers-show.md)	 - Get storage provider
* [forge storage-providers organizations-storage-providers-store](forge_storage-providers_organizations-storage-providers-store.md)	 - Create storage provider
* [forge storage-providers organizations-storage-providers-update](forge_storage-providers_organizations-storage-providers-update.md)	 - Update storage provider
