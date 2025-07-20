# Troubleshooting Common Microsoft Teams Issues

This guide provides quick-reference solutions for common Microsoft Teams issues, along with diagnostic tools and escalation procedures to help administrators resolve problems effectively.

## Common Problems and Fixes

Use the following table to identify and resolve frequent user-reported issues:

| Issue                        | Resolution Steps                                                                 |
|-----------------------------|-----------------------------------------------------------------------------------|
| User can't sign in          | - Verify user has the correct Microsoft 365 license assigned.                     |
|                             | - Confirm Multi-Factor Authentication (MFA) settings in Azure Active Directory.  |
| App not loading             | - Clear the Teams client cache:                                                  |
|                             |   - Windows: `%appdata%\Microsoft\Teams`                                         |
|                             |   - macOS: `~/Library/Application Support/Microsoft/Teams`                      |
|                             | - Reinstall or update the Teams app.                                             |
| Audio/video not working     | - Run the Teams **Device Settings** test in the client.                          |
|                             | - Check microphone and speaker permissions.                                      |
|                             | - Ensure audio/video drivers are up to date.                                     |
| Can't schedule a meeting    | - Confirm Exchange Online mailbox is licensed and available.                     |
|                             | - Ensure Teams and Outlook calendar integration is enabled.                      |

## Diagnostic Tools

Administrators can use the following tools to analyze issues in real-time or retrospectively:

### Microsoft 365 Health Dashboard

- Provides real-time service status for Microsoft Teams and related services.
- Accessible via the Microsoft 365 Admin Center > Health > Service health.
- Useful for checking outages or service disruptions.

### Call Quality Dashboard (CQD)

- Offers organization-wide call and meeting quality insights.
- Enables investigation of audio, video, and network-related issues.
- Use filters to identify recurring issues by user, location, or device.

### Teams Network Planner

- Helps IT plan and optimize network readiness for Teams.
- Simulates bandwidth requirements and infrastructure needs for voice and video.

## Escalation Procedures

If an issue cannot be resolved with internal tools, escalate to Microsoft Support.

### How to Escalate

1. Open the **Microsoft 365 Admin Center**: [https://admin.microsoft.com](https://admin.microsoft.com)
2. Navigate to **Support > New service request**.
3. Provide:
   - A detailed description of the issue
   - Steps to reproduce
   - Affected users and timeframe
4. Include logs or screenshots if available.

## Best Practices

- Establish an internal triage process before escalating externally.
- Educate support teams on basic troubleshooting techniques.
- Maintain documentation of past incidents and resolutions.
- Proactively monitor service health to identify trends or recurring failures.

For in-depth diagnostics, visit the [Microsoft Teams Troubleshooting Documentation](https://learn.microsoft.com/en-us/microsoftteams/troubleshoot/teams-welcome).
