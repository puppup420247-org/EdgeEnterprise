---
title: "Overview of Microsoft Edge security"
ms.author: srugh
author: srugh
manager: seanlyn
ms.date: 7/12/2019
audience: ITPro
ms.topic: conceptual
ms.prod: microsoft-edge
localization_priority: high
ms.collection: M365-modern-desktop
description: "Overview of deploying Microsoft Edge security"
---

# Overview of Microsoft Edge security
  
> [!NOTE]
> This article applies to Microsoft Edge version 77 or later.

IT admins in the enterprise are constantly facing a myriad of existing and emerging security challenges while protecting the corporate network and devices from malicious attacks and preventing unauthorized access and leaks of corporate data. Microsoft Edge provides several natively built, unique capabilities that help address these challenges.

## Conditional Access
A key aspect of cloud security is identity and access when it comes to managing your cloud resources. In a mobile-first, cloud-first world, users can access your organization's resources using a variety of devices and apps from anywhere. As a result of this, just focusing on who can access a resource is not sufficient anymore, you also need to factor-in how a resource is accessed into an access control decision. Azure Active Directory (Azure AD) Conditional Access helps you master the balance between security and productivity.

Microsoft Edge natively supports Azure AD Conditional Access. Microsoft Edge profile associated with enterprise AAD credentials is all what is needed to allow seamless access to enterprise cloud resources protected using Conditional Access. This support is available across all platforms which includes all versions of Windows and MacOS. 

### How to deploy Conditional Access in Azure Active Directory 
[Deploy Conditional Access](https://docs.microsoft.com/en-us/azure/active-directory/conditional-access/plan-conditional-access) provides a detailed guide to help deoploy Conditional Access in Azure Active Directory,

## Application Guard
Browsers remain the primary attack surface on client devices today because it’s their fundamental job to download and execute untrusted content from untrusted sources. Security incident prevention or detection/response strategies cannot guarantee 100% safety. Malicious actors are constantly at work to social engineer new forms of attacks against the browser. One of the security strategies to consider is the Assume Breach principle and ensure corporate network and other resources remain protected in such scenarios. 

Designed for Windows 10 and Microsoft Edge, Application Guard uses hardware isolation approach, to isolate untrusted site navigations to launch inside a container. This helps enterprises safeguard their corporate network and data in assumed breach scenarios while the employees browse the Internet. The enterprise administrator defines what is a trusted web sites, cloud resources, and internal networks, everything not on that list is considered untrusted and gets isolated from the corporate network and data on the device. Learn more about Application Guard [here](https://docs.microsoft.com/en-us/windows/security/threat-protection/windows-defender-application-guard/wd-app-guard-overview). 

  > [!TIP] 
  > Application Guard in Microsoft Edge (Chromium-based) is supported only on Windows 10 1809 (RS5) and above.

The following links provide additonal information to get started using Application Guard with Microsoft Edge. 

- [System Requirements](https://docs.microsoft.com/en-us/windows/security/threat-protection/windows-defender-application-guard/reqs-wd-app-guard)
- [Installing Application Guard](https://docs.microsoft.com/en-us/windows/security/threat-protection/windows-defender-application-guard/install-wd-app-guard)
- [Configuring OS Policies for Application Guard](https://docs.microsoft.com/en-us/windows/security/threat-protection/windows-defender-application-guard/configure-wd-app-guard)

## Windows Information Protection 
Stay tuned. Support for Windows Information protection is coming soon. 

## See also

- [Overview of Microsoft Edge in the enterprise](overview-edge-in-the-enterprise.md)
- [Microsoft Edge Enterprise landing page](https://aka.ms/EdgeEnterprise)
