## forge sites organizations-servers-sites-heartbeats-update

Update heartbeat

### Synopsis

Update a specific heartbeat for the site.

Processing mode: <small><code>sync</code></small>

```
forge sites organizations-servers-sites-heartbeats-update [flags]
```

### Examples

```
  forge sites organizations-servers-sites-heartbeats-update --organization <value> --server 12665 --site 354926 --heartbeat 178389 --name My Heartbeat
```

### Options

```
      --body string               Request body as JSON (alternative to individual flags). Can also be provided via stdin.
  -c, --custom-frequency string   A cron expression representing the custom frequency at which the client is expected to send a ping, if the frequency is set to -1.
  -f, --frequency string          options: 1, 5, 10, 30, 60, 1440, 10080, 312480, -1 [required]
  -g, --grace-period string       options: 1, 2, 5, 10, 30, 60 [required]
      --heartbeat int             The heartbeat ID [required]
  -h, --help                      help for organizations-servers-sites-heartbeats-update
  -n, --name string               The name of the heartbeat. [required]
      --organization string       The organization slug [required]
      --server int                The server ID [required]
      --site int                  The site ID [required]
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

* [forge sites](forge_sites.md)	 - Operations for sites
