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

This article shows you how to automate Microsoft Edge deployment and policy configuration for Windows 10 and macOS by using Microsoft Intune.

>[!NOTE]
>This article applies to Microsoft Edge version 77 or later.

You can deploy Microsoft Edge to Windows and macOS clients that are managed in your company's Intune tenant by adding apps containing the Microsoft Edge installation files to Intune. Like any Intune apps, you can configure app assignments to require Microsoft Edge deployment for selected users or devices or simply make the app available in the Company Portal for users to install at their discretion.

You can also configure Microsoft Edge policies and settings by adding a custom device configuration profile. If your company primarily uses Intune to manage and enforce policies on user devices, this is a good alternative to using Active Directory Group Policy or configuring local GPO settings on user devices.

You can read [Manage web access by using Microsoft Edge with Microsoft Intune](https://docs.microsoft.com/en-us/intune/manage-microsoft-edge) to learn more, but keep in mind that this article is specific to Microsoft Edge (EdgeHTML), not Microsoft Edge Enterprise (Chromium-based).

## Before you begin

- Review the information in [Add a Windows line-of-business app to Microsoft Intune](https://docs.microsoft.com/en-us/intune/lob-apps-windows).
- To create apps for **Windows 10**, download the Microsoft Edge Enterprise installation **.msi files** from the [Microsoft Edge Enterprise landing page](https://aka.ms/EdgeEnterprise). The installation files use the build channel and processor architecture in their names, and will be named like **MicrosoftEdgeDevEnterpriseX86.msi** or **MicrosoftEdgeBetaEnterpriseX64.msi**.
- To create apps for **macOS**, download the Microsoft Edge Enterprise **PKG for macOS** from the [Microsoft Edge Enterprise landing page](https://aka.ms/EdgeEnterprise).
- If you want to configure policies and settings for Microsoft Edge for Windows 10 using Intune, download the **Microsoft Edge policy template file** from the [Microsoft Edge Enterprise landing page](https://aka.ms/EdgeEnterprise).
- Make sure you store the Microsoft Edge installation and policy files in an accessible network location.

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

## Create a custom profile to manage Microsoft Edge for Windows 10

Using Microsoft Intune, you can add or create custom settings for your Windows 10 devices using _custom device configuration profiles_. Windows 10 custom profiles use Open Mobile Alliance Uniform Resource Identifier (OMA-URI) settings to configure different features. This section will help you create a custom profile for Windows 10 devices and import the Microsoft Edge policy template using ADMX ingestion to enable configuration of Microsoft Edge-specific application settings.

This procedure creates a new custom profile and imports the settings and policies from the Microsoft Edge policy template file **msedge.admx**. When you are done, go to [Add settings to the Microsoft Edge custom profile](#add-settings-to-the-microsoft-edge-for-windows-10-custom-profile) to configure specific settings.

1. If you haven't already, download the Microsoft Edge policy template .zip file from the [Microsoft Edge Enterprise landing page](https://aka.ms/EdgeEnterprise). You'll find the msedge.admx file at _/windows/admx/msedge.admx_.
1. Sign in to the [Microsoft Azure portal](https://portal.azure.com).
1. Select **Intune** from _All Services_, or search for Intune in the portal search box.
1. From the _Microsoft Intune - Overview_ blade, select **Device configuration** | **Profiles**.
1. On the top bar, select **Create profile**.

    ![Create profile](./media/edge-ent-intune/edge-intune-management-profile-create.png)
1. Enter the following values:

    |Field  |Value  |
    |---------|---------|
    |Name     |Enter a descriptive name, like _Edge Enterprise Configuration_         |
    |Description     |Optionally enter a description         |
    |Platform     |Windows 10 and later         |
    |Profile type     |Custom         |

1. Click **Settings**. The _Custom OMA-URI Settings_ blade opens to the right.
1. Click **Add**, and enter the following values:

    |Field  |Value  |
    |---------|---------|
    |Name     |Enter a descriptive name, like _Edge ADMX Ingestion_         |
    |Description     |Optionally enter a description         |
    |OMA-URI     |./Device/Vendor/MSFT/Policy/ConfigOperations/ADMXInstall/Edge/Policy/EdgeAdmx         |
    |Data type     |String         |

    ![Add row](./media/edge-ent-intune/edge-intune-management-profile-add-row.png)

1. When you select **String** from the _Data type_ drop-down, a **Value** field appears below. In a text editor, copy the entire contents of the **msedge.admx** file from the policy template you downloaded earlier and paste it into the **Value** field.
1. Click **OK** and **OK** again to save the OMA-URI settings.
1. Click **Create** to create the custom profile.

>[!NOTE]
>You can also configure the custom profile's **Scope** and **Applicability rules** to target specific devices.

### Add settings to the Microsoft Edge for Windows 10 custom profile

Now you can add specific application settings to the custom profile by adding rows containing OMA-URI strings and values. For a list of all available policies, see [Microsoft Edge - Policies](microsoft-edge-policies.md).

>[!NOTE]
>You can calculate the OMA-URI value for a given policy. See [URI format for configuring an app policy](https://docs.microsoft.com/en-us/windows/client-management/mdm/win32-and-centennial-app-policy-configuration#uri-format-for-configuring-an-app-policy) for more information.

In the following example, we will add a setting to always show the Home button in Microsoft Edge.

1. In Intune, select **Device configuration** | **Profiles**.
1. Locate the profile you created earlier and select it.
1. Click **Properties**, and in the pane that appears to the right, click **Settings**.
1. In the _Custom OMA-URI Settings_ pane, click **Add** and enter the following values:

    |Field  |Value  |
    |---------|---------|
    |Name     |Enter a descriptive name, like _ShowHomeButton_         |
    |Description     |Optionally enter a description         |
    |OMA-URI     |./Device/Vendor/MSFT/Policy/Config/Edge~Policy~microsoft_edge~Startup/ShowHomeButton         |
    |Data type     |String         |
    |Value        |\<enabled/\>    |

    ![Add row](./media/edge-ent-intune/edge-intune-management-profile-setting-add-row.png)

1. Click **OK** and **OK** again to save the OMA-URI settings.
1. Click **Save**.

When you are done, see [Assign user and device profiles in Microsoft Intune](https://docs.microsoft.com/en-us/intune/device-profile-assign) for information about how to assign the profile to your Azure Active Directory (Azure AD) user or device groups.

See [Use custom settings for Windows 10 devices in Intune](https://docs.microsoft.com/en-us/intune/custom-settings-windows-10) for more information about custom profiles in Intune, and [Win32 and Desktop Bridge app policy configuration](https://docs.microsoft.com/en-us/windows/client-management/mdm/win32-and-centennial-app-policy-configuration) for more information about how ADMX ingestion works for setting Windows policies using Intune.

## Create a custom profile to update Microsoft Edge for Windows 10

You can create a custom profile to control Microsoft Edge updates using the msedgeupdate.admx file in the Microsoft Edge policy template file.

This procedure creates a new custom profile and imports the settings and policies from the Microsoft Edge policy template file **msedgeupdate.admx**. When you are done, go to [Add settings to the Microsoft Edge update custom profile](#add-settings-to-the-microsoft-edge-for-windows-10-update-custom-profile) to configure specific settings.

1. If you haven't already, download the Microsoft Edge policy template .zip file from the [Microsoft Edge Enterprise landing page](https://aka.ms/EdgeEnterprise). You'll find the msedgeupdate.admx file at _/windows/admx/msedgeupdate.admx_.
1. Sign in to the [Microsoft Azure portal](https://portal.azure.com).
1. Select **Intune** from _All Services_, or search for Intune in the portal search box.
1. From the _Microsoft Intune - Overview_ blade, select **Device configuration** | **Profiles**.
1. On the top bar, select **Create profile**.

    ![Create profile](./media/edge-ent-intune/edge-intune-update-profile-create.png)
1. Enter the following values:

    |Field  |Value  |
    |---------|---------|
    |Name     |Enter a descriptive name, like _Edge Enterprise Update Policies_         |
    |Description     |Optionally enter a description         |
    |Platform     |Windows 10 and later         |
    |Profile type     |Custom         |

1. Click **Settings**. The _Custom OMA-URI Settings_ blade opens to the right.
1. Click **Add**, and enter the following values:

    |Field  |Value  |
    |---------|---------|
    |Name     |Enter a descriptive name, like _Edge Update ADMX Ingestion_         |
    |Description     |Optionally enter a description         |
    |OMA-URI     |./Device/Vendor/MSFT/Policy/ConfigOperations/ADMXInstall/EdgeUpdate/Policy/EdgeUpdateAdmx         |
    |Data type     |String         |

    ![Add row](./media/edge-ent-intune/edge-intune-update-profile-add-row.png)

1. When you select **String** from the _Data type_ drop-down, a **Value** field appears below. In a text editor, copy the entire contents of the **msedgeupdate.admx** file from the policy template you downloaded earlier and paste it into the **Value** field.
1. Click **OK** and **OK** again to save the OMA-URI settings.
1. Click **Create** to create the custom profile.

### Add settings to the Microsoft Edge for Windows 10 update custom profile

Now you can add specific update settings to the custom profile by adding rows containing OMA-URI strings and values. For a list of all available update policies, see [Microsoft Edge - Update Policies](microsoft-edge-update-policies.md).

>[!NOTE]
>You can calculate the OMA-URI value for a given policy. See [URI format for configuring an app policy](https://docs.microsoft.com/en-us/windows/client-management/mdm/win32-and-centennial-app-policy-configuration#uri-format-for-configuring-an-app-policy) for more information.

In the following example, we will add a setting to disallow installation of Microsoft Edge Canary.

1. In Intune, select **Device configuration** | **Profiles**.
1. Locate the profile you created earlier and select it.
1. Click **Properties**, and in the pane that appears to the right, click **Settings**.
1. In the _Custom OMA-URI Settings_ pane, click **Add** and enter the following values:

    |Field  |Value  |
    |---------|---------|
    |Name     |Enter a descriptive name, like _DisallowMicrosoftEdgeCanary_         |
    |Description     |Optionally enter a description         |
    |OMA-URI     |./Device/Vendor/MSFT/Policy/Config/EdgeUpdate~Policy~Cat_GoogleUpdate~Cat_Applications~Cat_MicrosoftEdgeCanary/Pol_AllowInstallationMicrosoftEdgeCanary         |
    |Data type     |String         |
    |Value        |\<disabled/\>    |

    ![Add row](./media/edge-ent-intune/edge-intune-update-profile-setting-add-row.png)

1. Click **OK** and **OK** again to save the OMA-URI settings.
1. Click **Save**.

When you are done, see [Assign user and device profiles in Microsoft Intune](https://docs.microsoft.com/en-us/intune/device-profile-assign) for information about how to assign the profile to your Azure Active Directory (Azure AD) user or device groups.

See [Use custom settings for Windows 10 devices in Intune](https://docs.microsoft.com/en-us/intune/custom-settings-windows-10) for more information about custom profiles in Intune, and [Win32 and Desktop Bridge app policy configuration](https://docs.microsoft.com/en-us/windows/client-management/mdm/win32-and-centennial-app-policy-configuration) for more information about how ADMX ingestion works for setting Windows policies using Intune.

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
- [Add apps to Microsoft Intune](https://docs.microsoft.com/en-us/intune/apps-add)
- [Add a Windows line-of-business app to Microsoft Intune](https://docs.microsoft.com/en-us/intune/lob-apps-windows)
- [Assign apps to groups with Microsoft Intune](https://docs.microsoft.com/en-us/intune/apps-deploy)
- [Use custom settings for Windows 10 devices in Intune](https://docs.microsoft.com/en-us/intune/custom-settings-windows-10)
- [URI format for configuring an app policy](https://docs.microsoft.com/en-us/windows/client-management/mdm/win32-and-centennial-app-policy-configuration#uri-format-for-configuring-an-app-policy)
- [Deploy Microsoft Edge for macOS using Microsoft Intune](deploy-edge-to-the-mac.md#deploy-microsoft-edge-for-macos-using-microsoft-intune)
- [Use custom settings for macOS devices in Microsoft Intune](https://docs.microsoft.com/en-us/intune/custom-settings-macos)
