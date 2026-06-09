# rhis.core

Core shared utilities for the **RHIS (Red Hat Infrastructure Services)** Ansible namespace.

RHIS provides an opinionated, composable automation model for deploying and managing Red Hat
Infrastructure Services — IdM, Satellite, AAP, and their integrations — on bare metal, KVM,
VMware, and cloud. RHIS follows Red Hat recommended practice and configuration, giving operators
a proven starting point they can extend for their environment.

## Namespace

| Collection | Purpose |
|---|---|
| `rhis.core` | Shared utilities and common patterns (this collection) |
| `rhis.bootstrap` | Unattended RHEL installation via OEMDRV kickstart ISOs |
| `rhis.satellite` | Red Hat Satellite content, provisioning, and disconnected workflows |
| `rhis.idm` | Red Hat Identity Management (FreeIPA) configuration |
| `rhis.aap` | Ansible Automation Platform configuration and pipelines |

## Status

This collection is in early development. The RHIS projects currently ship as individual
`rhis-builder-*` git repositories. Collection packaging is a planned evolution of the existing
codebase — the role and variable structure is already collection-compatible.

## Requirements

- ansible-core >= 2.15
- Python >= 3.9

## License

GPL-2.0-or-later

## Author

parmstro (parmstro@redhat.com)
