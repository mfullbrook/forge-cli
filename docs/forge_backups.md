## forge backups

Operations for backups

### Synopsis

Operations for backups

```
forge backups [flags]
```

### Options

```
  -h, --help   help for backups
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
* [forge backups organizations-servers-database-backups-destroy](forge_backups_organizations-servers-database-backups-destroy.md)	 - Delete backup configuration
* [forge backups organizations-servers-database-backups-index](forge_backups_organizations-servers-database-backups-index.md)	 - List backup configurations
* [forge backups organizations-servers-database-backups-instances-destroy](forge_backups_organizations-servers-database-backups-instances-destroy.md)	 - Delete backup
* [forge backups organizations-servers-database-backups-instances-index](forge_backups_organizations-servers-database-backups-instances-index.md)	 - List backups
* [forge backups organizations-servers-database-backups-instances-restores-store](forge_backups_organizations-servers-database-backups-instances-restores-store.md)	 - Create a database restore from backup
* [forge backups organizations-servers-database-backups-instances-show](forge_backups_organizations-servers-database-backups-instances-show.md)	 - Get backup
* [forge backups organizations-servers-database-backups-instances-store](forge_backups_organizations-servers-database-backups-instances-store.md)	 - Create backup
* [forge backups organizations-servers-database-backups-show](forge_backups_organizations-servers-database-backups-show.md)	 - Get backup configuration
* [forge backups organizations-servers-database-backups-store](forge_backups_organizations-servers-database-backups-store.md)	 - Create backup configuration
* [forge backups organizations-servers-database-backups-update](forge_backups_organizations-servers-database-backups-update.md)	 - Update backup configuration
