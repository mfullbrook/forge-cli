## forge scheduled-jobs organizations-servers-sites-scheduled-jobs-store

Create site scheduled job

### Synopsis

Create a specific scheduled job for the site.

Processing mode: <small><code>async</code></small>

```
forge scheduled-jobs organizations-servers-sites-scheduled-jobs-store [flags]
```

### Examples

```
  forge scheduled-jobs organizations-servers-sites-scheduled-jobs-store --organization <value> --server 181290 --site 944759 --command echo $(whoami) --user root
```

### Options

```
      --body string           Request body as JSON (alternative to individual flags). Can also be provided via stdin.
      --command string        The command to run. [required]
      --cron string           The cron expression to use for the scheduled job. Only used if frequency is set to Custom.
  -f, --frequency string      options: minutely, hourly, nightly, weekly, monthly, reboot, custom [required]
  -g, --grace-period string   options: 1, 2, 5, 10, 30, 60
      --heartbeat string      Whether a heartbeat should be created for the scheduled job.
  -h, --help                  help for organizations-servers-sites-scheduled-jobs-store
  -n, --name string           The name of the command.
      --organization string   The organization slug [required]
      --server int            The server ID [required]
      --site int              The site ID [required]
  -u, --user string           The user to run the scheduled job as. [required]
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

* [forge scheduled-jobs](forge_scheduled-jobs.md)	 - Operations for scheduled-jobs
