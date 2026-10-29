# Lab report 01: Virtual cybersecurity lab setup

**Type:** Self-directed learning exercise  
**Tools:** VMware, Kali Linux, Metasploitable2  
**Evidence status:** Based on previously discussed lab configuration; original screenshots not yet attached.

## Aim

Practise setting up a repeatable environment for exploring Linux security tooling and a deliberately vulnerable Linux target.

## Work undertaken

- Worked with a Kali Linux VM for running security tools.
- Used a Metasploitable2 VM as the intentionally vulnerable target.
- Worked with NAT and host-only adapters for different connectivity needs.
- Maintained a named clean base snapshot to make the lab recoverable.

## Technical considerations

- A vulnerable target should not be bridged onto an untrusted physical network.
- Connectivity needs to be verified for each individual VM adapter.
- Snapshots reduce recovery time but do not replace secure network separation.

## Verification and evidence to add

- [ ] Screenshot of VMware adapter settings with sensitive details removed.
- [ ] Screenshot of the VM inventory showing the two lab machines.
- [ ] Date and versions of the environment used.
- [ ] Confirmation of a current host-only isolation test.

## Reflection

This exercise helped me understand the relationship between virtualisation, network interfaces, system isolation and safe security testing.
