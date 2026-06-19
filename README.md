# forge

Command-line interface for the *Forge* API.

[![Built by Speakeasy](https://img.shields.io/badge/Built_by-SPEAKEASY-374151?style=for-the-badge&labelColor=f3f4f6)](https://www.speakeasy.com/?utm_source=github-com/mfullbrook/forge-cli&utm_campaign=cli)
[![License: MIT](https://img.shields.io/badge/LICENSE_//_MIT-3b5bdb?style=for-the-badge&labelColor=eff6ff)](https://opensource.org/licenses/MIT)


<br /><br />
> [!IMPORTANT]
> This CLI is not yet ready for production use. To complete setup please follow the steps outlined in your [workspace](https://app.speakeasy.com/org/kaira-ventures/dev). Delete this section before > publishing to a package manager.

<!-- Start Summary [summary] -->
## Summary

Forge: Laravel Forge - API Documentation
<!-- End Summary [summary] -->

<!-- Start Table of Contents [toc] -->
## Table of Contents
<!-- $toc-max-depth=2 -->
* [forge](#forge)
  * [CLI Installation](#cli-installation)
  * [Shell Completion](#shell-completion)
  * [CLI Example Usage](#cli-example-usage)
  * [Authentication](#authentication)
  * [Available Commands](#available-commands)
  * [Request Body Input](#request-body-input)
  * [Server Selection](#server-selection)
  * [Output Formats](#output-formats)
  * [Error Handling](#error-handling)
  * [Diagnostics](#diagnostics)
* [Development](#development)
  * [Maturity](#maturity)
  * [Contributions](#contributions)

<!-- End Table of Contents [toc] -->

<!-- Start CLI Installation [installation] -->
## CLI Installation

### Quick Install (Linux/macOS)

```bash
curl -fsSL https://raw.githubusercontent.com/mfullbrook/forge-cli/main/scripts/install.sh | bash
```

### Quick Install (Windows PowerShell)

```powershell
iwr -useb https://raw.githubusercontent.com/mfullbrook/forge-cli/main/scripts/install.ps1 | iex
```

### Go Install

Alternatively, install directly via Go:

```bash
go install github.com/mfullbrook/forge-cli/cmd/forge@latest
```

### Manual Download

Download pre-built binaries for your platform from the [releases page](https://github.com/mfullbrook/forge-cli/releases).
<!-- End CLI Installation [installation] -->

<!-- Start Shell Completion [completion] -->
## Shell Completion

Shell completions are available for Bash, Zsh, Fish, and PowerShell.

### Bash

```bash
# Add to ~/.bashrc:
source <(forge completion bash)

# Or install permanently:
forge completion bash > /etc/bash_completion.d/forge
```

### Zsh

```zsh
# Add to ~/.zshrc:
source <(forge completion zsh)

# Or install permanently:
forge completion zsh > "${fpath[1]}/_forge"
```

### Fish

```fish
forge completion fish | source

# Or install permanently:
forge completion fish > ~/.config/fish/completions/forge.fish
```

### PowerShell

```powershell
forge completion powershell | Out-String | Invoke-Expression
```
<!-- End Shell Completion [completion] -->

<!-- Start CLI Example Usage [usage] -->
## CLI Example Usage

### Example

```bash
forge background-processes organizations-servers-background-processes-index --http 'Bearer test_token' --organization '<value>' --server 170230 --page-size 30 --filter-user forge --filter-site-id 1 --filter-directory /home/forge/forge.laravel.com

```
<!-- End CLI Example Usage [usage] -->

<!-- Start Authentication [security] -->
## Authentication

Authentication credentials can be configured in four ways (in order of priority):

### 1. Command-line flags

Pass credentials directly as flags to any command:

```bash
forge --http <value> --oauth2 <value> <command> [arguments]
```

### 2. Environment variables

Set credentials via environment variables:

| Variable | Description |
|----------|-------------|
| `FORGE_HTTP` | HTTP Bearer |
| `FORGE_OAUTH2` | OAuth2 Authorization |

### 3. OS Keychain (recommended for workstations)

Credentials are stored securely in your operating system's keychain when you run:

```bash
forge configure
```

Secret credentials (tokens, API keys, passwords) are automatically stored in:
- **macOS**: Keychain
- **Linux**: GNOME Keyring / KWallet (via D-Bus Secret Service)
- **Windows**: Windows Credential Locker

If no keychain is available (e.g., in CI environments), credentials fall back to the config file.

### 4. Configuration file

Run the interactive `configure` command to store non-secret settings:

```bash
forge configure
```

Configuration is stored in `~/.config/forge/config.yaml`.
<!-- End Authentication [security] -->

<!-- Start Available Commands [operations] -->
## Available Commands

<details open>
<summary>Available commands</summary>

### [background-processes](docs/forge_background-processes.md)

* [`organizations-servers-background-processes-index`](docs/forge_background-processes_organizations-servers-background-processes-index.md) - List background processes
* [`organizations-servers-background-processes-store`](docs/forge_background-processes_organizations-servers-background-processes-store.md) - Create background process
* [`organizations-servers-background-processes-show`](docs/forge_background-processes_organizations-servers-background-processes-show.md) - Get background process
* [`organizations-servers-background-processes-update`](docs/forge_background-processes_organizations-servers-background-processes-update.md) - Update background process
* [`organizations-servers-background-processes-destroy`](docs/forge_background-processes_organizations-servers-background-processes-destroy.md) - Delete background process
* [`organizations-servers-background-processes-log-show`](docs/forge_background-processes_organizations-servers-background-processes-log-show.md) - Get background process log

### [backups](docs/forge_backups.md)

* [`organizations-servers-database-backups-index`](docs/forge_backups_organizations-servers-database-backups-index.md) - List backup configurations
* [`organizations-servers-database-backups-store`](docs/forge_backups_organizations-servers-database-backups-store.md) - Create backup configuration
* [`organizations-servers-database-backups-show`](docs/forge_backups_organizations-servers-database-backups-show.md) - Get backup configuration
* [`organizations-servers-database-backups-update`](docs/forge_backups_organizations-servers-database-backups-update.md) - Update backup configuration
* [`organizations-servers-database-backups-destroy`](docs/forge_backups_organizations-servers-database-backups-destroy.md) - Delete backup configuration
* [`organizations-servers-database-backups-instances-index`](docs/forge_backups_organizations-servers-database-backups-instances-index.md) - List backups
* [`organizations-servers-database-backups-instances-store`](docs/forge_backups_organizations-servers-database-backups-instances-store.md) - Create backup
* [`organizations-servers-database-backups-instances-show`](docs/forge_backups_organizations-servers-database-backups-instances-show.md) - Get backup
* [`organizations-servers-database-backups-instances-destroy`](docs/forge_backups_organizations-servers-database-backups-instances-destroy.md) - Delete backup
* [`organizations-servers-database-backups-instances-restores-store`](docs/forge_backups_organizations-servers-database-backups-instances-restores-store.md) - Create a database restore from backup

### [commands](docs/forge_commands.md)

* [`organizations-servers-sites-commands-index`](docs/forge_commands_organizations-servers-sites-commands-index.md) - List commands
* [`organizations-servers-sites-commands-store`](docs/forge_commands_organizations-servers-sites-commands-store.md) - Create command
* [`organizations-servers-sites-commands-show`](docs/forge_commands_organizations-servers-sites-commands-show.md) - Get command
* [`organizations-servers-sites-commands-destroy`](docs/forge_commands_organizations-servers-sites-commands-destroy.md) - Delete command
* [`organizations-servers-sites-commands-output-show`](docs/forge_commands_organizations-servers-sites-commands-output-show.md) - Get command output

### [databases](docs/forge_databases.md)

* [`organizations-servers-database-schemas-index`](docs/forge_databases_organizations-servers-database-schemas-index.md) - List database schemas
* [`organizations-servers-database-schemas-store`](docs/forge_databases_organizations-servers-database-schemas-store.md) - Create database schema
* [`organizations-servers-database-schemas-show`](docs/forge_databases_organizations-servers-database-schemas-show.md) - Get database schema
* [`organizations-servers-database-schemas-destroy`](docs/forge_databases_organizations-servers-database-schemas-destroy.md) - Delete database schema
* [`organizations-servers-database-schemas-synchronizations-store`](docs/forge_databases_organizations-servers-database-schemas-synchronizations-store.md) - Update database schemas
* [`organizations-servers-database-users-index`](docs/forge_databases_organizations-servers-database-users-index.md) - List database users
* [`organizations-servers-database-users-store`](docs/forge_databases_organizations-servers-database-users-store.md) - Create database user
* [`organizations-servers-database-users-show`](docs/forge_databases_organizations-servers-database-users-show.md) - Get database user
* [`organizations-servers-database-users-update`](docs/forge_databases_organizations-servers-database-users-update.md) - Update database user
* [`organizations-servers-database-users-destroy`](docs/forge_databases_organizations-servers-database-users-destroy.md) - Delete database user
* [`organizations-servers-database-password-update`](docs/forge_databases_organizations-servers-database-password-update.md) - Update the password for the database

### [deployments](docs/forge_deployments.md)

* [`organizations-servers-sites-webhooks-index`](docs/forge_deployments_organizations-servers-sites-webhooks-index.md) - List site webhooks
* [`organizations-servers-sites-webhooks-store`](docs/forge_deployments_organizations-servers-sites-webhooks-store.md) - Create site webhook
* [`organizations-servers-sites-webhooks-show`](docs/forge_deployments_organizations-servers-sites-webhooks-show.md) - Get site webhook
* [`organizations-servers-sites-webhooks-destroy`](docs/forge_deployments_organizations-servers-sites-webhooks-destroy.md) - Delete site webhook
* [`organizations-servers-sites-deployments-index`](docs/forge_deployments_organizations-servers-sites-deployments-index.md) - List deployments
* [`organizations-servers-sites-deployments-store`](docs/forge_deployments_organizations-servers-sites-deployments-store.md) - Create deployment
* [`organizations-servers-sites-deployments-status-show`](docs/forge_deployments_organizations-servers-sites-deployments-status-show.md) - Get deployment status
* [`organizations-servers-sites-deployments-status-destroy`](docs/forge_deployments_organizations-servers-sites-deployments-status-destroy.md) - Update deployment state
* [`organizations-servers-sites-deployments-script-show`](docs/forge_deployments_organizations-servers-sites-deployments-script-show.md) - Get deployment script
* [`organizations-servers-sites-deployments-script-update`](docs/forge_deployments_organizations-servers-sites-deployments-script-update.md) - Update deployment script
* [`organizations-servers-sites-deployments-deploy-hook-show`](docs/forge_deployments_organizations-servers-sites-deployments-deploy-hook-show.md) - Get the deployment trigger URL
* [`organizations-servers-sites-deployments-deploy-hook-update`](docs/forge_deployments_organizations-servers-sites-deployments-deploy-hook-update.md) - Update deployment trigger URL
* [`organizations-servers-sites-deployments-push-to-deploy-store`](docs/forge_deployments_organizations-servers-sites-deployments-push-to-deploy-store.md) - Create push to deploy configuration
* [`organizations-servers-sites-deployments-push-to-deploy-destroy`](docs/forge_deployments_organizations-servers-sites-deployments-push-to-deploy-destroy.md) - Delete push to deploy configuration
* [`organizations-servers-sites-deployments-show`](docs/forge_deployments_organizations-servers-sites-deployments-show.md) - Get deployment
* [`organizations-servers-sites-deployments-log-show`](docs/forge_deployments_organizations-servers-sites-deployments-log-show.md) - Get deployment output
* [`organizations-servers-sites-deploy-key-show`](docs/forge_deployments_organizations-servers-sites-deploy-key-show.md) - Get deploy key
* [`organizations-servers-sites-deploy-key-store`](docs/forge_deployments_organizations-servers-sites-deploy-key-store.md) - Create deploy key
* [`organizations-servers-sites-deploy-key-destroy`](docs/forge_deployments_organizations-servers-sites-deploy-key-destroy.md) - Delete deploy key

### [firewall-rules](docs/forge_firewall-rules.md)

* [`organizations-servers-firewall-rules-index`](docs/forge_firewall-rules_organizations-servers-firewall-rules-index.md) - List server firewall rules
* [`organizations-servers-firewall-rules-store`](docs/forge_firewall-rules_organizations-servers-firewall-rules-store.md) - Create server firewall rule
* [`organizations-servers-firewall-rules-show`](docs/forge_firewall-rules_organizations-servers-firewall-rules-show.md) - Get server firewall rule
* [`organizations-servers-firewall-rules-destroy`](docs/forge_firewall-rules_organizations-servers-firewall-rules-destroy.md) - Delete server firewall rule

### [integrations](docs/forge_integrations.md)

* [`organizations-servers-sites-integrations-horizon-show`](docs/forge_integrations_organizations-servers-sites-integrations-horizon-show.md) - Get Laravel Horizon integration status
* [`organizations-servers-sites-integrations-horizon-store`](docs/forge_integrations_organizations-servers-sites-integrations-horizon-store.md) - Create Laravel Horizon integration
* [`organizations-servers-sites-integrations-horizon-destroy`](docs/forge_integrations_organizations-servers-sites-integrations-horizon-destroy.md) - Delete Laravel Horizon integration
* [`organizations-servers-sites-integrations-octane-show`](docs/forge_integrations_organizations-servers-sites-integrations-octane-show.md) - Get Laravel Octane integration status
* [`organizations-servers-sites-integrations-octane-store`](docs/forge_integrations_organizations-servers-sites-integrations-octane-store.md) - Create Laravel Octane integration
* [`organizations-servers-sites-integrations-octane-destroy`](docs/forge_integrations_organizations-servers-sites-integrations-octane-destroy.md) - Delete Laravel Octane integration
* [`organizations-servers-sites-integrations-reverb-show`](docs/forge_integrations_organizations-servers-sites-integrations-reverb-show.md) - Get Laravel Reverb integration status
* [`organizations-servers-sites-integrations-reverb-store`](docs/forge_integrations_organizations-servers-sites-integrations-reverb-store.md) - Create Laravel Reverb integration
* [`organizations-servers-sites-integrations-reverb-destroy`](docs/forge_integrations_organizations-servers-sites-integrations-reverb-destroy.md) - Delete Laravel Reverb integration
* [`organizations-servers-sites-integrations-inertia-show`](docs/forge_integrations_organizations-servers-sites-integrations-inertia-show.md) - Get Inertia integration status
* [`organizations-servers-sites-integrations-inertia-store`](docs/forge_integrations_organizations-servers-sites-integrations-inertia-store.md) - Create Inertia integration
* [`organizations-servers-sites-integrations-pulse-show`](docs/forge_integrations_organizations-servers-sites-integrations-pulse-show.md) - Get Laravel Pulse integration status
* [`organizations-servers-sites-integrations-pulse-store`](docs/forge_integrations_organizations-servers-sites-integrations-pulse-store.md) - Create Laravel Pulse integration
* [`organizations-servers-sites-integrations-pulse-destroy`](docs/forge_integrations_organizations-servers-sites-integrations-pulse-destroy.md) - Delete Laravel Pulse integration
* [`organizations-servers-sites-integrations-laravel-maintenance-show`](docs/forge_integrations_organizations-servers-sites-integrations-laravel-maintenance-show.md) - Get Laravel Maintenance integration status
* [`organizations-servers-sites-integrations-laravel-maintenance-store`](docs/forge_integrations_organizations-servers-sites-integrations-laravel-maintenance-store.md) - Create Laravel Maintenance integration
* [`organizations-servers-sites-integrations-laravel-maintenance-destroy`](docs/forge_integrations_organizations-servers-sites-integrations-laravel-maintenance-destroy.md) - Delete Laravel Maintenance integration
* [`organizations-servers-sites-integrations-laravel-scheduler-show`](docs/forge_integrations_organizations-servers-sites-integrations-laravel-scheduler-show.md) - Get Laravel Scheduler integration job
* [`organizations-servers-sites-integrations-laravel-scheduler-store`](docs/forge_integrations_organizations-servers-sites-integrations-laravel-scheduler-store.md) - Create Laravel Scheduler integration job
* [`organizations-servers-sites-integrations-laravel-scheduler-destroy`](docs/forge_integrations_organizations-servers-sites-integrations-laravel-scheduler-destroy.md) - Delete Laravel Scheduler integration job

### [logs](docs/forge_logs.md)

* [`organizations-servers-logs-show`](docs/forge_logs_organizations-servers-logs-show.md) - Get server log content
* [`organizations-servers-logs-destroy`](docs/forge_logs_organizations-servers-logs-destroy.md) - Delete server log content

### [monitors](docs/forge_monitors.md)

* [`organizations-servers-monitors-index`](docs/forge_monitors_organizations-servers-monitors-index.md) - List server monitors
* [`organizations-servers-monitors-store`](docs/forge_monitors_organizations-servers-monitors-store.md) - Create server monitor
* [`organizations-servers-monitors-show`](docs/forge_monitors_organizations-servers-monitors-show.md) - Get server monitor
* [`organizations-servers-monitors-destroy`](docs/forge_monitors_organizations-servers-monitors-destroy.md) - Delete server monitor

### [nginx](docs/forge_nginx.md)

* [`organizations-servers-nginx-templates-index`](docs/forge_nginx_organizations-servers-nginx-templates-index.md) - List Nginx templates
* [`organizations-servers-nginx-templates-store`](docs/forge_nginx_organizations-servers-nginx-templates-store.md) - Create Nginx template
* [`organizations-servers-nginx-templates-show`](docs/forge_nginx_organizations-servers-nginx-templates-show.md) - Get Nginx template
* [`organizations-servers-nginx-templates-update`](docs/forge_nginx_organizations-servers-nginx-templates-update.md) - Update Nginx template
* [`organizations-servers-nginx-templates-destroy`](docs/forge_nginx_organizations-servers-nginx-templates-destroy.md) - Delete Nginx template

### [organizations](docs/forge_organizations.md)

* [`index`](docs/forge_organizations_index.md) - List organizations
* [`show`](docs/forge_organizations_show.md) - Get organization
* [`server-credentials-index`](docs/forge_organizations_server-credentials-index.md) - List server credentials
* [`server-credentials-show`](docs/forge_organizations_server-credentials-show.md) - Get server credential
* [`server-credentials-vpcs-store`](docs/forge_organizations_server-credentials-vpcs-store.md) - Create a new VPC
* [`server-credentials-vpcs-index`](docs/forge_organizations_server-credentials-vpcs-index.md) - List VPCs
* [`server-credentials-vpcs-show`](docs/forge_organizations_server-credentials-vpcs-show.md) - Get VPC

### [providers](docs/forge_providers.md)

* [`index`](docs/forge_providers_index.md) - List providers
* [`show`](docs/forge_providers_show.md) - Get provider
* [`sizes-index`](docs/forge_providers_sizes-index.md) - List provider sizes
* [`sizes-show`](docs/forge_providers_sizes-show.md) - Get provider size
* [`regions-index`](docs/forge_providers_regions-index.md) - List provider regions
* [`regions-show`](docs/forge_providers_regions-show.md) - Get provider region
* [`regions-sizes-index`](docs/forge_providers_regions-sizes-index.md) - List provider region sizes
* [`regions-sizes-show`](docs/forge_providers_regions-sizes-show.md) - Get provider region size

### [recipes](docs/forge_recipes.md)

* [`organizations-recipes-index`](docs/forge_recipes_organizations-recipes-index.md) - List organization recipes
* [`organization-recipes-store`](docs/forge_recipes_organization-recipes-store.md) - Create recipe
* [`organizations-recipes-show`](docs/forge_recipes_organizations-recipes-show.md) - Get recipe
* [`organizations-recipes-update`](docs/forge_recipes_organizations-recipes-update.md) - Update recipe
* [`organizations-recipes-destroy`](docs/forge_recipes_organizations-recipes-destroy.md) - Delete recipe
* [`organizations-recipes-runs-index`](docs/forge_recipes_organizations-recipes-runs-index.md) - List recipe runs
* [`organizations-recipes-runs-store`](docs/forge_recipes_organizations-recipes-runs-store.md) - Create recipe run
* [`organizations-recipes-runs-show`](docs/forge_recipes_organizations-recipes-runs-show.md) - Get recipe run
* [`organizations-teams-recipes-index`](docs/forge_recipes_organizations-teams-recipes-index.md) - List team recipes
* [`organizations-teams-recipes-store`](docs/forge_recipes_organizations-teams-recipes-store.md) - Share recipe with the team
* [`organizations-teams-recipes-destroy`](docs/forge_recipes_organizations-teams-recipes-destroy.md) - Delete a recipe share
* [`forge-recipes-index`](docs/forge_recipes_forge-recipes-index.md) - List Forge's recipes
* [`forge-recipes-show`](docs/forge_recipes_forge-recipes-show.md) - Get Forge recipe
* [`forge-recipes-runs-store`](docs/forge_recipes_forge-recipes-runs-store.md) - Create Forge recipe run

### [redirect-rules](docs/forge_redirect-rules.md)

* [`organizations-servers-sites-redirect-rules-index`](docs/forge_redirect-rules_organizations-servers-sites-redirect-rules-index.md) - List site redirect rules
* [`organizations-servers-sites-redirect-rules-store`](docs/forge_redirect-rules_organizations-servers-sites-redirect-rules-store.md) - Create site redirect rule
* [`organizations-servers-sites-redirect-rules-show`](docs/forge_redirect-rules_organizations-servers-sites-redirect-rules-show.md) - Get site redirect rule
* [`organizations-servers-sites-redirect-rules-destroy`](docs/forge_redirect-rules_organizations-servers-sites-redirect-rules-destroy.md) - Delete site redirect rule

### [roles](docs/forge_roles.md)

* [`predefined-roles-index`](docs/forge_roles_predefined-roles-index.md) - List predefined roles
* [`predefined-roles-show`](docs/forge_roles_predefined-roles-show.md) - Get predefined role
* [`permissions-index`](docs/forge_roles_permissions-index.md) - List permissions
* [`permissions-show`](docs/forge_roles_permissions-show.md) - Get permission
* [`organizations-roles-store`](docs/forge_roles_organizations-roles-store.md) - Create role
* [`organizations-roles-index`](docs/forge_roles_organizations-roles-index.md) - List roles
* [`organizations-roles-show`](docs/forge_roles_organizations-roles-show.md) - Get role
* [`organizations-roles-update`](docs/forge_roles_organizations-roles-update.md) - Update role
* [`organizations-roles-destroy`](docs/forge_roles_organizations-roles-destroy.md) - Delete role
* [`organizations-roles-permissions-index`](docs/forge_roles_organizations-roles-permissions-index.md) - List role permissions

### [SSH-keys](docs/forge_SSH-keys.md)

* [`organizations-servers-ssh-keys-index`](docs/forge_SSH-keys_organizations-servers-ssh-keys-index.md) - List server SSH keys
* [`organizations-servers-ssh-keys-store`](docs/forge_SSH-keys_organizations-servers-ssh-keys-store.md) - Create server SSH key
* [`organizations-servers-ssh-keys-show`](docs/forge_SSH-keys_organizations-servers-ssh-keys-show.md) - Get server SSH key
* [`organizations-servers-ssh-keys-destroy`](docs/forge_SSH-keys_organizations-servers-ssh-keys-destroy.md) - Delete server SSH key
* [`organizations-servers-key-show`](docs/forge_SSH-keys_organizations-servers-key-show.md) - Get server public SSH key
* [`organizations-servers-key-update`](docs/forge_SSH-keys_organizations-servers-key-update.md) - Update server public SSH key

### [scheduled-jobs](docs/forge_scheduled-jobs.md)

* [`organizations-servers-scheduled-jobs-index`](docs/forge_scheduled-jobs_organizations-servers-scheduled-jobs-index.md) - List server scheduled jobs
* [`organizations-servers-scheduled-jobs-store`](docs/forge_scheduled-jobs_organizations-servers-scheduled-jobs-store.md) - Create scheduled job
* [`organizations-servers-scheduled-jobs-show`](docs/forge_scheduled-jobs_organizations-servers-scheduled-jobs-show.md) - Get scheduled job
* [`organizations-servers-scheduled-jobs-destroy`](docs/forge_scheduled-jobs_organizations-servers-scheduled-jobs-destroy.md) - Delete scheduled job
* [`organizations-servers-scheduled-jobs-outputs-show`](docs/forge_scheduled-jobs_organizations-servers-scheduled-jobs-outputs-show.md) - Get scheduled job output
* [`organizations-servers-sites-scheduled-jobs-index`](docs/forge_scheduled-jobs_organizations-servers-sites-scheduled-jobs-index.md) - List site scheduled jobs
* [`organizations-servers-sites-scheduled-jobs-store`](docs/forge_scheduled-jobs_organizations-servers-sites-scheduled-jobs-store.md) - Create site scheduled job
* [`organizations-servers-sites-scheduled-jobs-show`](docs/forge_scheduled-jobs_organizations-servers-sites-scheduled-jobs-show.md) - Get site scheduled job
* [`organizations-servers-sites-scheduled-jobs-destroy`](docs/forge_scheduled-jobs_organizations-servers-sites-scheduled-jobs-destroy.md) - Delete site scheduled job
* [`organizations-servers-sites-scheduled-jobs-outputs-show`](docs/forge_scheduled-jobs_organizations-servers-sites-scheduled-jobs-outputs-show.md) - Get site scheduled job output

### [security-rules](docs/forge_security-rules.md)

* [`organizations-servers-sites-security-rules-index`](docs/forge_security-rules_organizations-servers-sites-security-rules-index.md) - List site security rules
* [`organizations-servers-sites-security-rules-store`](docs/forge_security-rules_organizations-servers-sites-security-rules-store.md) - Create site security rule
* [`organizations-servers-sites-security-rules-show`](docs/forge_security-rules_organizations-servers-sites-security-rules-show.md) - Get site security rule
* [`organizations-servers-sites-security-rules-update`](docs/forge_security-rules_organizations-servers-sites-security-rules-update.md) - Update site security rule
* [`organizations-servers-sites-security-rules-destroy`](docs/forge_security-rules_organizations-servers-sites-security-rules-destroy.md) - Delete site security rule

### [server-credentials](docs/forge_server-credentials.md)

* [`organizations-teams-server-credentials-index`](docs/forge_server-credentials_organizations-teams-server-credentials-index.md) - List team server credentials
* [`organizations-teams-server-credentials-store`](docs/forge_server-credentials_organizations-teams-server-credentials-store.md) - Create a new server credential share
* [`organizations-teams-server-credentials-destroy`](docs/forge_server-credentials_organizations-teams-server-credentials-destroy.md) - Delete a server credential share

### [servers](docs/forge_servers.md)

* [`organizations-servers-index`](docs/forge_servers_organizations-servers-index.md) - List servers
* [`organizations-servers-store`](docs/forge_servers_organizations-servers-store.md) - Create server
* [`organizations-servers-archives-index`](docs/forge_servers_organizations-servers-archives-index.md) - List archived servers
* [`organizations-servers-archives-store`](docs/forge_servers_organizations-servers-archives-store.md) - Create an archived server
* [`organizations-servers-archives-destroy`](docs/forge_servers_organizations-servers-archives-destroy.md) - Delete archived server
* [`organizations-servers-background-processes-actions-store`](docs/forge_servers_organizations-servers-background-processes-actions-store.md) - Perform an action on a server background process
* [`organizations-servers-actions-store`](docs/forge_servers_organizations-servers-actions-store.md) - Create server action
* [`organizations-servers-services-nginx-actions-store`](docs/forge_servers_organizations-servers-services-nginx-actions-store.md) - Perform Nginx action
* [`organizations-servers-services-postgres-actions-store`](docs/forge_servers_organizations-servers-services-postgres-actions-store.md) - Perform Postgres action
* [`organizations-servers-services-redis-actions-store`](docs/forge_servers_organizations-servers-services-redis-actions-store.md) - Perform Redis action
* [`organizations-servers-services-mysql-actions-store`](docs/forge_servers_organizations-servers-services-mysql-actions-store.md) - Perform MySQL action
* [`organizations-servers-services-php-actions-store`](docs/forge_servers_organizations-servers-services-php-actions-store.md) - Perform PHP action
* [`organizations-servers-services-supervisor-actions-store`](docs/forge_servers_organizations-servers-services-supervisor-actions-store.md) - Perform Supervisor action
* [`organizations-servers-show`](docs/forge_servers_organizations-servers-show.md) - Get server
* [`organizations-servers-update`](docs/forge_servers_organizations-servers-update.md) - Update server
* [`organizations-servers-destroy`](docs/forge_servers_organizations-servers-destroy.md) - Delete server
* [`organizations-servers-network-show`](docs/forge_servers_organizations-servers-network-show.md) - Get server network
* [`organizations-servers-network-update`](docs/forge_servers_organizations-servers-network-update.md) - Update server network
* [`organizations-servers-events-index`](docs/forge_servers_organizations-servers-events-index.md) - List server events
* [`organizations-servers-events-show`](docs/forge_servers_organizations-servers-events-show.md) - Get server event
* [`organizations-servers-events-output-show`](docs/forge_servers_organizations-servers-events-output-show.md) - Get server event output
* [`organizations-servers-php-cli-version-show`](docs/forge_servers_organizations-servers-php-cli-version-show.md) - Get PHP CLI version
* [`organizations-servers-php-cli-version-update`](docs/forge_servers_organizations-servers-php-cli-version-update.md) - Update PHP CLI version
* [`organizations-servers-php-site-version-show`](docs/forge_servers_organizations-servers-php-site-version-show.md) - Get PHP site version
* [`organizations-servers-php-site-version-update`](docs/forge_servers_organizations-servers-php-site-version-update.md) - Update PHP site version
* [`organizations-servers-php-versions-index`](docs/forge_servers_organizations-servers-php-versions-index.md) - List PHP versions for server
* [`organizations-servers-php-versions-store`](docs/forge_servers_organizations-servers-php-versions-store.md) - Install new PHP version
* [`organizations-servers-php-versions-show`](docs/forge_servers_organizations-servers-php-versions-show.md) - Get PHP version
* [`organizations-servers-php-versions-update`](docs/forge_servers_organizations-servers-php-versions-update.md) - Update installed PHP version
* [`organizations-servers-php-versions-destroy`](docs/forge_servers_organizations-servers-php-versions-destroy.md) - Delete installed PHP version
* [`organizations-servers-php-versions-configs-fpm-show`](docs/forge_servers_organizations-servers-php-versions-configs-fpm-show.md) - Get PHP version FPM config
* [`organizations-servers-php-versions-configs-fpm-update`](docs/forge_servers_organizations-servers-php-versions-configs-fpm-update.md) - Update PHP version FPM config
* [`organizations-servers-php-versions-configs-cli-show`](docs/forge_servers_organizations-servers-php-versions-configs-cli-show.md) - Get PHP version CLI config
* [`organizations-servers-php-versions-configs-cli-update`](docs/forge_servers_organizations-servers-php-versions-configs-cli-update.md) - Update PHP version CLI config
* [`organizations-servers-php-versions-configs-pool-show`](docs/forge_servers_organizations-servers-php-versions-configs-pool-show.md) - Get PHP version pool config
* [`organizations-servers-php-versions-configs-pool-update`](docs/forge_servers_organizations-servers-php-versions-configs-pool-update.md) - Update PHP version pool config
* [`organizations-servers-php-max-upload-size-show`](docs/forge_servers_organizations-servers-php-max-upload-size-show.md) - Get server PHP max upload size
* [`organizations-servers-php-max-upload-size-update`](docs/forge_servers_organizations-servers-php-max-upload-size-update.md) - Update server PHP max upload size
* [`organizations-servers-php-max-execution-time-show`](docs/forge_servers_organizations-servers-php-max-execution-time-show.md) - Get server PHP max execution time
* [`organizations-servers-php-max-execution-time-update`](docs/forge_servers_organizations-servers-php-max-execution-time-update.md) - Update server PHP max execution time
* [`organizations-servers-php-opcache-show`](docs/forge_servers_organizations-servers-php-opcache-show.md) - Get server PHP OPcache status
* [`organizations-servers-php-opcache-store`](docs/forge_servers_organizations-servers-php-opcache-store.md) - Create PHP OPcache config
* [`organizations-servers-php-opcache-destroy`](docs/forge_servers_organizations-servers-php-opcache-destroy.md) - Delete PHP OPcache config
* [`organizations-teams-servers-index`](docs/forge_servers_organizations-teams-servers-index.md) - List team servers
* [`organizations-teams-servers-store`](docs/forge_servers_organizations-teams-servers-store.md) - Create a new server share
* [`organizations-teams-servers-destroy`](docs/forge_servers_organizations-teams-servers-destroy.md) - Delete a server share

### [sites](docs/forge_sites.md)

* [`index`](docs/forge_sites_index.md) - List sites
* [`organizations-sites-index`](docs/forge_sites_organizations-sites-index.md) - List sites for Organization
* [`organizations-sites-show`](docs/forge_sites_organizations-sites-show.md) - Get site
* [`organizations-servers-sites-index`](docs/forge_sites_organizations-servers-sites-index.md) - List sites for server
* [`organizations-servers-sites-store`](docs/forge_sites_organizations-servers-sites-store.md) - Create site
* [`organizations-servers-sites-store-on-balancer`](docs/forge_sites_organizations-servers-sites-store-on-balancer.md) - Create site on a load balancer
* [`organizations-servers-sites-update`](docs/forge_sites_organizations-servers-sites-update.md) - Update site
* [`organizations-servers-sites-destroy`](docs/forge_sites_organizations-servers-sites-destroy.md) - Delete site
* [`organizations-servers-sites-certificates-index`](docs/forge_sites_organizations-servers-sites-certificates-index.md) - List site certificates
* [`organizations-servers-sites-domains-index`](docs/forge_sites_organizations-servers-sites-domains-index.md) - List domains
* [`organizations-servers-sites-domains-store`](docs/forge_sites_organizations-servers-sites-domains-store.md) - Create domain
* [`organizations-servers-sites-domains-show`](docs/forge_sites_organizations-servers-sites-domains-show.md) - Get domain
* [`organizations-servers-sites-domains-update`](docs/forge_sites_organizations-servers-sites-domains-update.md) - Update domain
* [`organizations-servers-sites-domains-destroy`](docs/forge_sites_organizations-servers-sites-domains-destroy.md) - Delete domain
* [`organizations-servers-sites-domains-configurations`](docs/forge_sites_organizations-servers-sites-domains-configurations.md) - Get domain DNS configuration
* [`organizations-servers-sites-domains-actions-store`](docs/forge_sites_organizations-servers-sites-domains-actions-store.md) - Create domain action
* [`organizations-servers-sites-domains-nginx-show`](docs/forge_sites_organizations-servers-sites-domains-nginx-show.md) - Get domain Nginx configuration
* [`organizations-servers-sites-domains-nginx-update`](docs/forge_sites_organizations-servers-sites-domains-nginx-update.md) - Update domain Nginx configuration
* [`organizations-servers-sites-domains-certificate-show`](docs/forge_sites_organizations-servers-sites-domains-certificate-show.md) - Get active domain certificate
* [`organizations-servers-sites-domains-certificates-index`](docs/forge_sites_organizations-servers-sites-domains-certificates-index.md) - List domain certificates
* [`organizations-servers-sites-domains-certificates-store`](docs/forge_sites_organizations-servers-sites-domains-certificates-store.md) - Create domain certificate
* [`organizations-servers-sites-domains-certificates-active`](docs/forge_sites_organizations-servers-sites-domains-certificates-active.md) - Get active domain certificate
* [`organizations-servers-sites-domains-certificates-show`](docs/forge_sites_organizations-servers-sites-domains-certificates-show.md) - Get domain certificate
* [`organizations-servers-sites-domains-certificates-destroy`](docs/forge_sites_organizations-servers-sites-domains-certificates-destroy.md) - Delete domain certificate
* [`organizations-servers-sites-domains-certificates-actions-store`](docs/forge_sites_organizations-servers-sites-domains-certificates-actions-store.md) - Create domain certificate action
* [`organizations-servers-sites-healthcheck-show`](docs/forge_sites_organizations-servers-sites-healthcheck-show.md) - Get healthcheck endpoint
* [`organizations-servers-sites-healthcheck-update`](docs/forge_sites_organizations-servers-sites-healthcheck-update.md) - Update healthcheck endpoint
* [`organizations-servers-sites-environment-show`](docs/forge_sites_organizations-servers-sites-environment-show.md) - Get .env content
* [`organizations-servers-sites-environment-update`](docs/forge_sites_organizations-servers-sites-environment-update.md) - Update .env content
* [`organizations-servers-sites-nginx-show`](docs/forge_sites_organizations-servers-sites-nginx-show.md) - Get Nginx configuration
* [`organizations-servers-sites-nginx-update`](docs/forge_sites_organizations-servers-sites-nginx-update.md) - Update Nginx configuration
* [`organizations-servers-sites-composer-credentials-index`](docs/forge_sites_organizations-servers-sites-composer-credentials-index.md) - Get composer credentials for the site
* [`organizations-servers-sites-composer-credentials-store`](docs/forge_sites_organizations-servers-sites-composer-credentials-store.md) - Create composer credentials for the site
* [`organizations-servers-sites-composer-credentials-show`](docs/forge_sites_organizations-servers-sites-composer-credentials-show.md) - Get composer credential for the site
* [`organizations-servers-sites-composer-credentials-update`](docs/forge_sites_organizations-servers-sites-composer-credentials-update.md) - Update composer credentials for the site
* [`organizations-servers-sites-composer-credentials-destroy`](docs/forge_sites_organizations-servers-sites-composer-credentials-destroy.md) - Delete composer credentials for the site
* [`organizations-servers-sites-npm-credentials-index`](docs/forge_sites_organizations-servers-sites-npm-credentials-index.md) - Get NPM credentials for the site
* [`organizations-servers-sites-npm-credentials-store`](docs/forge_sites_organizations-servers-sites-npm-credentials-store.md) - Create NPM credentials for the site
* [`organizations-servers-sites-npm-credentials-show`](docs/forge_sites_organizations-servers-sites-npm-credentials-show.md) - Get NPM credential for the site
* [`organizations-servers-sites-npm-credentials-update`](docs/forge_sites_organizations-servers-sites-npm-credentials-update.md) - Update NPM credentials for the site
* [`organizations-servers-sites-npm-credentials-destroy`](docs/forge_sites_organizations-servers-sites-npm-credentials-destroy.md) - Delete npm credentials for the site
* [`organizations-servers-sites-load-balancing-nodes-index`](docs/forge_sites_organizations-servers-sites-load-balancing-nodes-index.md) - List load balancing nodes
* [`organizations-servers-sites-load-balancing-nodes-update`](docs/forge_sites_organizations-servers-sites-load-balancing-nodes-update.md) - Update load balancing nodes
* [`organizations-servers-sites-logs-nginx-access-show`](docs/forge_sites_organizations-servers-sites-logs-nginx-access-show.md) - Get Nginx access log content
* [`organizations-servers-sites-logs-nginx-access-destroy`](docs/forge_sites_organizations-servers-sites-logs-nginx-access-destroy.md) - Delete Nginx access log content
* [`organizations-servers-sites-logs-nginx-error-show`](docs/forge_sites_organizations-servers-sites-logs-nginx-error-show.md) - Get Nginx error log content
* [`organizations-servers-sites-logs-nginx-error-destroy`](docs/forge_sites_organizations-servers-sites-logs-nginx-error-destroy.md) - Delete Nginx error log content
* [`organizations-servers-sites-logs-application-show`](docs/forge_sites_organizations-servers-sites-logs-application-show.md) - Get site log content
* [`organizations-servers-sites-logs-application-destroy`](docs/forge_sites_organizations-servers-sites-logs-application-destroy.md) - Delete site log content
* [`organizations-servers-sites-heartbeats-index`](docs/forge_sites_organizations-servers-sites-heartbeats-index.md) - List heartbeats
* [`organizations-servers-sites-heartbeats-store`](docs/forge_sites_organizations-servers-sites-heartbeats-store.md) - Create heartbeat
* [`organizations-servers-sites-heartbeats-show`](docs/forge_sites_organizations-servers-sites-heartbeats-show.md) - Get heartbeat
* [`organizations-servers-sites-heartbeats-update`](docs/forge_sites_organizations-servers-sites-heartbeats-update.md) - Update heartbeat
* [`organizations-servers-sites-heartbeats-destroy`](docs/forge_sites_organizations-servers-sites-heartbeats-destroy.md) - Delete heartbeat

### [storage-providers](docs/forge_storage-providers.md)

* [`organizations-storage-providers-index`](docs/forge_storage-providers_organizations-storage-providers-index.md) - List storage providers
* [`organizations-storage-providers-store`](docs/forge_storage-providers_organizations-storage-providers-store.md) - Create storage provider
* [`organizations-storage-providers-show`](docs/forge_storage-providers_organizations-storage-providers-show.md) - Get storage provider
* [`organizations-storage-providers-update`](docs/forge_storage-providers_organizations-storage-providers-update.md) - Update storage provider
* [`organizations-storage-providers-destroy`](docs/forge_storage-providers_organizations-storage-providers-destroy.md) - Delete storage provider

### [teams](docs/forge_teams.md)

* [`organizations-teams-index`](docs/forge_teams_organizations-teams-index.md) - List teams
* [`organizations-teams-store`](docs/forge_teams_organizations-teams-store.md) - Create team
* [`organizations-teams-show`](docs/forge_teams_organizations-teams-show.md) - Get team
* [`organizations-teams-update`](docs/forge_teams_organizations-teams-update.md) - Update team
* [`organizations-teams-destroy`](docs/forge_teams_organizations-teams-destroy.md) - Delete team
* [`organizations-teams-members-index`](docs/forge_teams_organizations-teams-members-index.md) - List team members
* [`organizations-teams-members-show`](docs/forge_teams_organizations-teams-members-show.md) - Get team member
* [`organizations-teams-members-destroy`](docs/forge_teams_organizations-teams-members-destroy.md) - Delete team member
* [`organizations-teams-members-update`](docs/forge_teams_organizations-teams-members-update.md) - Update team member
* [`organizations-teams-invites-store`](docs/forge_teams_organizations-teams-invites-store.md) - Create team invite
* [`organizations-teams-invites-index`](docs/forge_teams_organizations-teams-invites-index.md) - List team invitations
* [`organizations-teams-invites-show`](docs/forge_teams_organizations-teams-invites-show.md) - Get team invitation
* [`organizations-teams-invites-destroy`](docs/forge_teams_organizations-teams-invites-destroy.md) - Delete team invitation

### [user](docs/forge_user.md)

* [`show`](docs/forge_user_show.md) - Get user
* [`me`](docs/forge_user_me.md) - Get user

</details>
<!-- End Available Commands [operations] -->

<!-- Start Request Body Input [stdinpiping] -->
## Request Body Input

Operations that accept a request body support three input methods, with a clear priority chain:

### Individual flags (highest priority)

```bash
forge <command> --name "Jane" --age 30
```

### `--body` flag

Provide the entire request body as a JSON string:

```bash
forge <command> --body '{"name": "John", "age": 30}'
```

Individual flags override `--body` values:

```bash
# Result: {name: "Jane", age: 30}
forge <command> --body '{"name": "John", "age": 30}' --name "Jane"
```

### Stdin piping (lowest priority)

Pipe JSON into any command that accepts a request body:

```bash
echo '{"name": "John", "age": 30}' | forge <command>
```

Individual flags override stdin values:

```bash
# Result: {name: "Jane", age: 30}
echo '{"name": "John", "age": 30}' | forge <command> --name "Jane"
```

This is useful for chaining commands, reading from files, or scripting:

```bash
# Read body from a file
forge <command> < request.json

# Pipe from another command
curl -s https://example.com/data.json | forge <command>
```

### Priority

When multiple input methods are used, the priority is:

| Priority | Source | Description |
|----------|--------|-------------|
| 1 (highest) | Individual flags | `--name "Jane"` always wins |
| 2 | `--body` flag | Whole-body JSON via flag |
| 3 (lowest) | Stdin | Piped JSON input |
<!-- End Request Body Input [stdinpiping] -->

<!-- Start Server Selection [server] -->
## Server Selection

### Override Server URL

Use `--server-url` to override the server URL entirely, bypassing any named or indexed server selection:

```bash
forge --server-url https://custom-api.example.com <command> [arguments]
```

**Precedence**: `--server-url` > `--server` > default
<!-- End Server Selection [server] -->

<!-- Start Output Formats [output-formats] -->
## Output Formats

Every command supports a `--output-format` flag that controls how the response is rendered to stdout.

### Available formats

| Format | Flag | Description |
|--------|------|-------------|
| Pretty | `--output-format pretty` (default) | Aligned key-value pairs with color, nested indentation. Human-readable at a glance. |
| JSON | `--output-format json` | JSON output. Passthrough when the response is already JSON (preserves original field order and numeric precision). Falls back to typed marshaling otherwise. |
| YAML | `--output-format yaml` | YAML output via standard marshaling. |
| Table | `--output-format table` | Tabular output for array responses. |
| TOON | `--output-format toon` | [Token-Oriented Object Notation](https://github.com/toon-format/spec) — a compact, line-oriented format that typically uses 30–60% fewer tokens than JSON. Well-suited for piping responses into LLM prompts. |

```bash
# Default pretty output
forge <command>

# Machine-readable JSON
forge <command> --output-format json

# TOON for LLM-friendly compact output
forge <command> --output-format toon

# Pipe JSON to jq without using --output-format
forge <command> --output-format json | jq '.fieldName'
```

### jq filtering

Use `--jq` to filter or transform the response inline using a [jq](https://jqlang.org) expression. This always outputs JSON and overrides `--output-format`:

```bash
# Extract a single field
forge <command> --jq '.name'

# Filter an array
forge <command> --jq '.items[] | select(.active == true)'
```

### Color control

Use `--color` to control terminal colors:

| Value | Behavior |
|-------|----------|
| `auto` (default) | Color when stdout is a TTY, plain text otherwise |
| `always` | Always colorize |
| `never` | Never colorize |

The `NO_COLOR` and `FORCE_COLOR` environment variables are also respected.

### Streaming and pagination

When using `--all` (pagination) or streaming operations, output is written incrementally as items arrive:

| Format | Streaming behavior |
|--------|-------------------|
| `json` | One compact JSON object per line ([NDJSON](https://github.com/ndjson/ndjson-spec)) |
| `yaml` | YAML documents separated by `---` |
| `toon` | One TOON-encoded object per block, separated by blank lines |
| `pretty` (default) | Pretty-printed items separated by blank lines |
<!-- End Output Formats [output-formats] -->

<!-- Start Error Handling [errors] -->
## Error Handling

The CLI uses standard exit codes to indicate success or failure:

| Exit Code | Meaning |
|-----------|---------|
| `0` | Success |
| `1` | Error (API error, invalid input, etc.) |

On success, the response data is printed to **stdout** as JSON. On failure, error details are printed to **stderr**.

```bash
# Capture output and handle errors
forge ... > output.json 2> error.log
if [ $? -ne 0 ]; then
  echo "Error occurred, see error.log"
fi
```
<!-- End Error Handling [errors] -->

<!-- Start Diagnostics [diagnostics] -->
## Diagnostics

The CLI includes two diagnostic flags available on all commands:

### Dry Run

Preview what would be sent without making any network calls:

```bash
forge <command> --dry-run
```

Output goes to stderr and includes:
- HTTP method and URL
- Request headers (sensitive values redacted)
- Request body preview (sensitive fields redacted)

The command exits successfully without contacting the API. This is useful for verifying request construction before executing.

### Debug

Log request and response diagnostics while running normally:

```bash
forge <command> --debug
```

Debug output goes to stderr and includes:
- Request method, URL, headers, and body preview
- Response status, headers, and body preview
- Transport errors (if any)

The command still executes normally and produces its regular output on stdout.

### Flag Precedence

If both `--dry-run` and `--debug` are set, `--dry-run` takes precedence and no network calls are made.

### Security

Sensitive information is automatically redacted in diagnostic output:
- **Headers**: `Authorization`, `Cookie`, `Set-Cookie`, `X-API-Key`, and other security headers show `[REDACTED]`
- **Body**: JSON fields named `password`, `secret`, `token`, `api_key`, `client_secret`, etc. show `[REDACTED]`

Diagnostic output should still be treated as potentially sensitive operational data.
<!-- End Diagnostics [diagnostics] -->

<!-- Placeholder for Future Speakeasy SDK Sections -->

# Development

## Maturity

This CLI is in beta, and there may be breaking changes between versions without a major version update. Therefore, we recommend pinning usage
to a specific package version. This way, you can install the same version each time without breaking changes unless you are intentionally
looking for the latest version.

## Contributions

While we value open-source contributions to this CLI, this library is generated programmatically. Any manual changes added to internal files will be overwritten on the next generation. 
We look forward to hearing your feedback. Feel free to open a PR or an issue with a proof of concept and we'll do our best to include it in a future release. 

### CLI Created by [Speakeasy](https://www.speakeasy.com/?utm_source=github-com/mfullbrook/forge-cli&utm_campaign=cli)
