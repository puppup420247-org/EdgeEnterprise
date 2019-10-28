---
title: "Microsoft Edge identity support and configuration"
ms.author: kvice
author: dan-wesley
manager: srugh
ms.date: 10/28/2019
audience: ITPro
ms.topic: conceptual
ms.prod: microsoft-edge
ms.localizationpriority: high
ms.collection: M365-modern-desktop
description: "Microsoft Edge identity support and configuration"
---

# Microsoft Edge identity support and configuration

This article describes how Microsoft Edge uses identity to support features such as sync and single sign-on. Microsoft Edge supports signing in with Active Directory (AD), Azure Active Directory (AAD), and Microsoft accounts (MSA).

> [!NOTE]
> This applies  to Microsoft Edge version 77 or later.

## Overview

When users sign in, they automatically benefit from single sign-on (SSO) when they visit websites that support their logged in account. When signed in, users can choose to sync their browsing data between their devices. Signing in is also needed to use authenticated browser features such as enterprise New tab page, Microsoft Search and Microsoft Information Protection.

## Authentication

To ensure that users are always authenticated and can benefit from authenticated features, they’re automatically signed into Microsoft Edge if they’re signed into Windows.  In addition, users can’t remove their signed profile for their work or school account. This setting can be changed using the [NonRemovableProfileEnabled](https://docs.microsoft.com/DeployEdge/microsoft-edge-policies#nonremovableprofileenabled) policy.

Users can sign into Microsoft Edge with more than one account, add profiles and then sign into each profile using different accounts.

> [!NOTE]
> If users want to browse unauthenticated, they can a profile or browse using the Guest profile.

## Authentication and features

The type of account used sign in determines which authentication and identity-based features are available and supported in Microsoft Edge. The following table summarizes the feature support for each type of account.

### Single Sign-On

Microsoft Edge supports the following approaches to single sign-on.

#### Seamless SSO

Point to SSO docs. No special config needed for Edge.
[Active Directory Seamless Single Sign-On](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-sso)

#### SSO with Primary Refresh Token (PRT)

No config needed
[What is a Primary Refresh Token?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)

#### Windows Integrated Authentication (WIA)

UA string needs to be updated in ADFS
[Configure browsers to use Windows Integrated Authentication (WIA) with AD FS](https://docs.microsoft.com/windows-server/identity/ad-fs/operations/configure-ad-fs-browser-wia)

## See also

- [Microsoft Edge Enterprise landing page](https://www.microsoftedgeinsider.com/enterprise)
- [Microsoft Edge documentation landing page](https://docs.microsoft.com/DeployEdge/)
- [Identity and access management](https://www.microsoft.com/security/technology/identity-access-management)
- [Identity platform](https://developer.microsoft.com/identity)
