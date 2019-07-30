---
title: "Deploy Microsoft Edge for macOS using Jamf"
ms.author: srugh
author: kelleyvice-MSFT
manager: laurawi
ms.date: 07/12/2019
audience: ITPro
ms.topic: reference
ms.prod: microsoft-edge
localization_priority: medium
ms.collection: M365-modern-desktop
description: "Documentation for automating Edge deployment with Jamf."
---

# Deploy to macOS

You can deploy Microsoft Edge for macOS using Microsoft Intune or Jamf.

> [!NOTE]
> This article applies to Microsoft Edge version 77 or later.

## Deploy Microsoft Edge for macOS using Microsoft Intune

You can deploy the Microsoft Edge .pkg installer as a line-of-business application using Microsoft Intune. This requires pre-processing the .pkg installer on a macOS device using the Intune App Wrapping Tool. The tool generates a .intunemac file that is uploaded to Microsoft Intune.

### Prerequisites

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

To deploy Microsoft Edge for macOS using Microsoft Intune:

1. Sign in to [Intune](https://go.microsoft.com/fwlink/?linkid=2090973).
2. On the **Intune** pane, choose **Client apps** > **Apps** > **Add** > **Line-of-business app** > **App package file**.
3. On the **App package file** pane, choose the browse button, and select the wrapped Microsoft Edge installation file with the extension *.intunemac*. When you are finished, choose **OK**.
4. Configure app information. When you are finished, choose **OK**. 
5. On the **Add app** pane, verify that the details for your app is correct.
6. Choose **Add**, to upload the app to Intune.
7. The app you have added is displayed in the apps list. You can now assign it to the groups you choose.

## Deploy Microsoft Edge for macOS using Jamf

You can automate deployment of Microsoft Edge for macOS using Jamf.

### Prerequisites

- Make sure that the Microsoft Edge installation file, **MicrosoftEdgeDev-\<version\>.pkg** is in an accessible location on your network. You can download the Microsoft Edge Enterprise installation files from the [Microsoft Edge Enterprise landing page](https://aka.ms/EdgeEnterprise).
- Ensure that you have permissions and log in to your Jamf Cloud account.

To deploy Microsoft Edge for macOS using Jamf:

1. Navigate to All Settings and click **Computer Management**.

    ![Click Computer Management](./media/mac-deploy/mac-1.png)

2. Click **Packages**.

    ![Click Packages](./media/mac-deploy/mac-2.png)

3. Click **New** to add a new package.

    ![Click New to add package](./media/mac-deploy/mac-3.png)

4. Enter the details of the new package and click **Save**.

    ![Click Save](./media/mac-deploy/mac-4.png)

    The new Microsoft Edge package is displayed under Packages.

    ![New package is displayed](./media/mac-deploy/mac-4a.png)

5. Navigate to **Computers**, select **Policies**, and then select **New**.
    - The new Policy pane is displayed.

    ![New policy pane](./media/mac-deploy/mac-5.png)

6. In the Options tab, select **General**.
    - Enter the display name for the policy.
    - Select the event to trigger the policy.

    ![Enter deployment details](./media/mac-deploy/mac-6.png)

7. Under the Options tab, click **Packages**. Then click **Configure**.

    ![Configure package](./media/mac-deploy/mac-7.png)

8. The package that you added earlier is displayed. Click **Add**.
    ![Add package](./media/mac-deploy/mac-8.png)

9. Select the distribution point and action, then click **Save**.
    ![Select distribution point](./media/mac-deploy/mac-9.png)

10. Click the **Scope** tab. From the TARGET COMPUTERS drop-down list, select the computers to deploy the package to. Click **Save**.
    ![Save the policy](./media/mac-deploy/mac-10.png)

11. Click **Done**.
    ![Click done](./media/mac-deploy/mac-11.png)

Congratulations! You’ve just finished deploying Microsoft Edge for macOS using Jamf.

You will have the deployed Microsoft Edge package configured when the defined trigger condition is true.

## See also

- [Overview of Microsoft Edge in the enterprise](overview-edge-in-the-enterprise.md)
- [Microsoft Edge Enterprise landing page](https://aka.ms/EdgeEnterprise)
- [Jamf.com](https://www.jamf.com/)
