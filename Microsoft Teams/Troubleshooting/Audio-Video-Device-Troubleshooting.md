# Audio and Video Device Troubleshooting in Microsoft Teams

Issues with microphones, speakers, or cameras can disrupt meetings and calls in Microsoft Teams. This guide helps diagnose and resolve device-related problems on desktop and web clients.

## Common Symptoms

- Microphone not detected or audio is low
- Camera not showing or blank screen during video calls
- Participants can’t hear or be heard
- Audio/video settings not saving
- Feedback, echo, or distorted sound

## User-Side Checklist

### 1. Test Devices in Teams

- Go to **Settings > Devices**
- Select correct microphone, speaker, and camera
- Click **Make a test call** to validate

### 2. Check Physical Connections

- Ensure the device is properly plugged in or paired (Bluetooth)
- Try a different USB port or headset if applicable

### 3. Update Device Drivers

- Update audio and video drivers via **Device Manager** (Windows)
- Install latest OS updates (macOS/Windows)

### 4. Close Conflicting Applications

- Close apps that may control or block devices (e.g., Zoom, OBS, Skype)
- Restart Teams and test again

## Browser Troubleshooting (Web)

- Ensure browser has permission to access microphone/camera
- In Chrome or Edge:
  - Click the lock icon in address bar
  - Allow mic and camera permissions
- Use **Incognito mode** to test for extensions causing conflicts

## Advanced Tips

| Issue | Resolution |
|-------|------------|
| Echo or feedback | Ask all users to use headphones |
| Audio delay | Switch from Bluetooth to wired headset |
| Camera flips image | Adjust settings in camera app or drivers |
| Mic volume too low | Manually raise input volume in OS settings |

## Admin-Level Settings

- Use Teams Admin Center > **Devices** to push configurations
- Check **Meeting policies** to ensure video is not disabled
- Use device logs for Teams-certified hardware (e.g., Teams Rooms)

## Resources

- Teams Device Settings:  
  https://learn.microsoft.com/en-us/microsoftteams/hardware-requirements

- Troubleshoot Teams Media Issues:  
  https://learn.microsoft.com/en-us/microsoftteams/troubleshoot/meetings/audio-video-issues

- Manage Devices in Teams Admin Center:  
  https://learn.microsoft.com/en-us/microsoftteams/manage-devices
