---
title: "IE mode FAQ"
ms.author: cjacks
author: cjacks
manager: saudm
ms.date: 03/05/2020
audience: ITPro
ms.topic: conceptual
ms.prod: microsoft-edge
ms.localizationpriority: high
ms.collection: M365-modern-desktop
description: "FAQ and Troubleshooting for Microsoft Edge with IE mode"
---

# IE mode FAQ

This article provides an FAQ and troubleshooting tips for Microsoft Edge (version 77 or later).

## Troubleshoot IE mode

Use the information in this section to diagnose and fix IE mode problems.

### Internet Explorer mode diagnostic information

You can get Internet Explorer mode diagnostic information on the Microsoft Edge Compatibility tab. To open this tab and see the Internet Explorer mode diagnostics page, go to *edge://compat/iediagnostic*. In addition to providing configuration information for the following categories, this page also gives actionable diagnostic messages.

- **Registry key check**. Checks to see if Internet Explorer is set up in the registry. If it isn't, the user will see a prompt to fix the issue. They can click **Fix it** to resolve the problem.
- **Internet Explorer mode**. The number **7** relates to the API version that's used, based on the configuration and OS. This is another setting that can generate an actionable diagnostic, and the user is prompted to install a **Windows Update**.
- **Internet Explorer mode setting**. This setting is turned on, using default integration and Internet Explorer mode integration policy.
- **Command line**. Shows the command line string and switches used to start Microsoft Edge. In this example, the path statement shows that Microsoft Edge is installed at the user level, and a Tab feature (Experiment) is enabled.
- **Group policy settings**. Turned on and using the Enterprise Mode IE website list (set as IE policy). At this stage the list is still pointing to a file share instead of *https://localhost/sites.xml*, the recommended configuration.<br>
Other settings, such as the Site list debug registry key, and the Enterprise mode site list (set as Microsoft Edge policy) aren't set.

### Error message: "To open this page in Internet Explorer mode, reinstall Microsoft Edge with administrator privileges."

You are receiving the message because you are missing the required updates. Please see the [prerequisites section](#prerequisites) for the required versions of Windows and Microsoft Edge.

Microsoft Edge version 77 or later needs to be installed at the system level, and Internet Explorer 11 needs to be enabled in Windows Features.

Possible reasons for this error:

- Microsoft Edge Canary is installed at the user level and doesn't prompt for elevation.
- Microsoft Edge Dev, Beta will prompt for elevation when installing, but if you cancel the elevation the installation will be continue at the user level.
- Internet Explorer 11 has been disabled in Windows Features.

Possible solutions:

- Run the installer for any channel at the system level: `installer.exe --system-level`.
- Enable Internet Explorer 11 in Windows Features.

To check that Microsoft Edge is installed at the systems level, type "edge://version" in the Microsoft Edge address bar. The Executable path will show a path starting with *C:\Program Files...*, which indicates a system install. If the Executable path begins with *C:\Users..*, uninstall and then reinstall Microsoft Edge with administrator privileges.

### Error message: "To open this page in IE mode, try restarting Microsoft Edge."

You're receiving this message because there was an unexpected error encountered in the Internet Explorer process. This should be resolved by restarting Microsoft Edge.

### Error message: "Turn off remote debugging to open this site in IE mode otherwise it might not work as expected."

You're receiving the message because you started remote debugging and you navigated to a web page that your organization has configured to run in IE mode.

If the intention is to run remote debug on this page you can continue to do so, but the webpage will be rendered in the Microsoft Edge engine.

## Frequently Asked Questions

### Will IE mode replace Internet Explorer 11?

We're committed to keeping Internet Explorer a supported, reliable, and safe browser. Internet Explorer is still a component of Windows and follows the support lifecycle of the OS on which it's installed. For details, see [Lifecycle FAQ - Internet Explorer](https://support.microsoft.com/help/17454/). While Microsoft continues to support and update Internet Explorer, the latest features and platform updates will only be available in Microsoft Edge.

### Can I use "Open with Explorer" or "View in File Explorer" in SharePoint with IE mode?

Yes, if this works in standalone Interenet Explorer 11 it will work in IE mode. However, rather than use the Open with Explorer option, the reccommended approach to managing files and folders outside of SharePoint is to [sync your SharePoint files](https://support.office.com/en-us/article/sync-sharepoint-files-with-the-onedrive-sync-app-6de9ede8-5b6e-4503-80b2-6190f3354a88) or [move or copy files in SharePoint](https://support.office.com/en-us/article/move-or-copy-files-in-sharepoint-00e2f483-4df3-46be-a861-1f5f0c1a87bc).
