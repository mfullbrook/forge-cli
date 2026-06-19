## forge

Forge: Laravel Forge - API Documentation

### Synopsis

Forge: Laravel Forge - API Documentation

```
forge [flags]
```

### Options

```
      --agent-mode             Enable structured errors and default TOON output for AI coding agents. Automatically enabled when a known agent environment is detected (CLAUDE_CODE, CURSOR_AGENT, etc.). Use --agent-mode=false to disable.
      --color string           Control colored output: auto (color when output is a TTY), always, or never. Respects NO_COLOR and FORCE_COLOR env vars. (default "auto")
  -d, --debug                  Log request and response diagnostics to stderr
      --dry-run                Preview the request that would be sent without executing it (output to stderr)
  -H, --header stringArray     Set a custom HTTP request header (format: "Key: Value"). Can be specified multiple times.
  -h, --help                   help for forge
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

* [forge SSH-keys](forge_SSH-keys.md)	 - Operations for SSH-keys
* [forge auth](forge_auth.md)	 - Manage authentication credentials
* [forge background-processes](forge_background-processes.md)	 - Operations for background-processes
* [forge backups](forge_backups.md)	 - Operations for backups
* [forge commands](forge_commands.md)	 - Operations for commands
* [forge configure](forge_configure.md)	 - Configure authentication credentials and preferences
* [forge databases](forge_databases.md)	 - Operations for databases
* [forge deployments](forge_deployments.md)	 - Operations for deployments
* [forge explore](forge_explore.md)	 - Interactively browse and run commands
* [forge firewall-rules](forge_firewall-rules.md)	 - Operations for firewall-rules
* [forge integrations](forge_integrations.md)	 - Operations for integrations
* [forge logs](forge_logs.md)	 - Operations for logs
* [forge monitors](forge_monitors.md)	 - Operations for monitors
* [forge nginx](forge_nginx.md)	 - Operations for nginx
* [forge organizations](forge_organizations.md)	 - Operations for organizations
* [forge providers](forge_providers.md)	 - Operations for providers
* [forge recipes](forge_recipes.md)	 - Operations for recipes
* [forge redirect-rules](forge_redirect-rules.md)	 - Operations for redirect-rules
* [forge roles](forge_roles.md)	 - Operations for roles
* [forge scheduled-jobs](forge_scheduled-jobs.md)	 - Operations for scheduled-jobs
* [forge security-rules](forge_security-rules.md)	 - Operations for security-rules
* [forge server-credentials](forge_server-credentials.md)	 - Operations for server-credentials
* [forge servers](forge_servers.md)	 - Operations for servers
* [forge sites](forge_sites.md)	 - Operations for sites
* [forge storage-providers](forge_storage-providers.md)	 - Operations for storage-providers
* [forge teams](forge_teams.md)	 - Operations for teams
* [forge user](forge_user.md)	 - Operations for user
* [forge version](forge_version.md)	 - Print the CLI version
* [forge whoami](forge_whoami.md)	 - Display current authentication configuration
