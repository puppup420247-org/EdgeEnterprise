---
title: "Microsoft Edge Release Notes Beta Channel Version 80"
ms.author: kvice
author: dan-wesley
manager: laurawi
ms.date: 01/15/2020
audience: ITPro
ms.topic: conceptual
ms.prod: microsoft-edge
ms.localizationpriority: high
ms.collection: M365-modern-desktop
description: "Microsoft Edge Release Notes Beta Channel Version 80"
---

# Microsoft Edge Release Notes Beta Channel Version 80

These release notes provide information about new features and non-security updates that are included in the Microsoft Edge Beta Channel Version 80.

## Feature updates

- Added an option to Reading View to increase text spacing. 
- Added a prompt to verify work or school accounts that are automatically added to Microsoft Edge but aren’t enabled for sync so that users are aware sync isn’t enabled. 
- Added support for Dolby Vision playback. 
- Enabled users of Windows Mixed Reality to view 360° videos on VR headsets. 
- Added support for erasing ink using the eraser side of a pen. 
- Added support for using the arrow keys and spacebar to draw on feedback screenshots in editor mode. 
- Added SmartScreen protection from downloading potentially unwanted apps. 
- Added dark theme support to certain UI that appears when the browser is managed by Group Policy. 
- Added dark theme support to the local new tab page that is shown when the device isn’t connected to the internet. 
- Added the ability for websites installed as apps to be restored when a browser session is restored after update, crash, etc. 
- Added support for periods in single-word intranet URLs. 
- Updated Adobe Flash to version 32.0.0.303. 
- Improved the reliability of screenshots so they stop appearing all black when submitting feedback. 

## Resolved issues

**Application Guard:** 

- Fixed an issue where Application Guard windows re-open when the browser is started even when the startup settings aren’t set to restore the previous session. 

- Fixed an issue where Application Guard windows sometimes crash upon startup. 

- Fixed an issue where navigation fails in Application Guard windows. 

- Fixed an issue where Application Guard windows open when the browser is launched even though they shouldn’t. 

- Fixed an issue where enabling Application Guard sometimes causes downloads to be blocked in non-Application Guard windows. 

- Fixed an issue where Application Guard windows hang upon startup. 

- Fixed an issue where all Microsoft Edge windows open completely white with no UI, but disabling Application Guard mitigates the issue. 

**Sign in and sync:** 

- Fixed a crash that occurs when favorites sync is enabled. 

- Fixed an issue where Microsoft Edge crashes shortly after launch for some users if sync is enabled. 

- Reduced the number of times sync errors result in a prompt for user interaction. 

- Fixed an issue where new data types are available to sync, but they aren’t enabled by default. 

- Fixed an issue where the sync customization page during the first run experience doesn’t properly enable sync for the selected items. 

- Fixed an issue where enabling sync during the first run experience doesn’t enable sync on certain data types. 

- Updated the sync Settings page to show more types of data that will be available in the future, but with the switches disabled until that data type is available. 

- Fixed an issue where syncing gets stuck in the "Setting up sync" state on browser startup. 

- Fixed an issue where sync sometimes fails after restoring tabs after a browser crash. 

- Reduced the number of times a user needs to sign out and sign back into the browser in order to fix sync. 

- Fixed an issue where navigating to the Sync Settings page always triggers a dialog to enable sync. 

- Fixed an issue where sync can’t be turned off while it’s in the "setting up" state. 

- Fixed an issue where deleted or edited favorites aren’t synced properly, causing the edit to be undone when it syncs back down. 

- Fixed an issue where typing passwords into password fields sometimes causes a tab crash. 

- Fixed an issue where favorites aren’t syncing properly between machines. 

- Fixed an issue where selecting context menu items on certain favorites entries causes a browser crash. 

- Fixed an issue where importing favorites from a file sometimes causes any favorites on the Favorites Bar not to be imported directly onto the Favorites Bar. 

