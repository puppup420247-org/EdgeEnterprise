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

## Before you begin

Before using the detailed instructions in this article, consider the following 2 steps to enable a side-by-side browser experience. These steps will let your users run the current version of Microsoft Edge and the next version of Microsoft Edge (Beta channel) side-by-side.

1. Prevent the automatic install of the next version of Microsoft Edge by Windows Update. For more information, see [Windows Update: FAQ](https://support.microsoft.com/help/12373/windows-update-faq)
2. Install the [Beta channel](https://www.microsoftedgeinsider.com) of the next version of Microsoft Edge.

   > [!NOTE]
   > This side-by-side solution is less complex and requires less management that the detailed solution described in this article.

## How operating system (OS) changes are triggered

After the systems are fully updated and [Anaheim stable] is installed, the following registry key and value is set:

- Key: `SOFTWARE\Microsoft\EdgeUpdate\ClientState\{56EB18F8-B008-4CBD-B6D2-8C97FE7E9062}`
- Key value: `BrowserReplacement`

> [!IMPORTANT]
> This key is over-written every time [Anaheim stable] is updated. As a best practice, we recommend that you don’t delete this key to allow users to access both versions of Microsoft Edge.

## How to enable a side-by-side experience with both versions of Microsoft Edge

If you want to allow your users to see both versions of Microsoft Edge…….
