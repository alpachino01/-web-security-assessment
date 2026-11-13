# Findings Register

| ID | Area | Observation | Status | Recommended action |
|---|---|---|---|---|
| OBS-01 | Nmap | 10 TCP ports reported open as `tcpwrapped`; 971 filtered; some closed | Observation, not a vulnerability | Owner to confirm required exposed services and firewall policy |
| OBS-02 | HTTP headers | Nikto suggested reviewing HSTS, CSP, Permissions-Policy, X-Content-Type-Options, and Referrer-Policy | Configuration review recommended | Validate headers against application requirements |
| LIM-01 | Nikto coverage | 499 requests, approximately 7%; stopped at 20-error limit | Incomplete | Do not treat as a complete scan |
| LIM-02 | SQLmap | SSL/TLS-related error; no conclusive test result | Inconclusive | Do not infer SQL injection or its absence |
| OBS-03 | Availability | Operator reported slowdown after ~5 minutes; site remained reachable after ~20 minutes | Unverified observation | Review server/CDN/WAF telemetry; do not claim DDoS resistance |

## Severity
No confirmed vulnerability has been assigned a severity because the supplied evidence does not establish an exploitable weakness.
