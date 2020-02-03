---
title: "Microsoft Edge in-page navigations for IE mode"
ms.author: shisub
author: dan-wesley
manager: srugh
ms.date: 02/03/2020
audience: ITPro
ms.topic: conceptual
ms.prod: microsoft-edge
ms.localizationpriority: high
ms.collection: M365-modern-desktop
description: "Force in-page navigations to stay in IE mode"
---

# Force in-page navigations to stay in IE mode

You can use this policy as a temporary solution to force all "in-page" navigations from IE mode sites to stay in IE mode.

An "in-page" navigation is started from a link, a script, or a form on the current page. It can also be a server-side redirect of a previous "in-page" navigation attempt. Conversely, a user can start a navigation that isn’t "in-page" that’s independent of the current page in several ways by using the browser controls. For example, using the address bar, the back button, or a favorite link.

>[!NOTE]
>This article applies to Microsoft Edge version 77 or later.

## Prerequisites

The following Windows updates are required for this policy:

- KB1
- KB2

## About this policy

This policy gives you time to identify and configure all of the authentication servers used by your IE mode sites. However, this policy will result in an inconsistent browsing experience, where some sites are rendered sometimes in Internet Explorer mode and at other times in Microsoft Edge mode, depending on whether or not the navigation to the site began from an Internet Explorer mode page. Any site that is not explicitly configured to open in a particular engine will be subject to this possible inconsistency.

If you enable this policy, we recommend that you disable it once you have identified all the authentication servers and added them to the site list as neutral. This will ensure that your modern sites never inadvertently render in Internet Explorer mode.

## Keep in-page navigations in IE mode

To keep automatic or all in-page navigations in Internet Explorer mode follow these steps:

1. Open Local Group Policy Editor.
2. Click **Computer Configuration** > **Administrative Templates** > **Microsoft Edge**.
3. Under **Setting**, double-click **Specify how "in-page" navigations to unconfigured sites behave when started from Internet Explorer mode pages**.
<!-- screen shot -->
4. Select **Enabled**, choose an option from the dropdown and then click **OK** or **Apply** to save the policy settings.
<!-- screen shot -->
## See also

- [Microsoft Edge Enterprise landing page](https://www.microsoftedgeinsider.com/enterprise)
