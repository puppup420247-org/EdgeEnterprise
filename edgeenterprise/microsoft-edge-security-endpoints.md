---
title: "Microsoft Edge URLs and IP address ranges"
ms.author: kvice
author: dan-wesley
manager: srugh
ms.date: 10/25/2019
audience: ITPro
ms.topic: conceptual
ms.prod: microsoft-edge
ms.localizationpriority: high
ms.collection: M365-modern-desktop
description: "Microsoft Edge URLs and IP address ranges"
---

# Microsoft Edge URLs and IP address ranges

Microsoft Edge requires connectivity to the Internet.

> [!NOTE]
> This applies  to Microsoft Edge version 77 or later.

## Overview

The following endpoint data below lists requirements for connectivity from a user’s machine to Microsoft Edge. It doesn't include network connections from Microsoft into a customer network, sometimes called hybrid or inbound network connections.

Data columns shown are:

- **ID**: The ID number of the row, also known as an endpoint set. This ID is the same as is returned by the web service for the endpoint set.
- **Category**: Shows whether the endpoint set is categorized as “Optimize”, “Allow”, or “Default”. You can read about these categories and guidance for management of them at <http://aka.ms/pnc>. This column also lists which endpoint sets are required to have network connectivity. For endpoint sets which are not required to have network connectivity, we provide notes in this field to indicate what functionality would be missing if the endpoint set is blocked. If you are excluding an entire service area, the endpoint sets listed as required do not require connectivity.
- **ER**: This is **Yes** if the endpoint set is supported over Azure ExpressRoute with Office 365 route prefixes. The BGP community that includes the route prefixes shown aligns with the service area listed. When ER is **No**, this means that ExpressRoute is not supported for this endpoint set. However, it should not be assumed that no routes are advertised for an endpoint set where ER is **No**.
- **Addresses**: Lists the FQDNs or wildcard domain names and IP Address ranges for the endpoint set. Note that an IP Address range is in CIDR format and may include many individual IP Addresses in the specified network.
- **Ports**: Lists the TCP or UDP ports that are combined with the Addresses to form the network endpoint. You may notice some duplication in IP Address ranges where there are different ports listed.

## Microsoft Edge

| ID | Category                  | ER  | Addresses                                                     | Ports        |
|----|---------------------------|-----|---------------------------------------------------------------|--------------|
| 1  | Optimize Required         | Yes | `Outlook.office.com<br>13.70.151.216/32, 13.71.127.197/32, 13.72.245.115/32`                                        | TCP: 443,80  |
| 2  | Allow Required            | Yes | `smtp.office365.com<br>13.70.151.216/32, 13.71.127.197/32, 13.72.245.115/32`                                        | TCP: 587     |
|    |                           |     |                                                               |              |

## See also

- [Microsoft Edge Enterprise landing page](https://www.microsoftedgeinsider.com/enterprise)
- [Microsoft Edge documentation landing page](https://docs.microsoft.com/DeployEdge/)