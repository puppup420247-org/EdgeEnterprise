---
title: "Microsoft Edge Release Notes Stable Channel Version 79"
ms.author: kvice
author: dan-wesley
manager: laurawi
ms.date: 01/15/2020
audience: ITPro
ms.topic: conceptual
ms.prod: microsoft-edge
ms.localizationpriority: high
ms.collection: M365-modern-desktop
description: "Microsoft Edge Release Notes Stable Channel Version 79"
---

# Microsoft Edge Release Notes Stable Channel Version 79

These release notes provide information about new features and non-security updates that are included in the Microsoft Edge Stable Channel Version 79.

## Features (first release)

- Internet Explorer mode
- Enterprise NTP
- SmartScreen
- PDF reader
- Offline installers
- Enterprise-grade PDF support
- Sign in, sync and multiple profiles
- 200+ browser and update policies
- Conditional Access
- Application Guard
- Microsoft Search in Bing
- Microsoft Edge DevTools
- Immersive reader
- Favorites button
- Extensions
- Guest mode
- Sync (favorites, passwords, settings, form fill)
- 4k streaming (Win10 only)
- Dolby audio & HDR (Win10 only)
- Video streaming battery claim (Win10 only)

## Resolved issues

**Internet Explorer mode:**

- Fixed an issue where switching between Internet Explorer mode and Microsoft Edge mode leaves webpages at the wrong zoom level on certain devices. 

- Fixed an issue where opening the downloads page on an Internet Explorer mode sometimes doesn’t open it in the foreground. 

- Fixed an issue where using the keyboard shortcut to open the downloads page on an Internet Explorer mode opens Microsoft Edge’s downloads, not IE’s. 

- Fixed an issue where Internet Explorer mode sometimes are zoomed improperly when they load. 

**Application Guard:**  

- Disabled hardware acceleration in Application Guard windows to prevent them from hanging on certain machines. 

- Fixed an issue where files that should be downloaded in Application Guard windows aren’t. 

- Fixed an issue where Windows Firewall prompts appear inside Application Guard windows. 

- Fixed an issue where Application Guard windows fail to navigate and show "This page is having a problem". 

- Fixed an issue where Application Guard windows don’t use dark theme even though the rest of the browser does. 

- Fixed an issue where Application Guard windows don’t have their tabs restored when Microsoft Edge is restarted. 

- Fixed an issue where Application Guard windows unexpectedly open up when the browser is launched. 

- Fixed some issues with Application Guard windows not  opening successfully. 

**Sign in and sync:** 

- Fixed some issues where enabling sync settings sometimes crashes the browser. 

- Fixed an issue where Sync was not working and showed an error next to the profile button on the toolbar. 

- Fixed an issue where users with multiple profiles see a generic icon instead of their profile picture on the Task Bar shortcut. 

- Fixed an issue where logging into the browser fails because the Sign In button isn’t functional. 

- Fixed an issue where sync doesn’t work, and users unexpectedly had to sign into the browser again in order to restore sync. 

- Fixed an issue where syncing doesn’t work after a user signs into the browser and tries to customize which types of data to sync. 

- Fixed an issue where the Sync page in Settings briefly shows incorrectly after confirming the settings. 

- Fixed an issue where "Your organization has turned off sync" messages appear when they shouldn’t be. 

- Fixed an issue where users signed into the browser with a personal Microsoft account are unable to sync favorites and other content. 

- Fixed an issue where the various sync toggles sometimes don’t work after signing in with a work or school account. 

- Fixed an issue where syncing is stuck in the "Setting up your sync…" state. 

- Fixed an issue where an extra "Work" browser profile gets automatically created for some users (note that this may not remove the extra profile; a future fix will ensure that.) 

- Fixed an issue where the button to sign out of the browser is sometimes missing from Settings. 

- Fixed some sign-in errors that occur when signing into the browser with a work or school account. 

- Fixed an issue where the warning about closing the browser while there’s an ongoing download never appears again after it’s dismissed the first time. 

- Fixed an issue where it’s possible to sign into a work or school account using the wrong type of email. 

- Fixed an issue where Single Sign-On signs users into the wrong account if they sign into the browser with a different work or school account than the one they’re currently signed into Windows with. 

