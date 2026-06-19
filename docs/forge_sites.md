## forge sites

Operations for sites

### Synopsis

Operations for sites

```
forge sites [flags]
```

### Options

```
  -h, --help   help for sites
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
* [forge sites index](forge_sites_index.md)	 - List sites
* [forge sites organizations-servers-sites-certificates-index](forge_sites_organizations-servers-sites-certificates-index.md)	 - List site certificates
* [forge sites organizations-servers-sites-composer-credentials-destroy](forge_sites_organizations-servers-sites-composer-credentials-destroy.md)	 - Delete composer credentials for the site
* [forge sites organizations-servers-sites-composer-credentials-index](forge_sites_organizations-servers-sites-composer-credentials-index.md)	 - Get composer credentials for the site
* [forge sites organizations-servers-sites-composer-credentials-show](forge_sites_organizations-servers-sites-composer-credentials-show.md)	 - Get composer credential for the site
* [forge sites organizations-servers-sites-composer-credentials-store](forge_sites_organizations-servers-sites-composer-credentials-store.md)	 - Create composer credentials for the site
* [forge sites organizations-servers-sites-composer-credentials-update](forge_sites_organizations-servers-sites-composer-credentials-update.md)	 - Update composer credentials for the site
* [forge sites organizations-servers-sites-destroy](forge_sites_organizations-servers-sites-destroy.md)	 - Delete site
* [forge sites organizations-servers-sites-domains-actions-store](forge_sites_organizations-servers-sites-domains-actions-store.md)	 - Create domain action
* [forge sites organizations-servers-sites-domains-certificate-show](forge_sites_organizations-servers-sites-domains-certificate-show.md)	 - Get active domain certificate
* [forge sites organizations-servers-sites-domains-certificates-actions-store](forge_sites_organizations-servers-sites-domains-certificates-actions-store.md)	 - Create domain certificate action
* [forge sites organizations-servers-sites-domains-certificates-active](forge_sites_organizations-servers-sites-domains-certificates-active.md)	 - Get active domain certificate
* [forge sites organizations-servers-sites-domains-certificates-destroy](forge_sites_organizations-servers-sites-domains-certificates-destroy.md)	 - Delete domain certificate
* [forge sites organizations-servers-sites-domains-certificates-index](forge_sites_organizations-servers-sites-domains-certificates-index.md)	 - List domain certificates
* [forge sites organizations-servers-sites-domains-certificates-show](forge_sites_organizations-servers-sites-domains-certificates-show.md)	 - Get domain certificate
* [forge sites organizations-servers-sites-domains-certificates-store](forge_sites_organizations-servers-sites-domains-certificates-store.md)	 - Create domain certificate
* [forge sites organizations-servers-sites-domains-configurations](forge_sites_organizations-servers-sites-domains-configurations.md)	 - Get domain DNS configuration
* [forge sites organizations-servers-sites-domains-destroy](forge_sites_organizations-servers-sites-domains-destroy.md)	 - Delete domain
* [forge sites organizations-servers-sites-domains-index](forge_sites_organizations-servers-sites-domains-index.md)	 - List domains
* [forge sites organizations-servers-sites-domains-nginx-show](forge_sites_organizations-servers-sites-domains-nginx-show.md)	 - Get domain Nginx configuration
* [forge sites organizations-servers-sites-domains-nginx-update](forge_sites_organizations-servers-sites-domains-nginx-update.md)	 - Update domain Nginx configuration
* [forge sites organizations-servers-sites-domains-show](forge_sites_organizations-servers-sites-domains-show.md)	 - Get domain
* [forge sites organizations-servers-sites-domains-store](forge_sites_organizations-servers-sites-domains-store.md)	 - Create domain
* [forge sites organizations-servers-sites-domains-update](forge_sites_organizations-servers-sites-domains-update.md)	 - Update domain
* [forge sites organizations-servers-sites-environment-show](forge_sites_organizations-servers-sites-environment-show.md)	 - Get .env content
* [forge sites organizations-servers-sites-environment-update](forge_sites_organizations-servers-sites-environment-update.md)	 - Update .env content
* [forge sites organizations-servers-sites-healthcheck-show](forge_sites_organizations-servers-sites-healthcheck-show.md)	 - Get healthcheck endpoint
* [forge sites organizations-servers-sites-healthcheck-update](forge_sites_organizations-servers-sites-healthcheck-update.md)	 - Update healthcheck endpoint
* [forge sites organizations-servers-sites-heartbeats-destroy](forge_sites_organizations-servers-sites-heartbeats-destroy.md)	 - Delete heartbeat
* [forge sites organizations-servers-sites-heartbeats-index](forge_sites_organizations-servers-sites-heartbeats-index.md)	 - List heartbeats
* [forge sites organizations-servers-sites-heartbeats-show](forge_sites_organizations-servers-sites-heartbeats-show.md)	 - Get heartbeat
* [forge sites organizations-servers-sites-heartbeats-store](forge_sites_organizations-servers-sites-heartbeats-store.md)	 - Create heartbeat
* [forge sites organizations-servers-sites-heartbeats-update](forge_sites_organizations-servers-sites-heartbeats-update.md)	 - Update heartbeat
* [forge sites organizations-servers-sites-index](forge_sites_organizations-servers-sites-index.md)	 - List sites for server
* [forge sites organizations-servers-sites-load-balancing-nodes-index](forge_sites_organizations-servers-sites-load-balancing-nodes-index.md)	 - List load balancing nodes
* [forge sites organizations-servers-sites-load-balancing-nodes-update](forge_sites_organizations-servers-sites-load-balancing-nodes-update.md)	 - Update load balancing nodes
* [forge sites organizations-servers-sites-logs-application-destroy](forge_sites_organizations-servers-sites-logs-application-destroy.md)	 - Delete site log content
* [forge sites organizations-servers-sites-logs-application-show](forge_sites_organizations-servers-sites-logs-application-show.md)	 - Get site log content
* [forge sites organizations-servers-sites-logs-nginx-access-destroy](forge_sites_organizations-servers-sites-logs-nginx-access-destroy.md)	 - Delete Nginx access log content
* [forge sites organizations-servers-sites-logs-nginx-access-show](forge_sites_organizations-servers-sites-logs-nginx-access-show.md)	 - Get Nginx access log content
* [forge sites organizations-servers-sites-logs-nginx-error-destroy](forge_sites_organizations-servers-sites-logs-nginx-error-destroy.md)	 - Delete Nginx error log content
* [forge sites organizations-servers-sites-logs-nginx-error-show](forge_sites_organizations-servers-sites-logs-nginx-error-show.md)	 - Get Nginx error log content
* [forge sites organizations-servers-sites-nginx-show](forge_sites_organizations-servers-sites-nginx-show.md)	 - Get Nginx configuration
* [forge sites organizations-servers-sites-nginx-update](forge_sites_organizations-servers-sites-nginx-update.md)	 - Update Nginx configuration
* [forge sites organizations-servers-sites-npm-credentials-destroy](forge_sites_organizations-servers-sites-npm-credentials-destroy.md)	 - Delete npm credentials for the site
* [forge sites organizations-servers-sites-npm-credentials-index](forge_sites_organizations-servers-sites-npm-credentials-index.md)	 - Get NPM credentials for the site
* [forge sites organizations-servers-sites-npm-credentials-show](forge_sites_organizations-servers-sites-npm-credentials-show.md)	 - Get NPM credential for the site
* [forge sites organizations-servers-sites-npm-credentials-store](forge_sites_organizations-servers-sites-npm-credentials-store.md)	 - Create NPM credentials for the site
* [forge sites organizations-servers-sites-npm-credentials-update](forge_sites_organizations-servers-sites-npm-credentials-update.md)	 - Update NPM credentials for the site
* [forge sites organizations-servers-sites-store](forge_sites_organizations-servers-sites-store.md)	 - Create site
* [forge sites organizations-servers-sites-store-on-balancer](forge_sites_organizations-servers-sites-store-on-balancer.md)	 - Create site on a load balancer
* [forge sites organizations-servers-sites-update](forge_sites_organizations-servers-sites-update.md)	 - Update site
* [forge sites organizations-sites-index](forge_sites_organizations-sites-index.md)	 - List sites for Organization
* [forge sites organizations-sites-show](forge_sites_organizations-sites-show.md)	 - Get site
