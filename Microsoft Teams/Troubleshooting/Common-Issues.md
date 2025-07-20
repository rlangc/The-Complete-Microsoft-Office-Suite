# FAQs & Troubleshooting Wiki: Common Problems & Solutions

## General FAQs

### 1. What is Microsoft Teams used for?
Microsoft Teams is a collaboration platform that combines chat, video conferencing, file sharing, task management, and app integrations to streamline teamwork across organizations.

### 2. Is Microsoft Teams free?
Yes, Microsoft offers a free version of Teams with limited features. Full features are available through a Microsoft 365 subscription.

### 3. What are Teams, Channels, and Chats?
- **Teams** are groups of people collaborating together, typically organized by department or project.
- **Channels** are sub-sections within teams used to organize conversations by topic.
- **Chats** are direct messages between individuals or small groups outside of team spaces.

### 4. How do I schedule a meeting in Teams?
- Go to the **Calendar** tab.
- Click **New Meeting**.
- Add title, participants, date, and time.
- Click **Save** to send invites.

## Common Issues & Troubleshooting

### 1. Teams Won’t Open or Load

**Possible Causes:**
- Corrupt cache files
- Internet connectivity issues
- Outdated application

**Solutions:**
- Restart Teams.
- Clear Teams cache:
  - **Windows:** Press `Win + R`, enter `%appdata%\Microsoft\Teams`, and delete contents.
  - **Mac:** Go to `~/Library/Application Support/Microsoft/Teams/` and delete files.
- Update Teams.
- Try using the web version at [teams.microsoft.com](https://teams.microsoft.com).

### 2. Can’t Sign In to Microsoft Teams

**Possible Causes:**
- Incorrect credentials
- Expired password
- Multi-factor authentication (MFA) issues

**Solutions:**
- Confirm correct credentials.
- Reset password if needed.
- Disable VPNs temporarily.
- Verify MFA codes.

### 3. No Sound in Meetings or Calls

**Possible Causes:**
- Incorrect audio device settings
- Microphone muted
- Outdated drivers

**Solutions:**
- Check Teams audio device settings.
- Ensure microphone is unmuted.
- Update audio drivers.
- Restart the device.

### 4. Video Not Working in Meetings

**Possible Causes:**
- Camera being used by another app
- Incorrect device selected
- Browser permissions not enabled

**Solutions:**
- Close other applications using the camera.
- Select the correct camera in Teams settings.
- Allow camera access through system privacy settings.

### 5. Can’t Share Screen in a Meeting

**Possible Causes:**
- Insufficient sharing permissions
- Issues with multiple monitors
- Organizational restrictions

**Solutions:**
- Ensure screen sharing permissions are enabled.
- Restart Teams and your device.
- For Mac users: Allow screen recording in system preferences.

### 6. Teams Notifications Not Working

**Possible Causes:**
- Do Not Disturb mode enabled
- Misconfigured notification settings
- System notifications disabled

**Solutions:**
- Update Teams notification settings.
- Check system-level notification permissions.
- Restart Teams.

### 7. Can’t Add External Users (Guests) to a Team

**Possible Causes:**
- Guest access not enabled
- Restrictive organizational policies

**Solutions:**
- Enable guest access in Microsoft Teams Admin Center.
- Update external sharing settings in Microsoft 365 Admin Center.
- Invite external users using their valid email addresses.

### 8. How to Recover a Deleted Team or Channel

**Solutions:**
- **Teams:** Recover from **Microsoft 365 Admin Center** > **Groups** > **Deleted Groups**.
- **Channels:** Manage the team, view **Deleted Channels**, and restore.

### 9. Teams Crashing or Freezing

**Possible Causes:**
- Outdated app version
- Corrupt installation
- Conflicting background applications

**Solutions:**
- Update or reinstall Microsoft Teams.
- Close unnecessary background apps.
- Clear cache regularly.

## Advanced Troubleshooting for IT Admins

### 1. How to Force Log Out Users

- Use **Teams Admin Center**:
  - Navigate to **Users** > select the user > **Sign Out**.
- Or use PowerShell:

```powershell

Remove-CsOnlineUser -Identity "user@domain.com"

```
