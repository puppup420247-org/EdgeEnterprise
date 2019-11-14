---
title: "Allow list for Microsoft Edge endpoints"
ms.author: kvice
author: dan-wesley
manager: srugh
ms.date: 11/12/2019
audience: ITPro
ms.topic: conceptual
ms.prod: microsoft-edge
ms.localizationpriority: high
ms.collection: M365-modern-desktop
description: "Allow list for Microsoft Edge endpoints"
---

# Allow list for Microsoft Edge endpoints

Microsoft Edge requires connectivity to the Internet to support its features. This article identifies the domain URLs that you need to add to the Allow list to ensure communications through firewalls and other security mechanisms.

> [!NOTE]
> This applies  to Microsoft Edge version 77 or later.

## Domain URLs to allow

Allow the following domain URLs for Microsoft Edge.

### Frontend services

- `https://msedge.api.cdp.microsoft.com`
- `https://msedgeextensions.api.cdp.microsoft.com`

### Experimentation and Configuration service

- `https://ecs.skype.com`

### HTTP traffic shaping, downloads, extensions and delivery optimization

- `http://msedge.f.tlu.dl.delivery.mp.microsoft.com` `(Frontend traffic shaping)`

- `http://msedge.f.dl.delivery.mp.microsoft.com` `(Frontend download)`
- `http://msedge.b.tlu.dl.delivery.mp.microsoft.com` `(Backend traffic shaping)`
- `http://msedge.b.dl.delivery.mp.microsoft.com` `(Backend download)`
- `http://msedgeextensions.f.tlu.dl.delivery.mp.microsoft.com` `(Frontend traffic shaping)`
- `http://msedgeextensions.f.dl.delivery.mp.microsoft.com` `(Frontend download)`
- `http://msedgeextensions.b.tlu.dl.delivery.mp.microsoft.com` `(Backend traffic shaping)`
- `http://msedgeextensions.b.dl.delivery.mp.microsoft.com` `(Backend download)`

- `http://dl.delivery.mp.microsoft.com` `(Delivery optimization)`

### HTTPS traffic shaping, downloads, extensions and delivery optimization

- `https://msedge.sf.tlu.dl.delivery.mp.microsoft.com` `(Frontend traffic shaping)`
- `https://msedge.sf.dl.delivery.mp.microsoft.com` `(Frontend download)`
- `https://msedge.sb.tlu.dl.delivery.mp.microsoft.com` `(Backend traffic shaping)`
- `https://msedge.sb.dl.delivery.mp.microsoft.com` `(Backend download)`

- `https://msedgeextensions.sf.tlu.dl.delivery.mp.microsoft.com` `(Frontend traffic shaping)`
- `https://msedgeextensions.sf.dl.delivery.mp.microsoft.com` `(Frontend download)`
- `https://msedgeextensions.sb.tlu.dl.delivery.mp.microsoft.com` `(Backend traffic shaping)`
- `https://msedgeextensions.sb.dl.delivery.mp.microsoft.com` `(Backend download)`

- `https://dl.delivery.mp.microsoft.com` `(Delivery optimization)`

> [!TIP]
> To simplify the allow list for HTTP and HTTPS downloads you can use this endpoint:  `*.dl.delivery.mp.microsoft.com`.

### Optionally for delivery optimization

- Client to Service communication: `*.do.dsp.mp.microsoft.com` (HTTP Port 80, HTTPS Port 443)
- Client to Client communication: Port 7680 should be open for inbound traffic

For more information about delivery optimization, see [Delivery Optimization for Windows 10 updates](https://aka.ms/waas-do).

## See also

- [Microsoft Edge Enterprise landing page](https://www.microsoftedgeinsider.com/enterprise)
- [Microsoft Edge documentation landing page](https://docs.microsoft.com/DeployEdge/)
- [Manage connection endpoints for Windows 10 Enterprise, version 1903](https://docs.microsoft.com/windows/privacy/manage-windows-1903-endpoints)
