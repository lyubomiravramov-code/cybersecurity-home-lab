# Nmap command reference (lab only)

**These are educational example commands, not a transcript of scans already performed.** Replace `<LAB_TARGET_IP>` with the IP address of an authorised isolated VM. Do not use these commands on public or third-party systems without permission.

## Confirm a lab target is reachable

```bash
nmap -sn <LAB_TARGET_IP>
```

`-sn` performs host discovery rather than port enumeration.

## Identify open TCP ports

```bash
nmap -sT --open <LAB_TARGET_IP>
```

`-sT` uses the TCP connect scanning method. `--open` limits displayed ports to open or possibly open states.

## Identify service versions on a specified port list

```bash
nmap -sV -p 21,22,80,443 <LAB_TARGET_IP>
```

`-sV` attempts service identification. The specified ports are illustrative: do not infer they were all present on the historical lab target.

## Save output for a report

```bash
nmap -sV -p 21,22,80,443 -oN lab-scan-local.txt <LAB_TARGET_IP>
```

Review and sanitise the saved file **before** deciding whether any excerpt can be shared publicly. Keep original logs private by default.

## Notes for interpreting results

- `open` means Nmap obtained evidence that a port accepts traffic; it does not mean a vulnerability was exploited.
- `filtered` means filtering prevents a definitive determination.
- Service names and version banners are indicative and may be inaccurate.
- Always record the scan date, scope and command when including real findings.
