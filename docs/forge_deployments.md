## forge deployments

Operations for deployments

### Synopsis

Operations for deployments

```
forge deployments [flags]
```

### Options

```
  -h, --help   help for deployments
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
* [forge deployments organizations-servers-sites-deploy-key-destroy](forge_deployments_organizations-servers-sites-deploy-key-destroy.md)	 - Delete deploy key
* [forge deployments organizations-servers-sites-deploy-key-show](forge_deployments_organizations-servers-sites-deploy-key-show.md)	 - Get deploy key
* [forge deployments organizations-servers-sites-deploy-key-store](forge_deployments_organizations-servers-sites-deploy-key-store.md)	 - Create deploy key
* [forge deployments organizations-servers-sites-deployments-deploy-hook-show](forge_deployments_organizations-servers-sites-deployments-deploy-hook-show.md)	 - Get the deployment trigger URL
* [forge deployments organizations-servers-sites-deployments-deploy-hook-update](forge_deployments_organizations-servers-sites-deployments-deploy-hook-update.md)	 - Update deployment trigger URL
* [forge deployments organizations-servers-sites-deployments-index](forge_deployments_organizations-servers-sites-deployments-index.md)	 - List deployments
* [forge deployments organizations-servers-sites-deployments-log-show](forge_deployments_organizations-servers-sites-deployments-log-show.md)	 - Get deployment output
* [forge deployments organizations-servers-sites-deployments-push-to-deploy-destroy](forge_deployments_organizations-servers-sites-deployments-push-to-deploy-destroy.md)	 - Delete push to deploy configuration
* [forge deployments organizations-servers-sites-deployments-push-to-deploy-store](forge_deployments_organizations-servers-sites-deployments-push-to-deploy-store.md)	 - Create push to deploy configuration
* [forge deployments organizations-servers-sites-deployments-script-show](forge_deployments_organizations-servers-sites-deployments-script-show.md)	 - Get deployment script
* [forge deployments organizations-servers-sites-deployments-script-update](forge_deployments_organizations-servers-sites-deployments-script-update.md)	 - Update deployment script
* [forge deployments organizations-servers-sites-deployments-show](forge_deployments_organizations-servers-sites-deployments-show.md)	 - Get deployment
* [forge deployments organizations-servers-sites-deployments-status-destroy](forge_deployments_organizations-servers-sites-deployments-status-destroy.md)	 - Update deployment state
* [forge deployments organizations-servers-sites-deployments-status-show](forge_deployments_organizations-servers-sites-deployments-status-show.md)	 - Get deployment status
* [forge deployments organizations-servers-sites-deployments-store](forge_deployments_organizations-servers-sites-deployments-store.md)	 - Create deployment
* [forge deployments organizations-servers-sites-webhooks-destroy](forge_deployments_organizations-servers-sites-webhooks-destroy.md)	 - Delete site webhook
* [forge deployments organizations-servers-sites-webhooks-index](forge_deployments_organizations-servers-sites-webhooks-index.md)	 - List site webhooks
* [forge deployments organizations-servers-sites-webhooks-show](forge_deployments_organizations-servers-sites-webhooks-show.md)	 - Get site webhook
* [forge deployments organizations-servers-sites-webhooks-store](forge_deployments_organizations-servers-sites-webhooks-store.md)	 - Create site webhook
