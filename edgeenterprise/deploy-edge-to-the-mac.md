---
title: "Deploy Microsoft Edge for MacOS using Jamf"
ms.author: srugh
author: kelleyvice-MSFT
manager: laurawi
ms.date: 7/10/2019
audience: ITPro
ms.topic: reference
ms.prod: microsoft-edge
localization_priority: high
ms.collection:
ms.custom:
description: "Documentation for automating Edge deployment with Jamf."
---

## Deploy Microsoft Edge for MacOS using Jamf
You can automate deployment of Microsoft Edge for MacOS using Jamf.

### Prerequisites

- Make sure that the Microsoft Edge PKG installation file, **MicrosoftEdgeDev-<version>.pkg** is in an accessible location on your network.
- Ensure that you have permissions and log in to your Jamf Cloud account.

To deploy Microsoft Edge for MacOS using Jamf:

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

Congratulations! You’ve just finished deploying Microsoft Edge for MacOS using Jamf.

You will have the deployed Microsoft Edge package configured when the defined trigger condition is true.

## See also

- [Overview of Edge in the enterprise](overview-edge-in-the-enterprise.md)
- [Microsoft Edge Enterprise landing page](https://aka.ms/EdgeEnterprise)
- [Jamf.com](https://www.jamf.com/)
