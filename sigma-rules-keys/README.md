# 🛡️ Custom SIGMA Rules — Keys Edition

This repo contains original SIGMA detection rules for:

- Windows AMSI bypass detection
- Rundll32 LOLBin abuse
- Linux LSASS dumping detection

## 📂 Structure

- `/sigma/windows` → Windows event logs
- `/sigma/linux` → Linux audit logs or process events
- `/convert` → sigmac configs for ELK, Splunk, Sentinel

## ⚙️ Example: Convert SIGMA to Splunk

```bash
sigmac -t splunk sigma/windows/win_susp_amsi_bypass.yml
```

## ✅ MITRE ATT&CK Mappings

- T1562.001 – Disable or Modify Tools
- T1218.011 – Signed Binary Proxy Execution: Rundll32
- T1003 – Credential Dumping (Linux)

> Stay proactive. Build detections before attackers build payloads.
