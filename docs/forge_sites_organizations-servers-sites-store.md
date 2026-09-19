## forge sites organizations-servers-sites-store

Create site

### Synopsis

Add a new site to the server.

Processing mode: <small><code>async</code></small>

```
forge sites organizations-servers-sites-store [flags]
```

### Examples

```
  forge sites organizations-servers-sites-store --organization <value> --server-param 343266 --type phpmyadmin
```

### Options

```
  -a, --allow-wildcard-subdomains             Whether to allow wildcard subdomains for the domain.
      --body string                           Request body as JSON (alternative to individual flags). Can also be provided via stdin; @path reads a file, @- reads stdin to EOF. Use --schema to print the exact JSON Schema.
  -b, --branch string                         string value
      --database-id int                       The ID of the database to use with the site.
      --database-user-id int                  The ID of the database user to use with the site.
      --domain-mode string                    JSON value (one of: string | CreateSiteDomainMode)
      --frontend-build-command string         The build command for frontend assets.
      --frontend-package-manager string       The package manager for frontend applications.
  -g, --generate-deploy-key                   boolean flag
  -h, --help                                  help for organizations-servers-sites-store
      --install-composer-dependencies         boolean flag
      --is-isolated                           boolean flag
      --isolated-user string                  string value
      --name string                           string value
      --nginx-template-id int                 integer value
      --nuxt-next-mode string                 The render mode for Next/Nuxt applications.
      --nuxt-next-port int                    The port used for Next/Nuxt applications.
      --organization string                   The organization slug [required]
      --php-version string                    options: php5, php56-old, php56, php70, php71, php72, php73, php74, php80, php81, php82, php83, php84, php85
      --private-deploy-key string             string value
      --public-deploy-key string              string value
      --push-to-deploy                        Automatically trigger a new deployment when changes are pushed to the environment's Git branch.
      --repository string                     string value
      --root-directory string                 string value
      --schema                                Print the exact JSON Schema of the request body and exit
      --server-param int                      The server ID [required]
      --shared-paths string                   A list of files or directories to be shared between releases for zero-downtime deployments.
      --source-control-provider string        All supported source control providers.
                                               (options: github, gitlab, bitbucket, gitlab-custom, custom)
      --source-control-provider-id string     integer value
      --statamic-setup string                 The type of setup for Statmic apps.
      --statamic-starter-kit string           The starter kit for the Statamic app.
      --statamic-super-user-email string      string value
      --statamic-super-user-password string   string value
      --tags string                           list of values
      --type string                           options: laravel, symfony, statamic, wordpress, phpmyadmin, php, nextjs, nuxtjs, static-html, other, custom [required]
      --web-directory string                  string value
      --www-redirect-type string              options: from-www, to-www, none
  -z, --zero-downtime-deployments             boolean flag
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

* [forge sites](forge_sites.md)	 - Operations for sites

### Machine interface

* `forge sites organizations-servers-sites-store --usage` — this command's flags, defaults and env vars as machine-readable KDL
* `forge sites organizations-servers-sites-store --schema` — the exact JSON Schema of the request body (all `$ref`s bundled)
* `forge sites organizations-servers-sites-store --dry-run` — preview the request without OS-keychain access or a network call (human preview on stderr)
* `--dry-run --output-format json` (or a caller-explicit `--jq`) writes one preview object per request as NDJSON on stdout; jq is not applied to previews
* `--output-format json` or `--jq <expr>` for machine-readable live output; in agent mode errors are a JSON envelope on stderr

Exit codes: 0 ok · 1 runtime · 2 usage · 3 authentication/authorization
