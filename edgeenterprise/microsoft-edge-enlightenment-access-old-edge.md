---
title: "Access the old version of Microsoft Edge"
ms.author: jtkim
author: dan-wesley
manager: srugh
ms.date: 08/19/2019
audience: ITPro
ms.topic: conceptual
ms.prod: microsoft-edge
localization_priority: medium
ms.collection: M365-modern-desktop
description: "How to access the old version of Microsoft Edge."
---

# How to access the old version of Microsoft Edge after installing the new version

This article describes how access the old version of Microsoft Edge after the new version is installed.

> [!NOTE]
> This article applies to Microsoft Edge stable version 79 or later.

The procedures in this article apply to systems that have been updated with the latest security updates, up to and including November 2019. When the next version of Microsoft Edge is installed, the old version will be hidden. All  attempts to launch the old version will  redirect the user to the newly installed version Microsoft Edge.

## How operating system (OS) changes are triggered

After the systems are fully updated and [Anaheim stable] is installed, the following registry key is set:<br>

```
"SOFTWARE\Microsoft\EdgeUpdate\ClientState\{56EB18F8-B008-4CBD-B6D2-8C97FE7E9062}"
Value: "BrowserReplacement"
```

> [!IMPORTANT]
> This key is over-written every time [Anaheim stable] is updated. As a best practice, we recommend that you don’t delete this key to allow users to access both versions of Microsoft Edge.


## How to enable a side-by-side experience with both versions of Microsoft Edge

If you want to allow your users to see both versions of Microsoft Edge…….
