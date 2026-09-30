## forge roles

Operations for roles

### Synopsis

Operations for roles

```
forge roles [flags]
```

### Options

```
  -h, --help   help for roles
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
* [forge roles organizations-roles-destroy](forge_roles_organizations-roles-destroy.md)	 - Delete role
* [forge roles organizations-roles-index](forge_roles_organizations-roles-index.md)	 - List roles
* [forge roles organizations-roles-permissions-index](forge_roles_organizations-roles-permissions-index.md)	 - List role permissions
* [forge roles organizations-roles-show](forge_roles_organizations-roles-show.md)	 - Get role
* [forge roles organizations-roles-store](forge_roles_organizations-roles-store.md)	 - Create role
* [forge roles organizations-roles-update](forge_roles_organizations-roles-update.md)	 - Update role
* [forge roles permissions-index](forge_roles_permissions-index.md)	 - List permissions
* [forge roles permissions-show](forge_roles_permissions-show.md)	 - Get permission
* [forge roles predefined-roles-index](forge_roles_predefined-roles-index.md)	 - List predefined roles
* [forge roles predefined-roles-show](forge_roles_predefined-roles-show.md)	 - Get predefined role

Exit codes: 0 ok · 1 runtime · 2 usage · 3 authentication/authorization
