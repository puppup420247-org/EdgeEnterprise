---
title: "Blocker Toolkit to disable automatic delivery of Microsoft Edge"
ms.author: kvice
author: dan-wesley
manager: srugh
ms.date: 12/11/2019
audience: ITPro
ms.topic: conceptual
ms.prod: microsoft-edge
ms.localizationpriority: high
ms.collection: M365-modern-desktop
description: "Blocker Toolkit to disable automatic delivery of Microsoft Edge"
---

# Blocker Toolkit to disable automatic delivery of Microsoft Edge

This article describes the Blocker Toolkit for disabling automatic delivery and installation of Microsoft Edge.

> [!NOTE]
> This applies to Microsoft Edge Stable channel.

## Overview

To help our customers become more secure and up-to-date, Microsoft will distribute Microsoft Edge (Chromium-based) through Automatic Updates for Windows 10 RS4 and newer. The Blocker Toolkit is intended for organizations that would like to block automatic delivery of Microsoft Edge (Chromium-based) to machines in environments where Automatic Updates is enabled. The Blocker Toolkit will not expire.

- For computers running Windows 10 RS4 and newer, the Blocker Toolkit prevents the machine from receiving Microsoft Edge (Chromium-based) via Automatic Updates.
- The Blocker Toolkit will not prevent users from manually installing Microsoft Edge (Chromium-based) from internet download, or from external media.
- Organizations do not need to deploy the Blocker Toolkit in environments managed with an update management solution such as Windows Server Update Services or System Center Configuration Manager. Organizations can use those products to fully manage deployment of updates released through Windows Update and Microsoft Update, including Microsoft Edge (Chromium-based), within their environment.

You can download the Blocker Toolkit executable file from [https://msedgeblockertoolkit.blob.core.windows.net/blockertoolkit/MicrosoftEdgeChromiumBlockerToolkit.exe](https://msedgeblockertoolkit.blob.core.windows.net/blockertoolkit/MicrosoftEdgeChromiumBlockerToolkit.exe).

### Toolkit components

This toolkit contains the following components:

- Executable blocker script (.CMD)
- Group Policy Administrative Template (.ADMX + .ADML)

### Supported Operating Systems

Windows 10 RS4 and newer.

## Blocker script

The script creates a registry key and sets the associated value to block or unblock (depending on the command-line option used) automatic delivery of Microsoft Edge (Chromium-based) on either the local machine or a remote target machine.

**Registry key:** `HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft\EdgeUpdate`<br>
**Key value name:** `DoNotUpdateToEdgeWithChromium`

| Value                | Result                         |
|----------------------|--------------------------------|
| *Key is not defined* | Distribution is *not* blocked. |
| 0                    | Distribution is *not* blocked. |
| 1                    | Distribution is blocked.       |

The script has the following command-line syntax:<br> 
`EdgeChromium_Blocker.cmd [<machine name>] [/B] [/U] [/H]`

### Machine name

The `<machine name>` parameter is optional. If not specified, the action is performed on the local machine. Otherwise, the remote machine is accessed through the remote registry capabilities of the `REG` command. If the remote registry can't be accessed due to security permissions or the remote machine can't be found, an error message is returned from the `REG` command.

### Switches

Switches used by the script are mutually exclusive and only the first valid switch from a given command is acted on. The script can be run multiple times on the same machine.

| Switch       | Description                              |
|--------------|------------------------------------------|
| `/B`         | Blocks distribution                      |
| `/U`         | Unblocks distribution                    |
| `/H` or `/?` | Displays the following summary help:<br>`This tool can be used to remotely block or unblock the delivery of Microsoft Edge (Chromium-based) through automatic Updates.`<br> `Usage:`<br>`EdgeChromium_Blocker.cmd [<machine name>] [/B][/U][/H]`<br>`B = Block Microsoft Edge (Chromium-based) deployment`<br>`U = Allow Microsoft Edge (Chromium-based) deployment`<br>`H = Help`<br>`Examples:`<br>`EdgeChromium_Blocker.cmd mymachine /B (blocks delivery on machine "mymachine")`<br>`EdgeChromium_Blocker.cmd /U (unblocks delivery on the local machine)`<br> |

## Group Policy Administrative Template (.ADMX + .ADML files)

The Group Policy Administrative Template (.ADMX + .ADML files) allows administrators to import the new Group Policy settings to block or unblock automatic delivery of Microsoft Edge (Chromium-based) into their Group Policy environment, and use Group Policy to centrally execute the action across systems in their environment.

Users running Windows 10 RS3 Enterprise/EDU and RS4 and newer, will see the policy under the following path:

```
/Computer Configuration  
  /Administrative Templates
    /Classic Administrative Templates  
      /Windows Components  
        /Windows Update  
          /Microsoft Edge (Chromium-based) Blockers
```

> [!NOTE]
> This setting is available only as a computer setting; there is no per-user setting.

> [!IMPORTANT]
> This registry setting isn't stored in a policies key and is considered a *preference*. Therefore, if the Group Policy Object that implements the setting is ever removed or the policy is set to **Not Configured**, the setting will remain. To unblock distribution of Microsoft Edge (Chromium-based) by using Group Policy, set the policy to **Disabled**.

## See also

- [Microsoft Edge Enterprise landing page](https://www.microsoftedgeinsider.com/enterprise)
- [Windows updates to support Microsoft Edge](https://docs.microsoft.com/deployedge/microsoft-edge-sysupdate-windows-updates)
- [How to access the old version of Microsoft Edge](https://docs.microsoft.com/deployedge/microsoft-edge-sysupdate-access-old-edge)