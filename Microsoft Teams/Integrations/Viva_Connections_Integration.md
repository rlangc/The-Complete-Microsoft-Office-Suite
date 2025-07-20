# Microsoft Viva Connections Integration with Teams

Microsoft Viva Connections brings together internal communications, company resources, and employee engagement tools into the Microsoft Teams environment. This guide outlines how to integrate Viva Connections into Teams and best practices for deployment.

## Overview

Viva Connections is a gateway to your digital workplace. It combines SharePoint, Yammer, Stream, and other Microsoft 365 services in a centralized experience accessible directly from Teams.

## Key Capabilities

- Personalized dashboard with links, cards, and widgets
- Curated news and announcements feed
- Access to SharePoint home sites from within Teams
- Custom branding and audience targeting
- Mobile-friendly experience via the Teams mobile app

## How to Set Up Viva Connections in Teams

1. Ensure your intranet has a **SharePoint home site** configured.
2. In the SharePoint admin center, set the site as the home site.
3. Customize your Viva dashboard via the **Dashboard** web part.
4. Use PowerShell to deploy the Viva Connections app to Teams:
   ```powershell
   Install-Module -Name Microsoft.Online.SharePoint.PowerShell
   Connect-SPOService -Url https://yourtenant-admin.sharepoint.com
   ```
5. Use the provided script and app package to pin Viva Connections as a Teams app.

> Reference deployment guide: https://learn.microsoft.com/en-us/viva/connections/viva-connections-overview

## Best Practices

- Design the dashboard around employee roles (e.g., frontline vs HQ staff).
- Use adaptive cards to show tasks, reminders, or company tools.
- Integrate links to HR systems, expense reports, IT support, and training portals.
- Brand the experience to reflect company culture and identity.
- Test the mobile experience for ease of access and usability.

## Use Cases

| Use Case                        | Description                                           |
|----------------------------------|-------------------------------------------------------|
| Company communications           | Central place for announcements, CEO messages         |
| New hire onboarding              | Launchpad for resources and orientation               |
| Unified access                   | One-click links to tools like policies, payroll, and time off |

## Governance and Security

- Access is controlled via Microsoft 365 group and SharePoint permissions.
- Customize access to content using audience targeting features.
- Ensure internal content is compliant with company policies.

## Resources

- Viva Connections Deployment Guide:  
  https://learn.microsoft.com/en-us/viva/connections/viva-connections-overview
- Create and manage the Viva dashboard:  
  https://learn.microsoft.com/en-us/viva/connections/viva-connections-dashboard
- Pin Viva Connections in Teams:  
  https://learn.microsoft.com/en-us/viva/connections/add-app-teams
