---
title: "Automate Microsoft Edge for macOS deployment with Microsoft Intune"
ms.author: kvice
author: dan-wesley
manager: laurawi
ms.date: 09/30/2019
audience: ITPro
ms.topic: technical
ms.prod: microsoft-edge
ms.localizationpriority: high
ms.collection: M365-modern-desktop
description: "How to automate Microsoft Edge for macOS deployment with Microsoft Intune."
---

# Deploy to macOS with Microsoft Intune

This article describes how to deploy Microsoft Edge for macOS using Microsoft Intune.

> [!NOTE]
> This article applies to Microsoft Edge version 77 or later.

## Introduction

You can deploy the Microsoft Edge .pkg installer as a line-of-business application using Microsoft Intune. This requires pre-processing the .pkg installer on a macOS device using the Intune App Wrapping Tool. The tool generates a .intunemac file that's uploaded to Microsoft Intune.

## Prerequisites

1. Download the [Intune App Wrapping Tool for macOS](https://github.com/msintuneappsdk/intune-app-wrapping-tool-mac). The tool must be run on a macOS device.

2. Mark the downloaded tool as an executable:

   - Start the Terminal app.
   - Change the directory to the location where `IntuneAppUtil` is located.
   - Run the following command to make the tool executable:<br>
     `chmod a+x ./IntuneAppUtil`
   - Test the tool by running: <br>
     `./IntuneAppUtil -h`

3. Use the `IntuneAppUtil` command to wrap the .pkg installer to a .intunemac file: <br>
   `./IntuneAppUtil -c MicrosoftEdgeDev-77.0.223.0.pkg -o <output_directory>`

## To deploy Microsoft Edge for macOS using Microsoft Intune:

1. Sign in to [Intune](https://go.microsoft.com/fwlink/?linkid=2090973).
2. On the **Intune** pane, choose **Client apps** > **Apps** > **Add** > **Line-of-business app** > **App package file**.
3. On the **App package file** pane, choose the browse button, and select the wrapped Microsoft Edge installation file with the extension *.intunemac*. When you are finished, choose **OK**.
4. Configure app information. When you are finished, choose **OK**.
5. On the **Add app** pane, verify that the details for your app is correct.
6. Choose **Add**, to upload the app to Intune.
7. The app you have added is displayed in the apps list. You can now assign it to the groups you choose.

Congratulations! You’ve just finished configuring using Intune to deploy Microsoft Edge for macOS.

## See also

- [Microsoft Edge Enterprise landing page](https://aka.ms/EdgeEnterprise)
- [Jamf.com](https://www.jamf.com/)
