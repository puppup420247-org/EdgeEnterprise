---
title: "Microsoft Edge privacy policy"
ms.author: likravit
author: dan-wesley
manager: srugh
ms.date: 07/29/2019
audience: ITPro
ms.topic: conceptual
ms.prod: microsoft-edge
localization_priority: medium
ms.collection: M365-modern-desktop
description: "Using Microsoft Edge privacy policy settings"
---

# Microsoft Edge privacy policy

Microsoft is committed to providing enterprises with the information and controls needed to make choices about data collection in Microsoft Edge.

By default, the Enterprise Canary and Developer channels of Microsoft Edge don’t send diagnostic data or site information to Microsoft. You can configure how Microsoft Edge handles data collection for your organization with the following group policies:

- Enable usage and crash-related data reporting.
- Send site information to improve Microsoft services.

## Policy settings

Download and use the latest Microsoft Edge Policy Template (For more information, see [Configure Microsoft Edge](configure-microsoft-edge.md).

### Enable usage and crash-related data reporting

For Windows 10 Beta and Stable channels of Microsoft Edge.

When configured, this policy will override the Windows diagnostic data setting for collection or non-collection of Microsoft Edge usage and crash related data. For more information, see [Configure Windows diagnostic data in your organization](https://go.microsoft.com/fwlink/?linkid=2099569).

- Enable this policy to send reporting of usage and crash-related data to Microsoft.
- Disable this policy if you don't want to send this data to Microsoft.

When configured, users can't change or override the policy setting.

When this policy isn't configured:

- On Windows 10 Beta and Stable channels. Microsoft Edge defaults to the Windows diagnostic data setting.
- On Windows 10 Canary and Dev channels. Microsoft Edge defaults to the user’s preference.
- On Windows 7, 8, and MacOS. Microsoft Edge defaults to the user’s preference.

### Send site information to improve Microsoft services

For Windows 10 Beta and Stable channels of Microsoft Edge.

When configured, this policy will override the Windows diagnostic data setting for collection or non-collection of Microsoft Edge website browsing information. For more information, see [Configure Windows diagnostic data in your organization](https://go.microsoft.com/fwlink/?linkid=2099569).

This policy setting lets you decide whether users can send information about websites they visit with Microsoft Edge to Microsoft. This information is used to improve services like Microsoft Search.

- Enable this policy to send information about the websites you visit with Microsoft Edge to Microsoft.
- Disable this policy if you don't want to send website browsing information to Microsoft.

When this policy isn't configured:

- On Windows 10, Beta and Stable channels. Microsoft Edge defaults to the Windows diagnostic data setting.
- On Windows 10, Canary and Dev channels. Microsoft Edge defaults to the user’s preference.
- On Windows 7, 8, and MacOS. Microsoft Edge defaults to the user’s preference.

## Additional privacy policy options

You may want to consider the following group policies related to data privacy:

- Block cookies on specific sites
- Block third party cookies
- Configure Do Not Track
- Disable InPrivate mode

## See also

- [Microsoft Edge policies](microsoft-edge-policies.md)