- Fixed an issue where the profile Settings page has no way for the user to fix an issue with their browser sign-in when one is needed. 

- Fixed an issue where users in certain countries who are not signed into Windows with a work or school account still are not able to remove "Work" profiles that were automatically added to Microsoft Edge even after a previous fix for this issue was shipped. 

- Fixed an issue for users of work and school accounts where websites that try and fail to use the browser profile’s credentials to log in don’t subsequently allow the user to fall back and try the user’s OS credentials. 

- Fixed an issue where users that are signed into Windows with a work or school account are unable to remove the "Work" account that is automatically added to Microsoft Edge. 

**SmartScreen:**  

- Fixed a SmartScreen crash when downloading certain items. 

- Fixed an issue where closing tabs that contain websites that are blocked by SmartScreen sometimes causes a browser crash. 

**MAC:** 

- Fixed an issue where feedback screenshots sometimes don’t work properly on Mac. 

- Fixed an issue where the keyboard shortcut for saving a PDF doesn’t work on Mac. 

- Fixed an issue where the Restart button is always visible on the language Settings page on Mac. 

- Fixed some issues with the Mac Touch Bar when working with multiple tabs at the same time. 

- Fixed an issue where some UI images on Mac have black backgrounds. 

- Fixed an issue where using the Mac Touch Bar to switch tabs sometimes doesn’t work properly if the tabs are playing video. 

- Fixed an issue where zoom is triggering in Reading View on Mac when it shouldn’t be. 

- Fixed an issue where Microsoft Edge on Mac hangs when a user clicks the Restart button on the Settings page to install an update. 

- Fixed an issue on Mac where feedback screenshots can’t be included when submitting feedback. 

- Fixed an issue where Microsoft Edge on Mac fails to install updates automatically. 

**PDF reader:**  

- Fixed an issue where saving a PDF that has been written on with ink sometimes results in a corrupted file. 

**Other:**  

- Fixed an issue where navigating to certain webpages with videos causes the tab to crash. 

- Fixed an issue where highlighting text on a webpage sometimes causes a browser crash. 

- Fixed an issue where the search engine can’t be edited because the Save button doesn’t work. 

- Fixed an issue where the current display language can be removed from Microsoft Edge even though it shouldn’t be. 

- Fixed an issue where Microsoft Edge installations on Azure Active Directory domain-joined machines get signed into the wrong account on first run. 

- Fixed an issue where some webpages aren’t able to be translated, and instead show an error saying that the source language and target language are the same. 

- Fixed an issue where Learn More links clicked during the First Run Experience open in tabs hidden behind the FRE instead of in a dialog above it. 

- Fixed an issue where desktop notifications are broken on Windows Insider builds. 

- Fixed an issue where Microsoft Edge sometimes fails to automatically update on Windows Insider builds. 

- Fixed an issue where uninstalling and reinstalling Microsoft Edge sometimes results in it no longer being able to launch on Windows Insider builds. 

- Updated the toolbar Feedback icon to be consistent with other Windows feedback icons. 

- Changed the color of the title bar of installed websites and PWAs to be the dominant color of the site’s favicon. 

- Fixed an issue where manually importing data from Chrome isn’t possible if there are too many Chrome browser profiles to fit in the dialog. 

- Fixed an issue where the UI and web content is sometimes seen doubled and shrunken on high DPI displays.   

- Fixed an issue where the Find bar sometimes disappears when the browser loses focus. 

- Fixed an issue where the 1px border on top of the window is missing. 

- Fixed an issue where the prompt to autofill a credit card has two checkboxes to save the card locally. 

- Fixed an issue where the browser UI sometimes appears to hang or turn all black, but it still responds to input and can be fixed by killing the GPU process. 

- Fixed an issue where using Read Aloud sometimes crashes the tab. 

- Fixed an issue where the font dropdown in Settings doesn’t work. 

- Fixed an issue where clicking on the Feedback button crashes the browser. 

