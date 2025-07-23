# Troubleshooting Teams Crashing or Not Starting

If Microsoft Teams is crashing, freezing, or failing to launch, it can often be resolved by clearing the cache, updating the app, or resolving conflicts with other software. This guide walks through common causes and fixes.

## Common Symptoms

- Teams doesn't open when launched
- "Microsoft Teams has stopped working" error
- Teams freezes or becomes unresponsive
- App closes immediately after opening
- Loading screen remains indefinitely

## Basic User Fixes

### 1. Restart Device

- Fully shut down and restart your PC or Mac
- Launch Teams again

### 2. Clear Teams Cache (Desktop App)

#### Windows:
1. Fully quit Teams from the system tray
2. Navigate to `%appdata%\Microsoft\Teams`
3. Delete contents of the following folders (do not delete the folders themselves):
   - `Application Cache`
   - `Blob_Storage`
   - `Cache`
   - `databases`
   - `GPUCache`
   - `IndexedDB`
   - `Local Storage`
   - `tmp`
4. Restart Teams

#### Mac:
- Navigate to `~/Library/Application Support/Microsoft/Teams`
- Delete the same folders as listed above

### 3. Reinstall Teams

- Uninstall Teams via Control Panel or Finder
- Download the latest version: https://teams.microsoft.com/downloads

## Advanced Troubleshooting

### Windows Event Viewer

- Check `Application` logs for Teams crashes
- Look for `.NET` or JavaScript errors

### Task Manager

- End any stuck **Teams.exe** processes
- Check for background apps consuming excess memory

## 🛠 Admin-Level Remediation

- Use Intune or Configuration Manager to push updates
- Check system policies or software restrictions preventing Teams execution
- Confirm antivirus or endpoint protection is not quarantining Teams

## Web Client Alternative

- If Teams won't start, use the web version: https://teams.microsoft.com
- Helpful for isolating desktop-specific issues

## Resources

- Microsoft Teams Installation Guide:  
  https://learn.microsoft.com/en-us/microsoftteams/install

- Teams Desktop Troubleshooting:  
  https://learn.microsoft.com/en-us/microsoftteams/troubleshoot/teams-sign-in/app-will-not-start

- Clean Install Guide:  
  https://learn.microsoft.com/en-us/microsoftteams/scripts/powershell-script-removes-teams
