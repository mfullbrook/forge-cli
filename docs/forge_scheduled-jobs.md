## forge scheduled-jobs

Operations for scheduled-jobs

### Synopsis

Operations for scheduled-jobs

```
forge scheduled-jobs [flags]
```

### Options

```
  -h, --help   help for scheduled-jobs
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
* [forge scheduled-jobs organizations-servers-scheduled-jobs-destroy](forge_scheduled-jobs_organizations-servers-scheduled-jobs-destroy.md)	 - Delete scheduled job
* [forge scheduled-jobs organizations-servers-scheduled-jobs-index](forge_scheduled-jobs_organizations-servers-scheduled-jobs-index.md)	 - List server scheduled jobs
* [forge scheduled-jobs organizations-servers-scheduled-jobs-outputs-show](forge_scheduled-jobs_organizations-servers-scheduled-jobs-outputs-show.md)	 - Get scheduled job output
* [forge scheduled-jobs organizations-servers-scheduled-jobs-show](forge_scheduled-jobs_organizations-servers-scheduled-jobs-show.md)	 - Get scheduled job
* [forge scheduled-jobs organizations-servers-scheduled-jobs-store](forge_scheduled-jobs_organizations-servers-scheduled-jobs-store.md)	 - Create scheduled job
* [forge scheduled-jobs organizations-servers-sites-scheduled-jobs-destroy](forge_scheduled-jobs_organizations-servers-sites-scheduled-jobs-destroy.md)	 - Delete site scheduled job
* [forge scheduled-jobs organizations-servers-sites-scheduled-jobs-index](forge_scheduled-jobs_organizations-servers-sites-scheduled-jobs-index.md)	 - List site scheduled jobs
* [forge scheduled-jobs organizations-servers-sites-scheduled-jobs-outputs-show](forge_scheduled-jobs_organizations-servers-sites-scheduled-jobs-outputs-show.md)	 - Get site scheduled job output
* [forge scheduled-jobs organizations-servers-sites-scheduled-jobs-show](forge_scheduled-jobs_organizations-servers-sites-scheduled-jobs-show.md)	 - Get site scheduled job
* [forge scheduled-jobs organizations-servers-sites-scheduled-jobs-store](forge_scheduled-jobs_organizations-servers-sites-scheduled-jobs-store.md)	 - Create site scheduled job
