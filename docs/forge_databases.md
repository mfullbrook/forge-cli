## forge databases

Operations for databases

### Synopsis

Operations for databases

```
forge databases [flags]
```

### Options

```
  -h, --help   help for databases
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
* [forge databases organizations-servers-database-password-update](forge_databases_organizations-servers-database-password-update.md)	 - Update the password for the database
* [forge databases organizations-servers-database-schemas-destroy](forge_databases_organizations-servers-database-schemas-destroy.md)	 - Delete database schema
* [forge databases organizations-servers-database-schemas-index](forge_databases_organizations-servers-database-schemas-index.md)	 - List database schemas
* [forge databases organizations-servers-database-schemas-show](forge_databases_organizations-servers-database-schemas-show.md)	 - Get database schema
* [forge databases organizations-servers-database-schemas-store](forge_databases_organizations-servers-database-schemas-store.md)	 - Create database schema
* [forge databases organizations-servers-database-schemas-synchronizations-store](forge_databases_organizations-servers-database-schemas-synchronizations-store.md)	 - Update database schemas
* [forge databases organizations-servers-database-users-destroy](forge_databases_organizations-servers-database-users-destroy.md)	 - Delete database user
* [forge databases organizations-servers-database-users-index](forge_databases_organizations-servers-database-users-index.md)	 - List database users
* [forge databases organizations-servers-database-users-show](forge_databases_organizations-servers-database-users-show.md)	 - Get database user
* [forge databases organizations-servers-database-users-store](forge_databases_organizations-servers-database-users-store.md)	 - Create database user
* [forge databases organizations-servers-database-users-update](forge_databases_organizations-servers-database-users-update.md)	 - Update database user
