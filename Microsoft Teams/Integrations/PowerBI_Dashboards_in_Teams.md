# Power BI Dashboards in Microsoft Teams

Power BI integrates directly with Microsoft Teams, allowing users to embed live dashboards, monitor KPIs, and collaborate on data insights without leaving the Teams environment. This guide outlines setup steps, use cases, and governance tips for embedding Power BI in Teams.

## Overview

Power BI and Teams work together to:

- Embed reports and dashboards as tabs in Teams channels
- Share insights during meetings and chats
- Enable faster data-driven decisions within collaboration spaces

## How to Add a Power BI Dashboard to Teams

### Option 1: From Teams

1. Navigate to the desired Teams channel.
2. Click **+ Add a tab** and select **Power BI**.
3. Choose the workspace and report you want to embed.
4. Click **Save** to display the report as a tab.

### Option 2: From Power BI

1. Open a report in Power BI (https://app.powerbi.com).
2. Click **File > Embed in Teams**.
3. Select the target team and channel to post the report.

## Use Cases

| Scenario                        | Benefit                                                |
|----------------------------------|--------------------------------------------------------|
| Sales team dashboard             | View quota progress, leads, and pipeline in real time  |
| Executive summary reports        | Align leadership with company-wide KPIs                |
| Project status reports           | Monitor timelines, risks, and milestones collaboratively|
| Helpdesk or service dashboards   | Track ticket resolution and customer satisfaction      |

## Permissions and Licensing

- Users must have a **Power BI Pro** or **Premium per User (PPU)** license to publish or view shared reports.
- Reports must reside in a **shared workspace**, not just in My Workspace.
- Ensure that team members have view or contributor permissions to access the embedded reports.

## Best Practices

- Use **row-level security (RLS)** to filter report data based on user roles.
- Create dedicated workspaces for each department or function.
- Limit the number of visualizations per report tab for performance and clarity.
- Regularly review report usage and refresh schedules.

## Security Considerations

- Audit report access via Power BI usage metrics and audit logs.
- Avoid embedding sensitive financial or HR reports unless secured by RLS.
- Align report data with compliance requirements (GDPR, HIPAA, etc.).

## Resources

- Power BI in Microsoft Teams Overview:  
  https://learn.microsoft.com/en-us/power-bi/collaborate-share/service-teams-integration
- Embed Power BI in Teams:  
  https://learn.microsoft.com/en-us/power-bi/collaborate-share/service-embed-report-teams
- Power BI Licensing Guide:  
  https://learn.microsoft.com/en-us/power-bi/fundamentals/service-license-types
