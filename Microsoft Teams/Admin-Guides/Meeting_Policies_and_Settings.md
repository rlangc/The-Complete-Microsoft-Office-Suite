# Managing Meetings in Microsoft Teams

This guide provides an overview of how administrators can manage meetings in Microsoft Teams through policies, best practices, and monitoring tools.

## Global and Per-User Policies

Meeting policies in Microsoft Teams determine what features are available to users before, during, and after meetings. These policies can be applied globally (org-wide) or tailored for specific users or groups.

### Key Policy Settings

- **Recording**
  - Enables or disables cloud recording of meetings.
  - Controls who can start a recording and where it is stored (OneDrive or SharePoint).

- **Transcription**
  - Allows live transcription during meetings.
  - Can be toggled on or off to support accessibility and post-meeting review.

- **Lobby Settings**
  - Defines who is admitted directly into the meeting and who must wait in the lobby.
  - Common settings include:
    - Everyone
    - People in my organization
    - Only invited users
    - Everyone except guests

### Where to Configure Policies

- Navigate to [https://admin.teams.microsoft.com](https://admin.teams.microsoft.com)
- Go to **Meetings** > **Meeting policies**
- Assign policies globally or per user using PowerShell or the Microsoft 365 admin portal

## Best Practices

Implementing thoughtful meeting policies improves security, collaboration, and compliance across the organization.

### Recommended Practices

- **Policy Segmentation**
  - Create different policies based on user roles:
    - Executives: Enable full meeting functionality
    - Frontline workers: Limit recording and transcription
    - Internal teams: Standard settings with some customization

- **Security Considerations**
  - Disable anonymous join to reduce risk of uninvited participants
  - Require lobby participation for external users
  - Limit who can present in meetings (e.g., only organizers)

- **Recording Governance**
  - Ensure compliance by managing who can record and how long recordings are retained
  - Use retention policies and expiration settings through Microsoft Purview

## Monitoring Meeting Health and Usage

Monitoring tools help administrators identify and troubleshoot meeting issues and assess adoption trends.

### Tools Available

- **Call Analytics**
  - Provides detailed diagnostics on individual call and meeting quality
  - Includes device, network, and endpoint metrics
  - Accessible via Microsoft Teams Admin Center

- **Call Quality Dashboard (CQD)**
  - Offers organization-wide trends and reporting on call quality
  - Useful for identifying systemic issues or high-risk locations

- **Usage Reports**
  - View usage metrics including meeting frequency, recording count, and feature adoption
  - Reports available through Microsoft 365 admin center and Power BI templates

## Summary Table

| Area              | Description                                             |
|-------------------|---------------------------------------------------------|
| Recording         | Enable or disable; control storage and permissions      |
| Transcription     | Optional feature for real-time and post-meeting review  |
| Lobby Controls    | Restrict or allow direct join for different participants|
| Policy Tiers      | Tailor policies by user role                            |
| Monitoring Tools  | Use Call Analytics and CQD for diagnostics              |

For more information, visit the [Microsoft Teams Meetings and Calling documentation](https://learn.microsoft.com/en-us/microsoftteams/meeting-policies-in-teams).
