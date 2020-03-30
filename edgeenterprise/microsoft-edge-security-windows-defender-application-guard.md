---
title: "Microsoft Edge and Windows Defender Application Guard"
ms.author: srugh
author: dan-wesley
manager: seanlyn
ms.date: 03/30/2020
audience: ITPro
ms.topic: conceptual
ms.prod: microsoft-edge
ms.localizationpriority: high
ms.collection: M365-modern-desktop
description: "Microsoft Edge support for Windows Defender Application Guard"
---

# Microsoft Edge support for Windows Defender Application Guard

This article describes how Microsoft Edge supports Windows Defender Application Guard.

> [!NOTE]
> This article applies to Microsoft Edge version 77 or later.

## Security overview

Browsers remain the primary attack surface on client devices because the browser's basic job is to let users access, download, and open untrusted content from untrusted sources. Malicious actors are constantly working to social engineer new forms of attacks against the browser. Security incident prevention or detection/response strategies can't guarantee 100% safety.

 The Assume Breach principle is a key security strategy. Adopt this strategy and ensure that corporate network and other resources remain protected in this scenario. For more information, see [Monitoring and testing tenant boundaries in Office 365](https://docs.microsoft.com/office365/Enterprise/office-365-monitoring-and-testing).

## About Windows Defender Application Guard

Designed for Windows 10 and Microsoft Edge, Windows Defender Application Guard uses a hardware isolation approach. This approach lets untrusted site navigations launch inside a container. Hardware isolation helps enterprises safeguard their corporate network and data in an assumed breach scenario while users browse the Internet.

The enterprise administrator defines what are trusted sites, cloud resources, and internal networks. Consider everything that's not in the trusted sites list to be untrusted. Isolate those sites from the corporate network and data on a user's device.

For more information, see [What is Application Guard and how does it work?](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-application-guard/wd-app-guard-overview#what-is-application-guard-and-how-does-it-work).

## Prerequisites

The following  requirements apply to devices using Windows Defender Application Guard with Microsoft Edge:

- Windows 10 1809 (RS5) and above.
- Only Windows client SKUs
- One of the management solutions described in [Software requirements](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-application-guard/reqs-wd-app-guard#software-requirements)

## How to install Windows Defender Application Guard

The following articles provide the information you need to install, configure, and test Windows Defender Application Guard with Microsoft Edge.

- [System requirements](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-application-guard/reqs-wd-app-guard)
- [Install Windows Defender Application Guard](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-application-guard/install-wd-app-guard)
- [Configure Windows Defender group policy settings](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-application-guard/configure-wd-app-guard)
- [Test Application Guard](https://docs.microsoft.com/windows/security/threat-protection/windows-defender-application-guard/test-scenarios-wd-app-guard)

## See also

- [Microsoft Edge Enterprise landing page](https://aka.ms/EdgeEnterprise)
- [Security overview](security-overview.md)
- [Windows Defender Advanced Threat Protection](https://query.prod.cms.rt.microsoft.com/cms/api/am/binary/RE2O8jv)
