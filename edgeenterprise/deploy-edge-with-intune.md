---
title: "Deploy Microsoft Edge using Microsoft Intune"
ms.author: kvice
author: kelleyvice-msft
manager: laurawi
ms.date: 09/4/2019
audience: ITPro
ms.topic: procedural
ms.prod: microsoft-edge
localization_priority: medium
ms.collection: M365-modern-desktop
description: "Learn how to deploy Microsoft Edge with Microsoft Intune."
---

# Deploy Microsoft Edge using Microsoft Intune

This article shows you how to automate Microsoft Edge deployment and configuration for Windows and macOS by using Microsoft Intune.

>[!NOTE]
>This article applies to Microsoft Edge version 77 or later.

You can deploy Microsoft Edge to Windows and macOS clients that are managed in your company's Intune tenant by adding apps containing the Microsoft Edge installation files to Intune. You can deploy Microsoft Edge with either Mobile Device Management (MDM) or Mobile Application Management (MAM). Like any Intune apps, you can configure app assignments to force Microsoft Edge deployment to selected users or devices or make the app available in the Company Portal for users to install at their discretion.

You can also configure Microsoft Edge policies and settings by adding a Device Configuration Profile. If your company primarily uses Intune to manage and enforce policies on user devices, this is a good alternative to using Active Directory Group Policy or local GPOs.

You can read [Manage web access by using Microsoft Edge with Microsoft Intune](https://docs.microsoft.com/en-us/intune/manage-microsoft-edge) to learn more, but keep in mind that this article is specific to Microsoft Edge (EdgeHTML), not Microsoft Edge Enterprise (Chromium-based).

## Before you begin

Review the information in [Add a Windows line-of-business app to Microsoft Intune](https://docs.microsoft.com/en-us/intune/lob-apps-windows).

Download the Microsoft Edge Enterprise installation files (**MicrosoftEdgeDevEnterpriseX64.msi** and/or **MicrosoftEdgeDevEnterpriseX86.msi**) from the [Microsoft Edge Enterprise landing page](https://aka.ms/EdgeEnterprise).

If you also want to configure settings for Microsoft Edge using Intune, download the Microsoft Edge policy templates for Intune from the [Microsoft Edge Enterprise landing page](https://aka.ms/EdgeEnterprise). Make sure you download the policy template that matches the channel of your installation files (Beta or Dev).

- [Microsoft Edge (Stable) Intune policy template](https://go.microsoft.com/fwlink/?linkid=2099617&clcid=0x409)
- [Microsoft Edge (Beta) Intune policy template](https://go.microsoft.com/fwlink/?linkid=2099618&clcid=0x409)
- [Microsoft Edge (Dev) Intune policy template](https://go.microsoft.com/fwlink/?linkid=2093504&clcid=0x409)

Make sure you store the Microsoft Edge installation and policy files in an accessible network location.

## Add Microsoft Edge for Windows to Intune

Follow the procedures in [Add a Windows line-of-business app to Microsoft Intune](https://docs.microsoft.com/en-us/intune/lob-apps-windows). This article contains procedures for adding an app like Edge Enterprise to your Microsoft Intune instance.

See [Add apps to Microsoft Intune](https://docs.microsoft.com/en-us/intune/apps-add) for general information about considerations, organization and troubleshooting apps in Intune.

### Configure Microsoft Edge settings using a custom profile

Using Microsoft Intune, you can add or create custom settings for your Windows 10 devices using "custom profiles". Windows 10 custom profiles use Open Mobile Alliance Uniform Resource Identifier (OMA-URI) settings to configure different features. You can create a custom profile and import the Microsoft Edge policy template using ADMX ingestion to enable configuration of Microsoft Edge-specific application settings.

#### Create a custom profile to manage Microsoft Edge

This procedure creates a new custom profile and imports the settings and policies from the Microsoft Edge policy template file **msedge.admx**. When you are done, go to 

1. Download the Microsoft Edge policy templates for Intune from the [Microsoft Edge Enterprise landing page](https://aka.ms/EdgeEnterprise). Make sure you download the policy template that matches the channel of your installation files (Stable, Beta or Dev).

    - [Microsoft Edge (Stable) Intune policy template](https://go.microsoft.com/fwlink/?linkid=2099617&clcid=0x409)
    - [Microsoft Edge (Beta) Intune policy template](https://go.microsoft.com/fwlink/?linkid=2099618&clcid=0x409)
    - [Microsoft Edge (Dev) Intune policy template](https://go.microsoft.com/fwlink/?linkid=2093504&clcid=0x409)

1. Sign in to the [Microsoft Azure portal](https://portal.azure.com).
1. Select **Intune** from _All Services_, or search for Intune in the portal search box.
1. From the _Microsoft Intune - Overview_ blade, select **Device configuration** | **Profiles**.
1. On the top bar, select **Create profile**.
1. Enter the following text:

    |Field  |Value  |
    |---------|---------|
    |Name     |Enter a descriptive name, like _Edge Enterprise Configuration_         |
    |Description     |Optionally enter a description         |
    |Platform     |Windows 10 and later         |
    |Profile type     |Custom         |

1. Click **Settings**. The _Custom OMA-URI Settings_ blade opens to the right.
1. Click **Add**, and enter the following text:

    |Field  |Value  |
    |---------|---------|
    |Name     |Enter a descriptive name, like _Edge ADMX Ingestion_         |
    |Description     |Optionally enter a description         |
    |OMA-URI     |./Device/Vendor/MSFT/Policy/ConfigOperations/ADMXInstall/Edge/Policy/EdgeAdmx         |
    |Data type     |String         |

1. When you select **String** from the _Data type_ drop-down, a **Value** field appears below. In a text editor, copy the entire contents of the **msedge.admx** file from the policy template you downloaded earlier and paste it into the **Value** field.
1. Click **OK** and **OK** again to save the OMA-URI settings.
1. Click **Create** to create the custom profile.

>[!NOTE]
>You can also configure the custom profile's **Scope** and **Applicability rules** to target specific devices.

#### Add settings to the Microsoft Edge custom profile

Now you can add specific application settings to the custom profile.



When you are done, see [Assign user and device profiles in Microsoft Intune](https://docs.microsoft.com/en-us/intune/device-profile-assign) for information about how to "assign" the profile to your Azure Active Directory (Azure AD) user or device groups.

See [Use custom settings for Windows 10 devices in Intune](https://docs.microsoft.com/en-us/intune/custom-settings-windows-10) for more information about custom profiles in Intune, and [Win32 and Desktop Bridge app policy configuration](https://docs.microsoft.com/en-us/windows/client-management/mdm/win32-and-centennial-app-policy-configuration) for more information about how ADMX ingestion works for setting Windows policies using Intune.

## Add Microsoft Edge for macOS to Intune

The process for adding a Microsoft Edge for macOS app is similar, but there are certain prerequisites for managing macOS and iOS devices in Intune.

- [Get an Apple MDM push certificate](https://docs.microsoft.com/en-us/intune/apple-mdm-push-certificate-get)
  
    An Apple MDM Push certificate is required for Intune to manage iOS and macOS devices. After you add the certificate to Intune, your users can enroll their devices using:

  - The Company Portal app.
  - Apple's bulk enrollment methods like the Device Enrollment Program, Apple School Manager, or Apple Configurator.

## Assign apps to groups with Microsoft Intune

After you've added an app to Microsoft Intune, you can assign the app to users and devices. It is important to note that you can assign an app to a device whether or not the device is managed by Intune.

For more information, see [Assign apps to groups with Microsoft Intune](https://docs.microsoft.com/en-us/intune/apps-deploy).
