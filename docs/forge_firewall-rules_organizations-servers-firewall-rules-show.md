## forge firewall-rules organizations-servers-firewall-rules-show

Get server firewall rule

### Synopsis

Get a specific firewall rule associated with the server.

Processing mode: <small><code>sync</code></small>

```
forge firewall-rules organizations-servers-firewall-rules-show [flags]
```

### Examples

```
  forge firewall-rules organizations-servers-firewall-rules-show --organization <value> --server 626909 --rule 462429
```

### Options

```
  -h, --help                  help for organizations-servers-firewall-rules-show
      --organization string   The organization slug [required]
  -r, --rule int              The rule ID [required]
  -s, --server int            The server ID [required]
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

* [forge firewall-rules](forge_firewall-rules.md)	 - Operations for firewall-rules
