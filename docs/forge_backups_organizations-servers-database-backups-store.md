## forge backups organizations-servers-database-backups-store

Create backup configuration

### Synopsis

Create a new backup configuration for the server.

Processing mode: <small><code>async</code></small>

```
forge backups organizations-servers-database-backups-store [flags]
```

### Examples

```
  forge backups organizations-servers-database-backups-store --organization <value> --server 176687 --storage-provider-id 890655 --frequency daily --retention 430741
```

### Options

```
      --body string                 Request body as JSON (alternative to individual flags). Can also be provided via stdin.
  -b, --bucket string               string value
  -c, --cron string                 string value
      --database-ids string         [required]
      --day string                  options: 0, 1, 2, 3, 4, 5, 6
      --directory string            string value
  -f, --frequency string            options: hourly, daily, weekly, custom [required]
  -h, --help                        help for organizations-servers-database-backups-store
      --name string                 string value
      --notification-email string   string value
      --organization string         The organization slug [required]
  -r, --retention int               [required]
      --server int                  The server ID [required]
      --storage-provider-id int     [required]
  -t, --time string                 options: 00:00, 00:30, 01:00, 01:30, 02:00, 02:30, 03:00, 03:30, 04:00, 04:30, 05:00, 05:30, 06:00, 06:30, 07:00, 07:30, 08:00, 08:30, 09:00, 09:30, 10:00, 10:30, 11:00, 11:30, 12:00, 12:30, 13:00, 13:30, 14:00, 14:30, 15:00, 15:30, 16:00, 16:30, 17:00, 17:30, 18:00, 18:30, 19:00, 19:30, 20:00, 20:30, 21:00, 21:30, 22:00, 22:30, 23:00, 23:30
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
      --server-url string      Override the default server URL
      --timeout string         HTTP request timeout (e.g., 30s, 5m, 100ms)
      --usage                  Print the CLI Usage schema in KDL format
```

### SEE ALSO

* [forge backups](forge_backups.md)	 - Operations for backups
