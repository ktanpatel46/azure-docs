---
title: Configure monitoring coverage
description: Learn how to configure the different monitoring components that are available in Defender for Servers in Microsoft Defender for Cloud.
ms.topic: install-set-up-deploy
ms.date: 01/25/2024
---

# Configure monitoring coverage

Microsoft Defender for Cloud's Defender for Servers plans contains components that monitor your environments to provide extended coverage on your servers. Each of these components can be enabled, disabled or configured to your meet your specific requirements. 

| Component | Availability | Description | Learn more |
|--|--|--|--|
| [Log Analytics agent](plan-defender-for-servers-agents.md) | Plan 1 and Plan 2 | Collects security-related configurations and event logs from the machine and stores the data in your Log Analytics default or custom workspace for analysis. | [Learn more](../azure-monitor/agents/log-analytics-agent.md) about the Log Analytics agent. |
| [Vulnerability assessment for machines](deploy-vulnerability-assessment-defender-vulnerability-management.md) | Plan 1 and Plan 2 |Enables vulnerability assessment on your Azure and hybrid machines. | [Learn more](monitoring-components.md) about how Defender for Cloud collects data. |
| [Endpoint protection](integration-defender-for-endpoint.md) | Plan 1 and Plan 2 | Enables protection powered by Microsoft Defender for Endpoint, including automatic agent deployment to your servers, and security data integration with Defender for Cloud | [Learn more](integration-defender-for-endpoint.md) about endpoint protection. |
| [Agentless scanning for machines](concept-agentless-data-collection.md) | Plan 2 | Scans your machines for installed software and vulnerabilities without relying on agents or impacting machine performance. | [Learn more](concept-agentless-data-collection.md) about agentless scanning for machines. |

When you enable Defender for Servers plan 2, all of these components are toggled to **On** by default.

## Configure Log Analytics agent

After enabling the Log Analytics agent, you'll be presented with the option to select which workspace should be utilized.

**To configure the Log Analytics agent**:

1. Select **Edit configuration**.

    :::image type="content" source="media/configure-servers-coverage/edit-configuration-log.png" alt-text="Screenshot that shows you where on the screen you need to select edit configuration, to edit the log analytics agent/azure monitor agent." lightbox="media/configure-servers-coverage/edit-configuration-log.png":::

1. Select either a **Default workspace(s)** or a **Custom workspace** depending on your need.

    :::image type="content" source="media/configure-servers-coverage/auto-provisioning-screen.png" alt-text="Screenshot of the auto provisioning configuration screen with the available options to select." lightbox="media/configure-servers-coverage/auto-provisioning-screen.png":::

1. Select **Apply**.

1. Select **Continue**.

## Configure vulnerability assessment for machines

Vulnerability assessment for machines allows you to select between two vulnerability assessment solutions:

- Microsoft Defender Vulnerability Management
- Microsoft Defender for Cloud integrated Qualys scanner

**To select either of the vulnerability assessment solutions**:

1. Select **Edit configuration**.

    :::image type="content" source="media/configure-servers-coverage/vulnerability-edit.png" alt-text="Screenshot that shows you where to select edit for vulnerabilities assessment for machines." lightbox="media/configure-servers-coverage/vulnerability-edit.png":::

1. In the Extension deployment configuration window, select either of the solutions depending on your need.

1. Select **Apply**.

1. Select **Continue**.

## Configure endpoint protection

With Microsoft Defender for Servers, you enable the protections provided by [Microsoft Defender for Endpoint](/microsoft-365/security/defender-endpoint/microsoft-defender-endpoint?view=o365-worldwide) to your server resources. Defender for Endpoint includes automatic agent deployment to your servers, and security data integration with Defender for Cloud.

To configure endpoint protection:

1. Toggle the switch to **On**.

1. Select **Continue**.

## Configure agentless scanning for machines

Defender for Cloud has the ability to scan your Azure machines for installed software and vulnerabilities without requiring you to install agents, have network connectivity or affect your machine's performance.

**To configure agentless scanning for machines**:

1. Select **Edit configuration**.

    :::image type="content" source="media/configure-servers-coverage/agentless-scanning-edit.png" alt-text="Screenshot that shows where you need to select to edit the configuration of the agentless scanner." lightbox="media/configure-servers-coverage/agentless-scanning-edit.png":::

1. Enter a tag name and tag value for any machines to be excluded from scans.

1. Select **Apply**.

1. Select **Continue**.

Learn more about agentless scanning and how to [enable agentless scanning](enable-agentless-scanning-vms.md) on other cloud environments.
