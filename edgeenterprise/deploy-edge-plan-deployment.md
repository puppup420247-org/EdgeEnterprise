---
title: "Plan your Deployment of Microsoft Edge"
ms.author: cjacks
author: appcompatguy
manager: saudm
ms.date: 11/12/2019
audience: ITPro
ms.topic: procedural
ms.prod: microsoft-edge
ms.localizationpriority: high
ms.collection: M365-modern-desktop
description: "Plan your deployment of Microsoft Edge"
---

# Plan your Deployment of Microsoft Edge

This article reviews recommended practices for deploying Microsoft Edge in an enterprise environment.

>[!NOTE]
>This article applies to Microsoft Edge version 77 or later.

## Evaluate your existing browser environment and browser needs

Taking time to understand your current state and project vision will help ensure that all project stakeholders are aligned and working towards the same end result.

Start with defining your current state:

- Which browsers are currently deployed in your environment?
- Which browser is set as the default browser?
- Do you need to use Internet Explorer for some of your apps?
- Do you use an Enterprise Mode Site List to configure Internet Explorer today?
- What OS platforms are supported in your environment? (Windows 10, macOS, Windows 7, Windows Server, etc.)
- What management tools do you use for browser management?
- Who is responsible for browser configuration and management?
- What is your process for validating browser compatibility?

Once you understand the current state, you can determine the desired state of your deployment:

