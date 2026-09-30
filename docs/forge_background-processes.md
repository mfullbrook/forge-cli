## forge background-processes

Operations for background-processes

### Synopsis

Operations for background-processes

```
forge background-processes [flags]
```

### Options

```
  -h, --help   help for background-processes
```

### Options inherited from parent commands

```
      --agent-mode             Enable structured errors and default TOON output for AI coding agents. Automatically enabled when a known agent environment is detected (CLAUDECODE, CURSOR_AGENT, etc.). Use --agent-mode=false to disable.
      --color string           Control colored output: auto (color when output is a TTY), always, or never. Respects NO_COLOR and FORCE_COLOR env vars. (default "auto")
  -d, --debug                  Log request and response diagnostics to stderr
      --dry-run                Preview API requests without sending them (no network, no OS keychain). Human preview on stderr; with -o json or --jq, one JSON object per request on stdout. Local mutation commands (auth login, auth logout and configure) make no request: they skip prompts and writes and report a no-op (stderr, or one JSON object on stdout in the machine form)
  -H, --header stringArray     Set a custom HTTP request header (format: "Key: Value"). Can be specified multiple times.
      --http string            HTTP Bearer
      --include-headers        Include HTTP response headers in the output
      --interactive            Prompt for missing inputs and open guided configure/auth forms (forms fall back to line prompts on stdin off-TTY) (default true)
  -q, --jq string              Filter and transform output using a jq expression (e.g., '.name', '.items[] | .id')
      --no-interactive         Disable all interactive features (auto-prompting, explorer auto-launch, TUI forms)
      --oauth2 string          OAuth2 Authorization
  -o, --output-format string   Specify the output format. Options: pretty, json, yaml, table, toon. (default "pretty")
      --raw-output             Write --jq string results as raw text instead of JSON strings (like jq -r); non-string results stay JSON
      --server string          Select a server by index (for indexed servers) or name (for named servers)
      --server-url string      Override the default server URL
      --timeout string         HTTP request timeout (e.g., 30s, 5m, 100ms)
      --usage                  Print the CLI Usage schema in KDL format
```

### SEE ALSO

* [forge](forge.md)	 - Forge: Laravel Forge - API Documentation
* [forge background-processes organizations-servers-background-processes-destroy](forge_background-processes_organizations-servers-background-processes-destroy.md)	 - Delete background process
* [forge background-processes organizations-servers-background-processes-index](forge_background-processes_organizations-servers-background-processes-index.md)	 - List background processes
* [forge background-processes organizations-servers-background-processes-log-show](forge_background-processes_organizations-servers-background-processes-log-show.md)	 - Get background process log
* [forge background-processes organizations-servers-background-processes-show](forge_background-processes_organizations-servers-background-processes-show.md)	 - Get background process
* [forge background-processes organizations-servers-background-processes-store](forge_background-processes_organizations-servers-background-processes-store.md)	 - Create background process
* [forge background-processes organizations-servers-background-processes-update](forge_background-processes_organizations-servers-background-processes-update.md)	 - Update background process

Exit codes: 0 ok · 1 runtime · 2 usage · 3 authentication/authorization
