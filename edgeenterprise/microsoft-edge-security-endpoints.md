---
title: "Allow list for Microsoft Edge endpoints"
ms.author: kvice
author: dan-wesley
manager: srugh
ms.date: 10/30/2019
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

### URLs to support frontend service

- `https://msedge.api.cdp.microsoft.com`
- `https://msedgeextensions.api.cdp.microsoft.com`

### URLs to support the Configuration and Experimentation service

- `https://ecs.skype.com`

### URLs to support HTTP downloads

- `http://msedge.f.tlu.dl.delivery.mp.microsoft.com`
- `http://msedge.f.dl.delivery.mp.microsoft.com`
- `http://msedge.b.tlu.dl.delivery.mp.microsoft.com`
- `http://msedge.b.dl.delivery.mp.microsoft.com`
- `http://msedgeextensions.f.tlu.dl.delivery.mp.microsoft.com`
- `http://msedgeextensions.f.dl.delivery.mp.microsoft.com`
- `http://msedgeextensions.b.tlu.dl.delivery.mp.microsoft.com`
- `http://msedgeextensions.b.dl.delivery.mp.microsoft.com`

### URLs to support HTTPS downloads

- `https://msedge.sf.tlu.dl.delivery.mp.microsoft.com`
- `https://msedge.sf.dl.delivery.mp.microsoft.com`
- `https://msedge.sb.tlu.dl.delivery.mp.microsoft.com`
- `https://msedge.sb.dl.delivery.mp.microsoft.com`
- `https://msedgeextensions.sf.tlu.dl.delivery.mp.microsoft.com`
- `https://msedgeextensions.sf.dl.delivery.mp.microsoft.com`
- `https://msedgeextensions.sb.tlu.dl.delivery.mp.microsoft.com`
- `https://msedgeextensions.sb.dl.delivery.mp.microsoft.com`

> [!NOTE]
> To simplify the allow list for HTTP and HTTPS downloads you can use this URL:  `*.dl.delivery.mp.microsoft.com`.

### Optionally for delivery optimization

- Client to Service communication: `*.do.dsp.mp.microsoft.com` (HTTP Port 80, HTTPS Port 443)
- Client to Client communication: Port 7680 should be open for inbound traffic

For more information about delivery optimization, see [Delivery Optimization for Windows 10 updates](https://aka.ms/waas-do).

## See also

- [Microsoft Edge Enterprise landing page](https://www.microsoftedgeinsider.com/enterprise)
- [Microsoft Edge documentation landing page](https://docs.microsoft.com/DeployEdge/)
