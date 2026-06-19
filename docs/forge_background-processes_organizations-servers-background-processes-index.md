## forge background-processes organizations-servers-background-processes-index

List background processes

### Synopsis

List all background processes on the server.

Processing mode: <small><code>sync</code></small>

```
forge background-processes organizations-servers-background-processes-index [flags]
```

### Examples

```
  forge background-processes organizations-servers-background-processes-index --organization <value> --server 170230
```

### Options

```
      --filter-directory string   The directory that the process is running in.
      --filter-site-id string     The site ID that the process is running for.
      --filter-user string        The user that the process is running as.
  -h, --help                      help for organizations-servers-background-processes-index
      --organization string       The organization slug [required]
      --page-cursor string        The cursor to start the pagination from.
      --page-size int             The number of results that will be returned per page. (default 30)
      --server int                The server ID [required]
      --sort user                 Available sorts are user. You can sort by multiple options by separating them with a comma. To sort in descending order, use `-` sign in front of the sort, for example: `-user`.
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

* [forge background-processes](forge_background-processes.md)	 - Operations for background-processes
