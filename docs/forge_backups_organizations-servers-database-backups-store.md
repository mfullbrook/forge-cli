## forge backups organizations-servers-database-backups-store

Create backup configuration

### Synopsis

Create a new backup configuration for the server.

Processing mode: <small><code>async</code></small>

```
forge backups organizations-servers-database-backups-store [flags]
```

### Examples

```
  forge backups organizations-servers-database-backups-store --organization <value> --server-param 176687 --storage-provider-id 890655 --frequency daily --retention 430741
```

### Options

```
      --body string                 Request body as JSON (alternative to individual flags). Can also be provided via stdin; @path reads a file, @- reads stdin to EOF. Use --schema to print the exact JSON Schema.
  -b, --bucket string               string value
  -c, --cron string                 string value
      --database-ids string         [required]
      --day string                  options: 0, 1, 2, 3, 4, 5, 6
      --directory string            string value
  -f, --frequency string            options: hourly, daily, weekly, custom [required]
  -h, --help                        help for organizations-servers-database-backups-store
      --name string                 string value
      --notification-email string   string value
      --organization string         The organization slug [required]
  -r, --retention int               [required]
      --schema                      Print the exact JSON Schema of the request body and exit
  -s, --server-param int            The server ID [required]
      --storage-provider-id int     [required]
  -t, --time string                 options: 00:00, 00:30, 01:00, 01:30, 02:00, 02:30, 03:00, 03:30, 04:00, 04:30, 05:00, 05:30, 06:00, 06:30, 07:00, 07:30, 08:00, 08:30, 09:00, 09:30, 10:00, 10:30, 11:00, 11:30, 12:00, 12:30, 13:00, 13:30, 14:00, 14:30, 15:00, 15:30, 16:00, 16:30, 17:00, 17:30, 18:00, 18:30, 19:00, 19:30, 20:00, 20:30, 21:00, 21:30, 22:00, 22:30, 23:00, 23:30
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

* [forge backups](forge_backups.md)	 - Operations for backups

### Machine interface

* `forge backups organizations-servers-database-backups-store --usage` — this command's flags, defaults and env vars as machine-readable KDL
* `forge backups organizations-servers-database-backups-store --schema` — the exact JSON Schema of the request body (all `$ref`s bundled)
* `forge backups organizations-servers-database-backups-store --dry-run` — preview the request without OS-keychain access or a network call (human preview on stderr)
* `--dry-run --output-format json` (or a caller-explicit `--jq`) writes one preview object per request as NDJSON on stdout; jq is not applied to previews
* `--output-format json` or `--jq <expr>` for machine-readable live output; in agent mode errors are a JSON envelope on stderr

Exit codes: 0 ok · 1 runtime · 2 usage · 3 authentication/authorization
