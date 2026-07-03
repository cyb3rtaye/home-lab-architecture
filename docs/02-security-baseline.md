# Security Baseline

## Ubuntu Security Tooling VM

- keep operating-system packages updated
- use a standard account for daily work and `sudo` only when required
- document packet-capture and alert-log locations
- confirm system time before collecting evidence
- restrict unnecessary inbound services

## Windows 10 Workstation VM

- keep Microsoft Defender and Windows Firewall enabled unless a test requires a documented exception
- use a dedicated lab account for controlled activity
- confirm Windows event-log availability
- restore temporary security changes after testing

## Evidence Handling

- store only lab-generated screenshots and captures
- do not commit credentials, tokens, private keys or personal data
- use clear filenames that describe the test and evidence source
- record command, source, target and timestamp for repeatability

## Lab Operating Rules

- perform testing only against systems owned and controlled in the lab
- avoid exposing intentionally vulnerable services to public networks
- take a VM snapshot before significant configuration changes
- document deviations from the baseline
