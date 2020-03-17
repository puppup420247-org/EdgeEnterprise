---
title: "Microsoft Edge and mixed content downloads"
ms.author: kele
author: dan-wesley
manager: srugh
ms.date: 03/17/2020
audience: ITPro
ms.topic: procedural
ms.prod: microsoft-edge
ms.localizationpriority: high
ms.collection: M365-modern-desktop
description: "Microsoft Edge and mixed content downloads"
---

# Learn about Microsoft Edge and mixed content downloads

This article explains mixed content downloads and how Microsoft Edge handles them.

>[!NOTE]
>This article applies to Microsoft Edge version 77 or later.

## What are mixed content downloads?

Mixed content downloads happen when a download was initiated from an HTML page that was loaded over a secure HTTPS connection, but one of the following scenarios exist:

- One or more of the download locations redirects was loaded over an insecure HTTP connection.
- The final download location was loaded over an insecure HTTP connection.

This is called mixed content downloads because both HTTP and HTTPS content is involved in reaching the final download destination, and the initial download request was activated from secure HTTPS. Modern browsers display warnings about this type of content to indicate to the user that this download may be transferred insecurely even though the original page accessed was secure.

## See also

- [Microsoft Edge Enterprise landing page](https://aka.ms/EdgeEnterprise)

> [!NOTE]
> Portions of this page are modifications based on work created and shared by Chromium.org and used according to terms 
  described in the [Creative Commons Attribution 4.0 International License](http://creativecommons.org/licenses/by/4.0/). The original page can be found [here](https://developers.google.com/web/fundamentals/security/prevent-mixed-content/what-is-mixed-content).
  
<a rel="license" href="http://creativecommons.org/licenses/by/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by/4.0/">Creative Commons Attribution 4.0 International License</a>.