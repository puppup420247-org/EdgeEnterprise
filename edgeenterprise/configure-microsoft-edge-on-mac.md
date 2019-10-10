---
title: "Configure Microsoft Edge for macOS"
ms.author: brianalt
author: kelleyvice-msft
manager: laurawi
ms.date: 10/09/2019
audience: ITPro
ms.topic: conceptual
ms.prod: microsoft-edge
ms.localizationpriority: high
ms.collection: M365-modern-desktop
description: "Configure Microsoft Edge policy settings on Mac devices"
---

# Configure Microsoft Edge policy settings on macOS

Use the following information to configure Microsoft Edge policy settings on your Mac devices.

> [!NOTE]
> This article applies to Microsoft Edge version 77 or later.

## Configure policy settings on macOS

Use a property list (.plist) file to set Microsoft Edge policies on Mac devices. You then convert this file to a configuration profile that can be deployed to your users' Mac devices using your preferred management tool, such as Microsoft Intune [using custom settings](https://docs.microsoft.com/intune/custom-settings-macos) or Jamf.

You can create the plist file with any text editor. However, it's easier to create and edit a plist file using a tool that formats the XML code for you. *Xcode* is a free integrated development environment that you can get from one of the following locations:

- the [Apple developer website](https://developer.apple.com/xcode/)
- the [Mac App Store](https://apps.apple.com/app/xcode/id497799835?mt=12)

After you create the contents of your plist file, you need to use a specific format for the file name. The plist file contains the name of the application (preference) domain for Edge in reverse-domain format, which is part of the file name. For example, the preference domain for the Dev channel is **com.microsoft.Edge**. Because this name is case sensitive, the plist file name has to match the domain name. The required name for your plist for the Dev channel would be *com.microsoft.Edge.plist*.

> [!IMPORTANT]
> Starting with build 78.0.249.2, all channels of Microsoft Edge on Mac will read from the **com.microsoft.Edge** preference domain. All prior releases will read from a channel specific domain, such as **com.microsoft.Edge.Dev**.

For a list of supported policies and their preference key names, see [Microsoft Edge browser policies reference](microsoft-edge-policies.md).

### Create a configuration profile

1. In Terminal, use the following command to create a plist for Microsoft Edge on your desktop with your preferred settings:

   ```cmd
   /usr/bin/defaults write ~/Desktop/com.microsoft.Edge.plist RestoreOnStartup -int 1
   ```

2. Convert the plist from binary to plain text format:

   ```cmd
   /usr/bin/plutil -convert xml1 ~/Desktop/com.microsoft.Edge.plist
   ```

3. Upload the converted plist to a Custom Settings payload in a new Configuration Profile in your MDM server or use your preferred conversion tool to create a configuration profile to upload.

In the policy templates file, which can be downloaded from the [Microsoft Edge Enterprise landing page](https://aka.ms/EdgeEnterprise), there's an example plist (*itadminexample.plist*) in the **examples** folder. The example file contains all supported data types that you can customize to define your policy settings.

## Frequently Asked Questions

### Can Microsoft Edge be configured to use master preferences?

Yes, you can configure Microsoft Edge to use a master preferences file.

 A master preferences file lets you configure default settings when Microsoft Edge is deployed. You can also use a master preferences file to apply settings on computers that aren't managed by a device management system. These settings are applied to the user’s profile the first time the user runs the browser. After the user runs the browser, changes to the master preferences file aren’t applied. A user can change settings from the master preferences in the browser. If you want to make a setting mandatory or change a setting after the first run of the browser, you must use a policy.

A master preferences file lets you to customize many different settings and preferences for the browser, including those shared with other Chromium based browsers and specific to Microsoft Edge.  Policy related preferences can be configured using the master preferences file. In cases where a policy is set and there’s a corresponding master preference set, the policy setting takes precedence.

> [!IMPORTANT]
> All the available preferences might not be consistent with Microsoft Edge terminology and naming conventions.  There’s no guarantee that these preferences will continue to work as expected in future releases. Preferences might be changed or ignored in later versions.

A master preferences file is a text file that’s formatted using JSON markup. This file needs to be added to the same directory as the msedge.exe executable. For system wide enterprise deployments on macOS this is typically: “*~/Library/Application Support/Microsoft/Microsoft Edge Master Preferences*" or "*/Library/Microsoft/Microsoft Edge Master Preferences*”.

## See also

- [Microsoft Edge Enterprise landing page](https://aka.ms/EdgeEnterprise)
- [Configure for Windows](configure-microsoft-edge.md)
- [Configure for Windows with Intune](configure-edge-with-intune.md)
