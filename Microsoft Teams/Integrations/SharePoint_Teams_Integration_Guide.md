# SharePoint + Microsoft Teams Integration Guide

Microsoft Teams integrates deeply with SharePoint to enable centralized file sharing, collaborative editing, and information management across teams and departments. This guide outlines how to configure and optimize SharePoint-Teams integration.

---

## Overview

Each Microsoft Team has a corresponding SharePoint site automatically created to store files shared within channels. You can also manually link other SharePoint resources into Teams tabs, enhancing access and collaboration.

---

## Integration Points

### 1. Channel Files

- Files shared in a standard channel are stored in the **Documents** library of the connected SharePoint site.
- Each channel has its own folder under the **Documents** library.

**Access Path**:
Teams > Channel > Files tab > Open in SharePoint

### 2. Adding SharePoint Tabs

- Use the **+ Add a tab** option in any channel.
- Select **Document Library**, **Pages**, or **Lists** to embed SharePoint resources.

**Use Cases**:
- Link a centralized knowledge base page
- Embed a process flow or SOPs stored in a SharePoint page

### 3. Lists in Teams

- SharePoint lists can be added as standalone tabs using the **Lists** app.
- Supports custom views, forms, and workflows.

---

## Steps to Add a SharePoint Document Library to Teams

1. Navigate to the desired Teams channel
2. Click the **+** tab and select **Document Library**
3. Enter the SharePoint URL or choose from existing libraries
4. Name the tab and click **Save**

---

## Steps to Add a SharePoint Page to Teams

1. Click **+ Add a tab** in a channel
2. Select the **Website** app
3. Paste the full URL of the SharePoint page
4. Name the tab and save

---

## Best Practices

- Use permissions in SharePoint to restrict sensitive folders, even within a team.
- Avoid editing folder names directly in SharePoint, as it may desync Teams tabs.
- Educate users to use “Open in SharePoint” for advanced features like version history or document metadata.

---

## Governance Considerations

- Monitor storage quotas and retention policies on SharePoint sites.
- Enforce naming conventions and lifecycle policies for Teams and their linked SharePoint sites.
- Use SharePoint hub sites to structure interconnected Teams and knowledge repositories.

---

## Resources

- SharePoint and Teams Overview:  
  https://learn.microsoft.com/en-us/sharepoint/teams-overview
- Lists in Teams:  
  https://learn.microsoft.com/en-us/microsoftteams/manage-lists-in-teams
- Teams File Collaboration with SharePoint:  
  https://learn.microsoft.com/en-us/microsoftteams/files-sharepoint