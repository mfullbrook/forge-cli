## forge storage-providers organizations-storage-providers-update

Update storage provider

### Synopsis

Update a storage provider for the organization.

Processing mode: <small><code>async</code></small>

```
forge storage-providers organizations-storage-providers-update [flags]
```

### Examples

```
  forge storage-providers organizations-storage-providers-update --organization <value> --storage-configuration 698133 --name <value> --provider s3
```

### Options

```
      --access-key string           string value
      --assume-role                 boolean flag
      --body string                 Request body as JSON (alternative to individual flags). Can also be provided via stdin.
  -b, --bucket string               string value
      --directory string            string value
  -e, --endpoint string             string value
  -h, --help                        help for organizations-storage-providers-update
  -n, --name string                 [required]
      --organization string         The organization slug [required]
  -p, --provider string             options: s3, spaces, hetzner, ovh, scaleway, custom [required]
  -r, --region string               string value
      --secret-key string           string value
      --storage-configuration int   The storage configuration ID [required]
  -u, --use-ec2-assumed-role        boolean flag
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

* [forge storage-providers](forge_storage-providers.md)	 - Operations for storage-providers
