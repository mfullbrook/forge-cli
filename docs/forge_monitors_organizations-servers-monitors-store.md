## forge monitors organizations-servers-monitors-store

Create server monitor

### Synopsis

Add a new monitor to the server.

Processing mode: <small><code>async</code></small>

```
forge monitors organizations-servers-monitors-store [flags]
```

### Examples

```
  forge monitors organizations-servers-monitors-store --organization <value> --server 555618 --type free_memory --operator gte --threshold 90
```

### Options

```
      --body string           Request body as JSON (alternative to individual flags). Can also be provided via stdin.
  -h, --help                  help for organizations-servers-monitors-store
  -m, --minutes int           The frequency in minutes to evaluate the monitor.
  -n, --notify string         The email address to notify when the monitor is in an alert state. [required]
      --operator string       options: gte, lte [required]
      --organization string   The organization slug [required]
  -s, --server int            The server ID [required]
      --threshold float       The threshold to alert on once breached. [required]
      --type string           options: cpu_load, disk, free_memory, used_memory [required]
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

* [forge monitors](forge_monitors.md)	 - Operations for monitors
