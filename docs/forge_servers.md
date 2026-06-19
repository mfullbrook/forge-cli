## forge servers

Operations for servers

### Synopsis

Operations for servers

```
forge servers [flags]
```

### Options

```
  -h, --help   help for servers
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

* [forge](forge.md)	 - Forge: Laravel Forge - API Documentation
* [forge servers organizations-servers-actions-store](forge_servers_organizations-servers-actions-store.md)	 - Create server action
* [forge servers organizations-servers-archives-destroy](forge_servers_organizations-servers-archives-destroy.md)	 - Delete archived server
* [forge servers organizations-servers-archives-index](forge_servers_organizations-servers-archives-index.md)	 - List archived servers
* [forge servers organizations-servers-archives-store](forge_servers_organizations-servers-archives-store.md)	 - Create an archived server
* [forge servers organizations-servers-background-processes-actions-store](forge_servers_organizations-servers-background-processes-actions-store.md)	 - Perform an action on a server background process
* [forge servers organizations-servers-destroy](forge_servers_organizations-servers-destroy.md)	 - Delete server
* [forge servers organizations-servers-events-index](forge_servers_organizations-servers-events-index.md)	 - List server events
* [forge servers organizations-servers-events-output-show](forge_servers_organizations-servers-events-output-show.md)	 - Get server event output
* [forge servers organizations-servers-events-show](forge_servers_organizations-servers-events-show.md)	 - Get server event
* [forge servers organizations-servers-index](forge_servers_organizations-servers-index.md)	 - List servers
* [forge servers organizations-servers-network-show](forge_servers_organizations-servers-network-show.md)	 - Get server network
* [forge servers organizations-servers-network-update](forge_servers_organizations-servers-network-update.md)	 - Update server network
* [forge servers organizations-servers-php-cli-version-show](forge_servers_organizations-servers-php-cli-version-show.md)	 - Get PHP CLI version
* [forge servers organizations-servers-php-cli-version-update](forge_servers_organizations-servers-php-cli-version-update.md)	 - Update PHP CLI version
* [forge servers organizations-servers-php-max-execution-time-show](forge_servers_organizations-servers-php-max-execution-time-show.md)	 - Get server PHP max execution time
* [forge servers organizations-servers-php-max-execution-time-update](forge_servers_organizations-servers-php-max-execution-time-update.md)	 - Update server PHP max execution time
* [forge servers organizations-servers-php-max-upload-size-show](forge_servers_organizations-servers-php-max-upload-size-show.md)	 - Get server PHP max upload size
* [forge servers organizations-servers-php-max-upload-size-update](forge_servers_organizations-servers-php-max-upload-size-update.md)	 - Update server PHP max upload size
* [forge servers organizations-servers-php-opcache-destroy](forge_servers_organizations-servers-php-opcache-destroy.md)	 - Delete PHP OPcache config
* [forge servers organizations-servers-php-opcache-show](forge_servers_organizations-servers-php-opcache-show.md)	 - Get server PHP OPcache status
* [forge servers organizations-servers-php-opcache-store](forge_servers_organizations-servers-php-opcache-store.md)	 - Create PHP OPcache config
* [forge servers organizations-servers-php-site-version-show](forge_servers_organizations-servers-php-site-version-show.md)	 - Get PHP site version
* [forge servers organizations-servers-php-site-version-update](forge_servers_organizations-servers-php-site-version-update.md)	 - Update PHP site version
* [forge servers organizations-servers-php-versions-configs-cli-show](forge_servers_organizations-servers-php-versions-configs-cli-show.md)	 - Get PHP version CLI config
* [forge servers organizations-servers-php-versions-configs-cli-update](forge_servers_organizations-servers-php-versions-configs-cli-update.md)	 - Update PHP version CLI config
* [forge servers organizations-servers-php-versions-configs-fpm-show](forge_servers_organizations-servers-php-versions-configs-fpm-show.md)	 - Get PHP version FPM config
* [forge servers organizations-servers-php-versions-configs-fpm-update](forge_servers_organizations-servers-php-versions-configs-fpm-update.md)	 - Update PHP version FPM config
* [forge servers organizations-servers-php-versions-configs-pool-show](forge_servers_organizations-servers-php-versions-configs-pool-show.md)	 - Get PHP version pool config
* [forge servers organizations-servers-php-versions-configs-pool-update](forge_servers_organizations-servers-php-versions-configs-pool-update.md)	 - Update PHP version pool config
* [forge servers organizations-servers-php-versions-destroy](forge_servers_organizations-servers-php-versions-destroy.md)	 - Delete installed PHP version
* [forge servers organizations-servers-php-versions-index](forge_servers_organizations-servers-php-versions-index.md)	 - List PHP versions for server
* [forge servers organizations-servers-php-versions-show](forge_servers_organizations-servers-php-versions-show.md)	 - Get PHP version
* [forge servers organizations-servers-php-versions-store](forge_servers_organizations-servers-php-versions-store.md)	 - Install new PHP version
* [forge servers organizations-servers-php-versions-update](forge_servers_organizations-servers-php-versions-update.md)	 - Update installed PHP version
* [forge servers organizations-servers-services-mysql-actions-store](forge_servers_organizations-servers-services-mysql-actions-store.md)	 - Perform MySQL action
* [forge servers organizations-servers-services-nginx-actions-store](forge_servers_organizations-servers-services-nginx-actions-store.md)	 - Perform Nginx action
* [forge servers organizations-servers-services-php-actions-store](forge_servers_organizations-servers-services-php-actions-store.md)	 - Perform PHP action
* [forge servers organizations-servers-services-postgres-actions-store](forge_servers_organizations-servers-services-postgres-actions-store.md)	 - Perform Postgres action
* [forge servers organizations-servers-services-redis-actions-store](forge_servers_organizations-servers-services-redis-actions-store.md)	 - Perform Redis action
* [forge servers organizations-servers-services-supervisor-actions-store](forge_servers_organizations-servers-services-supervisor-actions-store.md)	 - Perform Supervisor action
* [forge servers organizations-servers-show](forge_servers_organizations-servers-show.md)	 - Get server
* [forge servers organizations-servers-store](forge_servers_organizations-servers-store.md)	 - Create server
* [forge servers organizations-servers-update](forge_servers_organizations-servers-update.md)	 - Update server
* [forge servers organizations-teams-servers-destroy](forge_servers_organizations-teams-servers-destroy.md)	 - Delete a server share
* [forge servers organizations-teams-servers-index](forge_servers_organizations-teams-servers-index.md)	 - List team servers
* [forge servers organizations-teams-servers-store](forge_servers_organizations-teams-servers-store.md)	 - Create a new server share
