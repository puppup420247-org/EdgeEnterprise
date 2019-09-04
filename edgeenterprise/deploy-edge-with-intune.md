---
title: "Deploy Microsoft Edge using Microsoft Intune"
ms.author: kvice
author: kelleyvice-msft
manager: laurawi
ms.date: 09/4/2019
audience: ITPro
ms.topic: procedural
ms.prod: microsoft-edge
localization_priority: medium
ms.collection: M365-modern-desktop
description: "Learn how to deploy Microsoft Edge with Microsoft Intune."
---

# Deploy Microsoft Edge using Microsoft Intune

This article shows you how to automate Microsoft Edge deployment and configuration for Windows and macOS by using Microsoft Intune.

>[!NOTE]
>This article applies to Microsoft Edge version 77 or later.

You can deploy Microsoft Edge to Windows and macOS clients that are managed in your company's Intune tenant by adding apps containing the Microsoft Edge installation files to Intune. You can deploy Microsoft Edge with either Mobile Device Management (MDM) or Mobile Application Management (MAM). Like any Intune apps, you can configure app assignments to force Microsoft Edge deployment to selected users or devices or make the app available in the Company Portal for users to install at their discretion.

You can also configure Microsoft Edge policies and settings by adding a Device Configuration Profile. If your company primarily uses Intune to manage and enforce policies on user devices, this is a good alternative to using Active Directory Group Policy or local GPOs.

You can read [Manage web access by using Microsoft Edge with Microsoft Intune](https://docs.microsoft.com/en-us/intune/manage-microsoft-edge) to learn more, but keep in mind that this article is specific to Microsoft Edge (EdgeHTML), not Microsoft Edge Enterprise (Chromium-based).

## Before you begin

Review the information in [Add a Windows line-of-business app to Microsoft Intune](https://docs.microsoft.com/en-us/intune/lob-apps-windows). This article contains procedures for adding an app like Edge Enterprise to your Microsoft Intune instance.

Download the Microsoft Edge Enterprise installation files (**MicrosoftEdgeDevEnterpriseX64.msi** and/or **MicrosoftEdgeDevEnterpriseX86.msi**) from the [Microsoft Edge Enterprise landing page](https://aka.ms/EdgeEnterprise).

If you also want to configure settings for Microsoft Edge using Intune, download the Microsoft Edge policy templates for Intune from the [Microsoft Edge Enterprise landing page](https://aka.ms/EdgeEnterprise). Make sure you download the policy template that matches the channel of your installation files (Beta or Dev).

Make sure you store the Microsoft Edge installation and policy files in an accessible network location.

## Add Microsoft Edge as an app in Intune

