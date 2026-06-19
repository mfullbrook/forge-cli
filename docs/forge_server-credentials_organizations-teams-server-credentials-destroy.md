## forge server-credentials organizations-teams-server-credentials-destroy

Delete a server credential share

### Synopsis

Unshare a server credential with a team.

Processing mode: <small><code>sync</code></small>

```
forge server-credentials organizations-teams-server-credentials-destroy [flags]
```

### Examples

```
  forge server-credentials organizations-teams-server-credentials-destroy --organization <value> --team 543042 --credential 98202
```

### Options

```
  -c, --credential int        The credential ID [required]
  -h, --help                  help for organizations-teams-server-credentials-destroy
      --organization string   The organization slug [required]
  -t, --team int              The team ID [required]
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

* [forge server-credentials](forge_server-credentials.md)	 - Operations for server-credentials
