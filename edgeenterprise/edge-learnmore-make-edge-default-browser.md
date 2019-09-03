---
title: "Make Microsoft Edge the default browser on Windows"
ms.author: brianalt
author: dan-wesley
manager: srugh
ms.date: 09/03/2019
audience: ITPro
ms.topic: conceptual
ms.prod: microsoft-edge
localization_priority: medium
ms.collection: M365-modern-desktop
description: "Learn how to make Microsoft Edge the default browser"
---

# How to make Microsoft Edge your default browser

This article explains how you can make Microsoft Edge the default browser for your organization on Windows.

> [!NOTE]
> This article applies to Microsoft Edge version 77 or later on Windows 8 or later. For Windows 7 and Mac see the "[Set Microsoft Edge as default browser](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#defaultbrowsersettingenabled)" policy.

## Introduction

You can use the **Set a default associations configuration file** Group Policy or the [DefaultAssociationsConfiguration](https://docs.microsoft.com/windows/client-management/mdm/policy-csp-applicationdefaults#applicationdefaults-defaultassociationsconfiguration) Mobile Device Management setting to make Microsoft Edge the default browser for your organization.

To set Microsoft Edge Beta as the default browser for html files and http/https links use the following application association file example:

```xml
<?xml version="1.0" encoding="UTF-8"?>
<DefaultAssociations>
  <Association ApplicationName="Microsoft Edge Beta" ProgId="MSEdgeBHTML" Identifier=".html"/>
  <Association ApplicationName="Microsoft Edge Beta" ProgId="MSEdgeBHTML" Identifier="http"/>
  <Association ApplicationName="Microsoft Edge Beta" ProgId="MSEdgeBHTML" Identifier="https"/>  
</DefaultAssociations>
```

> [!NOTE]
> To make Microsoft Edge Dev the default browser, set **ApplicationName** to "Microsoft Edge Dev" and **ProgId** to "MSEdgeDHTML"

> [!NOTE]
> The default file associations are not applied if Microsoft Edge isn't installed on the target device. In this event, users will be prompted to select their default application when they open a link or a htm/html file.

## Set Microsoft Edge as the default browser on domain-joined devices

You can set Microsoft Edge as the default browser on domain-joined devices by configuring the **Set a default associations configuration file** group policy. Turning this group policy on requires you to create and store a default associations configuration file. This file is stored locally or on a network share. For more information about creating this file, see [Export or Import Default Application Associations](https://go.microsoft.com/fwlink/p/?LinkId=618268).

### To configure the group policy for a default file type and protocol associations configuration file:

1. Open the Group Policy editor and go to the **Computer Configuration\Administrative Templates\Windows Components\File Explorer**.
2. Select **Set a default associations configuration file**.
3. Click **policy setting**, and then click **Enabled**.
4. Under **Options:**, type the location to your default associations configuration file.
5. Click **OK** to save the policy settings.

The example in the next screenshot shows an associations file named *appassoc.xml* on a network share that is accessible from the target device.

   ![Enable file association in group policy](./media/edge-learnmore-make-edge-default-browser/edge-learnmore-app-associations.png)

   > [!NOTE]
   > If this setting is enabled and the user's device is domain-joined, the file is processed, and default associations are applied at logon. If this setting isn't configured or is turned off, or if the user's device isn't domain-joined, no associations are applied.

## Set Microsoft Edge as the default browser on Azure Active Directory joined devices

To set Microsoft Edge Beta as the default browser on Azure Active Directory joined devices follow the steps in the [DefaultAssociationsConfiguration](https://docs.microsoft.com/windows/client-management/mdm/policy-csp-applicationdefaults#applicationdefaults-defaultassociationsconfiguration) Mobile Device Management setting using the following application association file example.

```xml
<?xml version="1.0" encoding="UTF-8"?>
<DefaultAssociations>
  <Association ApplicationName="Microsoft Edge Beta" ProgId="MSEdgeBHTML" Identifier=".html"/>
  <Association ApplicationName="Microsoft Edge Beta" ProgId="MSEdgeBHTML" Identifier="http"/>
  <Association ApplicationName="Microsoft Edge Beta" ProgId="MSEdgeBHTML" Identifier="https"/>  
</DefaultAssociations>
```
## See also

<!-- - [Export or Import Default Application Associations](https://docs.microsoft.com/previous-versions/windows/it-pro/windows-8.1-and-8/hh825038(v=win.10)) -->
- [DISM - Deployment Image Servicing and Management](https://docs.microsoft.com/en-us/windows-hardware/manufacture/desktop/dism---deployment-image-servicing-and-management-technical-reference-for-windows)
- [DISM Overview](https://docs.microsoft.com/en-us/windows-hardware/manufacture/desktop/what-is-dism)
<!-- - [DISM Default Application Association Servicing Command-Line Options](https://docs.microsoft.com/en-us/windows-hardware/manufacture/desktop/dism-default-application-association-servicing-command-line-options) -->
