# Troubleshooting Meeting Join Issues in Microsoft Teams

When users are unable to join a Microsoft Teams meeting, the issue may be due to authentication errors, calendar sync failures, browser settings, or policy restrictions. This guide provides structured steps to diagnose and resolve join issues.

---

## 🔍 Common Symptoms

- “Something went wrong” error when clicking join link
- Stuck on “Connecting…” screen
- Join button not visible in calendar
- Meeting link opens Teams but not the meeting
- Audio/Video devices not connecting after joining

---

## ✅ Step-by-Step Troubleshooting

### 1. Check Join Method

- Try using both the **Teams desktop app** and **web browser**
- Use the **Teams mobile app** as a backup method

### 2. Clear Local Cache (Desktop App)

- Fully quit Teams
- Delete cache folders:
  - `%appdata%\Microsoft\Teams` (Windows)
  - `~/Library/Application Support/Microsoft/Teams` (Mac)
- Restart Teams and attempt to join again

### 3. Use Incognito/Private Browser (Web)

- Open the meeting link in a private browser session
- Confirm Teams cookies and scripts are allowed

### 4. Check Microsoft 365 Calendar Integration

- Open Outlook or Teams Calendar
- Ensure the meeting appears on the correct calendar
- If it doesn’t appear:
  - Confirm Exchange Online license is assigned
  - Check if calendar sync is delayed

### 5. External or Guest User Issues

- Guest may not be properly authenticated
- Ensure the meeting organizer allows guest access
- Organizer should:
  - Open meeting options > "Who can bypass the lobby"
  - Ensure guest emails are invited properly

---

## 🔒 Meeting Policy Settings (Admin-Level)

| Setting | Impact |
|---------|--------|
| Allow anonymous join | If disabled, external users can’t access the meeting |
| Lobby configuration | May cause attendees to wait indefinitely |
| Video and audio settings | May restrict functionality for some users |

Admins can adjust these under:  
**Teams Admin Center > Meetings > Meeting Policies**

---

## 🧪 Diagnostic Tips

- Run Teams Meeting Join Troubleshooter in SaRA tool: https://aka.ms/SaRA-Teams
- Try from a different network or device
- Ensure Teams service is healthy: https://portal.office.com/servicestatus

---

## 📞 Escalation

If all steps fail:

- Ask the meeting organizer to resend the invite
- Use a direct link (copy-paste into browser)
- Open a Microsoft 365 support ticket via Admin Center

---

## Resources

- Manage Meeting Policies:  
  https://learn.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams
- Teams Guest Access Settings:  
  https://learn.microsoft.com/en-us/microsoftteams/guest-access