- Fixed an issue where Netflix playback fails on certain machines. 

- Fixed an issue where Netflix playback fails with error D7356. 

- Fixed an issue where Netflix playback fails for certain videos with error D7381. 

- Fixed an issue where certain protected videos like from Netflix don’t work. 

- Fixed some issues where videos protected by DRM, such as on Netflix, don’t play. 

- Fixed an issue where typing the address of a website that’s already been visited doesn’t properly autocomplete the name of the website in the address bar dropdown. 

- Fixed an issue where some of the privacy links in the First Run Experience open in a new tab in the background instead of in a popup. 

- Fixed an issue where uninstalling PWAs or installed websites doesn’t also prompt to delete browsing data for that site. 

- Fixed an issue where searching from the address bar sometimes crashes the browser. 

- Fixed an issue where processes that grow too large and stop working aren’t automatically fixed. 

- Temporarily disabled one form of DRM support on ARM64, which may impact the ability to play certain DRM-protected videos. 

- Fixed an issue where windows that are minimized when the browser is restarted aren’t restored properly. 

- Fixed an issue where the space bar or enter key doesn’t work when typing in the address bar. 

- Fixed an issue where the Windows Hello prompt to log into a website with the user’s OS credentials sometimes shows in an infinite loop. 

- Fixed an issue where PWAs installed for one user on a machine sometimes can’t be launched by other users on the machine. 

- Fixed an issue where link context menus don’t show all the options if they’re opened via the keyboard instead of the mouse. 

- Fixed an issue where some websites that are pinned to the Task Bar launch new tabs instead of activating existing tabs when tabs with those websites already exist. 

- Fixed an issue where open tabs aren’t properly imported from Chrome. 

- Fixed an issue where the wrong icon appears on web notifications. 

- Fixed an issue where Microsoft Edge crashes on close, causing the Restore Tabs prompt to unexpectedly appear at startup. 

- Fixed an issue where only the first Microsoft Edge window opened in a session is all white with no UI. 

- Fixed an issue where pinning a website to the Taskbar fails. 

- Fixed an issue where extensions that are installed from the Chrome Web Store are not getting automatically updated. 

- Fixed an issue where the Taskbar icon for Microsoft Edge isn’t updated to the new icon for some users. 

- Fixed an issue where two Microsoft Edge icons sometimes appear on the Taskbar after a Microsoft Edge update. 

- Fixed an issue where the first run experience appears on every new tab for some users. 

- Fixed an issue where the password save prompt unexpectedly appears when filling out credit card info on certain websites. 

- Fixed an issue where the … menu appears truncated. 

- Fixed an issue where Microsoft Edge doesn’t interact properly with other applications that try to show dialogs in the foreground. 

- Fixed an issue where there are two Passwords toggles and no Favorites toggle on the Settings page. 

- Fixed an issue where importing browser data from other Chrome profiles than the default one shows an incorrect profile name during the import process. 

- Fixed an issue where the setting to show the favorites bar is not imported properly from Chrome. 

- Fixed an issue where right-clicking the back button crashes the browser. 

- Fixed an issue where certain DRM-protected videos don’t play. 

- Fixed an issue where Single Sign-On stops working and users unexpectedly see a username/password prompt to log into websites. 

- Fixed an issue where two Microsoft Edge shortcuts are sometimes on the Taskbar after an update. 

- Fixed an issue where Work profiles that were erroneously added to the browser were unremovable. 

- Fixed an issue where the first run experience sometimes runs every time the browser is opened. 

- Fixed an issue where open tabs sometimes aren’t properly imported from Chrome. 

- Fixed an issue where extensions aren’t sorted by name on the Extensions management page. 

- Fixed an issue where Microsoft Edge shortcuts were created in the wrong location in the Start menu. 

## See also

- [Microsoft Edge Enterprise landing page](https://aka.ms/EdgeEnterprise)
