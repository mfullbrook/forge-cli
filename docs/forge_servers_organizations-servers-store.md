## forge servers organizations-servers-store

Create server

### Synopsis

Create a new server in the organization. Supports both standard cloud providers
and custom VPS configurations.

Processing mode: <small><code>async</code></small>

```
forge servers organizations-servers-store [flags]
```

### Examples

```
  forge servers organizations-servers-store --organization <value> --name <value> --provider <value> --type app --ubuntu-version 22.04
```

### Options

```
      --add-key-to-source-control   boolean flag (default true)
      --akamai string               JSON object
      --aws string                  JSON object
      --body string                 Request body as JSON (alternative to individual flags). Can also be provided via stdin.
      --credential-id int           integer value
      --custom string               JSON object
      --database string             string value
      --database-type string        options: mysql, mysql8, mysql84, mysql9, mariadb, mariadb106, mariadb1011, mariadb114, postgres, postgres13, postgres14, postgres15, postgres16, postgres17, postgres18
  -h, --help                        help for organizations-servers-store
      --hetzner string              JSON object
  -l, --laravel string              JSON object
  -n, --name string                 [required]
      --ocean2 string               JSON object
      --organization string         The organization slug [required]
      --php-version string          options: php5, php56-old, php56, php70, php71, php72, php73, php74, php80, php81, php82, php83, php84, php85
      --provider string             [required]
  -r, --recipe-id string            integer value
      --tags string                 list of values
      --team-id string              integer value
      --type string                 options: app, web, loadbalancer, database, cache, worker, meilisearch, openclaw [required]
  -u, --ubuntu-version string       options: 22.04, 24.04 [required]
  -v, --vultr string                JSON object
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

* [forge servers](forge_servers.md)	 - Operations for servers
