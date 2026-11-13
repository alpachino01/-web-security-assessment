# Web Security Assessment (Initial, Non-Intrusive Review)

A beginner cybersecurity portfolio project documenting an initial web-security review using Kali Linux tools.

> **Safety and scope:** Publish this project only if you own the target or have explicit written authorization to assess it. The public version intentionally omits the target domain, IP address, raw scan output, and identifying screenshots. Do not upload information about a third-party system without permission.

## Project goals

- Review externally visible TCP port states with Nmap.

Review selected HTTP security-header observations with Nikto.

Document an SQLmap connectivity/TLS error without claiming an SQL-injection finding. Record performance observations separately from verified security-test results.

-Explain limitations and recommend defensive follow-up.

## Tools

-Kali Linux

Nmap

- Nikto

- SQLmap

## Summary of observations.

**Nmap: The captured output reported 10 TCP ports as 'open' with service detection shown as 'topwrapped, 971 ports as 'filtered', and some additional ports as closed. The service identities and firewall configuration were not independently confirmed.

-**Nikto:** The captured run targeted HTTP port 80, completed 499 requests (approximately 7%), reached a 20-error limit, and stopped before completion. It suggested reviewing several HTTP security headers.

**SOLmap:** The run did not complete because of an SSL/TLS-related error. This is inconclusive; it is not evidence that SQL injection is present or absent.

**Availability observation:** The operator reported degraded responsiveness after several minutes of multi-source traffic, while the site remained reachable after 20 minutes. This is an unverified observation, not a validated DDoS-resilience test.

## Important limitations

This was an initial and incomplete review, not a penetration test or certification. No confirmed exploitable vulnerability is documented. No claim is made that the target is secure or insecure.

## Repository contents

sanitized technical report REPORT.md

METHODOLOGY.md scope, safe workflow, and limitations FINDINGS.md concise findings and evidence confidence

EVIDENCE LOG_TEMPLATE.md template for future authorized evidence

DISCLAIMER.md authorization and responsible-disclosure notes

## Suggested next steps

1. Replace the scope placeholders in your private working copy with the authorized lab/asset details.

2. Keep the authorization record privately; do not publish personal or client information.

3. Add only sanitized screenshots from a lab you control.

4. Complete any follow-up checks only within the written scope.

5. Update the report with dates, tool versions, and reproducible evidence.

## Skills demonstrated

Network reconnaissance interpretation, web-server configuration review, tool-output analysis
evidence handling, technical reporting, and responsible security practice.
