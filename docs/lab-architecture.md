# Lab architecture

## Purpose

Build a separated practice environment for learning how hosts expose services and how analysts record network observations.

## Components used

| Component | Role |
| --- | --- |
| Kali Linux VM | Security analysis workstation |
| Metasploitable2 VM | Intentionally vulnerable learning target |
| VMware | Virtualisation platform |
| NAT adapter | Internet-facing connectivity for permitted updates, where enabled |
| Host-only adapter | Local communication between selected lab machines |

I have worked with both NAT and host-only configurations, but the **exact settings can vary between sessions**. The conceptual diagram in the main README is not a guarantee of total isolation.

## Safe setup guidance

1. Check each VM's adapter settings before starting exercises.
2. Keep vulnerable targets off bridged networks and avoid exposing them to untrusted networks.
3. Restrict target-to-internet access where practical; use an isolated host-only network for testing.
4. Create and label a clean snapshot to make experiments reversible.
5. Record a fresh IP address and topology privately for each session rather than committing it publicly.

## Validation checklist

- [ ] Confirm only intended VMs are reachable from the test VM.
- [ ] Confirm the vulnerable host cannot be reached from other household or public network segments.
- [ ] Save a fresh Kali VM snapshot.
- [ ] Record software versions privately.
- [ ] Take a sanitised screenshot of adapter settings (optional).

**Note:** This file documents a safe reference approach, not an audited inventory of the current home network.
