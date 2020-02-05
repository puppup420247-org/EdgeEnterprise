---
title: "Microsoft Edge release notes for Stable Channel in 2020"
ms.author: kvice
author: dan-wesley
manager: laurawi
ms.date: 02/05/2020
audience: ITPro
ms.topic: conceptual
ms.prod: microsoft-edge
ms.localizationpriority: high
ms.collection: M365-modern-desktop
description: "Microsoft Edge release notes for Stable Channel in 2020"
---

# Release notes for Microsoft Edge Stable Channel in 2020

These release notes provide information about new features and non-security updates that are included in the Microsoft Edge Stable Channel in 2020.

## Version 80.0.361.45: February 6

### Feature updates

- Added a prompt to verify work or school accounts that are automatically added to Microsoft Edge but aren’t enabled for sync so that users are aware sync isn’t enabled.
- Added SmartScreen protection from downloading potentially unwanted apps.
- Added support for Dolby Vision playback.
- Enabled users of Windows Mixed Reality to view 360° videos on VR headsets.
- Added an option to Reading View to increase text spacing.
- Added support for erasing ink using the eraser side of a pen.
- Added support for using the arrow keys and spacebar to draw on feedback screenshots in editor mode.
- Improved the reliability of screenshots so they stop appearing all black when submitting feedback.
- Added dark theme support to the local new tab page that is shown when the device isn’t connected to the internet.
- Added the ability for websites installed as apps to be restored when a browser session is restored after update, crash, etc.
- Added dark theme support to certain UI that appears when the browser is managed by Group Policy.
- Updated Adobe Flash to version 32.0.0.303.

### Group Policy updates

- 16 new policies have been added. Download the updated Administrative Templates from the [Microsoft Edge Enterprise landing page](https://aka.ms/EdgeEnterprise).
The following table lists the policies that were added.

| Policy name | Caption |
|-------------|---------|
|[AlternateErrorPagesEnabled](https://docs.microsoft.com/en-US/DeployEdge/microsoft-edge-policies#alternateerrorpagesenabled)|Suggest similar pages when a webpage can’t be found|
|[DefaultInsecureContentSetting](https://docs.microsoft.com/en-US/DeployEdge/microsoft-edge-policies#defaultinsecurecontentsetting)|Control use of insecure content exceptions|
|[DNSInterceptionChecksEnabled](https://docs.microsoft.com/en-US/DeployEdge/microsoft-edge-policies#dnsinterceptionchecksenabled)|DNS interception checks enabled|
|[HideFirstRunExperience](https://docs.microsoft.com/en-US/DeployEdge/microsoft-edge-policies#hidefirstrunexperience)|Hide the First-run experience and splash screen|
|[InsecureContentAllowedForUrls](https://docs.microsoft.com/en-US/DeployEdge/microsoft-edge-policies#insecurecontentallowedforurls)|Allow insecure content on specified sites|
|[InsecureContentBlockedForUrls](https://docs.microsoft.com/en-US/DeployEdge/microsoft-edge-policies#insecurecontentblockedforurls)|Block insecure content on specified sites|
|[LegacySameSiteCookieBehaviorEnabled](https://docs.microsoft.com/en-US/DeployEdge/microsoft-edge-policies#legacysamesitecookiebehaviorenabled)|Enable default legacy SameSite cookie behavior setting|
|[LegacySameSiteCookieBehaviorEnabledForDomainList](https://docs.microsoft.com/en-US/DeployEdge/microsoft-edge-policies#legacysamesitecookiebehaviorenabledfordomainlist)|Revert to legacy SameSite behavior for cookies on specified sites|
|[PaymentMethodQueryEnabled](https://docs.microsoft.com/en-US/DeployEdge/microsoft-edge-policies#paymentmethodqueryenabled)|Allow websites to query for available payment methods|
|[PersonalizationReportingEnabled](https://docs.microsoft.com/en-US/DeployEdge/microsoft-edge-policies#personalizationreportingenabled)|Allow personalization of ads, search and news by sending browsing history to Microsoft|
|[PinningWizardAllowed](https://docs.microsoft.com/en-US/DeployEdge/microsoft-edge-policies#pinningwizardallowed)|Allow Pin to taskbar wizard|
|[SmartScreenPuaEnabled](https://docs.microsoft.com/en-US/DeployEdge/microsoft-edge-policies#smartscreenpuaenabled)|Configure Microsoft Defender SmartScreen to block potentially unwanted apps|
|[TotalMemoryLimitMb](https://docs.microsoft.com/en-US/DeployEdge/microsoft-edge-policies#totalmemorylimitmb)|Set limit on megabytes of memory a single Microsoft Edge instance can use.|
|[WebAppInstallForceList](https://docs.microsoft.com/en-US/DeployEdge/microsoft-edge-policies#webappinstallforcelist)|Configure list of force-installed Web Apps|
|[WebComponentsV0Enabled](https://docs.microsoft.com/en-US/DeployEdge/microsoft-edge-policies#webcomponentsv0enabled)|Re-enable Web Components v0 API until M84.|
|[WebRtcLocalIpsAllowedUrls](https://docs.microsoft.com/en-US/DeployEdge/microsoft-edge-policies#webrtclocalipsallowedurls)|Manage exposure of local IP addresses by WebRTC|

- 1 deprecated policy

The following table lists the policy that was deprecated.

| Policy name | Caption |
|-------------|---------|
|[NewTabPageCompanyLogo](https://docs.microsoft.com/en-US/DeployEdge/microsoft-edge-policies#newtabpagecompanylogo)|Set new tab page company logo|

### Resolved issues

- Fixed an issue where audio is not working in Citrix environment.
- Fixed an issue where Microsoft Edge and legacy Microsoft Edge side by side experience results in broken legacy links and crashes.

## See also

- [Microsoft Edge Enterprise landing page](https://aka.ms/EdgeEnterprise)
