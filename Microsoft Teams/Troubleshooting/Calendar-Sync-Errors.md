# Troubleshooting Calendar Sync Errors in Microsoft Teams

Microsoft Teams syncs with Outlook and Exchange Online to display calendar events. If meetings are missing or outdated, this guide provides steps to resolve sync issues between Teams and users' calendars.

## Symptoms of Calendar Sync Issues

- Calendar tab in Teams is empty or missing meetings
- New Outlook events don’t appear in Teams
- Error: “We couldn’t find your calendar”
- Inconsistent time zones between Outlook and Teams

## Checklist: End-User Fixes

### 1. Verify Outlook Access

- Confirm the user can access their calendar in Outlook Web App (OWA)
- If not, the issue lies with the mailbox or Exchange Online setup

### 2. Restart Teams and Outlook

- Close both apps completely
- Restart device and check again

### 3. Check Calendar Permissions (Delegates)

- Shared or delegate calendars may not appear in Teams
- Teams currently does not support displaying shared calendars in the Calendar view

### 4. Time Zone Mismatch

- Ensure time zone settings match:
  - Teams: **Settings > General > Language**
  - Outlook Web: **Settings > View all Outlook settings > General > Language and time**

## Admin Troubleshooting

### 1. Check Microsoft Exchange Online License

- Teams calendar integration requires an Exchange Online mailbox
- Check that users have one assigned and provisioned

### 2. Mailbox Region

- Teams only supports mailboxes hosted in **Exchange Online**
- On-prem Exchange mailboxes won’t sync with Teams Calendar

### 3. Teams App Permissions

- Go to Teams Admin Center > Users
- Ensure correct meeting policy is assigned

## Diagnostic Tools

- Run **Microsoft Support and Recovery Assistant (SaRA)** with the “Outlook/Teams Calendar” troubleshooter:  
  https://aka.ms/SaRA-CalendarIssues

- Use PowerShell to confirm mailbox location:  
  ```powershell
  Get-Mailbox -Identity user@domain.com | FL Name, RecipientTypeDetails, RemoteRoutingAddress
  ```

## Resources

- Calendar Integration Overview:  
  https://learn.microsoft.com/en-us/microsoftteams/exchange-teams-interact

- Troubleshoot Missing Calendar in Teams:  
  https://learn.microsoft.com/en-us/microsoftteams/calendar-in-teams#troubleshooting

- Exchange Online Licensing Guide:  
  https://learn.microsoft.com/en-us/microsoft-365/enterprise/exchange-online
