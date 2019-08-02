---
title: "Create Microsoft Edge user data directory variables"
ms.author: brianalt
author: dan-wesley
manager: srugh
ms.date: 08/02/2019
audience: ITPro
ms.topic: procedural
ms.prod: microsoft-edge
localization_priority: medium
ms.collection: M365-modern-desktop
description: "Learn how to create Microsoft Edge user data directory variables"
---

# Create Microsoft Edge user data directory variables

This article explains how you can create user data directory variables that Microsoft Edge supports.

>[!NOTE]
>This article applies to Microsoft Edge version 77 or later.

## Supported directory variables

The policy for modifying user data directory and other paths supports variables. You can use variables instead of hard-coded paths for Microsoft Edge.

If you don't enable this policy, Microsoft Edge uses default profile path. A user can use the `--user-data-dir` command-line flag to override the default.

>[!TIP]
>To find out what version of Microsoft Edge >you installed, type “edge://version” as search input. The search result is the **About version** page. This page includes **Profile path**, which uses this format: *C:\Users\<Current-User>\AppData\Local\Microsoft\<Edge-Version>\User Data\Default*.

**Example:**

To store your profile data under user local application data on Windows instead of the default location.

Set the [UserDataDir](https://docs.microsoft.com/en-us/DeployEdge/microsoft-edge-policies#userdatadir) policy to **${local_app_data}\Edge\Profile**. On most Windows 10 installations, this resolves to *C:\Users\<Current-User>\AppData\Local\MicrosoftEdge\Profile*.

>[!IMPORTANT]
>Microsoft Edge profiles aren’t backward-compatible. Storing the user profile on a network drive and using it with different versions of Microsoft Edge can trigger crashes and data loss.

### Guidance for using variables for paths

Review the following guidance before using variables for paths.

- All policies that involve paths where Microsoft Edge stores different data are platform dependent. Some of these policies are available only on specific platforms, but others can be used on all platforms.
- To avoid errors caused by applications starting from different locations on different occasions, make sure that paths are absolute.
- Every variable can occur only once in a path. For most of them, this is the only meaningful way to use variables, because they resolve to absolute paths.
- Almost all policies will create the path if it doesn't exist (if possible in the existing circumstances.)
- Using network locations for some policies can lead to unexpected results due to differences in how different versions of Microsoft Edge handle the folder structure.

### Supported path variables

The following path variables are supported.

#### All platforms

**${user_name}** - The user who’s using Microsoft Edge. Example resolution: audreysmall

>[!NOTE]
>Microsoft Edge respects SUIDs (Set owner User ID up on execution).

**${machine_name}** - The machine name, possibly including the domain name. Example resolution:   audreysmall or audrey.ex.contoso.com

#### Windows only

 **${documents}** - The Documents folder for the current user. Example resolution: *C:\Users\Administrator\Documents*

**${local_app_data}** - The Application Data folder for the current user. Example resolution: *C:\Users\Administrator\AppData\Local*

**${roaming_app_data}** - The Roamed Application Data folder for the current user. Example resolution: *C:\Users\Administrator\AppData\Roaming*

 **${profile}** - The home folder for the current user. Example resolution: *C:\Users\Administrator*

**${global_app_data}** - The system-wide Application Data folder. Example resolution: *C:\AppData*

**${program_files}** - The Program Files folder for the current process. This depends on whether it’s a 32-bit or 64-bit process. Example resolution: *C:\Program Files (x86)*

**${windows}** - The Windows folder. Example resolution: *C:\Windows*

**${client_name)** - The name of the client PC connected to an RDP or Citrix session. Example resolution: *C:\edge_profiles\session_${client_name}* resolves to *C:\edge_profiles\session_&lt;ForlocalSessions&gt;* and *C:\edge_profiles\session_&lt;SomePCname&gt;* for remote sessions.

>[!NOTE]
>This variable is empty if it’s used from a local session. If it’s used in a path, prefix it with something that’s guaranteed not to be empty.

**${session_name}** - The name of the active session. Use this to distinguish multiple simultaneously connected remote sessions that are using a single user profile. Example resolution: *WinSta0 for local desktop sessions*

#### MacOS only

**${users}** - The folder where users' profiles are stored. Example resolution: */Users*

**${documents}** - The Documents folder for the current user. Example resolution: */Users/audreysmall/Documents*
