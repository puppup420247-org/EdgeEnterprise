---
title: "Microsoft Edge Roadmap"
ms.author: kvice
author: dan-wesley
manager: laurawi
ms.date: 01/15/2020
audience: ITPro
ms.topic: conceptual
ms.prod: microsoft-edge
ms.localizationpriority: high
ms.collection: M365-modern-desktop
description: "Microsoft Edge Roadmap"
---

# Microsoft Edge Roadmap

This article describes the roadmap for Microsoft Edge.

## Roadmap

| Description | Status | Tags | Release |
|--|--|--|--|
| Cookies default to SameSite=Lax<br>Description details:<br>"SameSite" is a reasonably robust defense against some classes of cross-site request forgery (CSRF) attacks, but developers currently need to opt-into its protections by specifying a SameSite attribute. In other words, developers are vulnerable to CSRF attacks by default. This change would allow developers to be protected by default, while allowing sites that require state in cross-site requests to opt-in to the status quo’s less-secure model. In addition, forcing sites to opt-in to SameSite=None gives the user agent the ability to provide users more transparency and control over tracking.<br>For [more information](https://docs.microsoft.com/microsoft-edge/web-platform/site-impacting-changes) | Experimentation<br> Or<br> In development | Microsoft Edge | Canary/Dev Channel M80 |
| Referrer Policy: Default to strict-origin-when-cross-origin<br>Web developers may specify a referrer policy on their documents, which impacts the Referer header sent on outgoing requests and navigations. When no such policy is specified, Microsoft Edge will now use strict-origin-when-cross-origin as the default policy, instead of no-referrer-when-downgrade. On cross-origin requests made from documents without a specified referrer policy, this reduces the Referer header to the initiating origin.<br>By default in Microsoft Edge, the HTTP `referer` header provides the full URL of the initiating document alongside every navigation and subresource request (except on requests from HTTPS to non-HTTPS origins). In the wild, a substantial majority of links and images follow this default. Referrers silently reveal users’ browsing habits, identities (for instance, when websites place user IDs in URLs), and credentials (via capability-granting URLs).<br>While developers have the option of setting a referrer policy to limit the amount of information that is sent, this requires an explicit opt-in effort, leading to low adoption.<br>For [more information](https://docs.microsoft.com/microsoft-edge/web-platform/site-impacting-changes)  | Experimentation<br> Or<br> In development      | Microsoft Edge   | Canary/Dev Channel M79  |
| Disallow synchronous XmlHttpRequest in page dismissal<br> Description details:<br> Sending of synchronous XmlHttpRequests during unload of a webpage will be removed. This change will improve browser performance and reliability, but may impact web applications that have not yet been updated to use more modern web APIs including sendBeacon and fetch.<br>Group Policy to disable this change and permit synchronous XHR during page dismissal will be available until Edge 88.<br> The current settings is behind a flag. Until enabled-by-default in Edge 82, this change can be previewed by setting edge://flags/#allow-sync-xhr-in-page-dismissal to Disabled.<br>For [more information](https://docs.microsoft.com/microsoft-edge/web-platform/site-impacting-changes) | In development      |  Microsoft Edge, SAP    | Edge 82       |

## See also

- [Microsoft Edge Enterprise landing page](https://aka.ms/EdgeEnterprise)
