## forge security-rules organizations-servers-sites-security-rules-index

List site security rules

### Synopsis

List all security rules associated with the site.

Processing mode: <small><code>sync</code></small>

```
forge security-rules organizations-servers-sites-security-rules-index [flags]
```

### Examples

```
  forge security-rules organizations-servers-sites-security-rules-index --organization <value> --server 863470 --site 589556
```

### Options

```
      --filter-path string     The path for the security rule.
      --filter-status string   The status of the security rule.
  -h, --help                   help for organizations-servers-sites-security-rules-index
      --organization string    The organization slug [required]
      --page-cursor string     The cursor to start the pagination from.
      --page-size int          The number of results that will be returned per page. (default 30)
      --server int             The server ID [required]
      --site int               The site ID [required]
      --sort path              Available sorts are path, `status`, `created_at`, `updated_at`. You can sort by multiple options by separating them with a comma. To sort in descending order, use `-` sign in front of the sort, for example: `-path`.
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

* [forge security-rules](forge_security-rules.md)	 - Operations for security-rules
