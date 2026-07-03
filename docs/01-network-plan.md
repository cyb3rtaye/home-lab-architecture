# Network Plan

## Addressing

| System | Address | Role |
|---|---:|---|
| Ubuntu VM | `192.168.1.3/24` | Monitoring and security tooling |
| Windows 10 VM | `192.168.1.4/24` | Workstation and traffic generator |
| Gateway | `192.168.1.1` | Gateway recorded in the original setup |

## Connectivity Validation

From Ubuntu:

```bash
ping 192.168.1.4
```

From Windows:

```powershell
ping 192.168.1.3
```

## Evidence

- [Ubuntu ping test](../assets/screenshots/ubuntu-ping-test.png)
- [Windows ping test](../assets/screenshots/windows-ping-test.png)
- [Host isolation](../assets/screenshots/host-isolation.png)

## Operational Notes

- Keep the test systems separated from production devices.
- Record address changes before running detection tests.
- Confirm the correct VirtualBox adapter before collecting evidence.
- Use timestamps consistently across systems when correlating events.
