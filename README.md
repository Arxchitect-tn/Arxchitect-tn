# Ajibola Lawal

### Self-hosted infrastructure · Agent automation · Diagnostic tooling

I build tools for running and troubleshooting systems: routing work across agent containers, monitoring a homelab, adapting API clients, and collecting Windows crash evidence remotely.

Based in Ontario, Canada. Currently working on agentic evaluation tooling and unattended automation on self-hosted hardware.

[Explore my repositories](https://github.com/Arxchitect-tn?tab=repositories) · [Project highlights](#project-highlights) · [Engineering-focus](#engineering-focus)

## Project highlights

| Project | What it solves | Built with |
| --- | --- | --- |
| [agent-mesh-dispatch](https://github.com/Arxchitect-tn/agent-mesh-dispatch) | Routes agent roles to containerized CLIs and coordinates a write → review → final-review pipeline. Includes a restricted SSH command entry point for scheduler integration. | Bash · Docker |
| [homelab-sentinel](https://github.com/Arxchitect-tn/homelab-sentinel) | Collects Linux host and container health into timestamped reports with graded exit codes, so warnings remain distinct from failures. | Bash · Linux · systemd |
| [provider-shim](https://github.com/Arxchitect-tn/provider-shim) | Adapts routing and authentication headers between API clients and a configured upstream endpoint. | JavaScript · Node.js |
| [windows-crash-triage](https://github.com/Arxchitect-tn/windows-crash-triage) | Collects Windows event-log evidence and minidump inventories over SSH, with a watchdog for newly observed errors. | Python · PowerShell · OpenSSH |

## Engineering focus

- **Observable automation.** Plain-text reports, explicit status codes, and state derived from the systems that actually run.
- **Clear trust boundaries.** Restricted scheduler commands, separate agent identities, and documented deployment assumptions.
- **Small, inspectable tools.** Scripts and adapters with direct configuration and few moving parts.
- **Evidence before conclusions.** Diagnostics that collect signals without pretending to replace a debugger or prove a root cause.

## Explore the work

Each project documents its own prerequisites, configuration, and limitations. Start with the README, then follow the implementation to see how the pieces fit together.

Questions and improvements belong in the relevant repository's issues or pull requests. Please keep credentials, private hostnames, and unsanitized diagnostic logs out of public reports.
