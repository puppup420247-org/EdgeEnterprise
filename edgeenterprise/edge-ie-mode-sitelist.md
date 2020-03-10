---
title: "Configure Sites on the Enterprise Mode Site List"
ms.author: cjacks
author: cjacks
manager: saudm
ms.date: 03/05/2020
audience: ITPro
ms.topic: conceptual
ms.prod: microsoft-edge
ms.localizationpriority: high
ms.collection: M365-modern-desktop
description: "Configure Enterprise Site List"
---

# Configure Sites on the Enterprise Mode Site List

This article describes changes to the Enterprise Mode Site List which support configuring IE mode for Microsoft Edge version 77 and later.

For additional details on the schema for the Enterprise Mode Site List XML file, see [Enterprise Mode schema v.2 guidance](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/enterprise-mode-schema-version-2-guidance).

## Updated schema elements

The following table describes the \<open-in app\> element added to the v.2 of the Enterprise Mode schema:

| **Element** | **Description** |
| --- | --- |
| \<open-in app="**true**"\> | A child element that controls what browser is used for sites. This element is required for sites that need to **open in IE11**.|

**Example:**

``` xml
<site url="contoso.com">

  <open-in app="true">IE11</open-in>

</site>
```

The following table shows the possible values of the \<open-in\> element:

| **Value** | **Description** |
| --- | --- |
| **\<open-in\>IE11\</open-in\>** | Opens the site in IE mode, when the user is in Microsoft Edge and "Configure Internet Explorer integration" is set to Enabled with the option "Internet Explorer mode". <br> Opens the site in Internet Explorer 11, when the user is in Microsoft Edge and "Configure Internet Explorer integration" is set to Enabled with the option "Internet Explorer 11". |
| **\<open-in app="**true**"\>IE11\</open-in\>** | Opens the site in IE11, regardless of which browser is opened by the user. |
| **\<open-in\>MSEdge\</open-in\>** | Opens the site in Microsoft Edge, regardless of which browser is opened by the user. |
| **\<open-in\>None or not specified\</open-in\>** | Opens the site in the default browser or in the browser where navigation was initiated. |

>[!NOTE]
> The attribute app=**"true"** is only recognized when associated to _'open-in' IE11_. Adding it to the other 'open-in' elements won't change browser behavior.   

## Configure neutral sites

In order for IE mode to work properly, authentication/ Single Sign-On servers will need to be explicitly configured as neutral sites. Otherwise, IE mode pages will try to redirect to Microsoft Edge (which is expected behavior for any site not on the site list), causing authentication to fail. This will result in a message to the user that they are not authenticated or in most cases, result an infinite authentication loop. 

Navigation to a neutral site will remain where it started - either in Microsoft Edge or in IE mode. Additionally, configuring neutral sites ensures that modern applications using the same authentication servers are not impacted. 

You can configure neutral sites by setting the *Open In* dropdown to 'None' in the Enterprise Mode Site List Manager tool or by directly updating the site list XML:

``` xml
<site url="login.contoso.com">
   
    <open-in>None</open-in>

</site>
```

To identify authentication servers, you can inspect the site in standalone IE11 with Developer Tools. If you need time to identify your authentication servers, you can configure a policy to ensure that all in-page navigations from IE mode remain in IE mode. It is recommended that you revisit this setting once you have identified and added your authentication servers to the site list. For more information, see [Configure in-page navigations to remain in IE mode](https://docs.microsoft.com/deployedge/microsoft-edge-policies#internetexplorerintegrationsiteredirect).


>[!NOTE]
   >Enterprise Mode schema v.1 isn't supported for IE mode integration. If you are currently using schema v.1 with Internet Explorer 11, you must upgrade to schema v.2. For more information, see [Enterprise Mode schema v.2 guidance](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/enterprise-mode-schema-version-2-guidance).
