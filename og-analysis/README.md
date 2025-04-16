# Log Analysis: Apache SSH Brute Force Attack

## 🔍 Incident Summary
While monitoring Apache logs from my EC2 instance, I observed a series of repeated failed login attempts from a single IP address — a textbook **brute force attack**.

## 📁 Log Evidence


## ⚠️ Indicators of Compromise (IOCs)
- IP: `185.234.219.201`
- Repeated login failures to SSH
- Attempted access to `admin` and `root` accounts

## 🛡️ Recommended Actions
1. Block the source IP using a firewall rule or `iptables`.
2. Set up Fail2Ban or another IDS to auto-block brute force attempts.
3. Ensure root login is disabled and MFA is enabled on privileged accounts.
4. Monitor for lateral movement or persistence techniques.

---

## 💬 Notes
This log analysis was conducted as part of my AWS cloud security training. I regularly review logs to detect real-world attack patterns and recommend mitigation strategies.
