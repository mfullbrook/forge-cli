## forge integrations organizations-servers-sites-integrations-laravel-maintenance-store

Create Laravel Maintenance integration

### Synopsis

Enable maintenance mode for the site.

Processing mode: <small><code>async</code></small>

```
forge integrations organizations-servers-sites-integrations-laravel-maintenance-store [flags]
```

### Examples

```
  forge integrations organizations-servers-sites-integrations-laravel-maintenance-store --organization <value> --server 696276 --site 480485 --status 304
```

### Options

```
      --body string           Request body as JSON (alternative to individual flags). Can also be provided via stdin.
  -h, --help                  help for organizations-servers-sites-integrations-laravel-maintenance-store
      --organization string   The organization slug [required]
  -r, --redirect string       The redirect URL to which all requests should be sent while in maintenance mode.
      --secret string         The secret phrase that allows access to the application while in maintenance mode.
      --server int            The server ID [required]
      --site int              The site ID [required]
      --status string         options: 304, 307, 410, 503 [required]
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

* [forge integrations](forge_integrations.md)	 - Operations for integrations
