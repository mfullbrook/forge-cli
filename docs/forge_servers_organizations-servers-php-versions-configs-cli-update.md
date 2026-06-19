## forge servers organizations-servers-php-versions-configs-cli-update

Update PHP version CLI config

### Synopsis

Processing mode: <small><code>async</code></small>

```
forge servers organizations-servers-php-versions-configs-cli-update [flags]
```

### Examples

```
  forge servers organizations-servers-php-versions-configs-cli-update --organization <value> --server 121987 --php-version 680535 --config-param <value>
```

### Options

```
      --body string           Request body as JSON (alternative to individual flags). Can also be provided via stdin.
  -c, --config-param string   [required]
  -h, --help                  help for organizations-servers-php-versions-configs-cli-update
      --organization string   The organization slug [required]
  -p, --php-version int       The php version ID [required]
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

* [forge servers](forge_servers.md)	 - Operations for servers
