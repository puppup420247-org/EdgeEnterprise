---
title: "Configure Microsoft Edge"
ms.author: brianalt
author: kelleyvice-MSFT
manager: laurawi
ms.date: 08/20/2019
audience: ITPro
ms.topic: reference
ms.prod: microsoft-edge
localization_priority: medium
ms.collection: M365-modern-desktop
description: "Configure Microsoft Edge on Windows and Mac devices"
---

# Configure Microsoft Edge

Use the following information to configure Microsoft Edge on your Windows and Mac devices.

> [!NOTE]
> This article applies to Microsoft Edge version 77 or later.

## Configure Microsoft Edge on Windows

You can use group policy objects (GPO) to configure Microsoft Edge and managed Microsoft Edge updates on all versions of Windows. You can also provision policy through the registry for Windows devices that are joined to a Microsoft Active Directory domain or Windows 10 Pro or Enterprise instances enrolled for device management.

Microsoft Edge supports mandatory and recommended policies. Mandatory policies override user preferences and prevents the user from changing it, while recommended policy provide a default setting that may be overridden by the user. Most policies are mandatory only; a subset are mandatory and recommended. If both versions of a policy are set, the mandatory one takes precedence.

Microsoft Edge has two administrative templates:

- _msedge.admx_ to [configure Microsoft Edge settings](microsoft-edge-policies.md)
- _msedgeupdate.admx_ to [manage Microsoft Edge updates](microsoft-edge-update-policies.md).

To get started, download and install the Microsoft Edge administrative template.

### 1. Download and install the Microsoft Edge administrative template

Go to the [Microsoft Edge Enterprise landing page](https://aka.ms/EdgeEnterprise) to download the Microsoft Edge policy templates file (_MicrosoftEdgePolicyTemplates.zip_).

To add the administrative template to configure Microsoft Edge:

1. Open the _MicrosoftEdgePolicyTemplates.zip_ file and go to **windows** > **admx**.
2. Copy the _msedge.admx_ file to your Policy Definition template folder. (Example: C:\Windows\PolicyDefinitions)
3. In the _admx_ folder, open the appropriate language folder. For example, if you’re in the U.S., open the **en-US** folder.
4. Copy the _msedge.adml_ file to the matching language folder in your Policy Definition folder. (Example: C:\Windows\PolicyDefinitions\en-US)
5. To confirm the files loaded correctly either open Local Group Policy Editor directly (Windows key + R and enter gpedit.msc) or open MMC and load the Local Group Policy Editor snap-in. If an error occurs, it’s usually because the files are in an incorrect location.

<!--
To add the administrative template to manage Microsoft Edge updates:

1. Open the _MicrosoftEdgePolicyTemplates.zip_ file and go to **windows** > **admx**.
2. Copy the _msedgeupdate.admx_ file to your Policy Definition template folder. (Example: C:\Windows\PolicyDefinitions)
3. In the _updatepolicies_ folder, open the appropriate language folder. For example, if you’re in Germany, open the **de-DE** folder.
4. Copy the _msedgeupdate.adml_ file to the matching language folder in your Policy Definition folder. (Example: C:\Windows\PolicyDefinitions\de-DE)
5. Open MMC and load the Local Group Policy Editor snap-in to confirm the files loaded correctly. If an error occurs, it’s usually because the files are in an incorrect location.

> [!NOTE]
> Currently the Microsoft Edge update policies are only localized in en-US. Additional language support will be added in a future release.
-->

### 2. Set mandatory or recommended policies

In Local Group Policy Editor, you can set mandatory or recommended policies to configure Microsoft Edge.

To configure a mandatory policy, open Local Group Policy Editor and go to **Administrative Templates** > **Microsoft Edge**.

To configure a recommended policy, open Local Group Policy Editor and go to **Administrative Templates** > **Microsoft Edge – Default Settings** (users can override).

![Open Local Group Policy Editor](./media/configure-microsoft-edge/edge-policy.png)

### 3. Test your policies

On a target client device, open Microsoft Edge and navigate to **edge://policy** to see all policies that are applied.

![View configured policies in browser](./media/configure-microsoft-edge/edge-gpEdit.png)

If the policies haven't propagated to the test machine or user, try executing the following command from a command prompt to refresh policy settings on client device:

``` command
gpupdate /force
```

You can also use REGEDIT.exe on the client device to view the registry settings. The settings are located at the registry path **HKLM\SOFTWARE\Policies\Microsoft\Edge**.

## Configure Microsoft Edge on Mac

Use a property list (.plist) file to set Microsoft Edge policies on Mac. You then convert this file to a configuration profile that can be deployed to your user's Mac devices using your preferred management tool, such as Microsoft Intune [using custom settings](https://docs.microsoft.com/intune/custom-settings-macos) or Jamf.

You can create the plist file with any text editor. It's usually easier to edit a plist file using an editing tool that formats the XML code for you, such as _Xcode_, which is available for free from the [Apple developer website](https://developer.apple.com).

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

In the policy template zip file, which can be downloaded from the [Microsoft Edge Enterprise landing page](https://aka.ms/EdgeEnterprise), there's an example plist (_itadminexample.plist_) in the **examples** folder. The example file contains all supported data types that you can customize to define your policy settings.

## See also

- [Overview of Microsoft Edge in the enterprise](overview-edge-in-the-enterprise.md)
- [Microsoft Edge Enterprise landing page](https://aka.ms/EdgeEnterprise)
