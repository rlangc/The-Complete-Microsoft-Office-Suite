# Troubleshooting Notification Problems in Microsoft Teams

If users are missing Teams notifications, it can affect collaboration and response times. This guide outlines how to diagnose and resolve issues related to banner alerts, emails, and feed notifications.

## Common Notification Issues

- No banners or sounds when receiving messages
- Notifications delayed or only visible in activity feed
- Missing missed call or voicemail alerts
- No badge count updates on desktop or mobile
- Quiet Hours or Focus Assist interfering with alerts

## User-Side Troubleshooting

### 1. Verify Teams Notification Settings

- Click on **Settings > Notifications**
- Ensure banner and sound are selected for:
  - Chat messages
  - Mentions
  - Meetings
  - Calls

### 2. Check Operating System Notification Settings

#### Windows:
- Go to **Settings > System > Notifications**
- Ensure Microsoft Teams is enabled for notifications

#### macOS:
- Open **System Preferences > Notifications**
- Select **Teams** and enable alerts and badges

### 3. Turn Off Focus Assist / Do Not Disturb

- Windows: **Action Center > Focus Assist** should be set to Off
- Mac: Check **Do Not Disturb** in **Control Center** or scheduled hours

## Mobile Notifications

- Open Teams > Tap your profile > **Notifications**
- Check push notification settings for calls, mentions, and messages
- Ensure OS-level permissions are enabled (iOS/Android Settings)

## Advanced Tips

| Issue | Fix |
|-------|-----|
| Delay in notifications | Log out and log back into Teams |
| Muted channel or chat | Click on “...” next to the chat > Unmute |
| Notification sounds missing | Re-enable sound alerts in Teams settings |
| No alerts during screen sharing | Teams suppresses alerts by design |

## Admin-Level Checks

- Confirm meeting/chat policies do not suppress alerts
- Check if a Quiet Hours policy is applied via Intune or endpoint manager
- Audit Teams update history for known notification bugs

## Resources

- Configure Notifications:  
  https://support.microsoft.com/en-us/office/manage-notifications-in-teams-1e6f0aa5-2a4b-4d55-8b11-8f331ec7945c

- macOS and Windows Notification Help:  
  https://learn.microsoft.com/en-us/microsoftteams/troubleshoot/notifications

- Mobile Notification Settings:  
  https://support.microsoft.com/en-us/office/change-notifications-on-mobile-devices-2b361938-5b07-45b1-9d70-36206eaeb3a5
