---
title: "Configure Microsoft Edge using Mobile Device Management"
ms.author: kvice
author: dan-wesley
manager: laurawi
ms.date: 10/17/2019
audience: ITPro
ms.topic: technical
ms.prod: microsoft-edge
ms.localizationpriority: high
ms.collection: M365-modern-desktop
description: "Configure Microsoft Edge using Mobile Device Management."
---

# Configure Microsoft Edge using Mobile Device Management

This article explains how to ingest the Microsoft Edge administrative template into Microsoft Intune and then use this template to create an Open Mobile Alliance Uniform Resource Identifier (OMA-URI). You can use this OMA-URI to set the Mobile Device Management (MDM) settings for Microsoft Edge.

In addition to using Microsoft Intune to configure Microsoft Edge on Windows 10 you can use [Mobile Device Management (MDM)](https://docs.microsoft.com/windows/client-management/mdm/) with your preferred Enterprise Mobility Management (EMM) or an MDM provider that supports [ADMX Ingestion](https://docs.microsoft.com/windows/client-management/mdm/win32-and-centennial-app-policy-configuration).

> [!NOTE]
> This article applies to Microsoft Edge version 77 or later.

## Prerequisites

Windows 10, with the following minimum system requirements:

- Windows 10, version 1903 with [KB4512941](https://support.microsoft.com/help/4512941/) and [KB4517211](https://support.microsoft.com/help/4517211/) installed
- Windows 10, version 1809 with [KB4512534](https://support.microsoft.com/help/4512534/) installed
- Windows 10, version 1803 with [KB4512509](https://support.microsoft.com/help/4512509/) installed
- Windows 10, version 1709 with [KB4516071](https://support.microsoft.com/help/4516071/) installed

## Microsoft Edge MDM support using ADMX Ingestion

dd

## Configure Microsoft Edge using MDM via custom OMA URI using ADMX Ingestion in Microsoft Intune

sda

### To ingest the Microsoft Edge ADMX file into Microsoft Intune

## Configure a Microsoft Edge policy with Microsoft Intune using Custom OMA-URI Settings

### Confirm that the policy was set

### Troubleshoot a policy setting

If a Microsoft Edge policy isn’t taking effect, try the following steps:

Open the edge://policy page on the target device (a device you assigned the profile to in Microsoft Intune) and search for the policy. If the policy isn’t on the edge://policy page, try the following:

- Check that the policy is in the registry and is correct. On the target device open the Windows 10 Registry Editor (**Windows key + r**, enter “*regedit*” and then press **Enter**.) Check that the policy is correctly defined in the *\Software\Policies\ Microsoft\Edge* path. If you don’t find the policy in the expected path, then the policy wasn’t pushed to the device correctly.
- Check that the OMA-URI path is correct, and the value is a valid XML string. If either of these are incorrect the policy won’t be pushed to the target device.

For more trouble shooting tips, see [Set up Microsoft Intune](https://docs.microsoft.com/intune/fundamentals/setup-steps) and [Sync devices](https://docs.microsoft.com/intune/remote-actions/device-sync).

## Create an OMA URI for Microsoft Edge policy

To configure a policy setting using a custom OMA URI you have to:

- create the OMA URI path
- use “String” as the path type
- set the value for the path

The next section describes how to create the OMA URI path, look up and define the value in XML format for mandatory and recommended browser polices, and update policies.

### Define the OMA URI path

You can use the following URI path formula as a guide for creating the OMA URI path.

**URI path formula:**<br>
./Device/Vendor/MSFT/Policy/Config/\<ADMXIngestName>~Policy~\<ADMXNamespace>~\<ADMXCategory>/\<PolicyName>

The next table shows the URI path parameters.

| Parameter         | Description                                                                                   |
|-------------------|-----------------------------------------------------------------------------------------------|
| \<ADMXIngestName> | Use "Edge" or what you defined when ingesting the administrative template. It must match what you set in the URI string when you ingested the ADMX file. For example, if you used “./Device/Vendor/MSFT/Policy/ConfigOperations/ADMXInstall/MicrosoftEdge/Policy/EdgeAdmx”, then use “MicrosoftEdge”. |
| \<ADMXNamespace>  | Either "microsoft_edge" or "microsoft_edge_recommended" depending on if you are setting a mandatory or a recommended policy.                                                                                  |
| \<ADMXCategory>   | The "ParentCategory" of the policy in the ADMX file. If the policy isn't grouped with a "ParentCategory" then the \<ADMXCategory> isn't used.                            |
| \<PolicyName>     | This is the policy name found in [Browser policy reference] and [Update policy reference]     |




### Define the data type

The OMA URI data type is always “String”.

### Define the value for browser policies

This section describes how to define the value in XML format for each data type. For non-Boolean data types, the value must start with the \<enabled/> element.

#### Boolean data type

For policies that are Boolean types use \<enabled/> or \<disabled/>.

#### Integer data type

The value always needs to start with the \<enabled/> element followed by \<data id="[valueName]" value="[decimal value]"/>. To find the value name and decimal value, use the following steps:

#### List of strings data type

The value always needs to start with the \<enabled/a> element followed by \<data id="[listID]" value="[string 1];[string 2];[string 3]"/>.

#### Dictionary or String data type

The value always needs to start with the \<enabled/> followed by \<data id="[textID]" value="[string]"/> .

## Create the OMA-URI for a recommended policy

Defining the URI path for recommended policies depends on the policy you want to configure.

The following table shows examples of OMA-URI paths for recommended policies.

|              Policy               |             OMA-URI                      |
|-----------------------------------|------------------------------------------|
| [RegisteredProtocolHandlers](https://docs.microsoft.com/deployedge/microsoft-edge-policies#registeredprotocolhandlers)                       | ./Device/Vendor/MSFT/Policy/Config/Edge~Policy~microsoft_edge_recommended~ContentSettings_recommended/RegisteredProtocolHandlers_recommended                        |
| [PasswordManagerEnabled](https://docs.microsoft.com/deployedge/microsoft-edge-policies#passwordmanagerenabled)                       | ./Device/Vendor/MSFT/Policy/Config/Edge~Policy~microsoft_edge_recommended~PasswordManager_recommended/PasswordManagerEnabled_recommended                        |
| [PrintHeaderFooter](https://docs.microsoft.com/deployedge/microsoft-edge-policies#printheaderfooter)                       | ./Device/Vendor/MSFT/Policy/Config/Edge~Policy~microsoft_edge_recommended~Printing_recommended/PrintHeaderFooter_recommended                        |
| [SmartScreenEnabled](https://docs.microsoft.com/deployedge/microsoft-edge-policies#smartscreenenabled)                       | ./Device/Vendor/MSFT/Policy/Config/Edge~Policy~microsoft_edge_recommended~SmartScreen_recommended/SmartScreenEnabled_recommended                        |
| [HomePageLocation](https://docs.microsoft.com/deployedge/microsoft-edge-policies#homepagelocation)                       | ./Device/Vendor/MSFT/Policy/Config/Edge~Policy~microsoft_edge_recommended~Startup_recommended/HomepageLocation_recommended                        |
| [ShowHomeButton](https://docs.microsoft.com/deployedge/microsoft-edge-policies#showhomebutton)                       | ./Device/Vendor/MSFT/Policy/Config/Edge~Policy~microsoft_edge_recommended~Startup_recommended/ShowHomeButton_recommended                        |
| [FavoritesBarEnabled](https://docs.microsoft.com/deployedge/microsoft-edge-policies#favoritesbarenabled)                       | ./Device/Vendor/MSFT/Policy/Config/Edge~Policy~microsoft_edge_recommended~/FavoritesBarEnabled_recommended                        |


## Example OMA-URI paths and values

This section shows OMA-URI examples that use different data types for values.

### Boolean data type

### Integer data type

### List of strings data type

### Dictionary and String data type

*ProxyMode example:*
| Field   | Value                                                                                |
|---------|--------------------------------------------------------------------------------------|
| Name    | Microsoft Edge: ProxyMode                                                            |
| OMA-URI | ./Device/Vendor/MSFT/Policy/Config/Edge~Policy~microsoft_edge~ProxyMode/ProxyMode    |
| Type    | String                                                                               |
| Value   | \<enabled/>\<data id="ProxyMode" value="auto_detect"/>                               |




## See also

- [Microsoft Edge Enterprise landing page](https://aka.ms/EdgeEnterprise)
- [Configure Microsoft Edge policy settings with Microsoft Intune](configure-edge-with-intune.md)
- [Mobile device management](https://docs.microsoft.com/windows/client-management/mdm/)
- [Use custom settings for Windows 10 devices in Intune](https://docs.microsoft.com/intune/configuration/custom-settings-windows-10)
- [Win32 and Desktop Bridge app policy configuration](https://docs.microsoft.com/windows/client-management/mdm/win32-and-centennial-app-policy-configuration)
- [Understanding ADMX-backed policies](https://docs.microsoft.com/windows/client-management/mdm/understanding-admx-backed-policies)