- Fixed an issue where users with multiple accounts lose their account pictures on Taskbar shortcuts. 

- Fixed an issue where the user’s name when signed into the browser has "Profile 1" appended to it. 

- Fixed an issue where the first run experience greets users as "Profile 1" instead of their name. 

- Fixed an issue where signing into the browser with an account that has no picture doesn’t properly set the browser’s profile picture to the default avatar if a profile picture was previously set for the profile. 

- Fixed an issue where profile pictures sometimes don’t appear in Settings. 

- Fixed an issue where mobile favorites that are imported from another browser aren’t placed in the correct folder. 

- Fixed a browser crash when importing data from another browser.

**MAC:** 

- Fixed an issue where the Mac Touch Bar sometimes doesn’t show the proper content. 

- Fixed an issue on Mac where clicking in menus sometimes doesn’t work. 

- Fixed an issue where zooming doesn’t work in Reading View on Mac. 

- Fixed an issue where the "Continue running background apps when Microsoft Edge is closed" setting is missing on Mac. 

- Fixed an issue on Mac where syncing for work or school accounts doesn’t work. 

- Fixed an issue where Microsoft Edge on Mac crashes when it checks for updates. 

- Fixed an issue where clicking on the prompt to restart Microsoft Edge to apply an update causes a hang on Mac. 

**F12 Developer Tools:** 

- Fixed an issue where the F12 Dev Tools on Mac sometimes doesn’t use the proper theme. 

- Fixed an issue where the F12 Dev Tools sometimes don’t use the proper theme on Mac. 

- Fixed an issue where corrupted characters appeared in the F12 Dev Tools. 

- Fixed an issue where the F12 Dev Tools feedback smiley face doesn’t render properly in light theme. 

- Fixed an issue where two "Initiator" tabs are visible in the F12 Dev Tools Network pane. 

- Fixed an issue where some context menu items in the F12 Dev Tools appear twice. 

- Fixed an issue where some UI overlaps in the F12 Dev Tools. 

- Fixed an issue where the Settings page constantly shows "looking for updates" without ever completing. 

**SmartScreen:**  

- Fixed an issue where the Delete button does not appear next to downloads that have been blocked by SmartScreen. 

- Fixed an issue where the warning not to close the browser because a download is in progress appears even though the user isn’t downloading anything. 

- Fixed an issue where websites that are blocked by SmartScreen aren’t removed from history. 

- Fixed an issue where the browser has high CPU usage when idle. 

- Fixed an issue where downloads blocked by SmartScreen don’t have the button to delete them straight from the Downloads shelf. 

**PDF reader:**  

- Fixed a webpage crash when viewing PDF documents. 

- Fixed an issue where the PDF toolbar is still visible when it shouldn’t be. 

- Fixed an issue where text selection in PDFs selects an extra character. 

- Fixed an issue where the arrow keys sometimes don’t work in PDF documents. 

- Fixed an issue where Netflix shows error D7354 when trying to play a video. 

- Fixed an issue where attempting to print a webpage while it’s in Reading View only prints a single paper’s worth of content instead of the entire webpage. 

**Favorites button:**  

- Fixed an issue where adding a new folder to Favorites from the Favorites management page isn’t possible because the Save button is disabled. 

- Added a right-click option to sort individual favorites folders by name from the Favorites management page. 

- Improved the reliability of history and favorites items appearing in the address bar suggestions dropdown. 

**Other:**

- Fixed an issue where certain Read Aloud voices don’t work properly. 

- Fixed an issue where searches from the address bar are always in English despite the user’s language being set to some other language. 

- Fixed an issue where Top Sites on the new tab page disappear or are reset after upgrading to a new version of Microsoft Edge. 

- Fixed an issue where translating a page into a different language and then back into its original language shows an error instead of performing the second translation. 

- Fixed an issue where certain webpage controls like the calendar picker aren’t appearing. 

- Fixed an issue where hitting the ESC key on the warning dialog that appears when attempting to close the browser while a download is in progress closes the browser instead of just dismissing the dialog. 

- Fixed an issue where autofill settings are unexpectedly turned off by default for some users. 

