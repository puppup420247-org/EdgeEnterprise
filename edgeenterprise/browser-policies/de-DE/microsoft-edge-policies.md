---
title: "Microsoft Edge Browser Policy Documentation"
ms.author: stmoody
author: brianalt-msft
manager: tahills
ms.date: 11/18/2019
audience: ITPro
ms.topic: reference
ms.prod: microsoft-edge
ms.localizationpriority: medium
ms.collection: M365-modern-desktop
ms.custom:
description: "Windows and Mac documentation for all policies supported by the Microsoft Edge Browser"
---

# Microsoft Edge – Richtlinien
Die neueste Version von Microsoft Edge enthält die folgenden Richtlinien. Mit diesen Richtlinien können Sie konfigurieren, wie Microsoft Edge in Ihrer Organisation ausgeführt wird.

Informationen zu einem zusätzlichen Satz von Richtlinien, die steuern, wie und wann Microsoft Edge aktualisiert wird, finden Sie unter [Microsoft Edge Update: Verweis auf Richtlinie](microsoft-edge-update-policies.md).

> [!HINWEIS]
> Dieser Artikel gilt für Microsoft Edge, Version 77 oder höher.

## Verfügbare Richtlinien
In diesen Tabellen werden alle browserbezogenen Gruppenrichtlinien aufgelistet, die in dieser Version von Microsoft Edge verfügbar sind. Verwenden Sie die Verknüpfungen in der Tabelle, um weitere Informationen zu bestimmten Richtlinien zu erhalten.

|||
|-|-|
|[Cast](#cast)|[Drucken](#drucken)|
|[Erweiterungen](#erweiterungen)|[HTTP-Authentifizierung](#http-authentifizierung)|
|[Inhaltseinstellungen](#inhaltseinstellungen)|[Kennwort-Manager und -schutz](#kennwort-manager-und--schutz)|
|[Natives Messaging](#natives-messaging)|[Proxyserver](#proxyserver)|
|[SmartScreen-Einstellungen](#smartscreen-einstellungen)|[Standardsuchanbieter](#standardsuchanbieter)|
|[Start, Startseite und neue Tabseite](#start-startseite-und-neue-tabseite)|[Additional](#additional)|


### [*Cast*](#cast-policies)
|Richtlinienname|Beschriftung|
|-|-|
|[EnableMediaRouter](#enablemediarouter)|Google Cast aktivieren|
|[ShowCastIconInToolbar](#showcasticonintoolbar)|Wiedergabesymbol in der Symbolleiste anzeigen|
### [*Drucken*](#drucken-policies)
|Richtlinienname|Beschriftung|
|-|-|
|[DefaultPrinterSelection](#defaultprinterselection)|Standardmäßige Druckerauswahl-Regeln|
|[PrintHeaderFooter](#printheaderfooter)|Kopf- und Fußzeilen drucken|
|[PrintPreviewUseSystemDefaultPrinter](#printpreviewusesystemdefaultprinter)|Den Systemstandarddrucker als Standarddrucker festlegen|
|[PrintingEnabled](#printingenabled)|Drucken ermöglichen|
|[UseSystemPrintDialog](#usesystemprintdialog)|Über Systemdruckdialogfeld drucken|
### [*Erweiterungen*](#erweiterungen-policies)
|Richtlinienname|Beschriftung|
|-|-|
|[ExtensionAllowedTypes](#extensionallowedtypes)|Zulässige Erweiterungstypen konfigurieren|
|[ExtensionInstallAllowlist](#extensioninstallallowlist)|Installation bestimmter Erweiterungen zulassen|
|[ExtensionInstallBlocklist](#extensioninstallblocklist)|Steuern, welche Erweiterungen nicht installiert werden können|
|[ExtensionInstallForcelist](#extensioninstallforcelist)|Steuern, welche Erweiterungen automatisch installiert werden|
|[ExtensionInstallSources](#extensioninstallsources)|Erweiterung und Benutzer-Skriptinstallationsquellen konfigurieren|
|[ExtensionSettings](#extensionsettings)|Einstellungen für Erweiterungsverwaltung konfigurieren|
### [*HTTP-Authentifizierung*](#http-authentifizierung-policies)
|Richtlinienname|Beschriftung|
|-|-|
|[AllowCrossOriginAuthPrompt](#allowcrossoriginauthprompt)|Übergreifende HTTP-Basic-Authentifizierungsaufforderungen zulassen|
|[AuthNegotiateDelegateAllowlist](#authnegotiatedelegateallowlist)|Gibt eine Liste der Server an, an die Microsoft Edge Anmeldeinformationen von Benutzern delegieren kann|
|[AuthSchemes](#authschemes)|Unterstützte Authentifizierungsschemas|
|[AuthServerAllowlist](#authserverallowlist)|Liste der zugelassenen Authentifizierungsserver konfigurieren|
|[DisableAuthNegotiateCnameLookup](#disableauthnegotiatecnamelookup)|CNAME-Lookup beim Aushandeln der Kerberos-Authentifizierung deaktivieren|
|[EnableAuthNegotiatePort](#enableauthnegotiateport)|Nicht standardmäßigen Port in Kerberos-SPN einschließen|
|[NtlmV2Enabled](#ntlmv2enabled)|Steuern, ob die NTLMv2-Authentifizierung aktiviert ist|
### [*Inhaltseinstellungen*](#inhaltseinstellungen-policies)
|Richtlinienname|Beschriftung|
|-|-|
|[AutoSelectCertificateForUrls](#autoselectcertificateforurls)|Clientzertifikate für diese Websites automatisch auswählen|
|[CookiesAllowedForUrls](#cookiesallowedforurls)|Cookies auf bestimmten Websites zulassen|
|[CookiesBlockedForUrls](#cookiesblockedforurls)|Cookies auf bestimmten Websites blockieren|
|[CookiesSessionOnlyForUrls](#cookiessessiononlyforurls)|Cookies von bestimmten Websites auf die aktuelle Sitzung beschränken|
|[DefaultCookiesSetting](#defaultcookiessetting)|Cookies konfigurieren|
|[DefaultGeolocationSetting](#defaultgeolocationsetting)|Standardeinstellung für Geolocation|
|[DefaultImagesSetting](#defaultimagessetting)|Standardeinstellung für Bilder|
|[DefaultJavaScriptSetting](#defaultjavascriptsetting)|Standard-JavaScript-Einstellung|
|[DefaultNotificationsSetting](#defaultnotificationssetting)|Standard-Benachrichtigungseinstellung|
|[DefaultPluginsSetting](#defaultpluginssetting)|Standardeinstellung für Adobe Flash|
|[DefaultPopupsSetting](#defaultpopupssetting)|Standardeinstellung für Popupfenster|
|[DefaultWebBluetoothGuardSetting](#defaultwebbluetoothguardsetting)|Verwendung der Web-Bluetooth-API steuern|
|[DefaultWebUsbGuardSetting](#defaultwebusbguardsetting)|Verwendung der WebUSB-API steuern|
|[ImagesAllowedForUrls](#imagesallowedforurls)|Bilder auf diesen Websites zulassen|
|[ImagesBlockedForUrls](#imagesblockedforurls)|Bilder auf bestimmten Websites blockieren|
|[JavaScriptAllowedForUrls](#javascriptallowedforurls)|JavaScript auf bestimmten Websites zulassen|
|[JavaScriptBlockedForUrls](#javascriptblockedforurls)|JavaScript auf bestimmten Websites blockieren|
|[LegacySameSiteCookieBehaviorEnabled](#legacysamesitecookiebehaviorenabled)|Einstellung des standardmäßigen Cookieverhaltens für SameSite der Vorgängerversion aktivieren|
|[LegacySameSiteCookieBehaviorEnabledForDomainList](#legacysamesitecookiebehaviorenabledfordomainlist)|Zurücksetzen auf das Verhalten der Vorgängerversion für SameSite für Cookies auf bestimmten Websites|
|[NotificationsAllowedForUrls](#notificationsallowedforurls)|Benachrichtigungen auf bestimmten Websites zulassen|
|[NotificationsBlockedForUrls](#notificationsblockedforurls)|Benachrichtigungen auf bestimmten Websites blockieren|
|[PluginsAllowedForUrls](#pluginsallowedforurls)|Adobe Flash-Plug-In auf bestimmten Websites zulassen|
|[PluginsBlockedForUrls](#pluginsblockedforurls)|Adobe Flash-Plug-In auf bestimmten Websites blockieren|
|[PopupsAllowedForUrls](#popupsallowedforurls)|Popupfenster auf bestimmten Websites zulassen|
|[PopupsBlockedForUrls](#popupsblockedforurls)|Popupfenster auf bestimmten Websites blockieren|
|[RegisteredProtocolHandlers](#registeredprotocolhandlers)|Protokollhandler registrieren|
|[WebUsbAllowDevicesForUrls](#webusballowdevicesforurls)|Gewährt bestimmten Websites Zugriff, damit eine Verbindung mit bestimmten USB-Geräten hergestellt werden kann.|
|[WebUsbAskForUrls](#webusbaskforurls)|WebUSB auf bestimmten Websites zulassen|
|[WebUsbBlockedForUrls](#webusbblockedforurls)|WebUSB auf bestimmten Websites blockieren|
### [*Kennwort-Manager und -schutz*](#kennwort-manager-und--schutz-policies)
|Richtlinienname|Beschriftung|
|-|-|
|[PasswordManagerEnabled](#passwordmanagerenabled)|Speichern von Kennwörtern im Kennwort-Manager ermöglichen|
|[PasswordProtectionChangePasswordURL](#passwordprotectionchangepasswordurl)|URL zum Ändern des Kennworts konfigurieren|
|[PasswordProtectionLoginURLs](#passwordprotectionloginurls)|Liste der Unternehmens-Anmelde-URLs konfigurieren, bei denen der Kennwortschutzdienst den Fingerabdruck des Kennworts aufzeichnen soll|
|[PasswordProtectionWarningTrigger](#passwordprotectionwarningtrigger)|Warnungstrigger für Kennwortschutz konfigurieren|
### [*Natives Messaging*](#natives-messaging-policies)
|Richtlinienname|Beschriftung|
|-|-|
|[NativeMessagingAllowlist](#nativemessagingallowlist)|Steuern, welche nativen Messaginghosts von Benutzern verwendet werden können|
|[NativeMessagingBlocklist](#nativemessagingblocklist)|Native Nachrichtensperrliste konfigurieren|
|[NativeMessagingUserLevelHosts](#nativemessaginguserlevelhosts)|Native Messaginghosts auf Benutzerebene zulassen (ohne Administratorberechtigungen installiert)|
### [*Proxyserver*](#proxyserver-policies)
|Richtlinienname|Beschriftung|
|-|-|
|[ProxyBypassList](#proxybypasslist)|Proxy-Umgehungsregeln konfigurieren|
|[ProxyMode](#proxymode)|Proxyservereinstellungen konfigurieren|
|[ProxyPacUrl](#proxypacurl)|Proxy-PAC-Datei-URL festlegen|
|[ProxyServer](#proxyserver)|Adresse oder URL des Proxyservers konfigurieren|
|[ProxySettings](#proxysettings)|Proxyeinstellungen|
### [*SmartScreen-Einstellungen*](#smartscreen-einstellungen-policies)
|Richtlinienname|Beschriftung|
|-|-|
|[PreventSmartScreenPromptOverride](#preventsmartscreenpromptoverride)|Umgehung der Microsoft Defender SmartScreen-Aufforderungen für Websites verhindern|
|[PreventSmartScreenPromptOverrideForFiles](#preventsmartscreenpromptoverrideforfiles)|Umgehung der Microsoft Defender SmartScreen-Warnungen für Downloads verhindern|
|[SmartScreenAllowListDomains](#smartscreenallowlistdomains)|Konfigurieren Sie die Liste der Domänen, für die Microsoft Defender SmartScreen keine Warnungen auslöst.|
|[SmartScreenEnabled](#smartscreenenabled)|Microsoft Defender SmartScreen konfigurieren|
|[SmartScreenForTrustedDownloadsEnabled](#smartscreenfortrusteddownloadsenabled)|Überprüfung von Downloads von vertrauenswürdigen Quellen durch Microsoft Defender SmartScreen erzwingen|
|[SmartScreenPuaEnabled](#smartscreenpuaenabled)|Microsoft Defender SmartScreen konfigurieren, um potenziell unerwünschte Apps zu blockieren|
### [*Standardsuchanbieter*](#standardsuchanbieter-policies)
|Richtlinienname|Beschriftung|
|-|-|
|[DefaultSearchProviderEnabled](#defaultsearchproviderenabled)|Standardsuchanbieter aktivieren|
|[DefaultSearchProviderEncodings](#defaultsearchproviderencodings)|Standardsuchanbieter-Codierungen|
|[DefaultSearchProviderImageURL](#defaultsearchproviderimageurl)|Gibt das Bildsuchfeature für den standardmäßigen Suchanbieter an|
|[DefaultSearchProviderImageURLPostParams](#defaultsearchproviderimageurlpostparams)|Parameter für eine Bild-URL, die POST verwendet|
|[DefaultSearchProviderKeyword](#defaultsearchproviderkeyword)|Stichwort für Standardsuchanbieter|
|[DefaultSearchProviderName](#defaultsearchprovidername)|Standardsuchanbietername|
|[DefaultSearchProviderSearchURL](#defaultsearchprovidersearchurl)|Such-URL für den Standardsuchanbieter|
|[DefaultSearchProviderSuggestURL](#defaultsearchprovidersuggesturl)|Standard-Suchanbieter-URL für Vorschläge|
### [*Start&comma; Startseite und neue Tabseite*](#start-startseite-und-neue-tabseite-policies)
|Richtlinienname|Beschriftung|
|-|-|
|[HomepageIsNewTabPage](#homepageisnewtabpage)|Neue Tabseite als Startseite festlegen|
|[HomepageLocation](#homepagelocation)|Homepage-URL konfigurieren|
|[NewTabPageCompanyLogo](#newtabpagecompanylogo)|Neues Firmenlogo auf der Registerkartenseite festlegen|
|[NewTabPageHideDefaultTopSites](#newtabpagehidedefaulttopsites)|Die Standardwebsites der obersten Ebene auf der neuen Tabseite ausblenden|
|[NewTabPageLocation](#newtabpagelocation)|URL für die neue Tabseite konfigurieren|
|[NewTabPageManagedQuickLinks](#newtabpagemanagedquicklinks)|Schnelllinks für neue Tabs festlegen|
|[NewTabPageSetFeedType](#newtabpagesetfeedtype)|Funktion für neue Tabseiten in Microsoft Edge konfigurieren|
|[RestoreOnStartup](#restoreonstartup)|Aktion, die beim Start ausgeführt werden soll|
|[RestoreOnStartupURLs](#restoreonstartupurls)|Websites, die beim Start des Browsers geöffnet werden sollen|
|[ShowHomeButton](#showhomebutton)|Schaltfläche „Startseite“ auf Symbolleiste anzeigen|
### [*Additional*](#additional-policies)
|Richtlinienname|Beschriftung|
|-|-|
|[AdsSettingForIntrusiveAdsSites](#adssettingforintrusiveadssites)|Anzeigeneinstellung für Websites mit aufdringlichen Anzeigen|
|[AllowDeletingBrowserHistory](#allowdeletingbrowserhistory)|Löschen des Browser- und Downloadverlaufs ermöglichen|
|[AllowFileSelectionDialogs](#allowfileselectiondialogs)|Dateiauswahl-Dialogfelder zulassen|
|[AllowPopupsDuringPageUnload](#allowpopupsduringpageunload)|Erlaubt einer Seite, Popups während des Entladens zu zeigen|
|[AllowSyncXHRInPageDismissal](#allowsyncxhrinpagedismissal)|Zulassen, dass Seiten beim Schließen synchrone XHR-Anforderungen senden|
|[AllowTrackingForUrls](#allowtrackingforurls)|Konfigurieren von Ausnahmen für die Tracking-Verhinderung für bestimmte Sites|
|[AlwaysOpenPdfExternally](#alwaysopenpdfexternally)|PDF-Dateien immer extern öffnen|
|[ApplicationLocaleValue](#applicationlocalevalue)|Anwendungsgebietsschema festlegen|
|[AudioCaptureAllowed](#audiocaptureallowed)|Audioaufnahme zulassen oder blockieren|
|[AudioCaptureAllowedUrls](#audiocaptureallowedurls)|Websites, die auf Audioaufnahmegeräte zugreifen können, ohne eine Berechtigung anzufordern|
|[AutoImportAtFirstRun](#autoimportatfirstrun)|Daten und Einstellungen eines anderen Browsers bei der ersten Ausführung automatisch importieren|
|[AutofillAddressEnabled](#autofilladdressenabled)|AutoAusfüllen für Adressen aktivieren|
|[AutofillCreditCardEnabled](#autofillcreditcardenabled)|AutoAusfüllen für Kreditkarten aktivieren|
|[AutoplayAllowed](#autoplayallowed)|Automatische Medienwiedergabe für Websites zulassen|
|[BackgroundModeEnabled](#backgroundmodeenabled)|Ausführen von Hintergrund-Apps fortsetzen, nachdem Microsoft Edge geschlossen wurde|
|[BackgroundTemplateListUpdatesEnabled](#backgroundtemplatelistupdatesenabled)|Ermöglicht für Sammlungen und andere Features, die Vorlagen verwenden, Hintergrundaktualisierungen der Liste mit den verfügbaren Vorlagen.|
|[BlockThirdPartyCookies](#blockthirdpartycookies)|Cookies von Drittanbietern blockieren|
|[BrowserAddProfileEnabled](#browseraddprofileenabled)|Profilerstellung über das Flyout-Menü „Identität” oder die Seite „Einstellungen” aktivieren|
|[BrowserGuestModeEnabled](#browserguestmodeenabled)|Gastmodus aktivieren|
|[BrowserNetworkTimeQueriesEnabled](#browsernetworktimequeriesenabled)|Abfragen bei einem Browser-Netzwerk-Zeitdienst zulassen|
|[BrowserSignin](#browsersignin)|Browser-Anmeldeeinstellungen|
|[BuiltInDnsClientEnabled](#builtindnsclientenabled)|Integrierten DNS-Client verwenden|
|[CertificateTransparencyEnforcementDisabledForCas](#certificatetransparencyenforcementdisabledforcas)|Erzwingung der Zertifikattransparenz für eine Liste von subjectPublicKeyInfo-Hashes deaktivieren|
|[CertificateTransparencyEnforcementDisabledForLegacyCas](#certificatetransparencyenforcementdisabledforlegacycas)|Erzwingung der Zertifikattransparenz für eine Liste der Legacy-Zertifizierungsstellen deaktivieren|
|[CertificateTransparencyEnforcementDisabledForUrls](#certificatetransparencyenforcementdisabledforurls)|Erzwingung der Zertifikattransparenz für bestimmte URLs deaktivieren|
|[ClearBrowsingDataOnExit](#clearbrowsingdataonexit)|Browserdaten löschen, wenn Microsoft Edge geschlossen wird|
|[ClickOnceEnabled](#clickonceenabled)|Benutzern das Öffnen von Dateien unter Verwendung des ClickOnce-Protokolls ermöglichen|
|[CommandLineFlagSecurityWarningsEnabled](#commandlineflagsecuritywarningsenabled)|Aktivieren von Sicherheitswarnungen für Befehlszeilenflags|
|[ComponentUpdatesEnabled](#componentupdatesenabled)|Komponentenupdates in Microsoft Edge aktivieren|
|[ConfigureDoNotTrack](#configuredonottrack)|Nicht verfolgen (Do not track) konfigurieren|
|[ConfigureOnlineTextToSpeech](#configureonlinetexttospeech)|Online-Text-zu-Sprache konfigurieren|
|[CustomHelpLink](#customhelplink)|Benutzerdefinierten Hilfelink angeben|
|[DefaultBrowserSettingEnabled](#defaultbrowsersettingenabled)|Microsoft Edge als Standardbrowser festlegen|
|[DeveloperToolsAvailability](#developertoolsavailability)|Steuern, wo Entwicklungstools verwendet werden können|
|[DirectInvokeEnabled](#directinvokeenabled)|Benutzern das Öffnen von Dateien unter Verwendung des DirectInvoke-Protokolls ermöglichen|
|[Disable3DAPIs](#disable3dapis)|Unterstützung für 3D-Grafik-APIs deaktivieren|
|[DisableScreenshots](#disablescreenshots)|Aufnahme von Screenshots deaktivieren|
|[DiskCacheDir](#diskcachedir)|Verzeichnis für Datenträgercache festlegen|
|[DiskCacheSize](#diskcachesize)|Größe des Datenträgercaches festlegen (in Bytes)|
|[DownloadDirectory](#downloaddirectory)|Downloadverzeichnis festlegen|
|[DownloadRestrictions](#downloadrestrictions)|Download-Einschränkungen zulassen|
|[EdgeCollectionsEnabled](#edgecollectionsenabled)|Aktivieren der Sammlungsfunktion|
|[EditFavoritesEnabled](#editfavoritesenabled)|Ermöglicht Benutzern das Bearbeiten von Favoriten.|
|[EnableDeprecatedWebPlatformFeatures](#enabledeprecatedwebplatformfeatures)|Veraltete Webplattformfeatures vorübergehend wieder aktivieren|
|[EnableDomainActionsDownload](#enabledomainactionsdownload)|Herunterladen von Domänenaktionen von Microsoft aktivieren|
|[EnableOnlineRevocationChecks](#enableonlinerevocationchecks)|Onlineprüfungen für OCSP/Sperrlisten aktivieren|
|[EnterpriseHardwarePlatformAPIEnabled](#enterprisehardwareplatformapienabled)|Ermöglichen der Verwendung der Enterprise Hardware Platform-API durch verwaltete Erweiterungen|
|[ExperimentationAndConfigurationServiceControl](#experimentationandconfigurationservicecontrol)|Steuern der Kommunikation mit dem Experimentier- und Konfigurationsdienst|
|[ExternalProtocolDialogShowAlwaysOpenCheckbox](#externalprotocoldialogshowalwaysopencheckbox)|Steuert, ob im Dialogfeld für externe Protokolle das Kontrollkästchen „Immer öffnen“ angezeigt wird.|
|[FavoritesBarEnabled](#favoritesbarenabled)|Favoritenleiste aktivieren|
|[ForceBingSafeSearch](#forcebingsafesearch)|Bing SafeSearch erzwingen|
|[ForceEphemeralProfiles](#forceephemeralprofiles)|Verwendung von kurzlebigen Profilen aktivieren|
|[ForceGoogleSafeSearch](#forcegooglesafesearch)|Google SafeSearch erzwingen|
|[ForceNetworkInProcess](#forcenetworkinprocess)|Ausführung von Netzwerkcode im Browserprozess erzwingen|
|[ForceYouTubeRestrict](#forceyoutuberestrict)|Minimalen eingeschränkten Modus für YouTube erzwingen|
|[FullscreenAllowed](#fullscreenallowed)|Vollbildmodus zulassen|
|[GoToIntranetSiteForSingleWordEntryInAddressBar](#gotointranetsiteforsinglewordentryinaddressbar)|Direkte Intranetsitenavigation erzwingen anstatt in der Adressleiste nach einzelnen Worteinträgen zu suchen|
|[HSTSPolicyBypassList](#hstspolicybypasslist)|Konfigurieren der Liste mit Namen, die die HSTS-Richtlinienprüfung umgehen|
|[HardwareAccelerationModeEnabled](#hardwareaccelerationmodeenabled)|Hardwarebeschleunigung verwenden (sofern verfügbar)|
|[ImportAutofillFormData](#importautofillformdata)|Importieren von AutoAusfüllen-Formulardaten zulassen|
|[ImportBrowserSettings](#importbrowsersettings)|Importieren von Browsereinstellungen zulassen|
|[ImportFavorites](#importfavorites)|Importieren von Favoriten zulassen|
|[ImportHistory](#importhistory)|Importieren des Browserverlaufs zulassen|
|[ImportHomepage](#importhomepage)|Importieren von Startseiteneinstellungen zulassen|
|[ImportOpenTabs](#importopentabs)|Importieren offener Tabs zulassen|
|[ImportPaymentInfo](#importpaymentinfo)|Import von Zahlungsinformationen zulassen|
|[ImportSavedPasswords](#importsavedpasswords)|Importieren gespeicherter Kennwörter zulassen|
|[ImportSearchEngine](#importsearchengine)|Importieren von Suchmaschineneinstellungen zulassen|
|[InPrivateModeAvailability](#inprivatemodeavailability)|Verfügbarkeit des InPrivate-Modus konfigurieren|
|[InternetExplorerIntegrationLevel](#internetexplorerintegrationlevel)|Internet Explorer-Integration konfigurieren|
|[InternetExplorerIntegrationSiteList](#internetexplorerintegrationsitelist)|Enterprise Mode Site List konfigurieren|
|[InternetExplorerIntegrationSiteRedirect](#internetexplorerintegrationsiteredirect)|Angeben des Verhaltens von seiteninternen Navigationsvorgängen zu nicht konfigurierten Websites, wenn diese über Seiten im Internet Explorer-Modus gestartet werden|
|[IsolateOrigins](#isolateorigins)|Websiteisolation für bestimmte Ursprünge aktivieren|
|[ManagedFavorites](#managedfavorites)|Favoriten konfigurieren|
|[ManagedSearchEngines](#managedsearchengines)|Suchmaschinen verwalten|
|[MaxConnectionsPerProxy](#maxconnectionsperproxy)|Maximale Anzahl gleichzeitiger Verbindungen mit dem Proxyserver|
|[MediaRouterCastAllowAllIPs](#mediaroutercastallowallips)|Google Cast erlauben, eine Verbindung mit CAST-Geräten auf allen IP-Adressen herzustellen|
|[MetricsReportingEnabled](#metricsreportingenabled)|Meldung von nutzungs- und absturzbezogenen Daten aktivieren|
|[NetworkPredictionOptions](#networkpredictionoptions)|Netzwerkvorhersage aktivieren|
|[NonRemovableProfileEnabled](#nonremovableprofileenabled)|Konfigurieren, ob für einen Benutzer beim Anmelden mit dem Geschäfts-, Schul-oder Unikonto immer automatisch ein Standardprofil vorhanden ist.|
|[OverrideSecurityRestrictionsOnInsecureOrigin](#overridesecurityrestrictionsoninsecureorigin)|Steuert, wo Sicherheitseinschränkungen für unsichere Ursprünge gelten|
|[PinningWizardAllowed](#pinningwizardallowed)|Allow Pin to taskbar wizard|
|[ProactiveAuthEnabled](#proactiveauthenabled)|Proaktive Authentifizierung aktivieren|
|[PromotionalTabsEnabled](#promotionaltabsenabled)|Tabfüllende Werbeinhalte ermöglichen|
|[PromptForDownloadLocation](#promptfordownloadlocation)|Fragen, wo heruntergeladene Dateien gespeichert werden sollen|
|[QuicAllowed](#quicallowed)|QUIC-Protokoll zulassen|
|[RelaunchNotification](#relaunchnotification)|Einen Benutzer benachrichtigen, dass ein Neustart des Browsers für ausstehende Updates empfohlen wird oder erforderlich ist|
|[RelaunchNotificationPeriod](#relaunchnotificationperiod)|Zeitraum für Aktualisierungsbenachrichtigungen festlegen|
|[RendererCodeIntegrityEnabled](#renderercodeintegrityenabled)|Renderercodeintegrität aktivieren|
|[RequireOnlineRevocationChecksForLocalAnchors](#requireonlinerevocationchecksforlocalanchors)|Geben Sie an, ob für lokale Vertrauensanker Online-OCSP/CRL-Überprüfungen erforderlich sind.|
|[ResolveNavigationErrorsUseWebService](#resolvenavigationerrorsusewebservice)|Auflösung von Navigationsfehlern mithilfe eines Webdienstes aktivieren|
|[RestrictSigninToPattern](#restrictsignintopattern)|Beschränken der Konten, die als primäre Microsoft Edge-Konten verwendet werden können|
|[RunAllFlashInAllowMode](#runallflashinallowmode)|Adobe Flash-Inhaltseinstellung auf alle Inhalte erweitern|
|[SSLErrorOverrideAllowed](#sslerroroverrideallowed)|Zulassen, dass Benutzer von der HTTPS-Warnungsseite aus fortfahren können|
|[SSLVersionMin](#sslversionmin)|Mindestversion von TLS aktiviert|
|[SavingBrowserHistoryDisabled](#savingbrowserhistorydisabled)|Speichern des Browserverlaufs deaktivieren|
|[SearchSuggestEnabled](#searchsuggestenabled)|Suchvorschläge aktivieren|
|[SecurityKeyPermitAttestation](#securitykeypermitattestation)|Websites oder Domänen, die keine Berechtigung zur Verwendung des direkten Sicherheitsschlüssel-Nachweises benötigen|
|[SendIntranetToInternetExplorer](#sendintranettointernetexplorer)|Alle Intranetsites an Internet Explorer senden|
|[SendSiteInfoToImproveServices](#sendsiteinfotoimproveservices)|Websiteinformationen zur Verbesserung von Microsoft-Diensten senden|
|[ShowOfficeShortcutInFavoritesBar](#showofficeshortcutinfavoritesbar)|Microsoft Office-Verknüpfung in der Favoritenleiste anzeigen|
|[SignedHTTPExchangeEnabled](#signedhttpexchangeenabled)|Unterstützung des signierten HTTP-Austauschs (SXG) aktivieren|
|[SitePerProcess](#siteperprocess)|Websiteisolation für jede Website aktivieren|
|[SpellcheckEnabled](#spellcheckenabled)|Rechtschreibprüfung aktivieren|
|[SpellcheckLanguage](#spellchecklanguage)|Spezifische Sprachen für die Rechtschreibprüfung aktivieren|
|[SpellcheckLanguageBlocklist](#spellchecklanguageblocklist)|Deaktivierung von Sprachen für die Rechtschreibprüfung erzwingen|
|[SuppressUnsupportedOSWarning](#suppressunsupportedoswarning)|Nicht unterstützte Betriebssystemwarnung unterdrücken|
|[SyncDisabled](#syncdisabled)|Synchronisierung von Daten mit Microsoft-Synchronisierungsdiensten deaktivieren|
|[TabFreezingEnabled](#tabfreezingenabled)|Einfrieren von Hintergrundtabs zulassen|
|[TaskManagerEndProcessEnabled](#taskmanagerendprocessenabled)|Beenden von Prozessen im Browser-Task-Manager ermöglichen|
|[TrackingPrevention](#trackingprevention)|Blockieren der Nachverfolgung der Webbrowsing-Aktivitäten von Benutzern|
|[TranslateEnabled](#translateenabled)|Übersetzung aktivieren|
|[URLAllowlist](#urlallowlist)|Liste zulässiger URLs definieren|
|[URLBlocklist](#urlblocklist)|Zugriff auf eine Liste von URLs blockieren|
|[UserDataDir](#userdatadir)|Benutzerdatenverzeichnis festlegen|
|[UserFeedbackAllowed](#userfeedbackallowed)|Benutzerfeedback zulassen|
|[VideoCaptureAllowed](#videocaptureallowed)|Videoaufnahme zulassen oder blockieren|
|[VideoCaptureAllowedUrls](#videocaptureallowedurls)|Websites, die auf Videoaufnahmegeräte zugreifen können, ohne eine Berechtigung anzufordern|
|[WPADQuickCheckEnabled](#wpadquickcheckenabled)|WPAD-Optimierung festlegen|
|[WebDriverOverridesIncompatiblePolicies](#webdriveroverridesincompatiblepolicies)|Zulassen, dass WebDriver inkompatible Richtlinien außer Kraft setzt|
|[WebRtcLocalhostIpHandling](#webrtclocalhostiphandling)|Verfügbarmachung der Localhost-IP-Adresse durch WebRTC beschränken|
|[WebRtcUdpPortRange](#webrtcudpportrange)|Bereich der lokalen, von WebRTC verwendeten UDP-Ports einschränken|




  ## Cast policies

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### EnableMediaRouter
  #### Google Cast aktivieren
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Aktivieren Sie diese Richtlinie, um Google Cast zu aktivieren. Benutzer können es dann über das App-Menü, über Seitenkontextmenüs, Mediensteuerungen auf Cast-fähigen Websites und (falls angezeigt) über das Cast-Symbolleistensymbol starten.

Deaktivieren Sie diese Richtlinie, um Google Cast zu deaktivieren.

Google Cast ist standardmäßig aktiviert.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Nein - Erfordert einen Neustart des Browsers

  #### Datentyp:
  Boolesch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: EnableMediaRouter
  - Gruppenrichtlinienname: Google Cast aktivieren
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/Cast
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: EnableMediaRouter
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000001
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: EnableMediaRouter
  - Beispielwert:
``` xml
<true/>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### ShowCastIconInToolbar
  #### Wiedergabesymbol in der Symbolleiste anzeigen
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Legen Sie diese Richtlinie auf true fest, um das Symbol der Cast-Symbolleiste in der Symbolleiste oder im Überlaufmenü anzuzeigen. Benutzer können es nicht entfernen.

Wenn Sie diese Richtlinie nicht konfigurieren oder deaktivieren, können Benutzer das Symbol über das Kontextmenü anheften oder entfernen.

Diese Richtlinie wird ignoriert und das Symbol wird in der Symbolleiste nicht angezeigt, wenn Sie auch die Richtlinie [EnableMediaRouter](#enablemediarouter) auf false festgelegt haben.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Nein - Erfordert einen Neustart des Browsers

  #### Datentyp:
  Boolesch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: ShowCastIconInToolbar
  - Gruppenrichtlinienname: Wiedergabesymbol in der Symbolleiste anzeigen
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/Cast
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: ShowCastIconInToolbar
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000000
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: ShowCastIconInToolbar
  - Beispielwert:
``` xml
<false/>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ## Drucken policies

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### DefaultPrinterSelection
  #### Standardmäßige Druckerauswahl-Regeln
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Überschreibt die Regeln für die Wahl des Standarddruckers von Microsoft Edge. Diese Richtlinie bestimmt die Regeln für die Wahl des Standarddruckers in Microsoft Edge, wenn ein Benutzer erstmals eine Seite drucken möchte.

Wenn diese Richtlinie festgelegt ist, versucht Microsoft Edge, einen Drucker zu finden, der über alle angegebenen Attribute verfügt, und verwendet diesen als Standarddrucker. Sollten die Kriterien von mehreren Druckern erfüllt werden, wird der erste passende Drucker verwendet.

Wenn Sie diese Richtlinie nicht konfigurieren oder bis zum Timeout keine passenden Drucker gefunden werden, wird als Standarddrucker entweder der integrierte PDF-Drucker (sofern vorhanden) oder kein Drucker verwendet.

Der Wert wird als JSON-Objekt nach dem folgenden Schema analysiert: { "type": "object", "properties": { "idPattern": { "description": "Regular expression to match printer id.", "type": "string" }, "namePattern": { "description": "Regular expression to match printer display name.", "type": "string" } } }

Wird ein Feld ausgelassen, bedeutet das, dass alle Werte geeignet sind. Wenn Sie also beispielsweise keine Konnektivität angeben, sucht die Druckvorschau nach allen Arten von lokalen Druckern. Muster für reguläre Ausdrücke müssen der JavaScript-RegExp-Syntax entsprechen, und beim Abgleich wird die Groß-/Kleinschreibung berücksichtigt.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Zeichenfolge

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: DefaultPrinterSelection
  - Gruppenrichtlinienname: Standardmäßige Druckerauswahl-Regeln
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/Drucken
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: DefaultPrinterSelection
  - Werttyp: REG_SZ
  ##### Beispielwert:
```
"{ "idPattern": ".*public", "namePattern": ".*Color" }"
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: DefaultPrinterSelection
  - Beispielwert:
``` xml
<string>{ "idPattern": ".*public", "namePattern": ".*Color" }</string>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### PrintHeaderFooter
  #### Kopf- und Fußzeilen drucken
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Erzwingt die Aktivierung oder Deaktivierung von Kopf- und Fußzeilen im Druckdialogfeld.

Wenn Sie diese Richtlinie nicht konfigurieren, kann der Benutzer entscheiden, ob Kopf- und Fußzeilen gedruckt werden sollen.

Wenn Sie diese Richtlinie deaktivieren, können Benutzer keine Kopf- und Fußzeilen drucken.

Wenn Sie diese Richtlinie aktivieren, werden Kopf- und Fußzeilen immer gedruckt.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Ja
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Boolesch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: PrintHeaderFooter
  - Gruppenrichtlinienname: Kopf- und Fußzeilen drucken
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/Drucken
  - Gruppenrichtlinienpfad (Empfohlen): Administrative Vorlagen/Microsoft Edge - Standardeinstellungen (können durch Benutzer überschrieben werden)/Drucken
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): SOFTWARE\Policies\Microsoft\Edge\Empfohlen
  - Wertname: PrintHeaderFooter
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000000
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: PrintHeaderFooter
  - Beispielwert:
``` xml
<false/>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### PrintPreviewUseSystemDefaultPrinter
  #### Den Systemstandarddrucker als Standarddrucker festlegen
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Weist Microsoft Edge an, den Standarddrucker des Systems anstelle des zuletzt verwendeten Druckers als Standardoption in der Seitenansicht zu verwenden.

Wenn Sie diese Richtlinie deaktivieren oder nicht konfigurieren, wird in der Seitenansicht der zuletzt verwendete Drucker als Standardziel ausgewählt.

Wenn Sie diese Richtlinie aktivieren, verwendet die Seitenansicht den Standarddrucker des Betriebssystems als Standardziel.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Ja
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Boolesch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: PrintPreviewUseSystemDefaultPrinter
  - Gruppenrichtlinienname: Den Systemstandarddrucker als Standarddrucker festlegen
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/Drucken
  - Gruppenrichtlinienpfad (Empfohlen): Administrative Vorlagen/Microsoft Edge - Standardeinstellungen (können durch Benutzer überschrieben werden)/Drucken
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): SOFTWARE\Policies\Microsoft\Edge\Empfohlen
  - Wertname: PrintPreviewUseSystemDefaultPrinter
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000000
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: PrintPreviewUseSystemDefaultPrinter
  - Beispielwert:
``` xml
<false/>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### PrintingEnabled
  #### Drucken ermöglichen
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Ermöglicht das Drucken in Microsoft Edge und verhindert, dass Benutzer diese Einstellung ändern.

Wenn Sie diese Richtlinie aktivieren oder nicht konfigurieren, können Benutzer drucken.

Wenn Sie diese Richtlinie deaktivieren, können Benutzer in Microsoft Edge nicht drucken. Das Drucken wird unter anderem im Schraubenschlüsselmenü, in Erweiterungen und in JavaScript-Anwendungen deaktiviert. Benutzer können weiterhin über Plug-Ins drucken, die Microsoft Edge beim Drucken umgehen. So verfügen beispielsweise bestimmte Adobe Flash-Anwendungen über eine Druckoption in ihrem Kontextmenü, was von dieser Richtlinie nicht abgedeckt wird.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Boolesch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: PrintingEnabled
  - Gruppenrichtlinienname: Drucken ermöglichen
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/Drucken
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: PrintingEnabled
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000001
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: PrintingEnabled
  - Beispielwert:
``` xml
<true/>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### UseSystemPrintDialog
  #### Über Systemdruckdialogfeld drucken
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Zeigt das Systemdruckdialogfeld anstelle der Druckvorschau an.

Wenn Sie diese Richtlinie aktivieren, öffnet Microsoft Edge das Systemdruckdialogfeld anstelle der integrierten Druckvorschau, wenn ein Benutzer eine Seite druckt.

Falls Sie diese Richtlinie nicht konfigurieren oder deaktivieren, lösen Druckbefehle den Druckvorschaubildschirm von Microsoft Edge aus.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Nein - Erfordert einen Neustart des Browsers

  #### Datentyp:
  Boolesch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: UseSystemPrintDialog
  - Gruppenrichtlinienname: Über Systemdruckdialogfeld drucken
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/Drucken
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: UseSystemPrintDialog
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000000
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: UseSystemPrintDialog
  - Beispielwert:
``` xml
<false/>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ## Erweiterungen policies

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### ExtensionAllowedTypes
  #### Zulässige Erweiterungstypen konfigurieren
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Steuert, welche Erweiterungstypen installiert werden können, und begrenzt den Laufzeitzugriff.

Diese Einstellung definiert die zulässigen Arten von Erweiterungen und mit welchen Hosts sie interagieren können. Der Wert ist eine Liste dieser Zeichenfolgen: "extension", "theme", "user_script", and "hosted_app". Weitere Informationen zu diesen Typen finden Sie in der Dokumentation zu Microsoft Edge-Erweiterungen.

Beachten Sie, dass diese Richtlinie auch Erweiterungen betrifft, die mit [ExtensionInstallForcelist](#extensioninstallforcelist) zwangsinstalliert werden sollen.

Wenn Sie diese Richtlinie aktivieren, werden nur Erweiterungen installiert, die einem Typ in der Liste entsprechen.

Wenn Sie diese Richtlinie nicht konfigurieren, werden keine Einschränkungen für die zulässigen Erweiterungstypen erzwungen.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Liste der Zeichenfolgen

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: ExtensionAllowedTypes
  - Gruppenrichtlinienname: Zulässige Erweiterungstypen konfigurieren
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/Erweiterungen
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge\ExtensionAllowedTypes
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: 1, 2, 3, ...
  - Werttyp: Liste von REG_SZ
  ##### Beispielwert:
```
SOFTWARE\Policies\Microsoft\Edge\ExtensionAllowedTypes\0 = "hosted_app"

```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: ExtensionAllowedTypes
  - Beispielwert:
``` xml
<array>
  <string>hosted_app</string>
</array>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### ExtensionInstallAllowlist
  #### Installation bestimmter Erweiterungen zulassen
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Standardmäßig sind alle Erweiterungen zugelassen. Wenn Sie jedoch alle Erweiterungen blockieren, indem Sie die Richtlinie "ExtensionInstallBlockList" auf "*" festlegen, können Benutzer nur Erweiterungen installieren, die in dieser Richtlinie definiert sind.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Liste der Zeichenfolgen

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: ExtensionInstallAllowlist
  - Gruppenrichtlinienname: Installation bestimmter Erweiterungen zulassen
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/Erweiterungen
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallAllowlist
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: 1, 2, 3, ...
  - Werttyp: Liste von REG_SZ
  ##### Beispielwert:
```
SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallAllowlist\0 = "extension_id1"
SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallAllowlist\1 = "extension_id2"

```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: ExtensionInstallAllowlist
  - Beispielwert:
``` xml
<array>
  <string>extension_id1</string>
  <string>extension_id2</string>
</array>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### ExtensionInstallBlocklist
  #### Steuern, welche Erweiterungen nicht installiert werden können
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Listet bestimmte Erweiterungen auf, die Benutzer NICHT in Microsoft Edge installieren können. Wenn Sie diese Richtlinie bereitstellen, werden sämtliche zuvor installierten Erweiterungen aus dieser Liste deaktiviert und können vom Benutzer nicht mehr aktiviert werden. Wenn Sie ein Element aus der Liste blockierter Erweiterungen entfernen, wird die entsprechende Erweiterung automatisch überall reaktiviert, wo sie zuvor installiert war.

Mit „*“ können Sie alle Erweiterungen blockieren, die nicht explizit in der Liste „Zulassen“ angegeben sind.

Wenn Sie diese Richtlinie nicht konfigurieren, können Benutzer beliebige Erweiterungen in Microsoft Edge installieren.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Liste der Zeichenfolgen

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: ExtensionInstallBlocklist
  - Gruppenrichtlinienname: Steuern, welche Erweiterungen nicht installiert werden können
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/Erweiterungen
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallBlocklist
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: 1, 2, 3, ...
  - Werttyp: Liste von REG_SZ
  ##### Beispielwert:
```
SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallBlocklist\0 = "extension_id1"
SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallBlocklist\1 = "extension_id2"

```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: ExtensionInstallBlocklist
  - Beispielwert:
``` xml
<array>
  <string>extension_id1</string>
  <string>extension_id2</string>
</array>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### ExtensionInstallForcelist
  #### Steuern, welche Erweiterungen automatisch installiert werden
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Gibt Erweiterungen an, die ohne Benutzerinteraktion installiert werden und die von Benutzer nicht deinstalliert oder deaktiviert werden können (zwangsinstallierte Erweiterungen). Alle von den Erweiterungen angeforderten Berechtigungen werden implizit und ohne Benutzerinteraktion erteilt, einschließlich aller zusätzlichen Berechtigungen, die von zukünftigen Versionen der Erweiterung angefordert werden. Zudem werden Berechtigungen für die Erweiterungs-APIs enterprise.deviceAttributes und enterprise.platformKeys erteilt. (Diese beiden APIs sind nur für Erweiterungen verfügbar, die zwangsinstalliert sind.)

Diese Richtlinie hat Vorrang vor einer möglicherweise widersprüchlichen [ExtensionInstallBlocklist](#extensioninstallblocklist)-Richtlinie. Wenn Sie eine Erweiterung aus der Liste der Zwangsinstallationen entfernen, wird sie automatisch von Microsoft Edge deinstalliert.

Für Windows-Geräte, die nicht mit einer Microsoft Active Directory-Domäne verbunden sind, ist die erzwungene Installation auf im Microsoft Store verfügbare Erweiterungen beschränkt.

Beachten Sie, dass Benutzer den Quellcode jeder Erweiterung mit Hilfe der Developer Tools ändern können, wodurch die Erweiterung möglicherweise nicht funktionsfähig ist. Wenn dies ein Problem ist, legen Sie die Richtlinie [DeveloperToolsAvailability](#developertoolsavailability) fest.

Verwenden Sie das folgende Format, um der Liste eine Erweiterung hinzuzufügen:

[extensionID];[updateURL]

- extensionID ist die aus 32 Buchstaben bestehende Zeichenfolge, die im Entwicklermodus unter edge://extensions steht.

- updateURL (optional) ist die Adresse des XML-Dokuments Update Manifest für die App oder Erweiterung, wie unter [https://go.microsoft.com/fwlink/?linkid=2095043](https://go.microsoft.com/fwlink/?linkid=2095043) beschrieben. Wenn Sie die updateURL nicht festlegen, wird die Microsoft Store Update-URL verwendet (derzeit https://edge.microsoft.com/extensionwebstorebase/v1/crx). Beachten Sie, dass die in dieser Richtlinie festgelegte Update-URL nur für die Erstinstallation verwendet wird. Nachfolgende Updates der Erweiterung verwenden die im Manifest der Erweiterung angegebene Update-URL.

Beispielsweise installiert gggmmkjegpiggikcnhidnjjhmicpibll;https://edge.microsoft.com/extensionwebstorebase/v1/crx die Microsoft Online App über die Microsoft Store-"Update"-URL. Weitere Informationen über Hosting-Erweiterungen finden Sie unter: [https://go.microsoft.com/fwlink/?linkid=2095044](https://go.microsoft.com/fwlink/?linkid=2095044).

Wenn Sie diese Richtlinie nicht konfigurieren, werden keine Erweiterungen automatisch installiert, und Benutzer können jede Erweiterung in Microsoft Edge deinstallieren.

Beachten Sie, dass diese Richtlinie nicht für den InPrivate-Modus gilt.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Liste der Zeichenfolgen

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: ExtensionInstallForcelist
  - Gruppenrichtlinienname: Steuern, welche Erweiterungen automatisch installiert werden
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/Erweiterungen
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallForcelist
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: 1, 2, 3, ...
  - Werttyp: Liste von REG_SZ
  ##### Beispielwert:
```
SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallForcelist\0 = "gbchcmhmhahfdphkhkmpfmihenigjmpp;https://edge.microsoft.com/extensionwebstorebase/v1/crx"
SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallForcelist\1 = "abcdefghijklmnopabcdefghijklmnop"

```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: ExtensionInstallForcelist
  - Beispielwert:
``` xml
<array>
  <string>gbchcmhmhahfdphkhkmpfmihenigjmpp;https://edge.microsoft.com/extensionwebstorebase/v1/crx</string>
  <string>abcdefghijklmnopabcdefghijklmnop</string>
</array>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### ExtensionInstallSources
  #### Erweiterung und Benutzer-Skriptinstallationsquellen konfigurieren
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Definiert URLs, die Erweiterungen und Themen installieren können.

Standardmäßig müssen Benutzer für jede Erweiterung oder jedes Skript, das sie installieren möchten, eine *.crx-Datei herunterladen und diese dann auf die Microsoft Edge-Einstellungsseite ziehen. Diese Richtlinie ermöglicht es bestimmten URLs, die Erweiterung oder das Skript für den Benutzer zu installieren.

Jedes Element in dieser Liste ist ein erweiterungsartiges Zuordnungsmuster (siehe [https://go.microsoft.com/fwlink/?linkid=2095039](https://go.microsoft.com/fwlink/?linkid=2095039)). Benutzer können Elemente einfach von jeder URL installieren, die mit einem Element in dieser Liste übereinstimmt. Sowohl der Speicherort der *.crx-Datei als auch die Seite, von der aus der Download gestartet wird (d.h. der Referrer), müssen durch diese Muster erlaubt sein.

Die Richtlinie [ExtensionInstallBlocklist](#extensioninstallblocklist) hat Vorrang vor dieser Richtlinie. Alle Erweiterungen, die sich auf der Blockliste befinden, werden nicht installiert, auch wenn sie von einer Website auf dieser Liste stammen.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Liste der Zeichenfolgen

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: ExtensionInstallSources
  - Gruppenrichtlinienname: Erweiterung und Benutzer-Skriptinstallationsquellen konfigurieren
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/Erweiterungen
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallSources
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: 1, 2, 3, ...
  - Werttyp: Liste von REG_SZ
  ##### Beispielwert:
```
SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallSources\0 = "https://corp.contoso.com/*"

```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: ExtensionInstallSources
  - Beispielwert:
``` xml
<array>
  <string>https://corp.contoso.com/*</string>
</array>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### ExtensionSettings
  #### Einstellungen für Erweiterungsverwaltung konfigurieren
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Konfiguriert die Einstellungen für die Erweiterungsverwaltung für Microsoft Edge.

Diese Richtlinie steuert mehrere Einstellungen, einschließlich Einstellungen, die durch vorhandene erweiterungsbezogene Richtlinien gesteuert werden. Diese Richtlinie setzt alle Vorgänger-Richtlinien außer Kraft, wenn beide Einstellungen festgelegt sind.

Mit dieser Richtlinie wird der Konfiguration eine Erweiterungs-ID oder eine Update-URL zugeordnet. Mit einer Erweiterungs-ID wird die Konfiguration nur auf die angegebene Erweiterung angewendet. Legen Sie eine Standardkonfiguration für die spezielle ID "*" fest, die auf alle Erweiterungen angewendet werden soll, die nicht speziell in dieser Richtlinie aufgeführt sind. Mit einer Update-URL wird die Konfiguration auf alle Erweiterungen mit der genauen Update-URL angewendet, die im Manifest dieser Erweiterung angegeben ist, wie unter [https://go.microsoft.com/fwlink/?linkid=2095043](https://go.microsoft.com/fwlink/?linkid=2095043) beschrieben.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Wörterbuch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: ExtensionSettings
  - Gruppenrichtlinienname: Einstellungen für Erweiterungsverwaltung konfigurieren
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/Erweiterungen
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: ExtensionSettings
  - Werttyp: REG_SZ
  ##### Beispielwert:
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


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: ExtensionSettings
  - Beispielwert:
``` xml
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
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ## HTTP-Authentifizierung policies

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### AllowCrossOriginAuthPrompt
  #### Übergreifende HTTP-Basic-Authentifizierungsaufforderungen zulassen
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Steuert, ob untergeordnete Inhalte von Drittanbietern auf einer Seite ein Dialogfeld für die HTTP-Standardauthentifizierung öffnen können.

Dies ist normalerweise im Sinne der Phishing-Abwehr deaktiviert. Wenn Sie diese Richtlinie nicht konfigurieren, ist sie deaktiviert, und untergeordnete Inhalte von Drittanbietern können kein Dialogfeld für die HTTP-Standardauthentifizierung öffnen.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Boolesch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: AllowCrossOriginAuthPrompt
  - Gruppenrichtlinienname: Übergreifende HTTP-Basic-Authentifizierungsaufforderungen zulassen
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/HTTP-Authentifizierung
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: AllowCrossOriginAuthPrompt
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000000
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: AllowCrossOriginAuthPrompt
  - Beispielwert:
``` xml
<false/>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### AuthNegotiateDelegateAllowlist
  #### Gibt eine Liste der Server an, an die Microsoft Edge Anmeldeinformationen von Benutzern delegieren kann
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Konfigurieren Sie die Liste der Server, an die Microsoft Edge delegieren kann.

Trennen Sie mehrere Servernamen durch Kommas. Platzhalter (*) sind zulässig.

Wenn Sie diese Richtlinie nicht konfigurieren, wird Microsoft Edge keine Benutzeranmeldeinformationen delegieren, auch wenn ein Server als Intranet erkannt wird.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Nein - Erfordert einen Neustart des Browsers

  #### Datentyp:
  Zeichenfolge

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: AuthNegotiateDelegateAllowlist
  - Gruppenrichtlinienname: Gibt eine Liste der Server an, an die Microsoft Edge Anmeldeinformationen von Benutzern delegieren kann
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/HTTP-Authentifizierung
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: AuthNegotiateDelegateAllowlist
  - Werttyp: REG_SZ
  ##### Beispielwert:
```
"contoso.com"
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: AuthNegotiateDelegateAllowlist
  - Beispielwert:
``` xml
<string>contoso.com</string>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### AuthSchemes
  #### Unterstützte Authentifizierungsschemas
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Gibt an, welche HTTP-Authentifizierungsschemas unterstützt werden.

Sie können die Richtlinie mit folgenden Werten konfigurieren: „Basic“, „Digest“, „NTLM“ und „Negotiate“. Trennen Sie mehrere Werte durch Kommas.

Wenn Sie diese Richtlinie nicht konfigurieren, werden alle vier Schemas verwendet.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Nein - Erfordert einen Neustart des Browsers

  #### Datentyp:
  Zeichenfolge

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: AuthSchemes
  - Gruppenrichtlinienname: Unterstützte Authentifizierungsschemas
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/HTTP-Authentifizierung
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: AuthSchemes
  - Werttyp: REG_SZ
  ##### Beispielwert:
```
"basic,digest,ntlm,negotiate"
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: AuthSchemes
  - Beispielwert:
``` xml
<string>basic,digest,ntlm,negotiate</string>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### AuthServerAllowlist
  #### Liste der zugelassenen Authentifizierungsserver konfigurieren
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Legt fest, welche Server für die integrierte Authentifizierung aktiviert werden sollen. Die integrierte Authentifizierung ist nur aktiviert, wenn Microsoft Edge eine Anfrage zur Authentifizierung von einem Proxy oder einem Server in dieser Liste erhält.

Trennen Sie mehrere Servernamen durch Kommas. Platzhalter (*) sind zulässig.

Falls Sie diese Richtlinie nicht konfigurieren, versucht Microsoft Edge zu erkennen, ob sich ein Server im Intranet befindet, nur dann reagiert er auf IWA-Anfragen. Falls sich der Server im Internet befindet, werden IWA-Anfragen von ihm durch Microsoft Edge ignoriert.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Nein - Erfordert einen Neustart des Browsers

  #### Datentyp:
  Zeichenfolge

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: AuthServerAllowlist
  - Gruppenrichtlinienname: Liste der zugelassenen Authentifizierungsserver konfigurieren
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/HTTP-Authentifizierung
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: AuthServerAllowlist
  - Werttyp: REG_SZ
  ##### Beispielwert:
```
"*contoso.com,contoso.com"
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: AuthServerAllowlist
  - Beispielwert:
``` xml
<string>*contoso.com,contoso.com</string>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### DisableAuthNegotiateCnameLookup
  #### CNAME-Lookup beim Aushandeln der Kerberos-Authentifizierung deaktivieren
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Bestimmt, ob der generierte Kerberos-SPN auf dem kanonischen DNS-Namen (CNAME) oder auf dem ursprünglichen eingegebenen Namen basiert.

Wenn Sie diese Richtlinie aktivieren, wird die CNAME-Suche übersprungen und der Servername (wie eingegeben) verwendet.

Wenn Sie diese Richtlinie deaktivieren oder nicht konfigurieren, wird der kanonische Name des Servers verwendet. Dieser wird durch die CNAME-Suche bestimmt.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Nein - Erfordert einen Neustart des Browsers

  #### Datentyp:
  Boolesch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: DisableAuthNegotiateCnameLookup
  - Gruppenrichtlinienname: CNAME-Lookup beim Aushandeln der Kerberos-Authentifizierung deaktivieren
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/HTTP-Authentifizierung
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: DisableAuthNegotiateCnameLookup
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000000
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: DisableAuthNegotiateCnameLookup
  - Beispielwert:
``` xml
<false/>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### EnableAuthNegotiatePort
  #### Nicht standardmäßigen Port in Kerberos-SPN einschließen
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Gibt an, ob der generierte Kerberos-SPN einen nicht standardmäßigen Anschluss enthalten soll

Wenn Sie diese Richtlinie aktivieren und ein Benutzer einen nicht standardmäßigen Port (einen anderen Port als 80 oder 443) in einer URL enthält, ist dieser in den generierten Kerberos-SPN enthalten

Wenn Sie diese Richtlinie nicht konfigurieren oder deaktivieren, enthalten die generierten Kerberos-SPN in keinem Fall einen Port.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Nein - Erfordert einen Neustart des Browsers

  #### Datentyp:
  Boolesch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: EnableAuthNegotiatePort
  - Gruppenrichtlinienname: Nicht standardmäßigen Port in Kerberos-SPN einschließen
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/HTTP-Authentifizierung
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: EnableAuthNegotiatePort
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000000
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: EnableAuthNegotiatePort
  - Beispielwert:
``` xml
<false/>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### NtlmV2Enabled
  #### Steuern, ob die NTLMv2-Authentifizierung aktiviert ist
  >Unterstützte Versionen: Microsoft Edge unter Mac seit Version 77 oder höher

  #### Beschreibung
  Steuert, ob NTLMv2 aktiviert ist.

Alle neueren Versionen von Samba- und Windows-Servern unterstützen NTLMv2. Sie sollten NTLMv2 nur deaktivieren, um Probleme mit Rückwärtskompatibilität zu beheben, da dadurch die Sicherheit der Authentifizierung verringert wird.

Wenn Sie diese Richtlinie nicht konfigurieren, ist NTLMv2 standardmäßig aktiviert.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Boolesch

  

  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: NtlmV2Enabled
  - Beispielwert:
``` xml
<true/>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ## Inhaltseinstellungen policies

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### AutoSelectCertificateForUrls
  #### Clientzertifikate für diese Websites automatisch auswählen
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Geben Sie eine Websiteliste auf der Grundlage von URL-Mustern an, für die Microsoft Edge automatisch ein Clientzertifikat auswählen soll, wenn von der Website eines angefordert wird.

Der Wert muss ein Zeichenfolgenarray mit JSON-Wörterbüchern sein. Die einzelnen Wörterbücher müssen jeweils das Format { "pattern": "$URL_PATTERN", "filter" : $FILTER } besitzen, wobei $URL_PATTERN ein Inhaltseinstellungsmuster ist. $FILTER schränkt ein, welche Clientzertifikate der Browser automatisch auswählen kann. Unabhängig von diesem Filter können nur Zertifikate verwendet werden, die der Zertifikatanforderung des Servers entsprechen. Beispiel: Wenn $FILTER das Format { "ISSUER": { "CN": "$ISSUER_CN" } } hat, können zusätzlich nur Clientzertifikate verwendet werden, die von einem Zertifikat mit dem allgemeinen Namen $ISSUER_CN ausgestellt wurden. Wenn $FILTER einen Abschnitt vom Typ "ISSUER" und einen Abschnitt vom Typ "SUBJECT" enthält, muss ein Clientzertifikat beide Bedingungen erfüllen, um ausgewählt werden zu können. Wenn $FILTER eine Organisation („O“) angibt, muss ein Zertifikat über mindestens eine Organisation verfügen, die dem angegebenen Wert entspricht, um ausgewählt werden zu können. Wenn $FILTER eine Organisationseinheit („OU“) angibt, muss ein Zertifikat über mindestens eine Organisationseinheit verfügen, die dem angegebenen Wert entspricht, um ausgewählt werden zu können. Wenn es sich bei $FILTER um das leere Wörterbuch {} handelt, wird die Clientzertifikatauswahl nicht weiter eingeschränkt.

Wenn Sie diese Richtlinie nicht konfigurieren, erfolgt keine automatische Auswahl für Websites.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Liste der Zeichenfolgen

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: AutoSelectCertificateForUrls
  - Gruppenrichtlinienname: Clientzertifikate für diese Websites automatisch auswählen
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/Inhaltseinstellungen
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge\AutoSelectCertificateForUrls
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: 1, 2, 3, ...
  - Werttyp: Liste von REG_SZ
  ##### Beispielwert:
```
SOFTWARE\Policies\Microsoft\Edge\AutoSelectCertificateForUrls\0 = "{"pattern":"https://www.contoso.com","filter":{"ISSUER":{"CN":"certificate issuer name", "L": "certificate issuer location", "O": "certificate issuer org", "OU": "certificate issuer org unit"}, "SUBJECT":{"CN":"certificate subject name", "L": "certificate subject location", "O": "certificate subject org", "OU": "certificate subject org unit"}}}"

```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: AutoSelectCertificateForUrls
  - Beispielwert:
``` xml
<array>
  <string>{"pattern":"https://www.contoso.com","filter":{"ISSUER":{"CN":"certificate issuer name", "L": "certificate issuer location", "O": "certificate issuer org", "OU": "certificate issuer org unit"}, "SUBJECT":{"CN":"certificate subject name", "L": "certificate subject location", "O": "certificate subject org", "OU": "certificate subject org unit"}}}</string>
</array>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### CookiesAllowedForUrls
  #### Cookies auf bestimmten Websites zulassen
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Definiert basierend auf URL-Mustern eine Liste von Sites, die Cookies setzen dürfen.

Wenn Sie diese Richtlinie nicht konfigurieren, wird für alle Sites der globale Standardwert (falls festgelegt) aus der Richtlinie [DefaultCookiesSetting](#defaultcookiessetting) oder die persönliche Konfiguration des Benutzers verwendet.

Weitere Informationen finden Sie in den Richtlinien [CookiesBlockedForUrls](#cookiesblockedforurls) und [CookiesSessionOnlyForUrls](#cookiessessiononlyforurls).

Beachten Sie, dass es keine widersprüchlichen URL-Muster für die folgenden drei Richtlinien geben darf:

- [CookiesBlockedForUrls](#cookiesblockedforurls)

- CookiesAllowedForUrls

- [CookiesSessionOnlyForUrls](#cookiessessiononlyforurls)

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Liste der Zeichenfolgen

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: CookiesAllowedForUrls
  - Gruppenrichtlinienname: Cookies auf bestimmten Websites zulassen
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/Inhaltseinstellungen
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge\CookiesAllowedForUrls
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: 1, 2, 3, ...
  - Werttyp: Liste von REG_SZ
  ##### Beispielwert:
```
SOFTWARE\Policies\Microsoft\Edge\CookiesAllowedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\CookiesAllowedForUrls\1 = "[*.]contoso.edu"

```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: CookiesAllowedForUrls
  - Beispielwert:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### CookiesBlockedForUrls
  #### Cookies auf bestimmten Websites blockieren
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Definiert basierend auf URL-Mustern eine Liste von Sites, die keine Cookies setzen dürfen.

Wenn Sie diese Richtlinie nicht konfigurieren, wird für alle Sites der globale Standardwert (falls festgelegt) aus der Richtlinie [DefaultCookiesSetting](#defaultcookiessetting) oder die persönliche Konfiguration des Benutzers verwendet.

Weitere Informationen finden Sie in den Richtlinien [CookiesAllowedForUrls](#cookiesallowedforurls) und [CookiesSessionOnlyForUrls](#cookiessessiononlyforurls).

Beachten Sie, dass es keine widersprüchlichen URL-Muster für die folgenden drei Richtlinien geben darf:

- CookiesBlockedForUrls

- [CookiesAllowedForUrls](#cookiesallowedforurls)

- [CookiesSessionOnlyForUrls](#cookiessessiononlyforurls)

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Liste der Zeichenfolgen

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: CookiesBlockedForUrls
  - Gruppenrichtlinienname: Cookies auf bestimmten Websites blockieren
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/Inhaltseinstellungen
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge\CookiesBlockedForUrls
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: 1, 2, 3, ...
  - Werttyp: Liste von REG_SZ
  ##### Beispielwert:
```
SOFTWARE\Policies\Microsoft\Edge\CookiesBlockedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\CookiesBlockedForUrls\1 = "[*.]contoso.edu"

```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: CookiesBlockedForUrls
  - Beispielwert:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### CookiesSessionOnlyForUrls
  #### Cookies von bestimmten Websites auf die aktuelle Sitzung beschränken
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Cookies, die von Websites erstellt werden, die einem von Ihnen definierten URL-Muster entsprechen, werden nach Beendigung der Sitzung (wenn das Fenster geschlossen wird) gelöscht.

Cookies, die von Websites erstellt werden, die nicht mit dem Muster übereinstimmen, werden durch die Richtlinie [DefaultCookiesSetting](#defaultcookiessetting) (falls konfiguriert) oder durch die persönliche Konfiguration des Benutzers gesteuert. Dies ist auch das Standardverhalten, wenn Sie diese Richtlinie nicht konfigurieren.

Wenn Microsoft Edge im Hintergrundmodus läuft, wird die Sitzung möglicherweise nicht geschlossen, nachdem das letzte Fenster geschlossen wurde, was bedeutet, dass die Cookies beim Schließen des Fensters nicht gelöscht werden. In der Richtlinie [BackgroundModeEnabled](#backgroundmodeenabled) finden Sie Informationen über das Verhalten von Microsoft Edge im Hintergrundmodus.

Sie können auch die Richtlinien [CookiesAllowedForUrls](#cookiesallowedforurls) und [CookiesBlockedForUrls](#cookiesblockedforurls) verwenden, um zu steuern, welche Websites Cookies erstellen können.

Beachten Sie, dass es keine widersprüchlichen URL-Muster für die folgenden drei Richtlinien geben darf:

- [CookiesBlockedForUrls](#cookiesblockedforurls)

- [CookiesAllowedForUrls](#cookiesallowedforurls)

- CookiesSessionOnlyForUrls

Wenn Sie die Richtlinie [RestoreOnStartup](#restoreonstartup) zur Wiederherstellung von URLs aus früheren Sitzungen aktivieren, wird diese Richtlinie ignoriert, und Cookies werden für diese Seiten dauerhaft gespeichert.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Liste der Zeichenfolgen

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: CookiesSessionOnlyForUrls
  - Gruppenrichtlinienname: Cookies von bestimmten Websites auf die aktuelle Sitzung beschränken
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/Inhaltseinstellungen
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge\CookiesSessionOnlyForUrls
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: 1, 2, 3, ...
  - Werttyp: Liste von REG_SZ
  ##### Beispielwert:
```
SOFTWARE\Policies\Microsoft\Edge\CookiesSessionOnlyForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\CookiesSessionOnlyForUrls\1 = "[*.]contoso.edu"

```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: CookiesSessionOnlyForUrls
  - Beispielwert:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### DefaultCookiesSetting
  #### Cookies konfigurieren
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Steuert, ob Websites Cookies auf dem Gerät des Benutzers erstellen können. Es kann entweder jede oder keine Website Cookies erstellen. Sie können diese Richtlinie nicht verwenden, um Cookies von bestimmten Websites zuzulassen.

Legen Sie die Richtlinie auf "SessionOnly" (4) fest, um Cookies zu löschen, wenn die Sitzung geschlossen wird. Wird Microsoft Edge im Hintergrundmodus ausgeführt, wird die Sitzung möglicherweise nicht geschlossen, sobald das letzte Fenster geschlossen wird, was bedeutet, dass die Cookies nicht gelöscht werden, wenn das Fenster geschlossen wird. In der Richtlinie [BackgroundModeEnabled](#backgroundmodeenabled) finden Sie weitere Informationen über das Verhalten von Microsoft Edge im Hintergrundmodus.

Wenn Sie diese Richtlinie nicht konfigurieren, wird die Standardeinstellung 'AllowCookies' (1) verwendet, und Benutzer können diese Einstellung in den Microsoft Edge-Einstellungen ändern. (Wenn Sie nicht möchten, dass Benutzer diese Einstellung ändern können, legen Sie die Richtlinie fest.)

* 1 = Alle Sites dürfen Cookies erstellen

* 2 = Keine Site darf Cookies erstellen

* 4 = Cookies nur für die Dauer der Sitzung speichern

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Ganze Zahl

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: DefaultCookiesSetting
  - Gruppenrichtlinienname: Cookies konfigurieren
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/Inhaltseinstellungen
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: DefaultCookiesSetting
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000001
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: DefaultCookiesSetting
  - Beispielwert:
``` xml
<integer>1</integer>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### DefaultGeolocationSetting
  #### Standardeinstellung für Geolocation
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Legen Sie fest, ob Websites die physischen Standorte der Benutzer nachverfolgen können. Sie können die Nachverfolgung standardmäßig zulassen (1), sie standardmäßig verweigern (2) oder den Benutzer bei jeder Anforderung einer Website (3) fragen.

Wenn Sie diese Richtlinie nicht konfigurieren, wird die Richtlinie „AskGeolocation“ verwendet, und der Benutzer kann sie ändern.

* 1 = Websites erlauben, die physischen Standorte der Benutzer zu verfolgen

* 2 = Keiner Website das Nachverfolgen der physischen Standorte der Benutzer erlauben

* 3 = Fragen, wenn eine Website die physischen Standorte der Benutzer nachverfolgen möchte

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Ganze Zahl

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: DefaultGeolocationSetting
  - Gruppenrichtlinienname: Standardeinstellung für Geolocation
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/Inhaltseinstellungen
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: DefaultGeolocationSetting
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000001
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: DefaultGeolocationSetting
  - Beispielwert:
``` xml
<integer>1</integer>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### DefaultImagesSetting
  #### Standardeinstellung für Bilder
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Legen Sie fest, ob Websites Bilder anzeigen können. Sie können es für Bilder auf allen Websites (1) zulassen oder für alle Websites (2) sperren.

Falls Sie diese Richtlinie nicht konfigurieren, sind Bilder standardmäßig erlaubt, und der Benutzer kann diese Einstellung ändern.

* 1 = Allen Websites erlauben, alle Bilder anzuzeigen

* 2 = Keiner Website erlauben, Bilder anzuzeigen

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Ganze Zahl

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: DefaultImagesSetting
  - Gruppenrichtlinienname: Standardeinstellung für Bilder
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/Inhaltseinstellungen
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: DefaultImagesSetting
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000001
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: DefaultImagesSetting
  - Beispielwert:
``` xml
<integer>1</integer>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### DefaultJavaScriptSetting
  #### Standard-JavaScript-Einstellung
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Legen Sie fest, ob Websites JavaScript ausführen können. Sie können das für alle Websites (1) zulassen oder für alle Websites (2) sperren.

Falls Sie diese Richtlinie nicht konfigurieren, können alle Websites standardmäßig JavaScript ausführen, und der Benutzer kann diese Einstellung ändern.

* 1 = Allen Websites erlauben, JavaScript auszuführen

* 2 = Keiner Website erlauben, JavaScript auszuführen

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Ganze Zahl

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: DefaultJavaScriptSetting
  - Gruppenrichtlinienname: Standard-JavaScript-Einstellung
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/Inhaltseinstellungen
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: DefaultJavaScriptSetting
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000001
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: DefaultJavaScriptSetting
  - Beispielwert:
``` xml
<integer>1</integer>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### DefaultNotificationsSetting
  #### Standard-Benachrichtigungseinstellung
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Legen Sie fest, ob Websites Desktopbenachrichtigungen anzeigen dürfen. Sie können sie standardmäßig zulassen (1), sie standardmäßig verweigern (2) oder den Benutzer jedes Mal fragen, wenn eine Website eine Benachrichtigung anzeigen möchte (3).

Wenn Sie diese Richtlinie nicht konfigurieren, sind Benachrichtigungen standardmäßig zulässig, und der Benutzer kann diese Einstellung ändern.

* 1 = Zulassen, dass Websites Desktopbenachrichtigungen anzeigen.

* 2 = Keine Website zum Anzeigen von Desktopbenachrichtigungen zulassen.

* 3 = Jedes Mal nachfragen, wenn eine Website Desktopbenachrichtigungen anzeigen soll.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Ganze Zahl

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: DefaultNotificationsSetting
  - Gruppenrichtlinienname: Standard-Benachrichtigungseinstellung
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/Inhaltseinstellungen
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: DefaultNotificationsSetting
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000002
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: DefaultNotificationsSetting
  - Beispielwert:
``` xml
<integer>2</integer>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### DefaultPluginsSetting
  #### Standardeinstellung für Adobe Flash
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Legt fest, ob Websites, die nicht von [PluginsAllowedForUrls](#pluginsallowedforurls) oder [PluginsBlockedForUrls](#pluginsblockedforurls) abgedeckt sind, automatisch das Adobe Flash-Plug-In ausführen. Sie können 'BlockPlugins' (2) auswählen, um Adobe Flash auf allen Seiten zu blockieren, oder Sie können 'ClickToPlay' (3) wählen, um Adobe Flash ausführen zu lassen, aber den Benutzer auffordern, zum Starten auf den Platzhalter zu klicken. Auf jeden Fall haben die Richtlinien [PluginsAllowedForUrls](#pluginsallowedforurls) und [PluginsBlockedForUrls](#pluginsblockedforurls) Vorrang vor 'DefaultPluginsSetting'.

Die automatische Wiedergabe ist nur für Domänen zulässig, die explizit in der Richtlinie [PluginsAllowedForUrls](#pluginsallowedforurls) aufgeführt sind. Wenn Sie die automatische Wiedergabe für alle Sites aktivieren möchten, sollten Sie http://* und https://* zu dieser Liste hinzufügen.

Wenn Sie diese Richtlinie nicht konfigurieren, kann der Benutzer diese Einstellung manuell ändern.

* 2 = Plug-In Adobe Flash blockieren

* 3 = Wiedergabe durch Anklicken

Das frühere '1' Option erlaubte die Wiedergabe allgemein, aber diese Funktionalität wird nun nur noch von der Richtlinie [PluginsAllowedForUrls](#pluginsallowedforurls) verwaltet. In bestehende Richtlinien steht '1' für den Modus "Wiedergabe durch Anklicken".

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Ganze Zahl

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: DefaultPluginsSetting
  - Gruppenrichtlinienname: Standardeinstellung für Adobe Flash
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/Inhaltseinstellungen
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: DefaultPluginsSetting
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000002
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: DefaultPluginsSetting
  - Beispielwert:
``` xml
<integer>2</integer>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### DefaultPopupsSetting
  #### Standardeinstellung für Popupfenster
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Legen Sie fest, ob Websites Popupfenster anzeigen dürfen. Sie können sie auf allen Websites zulassen (1) oder auf allen Websites blockieren (2).

Wenn Sie diese Richtlinie nicht konfigurieren, werden Popupfenster standardmäßig blockiert, und Benutzer können diese Einstellung ändern.

* 1 = Zulassen, dass alle Websites Popups anzeigen

* 2 = Keiner Website das Anzeigen von Popupfenstern erlauben

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Ganze Zahl

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: DefaultPopupsSetting
  - Gruppenrichtlinienname: Standardeinstellung für Popupfenster
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/Inhaltseinstellungen
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: DefaultPopupsSetting
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000001
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: DefaultPopupsSetting
  - Beispielwert:
``` xml
<integer>1</integer>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### DefaultWebBluetoothGuardSetting
  #### Verwendung der Web-Bluetooth-API steuern
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Steuern Sie, ob Websites auf Bluetooth-Geräte in der Nähe zugreifen können. Sie können den Zugriff vollständig blockieren oder so konfigurieren, dass die Website den Benutzer bei jedem Zugriff auf ein Bluetooth-Gerät abfragen muss.

Wenn Sie diese Richtlinie nicht konfigurieren, wird der Standardwert (3, d. h., Benutzer werden jedes Mal abgefragt) verwendet, und Benutzer können ihn ändern.

* 2 = Keiner Website erlauben, den Zugriff auf Bluetooth-Geräte über die Web-Bluetooth-API anzufordern.

* 3 = Websites erlauben, den Zugriff auf ein Bluetooth-Gerät in der Nähe beim Benutzer anzufordern.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Ganze Zahl

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: DefaultWebBluetoothGuardSetting
  - Gruppenrichtlinienname: Verwendung der Web-Bluetooth-API steuern
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/Inhaltseinstellungen
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: DefaultWebBluetoothGuardSetting
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000002
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: DefaultWebBluetoothGuardSetting
  - Beispielwert:
``` xml
<integer>2</integer>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### DefaultWebUsbGuardSetting
  #### Verwendung der WebUSB-API steuern
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Legt fest, ob Websites auf angeschlossene USB-Geräte zugreifen können. Sie können den Zugriff vollständig blockieren oder den Benutzer jedes Mal fragen, wenn eine Website Zugriff auf angeschlossene USB-Geräte erhalten möchte.

Sie können diese Richtlinie für bestimmte URL-Muster mi den Richtlinien [WebUsbAskForUrls](#webusbaskforurls) und [WebUsbBlockedForUrls](#webusbblockedforurls) außer Kraft setzen.

Wenn Sie diese Richtlinie nicht konfigurieren, können Websites Benutzer fragen, ob sie standardmäßig auf die angeschlossenen USB-Geräte zugreifen können (3), und Benutzer können diese Einstellung ändern.

* 2 = Keine Site darf über die WebUSB-API den Zugriff auf USB-Geräte anfordern

* 3 = Websites dürfen den Benutzer auffordern, den Zugriff auf ein angeschlossenes USB-Gerät zu gewähren

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Ganze Zahl

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: DefaultWebUsbGuardSetting
  - Gruppenrichtlinienname: Verwendung der WebUSB-API steuern
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/Inhaltseinstellungen
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: DefaultWebUsbGuardSetting
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000002
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: DefaultWebUsbGuardSetting
  - Beispielwert:
``` xml
<integer>2</integer>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### ImagesAllowedForUrls
  #### Bilder auf diesen Websites zulassen
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Definiert basierend auf URL-Mustern eine Liste von Sites, die Bilder anzeigen dürfen.

Wenn Sie diese Richtlinie nicht konfigurieren, wird der globale Standardwert aus der Richtlinie [DefaultImagesSetting](#defaultimagessetting) (sofern festgelegt) oder der persönlichen Konfiguration des Benutzers für alle Websites verwendet.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Liste der Zeichenfolgen

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: ImagesAllowedForUrls
  - Gruppenrichtlinienname: Bilder auf diesen Websites zulassen
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/Inhaltseinstellungen
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge\ImagesAllowedForUrls
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: 1, 2, 3, ...
  - Werttyp: Liste von REG_SZ
  ##### Beispielwert:
```
SOFTWARE\Policies\Microsoft\Edge\ImagesAllowedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\ImagesAllowedForUrls\1 = "[*.]contoso.edu"

```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: ImagesAllowedForUrls
  - Beispielwert:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### ImagesBlockedForUrls
  #### Bilder auf bestimmten Websites blockieren
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Definiert basierend auf URL-Mustern eine Liste von Sites, die Bilder anzeigen dürfen.

Wenn Sie diese Richtlinie nicht konfigurieren, wird für alle Sites der globale Standardwert (falls festgelegt) aus der Richtlinie [DefaultImagesSetting](#defaultimagessetting) oder die persönliche Konfiguration des Benutzers verwendet.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Liste der Zeichenfolgen

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: ImagesBlockedForUrls
  - Gruppenrichtlinienname: Bilder auf bestimmten Websites blockieren
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/Inhaltseinstellungen
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge\ImagesBlockedForUrls
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: 1, 2, 3, ...
  - Werttyp: Liste von REG_SZ
  ##### Beispielwert:
```
SOFTWARE\Policies\Microsoft\Edge\ImagesBlockedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\ImagesBlockedForUrls\1 = "[*.]contoso.edu"

```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: ImagesBlockedForUrls
  - Beispielwert:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### JavaScriptAllowedForUrls
  #### JavaScript auf bestimmten Websites zulassen
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Definiert basierend auf URL-Mustern eine Liste von Sites, auf denen die Ausführung von JavaScript erlaubt ist.

Wenn Sie diese Richtlinie nicht konfigurieren, wird für alle Sites der globale Standardwert (falls festgelegt) aus der Richtlinie [DefaultJavaScriptSetting](#defaultjavascriptsetting) oder die persönliche Konfiguration des Benutzers verwendet.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Liste der Zeichenfolgen

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: JavaScriptAllowedForUrls
  - Gruppenrichtlinienname: JavaScript auf bestimmten Websites zulassen
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/Inhaltseinstellungen
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge\JavaScriptAllowedForUrls
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: 1, 2, 3, ...
  - Werttyp: Liste von REG_SZ
  ##### Beispielwert:
```
SOFTWARE\Policies\Microsoft\Edge\JavaScriptAllowedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\JavaScriptAllowedForUrls\1 = "[*.]contoso.edu"

```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: JavaScriptAllowedForUrls
  - Beispielwert:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### JavaScriptBlockedForUrls
  #### JavaScript auf bestimmten Websites blockieren
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Definiert basierend auf URL-Mustern eine Liste von Sites, auf denen die Ausführung von JavaScript blockiert wird.

Wenn Sie diese Richtlinie nicht konfigurieren, wird für alle Sites der globale Standardwert (falls festgelegt) aus der Richtlinie [DefaultJavaScriptSetting](#defaultjavascriptsetting) oder die persönliche Konfiguration des Benutzers verwendet.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Liste der Zeichenfolgen

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: JavaScriptBlockedForUrls
  - Gruppenrichtlinienname: JavaScript auf bestimmten Websites blockieren
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/Inhaltseinstellungen
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge\JavaScriptBlockedForUrls
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: 1, 2, 3, ...
  - Werttyp: Liste von REG_SZ
  ##### Beispielwert:
```
SOFTWARE\Policies\Microsoft\Edge\JavaScriptBlockedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\JavaScriptBlockedForUrls\1 = "[*.]contoso.edu"

```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: JavaScriptBlockedForUrls
  - Beispielwert:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### LegacySameSiteCookieBehaviorEnabled
  #### Einstellung des standardmäßigen Cookieverhaltens für SameSite der Vorgängerversion aktivieren
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 80 oder höher

  #### Beschreibung
  Ermöglicht das Zurücksetzen aller Cookies auf das Verhalten der Vorgängerversion für SameSite. Das Zurücksetzen auf das Verhalten der Vorgängerversion bewirkt, dass Cookies, die kein SameSite-Attribut angeben, so behandelt werden, als ob sie "SameSite=None" wären, und "SameSite=None"-Cookies müssen das "Secure"-Attribut nicht mehr enthalten.

Sie können die folgenden Werte für diese Richtlinie festlegen:

* 1 = Zurücksetzen auf Verhalten der Vorgängerversion für SameSite für Cookies auf allen Websites

* 2 = Verhalten für SameSite-by-default für Cookies auf allen Websites verwenden

Wenn Sie diese Richtlinie nicht festlegen, hängt das Standardverhalten für Cookies, die kein SameSite-Attribut angeben, von anderen Konfigurationsquellen für die SameSite-by-default-Funktion ab. Diese Funktion kann durch einen Feld-Text oder durch Aktivieren des same-site-by-default-cookies-Flags in „edge://flags“ festgelegt werden.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Ganze Zahl

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: LegacySameSiteCookieBehaviorEnabled
  - Gruppenrichtlinienname: Einstellung des standardmäßigen Cookieverhaltens für SameSite der Vorgängerversion aktivieren
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/Inhaltseinstellungen
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: LegacySameSiteCookieBehaviorEnabled
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000001
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: LegacySameSiteCookieBehaviorEnabled
  - Beispielwert:
``` xml
<integer>1</integer>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### LegacySameSiteCookieBehaviorEnabledForDomainList
  #### Zurücksetzen auf das Verhalten der Vorgängerversion für SameSite für Cookies auf bestimmten Websites
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 80 oder höher

  #### Beschreibung
  Cookies, die für Domänen festgelegt sind, die bestimmten Mustern entsprechen, werden auf das Verhalten für SameSite zurückgesetzt.

Das Zurücksetzen auf das Verhalten der Vorgängerversion bewirkt, dass Cookies, die kein SameSite-Attribut angeben, so behandelt werden, als ob sie "SameSite=None" wären, und "SameSite=None"-Cookies müssen das "Secure"-Attribut nicht mehr enthalten.

Wenn Sie diese Richtlinie nicht festlegen, wird der globale Standardwert verwendet. Der globale Standard wird auch für Cookies auf Domänen verwendet, die nicht durch die von Ihnen angegebenen Muster abgedeckt sind.

Der globale Standardwert kann mithilfe der Richtlinie [LegacySameSiteCookieBehaviorEnabled](#legacysamesitecookiebehaviorenabled) konfiguriert werden. Wenn [LegacySameSiteCookieBehaviorEnabled](#legacysamesitecookiebehaviorenabled) aufgehoben wird, wird der globale Standardwert auf andere Konfigurationsquellen zurückgesetzt.

Beachten Sie, dass Muster, die Sie in dieser Richtlinie auflisten, als Domänen und nicht als URLs behandelt werden, daher sollten Sie kein Schema und keinen Port angeben.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Liste der Zeichenfolgen

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: LegacySameSiteCookieBehaviorEnabledForDomainList
  - Gruppenrichtlinienname: Zurücksetzen auf das Verhalten der Vorgängerversion für SameSite für Cookies auf bestimmten Websites
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/Inhaltseinstellungen
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge\LegacySameSiteCookieBehaviorEnabledForDomainList
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: 1, 2, 3, ...
  - Werttyp: Liste von REG_SZ
  ##### Beispielwert:
```
SOFTWARE\Policies\Microsoft\Edge\LegacySameSiteCookieBehaviorEnabledForDomainList\0 = "www.example.com"
SOFTWARE\Policies\Microsoft\Edge\LegacySameSiteCookieBehaviorEnabledForDomainList\1 = "[*.]example.edu"

```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: LegacySameSiteCookieBehaviorEnabledForDomainList
  - Beispielwert:
``` xml
<array>
  <string>www.example.com</string>
  <string>[*.]example.edu</string>
</array>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### NotificationsAllowedForUrls
  #### Benachrichtigungen auf bestimmten Websites zulassen
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Definiert eine Liste von Websites, die auf URL-Mustern basieren und Benachrichtigungen anzeigen können.

Wenn Sie diese Richtlinie nicht konfigurieren, wird für alle Sites der globale Standardwert (falls festgelegt) aus der Richtlinie [DefaultNotificationsSetting](#defaultnotificationssetting) oder die persönliche Konfiguration des Benutzers verwendet.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Liste der Zeichenfolgen

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: NotificationsAllowedForUrls
  - Gruppenrichtlinienname: Benachrichtigungen auf bestimmten Websites zulassen
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/Inhaltseinstellungen
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge\NotificationsAllowedForUrls
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: 1, 2, 3, ...
  - Werttyp: Liste von REG_SZ
  ##### Beispielwert:
```
SOFTWARE\Policies\Microsoft\Edge\NotificationsAllowedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\NotificationsAllowedForUrls\1 = "[*.]contoso.edu"

```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: NotificationsAllowedForUrls
  - Beispielwert:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### NotificationsBlockedForUrls
  #### Benachrichtigungen auf bestimmten Websites blockieren
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Definiert basierend auf URL-Mustern eine Liste von Sites, auf denen die Anzeige von Benachrichtigungen blockiert wird.

Wenn Sie diese Richtlinie nicht konfigurieren, wird für alle Sites der globale Standardwert aus der Richtlinie [DefaultNotificationsSetting](#defaultnotificationssetting) (falls festgelegt) oder die persönliche Konfiguration des Benutzers verwendet.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Liste der Zeichenfolgen

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: NotificationsBlockedForUrls
  - Gruppenrichtlinienname: Benachrichtigungen auf bestimmten Websites blockieren
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/Inhaltseinstellungen
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge\NotificationsBlockedForUrls
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: 1, 2, 3, ...
  - Werttyp: Liste von REG_SZ
  ##### Beispielwert:
```
SOFTWARE\Policies\Microsoft\Edge\NotificationsBlockedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\NotificationsBlockedForUrls\1 = "[*.]contoso.edu"

```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: NotificationsBlockedForUrls
  - Beispielwert:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### PluginsAllowedForUrls
  #### Adobe Flash-Plug-In auf bestimmten Websites zulassen
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Definiert basierend auf URL-Mustern eine Liste von Sites, auf denen das Adobe Flash-Plug-In ausgeführt werden darf.

Wenn Sie diese Richtlinie nicht konfigurieren, wird für alle Sites der globale Standardwert aus der Richtlinie [DefaultPluginsSetting](#defaultpluginssetting) (falls festgelegt) oder die persönliche Konfiguration des Benutzers verwendet.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Liste der Zeichenfolgen

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: PluginsAllowedForUrls
  - Gruppenrichtlinienname: Adobe Flash-Plug-In auf bestimmten Websites zulassen
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/Inhaltseinstellungen
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge\PluginsAllowedForUrls
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: 1, 2, 3, ...
  - Werttyp: Liste von REG_SZ
  ##### Beispielwert:
```
SOFTWARE\Policies\Microsoft\Edge\PluginsAllowedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\PluginsAllowedForUrls\1 = "[*.]contoso.edu"

```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: PluginsAllowedForUrls
  - Beispielwert:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### PluginsBlockedForUrls
  #### Adobe Flash-Plug-In auf bestimmten Websites blockieren
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Definiert basierend auf URL-Mustern eine Liste von Sites, auf denen Adobe Flash blockiert wird.

Wenn Sie diese Richtlinie nicht konfigurieren, wird für alle Sites der globale Standardwert aus der Richtlinie [DefaultPluginsSetting](#defaultpluginssetting) (falls festgelegt) oder die persönliche Konfiguration des Benutzers verwendet.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Liste der Zeichenfolgen

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: PluginsBlockedForUrls
  - Gruppenrichtlinienname: Adobe Flash-Plug-In auf bestimmten Websites blockieren
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/Inhaltseinstellungen
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge\PluginsBlockedForUrls
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: 1, 2, 3, ...
  - Werttyp: Liste von REG_SZ
  ##### Beispielwert:
```
SOFTWARE\Policies\Microsoft\Edge\PluginsBlockedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\PluginsBlockedForUrls\1 = "[*.]contoso.edu"

```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: PluginsBlockedForUrls
  - Beispielwert:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### PopupsAllowedForUrls
  #### Popupfenster auf bestimmten Websites zulassen
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Definiert basierend auf URL-Mustern eine Liste von Sites, die Popup-Fenstern öffnen dürfen.

Wenn Sie diese Richtlinie nicht konfigurieren, wird für alle Sites der globale Standardwert (falls festgelegt) aus der Richtlinie [DefaultPopupsSetting](#defaultpopupssetting) oder die persönliche Konfiguration des Benutzers verwendet.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Liste der Zeichenfolgen

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: PopupsAllowedForUrls
  - Gruppenrichtlinienname: Popupfenster auf bestimmten Websites zulassen
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/Inhaltseinstellungen
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge\PopupsAllowedForUrls
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: 1, 2, 3, ...
  - Werttyp: Liste von REG_SZ
  ##### Beispielwert:
```
SOFTWARE\Policies\Microsoft\Edge\PopupsAllowedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\PopupsAllowedForUrls\1 = "[*.]contoso.edu"

```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: PopupsAllowedForUrls
  - Beispielwert:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### PopupsBlockedForUrls
  #### Popupfenster auf bestimmten Websites blockieren
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Definiert basierend auf URL-Mustern eine Liste von Sites, auf denen das Öffnen von Popup-Fenstern blockiert wird.

Wenn Sie diese Richtlinie nicht konfigurieren, wird für alle Sites der globale Standardwert (falls festgelegt) aus der Richtlinie [DefaultPopupsSetting](#defaultpopupssetting) oder die persönliche Konfiguration des Benutzers verwendet.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Liste der Zeichenfolgen

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: PopupsBlockedForUrls
  - Gruppenrichtlinienname: Popupfenster auf bestimmten Websites blockieren
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/Inhaltseinstellungen
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge\PopupsBlockedForUrls
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: 1, 2, 3, ...
  - Werttyp: Liste von REG_SZ
  ##### Beispielwert:
```
SOFTWARE\Policies\Microsoft\Edge\PopupsBlockedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\PopupsBlockedForUrls\1 = "[*.]contoso.edu"

```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: PopupsBlockedForUrls
  - Beispielwert:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### RegisteredProtocolHandlers
  #### Protokollhandler registrieren
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Registriert eine Liste mit Protokollhandlern. Legen Sie die Protokolleigenschaft auf das Schema (beispielsweise „mailto“) und die URL-Eigenschaft auf das URL-Muster der Anwendung fest, die das Schema behandelt. Das Muster kann ein Vorkommen von „%s“ enthalten, das später durch die behandelte URL ersetzt wird.

Sie können einen bestimmten Wert für diese Richtlinie vorschlagen, dessen Verwendung aber für Ihre Benutzer nicht erzwingen.

Die von der Richtlinie registrierten Protokollhandler werden mit ggf. vom Benutzer registrierten Handlern zusammengeführt, und beide können verwendet werden. Der Benutzer kann die durch die Richtlinie installierten Protokollhandler überschreiben, indem er einen neuen Standardhandler installiert. Er kann jedoch keine von der Richtlinie registrierten Protokollhandler entfernen.

  #### Unterstützte Features:
  - Kann zwingend sein: Nein
  - Kann empfohlen werden: Ja
  - Dynamische Richtlinienaktualisierung: Nein - Erfordert einen Neustart des Browsers

  #### Datentyp:
  Wörterbuch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: RegisteredProtocolHandlers
  - Gruppenrichtlinienname: Protokollhandler registrieren
  - Gruppenrichtlinienpfad (Erforderlich): Nicht zutreffend
  - Gruppenrichtlinienpfad (Empfohlen): Administrative Vorlagen/Microsoft Edge - Standardeinstellungen (können durch Benutzer überschrieben werden)/Inhaltseinstellungen
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): Nicht zutreffend
  - Pfad (Empfohlen): SOFTWARE\Policies\Microsoft\Edge\Empfohlen
  - Wertname: RegisteredProtocolHandlers
  - Werttyp: REG_SZ
  ##### Beispielwert:
```
SOFTWARE\Policies\Microsoft\Edge\RegisteredProtocolHandlers = [
  {
    "default": true, 
    "protocol": "mailto", 
    "url": "https://mail.contoso.com/mail/?extsrc=mailto&url=%s"
  }
]
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: RegisteredProtocolHandlers
  - Beispielwert:
``` xml
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
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### WebUsbAllowDevicesForUrls
  #### Gewährt bestimmten Websites Zugriff, damit eine Verbindung mit bestimmten USB-Geräten hergestellt werden kann.
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Ermöglicht es Ihnen, eine Liste von URLs anzugeben, die festlegen, welche Websites automatisch die Berechtigung zum Zugriff auf ein USB-Gerät mit den angegebenen Hersteller- und Produkt-IDs erhalten. Jedes Element in der Liste muss sowohl Geräte als auch URLs enthalten, damit die Richtlinie gültig ist. Jedes Element in Geräten kann eine Lieferanten-ID und ein Produkt-ID-Feld enthalten. Jede fehlende ID wird mit einer Ausnahme als Wildcard behandelt, und diese Ausnahme besteht darin, dass eine Produkt-ID nicht angegeben werden kann, ohne dass auch eine Lieferanten-ID angegeben wird. Andernfalls ist die Richtlinie nicht gültig und wird ignoriert.

Das USB-Berechtigungsmodell verwendet die URL der anfragenden Website ("anfragende URL") und die URL der obersten Frame-Site ("eingebettete URL"), um der anfragenden URL die Berechtigung zum Zugriff auf das USB-Gerät zu erteilen. Die anfragende URL kann sich von der einbettenden URL unterscheiden, wenn die anfragende Website in einem Iframe geladen wird. Daher kann das Feld "urls" bis zu zwei URL-Zeichenketten enthalten, die durch ein Komma getrennt sind, um die anfragende bzw. einbettende URL anzugeben. Ist nur eine URL angegeben, wird der Zugriff auf die entsprechenden USB-Geräte gewährt, wenn die URL der anfragenden Website unabhängig vom Einbettungsstatus mit dieser URL übereinstimmt. Die URLs in "urls" müssen gültige URLs sein, sonst wird die Richtlinie ignoriert.

Wenn diese Richtlinie nicht festgelegt ist, wird der globale Standardwert für alle Websites verwendet, entweder aus der Richtlinie [DefaultWebUsbGuardSetting](#defaultwebusbguardsetting) (sofern festgelegt) oder aus der persönlichen Konfiguration des Benutzers.

Die URL-Muster in dieser Richtlinie dürfen nicht mit kollidieren, die in [WebUsbBlockedForUrls](#webusbblockedforurls) festgelegt sind. Wenn es zu einem Konflikt kommt, hat diese Richtlinie Vorrang vor [WebUsbBlockedForUrls](#webusbblockedforurls) und [WebUsbAskForUrls](#webusbaskforurls).

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Wörterbuch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: WebUsbAllowDevicesForUrls
  - Gruppenrichtlinienname: Gewährt bestimmten Websites Zugriff, damit eine Verbindung mit bestimmten USB-Geräten hergestellt werden kann.
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/Inhaltseinstellungen
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: WebUsbAllowDevicesForUrls
  - Werttyp: REG_SZ
  ##### Beispielwert:
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


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: WebUsbAllowDevicesForUrls
  - Beispielwert:
``` xml
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
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### WebUsbAskForUrls
  #### WebUSB auf bestimmten Websites zulassen
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Definiert basierend auf URL-Mustern eine Liste von Sites, die den Benutzer nicht auffordern können, ihm Zugriff auf ein USB-Gerät zu gewähren.

Wenn Sie diese Richtlinie nicht konfigurieren, wird für alle Sites der globale Standardwert aus der Richtlinie [DefaultWebUsbGuardSetting](#defaultwebusbguardsetting) (falls festgelegt) oder die persönliche Konfiguration des Benutzers verwendet.

Die in dieser Richtlinie definierten URL-Muster dürfen nicht mit denen aus der Richtlinie [WebUsbBlockedForUrls](#webusbblockedforurls) übereinstimmen, denn Sie können eine URL nicht gleichzeitig zulassen und blockieren.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Liste der Zeichenfolgen

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: WebUsbAskForUrls
  - Gruppenrichtlinienname: WebUSB auf bestimmten Websites zulassen
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/Inhaltseinstellungen
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge\WebUsbAskForUrls
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: 1, 2, 3, ...
  - Werttyp: Liste von REG_SZ
  ##### Beispielwert:
```
SOFTWARE\Policies\Microsoft\Edge\WebUsbAskForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\WebUsbAskForUrls\1 = "[*.]contoso.edu"

```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: WebUsbAskForUrls
  - Beispielwert:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### WebUsbBlockedForUrls
  #### WebUSB auf bestimmten Websites blockieren
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Definiert basierend auf URL-Mustern eine Liste von Sites, die den Benutzer nicht auffordern können, ihm Zugriff auf ein USB-Gerät zu gewähren.

Wenn Sie diese Richtlinie nicht konfigurieren, wird für alle Sites der globale Standardwert aus der Richtlinie [DefaultWebUsbGuardSetting](#defaultwebusbguardsetting) (falls festgelegt) oder die persönliche Konfiguration des Benutzers verwendet.

URL-Muster in dieser Richtlinie dürfen nicht mit denen aus der Richtlinie [WebUsbAskForUrls](#webusbaskforurls) übereinstimmen, denn Sie können eine URL nicht gleichzeitig zulassen und blockieren.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Liste der Zeichenfolgen

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: WebUsbBlockedForUrls
  - Gruppenrichtlinienname: WebUSB auf bestimmten Websites blockieren
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/Inhaltseinstellungen
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge\WebUsbBlockedForUrls
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: 1, 2, 3, ...
  - Werttyp: Liste von REG_SZ
  ##### Beispielwert:
```
SOFTWARE\Policies\Microsoft\Edge\WebUsbBlockedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\WebUsbBlockedForUrls\1 = "[*.]contoso.edu"

```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: WebUsbBlockedForUrls
  - Beispielwert:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ## Kennwort-Manager und -schutz policies

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### PasswordManagerEnabled
  #### Speichern von Kennwörtern im Kennwort-Manager ermöglichen
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Ermöglicht Microsoft Edge das Speichern von Benutzerkennwörtern.

Wenn Sie diese Richtlinie aktivieren, können Benutzer ihre Kennwörter in Microsoft Edge speichern. Beim nächsten Besuch der Website fügt Microsoft Edge das Kennwort automatisch ein.

Wenn Sie diese Richtlinie deaktivieren, können Benutzer keine neuen Kennwörter speichern. Zuvor gespeicherte Kennwörter können jedoch weiterhin verwendet werden.

Wenn Sie diese Richtlinie aktivieren oder deaktivieren, kann sie von Benutzern in Microsoft Edge nicht geändert oder überschrieben werden. Wenn Sie die Richtlinie nicht konfigurieren, können Benutzer Kennwörter speichern und dieses Feature deaktivieren.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Ja
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Boolesch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: PasswordManagerEnabled
  - Gruppenrichtlinienname: Speichern von Kennwörtern im Kennwort-Manager ermöglichen
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/Kennwort-Manager und -schutz
  - Gruppenrichtlinienpfad (Empfohlen): Administrative Vorlagen/Microsoft Edge - Standardeinstellungen (können durch Benutzer überschrieben werden)/Kennwort-Manager und -schutz
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): SOFTWARE\Policies\Microsoft\Edge\Empfohlen
  - Wertname: PasswordManagerEnabled
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000001
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: PasswordManagerEnabled
  - Beispielwert:
``` xml
<true/>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### PasswordProtectionChangePasswordURL
  #### URL zum Ändern des Kennworts konfigurieren
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Konfiguriert die URL zum Ändern des Kennworts (nur HTTP- und HTTPS-Schemas).

Der Kennwortschutzdienst leitet Benutzer an diese URL weiter, damit sie ihr Kennwort ändern können, nachdem eine Warnung im Browser angezeigt wurde.

Wenn Sie diese Richtlinie aktivieren, leitet der Kennwortschutzdienst Benutzer an diese URL weiter, damit sie ihr Kennwort ändern können.

Wenn Sie diese Richtlinie deaktivieren oder nicht konfigurieren, werden Benutzer nicht an eine URL für die Kennwortänderung weitergeleitet.

Diese Richtlinie ist nur für Windows-Instanzen verfügbar, die mit einer Microsoft Active Directory-Domäne oder mit Windows 10 Pro- oder Enterprise-Instanzen verknüpft sind, die für die Geräteverwaltung registriert sind.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Zeichenfolge

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: PasswordProtectionChangePasswordURL
  - Gruppenrichtlinienname: URL zum Ändern des Kennworts konfigurieren
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/Kennwort-Manager und -schutz
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: PasswordProtectionChangePasswordURL
  - Werttyp: REG_SZ
  ##### Beispielwert:
```
"https://contoso.com/change_password.html"
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: PasswordProtectionChangePasswordURL
  - Beispielwert:
``` xml
<string>https://contoso.com/change_password.html</string>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### PasswordProtectionLoginURLs
  #### Liste der Unternehmens-Anmelde-URLs konfigurieren, bei denen der Kennwortschutzdienst den Fingerabdruck des Kennworts aufzeichnen soll
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Konfigurieren Sie die Liste der Unternehmens-Anmelde-URLs (nur HTTP- und HTTPS-Schemas), bei denen Microsoft Edge den Fingerabdruck von Kennwörtern erfassen und zur Kennwort-Wiederverwendungserkennung verwenden soll.

Wenn Sie diese Richtlinie aktivieren, erfasst der Kennwortschutzdienst Fingerabdrücke von Kennwörtern für die definierten URLs.

Wenn Sie diese Richtlinie deaktivieren oder nicht konfigurieren, werden keine Kennwortfingerabdrücke erfasst.

Diese Richtlinie ist nur für Windows-Instanzen verfügbar, die mit einer Microsoft Active Directory-Domäne oder mit Windows 10 Pro- oder Enterprise-Instanzen verknüpft sind, die für die Geräteverwaltung registriert sind.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Liste der Zeichenfolgen

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: PasswordProtectionLoginURLs
  - Gruppenrichtlinienname: Liste der Unternehmens-Anmelde-URLs konfigurieren, bei denen der Kennwortschutzdienst den Fingerabdruck des Kennworts aufzeichnen soll
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/Kennwort-Manager und -schutz
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge\PasswordProtectionLoginURLs
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: 1, 2, 3, ...
  - Werttyp: Liste von REG_SZ
  ##### Beispielwert:
```
SOFTWARE\Policies\Microsoft\Edge\PasswordProtectionLoginURLs\0 = "https://contoso.com/login.html"
SOFTWARE\Policies\Microsoft\Edge\PasswordProtectionLoginURLs\1 = "https://login.contoso.com"

```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: PasswordProtectionLoginURLs
  - Beispielwert:
``` xml
<array>
  <string>https://contoso.com/login.html</string>
  <string>https://login.contoso.com</string>
</array>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### PasswordProtectionWarningTrigger
  #### Warnungstrigger für Kennwortschutz konfigurieren
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Steuert, wann eine Warnung zum Passwortschutz angezeigt werden soll. Der Passwortschutz warnt Benutzer, wenn sie ihr geschütztes Passwort auf potenziell verdächtigen Websites wiederverwenden.

Sie können die Richtlinien [PasswordProtectionLoginURLs](#passwordprotectionloginurls) und [PasswordProtectionChangePasswordURL](#passwordprotectionchangepasswordurl) verwenden, um zu konfigurieren, welche Passwörter geschützt werden sollen.

Ausnahmen: Passwörter, die in [PasswordProtectionLoginURLs](#passwordprotectionloginurls) und [PasswordProtectionChangePasswordURL](#passwordprotectionchangepasswordurl) aufgeführt sind, lösen keine Warnung für den Passwortschutz aus. Das gilt auch für alle in [SmartScreenAllowListDomains](#smartscreenallowlistdomains) angegebenen Sites.

Mit 'PasswordProtectionWarningOff' (0) werden keine Warnungen für den Passwortschutz angezeigt.

Mit 'PasswordProtectionWarningOnPasswordReuse' (1) werden Warnungen für den Passwortschutz angezeigt, wenn der Benutzer sein geschütztes Passwort auf einer nicht auf einer Whitelist stehenden Website wiederverwendet.

Wenn Sie diese Richtlinie deaktivieren oder nicht konfigurieren, wird der Warnungstrigger nicht angezeigt.

* 0 = Die Passwortschutzwarnung ist deaktiviert.

* 1 = Die Passwortschutzwarnung wird durch Passwortwiederholung ausgelöst.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Ganze Zahl

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: PasswordProtectionWarningTrigger
  - Gruppenrichtlinienname: Warnungstrigger für Kennwortschutz konfigurieren
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/Kennwort-Manager und -schutz
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: PasswordProtectionWarningTrigger
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000001
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: PasswordProtectionWarningTrigger
  - Beispielwert:
``` xml
<integer>1</integer>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ## Natives Messaging policies

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### NativeMessagingAllowlist
  #### Steuern, welche nativen Messaginghosts von Benutzern verwendet werden können
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Listet bestimmte native Messaging-Hosts auf, die Benutzer in Microsoft Edge verwenden können.

Standardmäßig sind alle nativen Messaging-Hosts zugelassen. Wenn Sie die Richtlinie [NativeMessagingBlocklist](#nativemessagingblocklist) auf * setzen, werden alle nativen Messaging-Hosts blockiert und nur die hier aufgeführten nativen Messaging-Hosts geladen.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Liste der Zeichenfolgen

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: NativeMessagingAllowlist
  - Gruppenrichtlinienname: Steuern, welche nativen Messaginghosts von Benutzern verwendet werden können
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/Natives Messaging
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge\NativeMessagingAllowlist
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: 1, 2, 3, ...
  - Werttyp: Liste von REG_SZ
  ##### Beispielwert:
```
SOFTWARE\Policies\Microsoft\Edge\NativeMessagingAllowlist\0 = "com.native.messaging.host.name1"
SOFTWARE\Policies\Microsoft\Edge\NativeMessagingAllowlist\1 = "com.native.messaging.host.name2"

```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: NativeMessagingAllowlist
  - Beispielwert:
``` xml
<array>
  <string>com.native.messaging.host.name1</string>
  <string>com.native.messaging.host.name2</string>
</array>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### NativeMessagingBlocklist
  #### Native Nachrichtensperrliste konfigurieren
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Gibt an, welche nativen Messaginghosts nicht verwendet werden sollen.

Verwenden Sie "*", um alle nativen Messaginghosts zu blockieren, sofern Sie nicht explizit in der Liste "Zulassen" aufgeführt sind.

Wenn Sie diese Richtlinie nicht konfigurieren, werden von Microsoft Edge alle installierten nativen Messaginghosts geladen.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Liste der Zeichenfolgen

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: NativeMessagingBlocklist
  - Gruppenrichtlinienname: Native Nachrichtensperrliste konfigurieren
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/Natives Messaging
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge\NativeMessagingBlocklist
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: 1, 2, 3, ...
  - Werttyp: Liste von REG_SZ
  ##### Beispielwert:
```
SOFTWARE\Policies\Microsoft\Edge\NativeMessagingBlocklist\0 = "com.native.messaging.host.name1"
SOFTWARE\Policies\Microsoft\Edge\NativeMessagingBlocklist\1 = "com.native.messaging.host.name2"

```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: NativeMessagingBlocklist
  - Beispielwert:
``` xml
<array>
  <string>com.native.messaging.host.name1</string>
  <string>com.native.messaging.host.name2</string>
</array>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### NativeMessagingUserLevelHosts
  #### Native Messaginghosts auf Benutzerebene zulassen (ohne Administratorberechtigungen installiert)
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Aktiviert die Installation von nativen Messaginghosts auf Benutzerebene.

Wenn sie diese Richtlinie deaktivieren, verwendet Microsoft Edge nur native Messaginghosts, die auf der Systemebene installiert sind.

Wenn sie diese Richtlinie nicht konfigurieren, wird von Microsoft Edge standardmäßig die Verwendung von nativen Messaginghosts auf Benutzerebene zugelassen.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Boolesch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: NativeMessagingUserLevelHosts
  - Gruppenrichtlinienname: Native Messaginghosts auf Benutzerebene zulassen (ohne Administratorberechtigungen installiert)
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/Natives Messaging
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: NativeMessagingUserLevelHosts
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000000
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: NativeMessagingUserLevelHosts
  - Beispielwert:
``` xml
<false/>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ## Proxyserver policies

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### ProxyBypassList
  #### Proxy-Umgehungsregeln konfigurieren
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Definiert eine Liste von Hosts, für die Microsoft Edge jeden Proxy umgeht.

Diese Richtlinie wird nur angewendet, wenn Sie 'Feste Proxy-Server verwenden' in der Richtlinie [ProxyMode](#proxymode) ausgewählt haben. Aktivieren oder konfigurieren Sie diese Richtlinie nicht, wenn Sie einen anderen Modus für die Konfiguration von Proxy-Richtlinien ausgewählt haben.

Wenn Sie diese Richtlinie aktivieren, können Sie eine Liste von Hosts erstellen, für die Microsoft Edge keinen Proxy verwendet.

Wenn Sie diese Richtlinie nicht konfigurieren, wird keine Liste der Hosts erstellt, für die Microsoft Edge einen Proxy umgeht. Konfigurieren Sie diese Richtlinie nicht, wenn Sie eine andere Methode zum Festlegen von Proxy-Richtlinien angegeben haben.

Detaillierte Beispiele finden Sie unter [https://go.microsoft.com/fwlink/?linkid=2094936](https://go.microsoft.com/fwlink/?linkid=2094936).

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Zeichenfolge

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: ProxyBypassList
  - Gruppenrichtlinienname: Proxy-Umgehungsregeln konfigurieren
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/Proxyserver
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: ProxyBypassList
  - Werttyp: REG_SZ
  ##### Beispielwert:
```
"https://www.contoso.com, https://www.fabrikam.com"
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: ProxyBypassList
  - Beispielwert:
``` xml
<string>https://www.contoso.com, https://www.fabrikam.com</string>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### ProxyMode
  #### Proxyservereinstellungen konfigurieren
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Gibt die Proxy-Server-Einstellungen an, die von Microsoft Edge verwendet werden. Wenn Sie diese Richtlinie aktivieren, können Benutzer die Proxy-Einstellungen nicht ändern.

Wenn Sie sich dafür entscheiden, niemals einen Proxy-Server zu verwenden und sich immer direkt zu verbinden, werden alle anderen Optionen ignoriert.

Wenn Sie sich für die Verwendung von System-Proxy-Einstellungen entscheiden, werden alle anderen Optionen ignoriert.

Wenn Sie die automatische Erkennung des Proxy-Servers wählen, werden alle anderen Optionen ignoriert.

Wenn Sie den festen Server-Proxy-Modus wählen, können Sie weitere Optionen in [ProxyServer](#proxyserver) und 'Kommagetrennte Liste der Proxy-Bypassregeln' angeben.

Wenn Sie sich für die Verwendung eines PAC-Proxy-Skripts entscheiden, müssen Sie die URL zum Skript unter 'URL für eine proxy.pac-Datei' angeben.

Detaillierte Beispiele finden Sie unter [https://go.microsoft.com/fwlink/?linkid=2094936](https://go.microsoft.com/fwlink/?linkid=2094936)

Wenn Sie diese Richtlinie aktivieren, ignoriert Microsoft Edge alle proxybezogenen Optionen, die über die Befehlszeile angegeben werden.

Wenn Sie diese Richtlinie nicht konfigurieren, können Benutzer ihre eigenen Proxy-Einstellungen auswählen.

* "direct" = Niemals einen Proxy verwenden

* "auto_detect" = Proxy-Einstellungen automatisch erkennen

* "pac_script" = PAC-Proxy-Skript verwenden

* "fixed_servers" = Feste Proxy-Server verwenden

* "system" = System-Proxy-Einstellungen verwenden

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Zeichenfolge

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: ProxyMode
  - Gruppenrichtlinienname: Proxyservereinstellungen konfigurieren
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/Proxyserver
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: ProxyMode
  - Werttyp: REG_SZ
  ##### Beispielwert:
```
"direct"
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: ProxyMode
  - Beispielwert:
``` xml
<string>direct</string>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### ProxyPacUrl
  #### Proxy-PAC-Datei-URL festlegen
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Gibt die URL für eine PAC-Datei (Proxy Auto-Config) an.

Diese Richtlinie wird nur angewendet, wenn Sie 'Ein PAC-Proxyskript verwenden' in der Richtlinie [ProxyMode](#proxymode) verwenden. Wenn Sie einen anderen Modus für die Konfiguration von Proxy-Richtlinien ausgewählt haben, aktivieren oder konfigurieren Sie diese Richtlinie nicht.

Wenn Sie diese Richtlinie aktivieren, können Sie die URL für eine PAC-Datei angeben, die definiert, wie der Browser automatisch den geeigneten Proxy-Server für den Abruf einer bestimmten Website auswählt.

Wenn Sie diese Richtlinie deaktivieren oder nicht konfigurieren, wird keine PAC-Datei angegeben. Konfigurieren Sie diese Richtlinie nicht, wenn Sie eine andere Methode zum Festlegen von Proxy-Richtlinien angegeben haben.

Detaillierte Beispiele finden Sie unter [https://go.microsoft.com/fwlink/?linkid=2094936](https://go.microsoft.com/fwlink/?linkid=2094936).

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Zeichenfolge

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: ProxyPacUrl
  - Gruppenrichtlinienname: Proxy-PAC-Datei-URL festlegen
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/Proxyserver
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: ProxyPacUrl
  - Werttyp: REG_SZ
  ##### Beispielwert:
```
"https://internal.contoso.com/example.pac"
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: ProxyPacUrl
  - Beispielwert:
``` xml
<string>https://internal.contoso.com/example.pac</string>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### ProxyServer
  #### Adresse oder URL des Proxyservers konfigurieren
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Gibt die URL für den Proxy-Server an.

Diese Richtlinie wird nur angewendet, wenn Sie 'Feste Proxy-Server verwenden' [ProxyMode](#proxymode) verwenden. Wenn Sie einen anderen Modus für die Konfiguration von Proxy-Richtlinien ausgewählt haben, aktivieren oder konfigurieren Sie diese Richtlinie nicht.

Wenn Sie diese Richtlinie aktivieren, wird der durch diese Richtlinie konfigurierte Proxy-Server für alle URLs verwendet.

Wenn Sie diese Richtlinie deaktivieren oder nicht konfigurieren, können Benutzer in diesem Proxy-Modus ihre eigenen Proxy-Einstellungen wählen. Konfigurieren Sie diese Richtlinie nicht, wenn Sie eine andere Methode zum Festlegen von Proxy-Richtlinien angegeben haben.

Weitere Optionen und detaillierte Beispiele finden Sie unter [https://go.microsoft.com/fwlink/?linkid=2094936](https://go.microsoft.com/fwlink/?linkid=2094936).

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Zeichenfolge

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: ProxyServer
  - Gruppenrichtlinienname: Adresse oder URL des Proxyservers konfigurieren
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/Proxyserver
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: ProxyServer
  - Werttyp: REG_SZ
  ##### Beispielwert:
```
"123.123.123.123:8080"
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: ProxyServer
  - Beispielwert:
``` xml
<string>123.123.123.123:8080</string>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### ProxySettings
  #### Proxyeinstellungen
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Konfiguriert die Proxy-Einstellungen für Microsoft Edge.

Wenn Sie diese Richtlinie aktivieren, ignoriert Microsoft Edge alle proxybezogenen Optionen, die über die Befehlszeile angegeben werden.

Wenn Sie diese Richtlinie nicht konfigurieren, können Benutzer ihre eigenen Proxy-Einstellungen auswählen.

Diese Richtlinie hat Vorrang vor den folgenden Einzelrichtlinien:

[ProxyMode](#proxymode)
[ProxyPacUrl](#proxypacurl)
[ProxyServer](#proxyserver)
[ProxyBypassList](#proxybypasslist)

Im Feld ProxyMode können Sie den Proxy-Server angeben, der von Microsoft Edge verwendet wird, und verhindern, dass Benutzer Proxy-Einstellungen ändern.

Das Feld ProxyPacUrl enthält eine URL zu einer Proxy-PAC-Datei.

Das Feld ProxyServer enthält eine URL für den Proxy-Server.

Das Feld ProxyBypassList enthält eine Liste mit Proxy-Host, die Microsoft Edge umgeht.

Wenn Sie den Wert' direct' für 'ProxyMode' wählen, wird kein Proxy verwendet, und alle anderen Felder werden ignoriert.

Wenn Sie den Wert 'system' für 'ProxyMode' wählen, wird der Proxy des Systems verwendet, und alle anderen Felder werden ignoriert.

Wenn Sie den Wert 'auto_detect' für 'ProxyMode' wählen, werden alle anderen Felder ignoriert.

Wenn Sie den Wert 'fixed_server' für 'ProxyMode' wählen, werden die Felder 'ProxyServer' und ProxyBypassList' verwendet.

Wenn Sie den Wert 'pac_script' als 'ProxyMode' wählen, werden die Felder ProxyPacUrl' und ProxyBypassList' verwendet.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Wörterbuch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: ProxySettings
  - Gruppenrichtlinienname: Proxyeinstellungen
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/Proxyserver
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: ProxySettings
  - Werttyp: REG_SZ
  ##### Beispielwert:
```
SOFTWARE\Policies\Microsoft\Edge\ProxySettings = {
  "ProxyBypassList": "https://www.example1.com,https://www.example2.com,https://internalsite/", 
  "ProxyMode": "direct", 
  "ProxyPacUrl": "https://internal.site/example.pac", 
  "ProxyServer": "123.123.123.123:8080"
}
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: ProxySettings
  - Beispielwert:
``` xml
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
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ## SmartScreen-Einstellungen policies

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### PreventSmartScreenPromptOverride
  #### Umgehung der Microsoft Defender SmartScreen-Aufforderungen für Websites verhindern
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  This policy setting lets you decide whether users can override the Microsoft Defender SmartScreen warnings about potentially malicious websites.

If you enable this setting, users can't ignore Microsoft Defender SmartScreen warnings and they are blocked from continuing to the site.

If you disable or don't configure this setting, users can ignore Microsoft Defender SmartScreen warnings and continue to the site.

This policy is available only on Windows instances that are joined to a Microsoft Active Directory domain; or on Windows 10 Pro or Enterprise instances that are enrolled for device management.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Boolesch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: PreventSmartScreenPromptOverride
  - Gruppenrichtlinienname: Umgehung der Microsoft Defender SmartScreen-Aufforderungen für Websites verhindern
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/SmartScreen-Einstellungen
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: PreventSmartScreenPromptOverride
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000001
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: PreventSmartScreenPromptOverride
  - Beispielwert:
``` xml
<true/>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### PreventSmartScreenPromptOverrideForFiles
  #### Umgehung der Microsoft Defender SmartScreen-Warnungen für Downloads verhindern
  >Unterstützte Versionen: Microsoft Edge unter Windows seit Version 77 oder höher und unter Mac seit Version 79 oder höher

  #### Beschreibung
  This policy lets you determine whether users can override Microsoft Defender SmartScreen warnings about unverified downloads.

If you enable this policy, users in your organization can't ignore Microsoft Defender SmartScreen warnings, and they're prevented from completing the unverified downloads.

If you disable or don't configure this policy, users can ignore Microsoft Defender SmartScreen warnings and complete unverified downloads.

This policy is available only on Windows instances that are joined to a Microsoft Active Directory domain; or on Windows 10 Pro or Enterprise instances that are enrolled for device management.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Boolesch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: PreventSmartScreenPromptOverrideForFiles
  - Gruppenrichtlinienname: Umgehung der Microsoft Defender SmartScreen-Warnungen für Downloads verhindern
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/SmartScreen-Einstellungen
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: PreventSmartScreenPromptOverrideForFiles
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000001
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: PreventSmartScreenPromptOverrideForFiles
  - Beispielwert:
``` xml
<true/>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### SmartScreenAllowListDomains
  #### Konfigurieren Sie die Liste der Domänen, für die Microsoft Defender SmartScreen keine Warnungen auslöst.
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Configure the list of Microsoft Defender SmartScreen trusted domains. This means:
Microsoft Defender SmartScreen won't check for potentially malicious resources like phishing software and other malware if the source URLs match these domains.
The Microsoft Defender SmartScreen download protection service won't check downloads hosted on these domains.

If you enable this policy, Microsoft Defender SmartScreen trusts these domains.
If you disable or don't set this policy, default Microsoft Defender SmartScreen protection is applied to all resources.

This policy is available only on Windows instances that are joined to a Microsoft Active Directory domain; or on Windows 10 Pro or Enterprise instances that are enrolled for device management.
Also note that this policy does not apply if your organization has enabled Microsoft Defender Advanced Threat Protection. You must configure your allow and block lists in Microsoft Defender Security Center instead.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Liste der Zeichenfolgen

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: SmartScreenAllowListDomains
  - Gruppenrichtlinienname: Konfigurieren Sie die Liste der Domänen, für die Microsoft Defender SmartScreen keine Warnungen auslöst.
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/SmartScreen-Einstellungen
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge\SmartScreenAllowListDomains
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: 1, 2, 3, ...
  - Werttyp: Liste von REG_SZ
  ##### Beispielwert:
```
SOFTWARE\Policies\Microsoft\Edge\SmartScreenAllowListDomains\0 = "mydomain.com"
SOFTWARE\Policies\Microsoft\Edge\SmartScreenAllowListDomains\1 = "myuniversity.edu"

```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: SmartScreenAllowListDomains
  - Beispielwert:
``` xml
<array>
  <string>mydomain.com</string>
  <string>myuniversity.edu</string>
</array>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### SmartScreenEnabled
  #### Microsoft Defender SmartScreen konfigurieren
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Mit dieser Richtlinieneinstellung können Sie festlegen, ob Microsoft Defender SmartScreen aktiviert werden soll. Microsoft Defender SmartScreen gibt Warnmeldungen aus, um Ihre Benutzer vor potenziellen Phishing-Versuchen und vor potenzieller Schadsoftware zu schützen. Standardmäßig ist Microsoft Defender SmartScreen aktiviert.

Wenn Sie diese Einstellung aktivieren, wird Microsoft Defender SmartScreen aktiviert.

Wenn Sie diese Einstellung deaktivieren, wird Microsoft Defender SmartScreen deaktiviert.

Wenn Sie diese Einstellung nicht konfigurieren, können Benutzer entscheiden, ob sie Microsoft Defender SmartScreen verwenden möchten.

Diese Richtlinie ist nur für Windows-Instanzen verfügbar, die mit einer Microsoft Active Directory-Domäne verbunden sind, oder für Windows 10 Pro- oder Enterprise-Instanzen, die für die Geräteverwaltung registriert sind.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Ja
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Boolesch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: SmartScreenEnabled
  - Gruppenrichtlinienname: Microsoft Defender SmartScreen konfigurieren
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/SmartScreen-Einstellungen
  - Gruppenrichtlinienpfad (Empfohlen): Administrative Vorlagen/Microsoft Edge - Standardeinstellungen (können durch Benutzer überschrieben werden)/SmartScreen-Einstellungen
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): SOFTWARE\Policies\Microsoft\Edge\Empfohlen
  - Wertname: SmartScreenEnabled
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000001
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: SmartScreenEnabled
  - Beispielwert:
``` xml
<true/>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### SmartScreenForTrustedDownloadsEnabled
  #### Überprüfung von Downloads von vertrauenswürdigen Quellen durch Microsoft Defender SmartScreen erzwingen
  >Unterstützte Versionen: Microsoft Edge unter Windows seit Version 78 oder höher

  #### Beschreibung
  Mit dieser Richtlinieneinstellung können Sie konfigurieren, ob Microsoft Defender SmartScreen die Downloadzuverlässigkeit von einer vertrauenswürdigen Quelle überprüft.

Wenn Sie diese Einstellung aktivieren oder nicht konfigurieren, überprüft Microsoft Defender SmartScreen die Downloadzuverlässigkeit unabhängig von der Quelle.

Wenn Sie diese Einstellung deaktivieren, überprüft Microsoft Defender SmartScreen die Downloadzuverlässigkeit beim Herunterladen von einer zuverlässigen Quelle nicht.

Diese Richtlinie ist nur für Windows-Instanzen verfügbar, die einer Microsoft Active Directory-Domäne angehören, oder auf Windows 10 Pro oder Unternehmensinstanzen, die für die Geräteverwaltung registriert sind.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Ja
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Boolesch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: SmartScreenForTrustedDownloadsEnabled
  - Gruppenrichtlinienname: Überprüfung von Downloads von vertrauenswürdigen Quellen durch Microsoft Defender SmartScreen erzwingen
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/SmartScreen-Einstellungen
  - Gruppenrichtlinienpfad (Empfohlen): Administrative Vorlagen/Microsoft Edge - Standardeinstellungen (können durch Benutzer überschrieben werden)/SmartScreen-Einstellungen
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): SOFTWARE\Policies\Microsoft\Edge\Empfohlen
  - Wertname: SmartScreenForTrustedDownloadsEnabled
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000000
```


  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### SmartScreenPuaEnabled
  #### Microsoft Defender SmartScreen konfigurieren, um potenziell unerwünschte Apps zu blockieren
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 80 oder höher

  #### Beschreibung
  Mit dieser Richtlinieneinstellung können Sie konfigurieren, ob die Blockierung potenziell unerwünschter Apps in Microsoft Defender SmartScreen aktiviert werden soll. Die Blockierung potenziell unerwünschter Apps in Microsoft Defender SmartScreen schützt Benutzer mithilfe von Warnmeldungen vor Adware, Coin Mining, Bundleware und anderen fragwürdigen Apps, die von Websites gehostet werden. Die Blockierung potenziell unerwünschter Apps in Microsoft Defender SmartScreen ist standardmäßig deaktiviert.

Wenn Sie diese Einstellung aktivieren, wird die Blockierung potenziell unerwünschter Apps in Microsoft Defender SmartScreen aktiviert.

Wenn Sie diese Einstellung deaktivieren, wird die Blockierung potenziell unerwünschter Apps in Microsoft Defender SmartScreen deaktiviert.

Wenn Sie diese Einstellung nicht konfigurieren, können Benutzer wählen, ob Sie die Blockierung potenziell unerwünschter Apps in Microsoft Defender SmartScreen verwenden möchten.

Diese Richtlinie ist nur für Windows-Instanzen verfügbar, die mit einer Microsoft Active Directory-Domäne verbunden sind, oder für Windows 10 Pro- oder Enterprise-Instanzen, die für die Geräteverwaltung registriert sind.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Ja
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Boolesch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: SmartScreenPuaEnabled
  - Gruppenrichtlinienname: Microsoft Defender SmartScreen konfigurieren, um potenziell unerwünschte Apps zu blockieren
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/SmartScreen-Einstellungen
  - Gruppenrichtlinienpfad (Empfohlen): Administrative Vorlagen/Microsoft Edge - Standardeinstellungen (können durch Benutzer überschrieben werden)/SmartScreen-Einstellungen
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): SOFTWARE\Policies\Microsoft\Edge\Empfohlen
  - Wertname: SmartScreenPuaEnabled
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000001
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: SmartScreenPuaEnabled
  - Beispielwert:
``` xml
<true/>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ## Standardsuchanbieter policies

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### DefaultSearchProviderEnabled
  #### Standardsuchanbieter aktivieren
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Ermöglicht die Verwendung eines Standardsuchanbieters.

Wenn Sie diese Richtlinie aktivieren, kann ein Benutzer nach einem Begriff suchen, indem er ihn auf der Adressleiste eingibt (vorausgesetzt, bei der Eingabe handelt es sich nicht um eine URL).

Sie können den zu verwendenden Standardsuchanbieter angeben, indem Sie die restlichen Standardsuchrichtlinien aktivieren. Wenn Sie diese leer lassen (also nicht konfigurieren), kann der Benutzer den Standardanbieter auswählen.

Wenn Sie diese Richtlinie deaktivieren, kann der Benutzer nicht über die Adressleiste suchen.

Wenn Sie diese Richtlinie aktivieren oder deaktivieren, kann sie von Benutzern nicht geändert oder überschrieben werden.

Wenn Sie diese Richtlinie nicht konfigurieren, wird der Standardsuchanbieter aktiviert, und der Benutzer kann den Standardsuchanbieter auswählen und die Suchanbieterliste festlegen.

Diese Richtlinie ist nur in Windows-Instanzen verfügbar, die einer Microsoft Active Directory-Domäne angehören, oder in Windows 10 Pro- oder Enterprise-Instanzen, die für die Geräteverwaltung registriert sind.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Boolesch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: DefaultSearchProviderEnabled
  - Gruppenrichtlinienname: Standardsuchanbieter aktivieren
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/Standardsuchanbieter
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: DefaultSearchProviderEnabled
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000001
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: DefaultSearchProviderEnabled
  - Beispielwert:
``` xml
<true/>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### DefaultSearchProviderEncodings
  #### Standardsuchanbieter-Codierungen
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Gibt die vom Suchanbieter unterstützten Zeichenkodierungen an. Kodierungen sind Codepage-Namen wie UTF-8, GB2312 und ISO-8859-1. Sie werden in der angegebenen Reihenfolge ausprobiert.

Diese Richtlinie ist optional. Ist sie nicht konfiguriert, wird der Standard UTF-8 verwendet.

Diese Richtlinie wird nur angewendet, wenn Sie die Richtlinien [DefaultSearchProviderEnabled](#defaultsearchproviderenabled) und [DefaultSearchProviderSearchURL](#defaultsearchprovidersearchurl) aktivieren.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Liste der Zeichenfolgen

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: DefaultSearchProviderEncodings
  - Gruppenrichtlinienname: Standardsuchanbieter-Codierungen
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/Standardsuchanbieter
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge\DefaultSearchProviderEncodings
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: 1, 2, 3, ...
  - Werttyp: Liste von REG_SZ
  ##### Beispielwert:
```
SOFTWARE\Policies\Microsoft\Edge\DefaultSearchProviderEncodings\0 = "UTF-8"
SOFTWARE\Policies\Microsoft\Edge\DefaultSearchProviderEncodings\1 = "UTF-16"
SOFTWARE\Policies\Microsoft\Edge\DefaultSearchProviderEncodings\2 = "GB2312"
SOFTWARE\Policies\Microsoft\Edge\DefaultSearchProviderEncodings\3 = "ISO-8859-1"

```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: DefaultSearchProviderEncodings
  - Beispielwert:
``` xml
<array>
  <string>UTF-8</string>
  <string>UTF-16</string>
  <string>GB2312</string>
  <string>ISO-8859-1</string>
</array>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### DefaultSearchProviderImageURL
  #### Gibt das Bildsuchfeature für den standardmäßigen Suchanbieter an
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Gibt die URL der Suchmaschine an, die für die Bildsuche verwendet wird. Suchanfragen werden mit der Methode GET gesendet.

Diese Richtlinie ist optional. Wenn Sie es nicht konfigurieren, ist die Bildsuche nicht verfügbar.

Geben Sie die URL der Bing-Bildsuche wie folgt an:
'{bing:baseURL}images/detail/search?iss=sbiupload&FORM=ANCMS1#enterInsights'.

Geben Sie die URL der Google-Bildsuche wie folgt an: '{google:baseURL}searchbyimage/upload'.

In der Richtlinie [DefaultSearchProviderImageURLPostParams](#defaultsearchproviderimageurlpostparams) finden Sie Informationen zum Konfigurieren der Bildsuche.

Diese Richtlinie wird nur angewendet, wenn Sie die Richtlinien [DefaultSearchProviderEnabled](#defaultsearchproviderenabled) und [DefaultSearchProviderSearchURL](#defaultsearchprovidersearchurl) aktivieren.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Zeichenfolge

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: DefaultSearchProviderImageURL
  - Gruppenrichtlinienname: Gibt das Bildsuchfeature für den standardmäßigen Suchanbieter an
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/Standardsuchanbieter
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: DefaultSearchProviderImageURL
  - Werttyp: REG_SZ
  ##### Beispielwert:
```
"https://search.contoso.com/searchbyimage/upload"
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: DefaultSearchProviderImageURL
  - Beispielwert:
``` xml
<string>https://search.contoso.com/searchbyimage/upload</string>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### DefaultSearchProviderImageURLPostParams
  #### Parameter für eine Bild-URL, die POST verwendet
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Wenn Sie diese Richtlinie aktivieren, werden die Parameter angegeben, die bei der Durchführung einer Bildsuche mit POST verwendet werden. Die Richtlinie besteht aus kommagetrennten Name/Wertpaaren. Wenn ein Wert ein Vorlagenparameter ist, wie im vorherigen Beispiel {imageThumbnail}, wird er durch echte Miniaturbilddaten ersetzt. Diese Richtlinie wird nur angewendet, wenn Sie die Richtlinien [DefaultSearchProviderEnabled](#defaultsearchproviderenabled) und [DefaultSearchProviderSearchURL](#defaultsearchprovidersearchurl) aktivieren.

Geben Sie die URL-Postparameter für die Bildsuche von Bing an als:
'imageBin={google:imageThumbnailBase64}'.

Geben Sie die URL-Postparameter für die Bildsuche von Google an als:
'encoded_image={google:imageThumbnail},image_url={google:imageURL},sbisrc={google:imageSearchSource},original_width={google:imageOriginalWidth},original_height={google:imageOriginalHeight}'.

If you don’t set this policy, image search requests are sent using the GET method.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Zeichenfolge

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: DefaultSearchProviderImageURLPostParams
  - Gruppenrichtlinienname: Parameter für eine Bild-URL, die POST verwendet
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/Standardsuchanbieter
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: DefaultSearchProviderImageURLPostParams
  - Werttyp: REG_SZ
  ##### Beispielwert:
```
"content={imageThumbnail},url={imageURL},sbisrc={SearchSource}"
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: DefaultSearchProviderImageURLPostParams
  - Beispielwert:
``` xml
<string>content={imageThumbnail},url={imageURL},sbisrc={SearchSource}</string>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### DefaultSearchProviderKeyword
  #### Stichwort für Standardsuchanbieter
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Gibt das Schlüsselwort an, das die Verknüpfung in der Adressleiste ist, mit der die Suche nach diesem Anbieter ausgelöst wird.

Diese Richtlinie ist optional. Wird sie nicht konfiguriert, aktiviert kein Schlüsselwort den Suchanbieter.

Diese Richtlinie wird nur angewendet, wenn Sie die Richtlinien [DefaultSearchProviderEnabled](#defaultsearchproviderenabled) und [DefaultSearchProviderSearchURL](#defaultsearchprovidersearchurl) aktivieren.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Zeichenfolge

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: DefaultSearchProviderKeyword
  - Gruppenrichtlinienname: Stichwort für Standardsuchanbieter
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/Standardsuchanbieter
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: DefaultSearchProviderKeyword
  - Werttyp: REG_SZ
  ##### Beispielwert:
```
"mis"
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: DefaultSearchProviderKeyword
  - Beispielwert:
``` xml
<string>mis</string>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### DefaultSearchProviderName
  #### Standardsuchanbietername
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Gibt den Namen des Standardsuchanbieters an.

Wenn Sie diese Richtlinie aktivieren, legen Sie den Namen des Standardsuchanbieters fest.

Wenn Sie diese Richtlinie nicht aktivieren oder leer lassen, wird der in der Such-URL angegebene Hostname verwendet.

'DefaultSearchProviderName' sollte auf einen vom Unternehmen zugelassenen verschlüsselten Suchanbieter festgelegt sein, der dem in DTBC-0008 eingestellten verschlüsselten Suchanbieter entspricht. Diese Richtlinie wird nur angewendet, wenn Sie die Richtlinien [DefaultSearchProviderEnabled](#defaultsearchproviderenabled) und [DefaultSearchProviderSearchURL](#defaultsearchprovidersearchurl) aktivieren.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Zeichenfolge

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: DefaultSearchProviderName
  - Gruppenrichtlinienname: Standardsuchanbietername
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/Standardsuchanbieter
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: DefaultSearchProviderName
  - Werttyp: REG_SZ
  ##### Beispielwert:
```
"My Intranet Search"
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: DefaultSearchProviderName
  - Beispielwert:
``` xml
<string>My Intranet Search</string>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### DefaultSearchProviderSearchURL
  #### Such-URL für den Standardsuchanbieter
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Gibt die URL der Suchmaschine an, die für eine Standardsuche verwendet wird. Die URL enthält die Zeichenkette'{searchTerms}'', die bei der Abfrage durch die Begriffe ersetzt wird, nach denen der Benutzer sucht.

Geben Sie die Such-URL von Bing an als:

'{bing:baseURL}search?q={searchTerms}'.

Geben Sie die Such-URL von Google an als:: '{google:baseURL}search?q={searchTerms}&{google:RLZ}{google:originalQueryForSuggestion}{google:assistedQueryStats}{google:searchFieldtrialParameter}{google:searchClient}{google:sourceId}ie={inputEncoding}'.

Diese Richtlinie ist erforderlich, wenn Sie die Richtlinie [DefaultSearchProviderEnabled](#defaultsearchproviderenabled) aktivieren. Wenn Sie diese Richtlinie nicht aktivieren, wird sie ignoriert.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Zeichenfolge

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: DefaultSearchProviderSearchURL
  - Gruppenrichtlinienname: Such-URL für den Standardsuchanbieter
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/Standardsuchanbieter
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: DefaultSearchProviderSearchURL
  - Werttyp: REG_SZ
  ##### Beispielwert:
```
"https://search.contoso.com/search?q={searchTerms}"
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: DefaultSearchProviderSearchURL
  - Beispielwert:
``` xml
<string>https://search.contoso.com/search?q={searchTerms}</string>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### DefaultSearchProviderSuggestURL
  #### Standard-Suchanbieter-URL für Vorschläge
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Gibt die URL für die Suchmaschine an, die verwendet wird, um Suchvorschläge bereitzustellen. Die URL enthält die Zeichenfolge '{searchTerms}', die zur Abfragezeit durch den bisher vom Benutzer eingegebenen Text ersetzt wird.

Diese Richtlinie ist optional. Wird sie nicht konfiguriert, werden den Benutzern keine Suchvorschläge angezeigt, sondern Vorschläge aus ihrem Browserverlauf und ihren Favoriten.

Die von Bing vorgeschlagene URL kann wie folgt angegeben werden:

'{bing:baseURL}qbox?query={searchTerms}'.

Die von Google vorgeschlagene URL kann wie folgt angegeben werden: '{google:baseURL}complete/search?output=chrome&q={searchTerms}'.

Diese Richtlinie wird nur angewendet, wenn Sie die Richtlinien [DefaultSearchProviderEnabled](#defaultsearchproviderenabled) und [DefaultSearchProviderSearchURL](#defaultsearchprovidersearchurl) aktivieren.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Zeichenfolge

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: DefaultSearchProviderSuggestURL
  - Gruppenrichtlinienname: Standard-Suchanbieter-URL für Vorschläge
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/Standardsuchanbieter
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: DefaultSearchProviderSuggestURL
  - Werttyp: REG_SZ
  ##### Beispielwert:
```
"https://search.contoso.com/suggest?q={searchTerms}"
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: DefaultSearchProviderSuggestURL
  - Beispielwert:
``` xml
<string>https://search.contoso.com/suggest?q={searchTerms}</string>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ## Start&comma; Startseite und neue Tabseite policies

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### HomepageIsNewTabPage
  #### Neue Tabseite als Startseite festlegen
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Konfiguriert die Standard-Startseite in Microsoft Edge. Sie können die Startseite auf eine von Ihnen angegebene URL festlegen oder auf "Neue Tabseite".

Wenn Sie diese Richtlinie aktivieren, wird die Seite „Neue Tab“ immer als Startseite verwendet, und der URL-Pfad der Startseite wird ignoriert.

Wenn Sie diese Richtlinie deaktivieren, kann die Startseite des Benutzers nicht die Seite „Neue Tab“ sein, es sei denn, die URL ist auf „edge://newtab“ festgelegt.

Wenn nicht konfiguriert, können Benutzer auswählen, ob die Seite „Neue Tab“ ihre Startseite sein soll.

Diese Richtlinie ist nur für Windows-Instanzen verfügbar, die mit einer Microsoft Active Directory-Domäne oder mit Windows 10 Pro- oder Enterprise-Instanzen verbunden sind, die für die Geräteverwaltung registriert sind.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Ja
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Boolesch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: HomepageIsNewTabPage
  - Gruppenrichtlinienname: Neue Tabseite als Startseite festlegen
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/Start, Startseite und neue Tabseite
  - Gruppenrichtlinienpfad (Empfohlen): Administrative Vorlagen/Microsoft Edge - Standardeinstellungen (können durch Benutzer überschrieben werden)/Start, Startseite und neue Tabseite
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): SOFTWARE\Policies\Microsoft\Edge\Empfohlen
  - Wertname: HomepageIsNewTabPage
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000001
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: HomepageIsNewTabPage
  - Beispielwert:
``` xml
<true/>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### HomepageLocation
  #### Homepage-URL konfigurieren
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Konfiguriert die standardmäßige URL der Homepage in Microsoft Edge.

Die Startseite ist die Seite, die durch die gleichnamige Schaltfläche geöffnet wird. Die Seiten, die sich beim Start öffnen, werden durch die Richtlinien [RestoreOnStartup](#restoreonstartup) gesteuert.

Sie können entweder eine URL hier eingeben oder die Startseite so einstellen, dass der neue Tab geöffnet wird. Wenn Sie die zweite Möglichkeit wählen, wird diese Richtlinie nicht wirksam.

Wenn Sie diese Richtlinie aktivieren, können Benutzer ihre Homepage-URL nicht ändern, aber sie können den neuen Tab als Startseite verwenden.

Wenn Sie diese Richtlinie deaktivieren oder nicht konfigurieren, können Benutzer ihre eigene Homepage wählen, solange die Richtlinie [HomepageIsNewTabPage](#homepageisnewtabpage) nicht aktiviert ist.

Diese Richtlinie ist nur auf Windows-Instanzen verfügbar, die zu einer Microsoft Active Directory-Domäne gehören, und für Windows 10 Pro- oder Enterprise-Instanzen, die für die Geräteverwaltung angemeldet sind.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Ja
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Zeichenfolge

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: HomepageLocation
  - Gruppenrichtlinienname: Homepage-URL konfigurieren
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/Start, Startseite und neue Tabseite
  - Gruppenrichtlinienpfad (Empfohlen): Administrative Vorlagen/Microsoft Edge - Standardeinstellungen (können durch Benutzer überschrieben werden)/Start, Startseite und neue Tabseite
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): SOFTWARE\Policies\Microsoft\Edge\Empfohlen
  - Wertname: HomepageLocation
  - Werttyp: REG_SZ
  ##### Beispielwert:
```
"https://www.contoso.com"
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: HomepageLocation
  - Beispielwert:
``` xml
<string>https://www.contoso.com</string>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### NewTabPageCompanyLogo
  #### Neues Firmenlogo auf der Registerkartenseite festlegen
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 79 oder höher

  #### Beschreibung
  Specifies the company logo to use on the new tab page in Microsoft Edge.

The policy should be configured as a string that expresses the logo(s) in JSON format. For example: { "default_logo": { "url": "https://www.contoso.com/logo.png", "hash": "cd0aa9856147b6c5b4ff2b7dfee5da20aa38253099ef1b4a64aced233c9afe29" }, "light_logo": { "url": "https://www.contoso.com/light_logo.png", "hash": "517d286edb416bb2625ccfcba9de78296e90da8e32330d4c9c8275c4c1c33737" } }

You configure this policy by specifying the URL from which Microsoft Edge can download the logo and its cryptographic hash (SHA-256), which is used to verify the integrity of the download. The logo must be in PNG or SVG format, and its file size must not exceed 16 MB. The logo is downloaded and cached, and it will be redownloaded whenever the URL or the hash changes. The URL must be accessible without any authentication.

The 'default_logo' is required and will be used when there's no background image. If 'light_logo' is provided, it will be used when the user's new tab page has a background image. We recommend a horizontal logo with a transparent background that is left-aligned and vertically centered. The logo should have a minimum height of 32 pixels and an aspect ratio from 1:1 to 4:1. The 'default_logo' should have proper contrast against a white/black background while the 'light_logo' should have proper contrast against a background image.

If you enable this policy, Microsoft Edge downloads and shows the specified logo(s) on the new tab page. Users can't override or hide the logo(s).

If you disable or don't configure this policy, Microsoft Edge will show no company logo or a Microsoft logo on the new tab page.

For help with determining the SHA-256 hash, see https://docs.microsoft.com/powershell/module/microsoft.powershell.utility/get-filehash.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Nein - Erfordert einen Neustart des Browsers

  #### Datentyp:
  Wörterbuch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: NewTabPageCompanyLogo
  - Gruppenrichtlinienname: Neues Firmenlogo auf der Registerkartenseite festlegen
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/Start, Startseite und neue Tabseite
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: NewTabPageCompanyLogo
  - Werttyp: REG_SZ
  ##### Beispielwert:
```
SOFTWARE\Policies\Microsoft\Edge\NewTabPageCompanyLogo = {
  "default_logo": {
    "hash": "cd0aa9856147b6c5b4ff2b7dfee5da20aa38253099ef1b4a64aced233c9afe29", 
    "url": "https://www.contoso.com/logo.png"
  }, 
  "light_logo": {
    "hash": "517d286edb416bb2625ccfcba9de78296e90da8e32330d4c9c8275c4c1c33737", 
    "url": "https://www.contoso.com/light_logo.png"
  }
}
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: NewTabPageCompanyLogo
  - Beispielwert:
``` xml
<key>NewTabPageCompanyLogo</key>
<dict>
  <key>default_logo</key>
  <dict>
    <key>hash</key>
    <string>cd0aa9856147b6c5b4ff2b7dfee5da20aa38253099ef1b4a64aced233c9afe29</string>
    <key>url</key>
    <string>https://www.contoso.com/logo.png</string>
  </dict>
  <key>light_logo</key>
  <dict>
    <key>hash</key>
    <string>517d286edb416bb2625ccfcba9de78296e90da8e32330d4c9c8275c4c1c33737</string>
    <key>url</key>
    <string>https://www.contoso.com/light_logo.png</string>
  </dict>
</dict>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### NewTabPageHideDefaultTopSites
  #### Die Standardwebsites der obersten Ebene auf der neuen Tabseite ausblenden
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Blendet die Standardwebsites auf der Tabseite "Neu" in Microsoft Edge aus.

Wenn Sie diese Richtlinie auf "true" festlegen, werden die Standardkacheln der Website der obersten Ebene ausgeblendet.

Wenn Sie diese Richtlinie auf "false" festlegen oder nicht konfigurieren, bleiben die Standardkacheln für die Website der obersten Ebene sichtbar.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Boolesch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: NewTabPageHideDefaultTopSites
  - Gruppenrichtlinienname: Die Standardwebsites der obersten Ebene auf der neuen Tabseite ausblenden
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/Start, Startseite und neue Tabseite
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: NewTabPageHideDefaultTopSites
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000001
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: NewTabPageHideDefaultTopSites
  - Beispielwert:
``` xml
<true/>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### NewTabPageLocation
  #### URL für die neue Tabseite konfigurieren
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Konfiguriert die Standard-URL für den neuen Tab.

Diese Richtlinie bestimmt die Seite, die geöffnet wird, wenn neue Tabs erstellt werden (auch wenn neue Fenster geöffnet werden). Sie wirkt sich auch auf die Startseite aus, wenn diese auf dem neuen Tab geöffnet werden soll.

Diese Richtlinie bestimmt nicht, welche Seite beim Start geöffnet wird; das wird gesteuert durch die Richtlinie [RestoreOnStartup](#restoreonstartup). Sie wirkt sich auch nicht auf die Startseite aus, wenn diese auf dem neuen Tab geöffnet werden soll.

Wenn Sie diese Richtlinie nicht konfigurieren, wird der standardmäßige neue Tab verwendet.

Wenn Sie diese Richtlinie konfigurieren *und* die Richtlinie [NewTabPageSetFeedType](#newtabpagesetfeedtype), hat diese Richtlinie Vorrang.

Wenn eine ungültige URL angegeben ist, wird der neue Tab about://blank geöffnet.

Diese Richtlinie ist nur auf Windows-Instanzen verfügbar, die zu einer Microsoft Active Directory-Domäne gehören, und für Windows 10 Pro- oder Enterprise-Instanzen, die für die Geräteverwaltung angemeldet sind.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Ja
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Zeichenfolge

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: NewTabPageLocation
  - Gruppenrichtlinienname: URL für die neue Tabseite konfigurieren
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/Start, Startseite und neue Tabseite
  - Gruppenrichtlinienpfad (Empfohlen): Administrative Vorlagen/Microsoft Edge - Standardeinstellungen (können durch Benutzer überschrieben werden)/Start, Startseite und neue Tabseite
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): SOFTWARE\Policies\Microsoft\Edge\Empfohlen
  - Wertname: NewTabPageLocation
  - Werttyp: REG_SZ
  ##### Beispielwert:
```
"https://www.fabrikam.com"
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: NewTabPageLocation
  - Beispielwert:
``` xml
<string>https://www.fabrikam.com</string>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### NewTabPageManagedQuickLinks
  #### Schnelllinks für neue Tabs festlegen
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 79 oder höher

  #### Beschreibung
  Microsoft Edge zeigt auf der neuen Tabseite standardmäßig Quicklinks aus von Benutzern hinzugefügten Verknüpfungen und zu den beliebtesten Websites basierend auf dem Browserverlauf an. Mit dieser Richtlinie können Sie auf der neuen Tabseite bis zu drei Quicklink-Kacheln konfigurieren, die als JSON-Objekt ausgedrückt werden:

[ { "url": "https://www.contoso.com", "title": "Contoso Portal", "pinned": true/false }, ... ]

Das Feld „url“ ist erforderlich; „title“ und „pinned“ sind optional. Wenn „title“ nicht angegeben ist, wird die URL als Standardtitel verwendet. Wenn „pinned“ nicht angegeben wird, ist der Standardwert „false“.

Microsoft Edge stellt diese in der aufgelisteten Reihenfolge von links nach rechts dar, wobei alle angehefteten Kacheln vor nicht angehefteten Kacheln angezeigt werden.

Wenn die Richtlinie als obligatorisch festgelegt ist, wird das Feld „pinned“ ignoriert, und alle Kacheln werden angeheftet. Die Kacheln können vom Benutzer nicht gelöscht werden und werden immer am Anfang der Quicklinks-Liste angezeigt.

Wenn die Richtlinie als empfohlen festgelegt ist, bleiben angeheftete Kacheln in der Liste, aber der Benutzer hat die Möglichkeit, sie zu bearbeiten und zu löschen. Nicht angeheftete Quicklink-Kacheln verhalten sich wie Standardwebsites der obersten Ebene und werden von der Liste gestrichen, wenn andere Websites häufiger besucht werden. Beim Anwenden von nicht angehefteten Links über diese Richtlinie auf ein vorhandenes Browserprofil werden die Links u. U. überhaupt nicht angezeigt, je nachdem, wie sie im Vergleich zum Browserverlauf des Benutzers eingestuft werden.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Ja
  - Dynamische Richtlinienaktualisierung: Nein - Erfordert einen Neustart des Browsers

  #### Datentyp:
  Wörterbuch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: NewTabPageManagedQuickLinks
  - Gruppenrichtlinienname: Schnelllinks für neue Tabs festlegen
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/Start, Startseite und neue Tabseite
  - Gruppenrichtlinienpfad (Empfohlen): Administrative Vorlagen/Microsoft Edge - Standardeinstellungen (können durch Benutzer überschrieben werden)/Start, Startseite und neue Tabseite
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): SOFTWARE\Policies\Microsoft\Edge\Empfohlen
  - Wertname: NewTabPageManagedQuickLinks
  - Werttyp: REG_SZ
  ##### Beispielwert:
```
SOFTWARE\Policies\Microsoft\Edge\NewTabPageManagedQuickLinks = [
  {
    "pinned": true, 
    "title": "Contoso Portal", 
    "url": "https://contoso.com"
  }, 
  {
    "title": "Fabrikam", 
    "url": "https://fabrikam.com"
  }
]
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: NewTabPageManagedQuickLinks
  - Beispielwert:
``` xml
<key>NewTabPageManagedQuickLinks</key>
<array>
  <dict>
    <key>pinned</key>
    <true/>
    <key>title</key>
    <string>Contoso Portal</string>
    <key>url</key>
    <string>https://contoso.com</string>
  </dict>
  <dict>
    <key>title</key>
    <string>Fabrikam</string>
    <key>url</key>
    <string>https://fabrikam.com</string>
  </dict>
</array>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### NewTabPageSetFeedType
  #### Funktion für neue Tabseiten in Microsoft Edge konfigurieren
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 79 oder höher

  #### Beschreibung
  Gibt Ihnen die Möglichkeit, für die neue Tabseite zwischen Microsoft News- oder Office 365-Feed zu wählen.

Wenn Sie diese Richtlinie auf den Microsoft News-Feed festlegen (0), wird Benutzern auf der neuen Tabseite der Microsoft News-Feed angezeigt.

Wenn Sie diese Richtlinie auf den Office 365-Feed festlegen (1), wird Benutzern mit einer Azure Active Directory-Browseranmeldung der Office 365-Feed auf der neuen Tabseite angezeigt.

Wenn Sie diese Richtlinie deaktivieren oder nicht konfigurieren, gilt Folgendes:

- Benutzern mit Azure Active Directory-Browseranmeldung wird neben dem Standardfeed für neue Tabseiten auch der Office 365-Feed angeboten.

- Benutzern ohne Azure Active Directory-Browseranmeldung wird der Standardfeed für neue Tabseiten angezeigt.

Wenn Sie diese Richtlinie *und* die Richtlinie [NewTabPageLocation](#newtabpagelocation) konfigurieren, hat [NewTabPageLocation](#newtabpagelocation) Vorrang.

Standardeinstellung: Deaktiviert oder nicht konfiguriert.

* 0 = Microsoft News-Feed

* 1 = Office 365-Feed

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Ja
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Ganze Zahl

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: NewTabPageSetFeedType
  - Gruppenrichtlinienname: Funktion für neue Tabseiten in Microsoft Edge konfigurieren
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/Start, Startseite und neue Tabseite
  - Gruppenrichtlinienpfad (Empfohlen): Administrative Vorlagen/Microsoft Edge - Standardeinstellungen (können durch Benutzer überschrieben werden)/Start, Startseite und neue Tabseite
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): SOFTWARE\Policies\Microsoft\Edge\Empfohlen
  - Wertname: NewTabPageSetFeedType
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000000
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: NewTabPageSetFeedType
  - Beispielwert:
``` xml
<integer>0</integer>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### RestoreOnStartup
  #### Aktion, die beim Start ausgeführt werden soll
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Geben Sie an, wie sich Microsoft Edge beim Starten verhält.

Wenn Sie einen neuen Tab beim Start immer öffnen möchten, wählen Sie „Neuen Tab öffnen“ (5).

Wenn Sie URLs erneut öffnen möchten, die beim letzten Schließen von Microsoft Edge geöffnet waren, wählen Sie „Letzte Sitzung wiederherstellen“ (1). Die Browsersitzung wird so wiederhergestellt, wie sie war. Beachten Sie, dass diese Option einige Einstellungen deaktiviert, die auf Sitzungen basieren oder Aktionen beim Beenden ausführen (z. B. Löschen von Browserdaten beim Beenden oder von reinen Sitzungscookies).

Wenn Sie einen bestimmten Satz von URLs öffnen möchten, wählen Sie „Liste mit URLs öffnen“ (4).

Das Deaktivieren dieser Einstellung entspricht einer fehlenden Konfiguration. Die Benutzer können sie in Microsoft Edge ändern. Diese Richtlinie ist nur für Windows-Instanzen verfügbar, die mit einer Microsoft Active Directory-Domäne oder Windows 10 Pro- oder Enterprise-Instanz verbunden sind, die für die Geräteverwaltung registriert sind

* 5 = Neuen Tab öffnen

* 1 = Letzte Sitzung wiederherstellen

* 4 = Liste der URLs öffnen

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Ja
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Ganze Zahl

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: RestoreOnStartup
  - Gruppenrichtlinienname: Aktion, die beim Start ausgeführt werden soll
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/Start, Startseite und neue Tabseite
  - Gruppenrichtlinienpfad (Empfohlen): Administrative Vorlagen/Microsoft Edge - Standardeinstellungen (können durch Benutzer überschrieben werden)/Start, Startseite und neue Tabseite
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): SOFTWARE\Policies\Microsoft\Edge\Empfohlen
  - Wertname: RestoreOnStartup
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000004
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: RestoreOnStartup
  - Beispielwert:
``` xml
<integer>4</integer>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### RestoreOnStartupURLs
  #### Websites, die beim Start des Browsers geöffnet werden sollen
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Gibt eine Liste von Websites an, die beim Start des Browsers automatisch geöffnet werden sollen. Wenn Sie diese Richtlinie nicht konfigurieren, wird beim Start keine Website geöffnet.

Diese Richtlinie funktioniert nur, wenn Sie zudem die Richtlinie [RestoreOnStartup](#restoreonstartup) auf 'URL-Liste öffnen' (4) festlegen.

Diese Richtlinie ist nur für Windows-Instanzen verfügbar, die zu einer Microsoft Active Directory-Domäne gehören, oder für Windows 10 Pro- und Enterprise-Instanzen, die für die Geräteverwaltung registriert sind.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Ja
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Liste der Zeichenfolgen

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: RestoreOnStartupURLs
  - Gruppenrichtlinienname: Websites, die beim Start des Browsers geöffnet werden sollen
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/Start, Startseite und neue Tabseite
  - Gruppenrichtlinienpfad (Empfohlen): Administrative Vorlagen/Microsoft Edge - Standardeinstellungen (können durch Benutzer überschrieben werden)/Start, Startseite und neue Tabseite
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge\RestoreOnStartupURLs
  - Pfad (Empfohlen): SOFTWARE\Policies\Microsoft\Edge\Empfohlen\RestoreOnStartupURLs
  - Wertname: 1, 2, 3, ...
  - Werttyp: Liste von REG_SZ
  ##### Beispielwert:
```
SOFTWARE\Policies\Microsoft\Edge\RestoreOnStartupURLs\0 = "https://contoso.com"
SOFTWARE\Policies\Microsoft\Edge\RestoreOnStartupURLs\1 = "https://www.fabrikam.com"

```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: RestoreOnStartupURLs
  - Beispielwert:
``` xml
<array>
  <string>https://contoso.com</string>
  <string>https://www.fabrikam.com</string>
</array>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### ShowHomeButton
  #### Schaltfläche „Startseite“ auf Symbolleiste anzeigen
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Zeigt die Schaltfläche „Start“ auf der Microsoft Edge-Symbolleiste an.

Aktivieren Sie diese Richtlinie, um die Schaltfläche „Start“ immer anzuzeigen. Deaktivieren Sie diese Option, um die Schaltfläche nie anzuzeigen.

Wenn Sie die Richtlinie nicht konfigurieren, können Benutzer auswählen, ob die Schaltfläche „Start“ angezeigt werden soll.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Ja
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Boolesch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: ShowHomeButton
  - Gruppenrichtlinienname: Schaltfläche „Startseite“ auf Symbolleiste anzeigen
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/Start, Startseite und neue Tabseite
  - Gruppenrichtlinienpfad (Empfohlen): Administrative Vorlagen/Microsoft Edge - Standardeinstellungen (können durch Benutzer überschrieben werden)/Start, Startseite und neue Tabseite
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): SOFTWARE\Policies\Microsoft\Edge\Empfohlen
  - Wertname: ShowHomeButton
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000001
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: ShowHomeButton
  - Beispielwert:
``` xml
<true/>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ## Additional policies

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### AdsSettingForIntrusiveAdsSites
  #### Anzeigeneinstellung für Websites mit aufdringlichen Anzeigen
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 78 oder höher

  #### Beschreibung
  Steuert, ob Werbung mit aufdringlichen Werbeanzeigen blockiert wird. Sie können für diese Richtlinie eine der folgenden Optionen festlegen:

* 1 = Lässt Werbung für alle Websites zu

* 2 = Blockiert Werbung auf Websites mit aufdringlichen Werbeanzeigen (Standardwert)

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Ganze Zahl

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: AdsSettingForIntrusiveAdsSites
  - Gruppenrichtlinienname: Anzeigeneinstellung für Websites mit aufdringlichen Anzeigen
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: AdsSettingForIntrusiveAdsSites
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000001
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: AdsSettingForIntrusiveAdsSites
  - Beispielwert:
``` xml
<integer>1</integer>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### AllowDeletingBrowserHistory
  #### Löschen des Browser- und Downloadverlaufs ermöglichen
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Ermöglicht das Löschen des Browser- und Downloadverlaufs und verhindert, dass Benutzer diese Einstellung ändern.

Hinweis: Auch wenn diese Richtlinie deaktiviert ist, ist nicht garantiert, dass Browser- und Downloadverlauf gespeichert werden: Benutzer können die Verlaufsdatenbankdateien direkt bearbeiten oder löschen, und der Browser kann beliebige oder alle Verlaufselemente jederzeit entfernen (basierend auf der Ablauffrist) oder archivieren.

Wenn Sie diese Richtlinie aktivieren oder nicht konfigurieren, können Benutzer den Browser- und Downloadverlauf löschen.

Wenn Sie diese Richtlinie deaktivieren, können Benutzer den Browser- und Downloadverlauf nicht löschen.

Wenn Sie diese Richtlinie aktivieren, achten Sie darauf, dass die Richtlinie „Clear browsing data when Microsoft Edge closes“ (Browserdaten löschen, wenn Microsoft Edge geschlossen wird) nicht aktiviert ist, da beide dazu dienen, Daten zu löschen. Wenn Sie beide Richtlinien aktivieren, hat die Richtlinie „Clear browsing data when Microsoft Edge closes“ (Browserdaten löschen, wenn Microsoft Edge geschlossen wird) Vorrang und löscht alle Daten, wenn Microsoft Edge geschlossen wird (unabhängig von der Konfiguration dieser Richtlinie).

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Boolesch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: AllowDeletingBrowserHistory
  - Gruppenrichtlinienname: Löschen des Browser- und Downloadverlaufs ermöglichen
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: AllowDeletingBrowserHistory
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000001
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: AllowDeletingBrowserHistory
  - Beispielwert:
``` xml
<true/>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### AllowFileSelectionDialogs
  #### Dateiauswahl-Dialogfelder zulassen
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Lassen Sie den Zugriff auf lokale Dateien zu, indem Sie Microsoft Edge Dateiauswahl-Dialogfelder anzeigen lassen.

Wenn Sie diese Richtlinie aktivieren oder nicht konfigurieren, können Benutzer Dateiauswahl-Dialogfelder normal öffnen.

Wenn Sie diese Richtlinie deaktivieren, wird immer dann eine Meldung angezeigt, wenn der Benutzer eine Aktion ausführt, die ein Dateiauswahl-Dialogfeld auslöst (z. B. das Importieren von Favoriten, das Hochladen von Dateien oder das Speichern von links). Es wird angenommen, dass der Benutzer im Dateiauswahl-Dialogfeld auf „Abbrechen” geklickt hat.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Boolesch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: AllowFileSelectionDialogs
  - Gruppenrichtlinienname: Dateiauswahl-Dialogfelder zulassen
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: AllowFileSelectionDialogs
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000001
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: AllowFileSelectionDialogs
  - Beispielwert:
``` xml
<true/>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### AllowPopupsDuringPageUnload
  #### Erlaubt einer Seite, Popups während des Entladens zu zeigen
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 78 oder höher

  #### Beschreibung
  Mit dieser Richtlinie kann ein Administrator angeben, dass beim Entladen einer Seite Popups angezeigt werden können.

Wenn die Richtlinie auf „aktiviert“ festgelegt ist, können Seiten Popups anzeigen, während sie entladen werden.

Wenn die Richtlinie auf „deaktiviert“ festgelegt oder nicht festgelegt ist, dürfen Seiten keine Popups anzeigen, während sie entladen werden. Dies entspricht der folgenden Spezifikation: (https://html.spec.whatwg.org/#apis-for-creating-and-navigating-browsing-contexts-by-name).

Diese Richtlinie wird künftig entfernt.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Nein - Erfordert einen Neustart des Browsers

  #### Datentyp:
  Boolesch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: AllowPopupsDuringPageUnload
  - Gruppenrichtlinienname: Erlaubt einer Seite, Popups während des Entladens zu zeigen
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: AllowPopupsDuringPageUnload
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000000
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: AllowPopupsDuringPageUnload
  - Beispielwert:
``` xml
<false/>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### AllowSyncXHRInPageDismissal
  #### Zulassen, dass Seiten beim Schließen synchrone XHR-Anforderungen senden
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 79 oder höher

  #### Beschreibung
  Mit dieser Richtlinie können Sie angeben, dass eine Seite beim Schließen synchrone XHR-Anforderungen senden kann.

Wenn Sie diese Richtlinie aktivieren, können Seiten beim Schließen synchrone XHR-Anforderungen senden.

Wenn Sie diese Richtlinie deaktivieren oder nicht konfigurieren, dürfen Seiten beim Schließen keine synchronen XHR-Anforderungen senden.

Diese Richtlinie ist temporärer Art und wird in einer zukünftigen Version entfernt.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Nein - Erfordert einen Neustart des Browsers

  #### Datentyp:
  Boolesch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: AllowSyncXHRInPageDismissal
  - Gruppenrichtlinienname: Zulassen, dass Seiten beim Schließen synchrone XHR-Anforderungen senden
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: AllowSyncXHRInPageDismissal
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000000
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: AllowSyncXHRInPageDismissal
  - Beispielwert:
``` xml
<false/>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### AllowTrackingForUrls
  #### Konfigurieren von Ausnahmen für die Tracking-Verhinderung für bestimmte Sites
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 78 oder höher

  #### Beschreibung
  Konfigurieren Sie die Liste der URL-Muster, die von der nach Tracking-Verhinderung ausgeschlossen sind.

Wenn Sie diese Richtlinie konfigurieren, wird die Liste der konfigurierten URL-Muster von der nach Tracking-Verhinderung ausgeschlossen.

Wenn Sie diese Richtlinie nicht konfigurieren, wird der globale Standardwert aus der Richtlinie "Blockieren der Nachverfolgung der Webbrowsing-Aktivitäten von Benutzern" (falls festgelegt) oder die persönliche Konfiguration des Benutzers für alle Websites verwendet.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Liste der Zeichenfolgen

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: AllowTrackingForUrls
  - Gruppenrichtlinienname: Konfigurieren von Ausnahmen für die Tracking-Verhinderung für bestimmte Sites
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge\AllowTrackingForUrls
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: 1, 2, 3, ...
  - Werttyp: Liste von REG_SZ
  ##### Beispielwert:
```
SOFTWARE\Policies\Microsoft\Edge\AllowTrackingForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\AllowTrackingForUrls\1 = "[*.]contoso.edu"

```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: AllowTrackingForUrls
  - Beispielwert:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### AlwaysOpenPdfExternally
  #### PDF-Dateien immer extern öffnen
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Deaktiviert den internen PDF-Viewer in Microsoft Edge.

Wenn Sie diese Richtlinie aktivieren, werden PDF-Dateien von Microsoft Edge als Downloads behandelt und können von den Benutzern mit der Standardanwendung geöffnet werden.

Wenn Sie diese Richtlinie deaktivieren oder nicht konfigurieren, werden PDF-Dateien von Microsoft Edge geöffnet (es sei denn, dies wird vom Benutzer deaktiviert).

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Boolesch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: AlwaysOpenPdfExternally
  - Gruppenrichtlinienname: PDF-Dateien immer extern öffnen
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: AlwaysOpenPdfExternally
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000001
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: AlwaysOpenPdfExternally
  - Beispielwert:
``` xml
<true/>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### ApplicationLocaleValue
  #### Anwendungsgebietsschema festlegen
  >Unterstützte Versionen: Microsoft Edge unter Windows seit Version 77 oder höher

  #### Beschreibung
  Konfiguriert das Anwendungsgebietsschema in Microsoft Edge und verhindert, dass Benutzer das Gebietsschema ändern.

Wenn Sie diese Richtlinie aktivieren, verwendet Microsoft Edge das angegebene Gebietsschema. Wenn das konfigurierte Gebietsschema nicht unterstützt wird, wird stattdessen "en-US" verwendet.

Wenn Sie diese Einstellung deaktivieren oder nicht konfigurieren, verwendet Microsoft Edge entweder das vom Benutzer angegebene bevorzugte Gebietsschema (falls konfiguriert) oder das Fallback-Gebietsschema "en-US".

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Ja
  - Dynamische Richtlinienaktualisierung: Nein - Erfordert einen Neustart des Browsers

  #### Datentyp:
  Zeichenfolge

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: ApplicationLocaleValue
  - Gruppenrichtlinienname: Anwendungsgebietsschema festlegen
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Administrative Vorlagen/Microsoft Edge - Standardeinstellungen (können durch Benutzer überschrieben werden)/
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): SOFTWARE\Policies\Microsoft\Edge\Empfohlen
  - Wertname: ApplicationLocaleValue
  - Werttyp: REG_SZ
  ##### Beispielwert:
```
"en"
```


  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### AudioCaptureAllowed
  #### Audioaufnahme zulassen oder blockieren
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Hier können Sie einstellen, ob ein Benutzer aufgefordert wird, einer Website Zugriff auf sein Audioaufnahmegerät zu gewähren. Diese Richtlinie gilt für alle URLs mit Ausnahme derjenigen, die in der Liste [AudioCaptureAllowedUrls](#audiocaptureallowedurls) konfiguriert sind.

Wenn Sie diese Richtlinie aktivieren oder nicht konfigurieren (Standardeinstellung), wird der Benutzer mit Ausnahme der URLs in der Liste [AudioCaptureAllowedUrls](#audiocaptureallowedurls) aufgefordert. Diese aufgeführten URLs erhalten ohne Aufforderung Zugriff.

Wenn Sie diese Richtlinie deaktivieren, wird der Benutzer nicht aufgefordert, und Audioaufnahmen sind nur für die URLs möglich, die in [AudioCaptureAllowedUrls](#audiocaptureallowedurls) konfiguriert sind.

Diese Richtlinie betrifft alle Arten von Audioeingängen, nicht nur das eingebaute Mikrofon.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Boolesch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: AudioCaptureAllowed
  - Gruppenrichtlinienname: Audioaufnahme zulassen oder blockieren
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: AudioCaptureAllowed
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000000
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: AudioCaptureAllowed
  - Beispielwert:
``` xml
<false/>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### AudioCaptureAllowedUrls
  #### Websites, die auf Audioaufnahmegeräte zugreifen können, ohne eine Berechtigung anzufordern
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Geben Sie Websites basierend auf URL-Mustern an, die Audioaufnahmegeräte verwenden können, ohne den Benutzer um Erlaubnis zu bitten. Muster in dieser Liste werden mit dem Sicherheitsursprung der anfordernden URL abgeglichen. Wenn sie übereinstimmen, wird der Website automatisch der Zugriff auf Audioaufnahmegeräte gewährt.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Liste der Zeichenfolgen

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: AudioCaptureAllowedUrls
  - Gruppenrichtlinienname: Websites, die auf Audioaufnahmegeräte zugreifen können, ohne eine Berechtigung anzufordern
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge\AudioCaptureAllowedUrls
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: 1, 2, 3, ...
  - Werttyp: Liste von REG_SZ
  ##### Beispielwert:
```
SOFTWARE\Policies\Microsoft\Edge\AudioCaptureAllowedUrls\0 = "https://www.contoso.com/"
SOFTWARE\Policies\Microsoft\Edge\AudioCaptureAllowedUrls\1 = "https://[*.]contoso.edu/"

```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: AudioCaptureAllowedUrls
  - Beispielwert:
``` xml
<array>
  <string>https://www.contoso.com/</string>
  <string>https://[*.]contoso.edu/</string>
</array>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### AutoImportAtFirstRun
  #### Daten und Einstellungen eines anderen Browsers bei der ersten Ausführung automatisch importieren
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Wenn Sie diese Richtlinie aktivieren, importiert Microsoft Edge automatisch alle unterstützten Datentypen und Einstellungen aus dem Standardbrowser oder einem anderen angegebenen Browser. Dadurch wird auch erzwungen, dass Microsoft Edge den Importabschnitt der erstmaligen Ausführung überspringt.

Wenn Sie diese Richtlinie auf „DisabledAutoImport“ (4) festlegen, wird der Importabschnitt der erstmaligen Ausführung vollständig übersprungen, und Microsoft Edge importiert keine Browserdaten und -einstellungen automatisch.

* 0 = Importiert automatisch alle unterstützten Datentypen und Einstellungen aus dem Standardbrowser.

* 1 = Importiert automatisch alle unterstützten Datentypen und Einstellungen aus Internet Explorer.

* 2 = Importiert automatisch alle unterstützten Datentypen und Einstellungen aus Google Chrome.

* 3 = Importiert automatisch alle unterstützten Datentypen und Einstellungen aus Safari.

* 4 = Deaktiviert den automatischen Import, und der Importabschnitt der erstmaligen Ausführung wird übersprungen.

**Hinweis**: Diese Richtlinie unterstützt derzeit das Importieren aus den folgenden Browsern: Internet Explorer (unter Windows 7, 8 und 10), Google Chrome (unter Windows 7, 8 und 10 sowie macOS) und Apple Safari (unter macOS).

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Nein - Erfordert einen Neustart des Browsers

  #### Datentyp:
  Ganze Zahl

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: AutoImportAtFirstRun
  - Gruppenrichtlinienname: Daten und Einstellungen eines anderen Browsers bei der ersten Ausführung automatisch importieren
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: AutoImportAtFirstRun
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000002
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: AutoImportAtFirstRun
  - Beispielwert:
``` xml
<integer>2</integer>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### AutofillAddressEnabled
  #### AutoAusfüllen für Adressen aktivieren
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Aktiviert das AutoAusfüllen-Feature und ermöglicht Benutzern das automatische Vervollständigen von Adressinformationen in Webformularen mithilfe zuvor gespeicherter Informationen.

Wenn Sie diese Richtlinie deaktivieren, werden die Adressinformationen von AutoAusfüllen niemals vorgeschlagen oder ausgefüllt, und es werden auch keine weiteren Adressinformationen gespeichert, die der Benutzer beim Browsen im Web ggf. übermittelt.

Wenn Sie diese Richtlinie aktivieren oder nicht konfigurieren, können Benutzer AutoAusfüllen für Adressen in der Benutzeroberfläche steuern.

Hinweis: Wenn Sie diese Richtlinie deaktivieren, werden dadurch auch sämtliche Aktivitäten für alle Webformulare (mit Ausnahme von Zahlungs- und Kennwortformularen) beendet. Es werden keine weiteren Einträge gespeichert, und von Microsoft Edge werden keine zuvor verwendeten Einträge vorgeschlagen oder automatisch ausgefüllt.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Ja
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Boolesch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: AutofillAddressEnabled
  - Gruppenrichtlinienname: AutoAusfüllen für Adressen aktivieren
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Administrative Vorlagen/Microsoft Edge - Standardeinstellungen (können durch Benutzer überschrieben werden)/
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): SOFTWARE\Policies\Microsoft\Edge\Empfohlen
  - Wertname: AutofillAddressEnabled
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000000
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: AutofillAddressEnabled
  - Beispielwert:
``` xml
<false/>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### AutofillCreditCardEnabled
  #### AutoAusfüllen für Kreditkarten aktivieren
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Aktiviert das AutoAusfüllen-Feature von Microsoft Edge und ermöglicht Benutzern das automatische Ausfüllen von Kreditkarteninformationen in Webformularen mit zuvor gespeicherten Angaben.

Wenn Sie diese Richtlinie deaktivieren, werden von AutoAusfüllen keine Kreditkarteninformationen vorgeschlagen oder ausgefüllt, und es werden auch keine weiteren Kreditkarteninformationen gespeichert, die der Benutzer ggf. beim Surfen im Web übermittelt.

Wenn Sie diese Richtlinie aktivieren oder nicht konfigurieren, können Benutzer das automatische Ausfüllen von Kreditkarteninformationen steuern.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Ja
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Boolesch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: AutofillCreditCardEnabled
  - Gruppenrichtlinienname: AutoAusfüllen für Kreditkarten aktivieren
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Administrative Vorlagen/Microsoft Edge - Standardeinstellungen (können durch Benutzer überschrieben werden)/
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): SOFTWARE\Policies\Microsoft\Edge\Empfohlen
  - Wertname: AutofillCreditCardEnabled
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000000
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: AutofillCreditCardEnabled
  - Beispielwert:
``` xml
<false/>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### AutoplayAllowed
  #### Automatische Medienwiedergabe für Websites zulassen
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 78 oder höher

  #### Beschreibung
  Diese Richtlinie steuert die automatische Medienwiedergabe für Websites.

Bei Verwendung der Standardeinstellung „Nicht konfiguriert“ werden die aktuellen Einstellungen für die automatische Medienwiedergabe verwendet, und Benutzer können die automatische Wiedergabe wie gewünscht konfigurieren.

Bei Verwendung der Einstellung „Aktiviert“ wird die automatische Medienwiedergabe auf „Zulassen“ festgelegt. In diesem Fall ist die automatische Medienwiedergabe auf allen Websites zulässig. Benutzer können diese Richtlinie nicht überschreiben.

Bei Verwendung der Einstellung „Deaktiviert“ wird die automatische Medienwiedergabe auf „Blockieren“ festgelegt. In diesem Fall ist die automatische Medienwiedergabe auf keinen Websites zulässig. Benutzer können diese Richtlinie nicht überschreiben.

Diese Richtlinie wird erst wirksam, nachdem ein Tab geschlossen und erneut geöffnet wurde.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Boolesch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: AutoplayAllowed
  - Gruppenrichtlinienname: Automatische Medienwiedergabe für Websites zulassen
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: AutoplayAllowed
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000001
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: AutoplayAllowed
  - Beispielwert:
``` xml
<true/>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### BackgroundModeEnabled
  #### Ausführen von Hintergrund-Apps fortsetzen, nachdem Microsoft Edge geschlossen wurde
  >Unterstützte Versionen: Microsoft Edge unter Windows seit Version 77 oder höher

  #### Beschreibung
  Ermöglicht es Microsoft Edge-Prozessen, beim Einloggen in das Betriebssystem zu starten und nach dem Schließen des letzten Browserfensters weiter zu laufen. In diesem Szenario bleiben die Hintergrundanwendungen und die aktuelle Browsersitzung aktiv, einschließlich aller Sitzungs-Cookies. Ein offener Hintergrundprozess zeigt ein Symbol in der Taskleiste an und kann von dort aus immer geschlossen werden.

Wenn Sie diese Richtlinie aktivieren, wird der Hintergrundmodus eingeschaltet.

Wenn Sie diese Richtlinie deaktivieren, wird der Hintergrundmodus ausgeschaltet.

Wenn Sie diese Richtlinie nicht konfigurieren, wird der Hintergrundmodus zunächst deaktiviert, und der Benutzer kann dessen Verhalten in edge://settings/system konfigurieren.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Ja
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Boolesch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: BackgroundModeEnabled
  - Gruppenrichtlinienname: Ausführen von Hintergrund-Apps fortsetzen, nachdem Microsoft Edge geschlossen wurde
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Administrative Vorlagen/Microsoft Edge - Standardeinstellungen (können durch Benutzer überschrieben werden)/
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): SOFTWARE\Policies\Microsoft\Edge\Empfohlen
  - Wertname: BackgroundModeEnabled
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000001
```


  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### BackgroundTemplateListUpdatesEnabled
  #### Ermöglicht für Sammlungen und andere Features, die Vorlagen verwenden, Hintergrundaktualisierungen der Liste mit den verfügbaren Vorlagen.
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 79 oder höher

  #### Beschreibung
  Ermöglicht es Ihnen, für Sammlungen und andere Features, die Vorlagen verwenden, Hintergrundaktualisierungen der Liste mit den verfügbaren Vorlagen zu aktivieren oder zu deaktivieren. Vorlagen werden verwendet, um umfassende Metadaten aus einer Webseite zu extrahieren, wenn die Seite in einer Sammlung gespeichert wird.

Wenn Sie diese Einstellung aktivieren oder diese nicht konfiguriert ist, wird die Liste mit den verfügbaren Vorlagen alle 24 Stunden im Hintergrund von einem Microsoft-Dienst heruntergeladen.

Wenn Sie diese Einstellung deaktivieren, wird die Liste mit den verfügbaren Vorlagen bei Bedarf heruntergeladen. Diese Art von Download kann für Sammlungen und andere Features ggf. zu geringen Leistungseinbußen führen.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Boolesch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: BackgroundTemplateListUpdatesEnabled
  - Gruppenrichtlinienname: Ermöglicht für Sammlungen und andere Features, die Vorlagen verwenden, Hintergrundaktualisierungen der Liste mit den verfügbaren Vorlagen.
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: BackgroundTemplateListUpdatesEnabled
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000001
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: BackgroundTemplateListUpdatesEnabled
  - Beispielwert:
``` xml
<true/>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### BlockThirdPartyCookies
  #### Cookies von Drittanbietern blockieren
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Blockieren Sie das Festlegen von Cookies für Webseitenelemente, die nicht der Domäne in der Adressleiste angehören.

Wenn Sie diese Richtlinie aktivieren, können Webseitenelemente, die nicht der Domäne in der Adressleiste angehören, keine Cookies festlegen.

Wenn Sie diese Richtlinie deaktivieren, können Webseitenelemente, die Domänen angehören, die nicht in der Adressleiste enthalten sind, Cookies festlegen.

Wenn Sie diese Richtlinie nicht konfigurieren, sind Cookies von Drittanbietern aktiviert, aber Benutzer können diese Einstellung ändern.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Ja
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Boolesch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: BlockThirdPartyCookies
  - Gruppenrichtlinienname: Cookies von Drittanbietern blockieren
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Administrative Vorlagen/Microsoft Edge - Standardeinstellungen (können durch Benutzer überschrieben werden)/
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): SOFTWARE\Policies\Microsoft\Edge\Empfohlen
  - Wertname: BlockThirdPartyCookies
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000000
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: BlockThirdPartyCookies
  - Beispielwert:
``` xml
<false/>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### BrowserAddProfileEnabled
  #### Profilerstellung über das Flyout-Menü „Identität” oder die Seite „Einstellungen” aktivieren
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Ermöglicht Benutzern das Erstellen neuer Profile mithilfe der Option **Profil hinzufügen**.
Wenn Sie diese Richtlinie aktivieren oder nicht konfigurieren, können Benutzer in Microsoft Edge die Option **Profil hinzufügen** im Flyoutmenü „Identität“ oder auf der Seite „Einstellungen“ verwenden, um neue Profile zu erstellen.

Wenn Sie diese Richtlinie deaktivieren, können Benutzer keine neuen Profile über das Flyoutmenü „Identität“ oder die Seite „Einstellungen“ hinzufügen.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Boolesch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: BrowserAddProfileEnabled
  - Gruppenrichtlinienname: Profilerstellung über das Flyout-Menü „Identität” oder die Seite „Einstellungen” aktivieren
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: BrowserAddProfileEnabled
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000001
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: BrowserAddProfileEnabled
  - Beispielwert:
``` xml
<true/>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### BrowserGuestModeEnabled
  #### Gastmodus aktivieren
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Aktivieren Sie die Option, um die Verwendung von Gastprofilen in Microsoft Edge zu ermöglichen. In einem Gastprofil importiert der Browser keine Browserdaten aus vorhandenen Profilen und löscht die Browserdaten, wenn alle Gastprofile geschlossen werden.

Wenn Sie diese Richtlinie aktivieren oder nicht konfigurieren, lässt Microsoft Edge das Surfen in Gastprofilen für Benutzer zu.

Wenn Sie diese Richtlinie deaktivieren, lässt Microsoft Edge das Surfen in Gastprofilen für Benutzer nicht zu.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Boolesch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: BrowserGuestModeEnabled
  - Gruppenrichtlinienname: Gastmodus aktivieren
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: BrowserGuestModeEnabled
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000001
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: BrowserGuestModeEnabled
  - Beispielwert:
``` xml
<true/>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### BrowserNetworkTimeQueriesEnabled
  #### Abfragen bei einem Browser-Netzwerk-Zeitdienst zulassen
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Verhindert, dass Microsoft Edge gelegentlich Abfragen an einen Browser-Netzwerkzeitdienst sendet, um einen genauen Zeitstempel abzurufen.

Wenn Sie diese Richtlinie deaktivieren, sendet Microsoft Edge keine Abfragen mehr an einen Browser-Netzwerkzeitdienst.

Wenn Sie diese Richtlinie aktivieren oder nicht konfigurieren, sendet Microsoft Edge gelegentlich Abfragen an einen Browser-Netzwerkzeitdienst.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Boolesch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: BrowserNetworkTimeQueriesEnabled
  - Gruppenrichtlinienname: Abfragen bei einem Browser-Netzwerk-Zeitdienst zulassen
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: BrowserNetworkTimeQueriesEnabled
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000001
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: BrowserNetworkTimeQueriesEnabled
  - Beispielwert:
``` xml
<true/>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### BrowserSignin
  #### Browser-Anmeldeeinstellungen
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Bestimmt, ob sich ein Benutzer mit seinem Konto bei Microsoft Edge anmelden und kontobezogene Dienste wie Synchronisieren und Einmaliges Anmelden verwenden kann. Um die Verfügbarkeit der Synchronisierung zu steuern, verwenden Sie stattdessen die Richtlinie [SyncDisabled](#syncdisabled).

Wenn Sie diese Richtlinie auf 'Browseranmeldung deaktivieren' festlegen, müssen Sie auch die Richtlinie [NonRemovableProfileEnabled](#nonremovableprofileenabled) deaktivieren, weil [NonRemovableProfileEnabled](#nonremovableprofileenabled) die Erstellung eines automatisch erstellten Browserprofiles deaktiviert. Wenn beide Richtlinien aktiviert sind, verwendet Microsoft Edge die Einstellung 'Browseranmeldung deaktivieren' und verhält sich so, als wäre [NonRemovableProfileEnabled](#nonremovableprofileenabled) deaktiviert.

Wenn Sie diese Richtlinie auf "Browseranmeldung aktivieren" (1) setzen, können sich Benutzer im Browser anmelden. Die Anmeldung im Browser bedeutet nicht, dass die Synchronisierung standardmäßig aktiviert ist; der Benutzer muss sich separat anmelden, um dieses Feature nutzen zu können.

Wenn Sie diese Richtlinie auf "Browseranmeldung erzwingen" (2) einstellen, müssen sich Benutzer in einem Profil anmelden, um den Browser verwenden zu können. Der Benutzer kann somit standardmäßig wählen zwischen der Synchronisierung mit seinem Konto (sofern diese nicht vom Domänenadministrator deaktiviert wurde) und der Richtlinie [SyncDisabled](#syncdisabled). Der Standardwert für die Richtlinie [BrowserGuestModeEnabled](#browserguestmodeenabled) ist false.

Wenn Sie diese Richtlinie nicht konfigurieren, kann der Benutzer entscheiden, ob er die Browseranmeldung aktivieren und nach eigenem Ermessen verwenden möchte.

* 0 = Browseranmeldung deaktivieren

* 1 = Browseranmeldung aktivieren

* 2 = Browseranmeldung erzwingen

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Nein - Erfordert einen Neustart des Browsers

  #### Datentyp:
  Ganze Zahl

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: BrowserSignin
  - Gruppenrichtlinienname: Browser-Anmeldeeinstellungen
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: BrowserSignin
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000002
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: BrowserSignin
  - Beispielwert:
``` xml
<integer>2</integer>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### BuiltInDnsClientEnabled
  #### Integrierten DNS-Client verwenden
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Steuert, ob der integrierte DNS-Client verwendet wird.

Wenn Sie diese Richtlinie aktivieren, wird der integrierte DNS-Client verwendet, sofern er verfügbar ist.

Wenn Sie diese Richtlinie deaktivieren, wird der Client nie verwendet.

Wenn Sie diese Richtlinie nicht konfigurieren, wird der integrierte DNS-Client standardmäßig auf MacOS aktiviert, und Benutzer können ändern, ob der integrierte DNS-Client verwendet werden soll, indem sie edge://flags bearbeiten oder ein Befehlszeilen-Kennzeichen angeben.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Boolesch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: BuiltInDnsClientEnabled
  - Gruppenrichtlinienname: Integrierten DNS-Client verwenden
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: BuiltInDnsClientEnabled
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000001
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: BuiltInDnsClientEnabled
  - Beispielwert:
``` xml
<true/>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### CertificateTransparencyEnforcementDisabledForCas
  #### Erzwingung der Zertifikattransparenz für eine Liste von subjectPublicKeyInfo-Hashes deaktivieren
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Deaktiviert die Erzwingung der Zertifikatstransparenzanforderungen für eine Liste von subjectPublicKeyInfo-Hashes.

Mit dieser Richtlinie können Sie die Offenlegungsanforderungen für die Zertifikatstransparenz für Zertifikatketten deaktivieren, die Zertifikate mit einem der angegebenen subjectPublicKeyInfo-Hashes enthalten. Auf diese Weise können Zertifikate, die ansonsten nicht vertrauenswürdig wären, weil sie nicht ordnungsgemäß öffentlich bekannt gegeben wurden, weiterhin für Enterprise-Hosts verwendet werden.

Um die Erzwingung der Zertifikatstransparenz zu deaktivieren, wenn diese Richtlinie festgelegt ist, muss eine der folgenden Bedingungen erfüllt sein:
1. Der Hash muss im subjectPublicKeyInfo-Element des Serverzertifikats enthalten sein.
2. Der Hash muss in einem subjectPublicKeyInfo-Element enthalten sein, das in einem Zertifizierungsstellenzertifikat in der Zertifikatkette enthalten ist, das Zertifizierungsstellenzertifikat muss durch die X.509v3-Erweiterung „nameConstraints“ beschränkt sein, „permittedSubtrees“ muss mindestens eine Namensbeschränkung vom Typ „directoryName“ enthalten, und „directoryName“ muss ein organizationName-Attribut enthalten.
3. Der Hash muss in einem subjectPublicKeyInfo-Element enthalten sein, das in einem Zertifizierungsstellenzertifikat in der Zertifikatkette enthalten ist, der Antragsteller des Zertifizierungsstellenzertifikats muss mindestens ein organizationName-Attribut enthalten, und das Zertifikat des Servers muss die gleiche Anzahl von organizationName-Attributen enthalten (in der gleichen Reihenfolge und Byte für Byte identisch).

Zur Angabe eines subjectPublicKeyInfo-Hashs werden der Name des Hashalgorithmus, das Zeichen „/“ und die Base64-Codierung des Hashalgorithmus verkettet, der auf das DER-codierte subjectPublicKeyInfo-Element des angegebenen Zertifikats angewendet wurde. Diese Base64-Codierung hat das gleiche Format wie ein SPKI-Fingerabdruck gemäß Definition in RFC 7469, Abschnitt 2.4. Nicht erkannte Hashalgorithmen werden ignoriert. Aktuell wird nur der Hashalgorithmus „sha256“ unterstützt.

Wenn Sie diese Richtlinie deaktivieren oder nicht konfigurieren, werden alle Zertifikate, die über Certificate Transparency offengelegt werden müssen, als nicht vertrauenswürdig behandelt, wenn sie nicht gemäß der Certificate Transparency-Richtlinie offengelegt werden.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Liste der Zeichenfolgen

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: CertificateTransparencyEnforcementDisabledForCas
  - Gruppenrichtlinienname: Erzwingung der Zertifikattransparenz für eine Liste von subjectPublicKeyInfo-Hashes deaktivieren
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge\CertificateTransparencyEnforcementDisabledForCas
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: 1, 2, 3, ...
  - Werttyp: Liste von REG_SZ
  ##### Beispielwert:
```
SOFTWARE\Policies\Microsoft\Edge\CertificateTransparencyEnforcementDisabledForCas\0 = "sha256/AAAAAAAAAAAAAAAAAAAAAA=="
SOFTWARE\Policies\Microsoft\Edge\CertificateTransparencyEnforcementDisabledForCas\1 = "sha256//////////////////////w=="

```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: CertificateTransparencyEnforcementDisabledForCas
  - Beispielwert:
``` xml
<array>
  <string>sha256/AAAAAAAAAAAAAAAAAAAAAA==</string>
  <string>sha256//////////////////////w==</string>
</array>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### CertificateTransparencyEnforcementDisabledForLegacyCas
  #### Erzwingung der Zertifikattransparenz für eine Liste der Legacy-Zertifizierungsstellen deaktivieren
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Deaktiviert die Erzwingung der Zertifikattransparenz-Anforderungen für eine Liste der Legacy-Zertifizierungsstellen (Cas).

Mit dieser Richtlinie können Sie die Offenlegungsanforderungen für die Zertifikattransparenz für Zertifikatketten deaktivieren, die Zertifikate mit einem der angegebenen subjectPublicKeyInfo-Hashes enthalten. Dadurch können Zertifikate, die ansonsten nicht vertrauenswürdig wären, da Sie nicht ordnungsgemäß veröffentlicht wurden, weiterhin für Unternehmens-Hosts verwendet werden.

Damit die Erzwingung der Zertifikattransparenz deaktiviert werden kann, müssen Sie den Hash auf einen subjectPublicKeyInfo festlegen, der in einem Zertifizierungsstellenzertifikat angezeigt wird, das als eine Legacy-Zertifizierungsstelle (Certification Authority, CA) erkannt wird. Eine Legacy-CA ist eine CA, die standardmäßig von mindestens einem der von Microsoft Edge unterstützten Betriebssysteme als vertrauenswürdig eingestuft wurde.

Sie geben einen subjectPublicKeyInfo-Hash an, indem Sie den Hashalgorithmusnamen, das Zeichen "/" und die Base64-Codierung dieses Hashalgorithmus, die auf den DER-codierten subjectPublicKeyInfo des angegebenen Zertifikats angewendet wurde, verketten. Diese Base64-Codierung hat das gleiche Format wie ein SPKI-Fingerabdruck gemäß der Definition in RFC 7469, Abschnitt 2.4. Nicht erkannte Hashalgorithmen werden ignoriert. Der einzige unterstützte Hashalgorithmus ist zu diesem Zeitpunkt "sha256".

Wenn Sie diese Richtlinie nicht konfigurieren, wird jedes Zertifikat, das über die Zertifikattransparenz offengelegt werden muss, als nicht vertrauenswürdig eingestuft, wenn es nicht gemäß der Zertifikattransparenz-Richtlinie offengelegt wird.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Liste der Zeichenfolgen

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: CertificateTransparencyEnforcementDisabledForLegacyCas
  - Gruppenrichtlinienname: Erzwingung der Zertifikattransparenz für eine Liste der Legacy-Zertifizierungsstellen deaktivieren
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge\CertificateTransparencyEnforcementDisabledForLegacyCas
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: 1, 2, 3, ...
  - Werttyp: Liste von REG_SZ
  ##### Beispielwert:
```
SOFTWARE\Policies\Microsoft\Edge\CertificateTransparencyEnforcementDisabledForLegacyCas\0 = "sha256/AAAAAAAAAAAAAAAAAAAAAA=="
SOFTWARE\Policies\Microsoft\Edge\CertificateTransparencyEnforcementDisabledForLegacyCas\1 = "sha256//////////////////////w=="

```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: CertificateTransparencyEnforcementDisabledForLegacyCas
  - Beispielwert:
``` xml
<array>
  <string>sha256/AAAAAAAAAAAAAAAAAAAAAA==</string>
  <string>sha256//////////////////////w==</string>
</array>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### CertificateTransparencyEnforcementDisabledForUrls
  #### Erzwingung der Zertifikattransparenz für bestimmte URLs deaktivieren
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Deaktiviert die Erzwingung der Certificate Transparency-Anforderungen für die aufgeführten URLs.

Mit dieser Richtlinie können Sie die Offenlegung von Zertifikaten für die Hostnamen in den angegebenen URLs über Certificate Transparency verhindern. Dies ermöglicht die Verwendung von Zertifikaten, die andernfalls als nicht vertrauenswürdig eingestuft würden, da sie nicht ordnungsgemäß offengelegt wurden. Gleichzeitig wird jedoch die Erkennung nicht korrekt ausgestellter Zertifikate für diese Hosts erschwert.

Orientieren Sie sich bei Ihrem URL-Muster an „[https://go.microsoft.com/fwlink/?linkid=2095322](https://go.microsoft.com/fwlink/?linkid=2095322)“. Da Zertifikate für einen bestimmten Hostnamen gültig sind (unabhängig von Schema, Port oder Pfad), wird lediglich der Hostnamenteil der URL berücksichtigt. Platzhalterhosts werden nicht unterstützt.

Wenn Sie diese Richtlinie nicht konfigurieren, wird jedes Zertifikat, das über Certificate Transparency offengelegt werden muss, als nicht vertrauenswürdig behandelt, wenn es nicht offengelegt wird.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Liste der Zeichenfolgen

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: CertificateTransparencyEnforcementDisabledForUrls
  - Gruppenrichtlinienname: Erzwingung der Zertifikattransparenz für bestimmte URLs deaktivieren
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge\CertificateTransparencyEnforcementDisabledForUrls
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: 1, 2, 3, ...
  - Werttyp: Liste von REG_SZ
  ##### Beispielwert:
```
SOFTWARE\Policies\Microsoft\Edge\CertificateTransparencyEnforcementDisabledForUrls\0 = "contoso.com"
SOFTWARE\Policies\Microsoft\Edge\CertificateTransparencyEnforcementDisabledForUrls\1 = ".contoso.com"

```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: CertificateTransparencyEnforcementDisabledForUrls
  - Beispielwert:
``` xml
<array>
  <string>contoso.com</string>
  <string>.contoso.com</string>
</array>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### ClearBrowsingDataOnExit
  #### Browserdaten löschen, wenn Microsoft Edge geschlossen wird
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 78 oder höher

  #### Beschreibung
  Beim Schließen von Microsoft Edge werden die Browserdaten standardmäßig nicht gelöscht. Zu den Browserdaten gehören Informationen, die in Formulare eingegeben werden, Kennwörter und sogar die besuchten Websites.

Wenn Sie diese Richtlinie aktivieren, werden alle Browserdaten beim Schließen von Microsoft Edge gelöscht.

Wenn Sie diese Richtlinie deaktivieren oder nicht konfigurieren, können Benutzer die Option „Browserdaten löschen” in den Einstellungen konfigurieren.

Wenn Sie diese Richtlinie aktivieren, aktivieren Sie nicht die Richtlinie [AllowDeletingBrowserHistory](#allowdeletingbrowserhistory), da beide Daten löschen. Wenn Sie beide aktivieren, hat diese Richtlinie Vorrang und löscht alle Daten, wenn Microsoft Edge geschlossen wird, unabhängig davon, wie [AllowDeletingBrowserHistory](#allowdeletingbrowserhistory) konfiguriert ist.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Ja
  - Dynamische Richtlinienaktualisierung: Nein - Erfordert einen Neustart des Browsers

  #### Datentyp:
  Boolesch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: ClearBrowsingDataOnExit
  - Gruppenrichtlinienname: Browserdaten löschen, wenn Microsoft Edge geschlossen wird
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Administrative Vorlagen/Microsoft Edge - Standardeinstellungen (können durch Benutzer überschrieben werden)/
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): SOFTWARE\Policies\Microsoft\Edge\Empfohlen
  - Wertname: ClearBrowsingDataOnExit
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000001
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: ClearBrowsingDataOnExit
  - Beispielwert:
``` xml
<true/>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### ClickOnceEnabled
  #### Benutzern das Öffnen von Dateien unter Verwendung des ClickOnce-Protokolls ermöglichen
  >Unterstützte Versionen: Microsoft Edge unter Windows seit Version 78 oder höher

  #### Beschreibung
  Ermöglicht Benutzern das Öffnen von Dateien unter Verwendung des ClickOnce-Protokolls. Mit dem ClickOnce-Protokoll können Websites anfordern, dass der Browser Dateien von einer bestimmten URL öffnet und dabei den ClickOnce-Dateihandler auf dem Computer oder Gerät des Benutzers verwendet.

Wenn Sie diese Richtlinie aktivieren, können Benutzer Dateien unter Verwendung des ClickOnce-Protokolls öffnen. Diese Richtlinie überschreibt die ClickOnce-Einstellung des Benutzers auf der Seite „edge://flags/“.

Wenn Sie diese Richtlinie deaktivieren, können Benutzer keine Dateien unter Verwendung des ClickOnce-Protokolls öffnen. Die Datei wird stattdessen über den Browser im Dateisystem gespeichert. Diese Richtlinie überschreibt die ClickOnce-Einstellung des Benutzers auf der Seite „edge://flags/“.

Wenn Sie diese Richtlinie nicht konfigurieren, können Benutzer keine Dateien unter Verwendung des ClickOnce-Protokolls öffnen. Benutzer haben die Möglichkeit, die Verwendung des ClickOnce-Protokolls auf der Seite „edge://flags/“ zu aktivieren.

Ist ClickOnce deaktiviert, können ClickOnce-Anwendungen (APPLICATION-Dateien) möglicherweise nicht ordnungsgemäß gestartet werden.

Weitere Informationen zu ClickOnce finden Sie unter [https://go.microsoft.com/fwlink/?linkid=2103872](https://go.microsoft.com/fwlink/?linkid=2103872) und [https://go.microsoft.com/fwlink/?linkid=2099880](https://go.microsoft.com/fwlink/?linkid=2099880).

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Boolesch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: ClickOnceEnabled
  - Gruppenrichtlinienname: Benutzern das Öffnen von Dateien unter Verwendung des ClickOnce-Protokolls ermöglichen
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: ClickOnceEnabled
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000000
```


  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### CommandLineFlagSecurityWarningsEnabled
  #### Aktivieren von Sicherheitswarnungen für Befehlszeilenflags
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 78 oder höher

  #### Beschreibung
  Wenn diese Richtlinie deaktiviert ist, wird verhindert, dass Sicherheitswarnungen angezeigt werden, wenn Microsoft Edge mit potenziell gefährlichen Befehlszeilenflags gestartet wird.

Wenn diese Option aktiviert oder nicht festgelegt ist, werden Sicherheitswarnungen angezeigt, wenn diese Befehlszeilenflags zum Starten von Microsoft Edge verwendet werden.

Beispielsweise generiert das Flag "--disable-gpu-sandbox" die folgende Warnung: Sie verwenden ein nicht unterstütztes Befehlszeilenflag: --disable-gpu-sandbox. Dies stellt ein Stabilitäts- und Sicherheitsrisiko dar.

Unter Windows ist diese Richtlinie nur für Instanzen verfügbar, die mit einer Microsoft Active Directory-Domäne verbunden sind, oder für Windows 10 Pro- (oder Enterprise-Instanzen), die für die Geräteverwaltung registriert sind.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Nein - Erfordert einen Neustart des Browsers

  #### Datentyp:
  Boolesch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: CommandLineFlagSecurityWarningsEnabled
  - Gruppenrichtlinienname: Aktivieren von Sicherheitswarnungen für Befehlszeilenflags
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: CommandLineFlagSecurityWarningsEnabled
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000001
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: CommandLineFlagSecurityWarningsEnabled
  - Beispielwert:
``` xml
<true/>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### ComponentUpdatesEnabled
  #### Komponentenupdates in Microsoft Edge aktivieren
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Wenn Sie diese Richtlinie aktivieren oder nicht konfigurieren, werden Komponentenupdates in Microsoft Edge aktiviert.

Wenn Sie diese Richtlinie deaktivieren oder auf „false” festlegen, werden Komponentenupdates für alle Komponenten in Microsoft Edge deaktiviert.

Einige Komponenten sind jedoch von dieser Richtlinie ausgenommen. Dazu gehören alle Komponenten, die keinen ausführbaren Code enthalten, die das Verhalten des Browsers nicht wesentlich verändern oder die für die Sicherheit von entscheidender Bedeutung sind. Das heißt, Updates, die als „sicherheitskritisch” eingestuft sind, werden auch dann angewendet, wenn Sie diese Richtlinie deaktivieren.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Nein - Erfordert einen Neustart des Browsers

  #### Datentyp:
  Boolesch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: ComponentUpdatesEnabled
  - Gruppenrichtlinienname: Komponentenupdates in Microsoft Edge aktivieren
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: ComponentUpdatesEnabled
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000001
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: ComponentUpdatesEnabled
  - Beispielwert:
``` xml
<true/>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### ConfigureDoNotTrack
  #### Nicht verfolgen (Do not track) konfigurieren
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Geben Sie an, ob „Nicht verfolgen“-Anfragen an Websites gesendet werden sollen, die um Nachverfolgungsinformationen bitten. „Nicht verfolgen“-Anfragen informieren die von Ihnen besuchten Websites, dass Ihre Browseraktivitäten nicht nachverfolgt werden sollen. Standardmäßig sendet Microsoft Edge keine „Nicht verfolgen“-Anfragen, Benutzer können dieses Feature allerdings aktivieren, damit sie gesendet werden.

Wenn Sie diese Richtlinie aktivieren, werden „Nicht verfolgen“-Anfragen immer an Websites gesendet, die um Nachverfolgungsinformationen bitten.

Wenn Sie diese Richtlinie deaktivieren, werden nie Anfragen gesendet.

Wenn Sie diese Richtlinie nicht konfigurieren, können Benutzer auswählen, ob diese Anfragen gesendet werden sollen.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Boolesch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: ConfigureDoNotTrack
  - Gruppenrichtlinienname: Nicht verfolgen (Do not track) konfigurieren
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: ConfigureDoNotTrack
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000000
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: ConfigureDoNotTrack
  - Beispielwert:
``` xml
<false/>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### ConfigureOnlineTextToSpeech
  #### Online-Text-zu-Sprache konfigurieren
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Legt fest, ob der Browser Online Text to Speech-Sprachfonts nutzen kann, die Teil der Azure Cognitive Services sind. Diese Sprachfonts sind qualitativ hochwertiger als die vorinstallierten Systemschriftarten.

Wenn Sie diese Richtlinie aktivieren oder nicht konfigurieren, können webbasierte Anwendungen, die die SpeechSynthesis-API einsetzen, Online Text to Speech-Sprachfonts verwenden.

Wenn Sie diese Richtlinie deaktivieren, sind die Sprachfonts nicht verfügbar.

Lesen Sie hier mehr über diese Funktion:
SpeechSynthesis API: [https://go.microsoft.com/fwlink/?linkid=2110038](https://go.microsoft.com/fwlink/?linkid=2110038)
Cognitive Services: [https://go.microsoft.com/fwlink/?linkid=2110141](https://go.microsoft.com/fwlink/?linkid=2110141)

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Boolesch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: ConfigureOnlineTextToSpeech
  - Gruppenrichtlinienname: Online-Text-zu-Sprache konfigurieren
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: ConfigureOnlineTextToSpeech
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000001
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: ConfigureOnlineTextToSpeech
  - Beispielwert:
``` xml
<true/>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### CustomHelpLink
  #### Benutzerdefinierten Hilfelink angeben
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 79 oder höher

  #### Beschreibung
  Geben Sie einen Link für das Hilfemenü oder die F1-Taste an.

Wenn Sie diese Richtlinie aktivieren, kann ein Administrator einen Link für das Hilfemenü oder die F1-Taste angeben.

Wenn Sie diese Richtlinie deaktivieren oder nicht konfigurieren, wird der Standardlink für das Hilfemenü oder die F1-Taste verwendet.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Zeichenfolge

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: CustomHelpLink
  - Gruppenrichtlinienname: Benutzerdefinierten Hilfelink angeben
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: CustomHelpLink
  - Werttyp: REG_SZ
  ##### Beispielwert:
```
"https://go.microsoft.com/fwlink/?linkid=2080734"
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: CustomHelpLink
  - Beispielwert:
``` xml
<string>https://go.microsoft.com/fwlink/?linkid=2080734</string>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### DefaultBrowserSettingEnabled
  #### Microsoft Edge als Standardbrowser festlegen
  >Unterstützte Versionen: Microsoft Edge unter Windows 7 und Mac seit Version 77 oder höher

  #### Beschreibung
  Konfiguriert die standardmäßigen Browserprüfungen in Microsoft Edge und verhindert, dass Benutzer sie ändern.

Wenn Sie diese Richtlinie aktivieren, überprüft Microsoft Edge beim Start immer, ob es sich um den Standardbrowser handelt, und registriert sich automatisch, sofern dies möglich ist.

Wenn Sie diese Richtlinie deaktivieren, prüft Microsoft Edge Benutzersteuerelemente zum Festlegen dieser Option nie oder deaktiviert sie nie.

Wenn Sie diese Richtlinie nicht konfigurieren, ermöglicht Microsoft Edge dem Benutzer zu steuern, ob es sich um den Standardbrowser handelt und ob Benutzerbenachrichtigungen angezeigt werden, wenn dies nicht der Fall ist.

Hinweis für Windows-Administratoren: Diese Richtlinie funktioniert nur für PCs mit Windows 7. Für spätere Windows-Versionen müssen Sie eine "Standardanwendungszuordnungsdatei" bereitstellen, die Microsoft Edge als den Handler für die https- und http-Protokolle (und optional das FTP-Protokoll und für Dateiformate wie .html, .htm, .pdf, .svg, .webp) festlegt. Weitere Informationen finden Sie unter "[https://go.microsoft.com/fwlink/?linkid=2094932](https://go.microsoft.com/fwlink/?linkid=2094932)".

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Boolesch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: DefaultBrowserSettingEnabled
  - Gruppenrichtlinienname: Microsoft Edge als Standardbrowser festlegen
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: DefaultBrowserSettingEnabled
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000001
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: DefaultBrowserSettingEnabled
  - Beispielwert:
``` xml
<true/>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### DeveloperToolsAvailability
  #### Steuern, wo Entwicklungstools verwendet werden können
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Steuert, wo Entwicklertools verwendet werden können.

Wenn Sie diese Richtlinie auf "DeveloperToolsDisallowedForForceInstalledExtensions" (0, Standardeinstellung) festlegen, können Benutzer im Allgemeinen auf die Entwicklertools und die JavaScript-Konsole zugreifen, jedoch nicht im Kontext von Erweiterungen, die von der Unternehmensrichtlinie installiert werden.

Wenn Sie diese Richtlinie auf "DeveloperToolsAllowed" (1) festlegen, können Benutzer in allen Kontexten, einschließlich der von der Unternehmensrichtlinie installierten Erweiterungen, auf die Entwicklertools und die JavaScript-Konsole zugreifen.

Wenn Sie diese Richtlinie auf "DeveloperToolsDisallowed" (2) festlegen, können Benutzer nicht auf die Entwicklertools zugreifen oder Websiteelemente überprüfen. Tastenkombinationen und Menü- oder Kontextmenüeinträge, die die Entwicklertools oder die JavaScript-Konsole öffnen, sind deaktiviert.

* 0 = Die Entwicklertools für Erweiterungen, die von der Unternehmensrichtlinie installiert wurden, blockieren, in anderen Kontexten zulassen

* 1 = Verwendung der Entwicklertools zulassen

* 2 = Verwendung der Entwicklertools nicht zulassen

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Ganze Zahl

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: DeveloperToolsAvailability
  - Gruppenrichtlinienname: Steuern, wo Entwicklungstools verwendet werden können
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: DeveloperToolsAvailability
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000002
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: DeveloperToolsAvailability
  - Beispielwert:
``` xml
<integer>2</integer>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### DirectInvokeEnabled
  #### Benutzern das Öffnen von Dateien unter Verwendung des DirectInvoke-Protokolls ermöglichen
  >Unterstützte Versionen: Microsoft Edge unter Windows seit Version 78 oder höher

  #### Beschreibung
  Ermöglicht Benutzern das Öffnen von Dateien unter Verwendung des DirectInvoke-Protokolls. Mit dem DirectInvoke-Protokoll können Websites anfordern, dass der Browser Dateien von einer bestimmten URL öffnet und dabei einen spezifischen Dateihandler auf dem Computer oder Gerät des Benutzers verwendet.

Wenn Sie diese Richtlinie aktivieren oder nicht konfigurieren, können Benutzer Dateien unter Verwendung des DirectInvoke-Protokolls öffnen.

Wenn Sie diese Richtlinie deaktivieren, können Benutzer keine Dateien unter Verwendung des DirectInvoke-Protokolls öffnen. Die Datei wird stattdessen im Dateisystem gespeichert.

Hinweis: Wenn Sie DirectInvoke deaktivieren, funktionieren bestimmte Microsoft Office SharePoint Online-Features möglicherweise nicht wie erwartet.

Weitere Informationen zu DirectInvoke finden Sie unter [https://go.microsoft.com/fwlink/?linkid=2103872](https://go.microsoft.com/fwlink/?linkid=2103872) und [https://go.microsoft.com/fwlink/?linkid=2099871](https://go.microsoft.com/fwlink/?linkid=2099871).

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Boolesch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: DirectInvokeEnabled
  - Gruppenrichtlinienname: Benutzern das Öffnen von Dateien unter Verwendung des DirectInvoke-Protokolls ermöglichen
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: DirectInvokeEnabled
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000000
```


  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### Disable3DAPIs
  #### Unterstützung für 3D-Grafik-APIs deaktivieren
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Verhindern Sie, dass Webseiten auf die Grafikprozessoreinheit (GPU) zugreifen. Insbesondere können Webseiten nicht auf die WebGL-API zugreifen und Plug-Ins nicht auf die Pepper 3D-API.

Wenn Sie diese Richtlinie nicht konfigurieren oder deaktivieren, können Webseiten möglicherweise die WebGL-API und Plug-Ins die Pepper 3D-API verwenden. Microsoft Edge könnte standardmäßig weiterhin die Übergabe von Befehlszeilenargumenten erfordern, um diese APIs zu verwenden.

Wenn die Richtlinie [HardwareAccelerationModeEnabled](#hardwareaccelerationmodeenabled) auf false festgelegt ist, wird die Einstellung für die Richtlinie 'Disable3DAPIs' ignoriert. Dies entspricht der Festlegung der Richtlinie 'Disable3DAPIs' auf true.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Boolesch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: Disable3DAPIs
  - Gruppenrichtlinienname: Unterstützung für 3D-Grafik-APIs deaktivieren
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: Disable3DAPIs
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000000
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: Disable3DAPIs
  - Beispielwert:
``` xml
<false/>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### DisableScreenshots
  #### Aufnahme von Screenshots deaktivieren
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Steuert, ob Benutzer Screenshots der Browserseite aufnehmen können.

Wenn diese Option aktiviert ist, können Benutzer keine Screenshots mithilfe von Tastenkombinationen oder Erweiterungs-APIs aufnehmen.

Wenn diese Richtlinie deaktiviert oder nicht konfiguriert wird, können Benutzer Screenshots aufnehmen.

Hinweis: Diese Richtlinie steuert Screenshots, die innerhalb des Browsers selbst erstellt wurden. Auch wenn Sie diese Richtlinie aktivieren, können Benutzer möglicherweise weiterhin Screenshots mit einer Methode außerhalb des Browsers (z. B. mit einem Betriebssystemfeature oder einer anderen Anwendung) aufnehmen.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Boolesch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: DisableScreenshots
  - Gruppenrichtlinienname: Aufnahme von Screenshots deaktivieren
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: DisableScreenshots
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000001
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: DisableScreenshots
  - Beispielwert:
``` xml
<true/>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### DiskCacheDir
  #### Verzeichnis für Datenträgercache festlegen
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Konfiguriert das Verzeichnis, das zum Speichern von zwischengespeicherten Dateien verwendet werden soll.

Wenn Sie diese Richtlinie aktivieren, verwendet Microsoft Edge das angegebene Verzeichnis, unabhängig davon, ob der Benutzer das Kennzeichen "--disk-cache-dir" angegeben hat. Um Datenverlust oder andere unerwartete Fehler zu vermeiden, konfigurieren Sie diese Richtlinie nicht auf das Stammverzeichnis eines Volumes oder auf ein Verzeichnis, das für andere Zwecke verwendet wird, da Microsoft Edge dessen Inhalt verwaltet.

Eine Liste der Variablen, die Sie beim Angeben von Verzeichnissen und Pfaden verwenden können, finden Sie unter "[https://go.microsoft.com/fwlink/?linkid=2095041](https://go.microsoft.com/fwlink/?linkid=2095041)".

Wenn Sie diese Richtlinie nicht konfigurieren, wird das standardmäßige Cache-Verzeichnis verwendet, und Benutzer können diesen Standard mit dem Befehlszeilen-Kennzeichen "--disk-cache-dir" überschreiben.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Nein - Erfordert einen Neustart des Browsers

  #### Datentyp:
  Zeichenfolge

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: DiskCacheDir
  - Gruppenrichtlinienname: Verzeichnis für Datenträgercache festlegen
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: DiskCacheDir
  - Werttyp: REG_SZ
  ##### Beispielwert:
```
"${user_home}/Edge_cache"
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: DiskCacheDir
  - Beispielwert:
``` xml
<string>${user_home}/Edge_cache</string>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### DiskCacheSize
  #### Größe des Datenträgercaches festlegen (in Bytes)
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Konfiguriert die Cachegröße (in Bytes), die zum Speichern von Dateien auf dem Datenträger verwendet wird.

Wenn sie diese Richtlinie aktivieren, verwendet Microsoft Edge die bereitgestellte Cachegröße, unabhängig davon, ob der Benutzer das Kennzeichen "--disk-cache-size" angegeben hat. Der in dieser Richtlinie angegebene Wert ist keine harte Grenze, sondern eher ein Vorschlag für das Cachingsystem. Jeder beliebige Wert unter einigen Megabytes ist zu klein und wird auf ein angemessenes Minimum aufgerundet.

Wenn Sie den Wert dieser Richtlinie auf "0" festlegen, wird die Standardcachegröße verwendet, und die Benutzer können sie nicht ändern.

Wenn Sie diese Richtlinie nicht konfigurieren, wird die Standardgröße verwendet, aber die Benutzer können sie mit dem Kennzeichen "--cache-cache-size" außer Kraft setzen.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Nein - Erfordert einen Neustart des Browsers

  #### Datentyp:
  Ganze Zahl

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: DiskCacheSize
  - Gruppenrichtlinienname: Größe des Datenträgercaches festlegen (in Bytes)
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: DiskCacheSize
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x06400000
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: DiskCacheSize
  - Beispielwert:
``` xml
<integer>104857600</integer>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### DownloadDirectory
  #### Downloadverzeichnis festlegen
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Konfiguriert das Verzeichnis, das beim Herunterladen von Dateien verwendet werden soll.

Wenn Sie diese Richtlinie aktivieren, verwendet Microsoft Edge das bereitgestellte Verzeichnis, unabhängig davon, ob der Benutzer ein Verzeichnis angegeben hat oder dass er jedes Mal zum Auswählen des Pfads zum Herunterladen aufgefordert werden möchte. Eine Liste der Variablen, die verwendet werden können, finden Sie unter [https://go.microsoft.com/fwlink/?linkid=2095041](https://go.microsoft.com/fwlink/?linkid=2095041).

Wenn Sie diese Richtlinie deaktivieren oder nicht konfigurieren, wird das standardmäßige Downloadverzeichnis verwendet, und der Benutzer kann es ändern.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Ja
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Zeichenfolge

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: DownloadDirectory
  - Gruppenrichtlinienname: Downloadverzeichnis festlegen
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Administrative Vorlagen/Microsoft Edge - Standardeinstellungen (können durch Benutzer überschrieben werden)/
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): SOFTWARE\Policies\Microsoft\Edge\Empfohlen
  - Wertname: DownloadDirectory
  - Werttyp: REG_SZ
  ##### Beispielwert:
```
"/home/${user_name}/Downloads"
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: DownloadDirectory
  - Beispielwert:
``` xml
<string>/home/${user_name}/Downloads</string>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### DownloadRestrictions
  #### Download-Einschränkungen zulassen
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Konfiguriert den Typ der Downloads, den Microsoft Edge vollständig blockiert, ohne dass Benutzer die Sicherheitsentscheidung außer Kraft setzen können.

Legen Sie „Gefährliche Downloads blockieren“ (1) fest, um alle Downloads außer diejenigen zuzulassen, die Microsoft Defender SmartScreen-Warnungen aufweisen.

Legen Sie „Potenziell gefährliche Downloads blockieren“ (2) fest, um alle Downloads außer diejenigen zuzulassen, die Microsoft Defender SmartScreen-Warnungen vor potenziell gefährlichen Downloads aufweisen.

Legen Sie „Alle Downloads blockieren“ (3) fest, um alle Downloads zu blockieren.

Wenn Sie diese Richtlinie nicht konfigurieren oder die Option „Keine besonderen Einschränkungen“ (0) festlegen, durchlaufen die Downloads die üblichen Sicherheitseinschränkungen basierend auf den Microsoft Defender SmartScreen-Analyseergebnissen.

Beachten Sie, dass diese Einschränkungen für Downloads von Webseiteninhalten sowie für die Kontextmenüoption „Link herunterladen“ gelten. Diese Einschränkungen gelten nicht für das Speichern oder Herunterladen der aktuell angezeigten Seite oder für die Option „Als PDF speichern“ in den Druckoptionen.

Weitere Informationen zu Microsoft Defender SmartScreen finden Sie unter „[https://go.microsoft.com/fwlink/?linkid=2094934](https://go.microsoft.com/fwlink/?linkid=2094934)“.

* 0 = Keine besonderen Einschränkungen

* 1 = Gefährliche Downloads blockieren

* 2 = Potenziell gefährliche Downloads blockieren

* 3 = Alle Downloads blockieren

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Ja
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Ganze Zahl

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: DownloadRestrictions
  - Gruppenrichtlinienname: Download-Einschränkungen zulassen
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Administrative Vorlagen/Microsoft Edge - Standardeinstellungen (können durch Benutzer überschrieben werden)/
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): SOFTWARE\Policies\Microsoft\Edge\Empfohlen
  - Wertname: DownloadRestrictions
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000002
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: DownloadRestrictions
  - Beispielwert:
``` xml
<integer>2</integer>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### EdgeCollectionsEnabled
  #### Aktivieren der Sammlungsfunktion
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 78 oder höher

  #### Beschreibung
  Ermöglicht Benutzern den Zugriff auf die Sammlungsfunktion, mit der Inhalte effizienter und mit Office-Integration gesammelt, organisiert, freigegeben und exportiert werden können.

Wenn Sie diese Richtlinie aktivieren oder nicht konfigurieren, können Benutzer auf die Sammlungsfunktion in Microsoft Edge zugreifen und diese verwenden.

Wenn Sie diese Richtlinie deaktivieren, können Benutzer nicht auf die Sammlungsfunktion Microsoft Edge zugreifen und diese nicht verwenden.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Nein - Erfordert einen Neustart des Browsers

  #### Datentyp:
  Boolesch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: EdgeCollectionsEnabled
  - Gruppenrichtlinienname: Aktivieren der Sammlungsfunktion
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: EdgeCollectionsEnabled
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000001
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: EdgeCollectionsEnabled
  - Beispielwert:
``` xml
<true/>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### EditFavoritesEnabled
  #### Ermöglicht Benutzern das Bearbeiten von Favoriten.
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Aktivieren Sie diese Richtlinie, um Benutzern das Hinzufügen, Entfernen und Ändern von Favoriten zu ermöglichen. Dies ist das Standardverhalten, wenn Sie die Richtlinie nicht konfigurieren.

Wenn Sie diese Richtlinie deaktivieren, können Benutzer keine Favoriten mehr hinzufügen, entfernen oder ändern. Bereits vorhandene Favoriten können weiterhin verwendet werden.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Boolesch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: EditFavoritesEnabled
  - Gruppenrichtlinienname: Ermöglicht Benutzern das Bearbeiten von Favoriten.
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: EditFavoritesEnabled
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000000
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: EditFavoritesEnabled
  - Beispielwert:
``` xml
<false/>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### EnableDeprecatedWebPlatformFeatures
  #### Veraltete Webplattformfeatures vorübergehend wieder aktivieren
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Geben Sie eine Liste der veralteten Webplattformfeatures an, um sie vorübergehend wieder zu aktivieren.

Mit dieser Richtlinie können Sie veraltete Webplattformfeatures für einen begrenzten Zeitraum wieder aktivieren. Die Features werden anhand eines Zeichenfolgen-Tags gekennzeichnet.

Falls Sie diese Richtlinie nicht konfigurieren, wenn die Liste leer ist, oder falls ein Feature keinem der unterstützten Zeichenfolgen-Tags entspricht, bleiben alle veralteten Webplattformfeatures deaktiviert.

Auch wenn die Richtlinie selbst auf den Plattformen oben unterstützt wird, ist das Feature, das sie aktiviert, möglicherweise nicht auf all diesen Plattformen verfügbar. Nicht alle veralteten Webplattformfeatures können erneut aktiviert werden. Nur die unten explizit aufgelisteten können erneut und nur für einen begrenzten Zeitraum aktiviert werden. Dies variiert je nach Feature. Sie können die Absicht hinter Änderungen des Webplattformfeatures unter https://bit.ly/blinkintents betrachten.

Das allgemeine Format des Zeichenfolgen-Tags lautet [DeprecatedFeatureName]_EffectiveUntil[yyyymmdd].

* "ExampleDeprecatedFeature_EffectiveUntil20080902" = ExampleDeprecatedFeature-API bis 2008/09/02 aktivieren

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Liste der Zeichenfolgen

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: EnableDeprecatedWebPlatformFeatures
  - Gruppenrichtlinienname: Veraltete Webplattformfeatures vorübergehend wieder aktivieren
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge\EnableDeprecatedWebPlatformFeatures
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: 1, 2, 3, ...
  - Werttyp: Liste von REG_SZ
  ##### Beispielwert:
```
SOFTWARE\Policies\Microsoft\Edge\EnableDeprecatedWebPlatformFeatures\0 = "ExampleDeprecatedFeature_EffectiveUntil20080902"

```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: EnableDeprecatedWebPlatformFeatures
  - Beispielwert:
``` xml
<array>
  <string>ExampleDeprecatedFeature_EffectiveUntil20080902</string>
</array>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### EnableDomainActionsDownload
  #### Herunterladen von Domänenaktionen von Microsoft aktivieren
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  In Microsoft Edge stellen Domänenaktionen eine Reihe von Kompatibilitätsfeatures dar, die dazu beitragen, dass der Browser im Web ordnungsgemäß funktioniert.

Microsoft verfügt über eine Liste mit Aktionen, die aus Kompatibilitätsgründen für bestimmte Domänen ausgeführt werden. So kann der Browser beispielsweise die Zeichenfolge des Benutzer-Agents auf einer Website ändern, wenn bei dieser Website aufgrund der neuen Zeichenfolge des Benutzer-Agents in Microsoft Edge Probleme auftreten. Jede dieser Aktionen ist als Übergangslösung gedacht, während Microsoft versucht, das Problem in Zusammenarbeit mit dem Websitebesitzer zu beheben.

Beim Start des Browsers (und danach in regelmäßigen Abständen) wird der Experimentier- und Konfigurationsdienst kontaktiert, auf dem sich die neueste Liste mit auszuführenden Kompatibilitätsaktionen befindet. Diese Liste wird nach dem erstmaligen Abruf lokal gespeichert und bei nachfolgenden Anforderungen nur noch aktualisiert, falls sich die Kopie auf dem Server geändert hat.

Wenn Sie diese Richtlinie aktivieren, wird die Liste mit Domänenaktionen weiterhin vom Experimentier- und Konfigurationsdienst heruntergeladen.

Wenn Sie diese Richtlinie deaktivieren, wird die Liste mit Domänenaktionen nicht mehr vom Experimentier- und Konfigurationsdienst heruntergeladen.

Wenn Sie diese Richtlinie nicht konfigurieren, wird die Liste mit Domänenaktionen weiterhin vom Experimentier- und Konfigurationsdienst heruntergeladen.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Boolesch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: EnableDomainActionsDownload
  - Gruppenrichtlinienname: Herunterladen von Domänenaktionen von Microsoft aktivieren
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: EnableDomainActionsDownload
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000001
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: EnableDomainActionsDownload
  - Beispielwert:
``` xml
<true/>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### EnableOnlineRevocationChecks
  #### Onlineprüfungen für OCSP/Sperrlisten aktivieren
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Onlinesperrprüfungen bieten keinen wesentlichen Sicherheitsvorteil und sind standardmäßig deaktiviert.

Wenn Sie diese Richtlinie aktivieren, führt Microsoft Edge Onlineprüfungen für OCSP/Sperrlisten auf leichte Fehler durch. „Leichter Fehler“ bedeutet, dass das Zertifikat als gültig gilt, wenn der Sperrserver nicht erreicht werden kann.

Wenn Sie die Richtlinie deaktivieren oder nicht konfigurieren, führt Microsoft Edge keine Onlinesperrprüfungen durch.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Boolesch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: EnableOnlineRevocationChecks
  - Gruppenrichtlinienname: Onlineprüfungen für OCSP/Sperrlisten aktivieren
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: EnableOnlineRevocationChecks
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000000
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: EnableOnlineRevocationChecks
  - Beispielwert:
``` xml
<false/>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### EnterpriseHardwarePlatformAPIEnabled
  #### Ermöglichen der Verwendung der Enterprise Hardware Platform-API durch verwaltete Erweiterungen
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 78 oder höher

  #### Beschreibung
  Wenn diese Richtlinie aktiviert ist, dürfen anhand der Unternehmensrichtlinie installierte Erweiterungen die Enterprise Hardware Platform-API verwenden.
Wenn diese Richtlinie deaktiviert oder nicht festgelegt ist, dürfen keine Erweiterungen die Enterprise Hardware Platform-API verwenden.
Diese Richtlinie gilt auch für Komponentenerweiterungen.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Boolesch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: EnterpriseHardwarePlatformAPIEnabled
  - Gruppenrichtlinienname: Ermöglichen der Verwendung der Enterprise Hardware Platform-API durch verwaltete Erweiterungen
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: EnterpriseHardwarePlatformAPIEnabled
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000001
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: EnterpriseHardwarePlatformAPIEnabled
  - Beispielwert:
``` xml
<true/>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### ExperimentationAndConfigurationServiceControl
  #### Steuern der Kommunikation mit dem Experimentier- und Konfigurationsdienst
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  In Microsoft Edge wird der Experimentier- und Konfigurationsdienst zum Bereitstellen der Experimentier- und Konfigurationsnutzlast verwendet.

Die Nutzlast für Experimente besteht aus einer Liste von frühzeitigen Entwicklungsfeatures, die Microsoft für Tests und Feedback aktiviert.

Die Konfigurationsnutzlast besteht aus einer Liste von Einstellungen, die Microsoft für Microsoft Edge bereitstellen möchte, um die Benutzerfreundlichkeit zu optimieren. Die Konfigurationsnutzlast kann z. B. angeben, wie oft Microsoft Edge Anforderungen an den Experimentier- und Konfigurationsdienst sendet, um die neueste Nutzlast abzurufen.

Wenn Sie diese Richtlinie auf den Modus „Konfigurationen und Experimente abrufen“ festlegen, wird die vollständige Nutzlast vom Experimentier- und Konfigurationsdienst heruntergeladen. Dazu gehört sowohl die Experimentier- als auch die Konfigurationsnutzlast.

Wenn Sie diese Richtlinie auf den Modus „Nur Konfigurationen abrufen“ festlegen, wird nur die Konfigurationsnutzlast übermittelt.

Wenn Sie diese Richtlinie auf „Kommunikation mit dem Test- und Konfigurationsdienst deaktivieren“ festlegen, wird die Kommunikation mit dem Experimentier- und Konfigurationsdienst vollständig beendet.

Wenn Sie diese Richtlinie nicht konfigurieren, ist das Verhalten auf einem verwalteten Gerät bei Beta- und Stable-Kanälen dasselbe wie im Modus „Nur Konfigurationen abrufen“.

Wenn Sie diese Richtlinie nicht konfigurieren ist das Verhalten auf einem nicht verwalteten Gerät dasselbe wie im Modus „Konfigurationen und Experimente abrufen“.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Ganze Zahl

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: ExperimentationAndConfigurationServiceControl
  - Gruppenrichtlinienname: Steuern der Kommunikation mit dem Experimentier- und Konfigurationsdienst
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: ExperimentationAndConfigurationServiceControl
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000002
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: ExperimentationAndConfigurationServiceControl
  - Beispielwert:
``` xml
<integer>2</integer>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### ExternalProtocolDialogShowAlwaysOpenCheckbox
  #### Steuert, ob im Dialogfeld für externe Protokolle das Kontrollkästchen „Immer öffnen“ angezeigt wird.
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 79 oder höher

  #### Beschreibung
  Diese Richtlinie steuert, ob in Bestätigungsaufforderungen für den Start externer Protokolle das Kontrollkästchen „Immer öffnen“ angezeigt wird.

Wenn Sie diese Richtlinie auf „true“ festlegen, kann der Benutzer „Immer öffnen“ auswählen, wenn eine Bestätigungsaufforderungen für ein externes Protokoll angezeigt wird. Daraufhin werden dem Benutzer keine Bestätigungsaufforderungen für dieses Protokoll mehr angezeigt.

Wenn Sie diese Richtlinie auf „false“ festlegen oder die Richtlinie nicht festgelegt ist, wird das Kontrollkästchen „Immer öffnen“ nicht angezeigt, und der Benutzer wird jedes Mal zur Bestätigung aufgefordert, wenn ein externes Protokoll aufgerufen wird.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Nein - Erfordert einen Neustart des Browsers

  #### Datentyp:
  Boolesch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: ExternalProtocolDialogShowAlwaysOpenCheckbox
  - Gruppenrichtlinienname: Steuert, ob im Dialogfeld für externe Protokolle das Kontrollkästchen „Immer öffnen“ angezeigt wird.
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: ExternalProtocolDialogShowAlwaysOpenCheckbox
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000001
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: ExternalProtocolDialogShowAlwaysOpenCheckbox
  - Beispielwert:
``` xml
<true/>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### FavoritesBarEnabled
  #### Favoritenleiste aktivieren
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Aktiviert oder deaktiviert die Favoritenleiste.

Wenn Sie diese Richtlinie aktivieren, wird den Benutzern die Favoritenleiste angezeigt.

Wenn Sie diese Richtlinie deaktivieren, wird den Benutzern die Favoritenleiste nicht angezeigt.

Wenn diese Richtlinie nicht konfiguriert ist, kann der Benutzer entscheiden, ob er die Favoritenleiste verwenden möchte.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Ja
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Boolesch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: FavoritesBarEnabled
  - Gruppenrichtlinienname: Favoritenleiste aktivieren
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Administrative Vorlagen/Microsoft Edge - Standardeinstellungen (können durch Benutzer überschrieben werden)/
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): SOFTWARE\Policies\Microsoft\Edge\Empfohlen
  - Wertname: FavoritesBarEnabled
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000001
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: FavoritesBarEnabled
  - Beispielwert:
``` xml
<true/>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### ForceBingSafeSearch
  #### Bing SafeSearch erzwingen
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Sorgt dafür, dass bei Abfragen in der Bing-Websuche der angegebene SafeSearch-Wert verwendet wird. Diese Einstellung kann von Benutzern nicht geändert werden.

Wenn Sie diese Richtlinie auf „Aus“ festlegen, wird für SafeSearch in der Bing-Suche der Wert von „bing.com“ verwendet.

Wenn Sie diese Richtlinie auf „Moderat“ festlegen, wird in SafeSearch die moderate Einstellung verwendet. Bei dieser Einstellung werden nicht jugendfreie Videos und Bilder, aber keine Texte aus den Suchergebnissen herausgefiltert.

Wenn Sie diese Richtlinie auf „Streng“ festlegen, wird in SafeSearch die strenge Einstellung verwendet. Bei dieser Einstellung werden nicht jugendfreie Texte, Bilder und Videos herausgefiltert.

Wenn Sie diese Richtlinie deaktivieren oder nicht konfigurieren, wird SafeSearch in der Bing-Suche nicht erzwungen, und Benutzer können den gewünschten Wert auf „bing.com“ festlegen.

* 0 = Keine Sucheinschränkungen in Bing konfigurieren

* 1 = Moderate Sucheinschränkungen in Bing konfigurieren

* 2 = Strenge Sucheinschränkungen in Bing konfigurieren

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Ganze Zahl

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: ForceBingSafeSearch
  - Gruppenrichtlinienname: Bing SafeSearch erzwingen
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: ForceBingSafeSearch
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000000
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: ForceBingSafeSearch
  - Beispielwert:
``` xml
<integer>0</integer>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### ForceEphemeralProfiles
  #### Verwendung von kurzlebigen Profilen aktivieren
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Steuert, ob Benutzerprofile auf den kurzlebigen Modus umgestellt werden. Ein kurzlebiges Profil wird zu Beginn einer Sitzung erstellt und am Ende der Sitzung gelöscht und ist dem ursprünglichen Profil des Benutzers zugeordnet

Wenn Sie diese Richtlinie aktivieren, werden Profile im kurzlebigen Modus ausgeführt. Dadurch können Benutzer auf ihren eigenen Geräten arbeiten, ohne die Browserdaten auf diesen Geräten zu speichern. Wenn Sie diese Richtlinie als Betriebssystemrichtlinie aktivieren (beispielsweise per Gruppenrichtlinienobjekt unter Windows), gilt sie für jedes Profil im System.

Wenn Sie diese Richtlinie deaktivieren oder nicht konfigurieren, stehen Benutzern ihre regulären Profile zur Verfügung, wenn Sie sich beim Browser anmelden.

Im kurzlebigen Modus werden Profildaten nur für die Dauer der Benutzersitzung auf dem Datenträger gespeichert. Features wie Browserverlauf, Erweiterungen und deren Daten, Webdaten wie Cookies und Webdatenbanken werden nach dem Schließen des Browsers nicht gespeichert. Ein Benutzer kann jedoch weiterhin beliebige Daten manuell auf den Datenträger herunterladen sowie Seiten speichern oder ausdrucken. Bei Benutzern mit aktivierter Synchronisierung werden alle Daten genau wie bei regulären Profilen in ihren Synchronisierungskonten gespeichert. Benutzer können außerdem den InPrivate-Modus im kurzlebigen Modus verwenden, sofern Sie dies nicht explizit deaktivieren.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Nein - Erfordert einen Neustart des Browsers

  #### Datentyp:
  Boolesch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: ForceEphemeralProfiles
  - Gruppenrichtlinienname: Verwendung von kurzlebigen Profilen aktivieren
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: ForceEphemeralProfiles
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000001
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: ForceEphemeralProfiles
  - Beispielwert:
``` xml
<true/>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### ForceGoogleSafeSearch
  #### Google SafeSearch erzwingen
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Erzwingt bei Abfragen in der Google Websuche, dass SafeSearch aktiviert wird, und verhindert, dass Benutzer diese Einstellung ändern.

Wenn Sie diese Richtlinie aktivieren, ist SafeSearch in der Google-Suche immer aktiv.

Wenn Sie diese Richtlinie deaktivieren oder nicht konfigurieren, wird SafeSearch in der Google-Suche nicht erzwungen.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Boolesch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: ForceGoogleSafeSearch
  - Gruppenrichtlinienname: Google SafeSearch erzwingen
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: ForceGoogleSafeSearch
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000000
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: ForceGoogleSafeSearch
  - Beispielwert:
``` xml
<false/>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### ForceNetworkInProcess
  #### Ausführung von Netzwerkcode im Browserprozess erzwingen
  >Unterstützte Versionen: Microsoft Edge unter Windows seit Version 78 oder höher

  #### Beschreibung
  Diese Richtlinie erzwingt die Ausführung des Netzwerkcodes im Browserprozess.

Diese Richtlinie ist standardmäßig deaktiviert. Falls sie aktiviert ist, sind Benutzer nicht vor Sicherheitsproblemen geschützt, sobald der Netzwerkprozess in einer Sandbox ausgeführt wird.

Diese Richtlinie soll Unternehmen eine Möglichkeit bieten, zu Drittanbietersoftware zu migrieren, die nicht von Hooking der Netzwerk-APIs abhängig ist. Proxyserver werden anstelle von LSPs und Win32-API-Patches empfohlen.

Falls diese Richtlinie nicht festgelegt ist, kann Netzwerkcode je nach Feld-Tests des NetworkService-Experiments außerhalb des Browserprozesses ausgeführt werden.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Nein - Erfordert einen Neustart des Browsers

  #### Datentyp:
  Boolesch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: ForceNetworkInProcess
  - Gruppenrichtlinienname: Ausführung von Netzwerkcode im Browserprozess erzwingen
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: ForceNetworkInProcess
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000000
```


  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### ForceYouTubeRestrict
  #### Minimalen eingeschränkten Modus für YouTube erzwingen
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Erzwingt einen minimalen eingeschränkten Modus für YouTube und verhindert, dass Benutzer einen weniger eingeschränkten Modus auswählen.

Wenn Sie diese Richtlinie auf „Streng“ (2) festlegen, wird der strenge eingeschränkte Modus für YouTube erzwungen.

Wenn Sie diese Richtlinie auf „Moderat“ (1) festlegen, kann der Benutzer nur den moderaten und den strengen Modus für YouTube verwenden, und der eingeschränkte Modus kann vom Benutzer nicht deaktiviert werden.

Wenn Sie diese Richtlinie auf „Aus“ (0) festlegen oder nicht konfigurieren, wird der eingeschränkte Modus für YouTube nicht erzwungen. Externe Richtlinien (beispielsweise YouTube-Richtlinien) können den eingeschränkten Modus allerdings weiterhin erzwingen.

* 0: Der eingeschränkte Modus für YouTube wird nicht erzwungen.

* 1: Für YouTube wird mindestens der moderate eingeschränkte Modus erzwungen.

* 2: Für YouTube wird der strenge eingeschränkte Modus erzwungen.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Ganze Zahl

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: ForceYouTubeRestrict
  - Gruppenrichtlinienname: Minimalen eingeschränkten Modus für YouTube erzwingen
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: ForceYouTubeRestrict
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000000
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: ForceYouTubeRestrict
  - Beispielwert:
``` xml
<integer>0</integer>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### FullscreenAllowed
  #### Vollbildmodus zulassen
  >Unterstützte Versionen: Microsoft Edge unter Windows seit Version 77 oder höher

  #### Beschreibung
  Legen Sie die Verfügbarkeit des Vollbildmodus fest. Die gesamte Microsoft Edge-Benutzeroberfläche ist ausgeblendet und nur Webinhalte sind sichtbar.

Falls Sie diese Richtlinie aktivieren oder nicht konfigurieren, können Benutzer, Apps und Erweiterungen mit entsprechenden Berechtigungen den Vollbildmodus öffnen.

Falls Sie diese Richtlinie deaktivieren, können Benutzer, Apps und Erweiterungen den Vollbildmodus nicht öffnen.

Das Öffnen von Microsoft Edge im Kioskmodus mithilfe der Befehlszeile ist nicht verfügbar, wenn der Vollbildmodus deaktiviert ist.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Boolesch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: FullscreenAllowed
  - Gruppenrichtlinienname: Vollbildmodus zulassen
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: FullscreenAllowed
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000001
```


  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### GoToIntranetSiteForSingleWordEntryInAddressBar
  #### Direkte Intranetsitenavigation erzwingen anstatt in der Adressleiste nach einzelnen Worteinträgen zu suchen
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 78 oder höher

  #### Beschreibung
  Wenn Sie diese Richtlinie aktivieren, wird beim obersten Ergebnis der automatischen Vorschläge in der Vorschlagsliste der Adressleiste zu Intranetsites navigiert, sofern auf der Adressleiste ein einzelnes Wort ohne Interpunktion eingegeben wurde.

Bei Eingabe eines einzelnen Worts ohne Interpunktion erfolgt standardmäßig eine Navigation zu einer Intranetsite, die dem eingegebenen Text entspricht.

Wenn Sie diese Richtlinie aktivieren, führt das zweite Ergebnis der automatischen Vorschläge in der Vorschlagsliste der Adressleiste zu einer exakt wie eingegebenen Websuche, vorausgesetzt, bei diesem Text handelt es sich um ein einzelnes Wort ohne Zeichensetzung. Der Standardsuchanbieter wird verwendet, es sein denn, es wurde auch eine Richtlinie zur Verhinderung der Websuche aktiviert.

Die Aktivierung dieser Richtlinie bewirkt Folgendes:

Bei Abfragen mit einem einzelnen Wort, die üblicherweise zu einem Verlaufselement aufgelöst würden, erfolgt keine Navigation zu Sites mehr. Stattdessen versucht der Browser, zu internen Sites zu navigieren, die im Intranet einer Organisation möglicherweise nicht vorhanden sind. Dies führt zu einem 404-Fehler.

Für beliebte Suchbegriffe, die aus einem Wort bestehen, müssen manuell Suchvorschläge ausgewählt werden, damit eine ordnungsgemäße Suche ausgeführt wird.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Boolesch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: GoToIntranetSiteForSingleWordEntryInAddressBar
  - Gruppenrichtlinienname: Direkte Intranetsitenavigation erzwingen anstatt in der Adressleiste nach einzelnen Worteinträgen zu suchen
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: GoToIntranetSiteForSingleWordEntryInAddressBar
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000000
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: GoToIntranetSiteForSingleWordEntryInAddressBar
  - Beispielwert:
``` xml
<false/>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### HSTSPolicyBypassList
  #### Konfigurieren der Liste mit Namen, die die HSTS-Richtlinienprüfung umgehen
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 79 oder höher

  #### Beschreibung
  Die in dieser Liste angegebenen Hostnamen werden von der HSTS-Richtlinienprüfung ausgenommen, die unter Umständen Anforderungen von „http://“ auf „https://“ aktualisiert. In dieser Richtlinie sind nur Hostnamen mit einzelner Bezeichnung zulässig. Hostnamen müssen vereinheitlicht werden. Alle IDNs müssen ins Format für A-Einträge konvertiert werden, und alle ASCII-Zeichen müssen in Kleinbuchstaben angegeben werden. Diese Richtlinie gilt nur für die angegebenen Hostnamen und nicht für Unterdomänen der Namen in der Liste.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Nein - Erfordert einen Neustart des Browsers

  #### Datentyp:
  Liste der Zeichenfolgen

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: HSTSPolicyBypassList
  - Gruppenrichtlinienname: Konfigurieren der Liste mit Namen, die die HSTS-Richtlinienprüfung umgehen
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge\HSTSPolicyBypassList
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: 1, 2, 3, ...
  - Werttyp: Liste von REG_SZ
  ##### Beispielwert:
```
SOFTWARE\Policies\Microsoft\Edge\HSTSPolicyBypassList\0 = "meet"

```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: HSTSPolicyBypassList
  - Beispielwert:
``` xml
<array>
  <string>meet</string>
</array>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### HardwareAccelerationModeEnabled
  #### Hardwarebeschleunigung verwenden (sofern verfügbar)
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Geben Sie an, ob die Hardwarebeschleunigung verwendet werden soll, sofern sie verfügbar ist. Wenn Sie diese Richtlinie aktivieren oder nicht konfigurieren, wird die Hardwarebeschleunigung aktiviert, solange kein GPU-Feature ausdrücklich blockiert wird.

Wenn Sie diese Richtlinie deaktivieren, wird die Hardwarebeschleunigung deaktiviert.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Nein - Erfordert einen Neustart des Browsers

  #### Datentyp:
  Boolesch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: HardwareAccelerationModeEnabled
  - Gruppenrichtlinienname: Hardwarebeschleunigung verwenden (sofern verfügbar)
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: HardwareAccelerationModeEnabled
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000001
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: HardwareAccelerationModeEnabled
  - Beispielwert:
``` xml
<true/>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### ImportAutofillFormData
  #### Importieren von AutoAusfüllen-Formulardaten zulassen
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Ermöglicht Benutzern das Importieren von AutoAusfüllen-Formulardaten aus einem anderen Browser in Microsoft Edge.

Wenn Sie diese Richtlinie aktivieren, wird die Option zum manuellen Importieren von AutoAusfüllen-Daten automatisch ausgewählt.

Wenn Sie diese Richtlinie deaktivieren, werden bei der ersten Ausführung keine AutoAusfüllen-Formulardaten importiert, und Benutzer können sie auch nicht manuell importieren.

Wenn Sie diese Richtlinie nicht konfigurieren, werden AutoAusfüllen-Daten bei der ersten Ausführung importiert, und die Benutzer können bei späteren Browsersitzungen wählen, ob Sie sie manuell importieren möchten.

Sie können diese Richtlinie als Empfehlung festlegen. Das bedeutet, dass Microsoft Edge AutoAusfüllen-Daten bei der ersten Ausführung importiert und Benutzer die Option **AutoAusfüllen-Daten** beim manuellen Importieren aktivieren oder deaktivieren können.

**Hinweis**: Mit dieser Richtlinie wird derzeit das Importieren aus Google Chrome (unter Windows 7, 8 und 10 sowie unter macOS) verwaltet.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Ja
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Boolesch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: ImportAutofillFormData
  - Gruppenrichtlinienname: Importieren von AutoAusfüllen-Formulardaten zulassen
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Administrative Vorlagen/Microsoft Edge - Standardeinstellungen (können durch Benutzer überschrieben werden)/
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): SOFTWARE\Policies\Microsoft\Edge\Empfohlen
  - Wertname: ImportAutofillFormData
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000001
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: ImportAutofillFormData
  - Beispielwert:
``` xml
<true/>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### ImportBrowserSettings
  #### Importieren von Browsereinstellungen zulassen
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 78 oder höher

  #### Beschreibung
  Ermöglicht Benutzern das Importieren von Browsereinstellungen aus einem anderen Browser in Microsoft Edge.

Wenn Sie diese Richtlinie aktivieren, ist das Kontrollkästchen **Browsereinstellungen** im Dialogfeld **Browserdaten importieren** automatisch aktiviert.

Wenn Sie diese Richtlinie deaktivieren, werden bei der ersten Ausführung keine Browsereinstellungen importiert, und Benutzer können sie auch nicht manuell importieren.

Wenn Sie diese Richtlinie nicht konfigurieren, werden Browsereinstellungen bei der ersten Ausführung importiert, und die Benutzer können bei späteren Browsersitzungen wählen, ob Sie sie manuell importieren möchten.

Sie können diese Richtlinie auch als Empfehlung festlegen. Das bedeutet, dass Microsoft Edge die Einstellungen bei der ersten Ausführung importiert und Benutzer die Option **Browsereinstellungen** beim manuellen Importieren aktivieren oder deaktivieren können.

**Hinweis**: Mit dieser Richtlinie wird derzeit das Importieren von Google Chrome (unter Windows 7, 8, und 10 sowie unter macOS) verwaltet.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Ja
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Boolesch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: ImportBrowserSettings
  - Gruppenrichtlinienname: Importieren von Browsereinstellungen zulassen
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Administrative Vorlagen/Microsoft Edge - Standardeinstellungen (können durch Benutzer überschrieben werden)/
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): SOFTWARE\Policies\Microsoft\Edge\Empfohlen
  - Wertname: ImportBrowserSettings
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000001
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: ImportBrowserSettings
  - Beispielwert:
``` xml
<true/>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### ImportFavorites
  #### Importieren von Favoriten zulassen
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Ermöglicht Benutzern das Importieren von Favoriten aus einem anderen Browser in Microsoft Edge.

Wenn Sie diese Richtlinie aktivieren, wird das Kontrollkästchen **Favoriten** im Dialogfeld **Browserdaten importieren** automatisch aktiviert.

Wenn Sie diese Richtlinie deaktivieren, werden bei der ersten Ausführung keine Favoriten importiert, und Benutzer können sie auch nicht manuell importieren.

Wenn Sie diese Richtlinie nicht konfigurieren, werden Favoriten bei der ersten Ausführung importiert, und die Benutzer können bei späteren Browsersitzungen wählen, ob Sie sie manuell importieren möchten.

Sie können diese Richtlinie auch als Empfehlung festlegen. Das bedeutet, dass Microsoft Edge Favoriten bei der ersten Ausführung importiert und Benutzer die Option **Favoriten** beim manuellen Importieren aktivieren oder deaktivieren können.

**Hinweis**: Mit dieser Richtlinie wird derzeit das Importieren aus Internet Explorer (unter Windows 7, 8 und 10) Google Chrome (unter Windows 7, 8 und 10 sowie unter macOS) und Apple Safari (unter macOS) verwaltet.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Ja
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Boolesch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: ImportFavorites
  - Gruppenrichtlinienname: Importieren von Favoriten zulassen
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Administrative Vorlagen/Microsoft Edge - Standardeinstellungen (können durch Benutzer überschrieben werden)/
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): SOFTWARE\Policies\Microsoft\Edge\Empfohlen
  - Wertname: ImportFavorites
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000001
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: ImportFavorites
  - Beispielwert:
``` xml
<true/>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### ImportHistory
  #### Importieren des Browserverlaufs zulassen
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Ermöglicht Benutzern das Importieren ihres Browserverlaufs aus einem anderen Browser in Microsoft Edge.

Wenn Sie diese Richtlinie aktivieren, wird das Kontrollkästchen **Browserverlauf** im Dialogfeld **Browserdaten importieren** automatisch aktiviert.

Wenn Sie diese Richtlinie deaktivieren, werden Browserverlaufsdaten bei der ersten Ausführung nicht importiert, und Benutzer können sie auch nicht manuell importieren.

Wenn Sie diese Richtlinie nicht konfigurieren, werden Browserverlaufsdaten bei der ersten Ausführung importiert, und die Benutzer können bei späteren Browsersitzungen wählen, ob Sie sie manuell importieren möchten.

Sie können diese Richtlinie auch als Empfehlung festlegen. Das bedeutet, dass Microsoft Edge den Browserverlauf bei der ersten Ausführung importiert und Benutzer die Option **Verlauf** beim manuellen Importieren aktivieren oder deaktivieren können.

**Hinweis**: Mit dieser Richtlinie wird derzeit das Importieren aus Internet Explorer (unter Windows 7, 8 und 10) Google Chrome (unter Windows 7, 8 und 10 sowie unter macOS) und Apple Safari (macOS) verwaltet.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Ja
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Boolesch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: ImportHistory
  - Gruppenrichtlinienname: Importieren des Browserverlaufs zulassen
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Administrative Vorlagen/Microsoft Edge - Standardeinstellungen (können durch Benutzer überschrieben werden)/
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): SOFTWARE\Policies\Microsoft\Edge\Empfohlen
  - Wertname: ImportHistory
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000001
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: ImportHistory
  - Beispielwert:
``` xml
<true/>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### ImportHomepage
  #### Importieren von Startseiteneinstellungen zulassen
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Ermöglicht Benutzern das Importieren ihrer Startseiteneinstellung aus einem anderen Browser in Microsoft Edge.

Wenn Sie diese Richtlinie aktivieren, wird die Option zum manuellen Importieren der Startseiteneinstellung automatisch ausgewählt.

Wenn Sie diese Richtlinie deaktivieren, wird die Startseiteneinstellung bei der ersten Ausführung nicht importiert, und Benutzer können sie auch nicht manuell importieren.

Wenn Sie diese Richtlinie nicht konfigurieren, wird die Startseiteneinstellung bei der ersten Ausführung importiert, und die Benutzer können bei späteren Browsersitzungen wählen, ob Sie sie manuell importieren möchten.

Sie können diese Richtlinie als Empfehlung festlegen. Das bedeutet, dass Microsoft Edge die Startseiteneinstellung bei der ersten Ausführung importiert und Benutzer die Option **Startseite** beim manuellen Importieren aktivieren oder deaktivieren können.

**Hinweis**: Mit dieser Richtlinie wird derzeit das Importieren aus Internet Explorer (unter Windows 7, 8 und 10) verwaltet.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Boolesch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: ImportHomepage
  - Gruppenrichtlinienname: Importieren von Startseiteneinstellungen zulassen
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: ImportHomepage
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000001
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: ImportHomepage
  - Beispielwert:
``` xml
<true/>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### ImportOpenTabs
  #### Importieren offener Tabs zulassen
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 79 oder höher

  #### Beschreibung
  Ermöglicht Benutzern das Importieren von Browsereinstellungen aus einem anderen Browser in Microsoft Edge.

Wenn Sie diese Richtlinie aktivieren, ist das Kontrollkästchen **Browsereinstellungen** im Dialogfeld **Browserdaten importieren** automatisch aktiviert.

Wenn Sie diese Richtlinie deaktivieren, werden bei der ersten Ausführung keine Browsereinstellungen importiert, und Benutzer können sie auch nicht manuell importieren.

Wenn Sie diese Richtlinie nicht konfigurieren, werden Browsereinstellungen bei der ersten Ausführung importiert, und die Benutzer können bei späteren Browsersitzungen wählen, ob Sie sie manuell importieren möchten.

Sie können diese Richtlinie auch als Empfehlung festlegen. Das bedeutet, dass Microsoft Edge die Einstellungen bei der ersten Ausführung importiert und Benutzer die Option **Browsereinstellungen** beim manuellen Importieren aktivieren oder deaktivieren können.

**Hinweis**: Mit dieser Richtlinie wird derzeit das Importieren von Google Chrome (unter Windows 7, 8, und 10 sowie unter macOS) verwaltet.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Ja
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Boolesch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: ImportOpenTabs
  - Gruppenrichtlinienname: Importieren offener Tabs zulassen
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Administrative Vorlagen/Microsoft Edge - Standardeinstellungen (können durch Benutzer überschrieben werden)/
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): SOFTWARE\Policies\Microsoft\Edge\Empfohlen
  - Wertname: ImportOpenTabs
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000001
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: ImportOpenTabs
  - Beispielwert:
``` xml
<true/>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### ImportPaymentInfo
  #### Import von Zahlungsinformationen zulassen
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Ermöglicht Benutzern das Importieren von Zahlungsinformationen aus einem anderen Browser in Microsoft Edge.

Wenn Sie diese Richtlinie aktivieren, wird das Kontrollkästchen **Zahlungsinformationen** automatisch im Dialogfeld **Browserdaten importieren** aktiviert.

Wenn Sie diese Richtlinie deaktivieren, werden Zahlungsinformationen bei der erstmaligen Ausführung nicht importiert, und Benutzer können sie nicht manuell importieren.

Wenn Sie diese Richtlinie nicht konfigurieren, werden Zahlungsinformationen bei der erstmaligen Ausführung importiert, und die Benutzer können auswählen, ob sie bei späteren Browsersitzungen manuell importiert werden sollen.

Sie können diese Richtlinie auch als Empfehlung festlegen. Dies bedeutet, dass Microsoft Edge Zahlungsinformationen bei der erstmaligen Ausführung importiert, Benutzer die Option **Zahlungsinformationen** aber während des manuellen Imports aktivieren oder deaktivieren können.

**Hinweis:** Diese Richtlinie dient derzeit zum Verwalten des Imports aus Google Chrome (unter Windows 7, 8 und 10 sowie macOS).

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Ja
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Boolesch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: ImportPaymentInfo
  - Gruppenrichtlinienname: Import von Zahlungsinformationen zulassen
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Administrative Vorlagen/Microsoft Edge - Standardeinstellungen (können durch Benutzer überschrieben werden)/
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): SOFTWARE\Policies\Microsoft\Edge\Empfohlen
  - Wertname: ImportPaymentInfo
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000001
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: ImportPaymentInfo
  - Beispielwert:
``` xml
<true/>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### ImportSavedPasswords
  #### Importieren gespeicherter Kennwörter zulassen
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Ermöglicht Benutzern das Importieren gespeicherter Kennwörter aus einem anderen Browser in Microsoft Edge.

Wenn Sie diese Richtlinie aktivieren, wird die Option zum manuellen Importieren gespeicherter Kennwörter automatisch ausgewählt.

Wenn Sie diese Richtlinie deaktivieren, werden gespeicherte Kennwörter bei der ersten Ausführung nicht importiert, und Benutzer können sie auch nicht manuell importieren.

Wenn Sie diese Richtlinie nicht konfigurieren, werden Kennwörter bei der ersten Ausführung importiert, und die Benutzer können bei späteren Browsersitzungen wählen, ob Sie sie manuell importieren möchten.

Sie können diese Richtlinie als Empfehlung festlegen. Das bedeutet, dass Microsoft Edge Kennwörter bei der ersten Ausführung importiert und Benutzer die Option **Kennwörter** beim manuellen Importieren aktivieren oder deaktivieren können.

**Hinweis**: Mit dieser Richtlinie wird derzeit das Importieren aus Internet Explorer (unter Windows 7, 8 und 10) und Google Chrome (unter Windows 7, 8 und 10 sowie unter macOS) verwaltet.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Ja
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Boolesch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: ImportSavedPasswords
  - Gruppenrichtlinienname: Importieren gespeicherter Kennwörter zulassen
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Administrative Vorlagen/Microsoft Edge - Standardeinstellungen (können durch Benutzer überschrieben werden)/
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): SOFTWARE\Policies\Microsoft\Edge\Empfohlen
  - Wertname: ImportSavedPasswords
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000001
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: ImportSavedPasswords
  - Beispielwert:
``` xml
<true/>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### ImportSearchEngine
  #### Importieren von Suchmaschineneinstellungen zulassen
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Ermöglicht Benutzern das Importieren von Suchmaschineneinstellungen aus einem anderen Browser in Microsoft Edge.

Wenn Sie diese Richtlinie aktivieren, wird die Option zum Importieren von Suchmaschineneinstellungen automatisch ausgewählt.

Wenn Sie diese Richtlinie deaktivieren, werden bei der ersten Ausführung keine Suchmaschineneinstellungen importiert, und Benutzer können sie auch nicht manuell importieren.

Wenn Sie diese Richtlinie nicht konfigurieren, werden Suchmaschineneinstellungen bei der ersten Ausführung importiert, und die Benutzer können bei späteren Browsersitzungen wählen, ob Sie sie manuell importieren möchten.

Sie können diese Richtlinie als Empfehlung festlegen. Das bedeutet, dass Microsoft Edge Suchmaschineneinstellungen bei der ersten Ausführung importiert und Benutzer die Option **Suchmaschine** beim manuellen Importieren aktivieren oder deaktivieren können.

**Hinweis**: Mit dieser Richtlinie wird derzeit das Importieren aus Internet Explorer (unter Windows 7, 8 und 10) verwaltet.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Ja
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Boolesch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: ImportSearchEngine
  - Gruppenrichtlinienname: Importieren von Suchmaschineneinstellungen zulassen
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Administrative Vorlagen/Microsoft Edge - Standardeinstellungen (können durch Benutzer überschrieben werden)/
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): SOFTWARE\Policies\Microsoft\Edge\Empfohlen
  - Wertname: ImportSearchEngine
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000001
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: ImportSearchEngine
  - Beispielwert:
``` xml
<true/>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### InPrivateModeAvailability
  #### Verfügbarkeit des InPrivate-Modus konfigurieren
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Gibt an, ob der Benutzer Seiten im InPrivate-Modus in Microsoft Edge öffnen kann.

Wenn Sie diese Richtlinie nicht konfigurieren oder auf „Aktiviert“ (0) festlegen, können Benutzer Seiten im InPrivate-Modus öffnen.

Legen Sie diese Richtlinie auf „Deaktivieren“ (1) fest, um Benutzer daran zu hindern, den InPrivate-Modus zu verwenden.

Legen Sie diese Richtlinie auf „Erzwungen“ (2) fest, um immer den InPrivate-Modus zu verwenden.

* 0 = InPrivate-Modus verfügbar

* 1 = InPrivate-Modus deaktiviert

* 2 = InPrivate-Modus erzwungen

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Ganze Zahl

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: InPrivateModeAvailability
  - Gruppenrichtlinienname: Verfügbarkeit des InPrivate-Modus konfigurieren
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: InPrivateModeAvailability
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000001
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: InPrivateModeAvailability
  - Beispielwert:
``` xml
<integer>1</integer>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### InternetExplorerIntegrationLevel
  #### Internet Explorer-Integration konfigurieren
  >Unterstützte Versionen: Microsoft Edge unter Windows seit Version 77 oder höher

  #### Beschreibung
  Anleitungen zum Konfigurieren der optimalen Benutzeroberfläche für den Internet Explorer-Modus finden Sie unter "[https://go.microsoft.com/fwlink/?linkid=2094210](https://go.microsoft.com/fwlink/?linkid=2094210)".

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Nein - Erfordert einen Neustart des Browsers

  #### Datentyp:
  Ganze Zahl

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: InternetExplorerIntegrationLevel
  - Gruppenrichtlinienname: Internet Explorer-Integration konfigurieren
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: InternetExplorerIntegrationLevel
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000001
```


  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### InternetExplorerIntegrationSiteList
  #### Enterprise Mode Site List konfigurieren
  >Unterstützte Versionen: Microsoft Edge unter Windows seit Version 78 oder höher

  #### Beschreibung
  Anleitungen zum Konfigurieren der optimalen Benutzeroberfläche für den Internet Explorer-Modus finden Sie unter "[https://go.microsoft.com/fwlink/?linkid=2094210](https://go.microsoft.com/fwlink/?linkid=2094210)".

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Nein - Erfordert einen Neustart des Browsers

  #### Datentyp:
  Zeichenfolge

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: InternetExplorerIntegrationSiteList
  - Gruppenrichtlinienname: Enterprise Mode Site List konfigurieren
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: InternetExplorerIntegrationSiteList
  - Werttyp: REG_SZ
  ##### Beispielwert:
```
"https://internal.contoso.com/sitelist.xml"
```


  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### InternetExplorerIntegrationSiteRedirect
  #### Angeben des Verhaltens von seiteninternen Navigationsvorgängen zu nicht konfigurierten Websites, wenn diese über Seiten im Internet Explorer-Modus gestartet werden
  >Unterstützte Versionen: Microsoft Edge unter Windows seit Version 79 oder höher

  #### Beschreibung
  Eine "In-Page"-Navigation wird über einen Link, ein Skript oder ein Formular auf der aktuellen Seite gestartet. Es kann auch eine serverseitige Umleitung eines früheren "In-Page"-Navigationsversuchs sein. Umgekehrt kann ein Benutzer über die Browser-Steuerelemente eine Navigation starten, die nicht "in-page" und unabhängig von der aktuellen Seite ist, beispielsweise über die Adressleiste, die Zurück-Taste oder einen Favoriten-Link.

Mit dieser Einstellung können Sie festlegen, ob die Navigation von im Internet Explorer-Modus geladenen Seiten zu nicht konfigurierten Websites (die nicht in der Siteliste für den Enterprise-Modus konfiguriert sind) wieder zu Microsoft Edge zurückkehrt oder im Internet Explorer-Modus bleibt.

Diese Einstellung funktioniert in Verbindung mit:
[InternetExplorerIntegrationLevel](#internetexplorerintegrationlevel) ist festgelegt auf "Internet Explorer-Modus" (1)
und der Richtlinie
[InternetExplorerIntegrationSiteList](#internetexplorerintegrationsitelist), wenn die Liste mindestens einen Eintrag enthält.

Wenn Sie diese Richtlinie deaktivieren oder nicht konfigurieren, werden in diesem Modus nur Websites geöffnet, die für das Öffnen im Internet Explorer-Modus konfiguriert sind. Jede Website, die nicht für das Öffnen im Internet Explorer-Modus konfiguriert ist, wird zurück zu Microsoft Edge umgeleitet.

Wenn Sie diese Richtlinie aktivieren, können Sie eine der folgenden Navigationsoptionen wählen:
0 - Standard. Nur Websites, die für das Öffnen im Internet Explorer-Modus konfiguriert sind, werden in diesem Modus geöffnet. Jede Website, die nicht für das Öffnen im Internet Explorer-Modus konfiguriert ist, wird zurück zu Microsoft Edge umgeleitet.
1 - Nur die automatische Navigationen im Internet Explorer-Modus beibehalten. Verwenden Sie diese Option, wenn Sie das Standarderlebnis wünschen, mit der Ausnahme, dass alle automatischen Navigationen (z.B. 302-Umleitungen) zu nicht konfigurierten Websites im Internet Explorer-Modus verbleiben.
2 - Alle Navigationen auf der Seite verbleiben im Internet Explorer-Modus (am wenigsten empfohlen). Alle Navigationen von Seiten, die im IE-Modus geladen wurden, zu nicht konfigurierten Websites verbleiben im Internet Explorer-Modus.

Weitere Informationen zum Internet Explorer-Modus finden Sie unter [https://go.microsoft.com/fwlink/?linkid=2105106](https://go.microsoft.com/fwlink/?linkid=2105106)

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Nein - Erfordert einen Neustart des Browsers

  #### Datentyp:
  Ganze Zahl

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: InternetExplorerIntegrationSiteRedirect
  - Gruppenrichtlinienname: Angeben des Verhaltens von seiteninternen Navigationsvorgängen zu nicht konfigurierten Websites, wenn diese über Seiten im Internet Explorer-Modus gestartet werden
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: InternetExplorerIntegrationSiteRedirect
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000000
```


  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### IsolateOrigins
  #### Websiteisolation für bestimmte Ursprünge aktivieren
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Gibt Quellen an, die isoliert in einem eigenen Prozess ausgeführt werden sollen.
Diese Richtlinie isoliert auch Quellen, die von Subdomains benannt werden. Beispielsweise bewirkt die Angabe von https://contoso.com/, dass https://foo.contoso.com/ als Teil der Website https://contoso.com/ isoliert wird.
Wenn die Richtlinie aktiviert ist, wird jeder in einer kommagetrennten Liste stehenden Quellen in einem eigenen Prozess ausgeführt.
Wenn Sie diese Richtlinie deaktivieren, sind die Features 'IsolateOrigins' und 'SitePerProcess' deaktiviert. Benutzer können die Richtlinie 'IsolateOrigins' weiterhin manuell über Befehlszeilen-Flags aktivieren.
Wenn Sie die Richtlinie nicht konfigurieren, kann der Benutzer diese Einstellung ändern.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Nein - Erfordert einen Neustart des Browsers

  #### Datentyp:
  Zeichenfolge

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: IsolateOrigins
  - Gruppenrichtlinienname: Websiteisolation für bestimmte Ursprünge aktivieren
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: IsolateOrigins
  - Werttyp: REG_SZ
  ##### Beispielwert:
```
"https://contoso.com/,https://fabrikam.com/"
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: IsolateOrigins
  - Beispielwert:
``` xml
<string>https://contoso.com/,https://fabrikam.com/</string>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### ManagedFavorites
  #### Favoriten konfigurieren
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Konfiguriert eine Liste verwalteter Favoriten.

Die Richtlinie erstellt eine Liste mit Favoriten. Jeder Favorit enthält die Schlüssel "Name" und "URL", die den Namen des Favoriten und sein Ziel enthalten. Sie können einen Unterordner konfigurieren, indem Sie einen Favoriten ohne einen "URL"-Schlüssel definieren, jedoch mit einem zusätzlichen "Children"-Schlüssel, der eine Liste der oben definierten Favoriten enthält (von denen einige möglicherweise wieder Ordner sind). Microsoft Edge ändert unvollständige URLs so, als ob sie über die Adressleiste eingegeben wurden, z. B. wird "microsoft.com" zu "https://microsoft.com/".

Diese Favoriten werden in einem Ordner abgelegt, der nicht vom Benutzer geändert werden kann (der Benutzer kann jedoch auswählen, dass er in der Favoritenleiste ausgeblendet werden soll). Standardmäßig lautet der Ordnername "Verwaltete Favoriten". Sie können ihn jedoch ändern, indem Sie der Liste der Favoriten ein Wörterbuch mit dem Schlüssel "toplevel_name" mit dem gewünschten Ordnernamen als Wert hinzufügen.

Verwaltete Favoriten werden nicht mit dem Benutzerkonto synchronisiert und können nicht durch Erweiterungen geändert werden.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Wörterbuch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: ManagedFavorites
  - Gruppenrichtlinienname: Favoriten konfigurieren
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: ManagedFavorites
  - Werttyp: REG_SZ
  ##### Beispielwert:
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


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: ManagedFavorites
  - Beispielwert:
``` xml
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
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### ManagedSearchEngines
  #### Suchmaschinen verwalten
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Hiermit können Sie eine Liste mit bis zu 10 Suchmaschinen konfigurieren, von denen eine als Standardsuchmaschine gekennzeichnet sein muss.
Sie müssen für keine Suchmaschine die Kodierung angeben.

Wenn Sie diese Richtlinie aktivieren, können Benutzer in der Liste keine Suchmaschine hinzufügen, entfernen oder ändern. Benutzer können jede Suchmaschine in der Liste als ihre Standardsuchmaschine festlegen.

Wenn Sie diese Richtlinie deaktivieren oder nicht konfigurieren, können Benutzer die Suchmaschinenliste nach Belieben ändern.

Wenn die Richtlinie [DefaultSearchProviderSearchURL](#defaultsearchprovidersearchurl) festgelegt ist, wird die Richtlinie (ManagedSearchEngines) ignoriert. Der Benutzer muss seinen Browser neu starten, um die Anwendung dieser Richtlinie abzuschließen.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Nein - Erfordert einen Neustart des Browsers

  #### Datentyp:
  Wörterbuch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: ManagedSearchEngines
  - Gruppenrichtlinienname: Suchmaschinen verwalten
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: ManagedSearchEngines
  - Werttyp: REG_SZ
  ##### Beispielwert:
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


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: ManagedSearchEngines
  - Beispielwert:
``` xml
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
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### MaxConnectionsPerProxy
  #### Maximale Anzahl gleichzeitiger Verbindungen mit dem Proxyserver
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Gibt die maximale Anzahl gleichzeitiger Verbindungen mit dem Proxyserver an.

Einige Proxyserver können keine hohe Anzahl gleichzeitiger Verbindungen pro Client verarbeiten. Sie können dies lösen, indem Sie für diese Richtlinie einen niedrigeren Wert festlegen.

Der Wert dieser Richtlinie muss niedriger als 100 und höher als 6 sein. Der Standardwert ist 32.

Einige Webanwendungen sind dafür bekannt, viele Verbindungen mit hängenden GETs zu verbrauchen. Das Senken der maximalen Anzahl auf weniger als 32 kann dazu führen, dass sich das Browsernetzwerk aufhängt, wenn zu viele Web-Apps dieser Art geöffnet sind.

Wenn Sie diese Richtlinie nicht konfigurieren, wird der Standardwert (32) verwendet.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Nein - Erfordert einen Neustart des Browsers

  #### Datentyp:
  Ganze Zahl

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: MaxConnectionsPerProxy
  - Gruppenrichtlinienname: Maximale Anzahl gleichzeitiger Verbindungen mit dem Proxyserver
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: MaxConnectionsPerProxy
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000020
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: MaxConnectionsPerProxy
  - Beispielwert:
``` xml
<integer>32</integer>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### MediaRouterCastAllowAllIPs
  #### Google Cast erlauben, eine Verbindung mit CAST-Geräten auf allen IP-Adressen herzustellen
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Aktivieren Sie diese Richtlinie, damit Google Cast eine Verbindung zu Cast-Geräten mit allen IP-Adressen herstellen kann, nicht nur mit privaten RFC1918/RFC4193-Adressen.

Deaktivieren Sie diese Richtlinie, um Google Cast auf Cast-Geräte mit privaten RFC1918/RFC4193-Adressen zu beschränken.

Wenn Sie diese Richtlinie nicht konfigurieren, verbindet sich Google Cast nur mit Cast-Geräten mit privaten RFC1918/RFC4193-Adressen, es sei denn, Sie aktivieren das CastAllowAllIPs-Feature.

Wenn die Richtlinie [EnableMediaRouter](#enablemediarouter) deaktiviert ist, hat diese Richtlinie keine Wirkung.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Boolesch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: MediaRouterCastAllowAllIPs
  - Gruppenrichtlinienname: Google Cast erlauben, eine Verbindung mit CAST-Geräten auf allen IP-Adressen herzustellen
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: MediaRouterCastAllowAllIPs
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000000
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: MediaRouterCastAllowAllIPs
  - Beispielwert:
``` xml
<false/>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### MetricsReportingEnabled
  #### Meldung von nutzungs- und absturzbezogenen Daten aktivieren
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  For Windows 10 Beta and Stable channels of Microsoft Edge, this policy when configured will override the Windows diagnostic data setting for collection or non-collection of Microsoft Edge usage and crash related data ([https://go.microsoft.com/fwlink/?linkid=2099569](https://go.microsoft.com/fwlink/?linkid=2099569)).

This policy enables reporting of usage and crash-related data about Microsoft Edge to Microsoft and prevents users from changing this setting.

Enable this policy to send reporting of usage and crash-related data to Microsoft. Disable this policy to not send the data to Microsoft. In both cases, users can't change or override the setting.

On Windows 10, Beta and Stable channels, this policy controls usage data. Crash-related data is determined by the Windows diagnostic data setting. If this policy is not configured, Microsoft Edge will default to the Windows diagnostic data setting.

On Windows 10, Canary and Dev channels, this policy controls usage and crash related data. If this policy is not configured, Microsoft Edge will default to the user's preference.

On Windows 7, 8, and Mac this policy controls usage and crash related data. If this policy is not configured, Microsoft Edge will default to the user's preference.

This policy is available only on Windows instances that are joined to a Microsoft Active Directory domain or Windows 10 Pro or Enterprise instances enrolled for device management.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Nein - Erfordert einen Neustart des Browsers

  #### Datentyp:
  Boolesch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: MetricsReportingEnabled
  - Gruppenrichtlinienname: Meldung von nutzungs- und absturzbezogenen Daten aktivieren
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: MetricsReportingEnabled
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000001
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: MetricsReportingEnabled
  - Beispielwert:
``` xml
<true/>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### NetworkPredictionOptions
  #### Netzwerkvorhersage aktivieren
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Aktiviert die Netzwerkvorhersage und verhindert, dass Benutzer diese Einstellung ändern.

Diese Richtlinie steuert DNS-Vorabrufe, TCP- und SSL-Vorabverbindungen sowie das Vorabrendern von Webseiten.

Wenn Sie diese Richtlinie nicht konfigurieren, ist die Netzwerkvorhersage aktiviert, kann aber vom Benutzer geändert werden.

* 0: Netzwerkaktionen werden für alle Netzwerkverbindungen vorhergesagt.

* 2: Netzwerkaktionen werden für keine Netzwerkverbindung vorhergesagt.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Ja
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Ganze Zahl

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: NetworkPredictionOptions
  - Gruppenrichtlinienname: Netzwerkvorhersage aktivieren
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Administrative Vorlagen/Microsoft Edge - Standardeinstellungen (können durch Benutzer überschrieben werden)/
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): SOFTWARE\Policies\Microsoft\Edge\Empfohlen
  - Wertname: NetworkPredictionOptions
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000001
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: NetworkPredictionOptions
  - Beispielwert:
``` xml
<integer>1</integer>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### NonRemovableProfileEnabled
  #### Konfigurieren, ob für einen Benutzer beim Anmelden mit dem Geschäfts-, Schul-oder Unikonto immer automatisch ein Standardprofil vorhanden ist.
  >Unterstützte Versionen: Microsoft Edge unter Windows seit Version 78 oder höher

  #### Beschreibung
  Mit dieser Richtlinie wird bestimmt, ob das Microsoft Edge-Profil, das für das Geschäfts-, Schul- oder Unikonto eines Benutzers automatisch angemeldet wird, entfernt werden kann.

Unabhängig davon, ob Sie diese Richtlinie aktivieren oder nicht konfigurieren, wird mit dem Geschäfts-, Schul- oder Unikonto des Benutzers unter Windows ein nicht entfernbares Profil erstellt. Dieses Profil kann nicht abgemeldet oder entfernt werden.

Wenn Sie diese Richtlinie deaktivieren, kann das Profil, das für das Geschäfts-, Schul- oder Unikonto eines Benutzers unter Windows automatisch angemeldet wird, abgemeldet oder entfernt werden.

Verwenden Sie die Richtlinie „BrowserSignIn“, falls Sie die Browseranmeldung vollständig deaktivieren möchten.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Boolesch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: NonRemovableProfileEnabled
  - Gruppenrichtlinienname: Konfigurieren, ob für einen Benutzer beim Anmelden mit dem Geschäfts-, Schul-oder Unikonto immer automatisch ein Standardprofil vorhanden ist.
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: NonRemovableProfileEnabled
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000001
```


  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### OverrideSecurityRestrictionsOnInsecureOrigin
  #### Steuert, wo Sicherheitseinschränkungen für unsichere Ursprünge gelten
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Gibt eine Liste mit Ursprüngen (URLs) oder Hostnamen-Mustern (z. B. „*.contoso.com“) an, für die keine Sicherheitseinschränkungen bei unsicheren Ursprüngen gelten.

Mit dieser Richtlinie können Sie die zulässigen Ursprünge für ältere Anwendungen angeben, die TLS nicht bereitstellen kann, oder einen Stagingserver für die interne Webentwicklung einrichten, sodass Entwickler Features testen können, die sichere Kontexte erfordern, ohne dass TLS auf dem Server bereitgestellt ist. Durch diese Richtlinie wird auch verhindert, dass der Ursprung in der Omnibox als „nicht sicher“ gekennzeichnet ist.

Das Festlegen einer Liste von URLs in dieser Richtlinie hat denselben Effekt wie das Festlegen des Befehlszeilenflags „--unsafely-treat-insecure-origin-as-secure“ in einer durch Kommas getrennte Liste derselben URLs. Wenn Sie diese Richtlinie aktivieren, wird das Befehlszeilenflag überschrieben.

Weitere Informationen zu sicheren Kontexten finden Sie unter https://www.w3.org/TR/secure-contexts/.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Nein - Erfordert einen Neustart des Browsers

  #### Datentyp:
  Liste der Zeichenfolgen

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: OverrideSecurityRestrictionsOnInsecureOrigin
  - Gruppenrichtlinienname: Steuert, wo Sicherheitseinschränkungen für unsichere Ursprünge gelten
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge\OverrideSecurityRestrictionsOnInsecureOrigin
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: 1, 2, 3, ...
  - Werttyp: Liste von REG_SZ
  ##### Beispielwert:
```
SOFTWARE\Policies\Microsoft\Edge\OverrideSecurityRestrictionsOnInsecureOrigin\0 = "http://testserver.contoso.com/"
SOFTWARE\Policies\Microsoft\Edge\OverrideSecurityRestrictionsOnInsecureOrigin\1 = "*.contoso.com"

```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: OverrideSecurityRestrictionsOnInsecureOrigin
  - Beispielwert:
``` xml
<array>
  <string>http://testserver.contoso.com/</string>
  <string>*.contoso.com</string>
</array>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### PinningWizardAllowed
  #### Allow Pin to taskbar wizard
  >Unterstützte Versionen: Microsoft Edge unter Windows seit Version 80 oder höher

  #### Beschreibung
  Microsoft Edge uses the Pin to taskbar wizard to help users pin suggested sites to the taskbar. The Pin to taskbar wizard feature is enabled by default and accessible to the user through the Settings and more menu.

If you enable this policy or don't configure it, users can call the Pin to taskbar wizard from the Settings and More menu. The wizard can also be called via a protocol launch.

If you disable this policy, the Pin to taskbar wizard is disabled in the menu and cannot be called via a protocol launch.

User settings to enable or disable the Pin to taskbar wizard aren't available.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Nein - Erfordert einen Neustart des Browsers

  #### Datentyp:
  Boolesch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: PinningWizardAllowed
  - Gruppenrichtlinienname: Allow Pin to taskbar wizard
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: PinningWizardAllowed
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000000
```


  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### ProactiveAuthEnabled
  #### Proaktive Authentifizierung aktivieren
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Hiermit können Sie konfigurieren, ob die proaktive Authentifizierung aktiviert werden soll.

Wenn sie diese Richtlinie aktivieren, versucht Microsoft Edge, den angemeldeten Benutzer proaktiv mit Microsoft-Diensten zu authentifizieren. Microsoft Edge sucht in regelmäßigen Abständen mit einem Onlinedienst ein aktualisiertes Manifest, das die Konfiguration enthält, in der die Vorgehensweise geregelt wird.

Wenn sie diese Richtlinie deaktivieren, versucht Microsoft Edge nicht, den angemeldeten Benutzer proaktiv mit Microsoft-Diensten zu authentifizieren. Microsoft Edge sucht dann nicht mehr mit einem Onlinedienst nach einem aktualisierten Manifest, das die entsprechende Konfiguration enthält.

Wenn Sie diese Richtlinie nicht konfigurieren, ist die proaktive Authentifizierung aktiviert.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Nein - Erfordert einen Neustart des Browsers

  #### Datentyp:
  Boolesch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: ProactiveAuthEnabled
  - Gruppenrichtlinienname: Proaktive Authentifizierung aktivieren
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: ProactiveAuthEnabled
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000001
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: ProactiveAuthEnabled
  - Beispielwert:
``` xml
<true/>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### PromotionalTabsEnabled
  #### Tabfüllende Werbeinhalte ermöglichen
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Steuert die Darstellung von Werbe- oder informativen Inhalten für vollständige Tabs. Mit dieser Einstellung wird die Darstellung von Willkommensseiten gesteuert, über die Benutzer sich bei Microsoft Edge anmelden, den Standardbrowser auswählen oder Informationen zu Produktfeatures erhalten.

Wenn sie diese Richtlinie aktivieren (auf "wahr" festlegen) oder nicht konfigurieren, kann Microsoft Edge Benutzern vollständige Tabinhalte anzeigen, um Produktinformationen bereitzustellen.

Wenn Sie diese Richtlinie deaktivieren (auf "false" festlegen), kann Microsoft Edge keine vollständigen Tabinhalte für Benutzer anzeigen.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Boolesch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: PromotionalTabsEnabled
  - Gruppenrichtlinienname: Tabfüllende Werbeinhalte ermöglichen
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: PromotionalTabsEnabled
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000000
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: PromotionalTabsEnabled
  - Beispielwert:
``` xml
<false/>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### PromptForDownloadLocation
  #### Fragen, wo heruntergeladene Dateien gespeichert werden sollen
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Legen Sie fest, ob vor dem Herunterladen gefragt wird, wo eine Datei gespeichert werden soll.

Wenn Sie diese Richtlinie aktivieren, wird der Benutzer vor dem Herunterladen gefragt, wo jede einzelne Datei gespeichert werden soll. Wenn Sie dies nicht konfigurieren, werden die Dateien automatisch am Standardspeicherort gespeichert, ohne dass der Benutzer gefragt wird.

Wenn Sie diese Richtlinie nicht konfigurieren, kann der Benutzer diese Einstellung ändern.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Boolesch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: PromptForDownloadLocation
  - Gruppenrichtlinienname: Fragen, wo heruntergeladene Dateien gespeichert werden sollen
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: PromptForDownloadLocation
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000000
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: PromptForDownloadLocation
  - Beispielwert:
``` xml
<false/>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### QuicAllowed
  #### QUIC-Protokoll zulassen
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Ermöglicht die Verwendung des QUIC-Protokolls in Microsoft Edge.

Wenn Sie diese Richtlinie aktivieren oder nicht konfigurieren, wird das QUIC-Protokoll zugelassen.

Wenn Sie diese Richtlinie deaktivieren, wird das QUIC-Protokoll blockiert.

QUIC ist ein Transportschicht-Netzwerkprotokoll, das die Leistung von Webanwendungen verbessern kann, die derzeit TCP verwenden.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Nein - Erfordert einen Neustart des Browsers

  #### Datentyp:
  Boolesch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: QuicAllowed
  - Gruppenrichtlinienname: QUIC-Protokoll zulassen
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: QuicAllowed
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000001
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: QuicAllowed
  - Beispielwert:
``` xml
<true/>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### RelaunchNotification
  #### Einen Benutzer benachrichtigen, dass ein Neustart des Browsers für ausstehende Updates empfohlen wird oder erforderlich ist
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Benachrichtigt Benutzer, dass sie Microsoft Edge neu starten müssen, um ein ausstehendes Update anzuwenden.

Wenn Sie diese Richtlinie nicht konfigurieren, fügt Microsoft Edge ein Wiederherstellungssymbol ganz rechts in der oberen Menüleiste ein, um den Benutzer aufzufordern, den Browser neu zu starten, damit das Update angewendet werden kann.

Wenn Sie diese Richtlinie aktivieren und auf "Empfohlen" (1) einstellen, werden die Benutzer durch eine wiederkehrende Warnung aufgefordert, einen Neustart auszuführen. Benutzer können diese Warnung ablehnen und den Neustart verschieben.

Wenn Sie die Richtlinie auf "Erforderlich" (2) festlegen, fordert eine wiederkehrende Warnung die Benutzer auf, den Browser automatisch neu zu starten, sobald ein Benachrichtigungszeitraum abgelaufen ist. Der Standardzeitraum beträgt sieben Tage. Sie können diesen Zeitraum mit der Richtlinie [RelaunchNotificationPeriod](#relaunchnotificationperiod) konfigurieren.

Die Sitzung des Benutzers wird beim Neustart des Browsers wiederhergestellt.

* Empfohlen (1) = Dem Benutzer wird in einer wiederkehrenden Meldung angezeigt, dass ein Neustart erfolgen sollte.

* Erforderlich (2) = Dem Benutzer wird in einer wiederkehrenden Meldung angezeigt, dass ein Neustart erforderlich ist.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Ganze Zahl

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: RelaunchNotification
  - Gruppenrichtlinienname: Einen Benutzer benachrichtigen, dass ein Neustart des Browsers für ausstehende Updates empfohlen wird oder erforderlich ist
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: RelaunchNotification
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000001
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: RelaunchNotification
  - Beispielwert:
``` xml
<integer>1</integer>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### RelaunchNotificationPeriod
  #### Zeitraum für Aktualisierungsbenachrichtigungen festlegen
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Allows you to set the time period, in milliseconds, over which users are notified that Microsoft Edge must be relaunched or that a Microsoft Edge OS device must be restarted to apply a pending update.

Over this time period, the user will be repeatedly informed of the need for an update. For Microsoft Edge OS devices, a restart notification appears in the system tray according to the RelaunchHeadsUpPeriod policy. For Microsoft Edge browsers, the app menu changes to indicate that a relaunch is needed once one third of the notification period passes. This notification changes color once two thirds of the notification period passes, and again once the full notification period has passed. The additional notifications enabled by the RelaunchNotification policy follow this same schedule.

If not set, the default period of 604800000 milliseconds (one week) is used.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Ganze Zahl

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: RelaunchNotificationPeriod
  - Gruppenrichtlinienname: Zeitraum für Aktualisierungsbenachrichtigungen festlegen
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: RelaunchNotificationPeriod
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x240c8400
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: RelaunchNotificationPeriod
  - Beispielwert:
``` xml
<integer>604800000</integer>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### RendererCodeIntegrityEnabled
  #### Renderercodeintegrität aktivieren
  >Unterstützte Versionen: Microsoft Edge unter Windows seit Version 78 oder höher

  #### Beschreibung
  Wenn diese Richtlinie aktiviert oder nicht definiert ist, wird die Renderercodeintegrität aktiviert. Diese Richtlinie sollte nur deaktiviert werden, wenn Kompatibilitätsprobleme mit Software von Drittanbietern auftreten, die innerhalb der Rendererprozesse von Microsoft Edge ausgeführt werden.

Das Deaktivieren dieser Richtlinie hat nachteilige Auswirkungen auf die Sicherheit und Stabilität von Microsoft Edge, da unbekannter und potentiell schädlicher Code innerhalb der Rendererprozesse von Microsoft Edge geladen werden kann.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Nein - Erfordert einen Neustart des Browsers

  #### Datentyp:
  Boolesch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: RendererCodeIntegrityEnabled
  - Gruppenrichtlinienname: Renderercodeintegrität aktivieren
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: RendererCodeIntegrityEnabled
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000000
```


  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### RequireOnlineRevocationChecksForLocalAnchors
  #### Geben Sie an, ob für lokale Vertrauensanker Online-OCSP/CRL-Überprüfungen erforderlich sind.
  >Unterstützte Versionen: Microsoft Edge unter Windows seit Version 77 oder höher

  #### Beschreibung
  Steuern Sie, ob Online Sperrüberprüfungen (OCSP/Zertifikatsperrlisten-Überprüfungen) erforderlich sind. Wenn Microsoft Edge keine Sperrstatusinformationen erhalten kann, werden diese Zertifikate als gesperrt behandelt ("harter Fehler").

Wenn Sie diese Richtlinie aktivieren, führt Microsoft Edge immer eine Sperrüberprüfung für Serverzertifikate durch, die erfolgreich überprüft werden und durch lokal installierte Zertifizierungsstellenzertifikate signiert sind.

Wenn Sie diese Richtlinie nicht konfigurieren oder deaktivieren, verwendet Microsoft Edge die vorhandenen Einstellungen für die Online-Sperrüberprüfung.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Boolesch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: RequireOnlineRevocationChecksForLocalAnchors
  - Gruppenrichtlinienname: Geben Sie an, ob für lokale Vertrauensanker Online-OCSP/CRL-Überprüfungen erforderlich sind.
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: RequireOnlineRevocationChecksForLocalAnchors
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000000
```


  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### ResolveNavigationErrorsUseWebService
  #### Auflösung von Navigationsfehlern mithilfe eines Webdienstes aktivieren
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Erlaubt Microsoft Edge, eine datenlose Verbindung zu einem Webservice herzustellen, um Netzwerke auf Konnektivität zu prüfen, beispielsweise die WLAN-Verbindung in Hotels und Flughäfen.

Wenn Sie diese Richtlinie aktivieren, wird ein Webservice für Tests der Netzwerkverbindung verwendet.

Wenn Sie diese Richtlinie deaktivieren, verwendet Microsoft Edge native APIs, um Probleme mit der Netzwerkverbindung und der Navigation zu beheben.

**Hinweis**: Mit Ausnahme von Windows 8 und späteren Versionen von Windows verwendet Microsoft Edge *immer* native APIs, um Verbindungsprobleme zu lösen.

Wenn Sie diese Richtlinie nicht konfigurieren, verwendet Microsoft Edge die Benutzereinstellung, die für Dienste unter edge://settings/privacy festgelegt ist.
Es gibt einen **Einen Webservice verwenden, um Navigationsfehler zu beheben**-Schalter, den der Benutzer ein- und ausschalten kann. Beachten Sie: Wenn Sie diese Richtlinie (ResolveNavigationErrorsUseWebService) aktiviert haben, ist die Einstellung **Einen Webservice verwenden, um Navigationsfehler zu beheben** aktiviert, aber der Benutzer kann die Einstellung nicht mit Hilfe des Umschalters ändern. Wenn Sie diese Richtlinie deaktiviert haben, wird die Einstellung **Einen Webservice verwenden, um Navigationsfehler zu beheben** deaktiviert, und der Benutzer kann die Einstellung nicht mit dem Umschalter ändern.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Ja
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Boolesch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: ResolveNavigationErrorsUseWebService
  - Gruppenrichtlinienname: Auflösung von Navigationsfehlern mithilfe eines Webdienstes aktivieren
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Administrative Vorlagen/Microsoft Edge - Standardeinstellungen (können durch Benutzer überschrieben werden)/
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): SOFTWARE\Policies\Microsoft\Edge\Empfohlen
  - Wertname: ResolveNavigationErrorsUseWebService
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000001
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: ResolveNavigationErrorsUseWebService
  - Beispielwert:
``` xml
<true/>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### RestrictSigninToPattern
  #### Beschränken der Konten, die als primäre Microsoft Edge-Konten verwendet werden können
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Legt fest, welche Konten in Microsoft Edge als primäre Browser-Konten festgelegt werden können (das Konto, das während des Synchronisierungs-Opt-in-Ablaufs ausgewählt wird).

Wenn ein Benutzer versucht, ein primäres Browser-Konto mit einem Benutzernamen festzulegen, der nicht mit diesem Muster übereinstimmt, wird er blockiert, und es wird eine entsprechende Fehlermeldung angezeigt.

Wenn Sie diese Richtlinie nicht konfigurieren oder leer lassen, können Benutzer in Microsoft Edge ein beliebiges Konto als primäres Browser-Konto festlegen.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Zeichenfolge

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: RestrictSigninToPattern
  - Gruppenrichtlinienname: Beschränken der Konten, die als primäre Microsoft Edge-Konten verwendet werden können
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: RestrictSigninToPattern
  - Werttyp: REG_SZ
  ##### Beispielwert:
```
".*@contoso.com"
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: RestrictSigninToPattern
  - Beispielwert:
``` xml
<string>.*@contoso.com</string>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### RunAllFlashInAllowMode
  #### Adobe Flash-Inhaltseinstellung auf alle Inhalte erweitern
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Wenn Sie diese Richtlinie aktivieren, werden alle Adobe Flash-Inhalte ausgeführt, die in Websites eingebettet sind, deren Inhaltseinstellungen (vom Benutzer oder über eine Unternehmensrichtlinie festgelegt)Adobe Flash zulassen. Dazu gehören auch Inhalte anderer Herkunft und/oder kleine Inhalte.

Informationen darüber, wie Sie steuern können, welche Websites Adobe Flash ausführen dürfen, finden Sie in den Spezifikationen der Richtlinien [DefaultPluginsSetting](#defaultpluginssetting), [PluginsAllowedForUrls](#pluginsallowedforurls) und [PluginsBlockedForUrls](#pluginsblockedforurls).

Wenn Sie diese Richtlinie deaktivieren oder nicht konfigurieren, können Adobe Flash-Inhalte aus anderen Quellen (von Websites, die nicht in den drei oben genannten Richtlinien aufgeführt sind) oder kleine Inhalte blockiert werden.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Boolesch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: RunAllFlashInAllowMode
  - Gruppenrichtlinienname: Adobe Flash-Inhaltseinstellung auf alle Inhalte erweitern
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: RunAllFlashInAllowMode
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000001
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: RunAllFlashInAllowMode
  - Beispielwert:
``` xml
<true/>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### SSLErrorOverrideAllowed
  #### Zulassen, dass Benutzer von der HTTPS-Warnungsseite aus fortfahren können
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Microsoft Edge zeigt eine Warnungsseite an, wenn Benutzer Websites mit SSL-Fehlern besuchen.

Wenn Sie diese Richtlinie aktivieren oder nicht konfigurieren (Standardeinstellung), können Benutzer durch diese Warnungsseiten klicken.

Wenn Sie diese Richtlinie deaktivieren, können Benutzer sich nicht durch eine Warnungsseite klicken.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Boolesch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: SSLErrorOverrideAllowed
  - Gruppenrichtlinienname: Zulassen, dass Benutzer von der HTTPS-Warnungsseite aus fortfahren können
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: SSLErrorOverrideAllowed
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000001
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: SSLErrorOverrideAllowed
  - Beispielwert:
``` xml
<true/>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### SSLVersionMin
  #### Mindestversion von TLS aktiviert
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Legt die minimale unterstützte SSL-Version fest. Wenn Sie diese Richtlinie nicht konfigurieren, verwendet Microsoft Edge die standardmäßige Minimalversion TLS 1.0.

Wenn Sie diese Richtlinie aktivieren, können Sie die minimale Version auf einen der folgenden Werte festlegen: „tls1“, „tls1.1“ oder „tls1.2“. Wenn festgelegt, verwendet Microsoft Edge keine SSL/TLS-Version, die niedriger als die angegebene Version ist. Unbekannte Werte werden ignoriert.

* "tls1" = TLS 1.0

* "tls1.1" = TLS 1.1

* "tls1.2" = TLS 1.2

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Zeichenfolge

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: SSLVersionMin
  - Gruppenrichtlinienname: Mindestversion von TLS aktiviert
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: SSLVersionMin
  - Werttyp: REG_SZ
  ##### Beispielwert:
```
"tls1"
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: SSLVersionMin
  - Beispielwert:
``` xml
<string>tls1</string>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### SavingBrowserHistoryDisabled
  #### Speichern des Browserverlaufs deaktivieren
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Deaktiviert das Speichern des Browserverlaufs und verhindert, dass Benutzer diese Einstellung ändern.

Wenn Sie diese Richtlinie aktivieren, wird der Browserverlauf nicht gespeichert, und auch die Tabsynchronisierung wird deaktiviert.

Wenn Sie diese Richtlinie deaktivieren oder nicht konfigurieren, wird der Browserverlauf gespeichert.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Boolesch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: SavingBrowserHistoryDisabled
  - Gruppenrichtlinienname: Speichern des Browserverlaufs deaktivieren
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: SavingBrowserHistoryDisabled
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000001
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: SavingBrowserHistoryDisabled
  - Beispielwert:
``` xml
<true/>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### SearchSuggestEnabled
  #### Suchvorschläge aktivieren
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Aktiviert Websuchvorschläge auf der Adressleiste und in der Liste mit automatischen Vorschlägen von Microsoft Edge und verhindert, dass Benutzer diese Richtlinie ändern.

Wenn Sie diese Richtlinie aktivieren, werden Websuchvorschläge verwendet.

Wenn Sie diese Richtlinie deaktivieren, werden keine Websuchvorschläge verwendet. Vorschläge aus dem lokalen Verlauf und aus den lokalen Favoriten werden jedoch weiterhin angezeigt. Außerdem werden weder die eingegebenen Zeichen noch die besuchten URLs in die an Microsoft übermittelten Telemetriedaten eingeschlossen.

Wenn Sie diese Richtlinie nicht festlegen, sind Suchvorschläge aktiviert. Dies kann jedoch vom Benutzer geändert werden.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Ja
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Boolesch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: SearchSuggestEnabled
  - Gruppenrichtlinienname: Suchvorschläge aktivieren
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Administrative Vorlagen/Microsoft Edge - Standardeinstellungen (können durch Benutzer überschrieben werden)/
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): SOFTWARE\Policies\Microsoft\Edge\Empfohlen
  - Wertname: SearchSuggestEnabled
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000001
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: SearchSuggestEnabled
  - Beispielwert:
``` xml
<true/>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### SecurityKeyPermitAttestation
  #### Websites oder Domänen, die keine Berechtigung zur Verwendung des direkten Sicherheitsschlüssel-Nachweises benötigen
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Gibt Websites und Domänen an, die keine explizite Benutzerberechtigung benötigen, wenn Nachweiszertifikate von Sicherheitsschlüsseln angefordert werden. Zusätzlich wird ein Signal an den Sicherheitsschlüssel gesendet, das angibt, dass es einen individuellen Nachweis verwenden kann. Ohne dies werden Benutzer jedes Mal aufgefordert, wenn eine Website Nachweise für Sicherheitsschlüssel anfordert.

Websites (z. B. https://contoso.com/some/path) stimmen nur als U2F-appIDs überein. Domänen (z. B. contoso.com) stimmen nur mit den webauthn-RP-IDs überein. Sie müssen sowohl die appID-URL als auch die Domäne auflisten, um U2F- und webauthn-APIs für eine bestimmte Website zu erfassen.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Liste der Zeichenfolgen

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: SecurityKeyPermitAttestation
  - Gruppenrichtlinienname: Websites oder Domänen, die keine Berechtigung zur Verwendung des direkten Sicherheitsschlüssel-Nachweises benötigen
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge\SecurityKeyPermitAttestation
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: 1, 2, 3, ...
  - Werttyp: Liste von REG_SZ
  ##### Beispielwert:
```
SOFTWARE\Policies\Microsoft\Edge\SecurityKeyPermitAttestation\0 = "https://contoso.com"

```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: SecurityKeyPermitAttestation
  - Beispielwert:
``` xml
<array>
  <string>https://contoso.com</string>
</array>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### SendIntranetToInternetExplorer
  #### Alle Intranetsites an Internet Explorer senden
  >Unterstützte Versionen: Microsoft Edge unter Windows seit Version 77 oder höher

  #### Beschreibung
  Anleitungen zum Konfigurieren der optimalen Benutzeroberfläche für den Internet Explorer-Modus finden Sie unter "[https://go.microsoft.com/fwlink/?linkid=2094210](https://go.microsoft.com/fwlink/?linkid=2094210)".

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Nein - Erfordert einen Neustart des Browsers

  #### Datentyp:
  Boolesch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: SendIntranetToInternetExplorer
  - Gruppenrichtlinienname: Alle Intranetsites an Internet Explorer senden
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: SendIntranetToInternetExplorer
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000001
```


  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### SendSiteInfoToImproveServices
  #### Websiteinformationen zur Verbesserung von Microsoft-Diensten senden
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Bei den Beta- und Stable-Kanälen von Windows 10 von Microsoft Edge überschreibt diese Richtlinie (falls konfiguriert) die Einstellung für die Windows-Diagnosedaten zur Erfassung bzw. Nicht-Erfassung von Microsoft Edge-Browsinginformationen auf Websites ([https://go.microsoft.com/fwlink/?linkid=2099569](https://go.microsoft.com/fwlink/?linkid=2099569)).

Anhand dieser Richtlinieneinstellung können Sie entscheiden, ob Benutzer Informationen zu Websites, die sie in Microsoft Edge besuchen, an Microsoft senden können, um Dienste wie die Suche zu verbessern.

Wenn Sie diese Richtlinie aktivieren, werden Informationen zu Websites, die Sie in Microsoft Edge aufgerufen haben, an Microsoft gesendet.

Wenn Sie diese Richtlinie deaktivieren, werden Informationen zu Websites, die Sie in Microsoft Edge aufgerufen haben, nicht an Microsoft gesendet.

In den Beta- und Stable-Kanälen von Windows 10 wird durch diese Richtlinie das Senden von Informationen zu Websitebesuchen von Benutzern gesteuert. Wenn diese Richtlinie nicht konfiguriert ist, ist in Microsoft Edge die Standardeinstellung für Windows-Diagnosedaten festgelegt.

In den Canary- und Dev-Kanälen von Windows 10, wird durch diese Richtlinie das Senden von Informationen zu Websitebesuchen von Benutzern gesteuert. Wenn diese Richtlinie nicht konfiguriert ist, ist in Microsoft Edge standardmäßig die Einstellung des Benutzers festgelegt.

Unter Windows 7, 8 und Mac wird durch diese Richtlinie das Senden von Informationen zu Websitebesuchen von Benutzern gesteuert. Wenn diese Richtlinie nicht konfiguriert ist, ist in Microsoft Edge standardmäßig die Einstellung des Benutzers festgelegt.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Nein - Erfordert einen Neustart des Browsers

  #### Datentyp:
  Boolesch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: SendSiteInfoToImproveServices
  - Gruppenrichtlinienname: Websiteinformationen zur Verbesserung von Microsoft-Diensten senden
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: SendSiteInfoToImproveServices
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000000
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: SendSiteInfoToImproveServices
  - Beispielwert:
``` xml
<false/>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### ShowOfficeShortcutInFavoritesBar
  #### Microsoft Office-Verknüpfung in der Favoritenleiste anzeigen
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Gibt an, ob in der Favoritenleiste eine Verknüpfung mit Office.com eingefügt werden soll. Benutzer, die bei Microsoft Edge angemeldet sind, werden von der Verknüpfung zu ihren Microsoft Office-Apps und -Dokumenten weitergeleitet.

Wenn diese Richtlinie aktiviert oder nicht konfiguriert ist, können Benutzer im Kontextmenü der Favoritenleiste wählen, ob die Verknüpfung angezeigt werden soll.

Wenn die Richtlinie deaktiviert ist, wird die Verknüpfung nicht angezeigt.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Boolesch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: ShowOfficeShortcutInFavoritesBar
  - Gruppenrichtlinienname: Microsoft Office-Verknüpfung in der Favoritenleiste anzeigen
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: ShowOfficeShortcutInFavoritesBar
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000000
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: ShowOfficeShortcutInFavoritesBar
  - Beispielwert:
``` xml
<false/>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### SignedHTTPExchangeEnabled
  #### Unterstützung des signierten HTTP-Austauschs (SXG) aktivieren
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 78 oder höher

  #### Beschreibung
  Aktivieren Sie die Unterstützung für Signed HTTP Exchange (SXG).

Wenn diese Richtlinie nicht festgelegt oder aktiviert ist, akzeptiert Microsoft Edge Webinhalte, die als Signed HTTP Exchanges bereitgestellt werden.

Wenn diese Richtlinie deaktiviert ist, können Signed HTTP Exchanges nicht geladen werden.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Boolesch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: SignedHTTPExchangeEnabled
  - Gruppenrichtlinienname: Unterstützung des signierten HTTP-Austauschs (SXG) aktivieren
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: SignedHTTPExchangeEnabled
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000001
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: SignedHTTPExchangeEnabled
  - Beispielwert:
``` xml
<true/>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### SitePerProcess
  #### Websiteisolation für jede Website aktivieren
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Die Richtlinie 'SitePerProcess' kann verwendet werden, um zu verhindern, dass Benutzer das Standardverhalten der Isolierung aller Sites abwählen. Beachten Sie, dass Sie auch die Richtlinie [IsolateOrigins](#isolateorigins) verwenden können, um zusätzliche Quellen feiner zu isolieren.
Wenn Sie diese Richtlinie aktivieren, können Benutzer das Standardverhalten, bei dem jede Website in ihrem eigenen Prozess ausgeführt wird, nicht abwählen.
Wenn Sie diese Richtlinie deaktivieren oder nicht konfigurieren, kann ein Benutzer die Isolierung der Website deaktivieren. (zum Beispiel durch Verwendung des Eintrags "Website-Isolierung deaktivieren" in edge://flags). Das Deaktivieren der Richtlinie oder das Nichtkonfigurieren der Richtlinie schaltet die Website-Isolierung nicht aus.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Nein - Erfordert einen Neustart des Browsers

  #### Datentyp:
  Boolesch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: SitePerProcess
  - Gruppenrichtlinienname: Websiteisolation für jede Website aktivieren
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: SitePerProcess
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000001
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: SitePerProcess
  - Beispielwert:
``` xml
<true/>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### SpellcheckEnabled
  #### Rechtschreibprüfung aktivieren
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Wenn Sie diese Richtlinie aktivieren oder nicht konfigurieren, kann der Benutzer die Rechtschreibprüfung verwenden.

Wenn Sie diese Richtlinie deaktivieren, kann der Benutzer die Rechtschreibprüfung nicht verwenden und die Richtlinien [SpellcheckLanguage](#spellchecklanguage) und [SpellcheckLanguageBlocklist](#spellchecklanguageblocklist) sind ebenfalls deaktiviert.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Boolesch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: SpellcheckEnabled
  - Gruppenrichtlinienname: Rechtschreibprüfung aktivieren
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: SpellcheckEnabled
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000000
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: SpellcheckEnabled
  - Beispielwert:
``` xml
<false/>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### SpellcheckLanguage
  #### Spezifische Sprachen für die Rechtschreibprüfung aktivieren
  >Unterstützte Versionen: Microsoft Edge unter Windows seit Version 77 oder höher

  #### Beschreibung
  Aktiviert verschiedene Sprachen für die Rechtschreibprüfung. Jede angegebene Sprache, die nicht erkannt wird, wird ignoriert.

Wenn Sie diese Richtlinie aktivieren, wird die Rechtschreibprüfung für die angegebenen Sprachen aktiviert sowie für alle Sprachen, die der Benutzer aktiviert hat.

Wenn Sie diese Richtlinie nicht konfigurieren oder deaktivieren, werden die Einstellungen des Benutzers für die Rechtschreibprüfung nicht geändert.

Wenn die Richtlinie [SpellcheckEnabled](#spellcheckenabled) deaktiviert ist, hat diese Richtlinie keine Wirkung.

Wenn eine Sprache sowohl in der Richtlinie SpellcheckLanguage' als auch in der Richtlinie [SpellcheckLanguageBlocklist](#spellchecklanguageblocklist) angegeben ist, wird die Sprache der Rechtschreibprüfung aktiviert.

Die unterstützten Sprachen sind: af, bg, ca, cs, cy, da, de, el, en-AU, en-CA, en-GB, en-US, es, es-419, es-AR, es-ES, es-MX, es-US, et, fa, fo, fr, he, hi, hr, hu, id, it, ko, lt, lv, nb, nl, pl, pt-BR, pt-PT, ro, ru, sh, sk, sl, sq, sr, sv, ta, tg, tr, uk, vi.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Liste der Zeichenfolgen

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: SpellcheckLanguage
  - Gruppenrichtlinienname: Spezifische Sprachen für die Rechtschreibprüfung aktivieren
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge\SpellcheckLanguage
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: 1, 2, 3, ...
  - Werttyp: Liste von REG_SZ
  ##### Beispielwert:
```
SOFTWARE\Policies\Microsoft\Edge\SpellcheckLanguage\0 = "fr"
SOFTWARE\Policies\Microsoft\Edge\SpellcheckLanguage\1 = "es"

```


  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### SpellcheckLanguageBlocklist
  #### Deaktivierung von Sprachen für die Rechtschreibprüfung erzwingen
  >Unterstützte Versionen: Microsoft Edge unter Windows seit Version 78 oder höher

  #### Beschreibung
  Deaktiviert zwangsweise die Rechtschreibprüfung für Sprachen. Nicht erkannte Sprachen in dieser Liste werden ignoriert.

Wenn Sie diese Richtlinie aktivieren, wird die Rechtschreibprüfung für die angegebenen Sprachen deaktiviert. Der Benutzer kann die Rechtschreibprüfung für Sprachen, die nicht in der Liste enthalten sind, weiterhin aktivieren oder deaktivieren.

Wenn Sie diese Richtlinie nicht festlegen oder deaktivieren, ändert sich nichts an den Einstellungen des Benutzers für die Rechtschreibprüfung.

Wenn die Richtlinie [SpellcheckEnabled](#spellcheckenabled) deaktiviert ist, hat diese Richtlinie keine Wirkung.

Wenn eine Sprache sowohl in der Richtlinie [SpellcheckLanguage](#spellchecklanguage) als auch in der Richtlinie 'SpellcheckLanguageBlocklist' enthalten ist, wird die Rechtschreibprüfung der Sprache aktiviert.

Die derzeit unterstützten Sprachen sind: af, bg, ca, cs, da, de, el, en-AU, en-CA, en-GB, en-US, es, es-419, es-AR, es-ES, es-MX, es-US, et, fa, fo, fr, he, hi, hr, hu, id, it, ko, lt, lv, nb, nl, pl, pt-BR, pt-PT, ro, ru, sh, sk, sl, sq, sr, sv, ta, tg, tr, uk, vi.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Liste der Zeichenfolgen

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: SpellcheckLanguageBlocklist
  - Gruppenrichtlinienname: Deaktivierung von Sprachen für die Rechtschreibprüfung erzwingen
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge\SpellcheckLanguageBlocklist
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: 1, 2, 3, ...
  - Werttyp: Liste von REG_SZ
  ##### Beispielwert:
```
SOFTWARE\Policies\Microsoft\Edge\SpellcheckLanguageBlocklist\0 = "fr"
SOFTWARE\Policies\Microsoft\Edge\SpellcheckLanguageBlocklist\1 = "es"

```


  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### SuppressUnsupportedOSWarning
  #### Nicht unterstützte Betriebssystemwarnung unterdrücken
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Unterdrückt die Warnung, die angezeigt wird, wenn Microsoft Edge auf einem nicht mehr unterstützten Computer oder Betriebssystem ausgeführt wird.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Nein - Erfordert einen Neustart des Browsers

  #### Datentyp:
  Boolesch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: SuppressUnsupportedOSWarning
  - Gruppenrichtlinienname: Nicht unterstützte Betriebssystemwarnung unterdrücken
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: SuppressUnsupportedOSWarning
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000001
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: SuppressUnsupportedOSWarning
  - Beispielwert:
``` xml
<true/>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### SyncDisabled
  #### Synchronisierung von Daten mit Microsoft-Synchronisierungsdiensten deaktivieren
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Deaktiviert das Synchronisieren von Daten Microsoft Edge und verhindert, dass Benutzer diese Einstellung ändern.

Wenn diese Richtlinie nicht festgelegt ist, können Benutzer die Synchronisierung entweder ein- oder ausschalten.

Aktivieren Sie diese Richtlinie nicht, wenn die Richtlinie 'RoamingProfileSupportEnabled' aktiviert ist, da 'RoamingProfileSupportEnabled' die Synchronisierungsfunktionalität dupliziert.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Ja
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Boolesch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: SyncDisabled
  - Gruppenrichtlinienname: Synchronisierung von Daten mit Microsoft-Synchronisierungsdiensten deaktivieren
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Administrative Vorlagen/Microsoft Edge - Standardeinstellungen (können durch Benutzer überschrieben werden)/
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): SOFTWARE\Policies\Microsoft\Edge\Empfohlen
  - Wertname: SyncDisabled
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000001
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: SyncDisabled
  - Beispielwert:
``` xml
<true/>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### TabFreezingEnabled
  #### Einfrieren von Hintergrundtabs zulassen
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 79 oder höher

  #### Beschreibung
  Hiermit können Sie steuern, ob mit Microsoft Edge das Einfrieren von Tabs möglich ist, die sich seit mindestens fünf Minuten im Hintergrund befinden.

Durch das Einfrieren von Tabs wird der Verbrauch von CPU-, Akku- und Arbeitsspeicherressourcen reduziert. Microsoft Edge nutzt Heuristik, um das Einfrieren von Tabs zu verhindern, auf denen im Hintergrund nützliche Vorgänge durchgeführt werden, z. B. Anzeigen von Benachrichtigungen, Wiedergeben von Sound und Streamen von Videos.

Wenn Sie diese Richtlinie aktivieren oder nicht konfigurieren, werden Tabs eingefroren, die sich seit mindestens fünf Minuten im Hintergrund befinden.

Wenn Sie diese Richtlinie deaktivieren, werden keine Tabs eingefroren.


  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Boolesch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: TabFreezingEnabled
  - Gruppenrichtlinienname: Einfrieren von Hintergrundtabs zulassen
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: TabFreezingEnabled
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000000
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: TabFreezingEnabled
  - Beispielwert:
``` xml
<false/>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### TaskManagerEndProcessEnabled
  #### Beenden von Prozessen im Browser-Task-Manager ermöglichen
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Wenn Sie diese Richtlinie aktivieren oder nicht konfigurieren, können Benutzer Prozesse im Browser-Task-Manager beenden. Wenn Sie die Richtlinie deaktivieren, können Benutzer keine Prozesse beenden, und die Schaltfläche „Prozess beenden“ ist im Browser-Task-Manager deaktiviert.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Boolesch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: TaskManagerEndProcessEnabled
  - Gruppenrichtlinienname: Beenden von Prozessen im Browser-Task-Manager ermöglichen
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: TaskManagerEndProcessEnabled
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000001
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: TaskManagerEndProcessEnabled
  - Beispielwert:
``` xml
<true/>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### TrackingPrevention
  #### Blockieren der Nachverfolgung der Webbrowsing-Aktivitäten von Benutzern
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 78 oder höher

  #### Beschreibung
  Hiermit können Sie entscheiden, ob Websites daran gehindert werden sollen, die Webbrowsing-Aktivitäten von Benutzern zu verfolgen.

Wenn Sie diese Richtlinie aktivieren, haben Sie die folgenden Optionen zum Festlegen der Stufe der Tracking-Verhinderung:

0 = Aus (keine Tracking-Verhinderung)
1 = Grundlegend (blockiert schädliche Tracker, Inhalte und Anzeigen werden personalisiert)
2 = Ausgeglichen (blockiert schädliche Tracker und Tracker von Websites, die der Benutzer nicht besucht hat; Inhalte und Anzeigen werden weniger personalisiert)
3 = Streng (blockiert schädliche Tracker und den Großteil der Tracker von allen Websites; Inhalte und Anzeigen weisen eine minimale Personalisierung auf; einige Teile von Websites funktionieren möglicherweise nicht)

Wenn Sie diese Richtlinie deaktivieren oder nicht konfigurieren, können Benutzer ihre eigene Ebene der Tracking-Verhinderung festlegen.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Ganze Zahl

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: TrackingPrevention
  - Gruppenrichtlinienname: Blockieren der Nachverfolgung der Webbrowsing-Aktivitäten von Benutzern
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: TrackingPrevention
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000002
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: TrackingPrevention
  - Beispielwert:
``` xml
<integer>2</integer>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### TranslateEnabled
  #### Übersetzung aktivieren
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Aktiviert den integrierten Microsoft-Übersetzungsdienst in Microsoft Edge.

Wenn Sie diese Richtlinie aktivieren, bietet Microsoft Edge dem Benutzer eine Übersetzungsfunktion in Form eines integrierten Übersetzungs-Flyouts (sofern geeignet) sowie eine Übersetzungsoption im Rechtsklick-Kontextmenü.

Deaktivieren Sie diese Richtlinie, um sämtliche integrierten Übersetzungsfeatures zu deaktivieren.

Wenn Sie die Richtlinie nicht konfigurieren, können Benutzer wählen, ob sie die Übersetzungsfunktion verwenden möchten.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Ja
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Boolesch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: TranslateEnabled
  - Gruppenrichtlinienname: Übersetzung aktivieren
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Administrative Vorlagen/Microsoft Edge - Standardeinstellungen (können durch Benutzer überschrieben werden)/
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): SOFTWARE\Policies\Microsoft\Edge\Empfohlen
  - Wertname: TranslateEnabled
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000001
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: TranslateEnabled
  - Beispielwert:
``` xml
<true/>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### URLAllowlist
  #### Liste zulässiger URLs definieren
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Ermöglicht Zugriff auf die aufgelisteten URLs als Ausnahmen von der URL-Blockierungsliste.

Formatieren Sie die URL-Muster gemäß [https://go.microsoft.com/fwlink/?linkid=2095322](https://go.microsoft.com/fwlink/?linkid=2095322).

Mit dieser Richtlinie können Sie Ausnahmen zu restriktiven Blockierungslisten öffnen. Sie können beispielsweise "*" in die Blockierungsliste aufnehmen, um alle Anfragen zu blockieren, und dann diese Richtlinie verwenden, um den Zugriff auf eine begrenzte Liste von URLs zu ermöglichen. Mit dieser Richtlinie können Sie Ausnahmen für bestimmte Systeme, Subdomänen anderer Domänen, Ports oder bestimmte Pfade öffnen.

Der spezifischste Filter bestimmt, ob eine URL blockiert oder erlaubt ist. Die zulässige Liste hat Vorrang vor der Blockierungsliste.

Diese Richtlinie ist auf 1000 Einträge begrenzt; nachfolgende Einträge werden ignoriert.

Wenn Sie diese Richtlinie nicht konfigurieren, gibt es keine Ausnahmen von der Blockierungsliste in der Richtlinie [URLBlocklist](#urlblocklist).

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Liste der Zeichenfolgen

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: URLAllowlist
  - Gruppenrichtlinienname: Liste zulässiger URLs definieren
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge\URLAllowlist
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: 1, 2, 3, ...
  - Werttyp: Liste von REG_SZ
  ##### Beispielwert:
```
SOFTWARE\Policies\Microsoft\Edge\URLAllowlist\0 = "contoso.com"
SOFTWARE\Policies\Microsoft\Edge\URLAllowlist\1 = "https://ssl.server.com"
SOFTWARE\Policies\Microsoft\Edge\URLAllowlist\2 = "hosting.com/good_path"
SOFTWARE\Policies\Microsoft\Edge\URLAllowlist\3 = "https://server:8080/path"
SOFTWARE\Policies\Microsoft\Edge\URLAllowlist\4 = ".exact.hostname.com"

```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: URLAllowlist
  - Beispielwert:
``` xml
<array>
  <string>contoso.com</string>
  <string>https://ssl.server.com</string>
  <string>hosting.com/good_path</string>
  <string>https://server:8080/path</string>
  <string>.exact.hostname.com</string>
</array>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### URLBlocklist
  #### Zugriff auf eine Liste von URLs blockieren
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Definiert basierend auf URL-Mustern eine Liste von Sites, die blockiert sind (der Benutzer kann sie nicht laden).

Formatieren Sie die URL-Muster gemäß [https://go.microsoft.com/fwlink/?linkid=2095322](https://go.microsoft.com/fwlink/?linkid=2095322).

Sie können in der Richtlinie [URLAllowlist](#urlallowlist) Ausnahmen definieren. Diese Richtlinien sind auf 1000 Einträge begrenzt; nachfolgende Einträge werden ignoriert.

Beachten Sie: Das Blockieren von internen 'edge://*'-URLs wird nicht empfohlen, weil es zu unerwarteten Fehlern führen kann.

Diese Richtlinie verhindert nicht, dass die Seite dynamisch durch JavaScript aktualisiert wird. Wenn Sie beispielsweise 'contoso.com/abc' blockieren, können Benutzer möglicherweise immer noch 'contoso.com' besuchen und auf einen Link klicken, um 'contoso.com/abc' aufzurufen, solange die Seite nicht aktualisiert wird.

Wenn Sie diese Richtlinie nicht konfigurieren, werden keine URLs blockiert.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Liste der Zeichenfolgen

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: URLBlocklist
  - Gruppenrichtlinienname: Zugriff auf eine Liste von URLs blockieren
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge\URLBlocklist
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: 1, 2, 3, ...
  - Werttyp: Liste von REG_SZ
  ##### Beispielwert:
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


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: URLBlocklist
  - Beispielwert:
``` xml
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
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### UserDataDir
  #### Benutzerdatenverzeichnis festlegen
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Konfiguriert das Verzeichnis, das zum Speichern von Benutzerdaten verwendet werden soll.

Wenn Sie diese Richtlinie aktivieren, verwendet Microsoft Edge das angegebene Verzeichnis, unabhängig davon, ob der Benutzer das Befehlszeilenflag '--user-data-dir' festgelegt hat.

Wenn Sie diese Richtlinie nicht aktivieren, wird der Standardprofilpfad verwendet, den der Benutzer jedoch mithilfe des Flags --user-data-dir' überschreiben kann. Benutzer finden das Verzeichnis für das Profil unter edge://version/ unter Profilpfad.

Um Datenverlust oder andere unerwartete Fehler zu vermeiden, konfigurieren Sie diese Richtlinie nicht für das Stammverzeichnis eines Volumes oder für ein Verzeichnis, das für andere Zwecke verwendet wird, da Microsoft Edge dessen Inhalt verwaltet.

Eine Liste der Variablen, die verwendet werden können, finden Sie unter [https://go.microsoft.com/fwlink/?linkid=2095041](https://go.microsoft.com/fwlink/?linkid=2095041).

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Nein - Erfordert einen Neustart des Browsers

  #### Datentyp:
  Zeichenfolge

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: UserDataDir
  - Gruppenrichtlinienname: Benutzerdatenverzeichnis festlegen
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: UserDataDir
  - Werttyp: REG_SZ
  ##### Beispielwert:
```
"${users}/${user_name}/Edge"
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: UserDataDir
  - Beispielwert:
``` xml
<string>${users}/${user_name}/Edge</string>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### UserFeedbackAllowed
  #### Benutzerfeedback zulassen
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Microsoft Edge verwendet das Edge-Feedbackfeature (standardmäßig aktiviert), um Benutzern das Übermitteln von Feedback, Vorschlägen oder Kundenumfragen sowie das Melden von Problemen mit dem Browser zu ermöglichen. Das Edge-Feedbackfeature kann standardmäßig nicht von Benutzern deaktiviert werden.

Wenn Sie diese Richtlinie aktivieren oder nicht konfigurieren, können Benutzer das Edge-Feedbackfeature aufrufen.

Wenn Sie diese Richtlinie deaktivieren, können Benutzer das Edge-Feedbackfeature nicht aufrufen.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Nein - Erfordert einen Neustart des Browsers

  #### Datentyp:
  Boolesch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: UserFeedbackAllowed
  - Gruppenrichtlinienname: Benutzerfeedback zulassen
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: UserFeedbackAllowed
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000001
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: UserFeedbackAllowed
  - Beispielwert:
``` xml
<true/>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### VideoCaptureAllowed
  #### Videoaufnahme zulassen oder blockieren
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Legt fest, ob Sites Videos aufnehmen können.

Ist diese Richtlinie aktiviert oder nicht konfiguriert (Standard), wird der Benutzer für alle Websites vor der Videoaufzeichnung um Erlaubnis gefragt. Ausnahme: Für Sites mit URLs, die in der Liste der Richtlinie [VideoCaptureAllowedUrls](#videocaptureallowedurls) aufgeführt sind, wird der Zugriff ohne Nachfrage gewährt.

Wenn Sie diese Richtlinie deaktivieren, wird der Benutzer nicht gefragt, und eine Videoaufnahme ist nur für URLs möglich, die in der Richtlinie [VideoCaptureAllowedUrls](#videocaptureallowedurls) konfiguriert sind.

Diese Richtlinie betrifft alle Arten von Videoeingängen, nicht nur die eingebaute Kamera.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Boolesch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: VideoCaptureAllowed
  - Gruppenrichtlinienname: Videoaufnahme zulassen oder blockieren
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: VideoCaptureAllowed
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000000
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: VideoCaptureAllowed
  - Beispielwert:
``` xml
<false/>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### VideoCaptureAllowedUrls
  #### Websites, die auf Videoaufnahmegeräte zugreifen können, ohne eine Berechtigung anzufordern
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Geben Sie Websites basierend auf URL-Mustern an, die Videoaufnahmegeräte verwenden können, ohne den Benutzer um Erlaubnis zu bitten. Muster in dieser Liste werden mit dem Sicherheitsursprung der anfordernden URL abgeglichen. Wenn sie übereinstimmen, wird der Website automatisch der Zugriff auf Videoaufnahmegeräte gewährt.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Ja

  #### Datentyp:
  Liste der Zeichenfolgen

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: VideoCaptureAllowedUrls
  - Gruppenrichtlinienname: Websites, die auf Videoaufnahmegeräte zugreifen können, ohne eine Berechtigung anzufordern
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge\VideoCaptureAllowedUrls
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: 1, 2, 3, ...
  - Werttyp: Liste von REG_SZ
  ##### Beispielwert:
```
SOFTWARE\Policies\Microsoft\Edge\VideoCaptureAllowedUrls\0 = "https://www.contoso.com/"
SOFTWARE\Policies\Microsoft\Edge\VideoCaptureAllowedUrls\1 = "https://[*.]contoso.edu/"

```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: VideoCaptureAllowedUrls
  - Beispielwert:
``` xml
<array>
  <string>https://www.contoso.com/</string>
  <string>https://[*.]contoso.edu/</string>
</array>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### WPADQuickCheckEnabled
  #### WPAD-Optimierung festlegen
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Ermöglicht das deaktivieren der WPAD-Optimierung (Web Proxy Auto-Discovery) in Microsoft Edge.

Wenn Sie diese Richtlinie deaktivieren, wird die WPAD-Optimierung deaktiviert. Dadurch muss der Browser länger auf DNS-basierte WPAD-Server warten.

Wenn Sie die Richtlinie aktivieren oder nicht konfigurieren, ist die WPAD-Optimierung aktiviert.

Unabhängig davon, ob oder wie diese Richtlinie aktiviert ist, kann die Einstellung für die WPAD-Optimierung nicht von Benutzern geändert werden.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Nein - Erfordert einen Neustart des Browsers

  #### Datentyp:
  Boolesch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: WPADQuickCheckEnabled
  - Gruppenrichtlinienname: WPAD-Optimierung festlegen
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: WPADQuickCheckEnabled
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000001
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: WPADQuickCheckEnabled
  - Beispielwert:
``` xml
<true/>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### WebDriverOverridesIncompatiblePolicies
  #### Zulassen, dass WebDriver inkompatible Richtlinien außer Kraft setzt
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Diese Richtlinie wurde in M80 entfernt, da sie nicht mehr notwendig ist, weil
WebDriver nun mit allen bestehenden Richtlinien kompatibel ist.

Diese Richtlinie ermöglicht es WebDriver-Benutzern, Richtlinien zu überschreiben,
die dessen Betrieb beeinträchtigen können.

Derzeit deaktiviert diese Richtlinie die Richtlinien [SitePerProcess](#siteperprocess) und [IsolateOrigins](#isolateorigins).

Wenn die Richtlinie aktiviert ist, kann WebDriver inkompatible
Richtlinien überschreiben.
Wenn die Richtlinie deaktiviert oder nicht konfiguriert ist, darf WebDriver inkompatible
Richtlinien nicht überschreiben.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Nein - Erfordert einen Neustart des Browsers

  #### Datentyp:
  Boolesch

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: WebDriverOverridesIncompatiblePolicies
  - Gruppenrichtlinienname: Zulassen, dass WebDriver inkompatible Richtlinien außer Kraft setzt
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: WebDriverOverridesIncompatiblePolicies
  - Werttyp: REG_DWORD
  ##### Beispielwert:
```
0x00000001
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: WebDriverOverridesIncompatiblePolicies
  - Beispielwert:
``` xml
<true/>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### WebRtcLocalhostIpHandling
  #### Verfügbarmachung der Localhost-IP-Adresse durch WebRTC beschränken
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Hiermit können Sie festlegen, ob WebRTC die localhost-IP-Adresse des Benutzers verfügbar macht.

Wenn Sie diese Richtlinie auf „AllowAllInterfaces“ ('default') oder „AllowPublicAndPrivateInterfaces“ ('default_public_and_private_interfaces') festlegen, macht WebRTC die localhost-IP-Adresse verfügbar.

Wenn Sie diese Richtlinie auf „AllowPublicInterfaceOnly“ ('default_public_interface_only') oder „DisableNonProxiedUdp“ ('disable_non_proxied_udp') festlegen, macht WebRTC die localhost-IP-Adresse nicht verfügbar.

Wenn Sie diese Richtlinie deaktivieren oder nicht festlegen, macht WebRTC die localhost-IP-Adresse verfügbar.

  * 'default' = Alle Schnittstellen zulassen. Dadurch wird die localhost-IP-Adresse verfügbar gemacht.
  * 'default_public_and_private_interfaces' = Öffentliche und private Schnittstellen über HTTP-Standardroute zulassen. Die localhost-IP-Adresse wird dadurch verfügbar gemacht.
  * 'default_public_interface_only' = Öffentliche Schnittstelle über HTTP-Standardroute zulassen. Dadurch wird die localhost-IP-Adresse nicht verfügbar gemacht.
  * 'disable_non_proxied_udp’ = Verwenden Sie TCP, es sei denn, der Proxyserver unterstützt UDP. Dadurch wird die localhost-IP-Adresse nicht verfügbar gemacht.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Nein - Erfordert einen Neustart des Browsers

  #### Datentyp:
  Zeichenfolge

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: WebRtcLocalhostIpHandling
  - Gruppenrichtlinienname: Verfügbarmachung der Localhost-IP-Adresse durch WebRTC beschränken
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: WebRtcLocalhostIpHandling
  - Werttyp: REG_SZ
  ##### Beispielwert:
```
"default"
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: WebRtcLocalhostIpHandling
  - Beispielwert:
``` xml
<string>default</string>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)

  ### WebRtcUdpPortRange
  #### Bereich der lokalen, von WebRTC verwendeten UDP-Ports einschränken
  >Unterstützte Versionen: Microsoft Edge unter Windows und Mac seit Version 77 oder höher

  #### Beschreibung
  Schränkt den von WebRTC verwendeten UDP-Portbereich auf ein angegebenes Portintervall (Endpunkte eingeschlossen) ein.

Wenn Sie diese Richtlinie konfigurieren, geben Sie den Bereich der lokalen UDP-Ports an, die von WebRTC verwendet werden können.

Wenn Sie diese Richtlinie nicht konfigurieren, oder wenn Sie sie auf eine leere Zeichenfolge oder einen ungültigen Portbereich festlegen, kann WebRTC einen beliebigen verfügbaren lokalen UDP-Port verwenden.

  #### Unterstützte Features:
  - Kann zwingend sein: Ja
  - Kann empfohlen werden: Nein
  - Dynamische Richtlinienaktualisierung: Nein - Erfordert einen Neustart des Browsers

  #### Datentyp:
  Zeichenfolge

  #### Windows-Informationen und-Einstellungen
  ##### Informationen zur Gruppenrichtlinie (ADMX)
  - Eindeutiger Name der Gruppenrichtlinie: WebRtcUdpPortRange
  - Gruppenrichtlinienname: Bereich der lokalen, von WebRTC verwendeten UDP-Ports einschränken
  - Gruppenrichtlinienpfad (Erforderlich): Administrative Vorlagen/Microsoft Edge/
  - Gruppenrichtlinienpfad (Empfohlen): Nicht zutreffend
  - Name der ADMX-Datei der Gruppenrichtlinie: MSEdge.admx
  ##### Windows-Registrierungseinstellungen
  - Pfad (Erforderlich): SOFTWARE\Policies\Microsoft\Edge
  - Pfad (Empfohlen): Nicht zutreffend
  - Wertname: WebRtcUdpPortRange
  - Werttyp: REG_SZ
  ##### Beispielwert:
```
"10000-11999"
```


  #### Mac-Informationen und -Einstellungen
  - Gewünschter Schlüsselname: WebRtcUdpPortRange
  - Beispielwert:
``` xml
<string>10000-11999</string>
```
  

  [Zurück nach oben](#microsoft-edge-–-richtlinien)


## Siehe auch
- [Konfigurieren von Microsoft Edge](configure-microsoft-edge.md)
- [Microsoft Edge: Zielseite für Unternehmen](https://aka.ms/EdgeEnterprise)