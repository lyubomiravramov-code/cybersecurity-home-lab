# Lab report 02: Nmap network reconnaissance

**Type:** Authorised laboratory reconnaissance  
**Tools:** Kali Linux, Nmap, Metasploitable2  
**Evidence status:** General steps and earlier observations; original scan log and dated screenshot pending.

## Aim

Identify services exposed by a deliberately vulnerable lab target and interpret their implications without confusing service discovery with proof of exploitation.

## Environment

The exercise involved Kali Linux and a Metasploitable2 target in a VMware virtual lab. Target addresses are intentionally omitted from this public portfolio.

## Approach

1. Confirm the intended Metasploitable2 virtual target and network scope.
2. Verify connectivity to the target inside the lab.
3. Perform authorised service discovery using Nmap.
4. Record open ports and any version hints returned by the tool.
5. Review the findings and decide which services warrant further defensive investigation.

See [`commands/nmap-reference.md`](../commands/nmap-reference.md) for annotated **example commands**, not asserted historic output.

## Previously noted observations

Earlier lab notes identified multiple services on the Metasploitable2 target and an intentionally broad attack surface. Database-related services were part of earlier analysis. **A current port-by-port result is not included here**, because a verifiable dated output has not been added.

## Interpretation

Exposed services can increase attack surface, especially when they are unnecessary, obsolete or poorly configured. However, Nmap version detection can be incomplete and a service banner alone does not confirm a vulnerability.

## Evidence to add

- [ ] Date of the lab session.
- [ ] Exact command run against the authorised VM.
- [ ] Sanitised Nmap output showing relevant ports.
- [ ] One screenshot demonstrating the scan in Kali Linux.
- [ ] Short explanation of two observed services and sensible mitigations.

## Reflection

I practised moving from raw scan observations to a structured security assessment and documenting uncertainty in my findings.
