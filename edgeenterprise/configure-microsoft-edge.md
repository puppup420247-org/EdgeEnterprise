--- 
title: "Configuring Microsoft Edge" 
ms.author: brianalt 
author: kelleyvice-MSFT
audience: ITPro 
ms.topic: reference
ms.prod: microsoft-edge
localization_priority: low
ms.collection: 
ms.custom: 
description: "Learn how to configure Microsoft Edge version 77 and later on Windows and Mac" 
---

# Configuring Microsoft Edge
Use the following information to configure Microsoft Edge on your Windows and Mac devices.

## Configure Microsoft Edge on Windows

The recommended way to configure policy on all versions of Windows is by using group policy objects (GPO). You can also provision policy through the  registry for Windows devices that are joined to a Microsoft Active Directory domain or Windows 10 Pro or Enterprise instances enrolled for device management.

Microsoft Edge supports mandatory and recommended policies. Mandatory policies override user preferences and prevents the user from changing it, while recommended policy provide a default setting that may be overridden by the user. Most policies are mandatory only; a subset are mandatory and recommended. If both versions of a policy are set, the mandatory one takes precedents. 

Microsoft Edge has two administrative templates: One to [configure Microsoft Edge settings](microsoft-edge-policies.md), and one to [manage Microsoft Edge updates](microsoft-edge-update-policies.md). 

## Configuring Microsoft Edge on Mac
Use a property list (.plist) file to set Microsoft Edge policies on Mac. The Microsoft Edge policy_template.zip file contains a sample plist file that you can customize to define policy settings. You then convert this file to a configuration profile that can be deployed to your user's Mac devices using your preferred management tool, such as Microsoft Intune or Jamf.

You can create the plist file with any text editor. It's usually easier to edit a plist file using an editing tool that formats the XML code for you, such as Xcode, which is available for free from the Apple developer website. After creating the contents of your plist file, you will need to name the file in a very specific way. The plist will need to contain the name of the application domain for Edge in reverse-domain format. For example, the required name for your plist for Dev channel is:  com.microsoft.Edge.Dev.plist. Note: the name is case sensitive. It needs to match this name exactly.

For information about the policies avaiable in Microsoft Edge, check out [Microsoft Edge - Policies](microsoft-edge-policies.md).
