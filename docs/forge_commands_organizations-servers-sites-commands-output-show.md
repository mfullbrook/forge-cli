## forge commands organizations-servers-sites-commands-output-show

Get command output

### Synopsis

Get the output of a specific command run.

Processing mode: <small><code>sync</code></small>

```
forge commands organizations-servers-sites-commands-output-show [flags]
```

### Examples

```
  forge commands organizations-servers-sites-commands-output-show --organization <value> --server 23007 --site 629434 --command 794687
```

### Options

```
  -c, --command int           The command ID [required]
  -h, --help                  help for organizations-servers-sites-commands-output-show
      --organization string   The organization slug [required]
      --server int            The server ID [required]
      --site int              The site ID [required]
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

* [forge commands](forge_commands.md)	 - Operations for commands
