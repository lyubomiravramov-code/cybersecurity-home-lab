# Network reconnaissance methodology

## Objective

Observe hosts and network services on an **explicitly authorised lab segment**, then record what the observations do and do not prove.

## Workflow

1. **Scope:** Name the virtual target, establish authorisation and confirm the lab's subnet privately.
2. **Connectivity:** Check host reachability and verify the VM network configuration.
3. **Discovery:** Use appropriate Nmap host discovery against the lab target only.
4. **Enumeration:** Inspect relevant TCP ports and detect service versions.
5. **Review:** Separate confirmed open ports from inferred product identity or vulnerability status.
6. **Document:** Save scan date, command, sanitised output and limitations.
7. **Suggest mitigations:** Remove unnecessary services, isolate testing targets and patch supported systems.

## Evidence standards

Every claim in a new report should say whether it is:

- **Observed:** supported by dated command output or a screenshot.
- **Previously noted:** described from earlier notes without new evidence attached.
- **Hypothesis:** a possible risk requiring validation.

An open port is not proof of compromise or exploitable vulnerability.
