# Teams Security and Compliance Configuration

This guide outlines essential tools and governance practices for securing Microsoft Teams and ensuring compliance across your organization. It covers data protection, user access controls, monitoring, and audit readiness.

## Core Tools

Microsoft 365 provides integrated tools to secure Teams communications and data while meeting regulatory and operational compliance requirements.

### Data Loss Prevention (DLP)

- **Purpose**: Prevent users from sharing sensitive information (e.g., credit card numbers, SSNs) inside or outside the organization.
- **Capabilities**:
  - Monitor and restrict sharing via Teams chat or channel messages
  - Automatically block or warn users when sensitive data is detected
- **Configuration**:
  - Set up policies in Microsoft Purview Compliance Portal
  - Apply policies based on location, user groups, or sensitivity labels

### eDiscovery

- **Purpose**: Conduct legal holds and content searches across Teams for litigation or compliance reviews.
- **Capabilities**:
  - Search messages, channel conversations, and shared files
  - Place specific users or teams on hold to preserve content
- **Tools**:
  - Microsoft Purview eDiscovery (Standard or Premium)

### Retention Policies

- **Purpose**: Manage how long messages, files, and recordings are retained or deleted in Teams.
- **Use Cases**:
  - Comply with legal or internal policy requirements
  - Automatically delete messages after a defined period
- **Configuration**:
  - Create policies via Microsoft Purview > Data Lifecycle Management

### Safe Links and Safe Attachments

- **Purpose**: Protect users from malicious URLs and file attachments in Teams.
- **Safe Links**:
  - Scans URLs in real-time to block known phishing sites
  - Works in Teams chat, channel messages, and shared documents
- **Safe Attachments**:
  - Opens files in a sandbox to detect malware before delivery
- **Management**:
  - Enabled and managed through Microsoft Defender for Office 365

## Governance

Strong governance practices help enforce security policies, manage access, and track activity across your Teams environment.

### Multi-Factor Authentication (MFA) and Conditional Access

- **MFA**:
  - Requires users to verify their identity using a second method (e.g., app code, phone)
  - Strongly recommended for all users, especially administrators

- **Conditional Access**:
  - Enforce controls based on user, location, device compliance, and risk level
  - Example: Block access from unmanaged devices outside corporate network

- **Configuration**:
  - Set policies in Azure Active Directory > Conditional Access

### Audit Logs

- **Purpose**: Track user and administrator actions across Teams
- **Activities Tracked**:
  - Team creation and deletion
  - File access and sharing
  - Policy changes and admin activity
- **Use Cases**:
  - Investigate security incidents
  - Monitor compliance with internal policies
- **Access**:
  - Available in Microsoft Purview > Audit

## Summary Table

| Tool/Policy              | Purpose                                              |
|--------------------------|------------------------------------------------------|
| Data Loss Prevention     | Prevent sensitive data sharing in chats and files    |
| eDiscovery               | Search and preserve content for legal purposes       |
| Retention Policies       | Control data lifecycle and message retention         |
| Safe Links/Attachments   | Protect users from malicious links and files         |
| MFA and Conditional Access | Secure access based on risk and user/device criteria |
| Audit Logs               | Monitor and report on Teams activity                 |

## Best Practices

- Regularly review DLP and retention policies with legal and compliance teams.
- Enable MFA for all users and configure granular conditional access policies.
- Establish a process for periodic audit log reviews and escalation.
- Document governance and security procedures as part of your IT compliance framework.

For setup guidance and advanced configuration, visit the [Microsoft Security and Compliance Documentation](https://learn.microsoft.com/en-us/microsoftteams/security-compliance-overview).
