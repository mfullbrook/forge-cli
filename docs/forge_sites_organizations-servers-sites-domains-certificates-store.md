## forge sites organizations-servers-sites-domains-certificates-store

Create domain certificate

### Synopsis

Create a new certificate for a given domain.

Processing mode: <small><code>async</code></small>

```
forge sites organizations-servers-sites-domains-certificates-store [flags]
```

### Examples

```
  forge sites organizations-servers-sites-domains-certificates-store --organization <value> --server 637553 --site 922912 --domain-record 181209 --type letsencrypt
```

### Options

```
      --body string           Request body as JSON (alternative to individual flags). Can also be provided via stdin.
      --clone string          JSON object
      --csr string            The configuration for a CSR (Certificate Signing Request).
      --domain-record int     The domain record ID [required]
      --enable                Whether to enable the certificate upon installation.
      --existing string       The configuration for an existing certificate.
  -h, --help                  help for organizations-servers-sites-domains-certificates-store
  -l, --letsencrypt string    The configuration for a Let's Encrypt certificate.
      --organization string   The organization slug [required]
      --server int            The server ID [required]
      --site int              The site ID [required]
  -t, --type string           The type of certificate to create. (options: letsencrypt, csr, existing, clone) [required]
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

* [forge sites](forge_sites.md)	 - Operations for sites
