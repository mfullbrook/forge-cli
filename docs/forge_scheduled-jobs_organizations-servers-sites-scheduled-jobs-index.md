## forge scheduled-jobs organizations-servers-sites-scheduled-jobs-index

List site scheduled jobs

### Synopsis

List all scheduled jobs associated with the site.

Processing mode: <small><code>sync</code></small>

```
forge scheduled-jobs organizations-servers-sites-scheduled-jobs-index [flags]
```

### Examples

```
  forge scheduled-jobs organizations-servers-sites-scheduled-jobs-index --organization <value> --server 374166 --site 637674
```

### Options

```
      --filter-status string   string value
      --filter-user string     string value
  -h, --help                   help for organizations-servers-sites-scheduled-jobs-index
      --organization string    The organization slug [required]
      --page-cursor string     The cursor to start the pagination from.
      --page-size int          The number of results that will be returned per page. (default 30)
      --server int             The server ID [required]
      --site int               The site ID [required]
      --sort created_at        Available sorts are created_at, `updated_at`, `status`. You can sort by multiple options by separating them with a comma. To sort in descending order, use `-` sign in front of the sort, for example: `-created_at`.
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

* [forge scheduled-jobs](forge_scheduled-jobs.md)	 - Operations for scheduled-jobs
