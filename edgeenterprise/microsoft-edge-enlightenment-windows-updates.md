---
title: "Windows updates for Microsoft Edge"
ms.author: jtkim
author: dan-wesley
manager: srugh
ms.date: 08/19/2019
audience: ITPro
ms.topic: conceptual
ms.prod: microsoft-edge
localization_priority: medium
ms.collection: M365-modern-desktop
description: "Windows updates for Microsoft Edge."
---

# Windows updates to support the next version of Microsoft Edge

This article describes how Windows will be updated to support the next version of Microsoft Edge.

> [!NOTE]
> This article applies to Microsoft Edge stable version 79 or later.

## Microsoft Edge and the Windows release cycle

The next version of Microsoft Edge isn’t bound to the Windows release cycle. Because the browser is de-coupled from the operating system (OS), changes will be made to Windows to ensure that the next version of Microsoft Edge fits seamlessly into Windows. As a result, feature updates will be released on a 6 week cycle (approximately.) Security and compatibility updates  will be shipped as needed.

## Updates and the user experience

Updates won’t change the user experience until the stable channel of the next version of Microsoft Edge is installed. Installing Microsoft Edge Beta, Dev, or Canary won’t trigger any changes in Windows. These browser releases will be installed alongside existing browsers.

When all the updates are applied AND the stable channel of the next version of Microsoft Edge is installed at the system-level, the following changes will take effect on the system:

- All start menu pins, tiles, and shortcuts will migrate to the next version of Microsoft Edge.
- All taskbar pins and shortcuts will migrate to the next version of Microsoft Edge.
- The next version of Microsoft Edge will be pinned to the taskbar.
- The next version of Microsoft Edge will add a shortcut to the desktop.
- Most protocols that Microsoft Edge handles by default will be migrated to the next version of Microsoft Edge.
- Current Microsoft Edge will be hidden from all UX surfaces in the OS, including settings, all apps, and any file or protocol support dialogs.
- All attempts to launch the current version of Microsoft Edge will redirect to the next version of Microsoft Edge.

  > [!NOTE]
  > User level installs won’t trigger these behaviors.

Along with the previous changes, there are changes that will happen regardless of whether the stable channel of the next version of Microsoft Edge is installed.

- Microsoft Edge will de-register for the books and XML protocols that the next version of Microsoft Edge doesn't support. Users attempting to open these protocols will get a dialog that prompts them to choose a default app.

## Timeline

The changes needed to support the described experience will be delivered with three updates for different versions of Windows.

### For Windows version 1903

- First set of changes in optional July 2019 update, delivered with the August 2019 security update.
- Second set of changes in the optional August 2019 update, delivered with the September 2019 security update.

  > [!NOTE]
  > This is the update where Microsoft Edge will de-register for the XML protocol.

- Third set of changes in the optional September 2019 update, delivered with the October 2019 security update.

  > [!NOTE]
  > This is the update where Microsoft Edge will no longer support eBooks.

### For Windows versions 1709, 1803, and 1809

- First set of changes in an optional August 2019 update, delivered with the September 2019 security update.
- Second set of changes in an optional September 2019 update, delivered with the October 2019 security update.

  > [!NOTE]
  > This is the update where Microsoft Edge will de-register for the XML protocol.

- Third set of changes in an optional October 2019 update, delivered with the November 2019 security update.

  > [!NOTE]
  > This is the update where Microsoft Edge will no longer support eBooks.

<!-- TBD, wave stuff?    -->
Wave 1
Do customers need to see the specific details of what’s in each wave, or is that too much?
Wave 2
Do customers need to see the specific details of what’s in each wave, or is that too much?
Wave 3
Do customers need to see the specific details of what’s in each wave, or is that too much?
