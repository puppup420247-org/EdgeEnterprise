---
title: "Deploy Microsoft Edge using Microsoft Intune"
ms.author: kvice
author: kelleyvice-msft
manager: laurawi
ms.date: 09/5/2019
audience: ITPro
ms.topic: procedural
ms.prod: microsoft-edge
localization_priority: medium
ms.collection: M365-modern-desktop
description: "Learn how to deploy Microsoft Edge with Microsoft Intune."
---

# Deploy Microsoft Edge using Microsoft Intune

This article shows you how to automate Microsoft Edge deployment and policy configuration for Windows 10 and macOS by using Microsoft Intune.

>[!NOTE]
>This article applies to Microsoft Edge version 77 or later.

You can deploy Microsoft Edge to Windows and macOS clients that are managed in your company's Intune tenant by adding apps containing the Microsoft Edge installation files to Intune. Like any Intune apps, you can configure app assignments to require Microsoft Edge deployment for selected users or devices or simply make the app available in the Company Portal for users to install at their discretion.

You can also configure Microsoft Edge policies and settings by adding a device configuration profile. Using Intune to manage and enforce policies is essentially equivalent to using Active Directory Group Policy or configuring local GPO settings on user devices.

You can read [Manage web access by using Microsoft Edge with Microsoft Intune](https://docs.microsoft.com/en-us/intune/manage-microsoft-edge) to learn more, but keep in mind that this article is specific to Microsoft Edge (EdgeHTML), not Microsoft Edge Enterprise (Chromium-based), and may contain references that do not apply.

## Before you begin

- Review the information in [Add a Windows line-of-business app to Microsoft Intune](https://docs.microsoft.com/en-us/intune/lob-apps-windows).
- To create apps for **Windows 10**, download the Microsoft Edge Enterprise installation **.msi files** from the [Microsoft Edge Enterprise landing page](https://aka.ms/EdgeEnterprise). The installation files use the build channel and processor architecture in their names, and will be named like **MicrosoftEdgeDevEnterpriseX86.msi** or **MicrosoftEdgeBetaEnterpriseX64.msi**.
- To create apps for **macOS**, download the Microsoft Edge Enterprise **PKG for macOS** from the [Microsoft Edge Enterprise landing page](https://aka.ms/EdgeEnterprise).
- Make sure you store the Microsoft Edge installation files in an accessible local or network location.

## Add an app to deploy Microsoft Edge for Windows 10 to Intune

This procedure creates an app for deployment of Microsoft Edge for Windows 10 in Intune.

>[!NOTE]
>You can only deploy Microsoft Edge with Mobile Device Management (MDM). Deployment with Mobile Application Management (MAM) is not supported.

1. Sign in to the [Microsoft Azure portal](https://portal.azure.com).
1. Select **Intune** from _All Services_, or search for Intune in the portal search box.
1. From the _Microsoft Intune - Overview_ blade, select **Client apps** | **Apps**.

    ![Client apps](./media/edge-ent-intune/edge-intune-apps.png)
1. On the top bar, select **Add**.
1. Initially, there is only one field named **App type**.

    ![App type](./media/edge-ent-intune/edge-intune-app-add-app-1.png)
1. Select **Line-of-business app** from the drop-down and additional fields appear.

    ![Line-of-business app](./media/edge-ent-intune/edge-intune-app-add-app-2.png)
1. Select **App package file**, and use the file chooser to select the .msi installation file. Information about the file will display under the file selection field. Click **OK** to continue.

    ![App package file](./media/edge-ent-intune/edge-intune-app-package-file.png)
1. Click **App information** and enter the following values:

    |Field  |Value  |
    |---------|---------|
    |Name     |This field is populated from the installer, but you can change it if you want          |
    |Description     |Enter a description         |
    |Publisher     |Microsoft         |
    |App install context     |This value is pre-selected and cannot be modified         |
    |Ignore app version    |This slider should be set to yes for apps that are automatically updated like Microsoft Edge.    |
    |Category    |Optionally select a category    |
    |Display this as a featured app in the Company Portal    |Optionally set this to Yes    |
    |Information URL    |Optionally add a URL to a page containing information about the app, such as <https://aka.ms/EdgeEnterprise>    |
    |Privacy URL    |Optionally add a URL to a page containing app privacy information, such as <https://privacy.microsoft.com/en-US/privacystatement>    |
    |Command-line arguments    |Optional. See [Microsoft Edge proxy settings](edge-learnmore-cmdline-options-proxy-settings.md) for information about command-line arguments    |
    |Developer    |Optional    |
    |Owner    |Optional    |
    |Notes    |Optional    |
    |Logo    |Optionally select a logo from an image file    |

    ![App information](./media/edge-ent-intune/edge-intune-app-information.png)

1. Optionally, select **Scope (Tags)** to apply existing tags for limiting deployment of the app to a specific scope.
1. Click **Add** to add the app.

When you are done, see [Assign apps to groups with Microsoft Intune](https://docs.microsoft.com/en-us/intune/apps-deploy) to learn how to deploy the app to users.

- You can refer to the procedures in [Add a Windows line-of-business app to Microsoft Intune](https://docs.microsoft.com/en-us/intune/lob-apps-windows) for general guidance and additional details.
- See [Add apps to Microsoft Intune](https://docs.microsoft.com/en-us/intune/apps-add) for information about general Intune app considerations, organization and troubleshooting.

## Create a profile to manage settings in Microsoft Edge for Windows 10

Using Microsoft Intune, you can create a configuration profile to manage settings for your Windows 10 devices with policies, functionality and experience equivalent to GPO. This section will help you create a profile to enable configuration of Microsoft Edge-specific application settings on Windows 10 devices.

This procedure creates an Administrative Templates profile using Microsoft Edge policy settings built into Intune. When you are done, see [Assign user and device profiles in Microsoft Intune](https://docs.microsoft.com/en-us/intune/device-profile-assign) for information about how to assign the profile to your Azure Active Directory (Azure AD) user or device groups.

1. Sign in to the [Microsoft Azure portal](https://portal.azure.com).
1. Select **Intune** from _All Services_, or search for Intune in the portal search box.
1. From the _Microsoft Intune - Overview_ blade, select **Device configuration** | **Profiles**.
1. On the top bar, select **Create profile**.
1. Enter the following values:

    |Field  |Value  |
    |---------|---------|
    |Name     |Enter a descriptive name, like _Microsoft Edge Policies_         |
    |Description     |Optionally enter a description         |
    |Platform     |Windows 10 and later         |
    |Profile type     |Administrative Templates         |

    ![Create profile](./media/edge-ent-intune/edge-intune-profile-create.png)
1. Click **Settings** to show all available settings.

    ![Create profile](./media/edge-ent-intune/edge-intune-policy-settings.png)
1. On the right upper corner of the window, select the **All products** drop-down and then select **Edge version 77 or later** to filter the list to show only Edge settings.

    ![Create profile](./media/edge-ent-intune/edge-intune-allproducts.png)
1. To configure a setting, select it from the list and use the settings window on the right to enable and configure the setting.

    ![Create profile](./media/edge-ent-intune/edge-intune-settings-config.png)
1. Click **Create** to create the profile.

When you are done, see [Assign user and device profiles in Microsoft Intune](https://docs.microsoft.com/en-us/intune/device-profile-assign) for information about how to assign the profile to your Azure Active Directory (Azure AD) user or device groups.

For more information on Windows 10 profiles, see [Use Windows 10 templates to configure group policy settings in Microsoft Intune](https://docs.microsoft.com/en-us/intune/administrative-templates-windows).

## Add an app to deploy Microsoft Edge for macOS to Intune

The process for adding Microsoft Edge for macOS is similar to the process for Windows devices, but there are certain prerequisites for managing macOS and iOS devices in Intune.

1. An Apple MDM Push certificate is required for Intune to manage iOS and macOS devices. If you haven't already configured Intune for the macOS, follow the instructions in [Get an Apple MDM push certificate](https://docs.microsoft.com/en-us/intune/apple-mdm-push-certificate-get).
1. Download the Microsoft Edge Enterprise **PKG for macOS** from the [Microsoft Edge Enterprise landing page](https://aka.ms/EdgeEnterprise).

    ![Download PKG for macOS](./media/edge-ent-intune/edge-intune-download-mac.png)
1. You must pre-process your .pkg file before you can upload the Microsoft Edge for macOS installation file to Microsoft Intune. Follow the instructions in [Deploy Microsoft Edge for macOS using Microsoft Intune](deploy-edge-to-the-mac.md#deploy-microsoft-edge-for-macos-using-microsoft-intune) to pre-process the file and add the app to Intune. You can refer to the instructions in the [Add Microsoft Edge for Windows to Intune](#add-an-app-to-deploy-microsoft-edge-for-windows-10-to-intune) section for information specific to Microsoft Edge.
    >[!NOTE]
    >The pre-processing of the .pkg file must take place on a macOS device.

1. Follow the instructions in [Assign apps to groups with Microsoft Intune](https://docs.microsoft.com/en-us/intune/apps-deploy) to learn how to deploy the app to users.
1. You can create custom settings for your macOS devices in Intune by creating a custom profile. Follow the instructions in [Use custom settings for macOS devices in Microsoft Intune](https://docs.microsoft.com/en-us/intune/custom-settings-macos) to create a custom profile for macOS devices.

## See also

- [Overview of Microsoft Edge in the enterprise](overview-edge-in-the-enterprise.md)
- [Microsoft Edge Enterprise landing page](https://aka.ms/EdgeEnterprise)
- [Manage web access by using Microsoft Edge with Microsoft Intune](https://docs.microsoft.com/en-us/intune/manage-microsoft-edge)
- [Use Windows 10 templates to configure group policy settings in Microsoft Intune](https://docs.microsoft.com/en-us/intune/administrative-templates-windows)
- [Add apps to Microsoft Intune](https://docs.microsoft.com/en-us/intune/apps-add)
- [Add a Windows line-of-business app to Microsoft Intune](https://docs.microsoft.com/en-us/intune/lob-apps-windows)
- [Assign apps to groups with Microsoft Intune](https://docs.microsoft.com/en-us/intune/apps-deploy)
- [Deploy Microsoft Edge for macOS using Microsoft Intune](deploy-edge-to-the-mac.md#deploy-microsoft-edge-for-macos-using-microsoft-intune)
- [Use custom settings for macOS devices in Microsoft Intune](https://docs.microsoft.com/en-us/intune/custom-settings-macos)
