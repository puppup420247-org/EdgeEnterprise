---
title: "Troubleshoot Microsoft Edge"
ms.author: kvice
author: dan-wesley
manager: laurawi
ms.date: 10/07/2019
audience: ITPro
ms.topic: conceptual
ms.prod: microsoft-edge
ms.localizationpriority: high
ms.collection: M365-modern-desktop
description: "Troubleshoot Microsoft Edge"
---

# Troubleshoot Microsoft Edge

Use the information in this article to troubleshoot Microsoft Edge problems.

> [!NOTE]
> This article applies to Microsoft Edge version 77 or later.

## How do I resolve Error Code -2147024540?

This error code corresponds to the following Windows Information Protection error:
*ERROR_EDP_POLICY_DENIES_OPERATION: The requested operation was blocked by Windows Information Protection policy. For more information, contact your system administrator*.

Microsoft Edge shows this error when the organization has enabled Windows Information Protection (WIP) to only allow users with approved applications to access corporate resources. In this case because Microsoft Edge isn't on the approved applications list, the admin will have to update the WIP policies to grant access to Microsoft Edge. Please download and apply the policy update in the [WIP Enterprise AppLocker Policy](https://download.microsoft.com/download/8/9/9/8995d820-065c-4ab1-aa2a-9d6dc0cd7ffa/MsEdge%20-%20WIP%20Enterprise%20AppLocker%20Policy%20Files.zip) file.

## See also

- [Microsoft Edge enterprise tech community](https://techcommunity.microsoft.com/t5/Enterprise/bd-p/EdgeInsiderEnterprise)
- [Contact Microsoft Edge support](https://microsoftedgesupport.microsoft.com/hc/)