- Do you want to [set Microsoft Edge as your default browser](https://docs.microsoft.com/en-us/DeployEdge/edge-default-browser)?
- Do you want to hide the legacy version of Microsoft Edge, or do you want to [leave it available for users](https://docs.microsoft.com/en-us/DeployEdge/microsoft-edge-sysupdate-access-old-edge)?
- How will you [configure Microsoft Edge](https://docs.microsoft.com/en-us/DeployEdge/configure-microsoft-edge)?
- What features are critical to configure as part of your initial deployment?
- What is the process for addressing any identified compatibility or configuration issues?

You should also understand the **pre-requisites** for features you are interested in, such as:

- [Windows Defender Application Guard](https://docs.microsoft.com/en-us/windows/security/threat-protection/windows-defender-application-guard/reqs-wd-app-guard)
- [Internet Explorer mode](https://docs.microsoft.com/en-us/DeployEdge/edge-ie-mode)
- [Authentication and sync](https://docs.microsoft.com/en-us/DeployEdge/microsoft-edge-security-identity)

With these answers in mind, you are ready to plan your deployment.

## Determine your deployment methodology

Once you know your desired end state, you are ready to start planning how to get there. There are two primary ways to deploy Microsoft Edge:

### Deploy to end users by role

If app compat is your primary concern, and you don't have a firm grasp on apps to test, you may want to consider deploying to end users by role, which allows each wave of a phased deployment to provide insight and feedback on apps which may need to have the configuration modified to address compatibility issues.

### Deploy to end users by site

If bandwidth is your primary concern, you may want to consider performing application compatibility validation up front, and then deploying to end users by site, in order to leverage caching other software delivery optimizations.

## Perform site discovery

If you have a dependency on legacy web applications, and plan to use Internet Explorer mode (which most customers do), then you probably need to perform some additional site discovery.

### If you have already deployed and configured the legacy version of Microsoft Edge

If you have already configured your Enterprise Site List to work  for the legacy version of Microsoft Edge, then your work is almost done! The one thing you may need to add are Neutral Sites.

Neutral Sites are typically sites that provide Single Sign-On (SSO). If navigated to from Microsoft Edge, then you want to stay in Microsoft Edge to authenticate. If navigated to from Internet Explorer mode, then you want to stay in Internet Explorer mode to authenticate.

Identify any SSO (or other neutral) sites that you use, and add these to your Enterprise Site List.

### If you have configured Internet Explorer as your default browser

If you are currently only using Internet Explorer, you may not know which sites have upgraded to modern web standards and which still require Internet Explorer. You will want to discover these sites and add them to the Enterprise Site List in order to leverage Internet Explorer mode only on the sites that require it.

You can use the [Enterprise Site Discovery](https://docs.microsoft.com/en-us/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery?redirectedfrom=MSDN) tools to discover the sites that may require Internet Explorer mode.

Once you have collected this data, we recommend a 4-step process to analyze the data you find:

1. Sort the data by domain, then by URL
2. Define the boundaries of an "app" to configure for Internet Explorer mode - you want to include all of the sites and web controls which define the app, without including any extra sites and controls by defining too broadly. Some sites may be as simple as "http://contoso.com/app1" while others you will need to define multiple pages and sites.
3. Test the app to verify that it does not work natively - many sites will offer modern content when they detect a modern browser, and only offer legacy content when they detect Internet Explorer
4. Add the app to your Enterprise Site list if it fails

Note: A best practice is to group sites so when you upgrade these apps, you make it easy to remove the entire site from Internet Explorer mode and start using a modern browser for that app.

## Determine your channel strategy

Microsoft Edge is released in [multiple channels](https://docs.microsoft.com/en-us/DeployEdge/microsoft-edge-channels).

>[!NOTE]
>You can install more than one channel on a device

The Stable Channel is what you will want to deploy to most devices.

We also recommend having a representative subset of devices configured to use the Beta Channel, in order to get a preview of changes to the browser and any resulting user or compatibility impact from changes in the browser.

You may also want to make the Dev Channel (or even the Canary Channel) available to some roles, such as web developers. Consider whether you would like to target some devices with more rapid channels, or simply make it available for users to opt to install.

Because you can install multiple channels on a device, you reduce the risk of testing. If you have a user who is using the Beta Channel, and there is a problem, they can start using the Stable Channel to unblock their productivity until the issue can be resolved. Note that, if you have enabled Sync, then your configuration will sync across channels, making it even easier to transition between channels.

## Define and configure policies

Once you have prepared your Enterprise Site List, we recommend defining and configuring policies that you intend to deploy with Microsoft Edge, to ensure that these policies are applied when you perform your testing.

First, consider the first-run experience you want your users to have. If you would like to automatically import settings from your current browser, configure the policy for [AutoImportAtFirstRun](https://docs.microsoft.com/en-us/DeployEdge/microsoft-edge-policies#autoimportatfirstrun).

For security policies, we recommend beginning with the Microsoft Edge Security Baseline. The Security Baseline can be applied using [Group Policy](https://techcommunity.microsoft.com/t5/Microsoft-Security-Baselines/Security-baseline-DRAFT-for-Chromium-based-Microsoft-Edge/ba-p/949991) or using [Microsoft Intune](https://docs.microsoft.com/en-us/intune/protect/security-baseline-settings-edge).

For other policies, we recommend reviewing the policy configurations for [Microsoft Edge](https://docs.microsoft.com/en-us/deployedge/microsoft-edge-policies) and [Microsoft Edge Updates](https://docs.microsoft.com/en-us/deployedge/microsoft-edge-update-policies).

### Define your update strategy and policies

You will also want to determine how you will update Microsoft Edge:

- **Allow Microsoft Edge to update itself** (default). If you choose to allow automatic updates of Microsoft Edge, then Microsoft Edge will automatically update itself at the pace determined by the channel(s) you have deployed.
- **Update Microsoft Edge at your own pace**. If you prefer to have explicit control over when updates are deployed, you can disable automatic updates and deploy it yourself (see the [Update Policy reference](https://docs.microsoft.com/en-us/DeployEdge/microsoft-edge-update-policies)). You will then need to deploy each new version of Edge using [Intune](https://docs.microsoft.com/en-us/intune/apps/apps-windows-edge?toc=https://docs.microsoft.com/DeployEdge/toc.json&bc=https://docs.microsoft.com/DeployEdge/breadcrumb/toc.json), [Configuration Manager](https://docs.microsoft.com/en-us/DeployEdge/deploy-edge-with-configuration-manager), or the deployment tool of your choice.

Regardless of your update strategy, we recommend leveraging a ringed deployment strategy. With automatic updates, that means having a representative sample of users running the Beta Channel, in order to identify issues with what will become the Stable Channel. With manual updates, that may also include additional validation of a pilot group once a new Stable Channel build is released, followed by broad deployment.

>[!NOTE]
>Microsoft Edge support will only apply to the most recent version of Microsoft Edge in each channel

## Perform app compat testing

Application compatibility for Microsoft Edge is extremely high - so high that Microsoft provides the following compatibility promises:

1. If it works on Microsoft Edge *version 45 and earlier*, it will work on Microsoft Edge *version 77 and later*.
2. If it works on Internet Explorer, it will work on Microsoft Edge in Internet Explorer mode.
3. If it works on Google Chrome, it will work on Microsoft Edge.

If you have an application where we do not meet this promise, then we stand behind the promise to fix it with [Microsoft App Assure](https://www.microsoft.com/en-us/fasttrack/microsoft-365/desktop-app-assure).

Despite this promise, we know that many organizations have to validate at least some applications for compliance or risk management reasons. So, even though we expect this to be very straightforward, it's nonetheless important to be organized in testing.

There are 2 primary ways to perform app compat testing:

1. Lab testing - applications are validated in a controlled environment, typically in a lab
2. Pilot testing - applications are validated by a limited number of users in their daily work environment

Choose the method that is most appropriate for each app, in order to manage risk without over-investing in compatibility testing.

## Deploy Microsoft Edge to a pilot group

Once you have defined your policies and performed initial app compat testing, you are ready to deploy to your pilot group!

If you are using Microsoft Intune, you can easily deploy it for both [Windows 10](https://docs.microsoft.com/en-us/intune/apps/apps-windows-edge) and [macOS](https://docs.microsoft.com/en-us/intune/apps/apps-edge-macos).

If you are using [Configuration Manager, you can easily deploy Microsoft Edge for Windows 10](https://docs.microsoft.com/en-us/DeployEdge/deploy-edge-with-configuration-manager).

If you are using another management tool, you can download and deploy the [MSI file for Microsoft Edge](https://www.microsoftedgeinsider.com/en-us/enterprise).

## Validate your deployment

Once you have deployed the pilot, you want to capture all of the feedback you get from your users.

- Capture feedback on compatibility, in case there are sites that belong on the Enterprise Site List which were not identified while you were preparing the initial list
- Capture feedback on the policy configuration, to ensure that users are able to use key features while still following security guidelines
- Identify any areas where training should be developed and delivered based on user questions

## Broad deployment of Microsoft Edge

Having configured and validated the pilot, you are now ready to execute the broad deployment of Microsoft Edge to all of your users, using the methodology identified during planning. Congratulations!