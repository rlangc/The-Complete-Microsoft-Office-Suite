# Network Connectivity Checklist for Microsoft Teams

Microsoft Teams requires stable internet connectivity and access to specific Microsoft 365 services to function correctly. This guide provides a step-by-step checklist to diagnose and resolve common network-related issues in Teams.

---

## 🔍 Symptoms of Network Issues

- Calls drop unexpectedly or are choppy
- Delayed or undelivered messages
- Meeting audio/video lags or freezes
- Failure to join meetings or load Teams interface
- Frequent reconnection attempts

---

## ✅ Basic Connectivity Checks

1. **Test Internet Speed**
   - Ensure a minimum of 1.2 Mbps upload/download per user for high-quality video.
   - Use tools like [speedtest.net](https://www.speedtest.net) or Microsoft's [Network Testing Companion](https://aka.ms/NWC).

2. **Restart Router and Devices**
   - Restart the user's PC and internet router.
   - Ensure other devices aren’t consuming excess bandwidth (streaming, downloads, etc.).

3. **Switch Networks**
   - Try connecting to a different Wi-Fi or switch to a wired Ethernet connection.

---

## 🌐 Domain and Port Requirements

Teams relies on access to Microsoft 365 endpoints.

### Allow the Following URLs

- `*.teams.microsoft.com`
- `*.skype.com`
- `*.office365.com`
- `*.microsoftonline.com`

Full list: [Microsoft 365 URLs and IP ranges](https://learn.microsoft.com/en-us/microsoft-365/enterprise/urls-and-ip-address-ranges)

### Required Ports

| Protocol | Port | Usage           |
|----------|------|------------------|
| TCP      | 443  | HTTPS (Teams signaling) |
| UDP      | 3478–3481 | Media traffic (audio/video/screen sharing) |

---

## 🛠 Advanced Troubleshooting

- **Run Teams Network Planner**  
  Use the built-in [Network Planner](https://aka.ms/teamsnetworkplanner) to model Teams bandwidth needs.

- **Check Firewall and Proxy**  
  Ensure no blocking of required URLs/ports. Bypass SSL inspection for Microsoft 365 traffic.

- **Verify DNS Resolution**  
  Run `nslookup teams.microsoft.com` to confirm DNS is resolving properly.

- **Check VPN Configuration**  
  VPNs may throttle traffic or block UDP. Use split tunneling for Teams domains when possible.

---

## 🧪 Diagnostic Tools

- `Teams Connectivity Test` (browser): https://connectivity.office.com/
- `Microsoft Support and Recovery Assistant (SaRA)`: https://aka.ms/SaRA-Teams
- Ping/traceroute to test route latency and packet loss

---

## 📄 Escalation Guidance

If issues persist after local checks:

- Open Microsoft 365 Admin Center
- Navigate to **Health > Service Health**
- Submit a support request if a Teams service degradation is not listed

---

## Related Resources

- Teams Network Requirements:  
  https://learn.microsoft.com/en-us/microsoftteams/prepare-network

- Microsoft Connectivity Analyzer:  
  https://testconnectivity.microsoft.com