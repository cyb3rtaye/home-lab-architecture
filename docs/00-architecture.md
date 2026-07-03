# Lab Architecture

## Purpose

Provide a repeatable environment for packet capture, intrusion-detection testing, alert validation and investigation documentation.

## Topology

```text
+--------------------------------+       +--------------------------------+
| Ubuntu security tooling VM     |       | Windows 10 workstation VM      |
| 192.168.1.3/24                 |<----->| 192.168.1.4/24                 |
| Packet capture and monitoring  |       | Controlled traffic generation  |
+--------------------------------+       +--------------------------------+
                  VirtualBox lab network: 192.168.1.0/24
```

## System Roles

### Ubuntu VM

- packet capture
- network analysis
- Snort sensor testing
- security-tool administration

### Windows 10 VM

- normal user activity
- controlled discovery and command tests
- endpoint telemetry generation when logging tools are enabled

## Detection Objectives

1. Confirm network visibility between the two systems.
2. Establish normal traffic baselines.
3. Generate controlled activity for detection validation.
4. Capture evidence that can be reviewed and documented.

## Diagram

![Network diagram](../assets/diagrams/network-diagram.png)
