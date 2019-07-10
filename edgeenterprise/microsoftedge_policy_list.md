--- 
title: "Microsoft Edge Browser Policy Documentation" 
ms.author: stmoody 
author: kelleyvice-MSFT
manager: laurawi
ms.date: 7/10/2019
audience: ITPro 
ms.topic: reference
ms.prod: microsoft-edge
localization_priority: high
ms.collection: 
ms.custom: 
description: "Windows and Mac documentation for all policies supported by the Microsoft Edge Browser" 
---

# Edge Policy Documentation
|Policy Name|Caption|
|-|-|
|Content settings||
|[AutoSelectCertificateForUrls](#automatically-select-client-certificates-for-these-sites-autoselectcertificateforurls)|Automatically select client certificates for these sites|
|[CookiesAllowedForUrls](#allow-cookies-on-specific-sites-cookiesallowedforurls)|Allow cookies on specific sites|
|[CookiesBlockedForUrls](#block-cookies-on-specific-sites-cookiesblockedforurls)|Block cookies on specific sites|
|[CookiesSessionOnlyForUrls](#limit-cookies-from-specific-websites-to-the-current-session-cookiessessiononlyforurls)|Limit cookies from specific websites to the current session|
|[DefaultCookiesSetting](#configure-cookies-defaultcookiessetting)|Configure cookies|
|[DefaultGeolocationSetting](#default-geolocation-setting-defaultgeolocationsetting)|Default geolocation setting|
|[DefaultImagesSetting](#default-images-setting-defaultimagessetting)|Default images setting|
|[DefaultJavaScriptSetting](#default-javascript-setting-defaultjavascriptsetting)|Default JavaScript setting|
|[DefaultNotificationsSetting](#default-notification-setting-defaultnotificationssetting)|Default notification setting|
|[DefaultPluginsSetting](#default-adobe-flash-setting-defaultpluginssetting)|Default Adobe Flash setting|
|[DefaultPopupsSetting](#default-pop-up-window-setting-defaultpopupssetting)|Default pop-up window setting|
|[DefaultWebBluetoothGuardSetting](#control-use-of-the-web-bluetooth-api-defaultwebbluetoothguardsetting)|Control use of the Web Bluetooth API|
|[DefaultWebUsbGuardSetting](#control-use-of-the-webusb-api-defaultwebusbguardsetting)|Control use of the WebUSB API|
|[ImagesAllowedForUrls](#allow-images-on-these-sites-imagesallowedforurls)|Allow images on these sites|
|[ImagesBlockedForUrls](#block-images-on-specific-sites-imagesblockedforurls)|Block images on specific sites|
|[JavaScriptAllowedForUrls](#allow-javascript-on-specific-sites-javascriptallowedforurls)|Allow JavaScript on specific sites|
|[JavaScriptBlockedForUrls](#block-javascript-on-specific-sites-javascriptblockedforurls)|Block JavaScript on specific sites|
|[NotificationsAllowedForUrls](#allow-notifications-on-specific-sites-notificationsallowedforurls)|Allow notifications on specific sites|
|[NotificationsBlockedForUrls](#block-notifications-on-specific-sites-notificationsblockedforurls)|Block notifications on specific sites|
|[PluginsAllowedForUrls](#allow-the-adobe-flash-plug-in-on-specific-sites-pluginsallowedforurls)|Allow the Adobe Flash plug-in on specific sites|
|[PluginsBlockedForUrls](#block-the-adobe-flash-plug-in-on-specific-sites-pluginsblockedforurls)|Block the Adobe Flash plug-in on specific sites|
|[PopupsAllowedForUrls](#allow-pop-up-windows-on-specific-sites-popupsallowedforurls)|Allow pop-up windows on specific sites|
|[PopupsBlockedForUrls](#block-pop-up-windows-on-specific-sites-popupsblockedforurls)|Block pop-up windows on specific sites|
|[RegisteredProtocolHandlers](#register-protocol-handlers-registeredprotocolhandlers)|Register protocol handlers|
|[WebUsbAllowDevicesForUrls](#grant-access-to-specific-sites-to-connect-to-specific-usb-devices-webusballowdevicesforurls)|Grant access to specific sites to connect to specific USB devices.|
|[WebUsbAskForUrls](#allow-webusb-on-specific-sites-webusbaskforurls)|Allow WebUSB on specific sites|
|[WebUsbBlockedForUrls](#block-webusb-on-specific-sites-webusbblockedforurls)|Block WebUSB on specific sites|
|Default search provider||
|[DefaultSearchProviderEnabled](#enable-the-default-search-provider-defaultsearchproviderenabled)|Enable the default search provider|
|[DefaultSearchProviderEncodings](#default-search-provider-encodings-defaultsearchproviderencodings)|Default search provider encodings|
|[DefaultSearchProviderImageURL](#specifies-the-search-by-image-feature-for-the-default-search-provider-defaultsearchproviderimageurl)|Specifies the search-by-image feature for the default search provider|
|[DefaultSearchProviderImageURLPostParams](#parameters-for-an-image-url-that-uses-post-defaultsearchproviderimageurlpostparams)|Parameters for an image URL that uses POST|
|[DefaultSearchProviderKeyword](#default-search-provider-keyword-defaultsearchproviderkeyword)|Default search provider keyword|
|[DefaultSearchProviderName](#default-search-provider-name-defaultsearchprovidername)|Default search provider name|
|[DefaultSearchProviderSearchURL](#default-search-provider-search-url-defaultsearchprovidersearchurl)|Default search provider search URL|
|[DefaultSearchProviderSuggestURL](#default-search-provider-url-for-suggestions-defaultsearchprovidersuggesturl)|Default search provider URL for suggestions|
|Extensions||
|[ExtensionAllowedTypes](#configure-allowed-extension-types-extensionallowedtypes)|Configure allowed extension types|
|[ExtensionInstallAllowlist](#allow-specific-extensions-to-be-installed-extensioninstallallowlist)|Allow specific extensions to be installed|
|[ExtensionInstallBlocklist](#control-which-extensions-cannot-be-installed-extensioninstallblocklist)|Control which extensions cannot be installed|
|[ExtensionInstallForcelist](#control-which-extensions-are-installed-silently-extensioninstallforcelist)|Control which extensions are installed silently|
|[ExtensionInstallSources](#configure-extension-and-user-script-install-sources-extensioninstallsources)|Configure extension and user script install sources|
|[ExtensionSettings](#configure-extension-management-settings-extensionsettings)|Configure extension management settings|
|Cast||
|[EnableMediaRouter](#enable-google-cast-enablemediarouter)|Enable Google Cast|
|[ShowCastIconInToolbar](#show-the-cast-icon-in-the-toolbar-showcasticonintoolbar)|Show the cast icon in the toolbar|
|HTTP authentication||
|[AllowCrossOriginAuthPrompt](#allow-cross-origin-http-basic-auth-prompts-allowcrossoriginauthprompt)|Allow cross-origin HTTP Basic Auth prompts|
|[AuthNegotiateDelegateAllowlist](#specifies-a-list-of-servers-that-microsoft-edge-can-delegate-user-credentials-to-authnegotiatedelegateallowlist)|Specifies a list of servers that Microsoft Edge can delegate user credentials to|
|[AuthSchemes](#supported-authentication-schemes-authschemes)|Supported authentication schemes|
|[AuthServerAllowlist](#configure-list-of-allowed-authentication-servers-authserverallowlist)|Configure list of allowed authentication servers|
|[DisableAuthNegotiateCnameLookup](#disable-cname-lookup-when-negotiating-kerberos-authentication-disableauthnegotiatecnamelookup)|Disable CNAME lookup when negotiating Kerberos authentication|
|[EnableAuthNegotiatePort](#include-non-standard-port-in-kerberos-spn-enableauthnegotiateport)|Include non-standard port in Kerberos SPN|
|[NtlmV2Enabled](#control-whether-ntlmv2-authentication-is-enabled-ntlmv2enabled)|Control whether NTLMv2 authentication is enabled|
|Native Messaging||
|[NativeMessagingAllowlist](#control-which-native-messaging-hosts-users-can-use-nativemessagingallowlist)|Control which native messaging hosts users can use|
|[NativeMessagingBlocklist](#configure-native-messaging-block-list-nativemessagingblocklist)|Configure native messaging block list|
|[NativeMessagingUserLevelHosts](#allow-user-level-native-messaging-hosts-installed-without-admin-permissions-nativemessaginguserlevelhosts)|Allow user-level native messaging hosts (installed without admin permissions)|
|Password manager and protection||
|[PasswordManagerEnabled](#enable-saving-passwords-to-the-password-manager-passwordmanagerenabled)|Enable saving passwords to the password manager|
|[PasswordProtectionChangePasswordURL](#configure-the-change-password-url-passwordprotectionchangepasswordurl)|Configure the change password URL|
|[PasswordProtectionLoginURLs](#configure-the-list-of-enterprise-login-urls-where-password-protection-service-should-capture-fingerprint-of-password-passwordprotectionloginurls)|Configure the list of enterprise login URLs where password protection service should capture fingerprint of password|
|[PasswordProtectionWarningTrigger](#configure-password-protection-warning-trigger-passwordprotectionwarningtrigger)|Configure password protection warning trigger|
|Printing||
|[DefaultPrinterSelection](#default-printer-selection-rules-defaultprinterselection)|Default printer selection rules|
|[PrintHeaderFooter](#print-headers-and-footers-printheaderfooter)|Print headers and footers|
|[PrintPreviewUseSystemDefaultPrinter](#set-the-system-default-printer-as-the-default-printer-printpreviewusesystemdefaultprinter)|Set the system default printer as the default printer|
|[PrintingEnabled](#enable-printing-printingenabled)|Enable printing|
|[UseSystemPrintDialog](#print-using-system-print-dialog-usesystemprintdialog)|Print using system print dialog|
|Proxy server||
|[ProxyBypassList](#configure-proxy-bypass-rules-proxybypasslist)|Configure proxy bypass rules|
|[ProxyMode](#configure-proxy-server-settings-proxymode)|Configure proxy server settings|
|[ProxyPacUrl](#set-the-proxy-pac-file-url-proxypacurl)|Set the proxy .pac file URL|
|[ProxyServer](#configure-address-or-url-of-proxy-server-proxyserver)|Configure address or URL of proxy server|
|[ProxySettings](#proxy-settings-proxysettings)|Proxy settings|
|SmartScreen settings||
|[PreventSmartScreenPromptOverride](#prevent-bypassing-microsoft-defender-smartscreen-prompts-for-sites-preventsmartscreenpromptoverride)|Prevent bypassing Microsoft Defender SmartScreen prompts for sites|
|[PreventSmartScreenPromptOverrideForFiles](#prevent-bypassing-of-microsoft-defender-smartscreen-warnings-about-downloads-preventsmartscreenpromptoverrideforfiles)|Prevent bypassing of Microsoft Defender SmartScreen warnings about downloads|
|[SmartScreenAllowListDomains](#configure-the-list-of-domains-for-which-smartscreen-wont-trigger-warnings-smartscreenallowlistdomains)|Configure the list of domains for which SmartScreen won't trigger warnings|
|[SmartScreenEnabled](#configure-microsoft-defender-smartscreen-smartscreenenabled)|Configure Microsoft Defender SmartScreen|
|Startup, home page and new tab page||
|[HomepageIsNewTabPage](#set-the-new-tab-page-as-the-home-page-homepageisnewtabpage)|Set the new tab page as the home page|
|[HomepageLocation](#configure-the-home-page-url-homepagelocation)|Configure the home page URL|
|[NewTabPageHideDefaultTopSites](#hide-the-default-top-sites-from-the-new-tab-page-newtabpagehidedefaulttopsites)|Hide the default top sites from the new tab page|
|[NewTabPageLocation](#configure-the-new-tab-page-url-newtabpagelocation)|Configure the new tab page URL|
|[RestoreOnStartup](#action-to-take-on-startup-restoreonstartup)|Action to take on startup|
|[RestoreOnStartupURLs](#sites-to-open-when-the-browser-starts-restoreonstartupurls)|Sites to open when the browser starts|
|[ShowHomeButton](#show-home-button-on-toolbar-showhomebutton)|Show Home button on toolbar|
|Ungrouped Policies||
|[AllowDeletingBrowserHistory](#enable-deleting-browser-and-download-history-allowdeletingbrowserhistory)|Enable deleting browser and download history|
|[AllowFileSelectionDialogs](#allow-file-selection-dialogs-allowfileselectiondialogs)|Allow file selection dialogs|
|[AlwaysOpenPdfExternally](#always-open-pdf-files-externally-alwaysopenpdfexternally)|Always open PDF files externally|
|[ApplicationLocaleValue](#set-application-locale-applicationlocalevalue)|Set application locale|
|[AudioCaptureAllowed](#allow-or-block-audio-capture-audiocaptureallowed)|Allow or block audio capture|
|[AudioCaptureAllowedUrls](#sites-that-can-access-audio-capture-devices-without-requesting-permission-audiocaptureallowedurls)|Sites that can access audio capture devices without requesting permission|
|[AutoImportAtFirstRun](#automatically-import-another-browsers-data-and-settings-at-first-run-autoimportatfirstrun)|Automatically import another browser's data and settings at first run|
|[AutofillAddressEnabled](#enable-autofill-for-addresses-autofilladdressenabled)|Enable AutoFill for addresses|
|[AutofillCreditCardEnabled](#enable-autofill-for-credit-cards-autofillcreditcardenabled)|Enable AutoFill for credit cards|
|[BackgroundModeEnabled](#continue-running-background-apps-after-microsoft-edge-closes-backgroundmodeenabled)|Continue running background apps after Microsoft Edge closes|
|[BlockThirdPartyCookies](#block-third-party-cookies-blockthirdpartycookies)|Block third party cookies|
|[BrowserAddProfileEnabled](#enable-profile-creation-from-the-identity-flyout-menu-or-the-settings-page-browseraddprofileenabled)|Enable profile creation from the Identity flyout menu or the Settings page|
|[BrowserGuestModeEnabled](#enable-guest-mode-browserguestmodeenabled)|Enable guest mode|
|[BrowserNetworkTimeQueriesEnabled](#allow-queries-to-a-browser-network-time-service-browsernetworktimequeriesenabled)|Allow queries to a Browser Network Time service|
|[BrowserSignin](#browser-sign-in-settings-browsersignin)|Browser sign-in settings|
|[BuiltInDnsClientEnabled](#use-built-in-dns-client-builtindnsclientenabled)|Use built-in DNS client|
|[CertificateTransparencyEnforcementDisabledForCas](#disable-certificate-transparency-enforcement-for-a-list-of-subjectpublickeyinfo-hashes-certificatetransparencyenforcementdisabledforcas)|Disable Certificate Transparency enforcement for a list of subjectPublicKeyInfo hashes|
|[CertificateTransparencyEnforcementDisabledForLegacyCas](#disable-certificate-transparency-enforcement-for-a-list-of-legacy-certificate-authorities-certificatetransparencyenforcementdisabledforlegacycas)|Disable Certificate Transparency enforcement for a list of legacy certificate authorities|
|[CertificateTransparencyEnforcementDisabledForUrls](#disable-certificate-transparency-enforcement-for-specific-urls-certificatetransparencyenforcementdisabledforurls)|Disable Certificate Transparency enforcement for specific URLs|
|[CoalesceH2ConnectionsWithClientCertificatesForHosts](#allow-http2-connection-coalescing-for-these-hosts-even-when-client-certificates-are-used-coalesceh2connectionswithclientcertificatesforhosts)|Allow HTTP/2 connection coalescing for these hosts even when client certificates are used|
|[ComponentUpdatesEnabled](#enable-component-updates-in-microsoft-edge-componentupdatesenabled)|Enable component updates in Microsoft Edge|
|[ConfigureDoNotTrack](#configure-do-not-track-configuredonottrack)|Configure Do Not Track|
|[ConfigureOnlineTextToSpeech](#configure-online-text-to-speech-configureonlinetexttospeech)|Configure Online Text To Speech|
|[DefaultBrowserSettingEnabled](#set-microsoft-edge-as-default-browser-defaultbrowsersettingenabled)|Set Microsoft Edge as default browser|
|[DeveloperToolsAvailability](#control-where-developer-tools-can-be-used-developertoolsavailability)|Control where developer tools can be used|
|[Disable3DAPIs](#disable-support-for-3d-graphics-apis-disable3dapis)|Disable support for 3D graphics APIs|
|[DisableScreenshots](#disable-taking-screenshots-disablescreenshots)|Disable taking screenshots|
|[DiskCacheDir](#set-disk-cache-directory-diskcachedir)|Set disk cache directory|
|[DiskCacheSize](#set-disk-cache-size-in-bytes-diskcachesize)|Set disk cache size, in bytes|
|[DownloadDirectory](#set-download-directory-downloaddirectory)|Set download directory|
|[DownloadRestrictions](#allow-download-restrictions-downloadrestrictions)|Allow download restrictions|
|[EditFavoritesEnabled](#allows-users-to-edit-favorites-editfavoritesenabled)|Allows users to edit favorites|
|[EnableDeprecatedWebPlatformFeatures](#re-enable-deprecated-web-platform-features-for-a-limited-time-enabledeprecatedwebplatformfeatures)|Re-enable deprecated web platform features for a limited time|
|[EnableDomainActionsDownload](#enable-domain-actions-download-from-microsoft-enabledomainactionsdownload)|Enable Domain Actions Download from Microsoft|
|[EnableOnlineRevocationChecks](#enable-online-ocspcrl-checks-enableonlinerevocationchecks)|Enable online OCSP/CRL checks|
|[FavoritesBarEnabled](#enable-favorites-bar-favoritesbarenabled)|Enable favorites bar|
|[ForceBingSafeSearch](#configure-bing-safesearch-forcebingsafesearch)|Configure Bing SafeSearch|
|[ForceEphemeralProfiles](#enable-use-of-ephemeral-profiles-forceephemeralprofiles)|Enable use of ephemeral profiles|
|[ForceGoogleSafeSearch](#enforce-google-safesearch-forcegooglesafesearch)|Enforce Google SafeSearch|
|[ForceYouTubeRestrict](#force-minimum-youtube-restricted-mode-forceyoutuberestrict)|Force minimum YouTube Restricted Mode|
|[FullscreenAllowed](#allow-full-screen-mode-fullscreenallowed)|Allow full screen mode|
|[HardwareAccelerationModeEnabled](#use-hardware-acceleration-when-available-hardwareaccelerationmodeenabled)|Use hardware acceleration when available|
|[ImportAutofillFormData](#allow-importing-of-autofill-form-data-importautofillformdata)|Allow importing of autofill form data|
|[ImportFavorites](#allow-importing-of-favorites-importfavorites)|Allow importing of favorites|
|[ImportHistory](#allow-importing-of-browsing-history-importhistory)|Allow importing of browsing history|
|[ImportHomepage](#allow-importing-of-home-page-settings-importhomepage)|Allow importing of home page settings|
|[ImportPaymentInfo](#allow-importing-of-payment-info-importpaymentinfo)|Allow importing of payment info|
|[ImportSavedPasswords](#allow-importing-of-saved-passwords-importsavedpasswords)|Allow importing of saved passwords|
|[ImportSearchEngine](#allow-importing-of-search-engine-settings-importsearchengine)|Allow importing of search engine settings|
|[InPrivateModeAvailability](#configure-inprivate-mode-availability-inprivatemodeavailability)|Configure InPrivate mode availability|
|[InternetExplorerIntegrationLevel](#configure-internet-explorer-integration-internetexplorerintegrationlevel)|Configure Internet Explorer integration|
|[IsolateOrigins](#enable-site-isolation-for-specific-origins-isolateorigins)|Enable site isolation for specific origins|
|[ManagedFavorites](#configure-favorites-managedfavorites)|Configure favorites|
|[ManagedSearchEngines](#manage-search-engines-managedsearchengines)|Manage Search Engines|
|[MaxConnectionsPerProxy](#maximum-number-of-concurrent-connections-to-the-proxy-server-maxconnectionsperproxy)|Maximum number of concurrent connections to the proxy server|
|[MediaRouterCastAllowAllIPs](#allow-google-cast-to-connect-to-cast-devices-on-all-ip-addresses-mediaroutercastallowallips)|Allow Google Cast to connect to Cast devices on all IP addresses|
|[MetricsReportingEnabled](#enable-usage-and-crash-related-data-reporting-metricsreportingenabled)|Enable usage and crash-related data reporting|
|[NetworkPredictionOptions](#enable-network-prediction-networkpredictionoptions)|Enable network prediction|
|[OverrideSecurityRestrictionsOnInsecureOrigin](#control-where-security-restrictions-on-insecure-origins-apply-overridesecurityrestrictionsoninsecureorigin)|Control where security restrictions on insecure origins apply|
|[ProactiveAuthEnabled](#enable-proactive-authentication-proactiveauthenabled)|Enable Proactive Authentication|
|[PromotionalTabsEnabled](#enable-full-tab-promotional-content-promotionaltabsenabled)|Enable full-tab promotional content|
|[PromptForDownloadLocation](#ask-where-to-save-downloaded-files-promptfordownloadlocation)|Ask where to save downloaded files|
|[QuicAllowed](#allow-quic-protocol-quicallowed)|Allow QUIC protocol|
|[RelaunchNotification](#notify-a-user-that-a-browser-restart-is-recommended-or-required-for-pending-updates-relaunchnotification)|Notify a user that a browser restart is recommended or required for pending updates|
|[RelaunchNotificationPeriod](#set-the-time-period-for-update-notifications-relaunchnotificationperiod)|Set the time period for update notifications|
|[RequireOnlineRevocationChecksForLocalAnchors](#specify-if-online-ocspcrl-checks-are-required-for-local-trust-anchors-requireonlinerevocationchecksforlocalanchors)|Specify if online OCSP/CRL checks are required for local trust anchors|
|[ResolveNavigationErrorsUseWebService](#enable-resolution-of-navigation-errors-using-a-web-service-resolvenavigationerrorsusewebservice)|Enable resolution of navigation errors using a web service|
|[RestrictSigninToPattern](#restrict-which-accounts-can-be-used-as-microsoft-edge-primary-accounts-restrictsignintopattern)|Restrict which accounts can be used as Microsoft Edge primary accounts|
|[RunAllFlashInAllowMode](#extend-adobe-flash-content-setting-to-all-content-runallflashinallowmode)|Extend Adobe Flash content setting to all content|
|[SSLErrorOverrideAllowed](#allow-users-to-proceed-from-the-ssl-warning-page-sslerroroverrideallowed)|Allow users to proceed from the SSL warning page|
|[SSLVersionMin](#minimum-ssl-version-enabled-sslversionmin)|Minimum SSL version enabled|
|[SavingBrowserHistoryDisabled](#disable-saving-browser-history-savingbrowserhistorydisabled)|Disable saving browser history|
|[SearchSuggestEnabled](#enable-search-suggestions-searchsuggestenabled)|Enable search suggestions|
|[SecurityKeyPermitAttestation](#websites-or-domains-that-dont-need-permission-to-use-direct-security-key-attestation-securitykeypermitattestation)|Websites or domains that don't need permission to use direct Security Key attestation|
|[SendIntranetToInternetExplorer](#send-all-intranet-sites-to-internet-explorer-sendintranettointernetexplorer)|Send all intranet sites to Internet Explorer|
|[SendSiteInfoToImproveServices](#send-site-information-to-improve-microsoft-services-sendsiteinfotoimproveservices)|Send site information to improve Microsoft services|
|[ShowOfficeShortcutInFavoritesBar](#show-microsoft-office-shortcut-in-favorites-bar-showofficeshortcutinfavoritesbar)|Show Microsoft Office shortcut in favorites bar|
|[SitePerProcess](#enable-site-isolation-for-every-site-siteperprocess)|Enable site isolation for every site|
|[SpellcheckEnabled](#enable-spellcheck-spellcheckenabled)|Enable spellcheck|
|[SpellcheckLanguage](#enable-specific-spellcheck-languages-spellchecklanguage)|Enable specific spellcheck languages|
|[SuppressUnsupportedOSWarning](#suppress-the-unsupported-os-warning-suppressunsupportedoswarning)|Suppress the unsupported OS warning|
|[SyncDisabled](#disable-synchronization-of-data-using-microsoft-sync-services-syncdisabled)|Disable synchronization of data using Microsoft sync services|
|[TabLifecyclesEnabled](#configure-tab-lifecycles-tablifecyclesenabled)|Configure tab lifecycles|
|[TaskManagerEndProcessEnabled](#enable-ending-processes-in-the-browser-task-manager-taskmanagerendprocessenabled)|Enable ending processes in the Browser task manager|
|[TranslateEnabled](#enable-translate-translateenabled)|Enable Translate|
|[URLAllowlist](#define-a-list-of-allowed-urls-urlallowlist)|Define a list of allowed URLs|
|[URLBlocklist](#block-access-to-a-list-of-urls-urlblocklist)|Block access to a list of URLs|
|[UserDataDir](#set-the-user-data-directory-userdatadir)|Set the user data directory|
|[UserFeedbackAllowed](#allow-user-feedback-userfeedbackallowed)|Allow user feedback|
|[VideoCaptureAllowed](#allow-or-block-video-capture-videocaptureallowed)|Allow or block video capture|
|[VideoCaptureAllowedUrls](#sites-that-can-access-video-capture-devices-without-requesting-permission-videocaptureallowedurls)|Sites that can access video capture devices without requesting permission|
|[WPADQuickCheckEnabled](#set-wpad-optimization-wpadquickcheckenabled)|Set WPAD optimization|
|[WebDriverOverridesIncompatiblePolicies](#allow-webdriver-to-override-incompatible-policies-webdriveroverridesincompatiblepolicies)|Allow WebDriver to Override Incompatible Policies|
|[WebRtcLocalhostIpHandling](#restrict-exposure-of-localhost-ip-address-by-webrtc-webrtclocalhostiphandling)|Restrict exposure of localhost IP address by WebRTC|
|[WebRtcUdpPortRange](#restrict-the-range-of-local-udp-ports-used-by-webrtc-webrtcudpportrange)|Restrict the range of local UDP ports used by WebRTC|




  ## Automatically select client certificates for these sites (AutoSelectCertificateForUrls)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Specify a list of sites, based on URL patterns, for which Microsoft Edge should automatically select a client certificate, if the site requests one.

The value must be an array of stringified JSON dictionaries. The form for each dictionary is { "pattern": "$URL_PATTERN", "filter" : $FILTER }, where $URL_PATTERN is a content setting pattern. $FILTER restricts from which client certificates the browser can automatically select. Independent of the filter, only certificates that match the server's certificate request can be used. For example, if $FILTER has the form { "ISSUER": { "CN": "$ISSUER_CN" } }, additionally only client certificates that are issued by a certificate with the CommonName $ISSUER_CN can be used. If $FILTER contains an "ISSUER" and a "SUBJECT" section, a client certificate must meet both conditions to be selected. If $FILTER specifies an organization ("O"), a certificate must have at least one organization that matches the specified value. If $FILTER specifies an organization unit ("OU"), a certificate must have at least one organization unit which matches the specified value. If $FILTER is the empty dictionary {}, the selection of client certificates isn't additionally restricted.

If you don't configure this policy, auto-selection isn't done for any site.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  List of strings

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: AutoSelectCertificateForUrls
  - GP name: Automatically select client certificates for these sites
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Content settings
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge\AutoSelectCertificateForUrls
  - Path (Recommended):N/A
  - Value Name:1, 2, 3, ...
  - Value Type:list of REG_SZ
  #### Example value: 
```
SOFTWARE\Policies\Microsoft\Edge\AutoSelectCertificateForUrls\0 = "{"pattern":"https://www.contoso.com","filter":{"ISSUER":{"CN":"certificate issuer name", "L": "certificate issuer location", "O": "certificate issuer org", "OU": "certificate issuer org unit"}, "SUBJECT":{"CN":"certificate subject name", "L": "certificate subject location", "O": "certificate subject org", "OU": "certificate subject org unit"}}}"

```


  ### Mac information and settings
  - Preference Key Name: AutoSelectCertificateForUrls
  - Example value: 
```
<array>
  <string>{"pattern":"https://www.contoso.com","filter":{"ISSUER":{"CN":"certificate issuer name", "L": "certificate issuer location", "O": "certificate issuer org", "OU": "certificate issuer org unit"}, "SUBJECT":{"CN":"certificate subject name", "L": "certificate subject location", "O": "certificate subject org", "OU": "certificate subject org unit"}}}</string>
</array>

```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Allow cookies on specific sites (CookiesAllowedForUrls)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Define a list of sites, based on URL patterns, that are allowed to set cookies.

If you don't configure this policy, the global default value from the 'DefaultCookiesSetting' policy (if set) or the user's personal configuration is used for all sites.

See the 'CookiesBlockedForUrls' and 'CookiesSessionOnlyForUrls' policies for more information.

Note there cannot be conflicting URL patterns set between these three policies:

- CookiesBlockedForUrls

- CookiesAllowedForUrls

- CookiesSesssionOnlyForUrls

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  List of strings

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: CookiesAllowedForUrls
  - GP name: Allow cookies on specific sites
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Content settings
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge\CookiesAllowedForUrls
  - Path (Recommended):N/A
  - Value Name:1, 2, 3, ...
  - Value Type:list of REG_SZ
  #### Example value: 
```
SOFTWARE\Policies\Microsoft\Edge\CookiesAllowedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\CookiesAllowedForUrls\1 = "[*.]contoso.edu"

```


  ### Mac information and settings
  - Preference Key Name: CookiesAllowedForUrls
  - Example value: 
```
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>

```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Block cookies on specific sites (CookiesBlockedForUrls)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Define a list of sites, based on URL patterns, that can't set cookies.

If you don't configure this policy, the global default value from the 'DefaultCookiesSetting' policy (if set) or the user's personal configuration is used for all sites.

See the 'CookiesAllowedForUrls' and 'CookiesSessionOnlyForUrls' policies for more information.

Note there cannot be conflicting URL patterns set between these three policies:

- CookiesBlockedForUrls

- CookiesAllowedForUrls

- CookiesSesssionOnlyForUrls

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  List of strings

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: CookiesBlockedForUrls
  - GP name: Block cookies on specific sites
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Content settings
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge\CookiesBlockedForUrls
  - Path (Recommended):N/A
  - Value Name:1, 2, 3, ...
  - Value Type:list of REG_SZ
  #### Example value: 
```
SOFTWARE\Policies\Microsoft\Edge\CookiesBlockedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\CookiesBlockedForUrls\1 = "[*.]contoso.edu"

```


  ### Mac information and settings
  - Preference Key Name: CookiesBlockedForUrls
  - Example value: 
```
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>

```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Limit cookies from specific websites to the current session (CookiesSessionOnlyForUrls)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Cookies created by websites that match a URL pattern you define are deleted when the session ends (when the window closes).

Cookies created by websites that don't match the pattern are controlled by the 'DefaultCookiesSetting' policy (if set) or by the user's personal configuration. This is also the default behavior if you don't configure this policy.

If Microsoft Edge is running in background mode, the session might not close when the last window is closed, meaning the cookies won't be cleared when the window closes. See the 'BackgroundModeEnabled' policy for information about configuring what happens when Microsoft Edge runs in background mode.

You can also use the 'CookiesAllowedForUrls' and 'CookiesBlockedForUrls' policies to control which websites can create cookies.

Note there cannot be conflicting URL patterns set between these three policies:

- CookiesBlockedForUrls

- CookiesAllowedForUrls

- CookiesSesssionOnlyForUrls

If you set the 'RestoreOnStartup' policy to restore URLs from previous sessions, this policy is ignored, and cookies are stored permanently for those sites.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  List of strings

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: CookiesSessionOnlyForUrls
  - GP name: Limit cookies from specific websites to the current session
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Content settings
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge\CookiesSessionOnlyForUrls
  - Path (Recommended):N/A
  - Value Name:1, 2, 3, ...
  - Value Type:list of REG_SZ
  #### Example value: 
```
SOFTWARE\Policies\Microsoft\Edge\CookiesSessionOnlyForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\CookiesSessionOnlyForUrls\1 = "[*.]contoso.edu"

```


  ### Mac information and settings
  - Preference Key Name: CookiesSessionOnlyForUrls
  - Example value: 
```
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>

```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Configure cookies (DefaultCookiesSetting)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Control whether websites can create cookies on the user's device. This policy is all or nothing - you can let all websites create cookies, or no websites create cookies. You can't use this policy to enable cookies from specific websites.

Set the policy to 'SessionOnly' (4) to clear cookies when the session closes. If Microsoft Edge is running in background mode, the session might not close when the last window is closed, meaning the cookies won't be cleared when the window closes. See 'BackgroundModeEnabled' policy for information about configuring what happens when Microsoft Edge runs in background mode.

If you don't configure this policy, the default 'AllowCookies' (1) is used, and users can change this setting in Microsoft Edge Settings. (If you don't want users to be able to change this setting, set the policy.)

* 1 = Let all sites create cookies

* 2 = Don't let any site create cookies

* 4 = Keep cookies for the duration of the session

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  Integer

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: DefaultCookiesSetting
  - GP name: Configure cookies
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Content settings
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:DefaultCookiesSetting
  - Value Type:REG_DWORD
  #### Example value: 
```
0x00000001
```


  ### Mac information and settings
  - Preference Key Name: DefaultCookiesSetting
  - Example value: 
```
1
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Default geolocation setting (DefaultGeolocationSetting)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Set whether websites can track users' physical locations. You can allow tracking by default (1), deny it by default (2), or ask the user each time a website requests their location (3).

If you don't configure this policy, 'AskGeolocation' policy is used and the user can change it.

* 1 = Allow sites to track users' physical location

* 2 = Don't allow any site to track users' physical location

* 3 = Ask whenever a site wants to track users' physical location

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  Integer

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: DefaultGeolocationSetting
  - GP name: Default geolocation setting
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Content settings
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:DefaultGeolocationSetting
  - Value Type:REG_DWORD
  #### Example value: 
```
0x00000001
```


  ### Mac information and settings
  - Preference Key Name: DefaultGeolocationSetting
  - Example value: 
```
1
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Default images setting (DefaultImagesSetting)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Set whether websites can display images. You can allow images on all sites (1) or block them on all sites (2).

If you don't configure this policy, images are allowed by default, and the user can change this setting.

* 1 = Allow all sites to show all images

* 2 = Don't allow any site to show images

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  Integer

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: DefaultImagesSetting
  - GP name: Default images setting
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Content settings
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:DefaultImagesSetting
  - Value Type:REG_DWORD
  #### Example value: 
```
0x00000001
```


  ### Mac information and settings
  - Preference Key Name: DefaultImagesSetting
  - Example value: 
```
1
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Default JavaScript setting (DefaultJavaScriptSetting)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Set whether websites can run JavaScript. You can allow it for all sites (1) or block it for all sites (2).

If you don't configure this policy, all sites can run JavaScript by default, and the user can change this setting.

* 1 = Allow all sites to run JavaScript

* 2 = Don't allow any site to run JavaScript

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  Integer

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: DefaultJavaScriptSetting
  - GP name: Default JavaScript setting
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Content settings
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:DefaultJavaScriptSetting
  - Value Type:REG_DWORD
  #### Example value: 
```
0x00000001
```


  ### Mac information and settings
  - Preference Key Name: DefaultJavaScriptSetting
  - Example value: 
```
1
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Default notification setting (DefaultNotificationsSetting)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Set whether websites can display desktop notifications. You can allow them by default (1), deny them by default (2), or have the user be asked each time a website wants to show a notification (3).

If you don't configure this policy, notifications are allowed by default, and the user can change this setting.

* 1 = Allow sites to show desktop notifications

* 2 = Don't allow any site to show desktop notifications

* 3 = Ask every time a site wants to show desktop notifications

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  Integer

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: DefaultNotificationsSetting
  - GP name: Default notification setting
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Content settings
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:DefaultNotificationsSetting
  - Value Type:REG_DWORD
  #### Example value: 
```
0x00000002
```


  ### Mac information and settings
  - Preference Key Name: DefaultNotificationsSetting
  - Example value: 
```
2
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Default Adobe Flash setting (DefaultPluginsSetting)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Determines whether websites that aren't covered by 'PluginsAllowedForUrls' or 'PluginsBlockedForUrls' can automatically run the Adobe Flash plug-in. You can select 'BlockPlugins' (2) to block Adobe Flash on all sites, or you can select 'ClickToPlay' (3) to let Adobe Flash run but require the user to click the placeholder to start it. In any case, the 'PluginsAllowedForUrls' and 'PluginsBlockedForUrls' policies take precedence over 'DefaultPluginsSetting'.

Automatic playback is only allowed for domains explicitly listed in the 'PluginsAllowedForUrls' policy. If you want to enable automatic playback for all sites, consider adding http://* and https://* to this list.

If you don't configure this policy, the user can change this setting manually.

* 2 = Block the Adobe Flash plug-in

* 3 = Click to play

The former '1' option set allow-all, but this functionality is now only handled by the 'PluginsAllowedForUrls' policy.  Existing policies using '1' will operate in Click-to-play mode.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  Integer

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: DefaultPluginsSetting
  - GP name: Default Adobe Flash setting
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Content settings
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:DefaultPluginsSetting
  - Value Type:REG_DWORD
  #### Example value: 
```
0x00000002
```


  ### Mac information and settings
  - Preference Key Name: DefaultPluginsSetting
  - Example value: 
```
2
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Default pop-up window setting (DefaultPopupsSetting)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Set whether websites can show pop-up windows. You can allow them on all websites (1) or block them on all sites (2).

If you don't configure this policy, pop-up windows are blocked by default, and users can change this setting.

* 1 = Allow all sites to show pop-ups

* 2 = Don't allow any site to show pop-up windows

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  Integer

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: DefaultPopupsSetting
  - GP name: Default pop-up window setting
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Content settings
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:DefaultPopupsSetting
  - Value Type:REG_DWORD
  #### Example value: 
```
0x00000001
```


  ### Mac information and settings
  - Preference Key Name: DefaultPopupsSetting
  - Example value: 
```
1
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Control use of the Web Bluetooth API (DefaultWebBluetoothGuardSetting)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Control whether websites can access nearby Bluetooth devices. You can completely block access or require the site to ask the user each time it wants to access a Bluetooth device.

If you don't configure this policy, the default value (3, meaning users are asked each time) is used and users can change it.

* 2 = Don't allow any site to request access to Bluetooth devices by using the Web Bluetooth API

* 3 = Allow sites to ask the user to grant access to a nearby Bluetooth device

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  Integer

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: DefaultWebBluetoothGuardSetting
  - GP name: Control use of the Web Bluetooth API
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Content settings
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:DefaultWebBluetoothGuardSetting
  - Value Type:REG_DWORD
  #### Example value: 
```
0x00000002
```


  ### Mac information and settings
  - Preference Key Name: DefaultWebBluetoothGuardSetting
  - Example value: 
```
2
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Control use of the WebUSB API (DefaultWebUsbGuardSetting)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Set whether websites can access connected USB devices. You can completely block access or ask the user each time a website wants to get access to connected USB devices.

You can override this policy for specific URL patterns by using the 'WebUsbAskForUrls' and 'WebUsbBlockedForUrls' policies.

If you don't configure this policy, sites can ask users whether they can access the connected USB devices (3) by default, and users can change this setting.

* 2 = Don't allow any site to request access to USB devices via the WebUSB API

* 3 = Allow sites to ask the user to grant access to a connected USB device

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  Integer

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: DefaultWebUsbGuardSetting
  - GP name: Control use of the WebUSB API
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Content settings
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:DefaultWebUsbGuardSetting
  - Value Type:REG_DWORD
  #### Example value: 
```
0x00000002
```


  ### Mac information and settings
  - Preference Key Name: DefaultWebUsbGuardSetting
  - Example value: 
```
2
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Allow images on these sites (ImagesAllowedForUrls)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Define a list of sites, based on URL patterns, that can display images.

If you don't configure this policy, the global default value is used for all sites either from the 'DefaultImagesSetting' policy (if set) or the user's personal configuration.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  List of strings

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: ImagesAllowedForUrls
  - GP name: Allow images on these sites
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Content settings
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge\ImagesAllowedForUrls
  - Path (Recommended):N/A
  - Value Name:1, 2, 3, ...
  - Value Type:list of REG_SZ
  #### Example value: 
```
SOFTWARE\Policies\Microsoft\Edge\ImagesAllowedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\ImagesAllowedForUrls\1 = "[*.]contoso.edu"

```


  ### Mac information and settings
  - Preference Key Name: ImagesAllowedForUrls
  - Example value: 
```
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>

```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Block images on specific sites (ImagesBlockedForUrls)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Define a list of sites, based on URL patterns, that aren't allowed to display images.

If you don't configure this policy, the global default value from the 'DefaultImagesSetting' policy (if set) or the user's personal configuration is used for all sites.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  List of strings

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: ImagesBlockedForUrls
  - GP name: Block images on specific sites
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Content settings
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge\ImagesBlockedForUrls
  - Path (Recommended):N/A
  - Value Name:1, 2, 3, ...
  - Value Type:list of REG_SZ
  #### Example value: 
```
SOFTWARE\Policies\Microsoft\Edge\ImagesBlockedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\ImagesBlockedForUrls\1 = "[*.]contoso.edu"

```


  ### Mac information and settings
  - Preference Key Name: ImagesBlockedForUrls
  - Example value: 
```
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>

```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Allow JavaScript on specific sites (JavaScriptAllowedForUrls)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Define a list of sites, based on URL patterns, that are allowed to run JavaScript.

If you don't configure this policy, the global default value from the 'DefaultJavaScriptSetting' policy (if set) or the user's personal configuration is used for all sites.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  List of strings

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: JavaScriptAllowedForUrls
  - GP name: Allow JavaScript on specific sites
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Content settings
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge\JavaScriptAllowedForUrls
  - Path (Recommended):N/A
  - Value Name:1, 2, 3, ...
  - Value Type:list of REG_SZ
  #### Example value: 
```
SOFTWARE\Policies\Microsoft\Edge\JavaScriptAllowedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\JavaScriptAllowedForUrls\1 = "[*.]contoso.edu"

```


  ### Mac information and settings
  - Preference Key Name: JavaScriptAllowedForUrls
  - Example value: 
```
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>

```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Block JavaScript on specific sites (JavaScriptBlockedForUrls)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Define a list of sites, based on URL patterns, that aren't allowed to run JavaScript.

If you don't configure this policy, the global default value from the 'DefaultJavaScriptSetting' policy (if set) or the user's personal configuration is used for all sites.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  List of strings

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: JavaScriptBlockedForUrls
  - GP name: Block JavaScript on specific sites
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Content settings
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge\JavaScriptBlockedForUrls
  - Path (Recommended):N/A
  - Value Name:1, 2, 3, ...
  - Value Type:list of REG_SZ
  #### Example value: 
```
SOFTWARE\Policies\Microsoft\Edge\JavaScriptBlockedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\JavaScriptBlockedForUrls\1 = "[*.]contoso.edu"

```


  ### Mac information and settings
  - Preference Key Name: JavaScriptBlockedForUrls
  - Example value: 
```
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>

```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Allow notifications on specific sites (NotificationsAllowedForUrls)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Define a list of sites, based on URL patterns, that can display notifications.

If you don't configure this policy, the global default value from the 'DefaultNotificationsSetting' policy (if set) or the user's personal configuration is used for all sites.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  List of strings

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: NotificationsAllowedForUrls
  - GP name: Allow notifications on specific sites
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Content settings
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge\NotificationsAllowedForUrls
  - Path (Recommended):N/A
  - Value Name:1, 2, 3, ...
  - Value Type:list of REG_SZ
  #### Example value: 
```
SOFTWARE\Policies\Microsoft\Edge\NotificationsAllowedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\NotificationsAllowedForUrls\1 = "[*.]contoso.edu"

```


  ### Mac information and settings
  - Preference Key Name: NotificationsAllowedForUrls
  - Example value: 
```
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>

```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Block notifications on specific sites (NotificationsBlockedForUrls)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Define a list of sites, based on URL patterns, that are blocked from displaying notifications.

If you don't configure this policy, the global default value from the 'DefaultNotificationsSetting' policy (if set) or the user's personal configuration is used for all sites.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  List of strings

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: NotificationsBlockedForUrls
  - GP name: Block notifications on specific sites
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Content settings
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge\NotificationsBlockedForUrls
  - Path (Recommended):N/A
  - Value Name:1, 2, 3, ...
  - Value Type:list of REG_SZ
  #### Example value: 
```
SOFTWARE\Policies\Microsoft\Edge\NotificationsBlockedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\NotificationsBlockedForUrls\1 = "[*.]contoso.edu"

```


  ### Mac information and settings
  - Preference Key Name: NotificationsBlockedForUrls
  - Example value: 
```
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>

```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Allow the Adobe Flash plug-in on specific sites (PluginsAllowedForUrls)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Define a list of sites, based on URL patterns, that can run the Adobe Flash plug-in.

If you don't configure this policy, the global default value from the 'DefaultPluginsSetting' policy (if set) or the user's personal configuration is used for all sites.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  List of strings

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: PluginsAllowedForUrls
  - GP name: Allow the Adobe Flash plug-in on specific sites
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Content settings
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge\PluginsAllowedForUrls
  - Path (Recommended):N/A
  - Value Name:1, 2, 3, ...
  - Value Type:list of REG_SZ
  #### Example value: 
```
SOFTWARE\Policies\Microsoft\Edge\PluginsAllowedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\PluginsAllowedForUrls\1 = "[*.]contoso.edu"

```


  ### Mac information and settings
  - Preference Key Name: PluginsAllowedForUrls
  - Example value: 
```
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>

```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Block the Adobe Flash plug-in on specific sites (PluginsBlockedForUrls)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Define a list of sites, based on URL patterns, that are blocked from running Adobe Flash.

If you don't configure this policy, the global default value from the 'DefaultPluginsSetting' policy (if set) or the user's personal configuration is used for all sites.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  List of strings

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: PluginsBlockedForUrls
  - GP name: Block the Adobe Flash plug-in on specific sites
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Content settings
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge\PluginsBlockedForUrls
  - Path (Recommended):N/A
  - Value Name:1, 2, 3, ...
  - Value Type:list of REG_SZ
  #### Example value: 
```
SOFTWARE\Policies\Microsoft\Edge\PluginsBlockedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\PluginsBlockedForUrls\1 = "[*.]contoso.edu"

```


  ### Mac information and settings
  - Preference Key Name: PluginsBlockedForUrls
  - Example value: 
```
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>

```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Allow pop-up windows on specific sites (PopupsAllowedForUrls)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Define a list of sites, based on URL patterns, that can open pop-up windows.

If you don't configure this policy, the global default value from the 'DefaultPopupsSetting' policy (if set) or the user's personal configuration is used for all sites.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  List of strings

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: PopupsAllowedForUrls
  - GP name: Allow pop-up windows on specific sites
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Content settings
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge\PopupsAllowedForUrls
  - Path (Recommended):N/A
  - Value Name:1, 2, 3, ...
  - Value Type:list of REG_SZ
  #### Example value: 
```
SOFTWARE\Policies\Microsoft\Edge\PopupsAllowedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\PopupsAllowedForUrls\1 = "[*.]contoso.edu"

```


  ### Mac information and settings
  - Preference Key Name: PopupsAllowedForUrls
  - Example value: 
```
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>

```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Block pop-up windows on specific sites (PopupsBlockedForUrls)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Define a list of sites, based on URL patterns, that are blocked from opening pop-up windows.

If you don't configure this policy, the global default value from the 'DefaultPopupsSetting' policy (if set) or the user's personal configuration is used for all sites.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  List of strings

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: PopupsBlockedForUrls
  - GP name: Block pop-up windows on specific sites
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Content settings
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge\PopupsBlockedForUrls
  - Path (Recommended):N/A
  - Value Name:1, 2, 3, ...
  - Value Type:list of REG_SZ
  #### Example value: 
```
SOFTWARE\Policies\Microsoft\Edge\PopupsBlockedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\PopupsBlockedForUrls\1 = "[*.]contoso.edu"

```


  ### Mac information and settings
  - Preference Key Name: PopupsBlockedForUrls
  - Example value: 
```
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>

```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Register protocol handlers (RegisteredProtocolHandlers)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Register a list of protocol handlers. Set the protocol property to the scheme (like 'mailto') and the url property to the URL pattern of the application that handles the scheme. The pattern can include a '%s', which will be replaced by the handled URL.

You can recommend a specific value for this policy, but you can't require that your users use it.

The protocol handlers registered by policy are merged with any handlers registered by the user, and both are available for use. The user can override the protocol handlers installed by policy by installing a new default handler, but they can't remove a protocol handler registered by policy.

  ### Supported features:
  - Can be mandatory: No
  - Can be recommended: Yes
  - Dynamic Policy Refresh: No - Requires browser restart

  ### Data Type:
  Dictionary

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: RegisteredProtocolHandlers
  - GP name: Register protocol handlers
  - GP path (Mandatory):N/A
  - GP path (Recommended): Administrative Templates/Microsoft Edge - Default Settings (users can override)/Content settings
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory):N/A
  - Path (Recommended): SOFTWARE\Policies\Microsoft\Edge\Recommended
  - Value Name:RegisteredProtocolHandlers
  - Value Type:REG_SZ
  #### Example value: 
```
SOFTWARE\Policies\Microsoft\Edge\RegisteredProtocolHandlers = [
  {
    "default": true, 
    "protocol": "mailto", 
    "url": "https://mail.contoso.com/mail/?extsrc=mailto&url=%s"
  }
]
```


  ### Mac information and settings
  - Preference Key Name: RegisteredProtocolHandlers
  - Example value: 
```
<key>RegisteredProtocolHandlers</key>
<array>
  <dict>
    <key>default</key>
    <true/>
    <key>protocol</key>
    <string>mailto</string>
    <key>url</key>
    <string>https://mail.contoso.com/mail/?extsrc=mailto&url=%s</string>
  </dict>
</array>
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Grant access to specific sites to connect to specific USB devices. (WebUsbAllowDevicesForUrls)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Define a list of sites that can automatically access a USB device with the given vendor and product IDs. Each item in the list must contain both devices and URLs in order for the policy to be valid. Each device definition contains a vendor ID and product ID field. Any ID that's not defined is treated as a wildcard with one exception: you can't specify a product ID without a vendor ID. If you do, the policy isn't valid and is ignored.

The USB permission model uses the URL of the requesting site ("requesting URL") and the URL of the top-level frame site ("embedding URL") to grant access for the requesting URL to the USB device. The requesting URL may be different than the embedding URL when the requesting site is loaded in an iframe. Because of this, the "urls" field can contain up to two URL strings, separated by a comma, to specify the requesting and embedding URL respectively. If only one URL is specified, then access to the corresponding USB devices is granted when the requesting site's URL matches this URL, regardless of embedding status. The URLs in "urls" must be valid URLs, otherwise the policy is ignored.

If you don't configure this policy, the global default value from the 'DefaultWebUsbGuardSetting' policy (if set) or the user's personal configuration is used for all sites.

URL patterns in this policy shouldn't clash with those configured in the 'WebUsbBlockedForUrls' policy. If there is a clash, this policy takes precedence over 'WebUsbBlockedForUrls' and 'WebUsbAskForUrls' policies.

Values for this policy and the DeviceWebUsbAllowDevicesForUrls policy are merged together.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  Dictionary

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: WebUsbAllowDevicesForUrls
  - GP name: Grant access to specific sites to connect to specific USB devices.
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Content settings
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:WebUsbAllowDevicesForUrls
  - Value Type:REG_SZ
  #### Example value: 
```
SOFTWARE\Policies\Microsoft\Edge\WebUsbAllowDevicesForUrls = [
  {
    "devices": [
      {
        "product_id": 5678, 
        "vendor_id": 1234
      }
    ], 
    "urls": [
      "https://contoso.com", 
      "https://fabrikam.com"
    ]
  }
]
```


  ### Mac information and settings
  - Preference Key Name: WebUsbAllowDevicesForUrls
  - Example value: 
```
<key>WebUsbAllowDevicesForUrls</key>
<array>
  <dict>
    <key>devices</key>
    <array>
      <dict>
        <key>product_id</key>
        <integer>5678</integer>
        <key>vendor_id</key>
        <integer>1234</integer>
      </dict>
    </array>
    <key>urls</key>
    <array>
      <string>https://contoso.com</string>
      <string>https://fabrikam.com</string>
    </array>
  </dict>
</array>
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Allow WebUSB on specific sites (WebUsbAskForUrls)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Define a list of sites, based on URL patterns, that can ask the user for access to a USB device.

If you don't configure this policy, the global default value from the 'DefaultWebUsbGuardSetting' policy (if set) or the user's personal configuration is used for all sites.

The URL patterns defined in this policy can't conflict with those configured in the 'WebUsbBlockedForUrls' policy - you can't both allow and block a URL.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  List of strings

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: WebUsbAskForUrls
  - GP name: Allow WebUSB on specific sites
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Content settings
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge\WebUsbAskForUrls
  - Path (Recommended):N/A
  - Value Name:1, 2, 3, ...
  - Value Type:list of REG_SZ
  #### Example value: 
```
SOFTWARE\Policies\Microsoft\Edge\WebUsbAskForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\WebUsbAskForUrls\1 = "[*.]contoso.edu"

```


  ### Mac information and settings
  - Preference Key Name: WebUsbAskForUrls
  - Example value: 
```
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>

```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Block WebUSB on specific sites (WebUsbBlockedForUrls)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Define a list of sites, based on URL patterns, that can't ask the user to grant them access to a USB device.

If you don't configure this policy, the global default value from the 'DefaultWebUsbGuardSetting' policy (if set) or the user's personal configuration is used for all sites.

URL patterns in this policy can't conflict with those configured in the 'WebUsbAskForUrls' policy. You can't both allow and block a URL.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  List of strings

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: WebUsbBlockedForUrls
  - GP name: Block WebUSB on specific sites
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Content settings
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge\WebUsbBlockedForUrls
  - Path (Recommended):N/A
  - Value Name:1, 2, 3, ...
  - Value Type:list of REG_SZ
  #### Example value: 
```
SOFTWARE\Policies\Microsoft\Edge\WebUsbBlockedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\WebUsbBlockedForUrls\1 = "[*.]contoso.edu"

```


  ### Mac information and settings
  - Preference Key Name: WebUsbBlockedForUrls
  - Example value: 
```
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>

```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Enable the default search provider (DefaultSearchProviderEnabled)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Enables the use of a default search provider.

If you enable this policy, a user can search for a term by typing in the address bar (as long as what they type isn't a URL).

You can specify the default search provider to use by enabling the rest of the default search policies. If these are left empty (not configured), the user can choose the default provider.

If you disable this policy, the user can't search from the address bar.

If you enable or disable this policy, users can't change or override it.

If you don't configure this policy, the default search provider is enabled, and the user can choose the default search provider and set the search provider list.

This policy is available only on Windows instances that are joined to a Microsoft Active Directory domain or Windows 10 Pro or Enterprise instances that are enrolled for device management.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  Boolean

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: DefaultSearchProviderEnabled
  - GP name: Enable the default search provider
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Default search provider
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:DefaultSearchProviderEnabled
  - Value Type:REG_DWORD
  #### Example value: 
```
True
```


  ### Mac information and settings
  - Preference Key Name: DefaultSearchProviderEnabled
  - Example value: 
```
True
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Default search provider encodings (DefaultSearchProviderEncodings)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Specify the character encodings supported by the search provider. Encodings are code page names like UTF-8, GB2312, and ISO-8859-1. They are tried in the order provided.

This policy is optional. If not configured, the default, UTF-8, is used.

This policy is applied only if you enable the 'DefaultSearchProviderEnabled' and 'DefaultSearchProviderSearchURL' policies.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  List of strings

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: DefaultSearchProviderEncodings
  - GP name: Default search provider encodings
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Default search provider
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge\DefaultSearchProviderEncodings
  - Path (Recommended):N/A
  - Value Name:1, 2, 3, ...
  - Value Type:list of REG_SZ
  #### Example value: 
```
SOFTWARE\Policies\Microsoft\Edge\DefaultSearchProviderEncodings\0 = "UTF-8"
SOFTWARE\Policies\Microsoft\Edge\DefaultSearchProviderEncodings\1 = "UTF-16"
SOFTWARE\Policies\Microsoft\Edge\DefaultSearchProviderEncodings\2 = "GB2312"
SOFTWARE\Policies\Microsoft\Edge\DefaultSearchProviderEncodings\3 = "ISO-8859-1"

```


  ### Mac information and settings
  - Preference Key Name: DefaultSearchProviderEncodings
  - Example value: 
```
<array>
  <string>UTF-8</string>
  <string>UTF-16</string>
  <string>GB2312</string>
  <string>ISO-8859-1</string>
</array>

```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Specifies the search-by-image feature for the default search provider (DefaultSearchProviderImageURL)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Specifies the URL to the search engine used for image search. Search requests are sent using the GET method.

This policy is optional. If you don't configure it, image search isn't available.

This policy is applied only if you enable the 'DefaultSearchProviderEnabled' and 'DefaultSearchProviderSearchURL' policies.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  String

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: DefaultSearchProviderImageURL
  - GP name: Specifies the search-by-image feature for the default search provider
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Default search provider
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:DefaultSearchProviderImageURL
  - Value Type:REG_SZ
  #### Example value: 
```
"https://search.contoso.com/searchbyimage/upload"
```


  ### Mac information and settings
  - Preference Key Name: DefaultSearchProviderImageURL
  - Example value: 
```
"https://search.contoso.com/searchbyimage/upload"
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Parameters for an image URL that uses POST (DefaultSearchProviderImageURLPostParams)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  If you enable this policy, it specifies the parameters used when an image search that uses POST is performed. The policy consists of comma-separated name/value pairs. If a value is a template parameter, like {imageThumbnail} in the preceding example, it’s replaced with real image thumbnail data. This policy is applied only if you enable the 'DefaultSearchProviderEnabled' and 'DefaultSearchProviderSearchURL' policies.

If you don’t set this policy, image search requests are sent using the GET method.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  String

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: DefaultSearchProviderImageURLPostParams
  - GP name: Parameters for an image URL that uses POST
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Default search provider
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:DefaultSearchProviderImageURLPostParams
  - Value Type:REG_SZ
  #### Example value: 
```
"content={imageThumbnail},url={imageURL},sbisrc={SearchSource}"
```


  ### Mac information and settings
  - Preference Key Name: DefaultSearchProviderImageURLPostParams
  - Example value: 
```
"content={imageThumbnail},url={imageURL},sbisrc={SearchSource}"
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Default search provider keyword (DefaultSearchProviderKeyword)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Specifies the keyword, which is the shortcut used in the Address Bar to trigger the search for this provider.

This policy is optional. If you don't configure it, no keyword activates the search provider.

This policy is applied only if you enable the 'DefaultSearchProviderEnabled' and 'DefaultSearchProviderSearchURL' policies.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  String

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: DefaultSearchProviderKeyword
  - GP name: Default search provider keyword
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Default search provider
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:DefaultSearchProviderKeyword
  - Value Type:REG_SZ
  #### Example value: 
```
"mis"
```


  ### Mac information and settings
  - Preference Key Name: DefaultSearchProviderKeyword
  - Example value: 
```
"mis"
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Default search provider name (DefaultSearchProviderName)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Specifies the name of the default search provider.

If you enable this policy, you set the name of the default search provider.

If you don't enable this policy or if you leave it empty, the host name specified by the search URL is used.

'DefaultSearchProviderName' should be set to an organization-approved encrypted search provider that corresponds to the encrypted search provider set in DTBC-0008. This policy is applied only if you enable the 'DefaultSearchProviderEnabled' and 'DefaultSearchProviderSearchURL' policies.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  String

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: DefaultSearchProviderName
  - GP name: Default search provider name
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Default search provider
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:DefaultSearchProviderName
  - Value Type:REG_SZ
  #### Example value: 
```
"My Intranet Search"
```


  ### Mac information and settings
  - Preference Key Name: DefaultSearchProviderName
  - Example value: 
```
"My Intranet Search"
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Default search provider search URL (DefaultSearchProviderSearchURL)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Specifies the URL of the search engine used for a default search. The URL contains the string '{searchTerms}', which is replaced at query time by the terms the user is searching for.

Specify Bing's search URL as:

'{bing:baseURL}search?q={searchTerms}'.

Specify Google's search URL as: '{google:baseURL}search?q={searchTerms}&{google:RLZ}{google:originalQueryForSuggestion}{google:assistedQueryStats}{google:searchFieldtrialParameter}{google:searchClient}{google:sourceId}ie={inputEncoding}'.

This policy is required when you enable the 'DefaultSearchProviderEnabled' policy; if you don't enable the latter policy, this policy is ignored.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  String

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: DefaultSearchProviderSearchURL
  - GP name: Default search provider search URL
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Default search provider
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:DefaultSearchProviderSearchURL
  - Value Type:REG_SZ
  #### Example value: 
```
"https://search.contoso.com/search?q={searchTerms}"
```


  ### Mac information and settings
  - Preference Key Name: DefaultSearchProviderSearchURL
  - Example value: 
```
"https://search.contoso.com/search?q={searchTerms}"
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Default search provider URL for suggestions (DefaultSearchProviderSuggestURL)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Specifies the URL for the search engine used to provide search suggestions. The URL contains the string '{searchTerms}', which is replaced at query time by the text the user has entered so far.

This policy is optional. If you don't configure it, users won't see search suggestions; they will see suggestions from their browsing history and favorites.

Bing's suggest URL can be specified as:

'{bing:baseURL}qbox?query={searchTerms}'.

Google's suggest URL can be specified as: '{google:baseURL}complete/search?output=chrome&q={searchTerms}'.

This policy is applied only if you enable the 'DefaultSearchProviderEnabled' and 'DefaultSearchProviderSearchURL' policies.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  String

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: DefaultSearchProviderSuggestURL
  - GP name: Default search provider URL for suggestions
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Default search provider
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:DefaultSearchProviderSuggestURL
  - Value Type:REG_SZ
  #### Example value: 
```
"https://search.contoso.com/suggest?q={searchTerms}"
```


  ### Mac information and settings
  - Preference Key Name: DefaultSearchProviderSuggestURL
  - Example value: 
```
"https://search.contoso.com/suggest?q={searchTerms}"
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Configure allowed extension types (ExtensionAllowedTypes)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Controls which extension types can be installed and limits runtime access.

This setting defines the allowed types of extensions and which hosts they can interact with. The value is a list of strings, each of which should be one of the following: "extension", "theme", "user_script", and "hosted_app". See the Microsoft Edge extensions documentation for more information on these types.

Note that this policy also affects extensions to be force-installed by using 'ExtensionInstallForcelist' policy.

If you enable this policy, only extensions that match a type in the list are installed.

If you don't configure this policy, no restrictions on the acceptable extension types are enforced.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  List of strings

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: ExtensionAllowedTypes
  - GP name: Configure allowed extension types
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Extensions
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge\ExtensionAllowedTypes
  - Path (Recommended):N/A
  - Value Name:1, 2, 3, ...
  - Value Type:list of REG_SZ
  #### Example value: 
```
SOFTWARE\Policies\Microsoft\Edge\ExtensionAllowedTypes\0 = "hosted_app"

```


  ### Mac information and settings
  - Preference Key Name: ExtensionAllowedTypes
  - Example value: 
```
<array>
  <string>hosted_app</string>
</array>

```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Allow specific extensions to be installed (ExtensionInstallAllowlist)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  By default, all extensions are allowed. However, if you block all extensions by setting the 'ExtensionInstallBlockList' policy to "*," users can only install extensions defined in this policy.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  List of strings

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: ExtensionInstallAllowlist
  - GP name: Allow specific extensions to be installed
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Extensions
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallAllowlist
  - Path (Recommended):N/A
  - Value Name:1, 2, 3, ...
  - Value Type:list of REG_SZ
  #### Example value: 
```
SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallAllowlist\0 = "extension_id1"
SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallAllowlist\1 = "extension_id2"

```


  ### Mac information and settings
  - Preference Key Name: ExtensionInstallAllowlist
  - Example value: 
```
<array>
  <string>extension_id1</string>
  <string>extension_id2</string>
</array>

```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Control which extensions cannot be installed (ExtensionInstallBlocklist)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  List specific extensions that users can NOT install in Microsoft Edge. When you deploy this policy, any extensions on this list that were previously installed will be disabled, and the user won't be able to enable them. If you remove an item from the list of blocked extensions, that extension is automatically re-enabled anywhere it was previously installed.

Use "*" to block all extensions that aren't explicitly listed in the allow list.

If you don't configure this policy, users can install any extension in Microsoft Edge.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  List of strings

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: ExtensionInstallBlocklist
  - GP name: Control which extensions cannot be installed
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Extensions
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallBlocklist
  - Path (Recommended):N/A
  - Value Name:1, 2, 3, ...
  - Value Type:list of REG_SZ
  #### Example value: 
```
SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallBlocklist\0 = "extension_id1"
SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallBlocklist\1 = "extension_id2"

```


  ### Mac information and settings
  - Preference Key Name: ExtensionInstallBlocklist
  - Example value: 
```
<array>
  <string>extension_id1</string>
  <string>extension_id2</string>
</array>

```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Control which extensions are installed silently (ExtensionInstallForcelist)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Specifies extensions that are installed silently, without user interaction, and that the users can't uninstall or disable ("force-installed"). All permissions requested by the extensions are granted implicitly, without user interaction, including any additional permissions requested by future versions of the extension. Furthermore, permissions are granted for the enterprise.deviceAttributes and enterprise.platformKeys extension APIs. (These two APIs are only available to extensions that are force-installed.)

This policy takes precedence over a potentially conflicting 'ExtensionInstallBlocklist' policy. When you take an extension off of the force-installed list it's automatically uninstalled by Microsoft Edge.

For Windows devices that aren't joined to a Microsoft Active Directory domain, forced installation is limited to extensions available in the Microsoft Store.

Note that users can modify the source code of any extension by using Developer Tools, potentially rendering the extension dysfunctional. If this is a concern, set the 'DeveloperToolsAvailability' policy.

Use the following format to add an extension to the list:

[extensionID];[updateURL]

- extensionID - the 32-letter string found on edge://extensions when in developer mode.

- updateURL (optional) is the address of the Update Manifest XML document for the app or extension, as described at https://docs.microsoft.com/Placeholder07A. If you don't set the updateURL, the Microsoft Store update URL is used (currently https://extensionwebstorebase.edgesv.net/v1/crx).  Note that the update URL set in this policy is only used for the initial installation; subsequent updates of the extension use the update URL indicated in the extension's manifest.

For example, gggmmkjegpiggikcnhidnjjhmicpibll;https://extensionwebstorebase.edgesv.net/v1/crx installs the Microsoft Online app from the Microsoft Store "update" URL. For more information about hosting extensions, see: https://docs.microsoft.com//Placeholder03B.

If you don't configure this policy, no extensions are installed automatically, and users can uninstall any extension in Microsoft Edge.

Note that this policy doesn't apply to InPrivate mode.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  List of strings

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: ExtensionInstallForcelist
  - GP name: Control which extensions are installed silently
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Extensions
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallForcelist
  - Path (Recommended):N/A
  - Value Name:1, 2, 3, ...
  - Value Type:list of REG_SZ
  #### Example value: 
```
SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallForcelist\0 = "gbchcmhmhahfdphkhkmpfmihenigjmpp;https://extensionwebstorebase.edgesv.net/v1/crx"
SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallForcelist\1 = "abcdefghijklmnopabcdefghijklmnop"

```


  ### Mac information and settings
  - Preference Key Name: ExtensionInstallForcelist
  - Example value: 
```
<array>
  <string>gbchcmhmhahfdphkhkmpfmihenigjmpp;https://extensionwebstorebase.edgesv.net/v1/crx</string>
  <string>abcdefghijklmnopabcdefghijklmnop</string>
</array>

```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Configure extension and user script install sources (ExtensionInstallSources)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Define URLs that can install extensions and themes.

By default, users have to download a *.crx file for each extension or script they want to install, and then drag it onto the Microsoft Edge settings page. This policy lets specific URLs use install the extension or script for the user.

Each item in this list is an extension-style match pattern (see https://docs.microsoft.com//Placeholder04). Users can easily install items from any URL that matches an item in this list. Both the location of the *.crx file and the page where the download is started from (in other words, the referrer) must be allowed by these patterns.

The 'ExtensionInstallBlocklist' policy takes precedence over this policy. Any extensions that's on the block list won't be installed, even if it comes from a site on this list.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  List of strings

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: ExtensionInstallSources
  - GP name: Configure extension and user script install sources
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Extensions
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallSources
  - Path (Recommended):N/A
  - Value Name:1, 2, 3, ...
  - Value Type:list of REG_SZ
  #### Example value: 
```
SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallSources\0 = "https://corp.contoso.com/*"

```


  ### Mac information and settings
  - Preference Key Name: ExtensionInstallSources
  - Example value: 
```
<array>
  <string>https://corp.contoso.com/*</string>
</array>

```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Configure extension management settings (ExtensionSettings)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Configures extension management settings for Microsoft Edge.

This policy controls multiple settings, including settings controlled by any existing extension-related policies. This policy overrides any legacy policies if both are set.

This policy maps an extension ID or an update URL to its configuration. With an extension ID, the configuration is applied only to the specified extension. Set a default configuration for the special ID "*", to apply to all extensions that aren't specifically listed in this policy. With an update URL, the configuration is applied to all extensions with the exact update URL stated in manifest of this extension, as described at https://docs.microsoft.com/Placeholder07A.

For a full description of possible settings and structure of this policy go to https://docs.microsoft.com/Placeholder07B.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  Dictionary

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: ExtensionSettings
  - GP name: Configure extension management settings
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Extensions
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:ExtensionSettings
  - Value Type:REG_SZ
  #### Example value: 
```
SOFTWARE\Policies\Microsoft\Edge\ExtensionSettings = {
  "*": {
    "allowed_types": [
      "hosted_app"
    ], 
    "blocked_install_message": "Custom error message.", 
    "blocked_permissions": [
      "downloads", 
      "bookmarks"
    ], 
    "install_sources": [
      "https://company-intranet/apps"
    ], 
    "installation_mode": "blocked", 
    "runtime_allowed_hosts": [
      "*://good.contoso.com"
    ], 
    "runtime_blocked_hosts": [
      "*://*.contoso.com"
    ]
  }, 
  "abcdefghijklmnopabcdefghijklmnop": {
    "blocked_permissions": [
      "history"
    ], 
    "installation_mode": "allowed", 
    "minimum_version_required": "1.0.1"
  }, 
  "bcdefghijklmnopabcdefghijklmnopa": {
    "allowed_permissions": [
      "downloads"
    ], 
    "installation_mode": "force_installed", 
    "runtime_allowed_hosts": [
      "*://good.contoso.com"
    ], 
    "runtime_blocked_hosts": [
      "*://*.contoso.com"
    ], 
    "update_url": "https://contoso.com/update_url"
  }, 
  "cdefghijklmnopabcdefghijklmnopab": {
    "blocked_install_message": "Custom error message.", 
    "installation_mode": "blocked"
  }, 
  "defghijklmnopabcdefghijklmnopabc,efghijklmnopabcdefghijklmnopabcd": {
    "blocked_install_message": "Custom error message.", 
    "installation_mode": "blocked"
  }, 
  "fghijklmnopabcdefghijklmnopabcde": {
    "blocked_install_message": "Custom removal message.", 
    "installation_mode": "removed"
  }, 
  "update_url:https://www.contoso.com/update.xml": {
    "allowed_permissions": [
      "downloads"
    ], 
    "blocked_permissions": [
      "wallpaper"
    ], 
    "installation_mode": "allowed"
  }
}
```


  ### Mac information and settings
  - Preference Key Name: ExtensionSettings
  - Example value: 
```
<key>ExtensionSettings</key>
<dict>
  <key>*</key>
  <dict>
    <key>allowed_types</key>
    <array>
      <string>hosted_app</string>
    </array>
    <key>blocked_install_message</key>
    <string>Custom error message.</string>
    <key>blocked_permissions</key>
    <array>
      <string>downloads</string>
      <string>bookmarks</string>
    </array>
    <key>install_sources</key>
    <array>
      <string>https://company-intranet/apps</string>
    </array>
    <key>installation_mode</key>
    <string>blocked</string>
    <key>runtime_allowed_hosts</key>
    <array>
      <string>*://good.contoso.com</string>
    </array>
    <key>runtime_blocked_hosts</key>
    <array>
      <string>*://*.contoso.com</string>
    </array>
  </dict>
  <key>abcdefghijklmnopabcdefghijklmnop</key>
  <dict>
    <key>blocked_permissions</key>
    <array>
      <string>history</string>
    </array>
    <key>installation_mode</key>
    <string>allowed</string>
    <key>minimum_version_required</key>
    <string>1.0.1</string>
  </dict>
  <key>bcdefghijklmnopabcdefghijklmnopa</key>
  <dict>
    <key>allowed_permissions</key>
    <array>
      <string>downloads</string>
    </array>
    <key>installation_mode</key>
    <string>force_installed</string>
    <key>runtime_allowed_hosts</key>
    <array>
      <string>*://good.contoso.com</string>
    </array>
    <key>runtime_blocked_hosts</key>
    <array>
      <string>*://*.contoso.com</string>
    </array>
    <key>update_url</key>
    <string>https://contoso.com/update_url</string>
  </dict>
  <key>cdefghijklmnopabcdefghijklmnopab</key>
  <dict>
    <key>blocked_install_message</key>
    <string>Custom error message.</string>
    <key>installation_mode</key>
    <string>blocked</string>
  </dict>
  <key>defghijklmnopabcdefghijklmnopabc,efghijklmnopabcdefghijklmnopabcd</key>
  <dict>
    <key>blocked_install_message</key>
    <string>Custom error message.</string>
    <key>installation_mode</key>
    <string>blocked</string>
  </dict>
  <key>fghijklmnopabcdefghijklmnopabcde</key>
  <dict>
    <key>blocked_install_message</key>
    <string>Custom removal message.</string>
    <key>installation_mode</key>
    <string>removed</string>
  </dict>
  <key>update_url:https://www.contoso.com/update.xml</key>
  <dict>
    <key>allowed_permissions</key>
    <array>
      <string>downloads</string>
    </array>
    <key>blocked_permissions</key>
    <array>
      <string>wallpaper</string>
    </array>
    <key>installation_mode</key>
    <string>allowed</string>
  </dict>
</dict>
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Enable Google Cast (EnableMediaRouter)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Enable this policy to enable Google Cast. Users will be able to launch it from the app menu, page context menus, media controls on Cast-enabled websites, and (if shown) the Cast toolbar icon.

Disable this policy to disable Google Cast.

By default, Google Cast is enabled.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: No - Requires browser restart

  ### Data Type:
  Boolean

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: EnableMediaRouter
  - GP name: Enable Google Cast
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Cast
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:EnableMediaRouter
  - Value Type:REG_DWORD
  #### Example value: 
```
True
```


  ### Mac information and settings
  - Preference Key Name: EnableMediaRouter
  - Example value: 
```
True
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Show the cast icon in the toolbar (ShowCastIconInToolbar)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Set this policy to true to show the Cast toolbar icon on the toolbar or the overflow menu. Users won't be able to remove it.

If you don't configure this policy or if you disable it, users can pin or remove the icon by using its contextual menu.

If you've also set the "EnableMediaRouter" policy to false, then this policy is ignored, and the toolbar icon isn't shown.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: No - Requires browser restart

  ### Data Type:
  Boolean

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: ShowCastIconInToolbar
  - GP name: Show the cast icon in the toolbar
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Cast
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:ShowCastIconInToolbar
  - Value Type:REG_DWORD
  #### Example value: 
```
False
```


  ### Mac information and settings
  - Preference Key Name: ShowCastIconInToolbar
  - Example value: 
```
False
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Allow cross-origin HTTP Basic Auth prompts (AllowCrossOriginAuthPrompt)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Controls whether third-party sub-content on a page can open an HTTP Basic Auth dialog box.

Typically, this is disabled as a phishing defense. If you don't configure this policy, it's disabled and third-party sub-content can't open a HTTP Basic Auth dialog box.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  Boolean

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: AllowCrossOriginAuthPrompt
  - GP name: Allow cross-origin HTTP Basic Auth prompts
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/HTTP authentication
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:AllowCrossOriginAuthPrompt
  - Value Type:REG_DWORD
  #### Example value: 
```
False
```


  ### Mac information and settings
  - Preference Key Name: AllowCrossOriginAuthPrompt
  - Example value: 
```
False
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Specifies a list of servers that Microsoft Edge can delegate user credentials to (AuthNegotiateDelegateAllowlist)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Configure the list of servers that Microsoft Edge can delegate to.

Separate multiple server names with commas. Wildcards (*) are allowed.

If you don't configure this policy Microsoft Edge won't delegate user credentials even if a server is detected as Intranet.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: No - Requires browser restart

  ### Data Type:
  String

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: AuthNegotiateDelegateAllowlist
  - GP name: Specifies a list of servers that Microsoft Edge can delegate user credentials to
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/HTTP authentication
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:AuthNegotiateDelegateAllowlist
  - Value Type:REG_SZ
  #### Example value: 
```
"contoso.com"
```


  ### Mac information and settings
  - Preference Key Name: AuthNegotiateDelegateAllowlist
  - Example value: 
```
"contoso.com"
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Supported authentication schemes (AuthSchemes)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Specifies which HTTP authentication schemes are supported.

You can configure the policy by using these values: 'basic', 'digest', 'ntlm', and 'negotiate'. Separate multiple values with commas.

If you don't configure this policy, all four schemes are used.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: No - Requires browser restart

  ### Data Type:
  String

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: AuthSchemes
  - GP name: Supported authentication schemes
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/HTTP authentication
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:AuthSchemes
  - Value Type:REG_SZ
  #### Example value: 
```
"basic,digest,ntlm,negotiate"
```


  ### Mac information and settings
  - Preference Key Name: AuthSchemes
  - Example value: 
```
"basic,digest,ntlm,negotiate"
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Configure list of allowed authentication servers (AuthServerAllowlist)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Specifies which servers to enable for integrated authentication. Integrated authentication is only enabled when Microsoft Edge receives an authentication challenge from a proxy or from a server in this list.

Separate multiple server names with commas. Wildcards (*) are allowed.

If you don't configure this policy, Microsoft Edge tries to detect if a server is on the intranet - only then will it respond to IWA requests. If the server is on the internet, IWA requests from it are ignored by Microsoft Edge.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: No - Requires browser restart

  ### Data Type:
  String

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: AuthServerAllowlist
  - GP name: Configure list of allowed authentication servers
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/HTTP authentication
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:AuthServerAllowlist
  - Value Type:REG_SZ
  #### Example value: 
```
"*contoso.com,fabrikam.com,*baz"
```


  ### Mac information and settings
  - Preference Key Name: AuthServerAllowlist
  - Example value: 
```
"*contoso.com,fabrikam.com,*baz"
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Disable CNAME lookup when negotiating Kerberos authentication (DisableAuthNegotiateCnameLookup)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Determines whether the generated Kerberos SPN is based on the canonical DNS name (CNAME) or on the original name entered.

If you enable this policy, CNAME lookup is skipped and the server name (as entered) is used.

If you disable this policy or don't configure it, the canonical name of the server is used.  This is determined through CNAME lookup.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: No - Requires browser restart

  ### Data Type:
  Boolean

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: DisableAuthNegotiateCnameLookup
  - GP name: Disable CNAME lookup when negotiating Kerberos authentication
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/HTTP authentication
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:DisableAuthNegotiateCnameLookup
  - Value Type:REG_DWORD
  #### Example value: 
```
False
```


  ### Mac information and settings
  - Preference Key Name: DisableAuthNegotiateCnameLookup
  - Example value: 
```
False
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Include non-standard port in Kerberos SPN (EnableAuthNegotiatePort)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Specifies whether the generated Kerberos SPN should include a non-standard port.

If you enable this policy, and a user includes a non-standard port (a port other than 80 or 443) in a URL, that port is included in the generated Kerberos SPN.

If you don't configure or disable this policy, the generated Kerberos SPN won't include a port in any case.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: No - Requires browser restart

  ### Data Type:
  Boolean

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: EnableAuthNegotiatePort
  - GP name: Include non-standard port in Kerberos SPN
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/HTTP authentication
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:EnableAuthNegotiatePort
  - Value Type:REG_DWORD
  #### Example value: 
```
False
```


  ### Mac information and settings
  - Preference Key Name: EnableAuthNegotiatePort
  - Example value: 
```
False
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Control whether NTLMv2 authentication is enabled (NtlmV2Enabled)
  >Supported Versions: Microsoft Edge on Mac since version 77 or later
  

  ### Description
  Controls whether NTLMv2 is enabled.

All recent versions of Samba and Windows servers support NTLMv2. You should only disable NTLMv2 to address issues with backwards compatibility as it reduces the security of authentication.

If you don't configure this policy, NTLMv2 is enabled by default.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  Boolean

  

  ### Mac information and settings
  - Preference Key Name: NtlmV2Enabled
  - Example value: 
```
True
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Control which native messaging hosts users can use (NativeMessagingAllowlist)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  List specific native messaging hosts that users can use in Microsoft Edge.

By default, all native messaging hosts are allowed. If you set the 'NativeMessagingBlocklist' policy to *, all native messaging hosts are blocked, and only native messaging hosts listed in here are loaded.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  List of strings

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: NativeMessagingAllowlist
  - GP name: Control which native messaging hosts users can use
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Native Messaging
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge\NativeMessagingAllowlist
  - Path (Recommended):N/A
  - Value Name:1, 2, 3, ...
  - Value Type:list of REG_SZ
  #### Example value: 
```
SOFTWARE\Policies\Microsoft\Edge\NativeMessagingAllowlist\0 = "com.native.messaging.host.name1"
SOFTWARE\Policies\Microsoft\Edge\NativeMessagingAllowlist\1 = "com.native.messaging.host.name2"

```


  ### Mac information and settings
  - Preference Key Name: NativeMessagingAllowlist
  - Example value: 
```
<array>
  <string>com.native.messaging.host.name1</string>
  <string>com.native.messaging.host.name2</string>
</array>

```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Configure native messaging block list (NativeMessagingBlocklist)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Specifies which native messaging hosts that shouldn't be used.

Use '*' to block all native messaging hosts unless they are explicitly listed in the allow list.

If you don't configure this policy, Microsoft Edge will load all installed native messaging hosts.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  List of strings

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: NativeMessagingBlocklist
  - GP name: Configure native messaging block list
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Native Messaging
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge\NativeMessagingBlocklist
  - Path (Recommended):N/A
  - Value Name:1, 2, 3, ...
  - Value Type:list of REG_SZ
  #### Example value: 
```
SOFTWARE\Policies\Microsoft\Edge\NativeMessagingBlocklist\0 = "com.native.messaging.host.name1"
SOFTWARE\Policies\Microsoft\Edge\NativeMessagingBlocklist\1 = "com.native.messaging.host.name2"

```


  ### Mac information and settings
  - Preference Key Name: NativeMessagingBlocklist
  - Example value: 
```
<array>
  <string>com.native.messaging.host.name1</string>
  <string>com.native.messaging.host.name2</string>
</array>

```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Allow user-level native messaging hosts (installed without admin permissions) (NativeMessagingUserLevelHosts)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Enables user-level installation of native messaging hosts.

If you disable this policy, Microsoft Edge will only use native messaging hosts installed on the system level.

By default, if you don't configure this policy, Microsoft Edge will allow usage of user-level native messaging hosts.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  Boolean

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: NativeMessagingUserLevelHosts
  - GP name: Allow user-level native messaging hosts (installed without admin permissions)
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Native Messaging
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:NativeMessagingUserLevelHosts
  - Value Type:REG_DWORD
  #### Example value: 
```
False
```


  ### Mac information and settings
  - Preference Key Name: NativeMessagingUserLevelHosts
  - Example value: 
```
False
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Enable saving passwords to the password manager (PasswordManagerEnabled)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Enable Microsoft Edge to save user passwords.

If you enable this policy, users can save their passwords in Microsoft Edge. The next time they visit the site, Microsoft Edge will enter the password automatically.

If you disable this policy, users can't save new passwords, but they can still use previously saved passwords.

If you enable or disable this policy, users can't change or override it in Microsoft Edge. If you don't configure it, users can save passwords, as well as turn this feature off.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: Yes
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  Boolean

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: PasswordManagerEnabled
  - GP name: Enable saving passwords to the password manager
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Password manager and protection
  - GP path (Recommended): Administrative Templates/Microsoft Edge - Default Settings (users can override)/Password manager and protection
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): SOFTWARE\Policies\Microsoft\Edge\Recommended
  - Value Name:PasswordManagerEnabled
  - Value Type:REG_DWORD
  #### Example value: 
```
True
```


  ### Mac information and settings
  - Preference Key Name: PasswordManagerEnabled
  - Example value: 
```
True
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Configure the change password URL (PasswordProtectionChangePasswordURL)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Configures the change password URL (HTTP and HTTPS schemes only).

Password protection service will send users to this URL to change their password after seeing a warning in the browser. In order for Microsoft Edge to correctly capture the new password fingerprint on your change password page, make sure it follows the guidelines on https://docs.microsoft.com/Placeholder10.

If you enable this policy, then password protection service sends users to this URL to change their password.

If you disable this policy or don't configure it, then password protection service will not redirect users to a change password URL.

This policy is available only on Windows instances that are joined to a Microsoft Active Directory domain or Windows 10 Pro or Enterprise instances that are enrolled for device management.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  String

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: PasswordProtectionChangePasswordURL
  - GP name: Configure the change password URL
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Password manager and protection
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:PasswordProtectionChangePasswordURL
  - Value Type:REG_SZ
  #### Example value: 
```
"https://contoso.com/change_password.html"
```


  ### Mac information and settings
  - Preference Key Name: PasswordProtectionChangePasswordURL
  - Example value: 
```
"https://contoso.com/change_password.html"
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Configure the list of enterprise login URLs where password protection service should capture fingerprint of password (PasswordProtectionLoginURLs)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Configure the list of enterprise login URLs (HTTP and HTTPS schemes only) where Microsoft Edge should capture the fingerprint of passwords and use it for password reuse detection. In order for Microsoft Edge to correctly capture password fingerprints, make sure your login pages follow the guidelines on https://docs.microsoft.com/Placeholder10.

If you enable this policy, the password protection service captures fingerprints of passwords on the defined URLs.

If you disable this policy or don't configure it, no password fingerprints are captured.

This policy is available only on Windows instances that are joined to a Microsoft Active Directory domain or Windows 10 Pro or Enterprise instances that are enrolled for device management.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  List of strings

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: PasswordProtectionLoginURLs
  - GP name: Configure the list of enterprise login URLs where password protection service should capture fingerprint of password
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Password manager and protection
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge\PasswordProtectionLoginURLs
  - Path (Recommended):N/A
  - Value Name:1, 2, 3, ...
  - Value Type:list of REG_SZ
  #### Example value: 
```
SOFTWARE\Policies\Microsoft\Edge\PasswordProtectionLoginURLs\0 = "https://contoso.com/login.html"
SOFTWARE\Policies\Microsoft\Edge\PasswordProtectionLoginURLs\1 = "https://login.contoso.com"

```


  ### Mac information and settings
  - Preference Key Name: PasswordProtectionLoginURLs
  - Example value: 
```
<array>
  <string>https://contoso.com/login.html</string>
  <string>https://login.contoso.com</string>
</array>

```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Configure password protection warning trigger (PasswordProtectionWarningTrigger)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Allows you to control when to trigger password protection warning. Password protection alerts users when they reuse their protected password on potentially suspicious sites.

You can use the 'PasswordProtectionLoginURLs' and 'PasswordProtectionChangePasswordURL' policies to configure which passwords to protect.

Exemptions: Passwords for the sites listed in 'PasswordProtectionLoginURLs' and 'PasswordProtectionChangePasswordURL', as well as for the sites listed in 'SmartScreenAllowListDomains', will not trigger a password-protection warning.

Set to 'PasswordProtectionWarningOff' (0) to not show password protection warningss.

Set to 'PasswordProtectionWarningOnPasswordReuse' (1) to show password protection warnings when the user reuses their protected password on a non-whitelisted site.

If you disable or don't configure this policy, then the warning trigger is not shown.

* 0 = Password protection warning is off.

* 1 = Password protection warning is triggered by password reuse.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  Integer

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: PasswordProtectionWarningTrigger
  - GP name: Configure password protection warning trigger
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Password manager and protection
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:PasswordProtectionWarningTrigger
  - Value Type:REG_DWORD
  #### Example value: 
```
0x00000001
```


  ### Mac information and settings
  - Preference Key Name: PasswordProtectionWarningTrigger
  - Example value: 
```
1
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Default printer selection rules (DefaultPrinterSelection)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Overrides Microsoft Edge default printer selection rules. This policy determines the rules for selecting the default printer in Microsoft Edge, which happens the first time a user tries to print a page.

When this policy is set, Microsoft Edge tries to find a printer that matches all of the specified attributes and uses it as default printer. If there are multiple printers that meet the criteria, the first printer that matches is used.

If you don't configure this policy or no matching printers are found within the timeout, the printer defaults to the built-in PDF printer or no printer, if the PDF printer isn't available.

The value is parsed as a JSON object, conforming to the following schema: { "type": "object", "properties": { "idPattern": { "description": "Regular expression to match printer id.", "type": "string" }, "namePattern": { "description": "Regular expression to match printer display name.", "type": "string" } } }

Omitting a field means all values match; for example, if you don't specify connectivity Print Preview starts discovering all kinds of local printers. Regular expression patterns must follow the JavaScript RegExp syntax and matches are case sensitive.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  String

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: DefaultPrinterSelection
  - GP name: Default printer selection rules
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Printing
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:DefaultPrinterSelection
  - Value Type:REG_SZ
  #### Example value: 
```
"{ "idPattern": ".*public", "namePattern": ".*Color" }"
```


  ### Mac information and settings
  - Preference Key Name: DefaultPrinterSelection
  - Example value: 
```
"{ "idPattern": ".*public", "namePattern": ".*Color" }"
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Print headers and footers (PrintHeaderFooter)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Force 'headers and footers' to be on or off in the printing dialog.

If you don't configure this policy, users can decide whether to print headers and footers.

If you disable this policy, users can't print headers and footers.

If you enable this policy, users always print headers and footers.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: Yes
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  Boolean

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: PrintHeaderFooter
  - GP name: Print headers and footers
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Printing
  - GP path (Recommended): Administrative Templates/Microsoft Edge - Default Settings (users can override)/Printing
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): SOFTWARE\Policies\Microsoft\Edge\Recommended
  - Value Name:PrintHeaderFooter
  - Value Type:REG_DWORD
  #### Example value: 
```
False
```


  ### Mac information and settings
  - Preference Key Name: PrintHeaderFooter
  - Example value: 
```
False
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Set the system default printer as the default printer (PrintPreviewUseSystemDefaultPrinter)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Tells Microsoft Edge to use the system default printer as the default choice in Print Preview instead of the most recently used printer.

If you disable this policy or don't configure it, Print Preview uses the most recently used printer as the default destination choice.

If you enable this policy, Print Preview uses the OS system default printer as the default destination choice.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: Yes
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  Boolean

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: PrintPreviewUseSystemDefaultPrinter
  - GP name: Set the system default printer as the default printer
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Printing
  - GP path (Recommended): Administrative Templates/Microsoft Edge - Default Settings (users can override)/Printing
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): SOFTWARE\Policies\Microsoft\Edge\Recommended
  - Value Name:PrintPreviewUseSystemDefaultPrinter
  - Value Type:REG_DWORD
  #### Example value: 
```
False
```


  ### Mac information and settings
  - Preference Key Name: PrintPreviewUseSystemDefaultPrinter
  - Example value: 
```
False
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Enable printing (PrintingEnabled)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Enables printing in Microsoft Edge and prevents users from changing this setting.

If you enable this policy or don't configure it, users can print.

If you disable this policy, users can't print from Microsoft Edge. Printing is disabled in the wrench menu, extensions, JavaScript applications, and so on. Users can still print from plug-ins that bypass Microsoft Edge while printing. For example, certain Adobe Flash applications have the print option in their context menu, which isn't covered by this policy.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  Boolean

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: PrintingEnabled
  - GP name: Enable printing
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Printing
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:PrintingEnabled
  - Value Type:REG_DWORD
  #### Example value: 
```
True
```


  ### Mac information and settings
  - Preference Key Name: PrintingEnabled
  - Example value: 
```
True
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Print using system print dialog (UseSystemPrintDialog)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Shows the system print dialog instead of print preview.

If you enable this policy, Microsoft Edge opens the system print dialog instead of the built-in print preview when a user prints a page.

If you don't configure or disable this policy, print commands trigger the Microsoft Edge print preview screen.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: No - Requires browser restart

  ### Data Type:
  Boolean

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: UseSystemPrintDialog
  - GP name: Print using system print dialog
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Printing
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:UseSystemPrintDialog
  - Value Type:REG_DWORD
  #### Example value: 
```
False
```


  ### Mac information and settings
  - Preference Key Name: UseSystemPrintDialog
  - Example value: 
```
False
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Configure proxy bypass rules (ProxyBypassList)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Defines a list of hosts for which Microsoft Edge bypasses any proxy.

This policy is applied only if you have selected 'Use fixed proxy servers' in the 'ProxyMode' policy. If you selected any other mode for configuring proxy policies, don't enable or configure this policy.

If you enable this policy, you can create a list of hosts for which Microsoft Edge doesn't use a proxy.

If you don't configure this policy, no list of hosts is created for which Microsoft Edge bypasses a proxy. Leave this policy unconfigured if you've specified any other method for setting proxy policies.

For more detailed examples go to https://docs.microsoft.com/Placeholder05.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  String

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: ProxyBypassList
  - GP name: Configure proxy bypass rules
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Proxy server
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:ProxyBypassList
  - Value Type:REG_SZ
  #### Example value: 
```
"https://www.contoso.com, https://www.fabrikam.com"
```


  ### Mac information and settings
  - Preference Key Name: ProxyBypassList
  - Example value: 
```
"https://www.contoso.com, https://www.fabrikam.com"
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Configure proxy server settings (ProxyMode)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Specify the proxy server settings used by Microsoft Edge. If you enable this policy, users can't change the proxy settings.

If you choose to never use a proxy server and to always connect directly, all other options are ignored.

If you choose to use system proxy settings, all other options are ignored.

If you choose to auto detect the proxy server, all other options are ignored.

If you choose fixed server proxy mode, you can specify further options in 'ProxyServer' and 'Comma-separated list of proxy bypass rules'.

If you choose to use a .pac proxy script, you must specify the URL to the script in 'URL to a proxy .pac file'.

For detailed examples, go to https://docs.microsoft.com/Placeholder05.

If you enable this policy, Microsoft Edge will ignore all proxy-related options specified from the command line.

If you don't configure this policy users can choose their own proxy settings.

* "direct" = Never use a proxy

* "auto_detect" = Auto detect proxy settings

* "pac_script" = Use a .pac proxy script

* "fixed_servers" = Use fixed proxy servers

* "system" = Use system proxy settings

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  String

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: ProxyMode
  - GP name: Configure proxy server settings
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Proxy server
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:ProxyMode
  - Value Type:REG_SZ
  #### Example value: 
```
"direct"
```


  ### Mac information and settings
  - Preference Key Name: ProxyMode
  - Example value: 
```
"direct"
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Set the proxy .pac file URL (ProxyPacUrl)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Specifies the URL for a proxy auto-config (PAC) file.

This policy is applied only if you selected 'Use a .pac proxy script' in the 'ProxyMode' policy. If you selected any other mode for configuring proxy policies, don't enable or configure this policy.

If you enable this policy, you can specify the URL for a PAC file, which defines how the browser automatically chooses the appropriate proxy server for fetching a particular website.

If you disable or don't configure this policy, no PAC file is specified. Leave this policy unconfigured if you've specified any other method for setting proxy policies.

For detailed examples, see https://docs.microsoft.com/Placeholder05.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  String

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: ProxyPacUrl
  - GP name: Set the proxy .pac file URL
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Proxy server
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:ProxyPacUrl
  - Value Type:REG_SZ
  #### Example value: 
```
"https://internal.contoso.com/example.pac"
```


  ### Mac information and settings
  - Preference Key Name: ProxyPacUrl
  - Example value: 
```
"https://internal.contoso.com/example.pac"
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Configure address or URL of proxy server (ProxyServer)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Specifies the URL of the proxy server.

This policy is applied only if you have selected 'Use fixed proxy servers' in the 'ProxyMode' policy. If you selected any other mode for configuring proxy policies, don't enable or configure this policy.

If you enable this policy, the proxy server configured by this policy will be used for all URLs.

If you disable or don't configure this policy, users can choose their own proxy settings while in this proxy mode. Leave this policy unconfigured if you've specified any other method for setting proxy policies.

For more options and detailed examples, see https://docs.microsoft.com/Placeholder05.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  String

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: ProxyServer
  - GP name: Configure address or URL of proxy server
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Proxy server
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:ProxyServer
  - Value Type:REG_SZ
  #### Example value: 
```
"123.123.123.123:8080"
```


  ### Mac information and settings
  - Preference Key Name: ProxyServer
  - Example value: 
```
"123.123.123.123:8080"
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Proxy settings (ProxySettings)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Configures the proxy settings for Microsoft Edge.

If you enable this policy, Microsoft Edge ignores all proxy-related options specified from the command line.

If you don't configure this policy, users can choose their own proxy settings.

This policy overrides the following individual policies:

ProxyMode
ProxyPacUrl
ProxyServer
ProxyBypassList

The ProxyMode field lets you specify the proxy server used by Microsoft Edge and prevents users from changing proxy settings.

The ProxyPacUrl field is a URL to a proxy .pac file.

The ProxyServer field is a URL for the proxy server.

The ProxyBypassList field is a list of proxy hosts that Microsoft Edge bypasses.

If you choose the 'direct' value as 'ProxyMode', a proxy is never used and all other fields are ignored.

If you choose the 'system' value as 'ProxyMode', the systems's proxy is used and all other fields are ignored.

If you choose the 'auto_detect' value as 'ProxyMode', all other fields are ignored.

If you choose the 'fixed_server' value as 'ProxyMode', the 'ProxyServer' and 'ProxyBypassList' fields are used.

If you choose the 'pac_script' value as 'ProxyMode', the 'ProxyPacUrl' and 'ProxyBypassList' fields are used.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  Dictionary

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: ProxySettings
  - GP name: Proxy settings
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Proxy server
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:ProxySettings
  - Value Type:REG_SZ
  #### Example value: 
```
SOFTWARE\Policies\Microsoft\Edge\ProxySettings = {
  "ProxyBypassList": "https://www.example1.com,https://www.example2.com,https://internalsite/", 
  "ProxyMode": "direct", 
  "ProxyPacUrl": "https://internal.site/example.pac", 
  "ProxyServer": "123.123.123.123:8080"
}
```


  ### Mac information and settings
  - Preference Key Name: ProxySettings
  - Example value: 
```
<key>ProxySettings</key>
<dict>
  <key>ProxyBypassList</key>
  <string>https://www.example1.com,https://www.example2.com,https://internalsite/</string>
  <key>ProxyMode</key>
  <string>direct</string>
  <key>ProxyPacUrl</key>
  <string>https://internal.site/example.pac</string>
  <key>ProxyServer</key>
  <string>123.123.123.123:8080</string>
</dict>
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Prevent bypassing Microsoft Defender SmartScreen prompts for sites (PreventSmartScreenPromptOverride)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  This policy setting lets you decide whether employees can override the Microsoft Defender SmartScreen warnings about potentially malicious websites.

If you enable this setting, employees can't ignore Microsoft Defender SmartScreen warnings and they are blocked from continuing to the site.

If you disable or don't configure this setting, employees can ignore Microsoft Defender SmartScreen warnings and continue to the site.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  Boolean

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: PreventSmartScreenPromptOverride
  - GP name: Prevent bypassing Microsoft Defender SmartScreen prompts for sites
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/SmartScreen settings
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:PreventSmartScreenPromptOverride
  - Value Type:REG_DWORD
  #### Example value: 
```
True
```


  ### Mac information and settings
  - Preference Key Name: PreventSmartScreenPromptOverride
  - Example value: 
```
True
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Prevent bypassing of Microsoft Defender SmartScreen warnings about downloads (PreventSmartScreenPromptOverrideForFiles)
  >Supported Versions: Microsoft Edge on Windows since version 77 or later
  

  ### Description
  This policy lets you determine whether users can override Microsoft Defender SmartScreen warnings about unverified downloads.

If you enable this policy, users in your organization can't ignore Microsoft Defender SmartScreen warnings, and they're prevented from completing the unverified downloads.

If you disable or don't configure this policy, users can ignore Microsoft Defender SmartScreen warnings and complete unverified downloads.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  Boolean

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: PreventSmartScreenPromptOverrideForFiles
  - GP name: Prevent bypassing of Microsoft Defender SmartScreen warnings about downloads
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/SmartScreen settings
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:PreventSmartScreenPromptOverrideForFiles
  - Value Type:REG_DWORD
  #### Example value: 
```
True
```


  

  [Back to Top](#Edge-Policy-Documentation)

  ## Configure the list of domains for which SmartScreen won't trigger warnings (SmartScreenAllowListDomains)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Configure the list of SmartScreen-trusted domains. This means:
SmartScreen won't check for potentially malicious resources like phishing software and other malware if the source URLs match these domains.
The SmartScreen download protection service won't check downloads hosted on these domains.

If you enable this policy, SmartScreen trusts these domains.
If you disable or don't set this policy, default SmartScreen protection is applied to all resources.
This policy is available only on Windows instances that are joined to a Microsoft Active Directory domain; or on Windows 10 Pro or Enterprise instances that are enrolled for device management.
Also note that this policy does not apply if your organization has enabled Microsoft Defender Advanced Threat Protection. You must configure your allow and block lists in Microsoft Defender Security Center instead.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  List of strings

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: SmartScreenAllowListDomains
  - GP name: Configure the list of domains for which SmartScreen won't trigger warnings
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/SmartScreen settings
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge\SmartScreenAllowListDomains
  - Path (Recommended):N/A
  - Value Name:1, 2, 3, ...
  - Value Type:list of REG_SZ
  #### Example value: 
```
SOFTWARE\Policies\Microsoft\Edge\SmartScreenAllowListDomains\0 = "mydomain.com"
SOFTWARE\Policies\Microsoft\Edge\SmartScreenAllowListDomains\1 = "myuniversity.edu"

```


  ### Mac information and settings
  - Preference Key Name: SmartScreenAllowListDomains
  - Example value: 
```
<array>
  <string>mydomain.com</string>
  <string>myuniversity.edu</string>
</array>

```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Configure Microsoft Defender SmartScreen (SmartScreenEnabled)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  This policy setting lets you configure whether to turn on Microsoft Defender SmartScreen. Microsoft Defender SmartScreen provides warning messages to help protect your employees from potential phishing scams and malicious software. By default, Microsoft Defender SmartScreen is turned on.

If you enable this setting, Microsoft Defender SmartScreen is turned on and employees can't turn it off.

If you disable this setting, Microsoft Defender SmartScreen is turned off and employees can't turn it on.

If you don't configure this setting, employees can choose whether to use Microsoft Defender SmartScreen.

This policy is available only on Windows instances that are joined to a Microsoft Active Director domain; or on Windows 10 Pro or Enterprise instances that are enrolled for device management.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: Yes
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  Boolean

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: SmartScreenEnabled
  - GP name: Configure Microsoft Defender SmartScreen
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/SmartScreen settings
  - GP path (Recommended): Administrative Templates/Microsoft Edge - Default Settings (users can override)/SmartScreen settings
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): SOFTWARE\Policies\Microsoft\Edge\Recommended
  - Value Name:SmartScreenEnabled
  - Value Type:REG_DWORD
  #### Example value: 
```
True
```


  ### Mac information and settings
  - Preference Key Name: SmartScreenEnabled
  - Example value: 
```
True
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Set the new tab page as the home page (HomepageIsNewTabPage)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Configures the default home page in Microsoft Edge. You can set the home page to a URL you specify or to the new tab page.

If you enable this policy, the new tab page is always used for the home page, and the home page URL location is ignored.

If you disable this policy, the user's home page can't be the new tab page, unless the URL is set to 'edge://newtab'.

If not configured users can choose whether the new tab page is their home page.

This policy is available only on Windows instances that are joined to a Microsoft Active Directory domain or Windows 10 Pro or Enterprise instances enrolled for device management.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: Yes
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  Boolean

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: HomepageIsNewTabPage
  - GP name: Set the new tab page as the home page
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Startup, home page and new tab page
  - GP path (Recommended): Administrative Templates/Microsoft Edge - Default Settings (users can override)/Startup, home page and new tab page
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): SOFTWARE\Policies\Microsoft\Edge\Recommended
  - Value Name:HomepageIsNewTabPage
  - Value Type:REG_DWORD
  #### Example value: 
```
True
```


  ### Mac information and settings
  - Preference Key Name: HomepageIsNewTabPage
  - Example value: 
```
True
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Configure the home page URL (HomepageLocation)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Configures the default home page URL in Microsoft Edge.

The home page is the page opened by the Home button. The pages that open on startup are controlled by the 'RestoreOnStartup' policies.

You can either set a URL here or set the home page to open the new tab page. If you select to open the new tab page, then this policy doesn't take effect.

If you enable this policy, users can't change their home page URL, but they can choose to use the new tab page as their home page.

If you disable or don't configure this policy, users can choose their own home page, as long as the 'HomepageIsNewTabPage' policy isn't enabled.

This policy is available only on Windows instances that are joined to a Microsoft Active Directory domain or Windows 10 Pro or Enterprise instances enrolled for device management.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: Yes
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  String

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: HomepageLocation
  - GP name: Configure the home page URL
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Startup, home page and new tab page
  - GP path (Recommended): Administrative Templates/Microsoft Edge - Default Settings (users can override)/Startup, home page and new tab page
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): SOFTWARE\Policies\Microsoft\Edge\Recommended
  - Value Name:HomepageLocation
  - Value Type:REG_SZ
  #### Example value: 
```
"https://www.contoso.com"
```


  ### Mac information and settings
  - Preference Key Name: HomepageLocation
  - Example value: 
```
"https://www.contoso.com"
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Hide the default top sites from the new tab page (NewTabPageHideDefaultTopSites)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Hides the default top sites from the new tab page in Microsoft Edge.

If you set this policy to true, the default top site tiles are hidden.

If you set this policy to false or don't configure it, the default top site tiles remain visible.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  Boolean

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: NewTabPageHideDefaultTopSites
  - GP name: Hide the default top sites from the new tab page
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Startup, home page and new tab page
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:NewTabPageHideDefaultTopSites
  - Value Type:REG_DWORD
  #### Example value: 
```
True
```


  ### Mac information and settings
  - Preference Key Name: NewTabPageHideDefaultTopSites
  - Example value: 
```
True
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Configure the new tab page URL (NewTabPageLocation)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Configures the default URL for the new tab page.

This policy determines the page that's opened when new tabs are created (including when new windows are opened). It also affects the startup page if that's set to open to the new tab page.

This policy doesn't determine which page opens on startup; that's controlled by the 'RestoreOnStartup' policy. It also doesn’t affect the home page if that’s set to open to the new tab page.

If you don't configure this policy, the default new tab page is used.

If you configure this policy *and* the 'NewTabPageSetFeedType' policy, this policy has precedence.

This policy is available only on Windows instances that are joined to a Microsoft Active Directory domain or Windows 10 Pro or Enterprise instances that are enrolled for device management.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: Yes
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  String

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: NewTabPageLocation
  - GP name: Configure the new tab page URL
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Startup, home page and new tab page
  - GP path (Recommended): Administrative Templates/Microsoft Edge - Default Settings (users can override)/Startup, home page and new tab page
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): SOFTWARE\Policies\Microsoft\Edge\Recommended
  - Value Name:NewTabPageLocation
  - Value Type:REG_SZ
  #### Example value: 
```
"https://www.fabrikam.com"
```


  ### Mac information and settings
  - Preference Key Name: NewTabPageLocation
  - Example value: 
```
"https://www.fabrikam.com"
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Action to take on startup (RestoreOnStartup)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Specify how Microsoft Edge behaves when it starts.

If you want a new tab to always open on startup, choose 'Open new tab' (5).

If you want to reopen URLs that were open the last time Microsoft Edge closed, choose 'Restore the last session' (1). The browsing session will be restored as it was. Note that this option disables some settings that rely on sessions or that perform actions on exit (such as Clear browsing data on exit or session-only cookies).

If you want to open a specific set of URLs, choose 'Open a list of URLs' (4).

Disabling this setting is equivalent to leaving it not configured. Users will be able to change it in Microsoft Edge.

This policy is available only on Windows instances that are joined to a Microsoft Active Directory domain or Windows 10 Pro or Enterprise instances enrolled for device management.

* 5 = Open a new tab

* 1 = Restore the last session

* 4 = Open a list of URLs

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: Yes
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  Integer

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: RestoreOnStartup
  - GP name: Action to take on startup
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Startup, home page and new tab page
  - GP path (Recommended): Administrative Templates/Microsoft Edge - Default Settings (users can override)/Startup, home page and new tab page
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): SOFTWARE\Policies\Microsoft\Edge\Recommended
  - Value Name:RestoreOnStartup
  - Value Type:REG_DWORD
  #### Example value: 
```
0x00000004
```


  ### Mac information and settings
  - Preference Key Name: RestoreOnStartup
  - Example value: 
```
4
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Sites to open when the browser starts (RestoreOnStartupURLs)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Specify a list of websites to open automatically when the browser starts. If you don't configure this policy, no site is opened on startup.

This policy only works if you also set the 'RestoreOnStartup' policy to 'Open a list of URLs' (4).

This policy is only available on Windows instances that are joined to a Microsoft Active Directory domain or Windows 10 Pro or Enterprise instances that are enrolled for device management.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: Yes
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  List of strings

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: RestoreOnStartupURLs
  - GP name: Sites to open when the browser starts
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Startup, home page and new tab page
  - GP path (Recommended): Administrative Templates/Microsoft Edge - Default Settings (users can override)/Startup, home page and new tab page
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge\RestoreOnStartupURLs
  - Path (Recommended): SOFTWARE\Policies\Microsoft\Edge\Recommended\RestoreOnStartupURLs
  - Value Name:1, 2, 3, ...
  - Value Type:list of REG_SZ
  #### Example value: 
```
SOFTWARE\Policies\Microsoft\Edge\RestoreOnStartupURLs\0 = "https://contoso.com"
SOFTWARE\Policies\Microsoft\Edge\RestoreOnStartupURLs\1 = "https://www.fabrikam.com"

```


  ### Mac information and settings
  - Preference Key Name: RestoreOnStartupURLs
  - Example value: 
```
<array>
  <string>https://contoso.com</string>
  <string>https://www.fabrikam.com</string>
</array>

```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Show Home button on toolbar (ShowHomeButton)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Shows the Home button on Microsoft Edge's toolbar.

Enable this policy to always show the Home button. Disable it to never show the button.

If you don't configure the policy, users can choose whether to show the home button.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: Yes
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  Boolean

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: ShowHomeButton
  - GP name: Show Home button on toolbar
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/Startup, home page and new tab page
  - GP path (Recommended): Administrative Templates/Microsoft Edge - Default Settings (users can override)/Startup, home page and new tab page
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): SOFTWARE\Policies\Microsoft\Edge\Recommended
  - Value Name:ShowHomeButton
  - Value Type:REG_DWORD
  #### Example value: 
```
True
```


  ### Mac information and settings
  - Preference Key Name: ShowHomeButton
  - Example value: 
```
True
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Enable deleting browser and download history (AllowDeletingBrowserHistory)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Enables deleting browser history and download history and prevents users from changing this setting.

Note that even with this policy is disabled, the browsing and download history aren't guaranteed to be retained: users can edit or delete the history database files directly, and the browser itself may remove (based on expiration period) or archive any or all history items at any time.

If you enable this policy or don't configure it, users can delete the browsing and download history.

If you disable this policy, users can't delete browsing and download history.

If you enable this policy, don't enable the 'Clear browsing data when Microsoft Edge closes' policy, because they both deal with deleting data. If you enable both, the 'Clear browsing data when Microsoft Edge closes' policy takes precedence and deletes all data when Microsoft Edge closes, regardless of how this policy is configured.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  Boolean

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: AllowDeletingBrowserHistory
  - GP name: Enable deleting browser and download history
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:AllowDeletingBrowserHistory
  - Value Type:REG_DWORD
  #### Example value: 
```
True
```


  ### Mac information and settings
  - Preference Key Name: AllowDeletingBrowserHistory
  - Example value: 
```
True
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Allow file selection dialogs (AllowFileSelectionDialogs)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Allow access to local files by letting Microsoft Edge display file selection dialogs.

If you enable or don't configure this policy, users can open file selection dialogs as normal.

If you disable this policy, whenever the user performs an action that triggers a file selection dialog (like importing favorites, uploading files, or saving links), a message is displayed instead, and the user is assumed to have clicked Cancel on the file selection dialog.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  Boolean

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: AllowFileSelectionDialogs
  - GP name: Allow file selection dialogs
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:AllowFileSelectionDialogs
  - Value Type:REG_DWORD
  #### Example value: 
```
True
```


  ### Mac information and settings
  - Preference Key Name: AllowFileSelectionDialogs
  - Example value: 
```
True
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Always open PDF files externally (AlwaysOpenPdfExternally)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Disables the internal PDF viewer in Microsoft Edge.

If you enable this policy Microsoft Edge treats PDF files as downloads and lets users open them with the default application.

If you don't configure this policy or disable it, Microsoft Edge will open PDF files (unless the user disables it).

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  Boolean

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: AlwaysOpenPdfExternally
  - GP name: Always open PDF files externally
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:AlwaysOpenPdfExternally
  - Value Type:REG_DWORD
  #### Example value: 
```
True
```


  ### Mac information and settings
  - Preference Key Name: AlwaysOpenPdfExternally
  - Example value: 
```
True
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Set application locale (ApplicationLocaleValue)
  >Supported Versions: Microsoft Edge on Windows since version 77 or later
  

  ### Description
  Configures the application locale in Microsoft Edge and prevents users from changing the locale.

If you enable this policy, Microsoft Edge uses the specified locale. If the configured locale isn't supported, 'en-US' is used instead.

If you disable or don't configure this setting, Microsoft Edge uses either the user-specified preferred locale (if configured) or the fallback locale 'en-US'.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: Yes
  - Dynamic Policy Refresh: No - Requires browser restart

  ### Data Type:
  String

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: ApplicationLocaleValue
  - GP name: Set application locale
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): Administrative Templates/Microsoft Edge - Default Settings (users can override)/
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): SOFTWARE\Policies\Microsoft\Edge\Recommended
  - Value Name:ApplicationLocaleValue
  - Value Type:REG_SZ
  #### Example value: 
```
"en"
```


  

  [Back to Top](#Edge-Policy-Documentation)

  ## Allow or block audio capture (AudioCaptureAllowed)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Allows you to set whether a user is prompted to grant a website access to their audio capture device. This policy applies to all URLs except for those configured in the 'AudioCaptureAllowedUrls' list.

If you enable this policy or don't configure it (the default setting), the user is prompted for audio capture access except from the URLs in the 'AudioCaptureAllowedUrls' list. These listed URLs are granted access without prompting.

If you disable this policy, the user is not prompted, and audio capture is accessible only to the URLs configured in 'AudioCaptureAllowedUrls'.

This policy affects all types of audio inputs, not only the built-in microphone.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  Boolean

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: AudioCaptureAllowed
  - GP name: Allow or block audio capture
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:AudioCaptureAllowed
  - Value Type:REG_DWORD
  #### Example value: 
```
False
```


  ### Mac information and settings
  - Preference Key Name: AudioCaptureAllowed
  - Example value: 
```
False
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Sites that can access audio capture devices without requesting permission (AudioCaptureAllowedUrls)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Specify websites, based on URL patterns, that can use audio capture devices without asking the user for permission. Patterns in this list are matched against the security origin of the requesting URL. If they match, the site is automatically granted access to audio capture devices.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  List of strings

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: AudioCaptureAllowedUrls
  - GP name: Sites that can access audio capture devices without requesting permission
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge\AudioCaptureAllowedUrls
  - Path (Recommended):N/A
  - Value Name:1, 2, 3, ...
  - Value Type:list of REG_SZ
  #### Example value: 
```
SOFTWARE\Policies\Microsoft\Edge\AudioCaptureAllowedUrls\0 = "https://www.contoso.com/"
SOFTWARE\Policies\Microsoft\Edge\AudioCaptureAllowedUrls\1 = "https://[*.]contoso.edu/"

```


  ### Mac information and settings
  - Preference Key Name: AudioCaptureAllowedUrls
  - Example value: 
```
<array>
  <string>https://www.contoso.com/</string>
  <string>https://[*.]contoso.edu/</string>
</array>

```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Automatically import another browser's data and settings at first run (AutoImportAtFirstRun)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  If you enable this policy, Microsoft Edge automatically imports all supported datatypes and settings from either the default browser or another specified browser. This also forces Microsoft Edge to skip the import section of the first-run experience.

If you set this policy to 'DisabledAutoImport' (4), the import section of the first-run experience is skipped entirely and Microsoft Edge doesn't import browser data and settings automatically.

* 0 = Automatically imports all supported datatypes and settings from the default browser

* 1 = Automatically imports all supported datatypes and settings from Internet Explorer

* 2 = Automatically imports all supported datatypes and settings from Google Chrome

* 3 = Automatically imports all supported datatypes and settings from Safari

* 4 = Disables automatic import, and the import section of the first-run experience is skipped

**Note**: This policy currently supports importing from Internet Explorer (on Windows 7, 8, and 10), Google Chrome (on Windows 7, 8, and 10 and on macOS) and Apple Safari (on macOS) browsers.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: No - Requires browser restart

  ### Data Type:
  Integer

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: AutoImportAtFirstRun
  - GP name: Automatically import another browser's data and settings at first run
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:AutoImportAtFirstRun
  - Value Type:REG_DWORD
  #### Example value: 
```
0x00000002
```


  ### Mac information and settings
  - Preference Key Name: AutoImportAtFirstRun
  - Example value: 
```
2
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Enable AutoFill for addresses (AutofillAddressEnabled)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Enables the AutoFill feature and allows users to auto-complete address information in web forms using previously stored information.

If you disable this policy, AutoFill never suggests or fills in address information, nor does it save additional address information that the user might submit while browsing the web.

If you enable this policy or don't configure it, users can control AutoFill for addresses in the user interface.

Note that if you disable this policy you also stop all activity for all web forms, except payment and password forms. No further entries are saved, and Microsoft Edge won't suggest or AutoFill any previous entries.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: Yes
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  Boolean

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: AutofillAddressEnabled
  - GP name: Enable AutoFill for addresses
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): Administrative Templates/Microsoft Edge - Default Settings (users can override)/
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): SOFTWARE\Policies\Microsoft\Edge\Recommended
  - Value Name:AutofillAddressEnabled
  - Value Type:REG_DWORD
  #### Example value: 
```
False
```


  ### Mac information and settings
  - Preference Key Name: AutofillAddressEnabled
  - Example value: 
```
False
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Enable AutoFill for credit cards (AutofillCreditCardEnabled)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Enables Microsoft Edge's AutoFill feature and lets users auto complete credit card information in web forms using previously stored information.

If you disable this policy, AutoFill never suggests or fills credit card information, nor will it save additional credit card information that users might submit while browsing the web.

If you enable this policy or don't configure it, users can control AutoFill for credit cards.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: Yes
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  Boolean

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: AutofillCreditCardEnabled
  - GP name: Enable AutoFill for credit cards
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): Administrative Templates/Microsoft Edge - Default Settings (users can override)/
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): SOFTWARE\Policies\Microsoft\Edge\Recommended
  - Value Name:AutofillCreditCardEnabled
  - Value Type:REG_DWORD
  #### Example value: 
```
False
```


  ### Mac information and settings
  - Preference Key Name: AutofillCreditCardEnabled
  - Example value: 
```
False
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Continue running background apps after Microsoft Edge closes (BackgroundModeEnabled)
  >Supported Versions: Microsoft Edge on Windows since version 77 or later
  

  ### Description
  Allows Microsoft Edge processes to start at OS sign-in and keep running after the last browser window is closed. In this scenario, background apps and the current browsing session remain active, including any session cookies. An open background process displays an icon in the system tray and can always be closed from there.

If you enable this policy, background mode is turned on.

If you disable this policy, background mode is turned off.

If you don't configure this policy, background mode is initially turned off, and the user can configure its behavior in edge://settings/system.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: Yes
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  Boolean

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: BackgroundModeEnabled
  - GP name: Continue running background apps after Microsoft Edge closes
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): Administrative Templates/Microsoft Edge - Default Settings (users can override)/
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): SOFTWARE\Policies\Microsoft\Edge\Recommended
  - Value Name:BackgroundModeEnabled
  - Value Type:REG_DWORD
  #### Example value: 
```
True
```


  

  [Back to Top](#Edge-Policy-Documentation)

  ## Block third party cookies (BlockThirdPartyCookies)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Block web page elements that aren't from the domain that's in the address bar from setting cookies.

If you enable this policy, web page elements that are not from the domain that is in the address bar can't set cookies

If you disable this policy, web page elements from domains other than in the address bar can set cookies.

If you don't configure this policy, third-party cookies are enabled but users can change this setting.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: Yes
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  Boolean

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: BlockThirdPartyCookies
  - GP name: Block third party cookies
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): Administrative Templates/Microsoft Edge - Default Settings (users can override)/
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): SOFTWARE\Policies\Microsoft\Edge\Recommended
  - Value Name:BlockThirdPartyCookies
  - Value Type:REG_DWORD
  #### Example value: 
```
False
```


  ### Mac information and settings
  - Preference Key Name: BlockThirdPartyCookies
  - Example value: 
```
False
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Enable profile creation from the Identity flyout menu or the Settings page (BrowserAddProfileEnabled)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Allows users to create new profiles, using the **Add profile** option.
If you enable this policy or don't configure it, Microsoft Edge allows users to use **Add profile** on the Identity flyout menu or the Settings page to create new profiles.

If you disable this policy, users cannot add new profiles from the Identity flyout menu or the Settings page.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  Boolean

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: BrowserAddProfileEnabled
  - GP name: Enable profile creation from the Identity flyout menu or the Settings page
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:BrowserAddProfileEnabled
  - Value Type:REG_DWORD
  #### Example value: 
```
True
```


  ### Mac information and settings
  - Preference Key Name: BrowserAddProfileEnabled
  - Example value: 
```
True
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Enable guest mode (BrowserGuestModeEnabled)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Enable the option to allow the use of guest profiles in Microsoft Edge. In a guest profile, the browser doesn't import browsing data from existing profiles, and it deletes browsing data when all guest profiles are closed.

If you enable this policy or don't configure it, Microsoft Edge lets users browse in guest profiles.

If you disable this policy, Microsoft Edge doesn't let users browse in guest profiles.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  Boolean

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: BrowserGuestModeEnabled
  - GP name: Enable guest mode
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:BrowserGuestModeEnabled
  - Value Type:REG_DWORD
  #### Example value: 
```
True
```


  ### Mac information and settings
  - Preference Key Name: BrowserGuestModeEnabled
  - Example value: 
```
True
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Allow queries to a Browser Network Time service (BrowserNetworkTimeQueriesEnabled)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Prevents Microsoft Edge from occasionally sending queries to a browser network time service to retrieve an accurate timestamp.

If you disable this policy, Microsoft Edge will stop sending queries to a browser network time service.

If you enable this policy or don't configure it, Microsoft Edge will occasionally send queries to a browser network time service.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  Boolean

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: BrowserNetworkTimeQueriesEnabled
  - GP name: Allow queries to a Browser Network Time service
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:BrowserNetworkTimeQueriesEnabled
  - Value Type:REG_DWORD
  #### Example value: 
```
True
```


  ### Mac information and settings
  - Preference Key Name: BrowserNetworkTimeQueriesEnabled
  - Example value: 
```
True
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Browser sign-in settings (BrowserSignin)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Specify whether a user can sign into Microsoft Edge with their account and use account-related services like sync and single sign on. To control the availability of sync, use the 'SyncDisabled' policy.

If you set this policy to 'Disable browser sign-in' (0), users can't sign into the browser and use account-based services. In this case users can't use browser-level features like sync - they're unavailable. If a user was signed in when you set the policy to "Disabled," they'll be signed out the next time they run Microsoft Edge, but their local profile data (like favorites and passwords) are preserved. The user can still sign into and use Microsoft web properties like bing.com and Office.com.

If you set this policy to 'Enable browser sign-in' (1), users can sign into the browser. Signing in to the browser means the user's account information is kept by the browser, but it doesn't mean that sync is turned on by default; the user must separately opt-in to use this feature. Enabling this policy prevents users from turning off the setting that allows browser sign-in.

If you set this policy to 'Force browser sign-in" (2) users have to sign into a profile to use the browser. This ensures that the policies associated with a managed account are applied and enforced. By default, this turns on sync for the account, unless sync is disabled by the domain admin or with the 'SyncDisabled' policy. The default value of 'BrowserGuestModeEnabled' policy is set to false. Note that existing unsigned profiles will be locked and inaccessible after you enable this policy. For more information, see help center article: https://docs.microsoft.com/Placeholder12.

If you don't configure this policy users can decide if they want to enable the browser sign-in option and use it as they see fit.

* 0 = Disable browser sign-in

* 1 = Enable browser sign-in

* 2 = Force users to sign-in to use the browser

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: No - Requires browser restart

  ### Data Type:
  Integer

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: BrowserSignin
  - GP name: Browser sign-in settings
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:BrowserSignin
  - Value Type:REG_DWORD
  #### Example value: 
```
0x00000002
```


  ### Mac information and settings
  - Preference Key Name: BrowserSignin
  - Example value: 
```
2
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Use built-in DNS client (BuiltInDnsClientEnabled)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Controls whether to use the built-in DNS client.

If you enable this policy, the built-in DNS client is used, if it's available.

If you disable this policy, the client is never used.

If you don't configure this policy, the built-in DNS client is enabled by default on MacOS, and users can change whether to use the built-in DNS client by editing edge://flags or by specifying a command-line flag.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  Boolean

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: BuiltInDnsClientEnabled
  - GP name: Use built-in DNS client
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:BuiltInDnsClientEnabled
  - Value Type:REG_DWORD
  #### Example value: 
```
True
```


  ### Mac information and settings
  - Preference Key Name: BuiltInDnsClientEnabled
  - Example value: 
```
True
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Disable Certificate Transparency enforcement for a list of subjectPublicKeyInfo hashes (CertificateTransparencyEnforcementDisabledForCas)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Disables enforcement of Certificate Transparency requirements for a list of subjectPublicKeyInfo hashes.

This policy lets you disable Certificate Transparency disclosure requirements for certificate chains that contain certificates with one of the specified subjectPublicKeyInfo hashes. This allows certificates that would otherwise be untrusted because they were not properly publicly disclosed to still be used for Enterprise hosts.

To disable Certificate Transparency enforcement when this policy is set, one of the following sets of conditions must be met:
1. The hash is of the server certificate's subjectPublicKeyInfo.
2. The hash is of a subjectPublicKeyInfo that appears in a CA certificate in the certificate chain, that CA certificate is constrained via the X.509v3 nameConstraints extension, one or more directoryName nameConstraints are present in the permittedSubtrees, and the directoryName contains an organizationName attribute.
3. The hash is of a subjectPublicKeyInfo that appears in a CA certificate in the certificate chain, the CA certificate has one or more organizationName attributes in the certificate Subject, and the server's certificate contains the same number of organizationName attributes, in the same order, and with byte-for-byte identical values.

A subjectPublicKeyInfo hash is specified by concatenating the hash algorithm name, the "/" character, and the Base64 encoding of that hash algorithm applied to the DER-encoded subjectPublicKeyInfo of the specified certificate. This Base64 encoding is the same format as an SPKI Fingerprint, as defined in RFC 7469, Section 2.4. Unrecognized hash algorithms are ignored. The only supported hash algorithm at this time is "sha256".

If you disable this policy or don't configure it, any certificate that's required to be disclosed via Certificate Transparency will be treated as untrusted if it's not disclosed according to the Certificate Transparency policy.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  List of strings

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: CertificateTransparencyEnforcementDisabledForCas
  - GP name: Disable Certificate Transparency enforcement for a list of subjectPublicKeyInfo hashes
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge\CertificateTransparencyEnforcementDisabledForCas
  - Path (Recommended):N/A
  - Value Name:1, 2, 3, ...
  - Value Type:list of REG_SZ
  #### Example value: 
```
SOFTWARE\Policies\Microsoft\Edge\CertificateTransparencyEnforcementDisabledForCas\0 = "sha256/AAAAAAAAAAAAAAAAAAAAAA=="
SOFTWARE\Policies\Microsoft\Edge\CertificateTransparencyEnforcementDisabledForCas\1 = "sha256//////////////////////w=="

```


  ### Mac information and settings
  - Preference Key Name: CertificateTransparencyEnforcementDisabledForCas
  - Example value: 
```
<array>
  <string>sha256/AAAAAAAAAAAAAAAAAAAAAA==</string>
  <string>sha256//////////////////////w==</string>
</array>

```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Disable Certificate Transparency enforcement for a list of legacy certificate authorities (CertificateTransparencyEnforcementDisabledForLegacyCas)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Disables enforcing Certificate Transparency requirements for a list of legacy certificate authorities (Cas).

This policy lets you disable Certificate Transparency disclosure requirements for certificate chains that contain certificates with one of the specified subjectPublicKeyInfo hashes. This allows certificates that would otherwise be untrusted because they were not properly publicly disclosed, continue to be used for enterprise hosts.

In order for Certificate Transparency enforcement to be disabled, you must set the hash to a subjectPublicKeyInfo appearing in a CA certificate that is recognized as a legacy certificate authority (CA). A legacy CA is a CA that has been publicly trusted by default by one or more operating systems supported by Microsoft Edge.

You specify a subjectPublicKeyInfo hash by concatenating the hash algorithm name, the "/" character, and the Base64 encoding of that hash algorithm applied to the DER-encoded subjectPublicKeyInfo of the specified certificate. This Base64 encoding is the same format as an SPKI Fingerprint, as defined in RFC 7469, Section 2.4. Unrecognized hash algorithms are ignored. The only supported hash algorithm at this time is "sha256".

If you don't configure this policy, any certificate that's required to be disclosed via Certificate Transparency will be treated as untrusted if it isn't disclosed according to the Certificate Transparency policy.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  List of strings

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: CertificateTransparencyEnforcementDisabledForLegacyCas
  - GP name: Disable Certificate Transparency enforcement for a list of legacy certificate authorities
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge\CertificateTransparencyEnforcementDisabledForLegacyCas
  - Path (Recommended):N/A
  - Value Name:1, 2, 3, ...
  - Value Type:list of REG_SZ
  #### Example value: 
```
SOFTWARE\Policies\Microsoft\Edge\CertificateTransparencyEnforcementDisabledForLegacyCas\0 = "sha256/AAAAAAAAAAAAAAAAAAAAAA=="
SOFTWARE\Policies\Microsoft\Edge\CertificateTransparencyEnforcementDisabledForLegacyCas\1 = "sha256//////////////////////w=="

```


  ### Mac information and settings
  - Preference Key Name: CertificateTransparencyEnforcementDisabledForLegacyCas
  - Example value: 
```
<array>
  <string>sha256/AAAAAAAAAAAAAAAAAAAAAA==</string>
  <string>sha256//////////////////////w==</string>
</array>

```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Disable Certificate Transparency enforcement for specific URLs (CertificateTransparencyEnforcementDisabledForUrls)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Disables enforcing Certificate Transparency requirements for the listed URLs.

This policy lets you not disclose certificates for the hostnames in the specified URLs via Certificate Transparency. This lets you use certificates that would otherwise be untrusted, because they weren't properly publicly disclosed, but it makes it harder to detect mis-issued certificates for those hosts.

Form your URL pattern according to https://docs.microsoft.com//Placeholder01. Because certificates are valid for a given hostname, independent of the scheme, port, or path, only the hostname part of the URL is considered. Wildcard hosts are not supported.

If you don't configure this policy, any certificate that should be disclosed via Certificate Transparency is treated as untrusted if it's not disclosed.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  List of strings

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: CertificateTransparencyEnforcementDisabledForUrls
  - GP name: Disable Certificate Transparency enforcement for specific URLs
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge\CertificateTransparencyEnforcementDisabledForUrls
  - Path (Recommended):N/A
  - Value Name:1, 2, 3, ...
  - Value Type:list of REG_SZ
  #### Example value: 
```
SOFTWARE\Policies\Microsoft\Edge\CertificateTransparencyEnforcementDisabledForUrls\0 = "contoso.com"
SOFTWARE\Policies\Microsoft\Edge\CertificateTransparencyEnforcementDisabledForUrls\1 = ".contoso.com"

```


  ### Mac information and settings
  - Preference Key Name: CertificateTransparencyEnforcementDisabledForUrls
  - Example value: 
```
<array>
  <string>contoso.com</string>
  <string>.contoso.com</string>
</array>

```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Allow HTTP/2 connection coalescing for these hosts even when client certificates are used (CoalesceH2ConnectionsWithClientCertificatesForHosts)
  >This is a future policy
  

  ### Description
  If you enable this policy, coalescing of HTTP/2 connections is allowed even when client certificates are being used.

If you leave this policy unconfigured, HTTP/2 connection coalescing isn't allowed on connections that are using client certificates. This is the default behavior.

In order to coalesce, both the host name of the potential new connection and the host name of an existing connection must match one or more patterns prescribed by this policy. This policy specifies a list of hosts, using the URLBlocklist filter format: "contoso.com" matches "contoso.com" and all subdomains (for example, "sub.contoso.com"), while ".contoso.net" matches exactly "contoso.net".

Coalescing requests to different hosts over connections that use client certificates can trigger security and privacy issues, as the ambient authority will be conveyed to all requests, even if the user did not explicitly approve this. Therefore, this policy is temporary and will be removed in a future release. For more info, see https://crbug.com/855690.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  List of strings

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: CoalesceH2ConnectionsWithClientCertificatesForHosts
  - GP name: Allow HTTP/2 connection coalescing for these hosts even when client certificates are used
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge\CoalesceH2ConnectionsWithClientCertificatesForHosts
  - Path (Recommended):N/A
  - Value Name:1, 2, 3, ...
  - Value Type:list of REG_SZ
  #### Example value: 
```
SOFTWARE\Policies\Microsoft\Edge\CoalesceH2ConnectionsWithClientCertificatesForHosts\0 = "contoso.com"

```


  ### Mac information and settings
  - Preference Key Name: CoalesceH2ConnectionsWithClientCertificatesForHosts
  - Example value: 
```
<array>
  <string>contoso.com</string>
</array>

```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Enable component updates in Microsoft Edge (ComponentUpdatesEnabled)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  If you enable or don't configure this policy, component updates are enabled in Microsoft Edge.

If you disable this policy or set it to false, component updates are disabled for all components in Microsoft Edge.

However, some components are exempt from this policy. This includes any component that doesn't contain executable code, that doesn't significantly alter the behavior of the browser, or that's critical for security. That is, updates that are deemed "critical for security" are still applied even if you disable this policy.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: No - Requires browser restart

  ### Data Type:
  Boolean

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: ComponentUpdatesEnabled
  - GP name: Enable component updates in Microsoft Edge
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:ComponentUpdatesEnabled
  - Value Type:REG_DWORD
  #### Example value: 
```
True
```


  ### Mac information and settings
  - Preference Key Name: ComponentUpdatesEnabled
  - Example value: 
```
True
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Configure Do Not Track (ConfigureDoNotTrack)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Specify whether to send Do Not Track requests to websites that ask for tracking info. Do Not Track requests let the websites you visit know that you don't want your browsing activity to be tracked. By default, Microsoft Edge doesn't send Do Not Track requests, but users can turn on this feature to send them.

If you enable this policy, Do Not Track requests are always sent to websites asking for tracking info.

If you disable this policy, requests are never sent.

If you don't configure this policy, users can choose whether to send these requests.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  Boolean

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: ConfigureDoNotTrack
  - GP name: Configure Do Not Track
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:ConfigureDoNotTrack
  - Value Type:REG_DWORD
  #### Example value: 
```
False
```


  ### Mac information and settings
  - Preference Key Name: ConfigureDoNotTrack
  - Example value: 
```
False
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Configure Online Text To Speech (ConfigureOnlineTextToSpeech)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Set whether the browser can leverage Online Text to Speech voice fonts, part of Azure Cognitive Services. These voice fonts are higher quality than the pre-installed system voice fonts.

If you enable or don't configure this policy, web-based applications that use the SpeechSynthesis API can use Online Text to Speech voice fonts.

If you disable this policy, the voice fonts aren't available.

Read more about this feature here:
SpeechSynthesis API: https://developer.mozilla.org/en-US/docs/Web/API/SpeechSynthesis
Cognitive Services: https://azure.microsoft.com/en-us/services/cognitive-services/text-to-speech/

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  Boolean

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: ConfigureOnlineTextToSpeech
  - GP name: Configure Online Text To Speech
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:ConfigureOnlineTextToSpeech
  - Value Type:REG_DWORD
  #### Example value: 
```
True
```


  ### Mac information and settings
  - Preference Key Name: ConfigureOnlineTextToSpeech
  - Example value: 
```
True
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Set Microsoft Edge as default browser (DefaultBrowserSettingEnabled)
  >Supported Versions: Microsoft Edge on Windows 7 and Mac since version 77 or later
  

  ### Description
  Configures the default browser checks in Microsoft Edge and prevents users from changing them.

If you enable this policy, Microsoft Edge always checks on startup whether it is the default browser and automatically registers itself, if possible.

If you disable this policy, Microsoft Edge never checks and disables user controls for setting this option.

If you don't configure this policy, Microsoft Edge lets the user control whether it's the default browser and whether to show user notifications when it isn't.

Note for Windows administrators: This policy only works for PCs running Windows 7. For later versions of Windows, you have to deploy a "default application associations" file that makes Microsoft Edge the handler for the https and http protocols (and, optionally, the ftp protocol and file formats such as .html, .htm, .pdf, .svg, .webp). See https://docs.microsoft.com//Placeholder02 for more information.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  Boolean

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: DefaultBrowserSettingEnabled
  - GP name: Set Microsoft Edge as default browser
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:DefaultBrowserSettingEnabled
  - Value Type:REG_DWORD
  #### Example value: 
```
True
```


  ### Mac information and settings
  - Preference Key Name: DefaultBrowserSettingEnabled
  - Example value: 
```
True
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Control where developer tools can be used (DeveloperToolsAvailability)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Control where developer tools can be used.

If you set this policy to 'DeveloperToolsDisallowedForForceInstalledExtensions' (0, the default), users can access the developer tools and the JavaScript console in general, but not in the context of extensions installed by enterprise policy.

If you set this policy to 'DeveloperToolsAllowed' (1), users can access the developer tools and the JavaScript console in all contexts, including extensions installed by enterprise policy.

If you set this policy to 'DeveloperToolsDisallowed' (2), users can't access the developer tools or inspect website elements. Keyboard shortcuts and menu or context menu entries that open the developer tools or the JavaScript Console are disabled.

* 0 = Block the developer tools on extensions installed by enterprise policy, allow in other contexts

* 1 = Allow using the developer tools

* 2 = Don't allow using the developer tools

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  Integer

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: DeveloperToolsAvailability
  - GP name: Control where developer tools can be used
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:DeveloperToolsAvailability
  - Value Type:REG_DWORD
  #### Example value: 
```
0x00000002
```


  ### Mac information and settings
  - Preference Key Name: DeveloperToolsAvailability
  - Example value: 
```
2
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Disable support for 3D graphics APIs (Disable3DAPIs)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Prevent web pages from accessing the graphics processing unit (GPU). Specifically, web pages can't access the WebGL API and plug-ins can't use the Pepper 3D API.

If you don't configure or disable this policy, it potentially allows web pages to use the WebGL API and plug-ins to use the Pepper 3D API. Microsoft Edge might, by default, still require command line arguments to be passed in order to use these APIs.

If 'HardwareAccelerationModeEnabled' policy is set to false, the setting for 'Disable3DAPIs' policy is ignored - it's the equivalent of setting 'Disable3DAPIs' policy to true.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  Boolean

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: Disable3DAPIs
  - GP name: Disable support for 3D graphics APIs
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:Disable3DAPIs
  - Value Type:REG_DWORD
  #### Example value: 
```
False
```


  ### Mac information and settings
  - Preference Key Name: Disable3DAPIs
  - Example value: 
```
False
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Disable taking screenshots (DisableScreenshots)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Controls if users can take screenshots of the browser page.

If enabled, user can't take screenshots by using keyboard shortcuts or extension APIs.

If disabled or don't configure this policy, users can take screenshots.

Please note this policy controls screenshots taken from within the browser itself. Even if you enable this policy, users might still be able to take screenshots using some method outside of the browser (like using an operating system feature or another application).

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  Boolean

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: DisableScreenshots
  - GP name: Disable taking screenshots
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:DisableScreenshots
  - Value Type:REG_DWORD
  #### Example value: 
```
True
```


  ### Mac information and settings
  - Preference Key Name: DisableScreenshots
  - Example value: 
```
True
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Set disk cache directory (DiskCacheDir)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Configures the directory to use to store cached files.

If you enable this policy, Microsoft Edge uses the provided directory regardless of whether the user has specified the '--disk-cache-dir' flag. To avoid data loss or other unexpected errors, don't configure this policy to a volume's root directory or to a directory used for other purposes, because Microsoft Edge manages its contents.

See https://docs.microsoft.com/Placeholder08 for a list of variables you can use when specifying directories and paths.

If you don't configure this policy, the default cache directory is used, and users can override that default with the '--disk-cache-dir' command line flag.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: No - Requires browser restart

  ### Data Type:
  String

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: DiskCacheDir
  - GP name: Set disk cache directory
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:DiskCacheDir
  - Value Type:REG_SZ
  #### Example value: 
```
"${user_home}/Edge_cache"
```


  ### Mac information and settings
  - Preference Key Name: DiskCacheDir
  - Example value: 
```
"${user_home}/Edge_cache"
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Set disk cache size, in bytes (DiskCacheSize)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Configures the size of the cache, in bytes, used to store files on the disk.

If you enable this policy, Microsoft Edge uses the provided cache size regardless of whether the user has specified the '--disk-cache-size' flag. The value specified in this policy isn't a hard boundary but rather a suggestion to the caching system; any value below a few megabytes is too small and will be rounded up to a reasonable minimum.

If you set the value of this policy to 0, the default cache size is used, and users can't change it.

If you don't configure this policy, the default size is used, but users can override it with the '--disk-cache-size' flag.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: No - Requires browser restart

  ### Data Type:
  Integer

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: DiskCacheSize
  - GP name: Set disk cache size, in bytes
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:DiskCacheSize
  - Value Type:REG_DWORD
  #### Example value: 
```
0x06400000
```


  ### Mac information and settings
  - Preference Key Name: DiskCacheSize
  - Example value: 
```
104857600
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Set download directory (DownloadDirectory)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Configures the directory to use when downloading files.

If you enable this policy, Microsoft Edge uses the provided directory regardless of whether the user has specified one or chosen to be prompted for download location every time. See https://docs.microsoft.com/Placeholder08 for a list of variables that can be used.

If you disable or don't configure this policy, the default download directory is used, and the user can change it.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: Yes
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  String

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: DownloadDirectory
  - GP name: Set download directory
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): Administrative Templates/Microsoft Edge - Default Settings (users can override)/
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): SOFTWARE\Policies\Microsoft\Edge\Recommended
  - Value Name:DownloadDirectory
  - Value Type:REG_SZ
  #### Example value: 
```
"/home/${user_name}/Downloads"
```


  ### Mac information and settings
  - Preference Key Name: DownloadDirectory
  - Example value: 
```
"/home/${user_name}/Downloads"
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Allow download restrictions (DownloadRestrictions)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Configures the type of downloads that Microsoft Edge completely blocks, without letting users override the security decision.

Set 'Block dangerous downloads' (1) to allow all downloads except for those that carry Microsoft Defender SmartScreen warnings.

Set 'Block potentially dangerous downloads' (2) to allow all downloads except for those that carry Microsoft Defender SmartScreen warnings of potentially dangerous downloads.

Set 'Block all downloads' (3) to block all downloads.

If you don't configure this policy or set the 'No special restrictions' (0) option, the downloads go through the usual security restrictions based on Microsoft Defender SmartScreen analysis results.

Note that these restrictions apply to downloads from web page content, as well as the 'download link...' context menu option. These restrictions don't apply to saving or downloading the currently displayed page, nor do they apply to the Save as PDF option from the printing options.

See https://docs.microsoft.com/Placeholder09 for more info on Microsoft Defender SmartScreen.

* 0 = No special restrictions

* 1 = Block dangerous downloads

* 2 = Block potentially dangerous downloads

* 3 = Block all downloads

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: Yes
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  Integer

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: DownloadRestrictions
  - GP name: Allow download restrictions
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): Administrative Templates/Microsoft Edge - Default Settings (users can override)/
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): SOFTWARE\Policies\Microsoft\Edge\Recommended
  - Value Name:DownloadRestrictions
  - Value Type:REG_DWORD
  #### Example value: 
```
0x00000002
```


  ### Mac information and settings
  - Preference Key Name: DownloadRestrictions
  - Example value: 
```
2
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Allows users to edit favorites (EditFavoritesEnabled)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Enable this policy to let users add, remove, and modify favorites. This is the default behavior if you don't configure the policy.

Disable this policy to stop users from adding, removing, or modifying favorites. They can still use existing favorites.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  Boolean

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: EditFavoritesEnabled
  - GP name: Allows users to edit favorites
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:EditFavoritesEnabled
  - Value Type:REG_DWORD
  #### Example value: 
```
False
```


  ### Mac information and settings
  - Preference Key Name: EditFavoritesEnabled
  - Example value: 
```
False
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Re-enable deprecated web platform features for a limited time (EnableDeprecatedWebPlatformFeatures)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Specify a list of deprecated web platform features to temporarily re-enable.

This policy lets you re-enable deprecated web platform features for a limited time. Features are identified by a string tag.

If you don't configure this policy, if the list is empty, or if a feature doesn't match one of the supported string tags, all deprecated web platform features remain disabled.

While the policy itself is supported on the above platforms, the feature it's enabling might not be available on all of those platforms. Not all deprecated Web Platform features can be re-enabled. Only those explicitly listed below can be re-enabled, and only for a limited period of time, which differs per feature. You can review the intent behind the Web Platform feature changes at https://bit.ly/blinkintents.

The general format of the string tag is [DeprecatedFeatureName]_EffectiveUntil[yyyymmdd].

* "ExampleDeprecatedFeature_EffectiveUntil20080902" = Enable ExampleDeprecatedFeature API through 2008/09/02

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  List of strings

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: EnableDeprecatedWebPlatformFeatures
  - GP name: Re-enable deprecated web platform features for a limited time
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge\EnableDeprecatedWebPlatformFeatures
  - Path (Recommended):N/A
  - Value Name:1, 2, 3, ...
  - Value Type:list of REG_SZ
  #### Example value: 
```
SOFTWARE\Policies\Microsoft\Edge\EnableDeprecatedWebPlatformFeatures\0 = "ExampleDeprecatedFeature_EffectiveUntil20080902"

```


  ### Mac information and settings
  - Preference Key Name: EnableDeprecatedWebPlatformFeatures
  - Example value: 
```
<array>
  <string>ExampleDeprecatedFeature_EffectiveUntil20080902</string>
</array>

```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Enable Domain Actions Download from Microsoft (EnableDomainActionsDownload)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  In Microsoft Edge, Domain Actions represent a series of compatibility features that help the browser work correctly on the web.

Microsoft keeps a list of actions to take on certain domains for compatibility reasons. For example, the browser may override the User Agent string on a website if that website is broken due to the new User Agent string on Microsoft Edge. Each of these actions is intended to be temporary while Microsoft tries to resolve the issue with the site owner.

When the browser starts up and then periodically afterwards, the browser will contact the Microsoft server that contains the most up to date list of compatibility actions to perform. This list is saved locally after it is first retrieved so that subsequent requests will only update the list if the server's copy has changed.

If you enable this policy, the list of Domain Actions will continue to be downloaded from a Microsoft server.

If you disable this policy, the list of Domain Actions will no longer be downloaded from a Microsoft server.

If you don't configure this policy, the list of Domain Actions will continue to be downloaded from a Microsoft server.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  Boolean

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: EnableDomainActionsDownload
  - GP name: Enable Domain Actions Download from Microsoft
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:EnableDomainActionsDownload
  - Value Type:REG_DWORD
  #### Example value: 
```
True
```


  ### Mac information and settings
  - Preference Key Name: EnableDomainActionsDownload
  - Example value: 
```
True
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Enable online OCSP/CRL checks (EnableOnlineRevocationChecks)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Enable this policy to use online OSCP/CRL checks, which are disabled by default in Microsoft Edge. (These soft-fail, online revocation checks provide no effective security benefit.)

If you disable the policy or don't configure it, Microsoft Edge doesn't perform online revocation checks.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  Boolean

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: EnableOnlineRevocationChecks
  - GP name: Enable online OCSP/CRL checks
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:EnableOnlineRevocationChecks
  - Value Type:REG_DWORD
  #### Example value: 
```
False
```


  ### Mac information and settings
  - Preference Key Name: EnableOnlineRevocationChecks
  - Example value: 
```
False
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Enable favorites bar (FavoritesBarEnabled)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Enables or disables the favorites bar.

If you enable this policy, users will see the favorites bar.

If you disable this policy, users won't see the favorites bar.

If this policy is not configured, then the user can decide to use the favorites bar or not.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: Yes
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  Boolean

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: FavoritesBarEnabled
  - GP name: Enable favorites bar
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): Administrative Templates/Microsoft Edge - Default Settings (users can override)/
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): SOFTWARE\Policies\Microsoft\Edge\Recommended
  - Value Name:FavoritesBarEnabled
  - Value Type:REG_DWORD
  #### Example value: 
```
True
```


  ### Mac information and settings
  - Preference Key Name: FavoritesBarEnabled
  - Example value: 
```
True
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Configure Bing SafeSearch (ForceBingSafeSearch)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Ensure that queries in Bing web search are done with SafeSearch set to the value specified. Users can't change this setting.

If you configure this policy to "Off", SafeSearch in Bing search falls back to the bing.com value.

If you configure this policy to "Moderate", the moderate setting is used in SafeSearch. The moderate setting filters adult videos and images but not text from search results.

If you configure this policy to "Strict", the strict setting in SafeSearch is used. The strict setting filters adult text, images, and videos.

If you disable this policy or don't configure it, SafeSearch in Bing search isn't enforced, and users can set the value they want on bing.com.

* 0 = Don't configure search restrictions in Bing

* 1 = Configure moderate search restrictions in Bing

* 2 = Configure strict search restrictions in Bing

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  Integer

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: ForceBingSafeSearch
  - GP name: Configure Bing SafeSearch
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:ForceBingSafeSearch
  - Value Type:REG_DWORD
  #### Example value: 
```
0x00000000
```


  ### Mac information and settings
  - Preference Key Name: ForceBingSafeSearch
  - Example value: 
```
0
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Enable use of ephemeral profiles (ForceEphemeralProfiles)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Controls whether user profiles are switched to ephemeral mode. An ephemeral profile is created when a session begins, is deleted when the session ends, and is associated with the user's original profile.

If you enable this policy, profiles run in ephemeral mode. This lets users work from their own devices without saving browsing data to those devices. If you enable this policy as an OS policy (by using GPO on Windows, for example), it applies to every profile on the system.

If you disable this policy or don't configure it, users get their regular profiles when they sign in to the browser.

In ephemeral mode, profile data is saved on disk only for the length of the user session. Features like browser history, extensions and their data, web data like cookies, and web databases aren't saved after the browser is closed. This doesn't prevent a user from manually downloading any data to disk, or from saving pages or printing them. If the user has enabled sync, all data is preserved in their sync accounts just like with regular profiles. Users can also use InPrivate browsing in ephemeral mode unless you explicitly disable this.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: No - Requires browser restart

  ### Data Type:
  Boolean

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: ForceEphemeralProfiles
  - GP name: Enable use of ephemeral profiles
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:ForceEphemeralProfiles
  - Value Type:REG_DWORD
  #### Example value: 
```
True
```


  ### Mac information and settings
  - Preference Key Name: ForceEphemeralProfiles
  - Example value: 
```
True
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Enforce Google SafeSearch (ForceGoogleSafeSearch)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Forces queries in Google Web Search to be performed with SafeSearch set to active, and prevents users from changing this setting.

If you enable this policy, SafeSearch in Google Search is always active.

If you disable this policy or don't configure it, SafeSearch in Google Search isn't enforced.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  Boolean

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: ForceGoogleSafeSearch
  - GP name: Enforce Google SafeSearch
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:ForceGoogleSafeSearch
  - Value Type:REG_DWORD
  #### Example value: 
```
False
```


  ### Mac information and settings
  - Preference Key Name: ForceGoogleSafeSearch
  - Example value: 
```
False
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Force minimum YouTube Restricted Mode (ForceYouTubeRestrict)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Enforces a minimum Restricted Mode on YouTube and prevents users from picking a less restricted mode.

Set to Strict (2) to enforce Strict Restricted Mode on YouTube.

Set to Moderate (1) to enforce the user to only use Moderate Restricted Mode and Strict Restricted Mode on YouTube. They can't disable Restricted Mode.

Set to Off (0) or don't configure this policy to not enforce Restricted Mode on YouTube. External policies such as YouTube policies might still enforce Restricted Mode.

* 0 = Do not enforce Restricted Mode on YouTube

* 1 = Enforce at least Moderate Restricted Mode on YouTube

* 2 = Enforce Strict Restricted Mode for YouTube

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  Integer

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: ForceYouTubeRestrict
  - GP name: Force minimum YouTube Restricted Mode
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:ForceYouTubeRestrict
  - Value Type:REG_DWORD
  #### Example value: 
```
0x00000000
```


  ### Mac information and settings
  - Preference Key Name: ForceYouTubeRestrict
  - Example value: 
```
0
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Allow full screen mode (FullscreenAllowed)
  >Supported Versions: Microsoft Edge on Windows since version 77 or later
  

  ### Description
  Set the availability of full screen mode - all Microsoft Edge UI is hidden and only web content is visible.

If you enable this policy or don't configure it, the user, apps, and extensions with appropriate permissions can enter full screen mode.

If you disable this policy, users, apps, and extensions can't enter full screen mode.

Opening Microsoft Edge in kiosk mode using the command line is unavailable when full screen mode is disabled.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  Boolean

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: FullscreenAllowed
  - GP name: Allow full screen mode
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:FullscreenAllowed
  - Value Type:REG_DWORD
  #### Example value: 
```
True
```


  

  [Back to Top](#Edge-Policy-Documentation)

  ## Use hardware acceleration when available (HardwareAccelerationModeEnabled)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Specify to use hardware acceleration, if it's available. If you enable this policy or don't configure it, hardware acceleration is enabled unless a GPU feature is explicitly blocked.

If you disable this policy, hardware acceleration is disabled.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: No - Requires browser restart

  ### Data Type:
  Boolean

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: HardwareAccelerationModeEnabled
  - GP name: Use hardware acceleration when available
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:HardwareAccelerationModeEnabled
  - Value Type:REG_DWORD
  #### Example value: 
```
True
```


  ### Mac information and settings
  - Preference Key Name: HardwareAccelerationModeEnabled
  - Example value: 
```
True
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Allow importing of autofill form data (ImportAutofillFormData)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Allows users to import autofill form data from another browser into Microsoft Edge.

If you enable this policy, the option to manually import autofill data is automatically selected.

If you disable this policy, autofill form data isn't imported at first run, and users can't import it manually.

If you don't configure this policy, autofill data is imported at first run, and users can choose whether to import this data manually during later browsing sessions.

You can set this policy as a recommendation. This means that Microsoft Edge will import autofill data on first run, but users can select or clear **autofill data** option during manual import.

**Note**: This policy currently manages importing from Google Chrome (on Windows 7, 8, and 10 and on macOS).

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: Yes
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  Boolean

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: ImportAutofillFormData
  - GP name: Allow importing of autofill form data
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): Administrative Templates/Microsoft Edge - Default Settings (users can override)/
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): SOFTWARE\Policies\Microsoft\Edge\Recommended
  - Value Name:ImportAutofillFormData
  - Value Type:REG_DWORD
  #### Example value: 
```
True
```


  ### Mac information and settings
  - Preference Key Name: ImportAutofillFormData
  - Example value: 
```
True
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Allow importing of favorites (ImportFavorites)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Allows users to import favorites from another browser into Microsoft Edge.

If you enable this policy, the **Favorites** check box is automatically selected in the **Import browser data** dialog box.

If you disable this policy, favorites aren't imported at first run, and users can’t import them manually.

If you don’t configure this policy, favorites are imported at first run, and users can choose whether to import them manually during later browsing sessions.

You can also set this policy as a recommendation. This means that Microsoft Edge imports favorites on first run, but users can select or clear the **favorites** option during manual import.

**Note**: This policy currently manages importing from Internet Explorer (on Windows 7, 8, and 10), Google Chrome (on Windows 7, 8, and 10 and on macOS) and Apple Safari (on macOS) browsers.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: Yes
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  Boolean

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: ImportFavorites
  - GP name: Allow importing of favorites
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): Administrative Templates/Microsoft Edge - Default Settings (users can override)/
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): SOFTWARE\Policies\Microsoft\Edge\Recommended
  - Value Name:ImportFavorites
  - Value Type:REG_DWORD
  #### Example value: 
```
True
```


  ### Mac information and settings
  - Preference Key Name: ImportFavorites
  - Example value: 
```
True
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Allow importing of browsing history (ImportHistory)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Allows users to import their browsing history from another browser into Microsoft Edge.

If you enable this policy, the **Browsing history** check box is automatically selected in the **Import browser data** dialog box.

If you disable this policy, browsing history data isn't imported at first run, and users can’t import this data manually.

If you don’t configure this policy, browsing history data is imported at first run, and users can choose whether to import it manually during later browsing sessions.

You can also set this policy as a recommendation. This means that Microsoft Edge imports browsing history on first run, but users can select or clear the **history** option during manual import.

**Note**: This policy currently manages importing from Internet Explorer (on Windows 7, 8, and 10), Google Chrome (on Windows 7, 8, and 10 and on macOS) and Apple Safari (macOS) browsers.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: Yes
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  Boolean

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: ImportHistory
  - GP name: Allow importing of browsing history
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): Administrative Templates/Microsoft Edge - Default Settings (users can override)/
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): SOFTWARE\Policies\Microsoft\Edge\Recommended
  - Value Name:ImportHistory
  - Value Type:REG_DWORD
  #### Example value: 
```
True
```


  ### Mac information and settings
  - Preference Key Name: ImportHistory
  - Example value: 
```
True
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Allow importing of home page settings (ImportHomepage)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Allows users to import their home page setting from another browser into Microsoft Edge.

If you enable this policy, the option to manually import the home page setting is automatically selected.

If you disable this policy, the home page setting isn’t imported at first run, and users can’t import it manually.

If you don’t configure this policy, the home page setting is imported at first run, and users can choose whether to import this data manually during later browsing sessions.

You can set this policy as a recommendation. This means that Microsoft Edge imports the home page setting on first run, but users can select or clear the **home page** option during manual import.

**Note**: This policy currently manages importing from Internet Explorer (on Windows 7, 8, and 10).

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  Boolean

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: ImportHomepage
  - GP name: Allow importing of home page settings
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:ImportHomepage
  - Value Type:REG_DWORD
  #### Example value: 
```
True
```


  ### Mac information and settings
  - Preference Key Name: ImportHomepage
  - Example value: 
```
True
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Allow importing of payment info (ImportPaymentInfo)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Allows users to import payment info from another browser into Microsoft Edge.

If you enable this policy, the **payment info** check box is automatically selected in the **Import browser data** dialog box.

If you disable this policy, payment info isn’t imported at first run, and users can’t import it manually.

If you don’t configure this policy, payment info is imported at first run, and users can choose whether to import it manually during later browsing sessions.

You can also set this policy as a recommendation. This means that Microsoft Edge imports payment info on first run, but users can select or clear the **payment info** option during manual import.

**Note:** This policy currently manages importing from Google Chrome (on Windows 7, 8, and 10 and on macOS).

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: Yes
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  Boolean

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: ImportPaymentInfo
  - GP name: Allow importing of payment info
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): Administrative Templates/Microsoft Edge - Default Settings (users can override)/
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): SOFTWARE\Policies\Microsoft\Edge\Recommended
  - Value Name:ImportPaymentInfo
  - Value Type:REG_DWORD
  #### Example value: 
```
True
```


  ### Mac information and settings
  - Preference Key Name: ImportPaymentInfo
  - Example value: 
```
True
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Allow importing of saved passwords (ImportSavedPasswords)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Allows users to import saved passwords from another browser into Microsoft Edge.

If you enable this policy, the option to manually import saved passwords is automatically selected.

If you disable this policy, saved passwords aren't imported on first run, and users can't import them manually.

If you don't configure this policy, passwords are imported at first run, and users can choose whether to import them manually during later browsing sessions.

You can set this policy as a recommendation. This means that Microsoft Edge imports passwords on first run, but users can select or clear the **passwords** option during manual import.

**Note**: This policy currently manages importing from Internet Explorer (on Windows 7, 8, and 10) and Google Chrome (on Windows 7, 8, and 10 and on macOS) browsers.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: Yes
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  Boolean

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: ImportSavedPasswords
  - GP name: Allow importing of saved passwords
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): Administrative Templates/Microsoft Edge - Default Settings (users can override)/
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): SOFTWARE\Policies\Microsoft\Edge\Recommended
  - Value Name:ImportSavedPasswords
  - Value Type:REG_DWORD
  #### Example value: 
```
True
```


  ### Mac information and settings
  - Preference Key Name: ImportSavedPasswords
  - Example value: 
```
True
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Allow importing of search engine settings (ImportSearchEngine)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Allows users to import search engine settings from another browser into Microsoft Edge.

If you enable, this policy, the option to import search engine settings is automatically selected.

If you disable this policy, search engine settings aren't imported at first run, and users can’t import them manually.

If you don’t configure this policy, search engine settings are imported at first run, and users can choose whether to import this data manually during later browsing sessions.

You can set this policy as a recommendation. This means that Microsoft Edge imports search engine settings on first run, but users can select or clear the **search engine** option during manual import.

**Note**: This policy currently manages importing from Internet Explorer (on Windows 7, 8, and 10).

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: Yes
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  Boolean

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: ImportSearchEngine
  - GP name: Allow importing of search engine settings
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): Administrative Templates/Microsoft Edge - Default Settings (users can override)/
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): SOFTWARE\Policies\Microsoft\Edge\Recommended
  - Value Name:ImportSearchEngine
  - Value Type:REG_DWORD
  #### Example value: 
```
True
```


  ### Mac information and settings
  - Preference Key Name: ImportSearchEngine
  - Example value: 
```
True
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Configure InPrivate mode availability (InPrivateModeAvailability)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Specifies whether the user can open pages in InPrivate mode in Microsoft Edge.

If you don't configure this policy or set it to 'Enabled' (0), users can open pages in InPrivate mode.

Set this policy to 'Disable' (1) to stop users from using InPrivate mode.

Set this policy to 'Forced' (2) to always use InPrivate mode.

* 0 = InPrivate mode available

* 1 = InPrivate mode disabled

* 2 = InPrivate mode forced

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  Integer

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: InPrivateModeAvailability
  - GP name: Configure InPrivate mode availability
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:InPrivateModeAvailability
  - Value Type:REG_DWORD
  #### Example value: 
```
0x00000001
```


  ### Mac information and settings
  - Preference Key Name: InPrivateModeAvailability
  - Example value: 
```
1
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Configure Internet Explorer integration (InternetExplorerIntegrationLevel)
  >Supported Versions: Microsoft Edge on Windows since version 77 or later
  

  ### Description
  Allows you to configure the scope of Internet Explorer integration in Microsoft Edge.

If you enable this policy, you can choose between the following options:
* Internet Explorer mode: provides full immersive integration of Internet Explorer with Microsoft Edge version 77 or later
* Internet Explorer 11: lets users open selected sites in the stand-alone version of Internet Explorer 11

If you disable or don’t configure this policy, all sites are opened in Microsoft Edge. This is the default behavior.

To configure this policy, you must first enable at least one of the following related policies. Otherwise, this policy will have no effect.
- Use the Enterprise Mode IE website list (‘SiteList’)
- Send all intranet sites to Internet Explorer (‘SendIntranetToInternetExplorer’)

For more info about how to use this policy together with other related policies to create the optimal configuration for your organization, see https://go.microsoft.com/fwlink/?linkid=2094210.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: No - Requires browser restart

  ### Data Type:
  Integer

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: InternetExplorerIntegrationLevel
  - GP name: Configure Internet Explorer integration
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:InternetExplorerIntegrationLevel
  - Value Type:REG_DWORD
  #### Example value: 
```
0x00000001
```


  

  [Back to Top](#Edge-Policy-Documentation)

  ## Enable site isolation for specific origins (IsolateOrigins)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Specify origins to run in isolation, in their own process.
This policy also isolates origins named by subdomains - for example, specifying https://contoso.com/ will cause https://foo.contoso.com/ to be isolated as part of the https://contoso.com/ site.
If the policy is enabled, each of the named origins in a comma-separated list will run in its own process.
If you disable this policy, then both the 'IsolateOrigins' and 'SitePerProcess' features are disabled. Users can still enable 'IsolateOrigins' policy manually, via command line flags.
If you don't configure the policy, the user can change this setting.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: No - Requires browser restart

  ### Data Type:
  String

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: IsolateOrigins
  - GP name: Enable site isolation for specific origins
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:IsolateOrigins
  - Value Type:REG_SZ
  #### Example value: 
```
"https://contoso.com/,https://fabrikam.com/"
```


  ### Mac information and settings
  - Preference Key Name: IsolateOrigins
  - Example value: 
```
"https://contoso.com/,https://fabrikam.com/"
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Configure favorites (ManagedFavorites)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Configures a list of managed favorites.

The policy creates a list of favorites. Each favorite contains the keys "name" and "url," which hold the favorite's name and its target. You can configure a subfolder by defining a favorites without an "url" key but with an additional "children" key that contains a list of favorites as defined above (some of which may be folders again). Microsoft Edge amends incomplete URLs as if they were submitted via the Address Bar, for example "microsoft.com" becomes "https://microsoft.com/".

These favorites are placed in a folder that can't be modified by the user (but the user can choose to hide it from the favorites bar). By default the folder name is "Managed favorites" but you can change it by adding to the list of favorites a dictionary containing the key "toplevel_name" with the desired folder name as the value.

Managed favorites are not synced to the user account and can't be modified by extensions.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  Dictionary

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: ManagedFavorites
  - GP name: Configure favorites
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:ManagedFavorites
  - Value Type:REG_SZ
  #### Example value: 
```
SOFTWARE\Policies\Microsoft\Edge\ManagedFavorites = [
  {
    "toplevel_name": "My managed favorites folder"
  }, 
  {
    "name": "Microsoft", 
    "url": "microsoft.com"
  }, 
  {
    "name": "Bing", 
    "url": "bing.com"
  }, 
  {
    "children": [
      {
        "name": "Microsoft Edge Insiders", 
        "url": "www.microsoftedgeinsider.com"
      }, 
      {
        "name": "Microsoft Edge", 
        "url": "www.microsoft.com/windows/microsoft-edge"
      }
    ], 
    "name": "Microsoft Edge links"
  }
]
```


  ### Mac information and settings
  - Preference Key Name: ManagedFavorites
  - Example value: 
```
<key>ManagedFavorites</key>
<array>
  <dict>
    <key>toplevel_name</key>
    <string>My managed favorites folder</string>
  </dict>
  <dict>
    <key>name</key>
    <string>Microsoft</string>
    <key>url</key>
    <string>microsoft.com</string>
  </dict>
  <dict>
    <key>name</key>
    <string>Bing</string>
    <key>url</key>
    <string>bing.com</string>
  </dict>
  <dict>
    <key>children</key>
    <array>
      <dict>
        <key>name</key>
        <string>Microsoft Edge Insiders</string>
        <key>url</key>
        <string>www.microsoftedgeinsider.com</string>
      </dict>
      <dict>
        <key>name</key>
        <string>Microsoft Edge</string>
        <key>url</key>
        <string>www.microsoft.com/windows/microsoft-edge</string>
      </dict>
    </array>
    <key>name</key>
    <string>Microsoft Edge links</string>
  </dict>
</array>
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Manage Search Engines (ManagedSearchEngines)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Lets you configure a list of list of up to 10 search engines, one of which must be marked as the default search engine.
You do not need to specify the encoding for any search engine.

If you enable this policy, users can't add, remove, or change any search engine in the list. Users can set their default search engine to any search engine in the list.

If you disable or don't configure this policy, users can modify the search engines list as desired.

If the 'DefaultSearchProviderSearchURL' policy is set, this policy ('ManagedSearchEngines') is ignored. The user must restart their browser to finish applying this policy.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: No - Requires browser restart

  ### Data Type:
  Dictionary

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: ManagedSearchEngines
  - GP name: Manage Search Engines
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:ManagedSearchEngines
  - Value Type:REG_SZ
  #### Example value: 
```
SOFTWARE\Policies\Microsoft\Edge\ManagedSearchEngines = [
  {
    "image_search_url": "https://www.example1.com/images/detail/search?iss=sbiupload", 
    "is_default": true, 
    "keyword": "example1.com", 
    "name": "Example1", 
    "search_url": "https://www.example1.com/search?q={searchTerms}", 
    "suggest_url": "https://www.example1.com/qbox?query={searchTerms}"
  }, 
  {
    "image_search_url": "https://www.example2.com/images/detail/search?iss=sbiupload", 
    "keyword": "example2.com", 
    "name": "Example2", 
    "search_url": "https://www.example2.com/search?q={searchTerms}", 
    "suggest_url": "https://www.example2.com/qbox?query={searchTerms}"
  }, 
  {
    "encoding": "UTF-8", 
    "image_search_url": "https://www.example3.com/images/detail/search?iss=sbiupload", 
    "keyword": "example3.com", 
    "name": "Example3", 
    "search_url": "https://www.example3.com/search?q={searchTerms}", 
    "suggest_url": "https://www.example3.com/qbox?query={searchTerms}"
  }
]
```


  ### Mac information and settings
  - Preference Key Name: ManagedSearchEngines
  - Example value: 
```
<key>ManagedSearchEngines</key>
<array>
  <dict>
    <key>image_search_url</key>
    <string>https://www.example1.com/images/detail/search?iss=sbiupload</string>
    <key>is_default</key>
    <true/>
    <key>keyword</key>
    <string>example1.com</string>
    <key>name</key>
    <string>Example1</string>
    <key>search_url</key>
    <string>https://www.example1.com/search?q={searchTerms}</string>
    <key>suggest_url</key>
    <string>https://www.example1.com/qbox?query={searchTerms}</string>
  </dict>
  <dict>
    <key>image_search_url</key>
    <string>https://www.example2.com/images/detail/search?iss=sbiupload</string>
    <key>keyword</key>
    <string>example2.com</string>
    <key>name</key>
    <string>Example2</string>
    <key>search_url</key>
    <string>https://www.example2.com/search?q={searchTerms}</string>
    <key>suggest_url</key>
    <string>https://www.example2.com/qbox?query={searchTerms}</string>
  </dict>
  <dict>
    <key>encoding</key>
    <string>UTF-8</string>
    <key>image_search_url</key>
    <string>https://www.example3.com/images/detail/search?iss=sbiupload</string>
    <key>keyword</key>
    <string>example3.com</string>
    <key>name</key>
    <string>Example3</string>
    <key>search_url</key>
    <string>https://www.example3.com/search?q={searchTerms}</string>
    <key>suggest_url</key>
    <string>https://www.example3.com/qbox?query={searchTerms}</string>
  </dict>
</array>
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Maximum number of concurrent connections to the proxy server (MaxConnectionsPerProxy)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Specifies the maximum number of simultaneous connections to the proxy server.

Some proxy servers can't handle a high number of concurrent connections per client - you can solve this by setting this policy to a lower value.

The value of this policy should be lower than 100 and higher than 6. The default value is 32.

Some web apps are known to consume many connections with hanging GETs - lowering the maximum connections below 32 may lead to browser networking hangs if too many of these kind of web apps are open.

If you don't configure this policy, the default value (32) is used.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: No - Requires browser restart

  ### Data Type:
  Integer

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: MaxConnectionsPerProxy
  - GP name: Maximum number of concurrent connections to the proxy server
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:MaxConnectionsPerProxy
  - Value Type:REG_DWORD
  #### Example value: 
```
0x00000020
```


  ### Mac information and settings
  - Preference Key Name: MaxConnectionsPerProxy
  - Example value: 
```
32
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Allow Google Cast to connect to Cast devices on all IP addresses (MediaRouterCastAllowAllIPs)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Enable this policy to let Google Cast connect to Cast devices on all IP addresses, not just RFC1918/RFC4193 private addresses.

Disable this policy to restrict Google Cast to Cast devices on RFC1918/RFC4193 private addresses.

If you don't configure this policy, Google Cast connects to Cast devices on RFC1918/RFC4193 private addresses only, unless you enable the CastAllowAllIPs feature.

If the 'EnableMediaRouter' policy is disabled, then this policy has no effect.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  Boolean

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: MediaRouterCastAllowAllIPs
  - GP name: Allow Google Cast to connect to Cast devices on all IP addresses
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:MediaRouterCastAllowAllIPs
  - Value Type:REG_DWORD
  #### Example value: 
```
False
```


  ### Mac information and settings
  - Preference Key Name: MediaRouterCastAllowAllIPs
  - Example value: 
```
False
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Enable usage and crash-related data reporting (MetricsReportingEnabled)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Enables reporting of usage and crash-related data about Microsoft Edge to Microsoft and prevents users from changing this setting.

Enable this policy to send reporting of usage and crash-related data to Microsoft. Disable this policy to not send the data to Microsoft. In both cases, users can't change or override the setting.

If you don't configure this policy, Microsoft Edge will use what the user chose upon installation / first run.

This policy is available only on Windows instances that are joined to a Microsoft Active Directory domain or Windows 10 Pro or Enterprise instances that are enrolled for device management.

On Windows 7, 8, and Mac this policy controls usage and crash-related data.

On Windows 10 Beta, Canary, Dev this policy controls only usage data. Crash data is controlled by the Windows diagnostic data setting (https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization#overview).

On Windows 10 Stable the usage and crash data collection is controlled by the Windows Diagnostic data setting (https://docs.microsoft.com/windows/privacy/configure-windows-diagnostic-data-in-your-organization#overview)

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: No - Requires browser restart

  ### Data Type:
  Boolean

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: MetricsReportingEnabled
  - GP name: Enable usage and crash-related data reporting
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:MetricsReportingEnabled
  - Value Type:REG_DWORD
  #### Example value: 
```
True
```


  ### Mac information and settings
  - Preference Key Name: MetricsReportingEnabled
  - Example value: 
```
True
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Enable network prediction (NetworkPredictionOptions)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Enables network prediction and prevents users from changing this setting.

This controls DNS prefetching, TCP and SSL preconnection, and prerendering of web pages.

If you don't configure this policy, network prediction is enabled but the user can change it.

* 0 = Predict network actions on any network connection

* 2 = Don't predict network actions on any network connection

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: Yes
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  Integer

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: NetworkPredictionOptions
  - GP name: Enable network prediction
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): Administrative Templates/Microsoft Edge - Default Settings (users can override)/
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): SOFTWARE\Policies\Microsoft\Edge\Recommended
  - Value Name:NetworkPredictionOptions
  - Value Type:REG_DWORD
  #### Example value: 
```
0x00000001
```


  ### Mac information and settings
  - Preference Key Name: NetworkPredictionOptions
  - Example value: 
```
1
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Control where security restrictions on insecure origins apply (OverrideSecurityRestrictionsOnInsecureOrigin)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Specifies a list of origins (URLs) or hostname patterns (like "*.contoso.com") for which security restrictions on insecure origins don't apply.

This policy lets you specify allowed origins for legacy applications that can't deploy TLS or set up a staging server for internal web development so that developers can test out features requiring secure contexts without having to deploy TLS on the staging server. This policy also prevents the origin from being labeled "Not Secure" in the omnibox.

Setting a list of URLs in this policy has the same effect as setting the command-line flag '--unsafely-treat-insecure-origin-as-secure' to a comma-separated list of the same URLs. If you enable this policy, it overrides the command-line flag.

For more information on secure contexts, see https://www.w3.org/TR/secure-contexts/.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: No - Requires browser restart

  ### Data Type:
  List of strings

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: OverrideSecurityRestrictionsOnInsecureOrigin
  - GP name: Control where security restrictions on insecure origins apply
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge\OverrideSecurityRestrictionsOnInsecureOrigin
  - Path (Recommended):N/A
  - Value Name:1, 2, 3, ...
  - Value Type:list of REG_SZ
  #### Example value: 
```
SOFTWARE\Policies\Microsoft\Edge\OverrideSecurityRestrictionsOnInsecureOrigin\0 = "http://testserver.contoso.com/"
SOFTWARE\Policies\Microsoft\Edge\OverrideSecurityRestrictionsOnInsecureOrigin\1 = "*.contoso.com"

```


  ### Mac information and settings
  - Preference Key Name: OverrideSecurityRestrictionsOnInsecureOrigin
  - Example value: 
```
<array>
  <string>http://testserver.contoso.com/</string>
  <string>*.contoso.com</string>
</array>

```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Enable Proactive Authentication (ProactiveAuthEnabled)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Lets you configure whether to turn on Proactive Authentication.

If you enable this policy, Microsoft Edge tries to proactively authenticate the signed-in user with Microsoft services. At regular intervals, Microsoft Edge checks with an online service for an updated manifest that contains the configuration that governs how to do this.

If you disable this policy, Microsoft Edge doesn't try to proactively authenticate the signed-in user with Microsoft services. Microsoft Edge no longer checks with an online service for an updated manifest that contains the configuration for doing this.

If you don't configure this policy, Proactive Authentication is turned on.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: No - Requires browser restart

  ### Data Type:
  Boolean

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: ProactiveAuthEnabled
  - GP name: Enable Proactive Authentication
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:ProactiveAuthEnabled
  - Value Type:REG_DWORD
  #### Example value: 
```
True
```


  ### Mac information and settings
  - Preference Key Name: ProactiveAuthEnabled
  - Example value: 
```
True
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Enable full-tab promotional content (PromotionalTabsEnabled)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Control the presentation of full-tab promotional or educational content. This setting controls the presentation of welcome pages that help users sign into Microsoft Edge, choose their default browser, or learn about product features.

If you enable this policy (set it true) or don't configure it, Microsoft Edge can show full-tab content to users to provide product information.

If you disable (set to false) this policy, Microsoft Edge can't show full-tab content to users.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  Boolean

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: PromotionalTabsEnabled
  - GP name: Enable full-tab promotional content
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:PromotionalTabsEnabled
  - Value Type:REG_DWORD
  #### Example value: 
```
False
```


  ### Mac information and settings
  - Preference Key Name: PromotionalTabsEnabled
  - Example value: 
```
False
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Ask where to save downloaded files (PromptForDownloadLocation)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Set whether to ask where to save a file before downloading it.

If you enable this policy, the user is asked where to save each file before downloading; if you don't configure it, files are saved automatically to the default location, without asking the user.

If you don't configure this policy, the user will be able to change this setting.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  Boolean

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: PromptForDownloadLocation
  - GP name: Ask where to save downloaded files
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:PromptForDownloadLocation
  - Value Type:REG_DWORD
  #### Example value: 
```
False
```


  ### Mac information and settings
  - Preference Key Name: PromptForDownloadLocation
  - Example value: 
```
False
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Allow QUIC protocol (QuicAllowed)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Allows use of the QUIC protocol in Microsoft Edge.

If you enable this policy or don't configure it, the QUIC protocol is allowed.

If you disable this policy, the QUIC protocol is blocked.

QUIC is a transport layer network protocol that can improve performance of web applications that currently use TCP.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: No - Requires browser restart

  ### Data Type:
  Boolean

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: QuicAllowed
  - GP name: Allow QUIC protocol
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:QuicAllowed
  - Value Type:REG_DWORD
  #### Example value: 
```
True
```


  ### Mac information and settings
  - Preference Key Name: QuicAllowed
  - Example value: 
```
True
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Notify a user that a browser restart is recommended or required for pending updates (RelaunchNotification)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Notify users that they need to restart Microsoft Edge to apply a pending update.

If you don't configure this policy, Microsoft Edge adds a recycle icon at the far right of the top menu bar to prompt users to restart the browser to apply the update.

If you enable this policy and set it to 'Recommended' (1), a recurring warning prompts users that a restart is recommended. Users can dismiss this warning and defer the restart.

If you set the policy to 'Required' (2), a recurring warning prompts users that the browser will be restarted automatically as soon as a notification period passes. The default period is seven days. You can configure this period with the 'RelaunchNotificationPeriod' policy.

The user's session is restored when the browser restarts.

* Recommended (1) = Show a recurring prompt to the user indicating that a restart is recommended

* Required (2) = Show a recurring prompt to the user indicating that a restart is required

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  Integer

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: RelaunchNotification
  - GP name: Notify a user that a browser restart is recommended or required for pending updates
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:RelaunchNotification
  - Value Type:REG_DWORD
  #### Example value: 
```
0x00000001
```


  ### Mac information and settings
  - Preference Key Name: RelaunchNotification
  - Example value: 
```
1
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Set the time period for update notifications (RelaunchNotificationPeriod)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Sets the time period, in milliseconds, over which users are notified that Microsoft Edge must be restarted to apply a pending update.

During this time period, the user is repeatedly informed that they need to restart. The app menu changes to indicate that a restart is needed when one third of the notification period passes. When two thirds of the notification period passes, the notification changes color, and again when the full notification period has passed. Additional notifications enabled by the 'RelaunchNotification' policy follow this same schedule.

If you don't configure this policy, the default period is 604800000 milliseconds (one week).

Restrictions:

* Minimum:3600000

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  Integer

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: RelaunchNotificationPeriod
  - GP name: Set the time period for update notifications
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:RelaunchNotificationPeriod
  - Value Type:REG_DWORD
  #### Example value: 
```
0x240c8400
```


  ### Mac information and settings
  - Preference Key Name: RelaunchNotificationPeriod
  - Example value: 
```
604800000
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Specify if online OCSP/CRL checks are required for local trust anchors (RequireOnlineRevocationChecksForLocalAnchors)
  >Supported Versions: Microsoft Edge on Windows since version 77 or later
  

  ### Description
  Control whether online revocation checks (OCSP/CRL checks) are required. If Microsoft Edge can't get revocation status information, these certificates are treated as revoked ("hard-fail").

If you enable this policy, Microsoft Edge always performs revocation checking for server certificates that successfully validate and are signed by locally-installed CA certificates.

If you don't configure or disable this policy, then Microsoft Edge uses the existing online revocation checking settings.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  Boolean

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: RequireOnlineRevocationChecksForLocalAnchors
  - GP name: Specify if online OCSP/CRL checks are required for local trust anchors
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:RequireOnlineRevocationChecksForLocalAnchors
  - Value Type:REG_DWORD
  #### Example value: 
```
False
```


  

  [Back to Top](#Edge-Policy-Documentation)

  ## Enable resolution of navigation errors using a web service (ResolveNavigationErrorsUseWebService)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Allow Microsoft Edge to issue a dataless connection to a web service to probe networks for connectivity in cases like hotel and airport Wi-Fi.

If you enable this policy, a web service is used for network connectivity tests.

If you disable this policy, Microsoft Edge uses native APIs to try to resolve network connectivity and navigation issues.

**Note**: Except on Windows 8 and later versions of Windows, Microsoft Edge *always* uses native APIs to resolve connectivity issues.

If you don't configure this policy, Microsoft Edge respects the user preference that's set under Services at edge://settings/privacy.
Specifically, there's a **Use a web service to help resolve navigation errors** toggle, which the user can switch on or off. Be aware that if you have enabled this policy (ResolveNavigationErrorsUseWebService), the **Use a web service to help resolve navigation errors** setting is turned on, but the user can't change the setting by using the toggle. If you have disabled this policy, the **Use a web service to help resolve navigation errors** setting is turned off, and the user can't change the setting by using the toggle.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: Yes
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  Boolean

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: ResolveNavigationErrorsUseWebService
  - GP name: Enable resolution of navigation errors using a web service
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): Administrative Templates/Microsoft Edge - Default Settings (users can override)/
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): SOFTWARE\Policies\Microsoft\Edge\Recommended
  - Value Name:ResolveNavigationErrorsUseWebService
  - Value Type:REG_DWORD
  #### Example value: 
```
True
```


  ### Mac information and settings
  - Preference Key Name: ResolveNavigationErrorsUseWebService
  - Example value: 
```
True
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Restrict which accounts can be used as Microsoft Edge primary accounts (RestrictSigninToPattern)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Determines which accounts can be set as browser primary accounts in Microsoft Edge (the account that is chosen during the Sync opt-in flow).

If a user tries to set a browser primary account with a username that doesn't match this pattern, they are blocked and see an appropriate error message.

If you don't configure this policy or leave it blank, users can set any account as a browser primary account in Microsoft Edge.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  String

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: RestrictSigninToPattern
  - GP name: Restrict which accounts can be used as Microsoft Edge primary accounts
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:RestrictSigninToPattern
  - Value Type:REG_SZ
  #### Example value: 
```
".*@contoso.com"
```


  ### Mac information and settings
  - Preference Key Name: RestrictSigninToPattern
  - Example value: 
```
".*@contoso.com"
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Extend Adobe Flash content setting to all content (RunAllFlashInAllowMode)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  If you enable this policy, all Adobe Flash content embedded in websites that are set to allow Adobe Flash in the content settings -- either by the user or by enterprise policy -- will run. This includes content from other origins and/or small content.

To control which websites are allowed to run Adobe Flash, see the specifications in the 'DefaultPluginsSetting', 'PluginsAllowedForUrls', and 'PluginsBlockedForUrls' policies.

If you disable this policy or don't configure it, Adobe Flash content from other origins (from sites that aren't specified in the three policies mentioned immediately above) or small content might be blocked.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  Boolean

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: RunAllFlashInAllowMode
  - GP name: Extend Adobe Flash content setting to all content
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:RunAllFlashInAllowMode
  - Value Type:REG_DWORD
  #### Example value: 
```
True
```


  ### Mac information and settings
  - Preference Key Name: RunAllFlashInAllowMode
  - Example value: 
```
True
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Allow users to proceed from the SSL warning page (SSLErrorOverrideAllowed)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Microsoft Edge shows a warning page when users visit sites that have SSL errors.

If you enable or don't configured (default) this policy, users can click through these warning pages.

If you disable this policy, users are blocked from clicking through any warning page.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  Boolean

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: SSLErrorOverrideAllowed
  - GP name: Allow users to proceed from the SSL warning page
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:SSLErrorOverrideAllowed
  - Value Type:REG_DWORD
  #### Example value: 
```
True
```


  ### Mac information and settings
  - Preference Key Name: SSLErrorOverrideAllowed
  - Example value: 
```
True
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Minimum SSL version enabled (SSLVersionMin)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Sets the minimum supported version of SSL. If you don't configure this policy, Microsoft Edge uses a default minimum version, TLS 1.0.

If you enable this policy, you can set the minimum version to one of the following values: "tls1", "tls1.1" or "tls1.2". When set, Microsoft Edge won't use any version of SSL/TLS lower than the specified version. Any unrecognized value is ignored.

* "tls1" = TLS 1.0

* "tls1.1" = TLS 1.1

* "tls1.2" = TLS 1.2

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  String

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: SSLVersionMin
  - GP name: Minimum SSL version enabled
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:SSLVersionMin
  - Value Type:REG_SZ
  #### Example value: 
```
"tls1"
```


  ### Mac information and settings
  - Preference Key Name: SSLVersionMin
  - Example value: 
```
"tls1"
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Disable saving browser history (SavingBrowserHistoryDisabled)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Disables saving browser history and prevents users from changing this setting.

If you enable this policy, browsing history isn't saved. This also disables tab syncing.

If you disable this policy or don't configure it, browsing history is saved.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  Boolean

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: SavingBrowserHistoryDisabled
  - GP name: Disable saving browser history
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:SavingBrowserHistoryDisabled
  - Value Type:REG_DWORD
  #### Example value: 
```
True
```


  ### Mac information and settings
  - Preference Key Name: SavingBrowserHistoryDisabled
  - Example value: 
```
True
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Enable search suggestions (SearchSuggestEnabled)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Enables web search suggestions in Microsoft Edge's Address Bar and Auto-Suggest List and prevents users from changing this policy.

If you enable this policy, web search suggestions are used.

If you disable this policy, web search suggestions are never used, however local history and local favorites suggestions still appear. If you disable this policy, neither the typed characters, nor the URLs visited will be included in telemetry to Microsoft.

If this policy is left not set, search suggestions are enabled but the user can change that.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: Yes
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  Boolean

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: SearchSuggestEnabled
  - GP name: Enable search suggestions
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): Administrative Templates/Microsoft Edge - Default Settings (users can override)/
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): SOFTWARE\Policies\Microsoft\Edge\Recommended
  - Value Name:SearchSuggestEnabled
  - Value Type:REG_DWORD
  #### Example value: 
```
True
```


  ### Mac information and settings
  - Preference Key Name: SearchSuggestEnabled
  - Example value: 
```
True
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Websites or domains that don't need permission to use direct Security Key attestation (SecurityKeyPermitAttestation)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Specifies websites and domains that don't need explicit user permission when attestation certificates from security keys are requested. Additionally, a signal is sent to the security key indicating that it can use individual attestation. Without this, users are prompted each time a site requests attestation of security keys.

Sites (like https://contoso.com/some/path) only match as U2F appIDs. Domains (like contoso.com) only match as webauthn RP IDs. To cover both U2F and webauthn APIs for a given site, you need to list both the appID URL and domain.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  List of strings

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: SecurityKeyPermitAttestation
  - GP name: Websites or domains that don't need permission to use direct Security Key attestation
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge\SecurityKeyPermitAttestation
  - Path (Recommended):N/A
  - Value Name:1, 2, 3, ...
  - Value Type:list of REG_SZ
  #### Example value: 
```
SOFTWARE\Policies\Microsoft\Edge\SecurityKeyPermitAttestation\0 = "https://contoso.com"

```


  ### Mac information and settings
  - Preference Key Name: SecurityKeyPermitAttestation
  - Example value: 
```
<array>
  <string>https://contoso.com</string>
</array>

```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Send all intranet sites to Internet Explorer (SendIntranetToInternetExplorer)
  >Supported Versions: Microsoft Edge on Windows since version 77 or later
  

  ### Description
  Allows you to configure whether your intranet sites are opened in Internet Explorer.

If you enable this policy, all intranet sites are automatically opened using the setting that’s configured in the ‘Configure Internet Explorer integration’ (‘InternetExplorerIntegrationLevel’) policy. The only exceptions are those sites configured with the open-in element in your Enterprise Mode Site List.

If you disable or don't configure this policy, your intranet sites are opened in Microsoft Edge, except for the sites listed in the Enterprise Mode Site List.

To enable this policy, you must first enable the ‘Configure Internet Explorer integration’ (‘InternetExplorerIntegrationLevel’) policy. Otherwise, this policy has no effect.

We strongly recommend keeping this policy in sync with the ‘Keep all intranet sites in Internet Explorer’ (‘KeepIntranetSitesInInternetExplorer’) policy. Additionally, it’s best to enable this policy only if your intranet sites have known compatibility problems with Microsoft Edge.

Related policies:
- Configure Internet Explorer integration (‘InternetExplorerIntegrationLevel’)
- Configure which version of Microsoft Edge to use for opening redirected sites (‘NeedEdgeBrowser’)
- Send all sites not included in the Enterprise Mode Site List to Microsoft Edge (‘SendIntranetToInternetExplorer’)
- Keep all intranet sites in Internet Explorer (‘KeepIntranetSitesInInternetExplorer’)

For more info about how to use this policy together with these related policies to create the optimal configuration for your organization, see https://go.microsoft.com/fwlink/?linkid=2094210.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: No - Requires browser restart

  ### Data Type:
  Boolean

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: SendIntranetToInternetExplorer
  - GP name: Send all intranet sites to Internet Explorer
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:SendIntranetToInternetExplorer
  - Value Type:REG_DWORD
  #### Example value: 
```
True
```


  

  [Back to Top](#Edge-Policy-Documentation)

  ## Send site information to improve Microsoft services (SendSiteInfoToImproveServices)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  This policy setting lets you decide whether users can send info about websites they visit in Microsoft Edge to Microsoft to improve services like search. The default value is taken from install.

If you enable this setting, info about websites visited in Microsoft Edge is always sent to Microsoft.

If you disable this setting, info about websites visited in Microsoft Edge is never sent to Microsoft.

If you don't configure this setting, users can choose whether or not to send website info to Microsoft.

Windows 7, 8, and Mac: Controls sending info about websites visited in Microsoft Edge to Microsoft.

Windows 10 (Edge Canary, Beta, Dev): Controls sending info about websites visited in Microsoft Edge to Microsoft.

Windows 10 (Edge stable): This policy doesn't control sending website info to Microsoft. This is controlled by the Windows Diagnostic Data setting

See https://docs.microsoft.com/en-us/windows/privacy/configure-windows-diagnostic-data-in-your-organization#overview

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: No - Requires browser restart

  ### Data Type:
  Boolean

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: SendSiteInfoToImproveServices
  - GP name: Send site information to improve Microsoft services
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:SendSiteInfoToImproveServices
  - Value Type:REG_DWORD
  #### Example value: 
```
False
```


  ### Mac information and settings
  - Preference Key Name: SendSiteInfoToImproveServices
  - Example value: 
```
False
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Show Microsoft Office shortcut in favorites bar (ShowOfficeShortcutInFavoritesBar)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Specifies whether to include a shortcut to Office.com in the favorites bar. For users signed into Microsoft Edge the shortcut takes users to their Microsoft Office apps and docs.

If this policy is enabled or not configure, users can choose whether to see the shortcut by changing the toggle in the favorites bar context menu.

If the policy is disabled, the shortcut won't be shown.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  Boolean

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: ShowOfficeShortcutInFavoritesBar
  - GP name: Show Microsoft Office shortcut in favorites bar
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:ShowOfficeShortcutInFavoritesBar
  - Value Type:REG_DWORD
  #### Example value: 
```
False
```


  ### Mac information and settings
  - Preference Key Name: ShowOfficeShortcutInFavoritesBar
  - Example value: 
```
False
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Enable site isolation for every site (SitePerProcess)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Enables site isolation using the 'IsolateOrigins' and 'SitePerProcess' features.
If the policy is enabled, each site will run in its own process.
If you disable this policy, both 'IsolateOrigins' and 'SitePerProcess' features are disabled. Users can enable 'SitePerProcess' policy manually, by using command line flags.
If you don't configure this policy, the user can change this setting.
You may want to consider the 'IsolateOrigins' policy setting to get the best of both worlds, isolation and limited impact for users, by using 'IsolateOrigins' with a list of the sites you want to isolate.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: No - Requires browser restart

  ### Data Type:
  Boolean

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: SitePerProcess
  - GP name: Enable site isolation for every site
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:SitePerProcess
  - Value Type:REG_DWORD
  #### Example value: 
```
True
```


  ### Mac information and settings
  - Preference Key Name: SitePerProcess
  - Example value: 
```
True
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Enable spellcheck (SpellcheckEnabled)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  If you enable or don't configure this policy, the user can use spellcheck.

If you disable this policy, the user can't use spellcheck and the 'SpellcheckLanguage' policy is also disabled.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  Boolean

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: SpellcheckEnabled
  - GP name: Enable spellcheck
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:SpellcheckEnabled
  - Value Type:REG_DWORD
  #### Example value: 
```
False
```


  ### Mac information and settings
  - Preference Key Name: SpellcheckEnabled
  - Example value: 
```
False
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Enable specific spellcheck languages (SpellcheckLanguage)
  >Supported Versions: Microsoft Edge on Windows since version 77 or later
  

  ### Description
  Enables different languages for spellcheck. Any language that you specify that isn't recognized is ignored.

If you enable this policy, spellcheck is enabled for the languages specified, as well as any languages the user has enabled.

If you don't configure or disable this policy, there's no change to the user's spellcheck preferences.

If the 'SpellcheckEnabled' policy is disabled, this policy will have no effect.

The supported languages are: af, bg, ca, cs, cy, da, de, el, en-AU, en-CA, en-GB, en-US, es, es-419, es-AR, es-ES, es-MX, es-US, et, fa, fo, fr, he, hi, hr, hu, id, it, ko, lt, lv, nb, nl, pl, pt-BR, pt-PT, ro, ru, sh, sk, sl, sq, sr, sv, ta, tg, tr, uk, vi.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  List of strings

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: SpellcheckLanguage
  - GP name: Enable specific spellcheck languages
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge\SpellcheckLanguage
  - Path (Recommended):N/A
  - Value Name:1, 2, 3, ...
  - Value Type:list of REG_SZ
  #### Example value: 
```
SOFTWARE\Policies\Microsoft\Edge\SpellcheckLanguage\0 = "fr"
SOFTWARE\Policies\Microsoft\Edge\SpellcheckLanguage\1 = "es"

```


  

  [Back to Top](#Edge-Policy-Documentation)

  ## Suppress the unsupported OS warning (SuppressUnsupportedOSWarning)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Suppresses the warning that appears when Microsoft Edge is running on a computer or operating system that is no longer supported.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: No - Requires browser restart

  ### Data Type:
  Boolean

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: SuppressUnsupportedOSWarning
  - GP name: Suppress the unsupported OS warning
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:SuppressUnsupportedOSWarning
  - Value Type:REG_DWORD
  #### Example value: 
```
True
```


  ### Mac information and settings
  - Preference Key Name: SuppressUnsupportedOSWarning
  - Example value: 
```
True
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Disable synchronization of data using Microsoft sync services (SyncDisabled)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Disables data synchronization in Microsoft Edge and prevents users from modifying this setting.

If this policy is not set, users will be able to either turn on or turn off sync.

Do not enable this policy when the policy 'RoamingProfileSupportEnabled' is enabled, as 'RoamingProfileSupportEnabled' duplicates the sync functionality.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: Yes
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  Boolean

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: SyncDisabled
  - GP name: Disable synchronization of data using Microsoft sync services
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): Administrative Templates/Microsoft Edge - Default Settings (users can override)/
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): SOFTWARE\Policies\Microsoft\Edge\Recommended
  - Value Name:SyncDisabled
  - Value Type:REG_DWORD
  #### Example value: 
```
True
```


  ### Mac information and settings
  - Preference Key Name: SyncDisabled
  - Example value: 
```
True
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Configure tab lifecycles (TabLifecyclesEnabled)
  >Supported Versions: Microsoft Edge on Windows since version 77 or later
  

  ### Description
  The tab lifecycles feature reclaims CPU and memory associated with running tabs that haven't been used in a long time, by first throttling, then freezing, and finally discarding them.

If you disable this policy, the tab lifecycles feature is disabled, and all tabs are left running normally.

If you enable or don't configure this policy, the tab lifecycles feature is enabled.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: No - Requires browser restart

  ### Data Type:
  Boolean

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: TabLifecyclesEnabled
  - GP name: Configure tab lifecycles
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:TabLifecyclesEnabled
  - Value Type:REG_DWORD
  #### Example value: 
```
False
```


  

  [Back to Top](#Edge-Policy-Documentation)

  ## Enable ending processes in the Browser task manager (TaskManagerEndProcessEnabled)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  If you enable or don't configure this policy, users can end processes in the Browser task manager. If you disable it, users can't end processes, and the End process button is disabled in the Browser task manager.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  Boolean

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: TaskManagerEndProcessEnabled
  - GP name: Enable ending processes in the Browser task manager
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:TaskManagerEndProcessEnabled
  - Value Type:REG_DWORD
  #### Example value: 
```
True
```


  ### Mac information and settings
  - Preference Key Name: TaskManagerEndProcessEnabled
  - Example value: 
```
True
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Enable Translate (TranslateEnabled)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Enables the integrated Microsoft translation service on Microsoft Edge.

If you enable this policy, Microsoft Edge offers translation functionality to the user by showing an integrated translate flyout (when appropriate) and a translate option on the right-click context menu.

Disable this policy to disable all built-in translate features.

If you don't configure the policy, users can choose whether to use the translation functionality or not.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: Yes
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  Boolean

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: TranslateEnabled
  - GP name: Enable Translate
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended): Administrative Templates/Microsoft Edge - Default Settings (users can override)/
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended): SOFTWARE\Policies\Microsoft\Edge\Recommended
  - Value Name:TranslateEnabled
  - Value Type:REG_DWORD
  #### Example value: 
```
True
```


  ### Mac information and settings
  - Preference Key Name: TranslateEnabled
  - Example value: 
```
True
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Define a list of allowed URLs (URLAllowlist)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Allow access to the listed URLs, as exceptions to the URL block list.

Format the URL pattern according to https://docs.microsoft.com//Placeholder01 .

You can use this policy to open exceptions to restrictive block lists. For example, you can include '*' in the block list to block all requests, and then use this policy to allow access to a limited list of URLs. You can use this policy to open exceptions to certain schemes, subdomains of other domains, ports, or specific paths.

The most specific filter determines if a URL is blocked or allowed. The allowed list takes precedence over the block list.

This policy is limited to 1000 entries; subsequent entries are ignored.

If you don't configure this policy, there are no exceptions to the block list in the 'URLBlocklist' policy.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  List of strings

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: URLAllowlist
  - GP name: Define a list of allowed URLs
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge\URLAllowlist
  - Path (Recommended):N/A
  - Value Name:1, 2, 3, ...
  - Value Type:list of REG_SZ
  #### Example value: 
```
SOFTWARE\Policies\Microsoft\Edge\URLAllowlist\0 = "contoso.com"
SOFTWARE\Policies\Microsoft\Edge\URLAllowlist\1 = "https://ssl.server.com"
SOFTWARE\Policies\Microsoft\Edge\URLAllowlist\2 = "hosting.com/good_path"
SOFTWARE\Policies\Microsoft\Edge\URLAllowlist\3 = "https://server:8080/path"
SOFTWARE\Policies\Microsoft\Edge\URLAllowlist\4 = ".exact.hostname.com"

```


  ### Mac information and settings
  - Preference Key Name: URLAllowlist
  - Example value: 
```
<array>
  <string>contoso.com</string>
  <string>https://ssl.server.com</string>
  <string>hosting.com/good_path</string>
  <string>https://server:8080/path</string>
  <string>.exact.hostname.com</string>
</array>

```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Block access to a list of URLs (URLBlocklist)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Define a list of sites, based on URL patterns, that are blocked (your users can't load them).

Format the URL pattern according to https://docs.microsoft.com//Placeholder01.

You can define exceptions in the 'URLAllowlist' policy. These policies are limited to 1000 entries; subsequent entries are ignored.

Note that blocking internal 'edge://*' URLs isn't recommended - this may lead to unexpected errors.

This policy doesn't prevent the page from updating dynamically through JavaScript. For example, if you block 'contoso.com/abc', users might still be able to visit 'contoso.com' and click on a link to visit 'contoso.com/abc', as long as the page doesn't refresh.

If you don't configure this policy, no URLs are blocked.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  List of strings

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: URLBlocklist
  - GP name: Block access to a list of URLs
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge\URLBlocklist
  - Path (Recommended):N/A
  - Value Name:1, 2, 3, ...
  - Value Type:list of REG_SZ
  #### Example value: 
```
SOFTWARE\Policies\Microsoft\Edge\URLBlocklist\0 = "contoso.com"
SOFTWARE\Policies\Microsoft\Edge\URLBlocklist\1 = "https://ssl.server.com"
SOFTWARE\Policies\Microsoft\Edge\URLBlocklist\2 = "hosting.com/bad_path"
SOFTWARE\Policies\Microsoft\Edge\URLBlocklist\3 = "https://server:8080/path"
SOFTWARE\Policies\Microsoft\Edge\URLBlocklist\4 = ".exact.hostname.com"
SOFTWARE\Policies\Microsoft\Edge\URLBlocklist\5 = "file://*"
SOFTWARE\Policies\Microsoft\Edge\URLBlocklist\6 = "custom_scheme:*"
SOFTWARE\Policies\Microsoft\Edge\URLBlocklist\7 = "*"

```


  ### Mac information and settings
  - Preference Key Name: URLBlocklist
  - Example value: 
```
<array>
  <string>contoso.com</string>
  <string>https://ssl.server.com</string>
  <string>hosting.com/bad_path</string>
  <string>https://server:8080/path</string>
  <string>.exact.hostname.com</string>
  <string>file://*</string>
  <string>custom_scheme:*</string>
  <string>*</string>
</array>

```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Set the user data directory (UserDataDir)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Set the directory to use for storing user data.

If you enable this policy, Microsoft Edge uses the specified directory regardless of whether the user has set the '--user-data-dir' command-line flag.

If you don't enable this policy, the default profile path is used, but the user can override it by using the '--user-data-dir' flag. Users can find the directory for the profile at edge://version/ under profile path.

To avoid data loss or other errors, don't configure this policy to a volume's root directory or to a directory that's used for other purposes, because Microsoft Edge manages its contents.

See https://docs.microsoft.com/Placeholder08 for a list of variables that can be used.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: No - Requires browser restart

  ### Data Type:
  String

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: UserDataDir
  - GP name: Set the user data directory
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:UserDataDir
  - Value Type:REG_SZ
  #### Example value: 
```
"${users}/${user_name}/Edge"
```


  ### Mac information and settings
  - Preference Key Name: UserDataDir
  - Example value: 
```
"${users}/${user_name}/Edge"
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Allow user feedback (UserFeedbackAllowed)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Microsoft Edge uses the Edge Feedback feature (enabled by default) to allow users to send feedback, suggestions or customer surveys and to report any issues with the browser. Also, by default, users can't disable (turn off) the Edge Feedback feature.

If you enable this policy or don't configure it, users can invoke Edge Feedback.

If you disable this policy, users can't invoke Edge Feedback.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: No - Requires browser restart

  ### Data Type:
  Boolean

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: UserFeedbackAllowed
  - GP name: Allow user feedback
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:UserFeedbackAllowed
  - Value Type:REG_DWORD
  #### Example value: 
```
True
```


  ### Mac information and settings
  - Preference Key Name: UserFeedbackAllowed
  - Example value: 
```
True
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Allow or block video capture (VideoCaptureAllowed)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Control whether sites can capture video.

If enabled or not configured (default), the user will be asked about video capture access for all sites except those with URLs configured in the 'VideoCaptureAllowedUrls' policy list, which will be granted access without prompting.

If you disable this policy, the user isn't prompted, and video capture is only available to URLs configured in 'VideoCaptureAllowedUrls' policy.

This policy affects all types of video inputs, not only the built-in camera.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  Boolean

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: VideoCaptureAllowed
  - GP name: Allow or block video capture
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:VideoCaptureAllowed
  - Value Type:REG_DWORD
  #### Example value: 
```
False
```


  ### Mac information and settings
  - Preference Key Name: VideoCaptureAllowed
  - Example value: 
```
False
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Sites that can access video capture devices without requesting permission (VideoCaptureAllowedUrls)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Specify websites, based on URL patterns, that can use video capture devices without asking the user for permission. Patterns in this list are matched against the security origin of the requesting URL. If they match, the site is automatically granted access to video capture devices.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: Yes

  ### Data Type:
  List of strings

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: VideoCaptureAllowedUrls
  - GP name: Sites that can access video capture devices without requesting permission
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge\VideoCaptureAllowedUrls
  - Path (Recommended):N/A
  - Value Name:1, 2, 3, ...
  - Value Type:list of REG_SZ
  #### Example value: 
```
SOFTWARE\Policies\Microsoft\Edge\VideoCaptureAllowedUrls\0 = "https://www.contoso.com/"
SOFTWARE\Policies\Microsoft\Edge\VideoCaptureAllowedUrls\1 = "https://[*.]contoso.edu/"

```


  ### Mac information and settings
  - Preference Key Name: VideoCaptureAllowedUrls
  - Example value: 
```
<array>
  <string>https://www.contoso.com/</string>
  <string>https://[*.]contoso.edu/</string>
</array>

```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Set WPAD optimization (WPADQuickCheckEnabled)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Allows you to turn off WPAD (Web Proxy Auto-Discovery) optimization in Microsoft Edge.

If you disable this policy, WPAD optimization is disabled, which makes the browser wait longer for DNS-based WPAD servers.

If you enable or don't configure the policy, WPAD optimization is enabled.

Independent of whether or how this policy is enabled, the WPAD optimization setting cannot be changed by users.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: No - Requires browser restart

  ### Data Type:
  Boolean

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: WPADQuickCheckEnabled
  - GP name: Set WPAD optimization
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:WPADQuickCheckEnabled
  - Value Type:REG_DWORD
  #### Example value: 
```
True
```


  ### Mac information and settings
  - Preference Key Name: WPADQuickCheckEnabled
  - Example value: 
```
True
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Allow WebDriver to Override Incompatible Policies (WebDriverOverridesIncompatiblePolicies)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  This policy lets users of the WebDriver interface override policies that could interfere with its operation.

If you enable this policy, WebDriver can be configured to override incompatible policies.

If you disable this policy or don't configure it, WebDriver can't be configured to override incompatible policies.

Note: Currently, the 'SitePerProcess' and 'IsolateOrigins' policies have been verified to interfere with WebDriver operations. In the future, additional policies may be determined to interfere with WebDriver.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: No - Requires browser restart

  ### Data Type:
  Boolean

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: WebDriverOverridesIncompatiblePolicies
  - GP name: Allow WebDriver to Override Incompatible Policies
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:WebDriverOverridesIncompatiblePolicies
  - Value Type:REG_DWORD
  #### Example value: 
```
True
```


  ### Mac information and settings
  - Preference Key Name: WebDriverOverridesIncompatiblePolicies
  - Example value: 
```
True
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Restrict exposure of localhost IP address by WebRTC (WebRtcLocalhostIpHandling)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Allows you to set whether or not WebRTC exposes the user's localhost IP address.

If you set this policy to "AllowAllInterfaces" ('default') or "AllowPublicAndPrivateInterfaces" ('default_public_and_private_interfaces'), WebRTC exposes the localhost IP address.

If you set this policy to "AllowPublicInterfaceOnly" ('default_public_interface_only') or "DisableNonProxiedUdp" ('disable_non_proxied_udp'), WebRTC doesn't expose the localhost IP address.

If you don't set this policy, or if you disable it, WebRTC exposes the localhost IP address.

  * 'default' = Allow all interfaces. This exposes the localhost IP address.
  * 'default_public_and_private_interfaces' = Allow public and private interfaces over http default route. This exposes the localhost IP address.
  * 'default_public_interface_only' = Allow public interface over http default route. This doesn't expose the localhost IP address.
  * 'disable_non_proxied_udp' = Use TCP unless proxy server supports UDP. This doesn't expose the localhost IP address.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: No - Requires browser restart

  ### Data Type:
  String

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: WebRtcLocalhostIpHandling
  - GP name: Restrict exposure of localhost IP address by WebRTC
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:WebRtcLocalhostIpHandling
  - Value Type:REG_SZ
  #### Example value: 
```
"default"
```


  ### Mac information and settings
  - Preference Key Name: WebRtcLocalhostIpHandling
  - Example value: 
```
"default"
```
  

  [Back to Top](#Edge-Policy-Documentation)

  ## Restrict the range of local UDP ports used by WebRTC (WebRtcUdpPortRange)
  >Supported Versions: Microsoft Edge on Windows and Mac since version 77 or later
  

  ### Description
  Restricts the UDP port range used by WebRTC to a specified port interval (endpoints included).

If you don't configure this policy or set it to an empty string or invalid port range, WebRTC can use any available local UDP port.

  ### Supported features:
  - Can be mandatory: Yes
  - Can be recommended: No
  - Dynamic Policy Refresh: No - Requires browser restart

  ### Data Type:
  String

  ### Windows information and settings
  #### Group Policy (ADMX) info
  - GP unique name: WebRtcUdpPortRange
  - GP name: Restrict the range of local UDP ports used by WebRTC
  - GP path (Mandatory): Administrative Templates/Microsoft Edge/
  - GP path (Recommended):N/A
  - GP ADMX file name: MSEdge.admx
  #### Windows Registry Settings
  - Path (Mandatory): SOFTWARE\Policies\Microsoft\Edge
  - Path (Recommended):N/A
  - Value Name:WebRtcUdpPortRange
  - Value Type:REG_SZ
  #### Example value: 
```
"10000-11999"
```


  ### Mac information and settings
  - Preference Key Name: WebRtcUdpPortRange
  - Example value: 
```
"10000-11999"
```
  

  [Back to Top](#Edge-Policy-Documentation)