- Fixed an issue where cookies are unexpectedly disabled on new installations. 

- Fixed an issue where certain icons are inappropriately mirrored in right-to-left language installations. 

- Fixed an issue where checking for Microsoft Edge updates results in the following error: “We couldn't create that component (error code 3: 0x80080005 -- system level)”. 

- Fixed an issue where users can’t click on certain browser UI while the print dialog is open. 

- Fixed an issue where importing settings from Chrome causes webpage text to be smaller than normal. 

- Fixed an issue where Reading View doesn’t properly support right-to-left languages. 

- Fixed an issue where some buttons appeared circular when they’re hovered over instead of square/rectangular. 

- Fixed an issue where tooltips sometimes don’t draw their entire border properly. 

- Fixed an issue where changing which content is shown on the new tab page sometimes causes the wrong favicon to be shown on the tab. 

- Fixed an issue where the number of InPrivate windows currently open isn’t displayed next to the InPrivate indicator in the toolbar. 

- Fixed an issue where the search engine imported from the existing version of Microsoft Edge isn’t set as the default search engine after import. 

- Fixed an issue where the feedback dialog window control buttons appear to be blurry. 

- Fixed an issue where the first run experience sometimes appears on top of web page content instead of on a new tab. 

- Fixed an issue where Read Aloud would sometimes stop when reading long words. 

- Fixed an issue where tooltips don't appear when hovering over links, UI, etc. 

- Fixed an issue where the option to open a new tab from the tab band’s context menu appears twice. 

- Fixed an issue where windows sometimes have a 1px colored line on top of them. 

- Fixed an issue where watching certain videos in full screen causes playback to freeze. 

- Fixed an issue where trying to import data from the same browser multiple times fails on the subsequent attempts. 

- Fixed an issue where certain settings aren’t imported correctly from the previous version of Microsoft Edge. 

- Fixed an issue where the icons for the buttons on the toolbar like the back button or the … menu aren’t centered in the button. 

- Fixed an issue where a new taskbar shortcut is created when Microsoft Edge is updated to a newer version even though there’s already an existing shortcut. 

- Fixed an issue where the X button to close a tab is incorrectly placed when tab sizes are sufficiently small. 

- Fixed an issue where the X button to close a tab sometimes stays highlighted even when it’s not being interacted with. 

- Fixed an issue where some sections of the edge://accessibility page are missing. 

- Fixed an issue where websites installed as Apps don’t properly respond to changes in the browser’s theme. 

- Fixed an issue where websites installed as Apps sometimes aren’t removed from every list in the browser when they’re uninstalled. 

- Fixed an issue where feedback screenshots that are cropped become much lower quality. 

- Fixed an issue where the “Save and Include” button on the feedback diagnostic data windows isn’t visible. 

- Fixed an issue where the retry button on deleted downloads appears to be disabled. 

- Fixed an issue where Flash settings are sometimes not properly displayed. 

- Fixed an issue where context menus on the Settings page sometimes don’t dismiss properly. 

- Fixed an issue where the Delete Browsing Data popup is sometimes missing some of its contents. 

- Fixed an issue where the link to the Extensions store was missing on the Extensions page when no Extensions are installed. 

- Fixed an issue where watching DRM video like Netflix causes some devices to freeze. 

- Fixed an issue where the translation popup didn’t have a button to close it. 

- Fixed some issues when adding or deleting words in the spellcheck dictionary. 

- Fixed an issue where the new tab button is invisible on Windows 7 if the Aero theme is used. 

- Fixed an issue where webpages sometimes crash when typing in passwords. 

- Temporarily disabled Renderer Code Integrity by default to prevent situations where it causes all tabs to crash upon loading. 

- Fixed an issue where the browser sometimes crashes after completing the first run experience. 

- Fixed an issue where typing in the address bar sometimes causes the browser to crash. 

- Fixed an issue where using ctrl+F to find something on a webpage while certain things on the page are highlighted leads to a crash. 

- Fixed an issue where importing data from another browser can sometimes cause the tab to crash. 

## See also

- [Microsoft Edge Enterprise landing page](https://aka.ms/EdgeEnterprise)
