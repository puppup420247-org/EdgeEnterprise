---
title: "Configure IE mode Policies"
ms.author: cjacks
author: cjacks
manager: saudm
ms.date: 03/05/2020
audience: ITPro
ms.topic: conceptual
ms.prod: microsoft-edge
ms.localizationpriority: high
ms.collection: M365-modern-desktop
description: "Configure IE mode policies"
---

# Configure IE mode policies

This article explains how to configure IE mode policies.

Configuring IE mode requires three steps:

1. [Configure Internet Explorer integration](#Configure-Internet-Explorer-Integration)
2. [Redirect sites from Microsoft Edge to IE mode](#Redirect-sites-from-Microsoft-Edge-to-IE-mode)
3. (Optional) [Redirect sites from IE to Microsoft Edge](#Redirect-sites-from-IE-to-Microsoft-Edge)

> [!NOTE]
> Policies to enable IE mode can be configured through Intune. For more information, see [Add Microsoft Edge to Microsoft Intune](https://docs.microsoft.com/intune/apps/apps-windows-edge?toc=https://docs.microsoft.com/DeployEdge/toc.json&bc=https://docs.microsoft.com/DeployEdge/breadcrumb/toc.json) and [Configure Microsoft Edge policies with Microsoft Intune](https://docs.microsoft.com/DeployEdge/configure-edge-with-intune).

## Configure Internet Explorer integration

Internet Explorer can be integrated either to open directly within Microsoft Edge (IE mode), or to open with a standalone Internet Explorer 11 window. Most users prefer when sites open directly within Microsoft Edge in IE mode.

### Enable Internet Explorer integration using Group Policy

1. Download and use the latest [Microsoft Edge Policy Template](https://www.microsoft.com/en-us/edge/business/download).
2. Open Group Policy Editor.
3. Click **Computer Configuration** > **Administrative Templates** > **Microsoft Edge**.
4. Double-click **Configure Internet Explorer integration**.
5. Select **Enabled**.
6. Under **Options**, set the dropdown value to 
   -  **Internet Explorer mode** if you want sites to open in IE mode on Edge
   -  **Internet Explorer 11** if you want sites to open in a standalone Internet Explorer 11 window
   -  **None** if you want to disable Internet Explorer mode when it is set via edge://flags or through command line options.

   > [!NOTE]
   > Setting the policy to **Disabled** implies IE mode is disabled by policy, but can be set through edge://flags or command line options.
7. Click **OK** or **Apply** to save this policy setting.

## Redirect sites from Microsoft Edge to IE mode

There are 2 options for identifying which sites should open in IE mode:

- (Recommended) [Configure sites on the Enterprise Site list](#configure-sites-on-the-enterprise-site-list)
- [Configure all Intranet sites](#configure-all-intranet-sites)

### Configure sites on the Enterprise Site list

You can use the following group policies to configure specific sites to open in IE mode:

- [Use the Enterprise Mode IE website list](#Configure-using-the-Use-the-Enterprise-Mode-IE-website-list-policy) (Internet Explorer)
- [Configure the Enterprise Mode Site List](#Configure-using-the-Configure-the-Enterprise-Mode-Site-List-policy) (Microsoft Edge, version 78 or later)<br/>This policy lets you create a separate Enterprise Mode Site list for Microsoft Edge. Enabling this policy overrides the settings in the "Use the Enterprise Mode IE website list" policy, provided that "Configure Internet Explorer integration" is enabled. Disabling or not configuring this policy doesn't affect the default behavior of the "Configure Internet Explorer integration" policy.
    > [!NOTE]
    > It is not mandatory to configure the Microsoft Edge policy. Many organizations use this as an override, allowing them to target the current Site List at all users with the IE policy, and more easily target an updated version to pilot uses with the Microsoft Edge policy.

For more information about Enterprise Mode Site lists, see:

- [Use the Enterprise Mode Site List Manager](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/use-the-enterprise-mode-site-list-manager)
- [Add multiple sites to the Enterprise Mode site list using a file and the Enterprise Mode Site List Manager (schema v.2)](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/add-multiple-sites-to-enterprise-mode-site-list-using-the-version-2-schema-and-enterprise-mode-tool).

### Configure using the Use the Enterprise Mode IE website list policy

IE mode can use the existing policy configuring the Enterprise Site List for Internet Explorer, allowing you to create and maintain a single list.

1. Create or re-use a Site List XML
    1. All sites that have the element _\<open-in\>IE11\</open-in\>_ will now open in IE mode.
2. Open Group Policy Editor.
3. Click **Computer Configuration** > **Administrative Templates** > **Windows Components** > **Internet Explorer**.
4. Double-click **Use the Enterprise Mode IE website list**.
5. Select **Enabled**.
6. Under **Options**, type the location of website list. You can use one of the following locations:
    - (Recommended) HTTPS location: **https**:**//iemode/sites.xml**
    - Local network file: **\\\network\shares\sites.xml**
    - Local file: **file:///c:/Users/\<user\>/Documents/sites.xml**
7. Click **OK** or **Apply** to save these settings.

### Configure using the Configure the Enterprise Mode Site List policy

IE mode can also be configured with a separate policy for Microsoft Edge. This allows you to override the existing site list for the sake of conducting a limited pilot, or to manage a separate list of only sites that need IE.

1. Create or re-use a Site List XML
    1. All sites that have the element _\<open-in\>IE11\</open-in\>_ will now open in IE mode.
2. Open Group Policy Editor.
3. Click **Computer Configuration** > **Administrative Templates** > **Microsoft Edge**.
4. Double-click **Configure the Enterprise Mode Site List**.
5. Select **Enabled**.
6. Under **Options**, type the location of website list. You can use one of the following locations:
    - (Recommended) HTTPS location: **https**:**//iemode/sites.xml** <!--Trying to keep this from being an active link in MD -->
    - Local network file: **\\\network\shares\sites.xml**
    - Local file: **file:///c:/Users/\<user\>/Documents/sites.xml**
7. Click **OK** or **Apply** to save these settings.

### Configure all intranet sites

IE mode can be configured as enabled by default for the Local Intranet zone. You can still opt a site in the Local Intranet zone out of using IE mode by implementing an Enterprise Mode Site List, specifying the URL, and configuring the site to open in Microsoft Edge.

>[!NOTE]
>
> The Local Intranet zone contains explicitly added sites, but also assigns sites to this zone using heuristics. This can include dotless host names (e.g. **https**:**//payroll**) and sites that the proxy configuration script configures to bypass the proxy. If an external party controls DNS or proxy, they could potentially force websites into IE mode.

1. Open Local Group Policy Editor.
2. Click **Computer Configuration** > **Administrative Templates** > **Microsoft Edge**.
3. Double-click **Send all intranet sites to Internet Explorer**.
4. Select **Enabled**, and then click **OK** or **Apply** to save the policy settings.

## Redirect sites from IE to Microsoft Edge

If you only want users to use Internet Explorer for those sites that require it, and would like to prevent Internet Explorer from being used for other sites, you can configure Internet Explorer to automatically redirect any sites that are not on the Enterprise Mode Site List back to Microsoft Edge.

1. Open Group Policy Editor.
2. Click **Computer Configuration** > **Administrative Tools** > **Windows Components** > **Internet Explorer**.
3. Double-click **Send all sites not included in the Enterprise Mode Site List to Microsoft Edge.**
4. Select **Enabled**
5. Click **OK** or **Apply** to save these settings.
6. Double-click **Configure which channel of Microsoft Edge to use for opening redirected sites**.
7. Select **Enabled**.
8. Under **Options**, select your top three choices for the channel to use - Internet Explorer will redirect to the highest ranked choice that the user has installed on that device:
   - Microsoft Edge Stable
   - Microsoft Edge Beta version 77 or later
   - Microsoft Edge Dev version 77 or later
   - Microsoft Edge Canary version 77 or later
   - Microsoft Edge version 45 or earlier
9. Click **OK** or **Apply** to save these settings.

