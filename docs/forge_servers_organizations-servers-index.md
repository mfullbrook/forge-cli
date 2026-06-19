## forge servers organizations-servers-index

List servers

### Synopsis

Show all servers for the organization.

Processing mode: <small><code>sync</code></small>

```
forge servers organizations-servers-index [flags]
```

### Examples

```
  forge servers organizations-servers-index --organization <value>
```

### Options

```
      --filter-database-type string    The database type of the server.
      --filter-ip-address string       The IP address of the server.
      --filter-name string             The name of the server.
      --filter-php-version string      The PHP version of the server.
      --filter-provider string         The provider of the server.
      --filter-region string           The region where the server is located.
      --filter-size string             The size of the server.
      --filter-ubuntu-version string   The Ubuntu version of the server.
  -h, --help                           help for organizations-servers-index
      --organization string            The organization slug [required]
      --page-cursor string             The cursor to start the pagination from.
      --page-size int                  The number of results that will be returned per page. (default 30)
  -s, --sort name                      Available sorts are name, `provider`, `ubuntu_version`, `region`, `php_version`, `created_at`, `updated_at`. You can sort by multiple options by separating them with a comma. To sort in descending order, use `-` sign in front of the sort, for example: `-name`.
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
