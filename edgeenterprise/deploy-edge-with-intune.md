---
title: "Deploy Microsoft Edge for Windows 10 using Microsoft Intune"
ms.author: kvice
author: kelleyvice-msft
manager: laurawi
ms.date: 09/18/2019
audience: ITPro
ms.topic: procedural
ms.prod: microsoft-edge
localization_priority: medium
ms.collection: M365-modern-desktop
description: "Learn how to deploy Microsoft Edge for Windows 10 using Microsoft Intune."
---

# Deploy Microsoft Edge for Windows 10 using Microsoft Intune

This article shows you how to automate Microsoft Edge deployment and policy configuration for Windows 10 by using Microsoft Intune.

>[!NOTE]
>This article applies to Microsoft Edge version 77 or later.

You can deploy Microsoft Edge to Windows clients that are managed in your company's Intune tenant by adding apps containing the Microsoft Edge installation files to Intune. Like any Intune apps, you can configure app assignments to require Microsoft Edge deployment for selected users or devices. You can also make the app available in the Company Portal for users to install when they want to.

Additionally, you can configure Microsoft Edge policies and settings by adding a device configuration profile. Using Intune to manage and enforce policies is essentially equivalent to using Active Directory Group Policy or configuring local Group Policy Object (GPO) settings on user devices. For more information, see [Configure Microsoft Edge for Windows 10 using Microsoft Intune](configure-edge-with-intune.md).

>[!TIP]
>For more information about deploying Microsoft Edge for macOS using Windows Intune, see [Deploy to macOS with Microsoft Intune](deploy-edge-mac-intune.md).

## Before you begin

- Review the information in [Add a Windows line-of-business app to Microsoft Intune](https://docs.microsoft.com/en-us/intune/lob-apps-windows).
- To create apps for **Windows 10**, download the Microsoft Edge Enterprise installation **.msi files** from the [Microsoft Edge Enterprise landing page](https://aka.ms/EdgeEnterprise). The installation files use the build channel and processor architecture in their names, and will have names like **MicrosoftEdgeDevEnterpriseX86.msi** or **MicrosoftEdgeBetaEnterpriseX64.msi**.
- To create apps for **macOS**, download the Microsoft Edge Enterprise **PKG for macOS** from the [Microsoft Edge Enterprise landing page](https://aka.ms/EdgeEnterprise).
- Make sure you store the Microsoft Edge installation files in an accessible local or network location.

## Add an app to deploy Microsoft Edge for Windows 10 to Intune

This procedure creates an app for deploying Microsoft Edge for Windows 10 in Intune.

>[!NOTE]
>You can only deploy Microsoft Edge with Mobile Device Management (MDM). Deploying with Mobile Application Management (MAM) isn't supported.

1. Sign in to the [Microsoft Azure portal](https://portal.azure.com).
2. Select **Intune** from _All Services_, or search for Intune in the portal search box.
3. From the _Microsoft Intune - Overview_ blade, select **Client apps** | **Apps**.

    ![Client apps](./media/edge-ent-intune/edge-intune-apps.png)

4. On the top command bar, select **Add**.
5. Initially, there's only one field named **App type**.

    ![App type](./media/edge-ent-intune/edge-intune-app-add-app-1.png)

6. Select **Line-of-business app** from the drop-down list and additional fields are shown.

    ![Line-of-business app](./media/edge-ent-intune/edge-intune-app-add-app-2.png)

7. Select **App package file**, and use the file chooser to pick the .msi installation file. Information about the file will display under the file selection field. Click **OK** to continue.

    ![App package file](./media/edge-ent-intune/edge-intune-app-package-file.png)

8. Click **App information** and enter the following values:

    |Field  |Value  |
    |---------|---------|
    |Name     |This field is populated from the installer, but you can change it if you want          |
    |Description     |Enter a description         |
    |Publisher     |Microsoft         |
    |App install context     |This value is pre-selected and can't be modified         |
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

9. Optionally, select **Scope (Tags)** to apply existing tags for limiting deployment of the app to a specific scope.
10. Click **Add** to add the app.

When you're finished, see [Assign apps to groups with Microsoft Intune](https://docs.microsoft.com/en-us/intune/apps-deploy) to learn how to deploy the app to users.

**Other resources:**

- You can refer to the procedures in [Add a Windows line-of-business app to Microsoft Intune](https://docs.microsoft.com/en-us/intune/lob-apps-windows) for general guidance and additional details.
- See [Add apps to Microsoft Intune](https://docs.microsoft.com/en-us/intune/apps-add) for information about general Intune app considerations, organization and troubleshooting.

## See also

- [Overview of Microsoft Edge in the enterprise](overview-edge-in-the-enterprise.md)
- [Microsoft Edge Enterprise landing page](https://aka.ms/EdgeEnterprise)
- [Use Windows 10 templates to configure group policy settings in Microsoft Intune](https://docs.microsoft.com/en-us/intune/administrative-templates-windows)
- [Add apps to Microsoft Intune](https://docs.microsoft.com/en-us/intune/apps-add)
- [Add a Windows line-of-business app to Microsoft Intune](https://docs.microsoft.com/en-us/intune/lob-apps-windows)
- [Assign apps to groups with Microsoft Intune](https://docs.microsoft.com/en-us/intune/apps-deploy)
