# Home Lab Architecture

## Overview

This repository documents the original VirtualBox lab used for network monitoring, controlled traffic generation and detection practice.

## Assets

| System | Address | Role |
|---|---:|---|
| Ubuntu VM | `192.168.1.3/24` | Security tooling, packet capture and network monitoring |
| Windows 10 VM | `192.168.1.4/24` | User workstation and controlled traffic generator |

## Network

- Subnet: `192.168.1.0/24`
- Documented gateway: `192.168.1.1`
- Virtualisation: VirtualBox
- Testing: isolated from production systems

## Repository Structure

```text
home-lab-architecture/
├── assets/
│   ├── diagrams/
│   └── screenshots/
├── docs/
│   ├── 00-architecture.md
│   ├── 01-network-plan.md
│   └── 02-security-baseline.md
└── README.md
```

## Documentation

- [`docs/00-architecture.md`](docs/00-architecture.md) — topology and system roles
- [`docs/01-network-plan.md`](docs/01-network-plan.md) — addressing and connectivity tests
- [`docs/02-security-baseline.md`](docs/02-security-baseline.md) — baseline controls and operating rules

## Evidence

- [Network diagram](assets/diagrams/network-diagram.png)
- [Ubuntu connectivity test](assets/screenshots/ubuntu-ping-test.png)
- [Windows connectivity test](assets/screenshots/windows-ping-test.png)
- [Host isolation evidence](assets/screenshots/host-isolation.png)

## Security Scope

All testing was performed inside a controlled, non-production lab.
