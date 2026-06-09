# elise.core

Core shared utilities for the **ELISE (Enterprise Linux Infrastructure Standard Environment)**
Ansible namespace.

## What is ELISE?

ELISE is an upstream community project providing an opinionated, composable automation model
for deploying and managing enterprise Linux infrastructure — IdM, Satellite, AAP, and their
integrations — on bare metal, KVM, VMware, and cloud.

ELISE follows Red Hat recommended practice and configuration, giving operators a proven starting
point they can extend for their environment.

**ELISE is the upstream. RHIS (Red Hat Infrastructure Services) is the downstream.**
This mirrors the relationship between Fedora and RHEL, or upstream Kubernetes and OpenShift —
ELISE is where the community builds and governs; downstream products consume and extend it.

## Namespace

| Collection | Purpose |
|---|---|
| `elise.core` | Shared utilities and common patterns (this collection) |
| `elise.bootstrap` | Unattended RHEL installation via OEMDRV kickstart ISOs |
| `elise.satellite` | Red Hat Satellite — content, provisioning, disconnected workflows |
| `elise.idm` | Red Hat Identity Management (FreeIPA) configuration |
| `elise.aap` | Ansible Automation Platform configuration and pipelines |

## Status

This collection is in early development. The ELISE projects currently ship as individual
`rhis-builder-*` git repositories under the `parmstro` GitHub namespace. Collection packaging
is a planned evolution — the role and variable structure is already collection-compatible.

## Relationship to RHIS

```
elise-project (upstream community)
    └── elise.satellite, elise.idm, elise.aap, elise.bootstrap, elise.core

RHIS (downstream)
    └── Consumes and extends ELISE collections
    └── Red Hat supported configuration and integration
```

## Requirements

- ansible-core >= 2.15
- Python >= 3.9

## License

GPL-2.0-or-later

## Contributing

Contributions welcome. Please open issues and pull requests at
https://github.com/elise-project/elise-collection-core

## Author

parmstro (parmstro@redhat.com)
