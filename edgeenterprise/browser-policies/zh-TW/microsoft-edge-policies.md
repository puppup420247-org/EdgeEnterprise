---
title: "Microsoft Edge Browser Policy Documentation"
ms.author: stmoody
author: brianalt-msft
manager: tahills
ms.date: 11/26/2019
audience: ITPro
ms.topic: reference
ms.prod: microsoft-edge
ms.localizationpriority: medium
ms.collection: M365-modern-desktop
ms.custom:
description: "Windows and Mac documentation for all policies supported by the Microsoft Edge Browser"
---

# Microsoft Edge - 原則
最新版本的 Microsoft Edge 包含下列原則。您可以使用這些原則設定 Microsoft Edge 在組織中的運行方式。

有關使用其他群組原則，控制 Microsoft Edge 的更新方式及更新時間，請查看 [Microsoft Edge 更新原則參考](microsoft-edge-update-policies.md)

> [!注意]
> 此文章適用於 Microsoft Edge 77 版本或更新版本。

## 可用的原則
下清單格列出在此版本的 Microsoft Edge 中可用的所有與瀏覽器相關的群組原則。使用表格中的連結取得特定政策的更多詳細資訊。

|||
|-|-|
|[Cast](#cast)|[HTTP 驗證](#http-驗證)|
|[Proxy 伺服器](#proxy-伺服器)|[SmartScreen 設定](#smartscreen-設定)|
|[內容設定](#內容設定)|[列印](#列印)|
|[原生訊息](#原生訊息)|[啟動、首頁和新索引標籤頁面](#啟動、首頁和新索引標籤頁面)|
|[密碼管理員和防護](#密碼管理員和防護)|[擴充功能](#擴充功能)|
|[預設搜尋提供者](#預設搜尋提供者)|[Additional](#additional)|


### [*Cast*](#cast-policies)
|原則名稱|標題|
|-|-|
|[EnableMediaRouter](#enablemediarouter)|啟用 Google Cast|
|[ShowCastIconInToolbar](#showcasticonintoolbar)|在工具列中顯示轉換圖示|
### [*HTTP 驗證*](#http-驗證-policies)
|原則名稱|標題|
|-|-|
|[AllowCrossOriginAuthPrompt](#allowcrossoriginauthprompt)|允許跨原始來源 HTTP Basic Auth 提示|
|[AuthNegotiateDelegateAllowlist](#authnegotiatedelegateallowlist)|指定 Microsoft Edge 可以委派使用者認證的伺服器清單|
|[AuthSchemes](#authschemes)|支援的驗證配置|
|[AuthServerAllowlist](#authserverallowlist)|設定允許驗證伺服器的清單|
|[DisableAuthNegotiateCnameLookup](#disableauthnegotiatecnamelookup)|當協調 Kerberos 驗證時停用 CNAME 查閱|
|[EnableAuthNegotiatePort](#enableauthnegotiateport)|Kerberos SPN 中包含非標準連接埠|
|[NtlmV2Enabled](#ntlmv2enabled)|控制是否要啟用 NTLMv2 驗證|
### [*Proxy 伺服器*](#proxy-伺服器-policies)
|原則名稱|標題|
|-|-|
|[ProxyBypassList](#proxybypasslist)|設定 Proxy 許可規則|
|[ProxyMode](#proxymode)|設定 proxy 伺服器設定|
|[ProxyPacUrl](#proxypacurl)|設定 Proxy .pac 檔案 URL|
|[ProxyServer](#proxyserver)|設定 Proxy 伺服器的地址或 URL|
|[ProxySettings](#proxysettings)|Proxy 設定|
### [*SmartScreen 設定*](#smartscreen-設定-policies)
|原則名稱|標題|
|-|-|
|[PreventSmartScreenPromptOverride](#preventsmartscreenpromptoverride)|防止略過 [Microsoft Defender SmartScreen] 提示網站|
|[PreventSmartScreenPromptOverrideForFiles](#preventsmartscreenpromptoverrideforfiles)|防止略過關於下載項目的 Microsoft Defender SmartScreen 警告|
|[SmartScreenAllowListDomains](#smartscreenallowlistdomains)|設定的網域的 Microsoft Defender SmartScreen 篩選工具將不會觸發警告的清單|
|[SmartScreenEnabled](#smartscreenenabled)|設定 Microsoft Defender SmartScreen|
|[SmartScreenForTrustedDownloadsEnabled](#smartscreenfortrusteddownloadsenabled)|強制 Microsoft Defender SmartScreen 檢查來自受信任來源的下載|
|[SmartScreenPuaEnabled](#smartscreenpuaenabled)|設定 Microsoft Defender SmartScreen 以封鎖潛在不需要的應用程式|
### [*內容設定*](#內容設定-policies)
|原則名稱|標題|
|-|-|
|[AutoSelectCertificateForUrls](#autoselectcertificateforurls)|自動選取這些網站的用戶端憑證|
|[CookiesAllowedForUrls](#cookiesallowedforurls)|允許在特定網站上的 Cookie|
|[CookiesBlockedForUrls](#cookiesblockedforurls)|封鎖特定網站上的 Cookie|
|[CookiesSessionOnlyForUrls](#cookiessessiononlyforurls)|限制來自特定網站的 Cookie 匯入目前的工作階段|
|[DefaultCookiesSetting](#defaultcookiessetting)|設定 Cookie|
|[DefaultGeolocationSetting](#defaultgeolocationsetting)|預設地理位置設定值|
|[DefaultImagesSetting](#defaultimagessetting)|設定影像設定|
|[DefaultInsecureContentSetting](#defaultinsecurecontentsetting)|Control use of insecure content exceptions|
|[DefaultJavaScriptSetting](#defaultjavascriptsetting)|預設 JavaScript 設定|
|[DefaultNotificationsSetting](#defaultnotificationssetting)|預設通知設定|
|[DefaultPluginsSetting](#defaultpluginssetting)|預設 Adobe Flash 設定|
|[DefaultPopupsSetting](#defaultpopupssetting)|預設快顯視窗設定|
|[DefaultWebBluetoothGuardSetting](#defaultwebbluetoothguardsetting)|控制 Web 藍牙 API 的使用|
|[DefaultWebUsbGuardSetting](#defaultwebusbguardsetting)|控制 WebUSB API 的使用|
|[ImagesAllowedForUrls](#imagesallowedforurls)|允許這些網站上的影像|
|[ImagesBlockedForUrls](#imagesblockedforurls)|特定網站上的封鎖影像|
|[InsecureContentAllowedForUrls](#insecurecontentallowedforurls)|Allow insecure content on specified sites|
|[InsecureContentBlockedForUrls](#insecurecontentblockedforurls)|Block insecure content on specified sites|
|[JavaScriptAllowedForUrls](#javascriptallowedforurls)|允許特定網站上的 JavaScript|
|[JavaScriptBlockedForUrls](#javascriptblockedforurls)|封鎖特定網站上的 JavaScript|
|[LegacySameSiteCookieBehaviorEnabled](#legacysamesitecookiebehaviorenabled)|啟用預設舊版 SameSite Cookie 行為設定|
|[LegacySameSiteCookieBehaviorEnabledForDomainList](#legacysamesitecookiebehaviorenabledfordomainlist)|將指定網站上的 Cookie 恢復至舊版 SameSite 行為|
|[NotificationsAllowedForUrls](#notificationsallowedforurls)|允許特定網站上的通知|
|[NotificationsBlockedForUrls](#notificationsblockedforurls)|封鎖特定網站上的通知|
|[PluginsAllowedForUrls](#pluginsallowedforurls)|允許特定網站上的 Adobe Flash 外掛程式|
|[PluginsBlockedForUrls](#pluginsblockedforurls)|封鎖特定網站上的 Adobe Flash 外掛程式|
|[PopupsAllowedForUrls](#popupsallowedforurls)|允許特定站台上的快顯視窗|
|[PopupsBlockedForUrls](#popupsblockedforurls)|封鎖特定網站上的快顯視窗|
|[RegisteredProtocolHandlers](#registeredprotocolhandlers)|登錄通訊協定處理常式|
|[WebUsbAllowDevicesForUrls](#webusballowdevicesforurls)|授與特定網站連線到特定 USB 裝置的存取權|
|[WebUsbAskForUrls](#webusbaskforurls)|在特定站台上允許 WebUSB|
|[WebUsbBlockedForUrls](#webusbblockedforurls)|封鎖特定網站上的 WebUSB|
### [*列印*](#列印-policies)
|原則名稱|標題|
|-|-|
|[DefaultPrinterSelection](#defaultprinterselection)|預設印表機選取規則|
|[PrintHeaderFooter](#printheaderfooter)|列印頁首與頁尾|
|[PrintPreviewUseSystemDefaultPrinter](#printpreviewusesystemdefaultprinter)|將系統預設的印表機設定為預設印表機|
|[PrintingEnabled](#printingenabled)|啟用列印|
|[UseSystemPrintDialog](#usesystemprintdialog)|列印使用系統列印對話方塊|
### [*原生訊息*](#原生訊息-policies)
|原則名稱|標題|
|-|-|
|[NativeMessagingAllowlist](#nativemessagingallowlist)|原生訊息中心裝載使用者可以使用的控制項|
|[NativeMessagingBlocklist](#nativemessagingblocklist)|設定原生訊息中心的封鎖清單|
|[NativeMessagingUserLevelHosts](#nativemessaginguserlevelhosts)|允許使用者層級的原生訊息中心主機 (無需系統管理員權限即可安裝)|
### [*啟動、首頁和新索引標籤頁面*](#啟動、首頁和新索引標籤頁面-policies)
|原則名稱|標題|
|-|-|
|[HomepageIsNewTabPage](#homepageisnewtabpage)|將新的索引標籤頁面設定為 [首頁]|
|[HomepageLocation](#homepagelocation)|設定首頁頁面 URL|
|[NewTabPageCompanyLogo](#newtabpagecompanylogo)|設定新索引標籤頁面公司標誌|
|[NewTabPageHideDefaultTopSites](#newtabpagehidedefaulttopsites)|隱藏新索引標籤頁面中的預設熱門網站|
|[NewTabPageLocation](#newtabpagelocation)|設定新索引標籤頁面 URL|
|[NewTabPageManagedQuickLinks](#newtabpagemanagedquicklinks)|設定新的索引標籤頁面快速連結|
|[NewTabPageSetFeedType](#newtabpagesetfeedtype)|設定 Microsoft Edge 的新索引標籤頁面體驗|
|[RestoreOnStartup](#restoreonstartup)|啟動時所採取的動作|
|[RestoreOnStartupURLs](#restoreonstartupurls)|瀏覽器啟動時開啟的網站|
|[ShowHomeButton](#showhomebutton)|在工具列上顯示 [首頁] 按鈕|
### [*密碼管理員和防護*](#密碼管理員和防護-policies)
|原則名稱|標題|
|-|-|
|[PasswordManagerEnabled](#passwordmanagerenabled)|啟用儲存密碼的密碼管理員|
|[PasswordProtectionChangePasswordURL](#passwordprotectionchangepasswordurl)|設定變更密碼 URL|
|[PasswordProtectionLoginURLs](#passwordprotectionloginurls)|設定密碼保護服務應擷取密碼指紋的企業登入 URL 清單|
|[PasswordProtectionWarningTrigger](#passwordprotectionwarningtrigger)|設定密碼保護警告觸發程序|
### [*擴充功能*](#擴充功能-policies)
|原則名稱|標題|
|-|-|
|[ExtensionAllowedTypes](#extensionallowedtypes)|設定允許的延伸模組類型|
|[ExtensionInstallAllowlist](#extensioninstallallowlist)|允許特定安裝擴充功能|
|[ExtensionInstallBlocklist](#extensioninstallblocklist)|控制不能安裝哪些擴充程式|
|[ExtensionInstallForcelist](#extensioninstallforcelist)|控制哪些擴充功能會默默地安裝|
|[ExtensionInstallSources](#extensioninstallsources)|設定擴充功能與使用者指令碼安裝來源|
|[ExtensionSettings](#extensionsettings)|設定擴充功能管理設定|
### [*預設搜尋提供者*](#預設搜尋提供者-policies)
|原則名稱|標題|
|-|-|
|[DefaultSearchProviderEnabled](#defaultsearchproviderenabled)|啟用預設搜尋提供者|
|[DefaultSearchProviderEncodings](#defaultsearchproviderencodings)|預設搜尋提供者編碼|
|[DefaultSearchProviderImageURL](#defaultsearchproviderimageurl)|指定預設搜尋提供者的影像搜尋功能|
|[DefaultSearchProviderImageURLPostParams](#defaultsearchproviderimageurlpostparams)|使用 POST 的影像 URL 參數|
|[DefaultSearchProviderKeyword](#defaultsearchproviderkeyword)|預設搜尋提供者關鍵字|
|[DefaultSearchProviderName](#defaultsearchprovidername)|預設搜尋提供者名稱|
|[DefaultSearchProviderSearchURL](#defaultsearchprovidersearchurl)|預設搜尋提供者搜尋 URL|
|[DefaultSearchProviderSuggestURL](#defaultsearchprovidersuggesturl)|預設建議的搜尋提供者 URL|
### [*Additional*](#additional-policies)
|原則名稱|標題|
|-|-|
|[AdsSettingForIntrusiveAdsSites](#adssettingforintrusiveadssites)|含有干擾廣告網站的廣告設定|
|[AllowDeletingBrowserHistory](#allowdeletingbrowserhistory)|啟用刪除瀏覽器和下載歷程記錄|
|[AllowFileSelectionDialogs](#allowfileselectiondialogs)|允許檔案選取項目對話方塊|
|[AllowPopupsDuringPageUnload](#allowpopupsduringpageunload)|允許在網頁卸載時顯示快顯視窗|
|[AllowSyncXHRInPageDismissal](#allowsyncxhrinpagedismissal)|允許頁面在頁面關閉期間發送同步 XHR 請求|
|[AllowTrackingForUrls](#allowtrackingforurls)|設定特定網站的追蹤防止例外狀況|
|[AlwaysOpenPdfExternally](#alwaysopenpdfexternally)|一律開啟外部 PDF 檔案|
|[ApplicationLocaleValue](#applicationlocalevalue)|設定應用程式地區設定|
|[AudioCaptureAllowed](#audiocaptureallowed)|允許或封鎖音訊擷取|
|[AudioCaptureAllowedUrls](#audiocaptureallowedurls)|無需請求權限即可存取音訊擷取裝置的網站|
|[AutoImportAtFirstRun](#autoimportatfirstrun)|在首次執行時，自動匯入其他瀏覽器的資料和設定|
|[AutofillAddressEnabled](#autofilladdressenabled)|啟用 [自動填滿] 位址|
|[AutofillCreditCardEnabled](#autofillcreditcardenabled)|啟用信用卡「自動填滿」功能|
|[AutoplayAllowed](#autoplayallowed)|允許網站自動播放媒體|
|[BackgroundModeEnabled](#backgroundmodeenabled)|在 Microsoft Edge 關閉後繼續執行背景應用程式|
|[BackgroundTemplateListUpdatesEnabled](#backgroundtemplatelistupdatesenabled)|對 [集合] 可用的範本清單和其他使用範本的功能啟用背景更新。|
|[BlockThirdPartyCookies](#blockthirdpartycookies)|封鎖第三方 Cookie|
|[BrowserAddProfileEnabled](#browseraddprofileenabled)|啟用從 [身分識別] 飛出視窗功能表或 [設定] 頁面建立設定檔|
|[BrowserGuestModeEnabled](#browserguestmodeenabled)|啟用來賓模式|
|[BrowserNetworkTimeQueriesEnabled](#browsernetworktimequeriesenabled)|允許查詢瀏覽器網路時間服務|
|[BrowserSignin](#browsersignin)|瀏覽器登入設定|
|[BuiltInDnsClientEnabled](#builtindnsclientenabled)|使用內建 DNS 用戶端|
|[CertificateTransparencyEnforcementDisabledForCas](#certificatetransparencyenforcementdisabledforcas)|停用 subjectPublicKeyInfo 雜湊清單的憑證透明度強化|
|[CertificateTransparencyEnforcementDisabledForLegacyCas](#certificatetransparencyenforcementdisabledforlegacycas)|停用舊版憑證授權單位清單的 [憑證透明度] 強化|
|[CertificateTransparencyEnforcementDisabledForUrls](#certificatetransparencyenforcementdisabledforurls)|停用針對特定 URL 的憑證透明度強化|
|[ClearBrowsingDataOnExit](#clearbrowsingdataonexit)|當 Microsoft Edge 關閉時清除瀏覽資料|
|[ClickOnceEnabled](#clickonceenabled)|允許使用者透過 ClickOnce 協定打開檔案|
|[CommandLineFlagSecurityWarningsEnabled](#commandlineflagsecuritywarningsenabled)|啟用命令列旗標的安全性警告|
|[ComponentUpdatesEnabled](#componentupdatesenabled)|啟用 Microsoft Edge 中的元件更新|
|[ConfigureDoNotTrack](#configuredonottrack)|設定 [不要追蹤]|
|[ConfigureOnlineTextToSpeech](#configureonlinetexttospeech)|設定線上文字轉語音|
|[CustomHelpLink](#customhelplink)|指定自訂 [説明] 連結|
|[DefaultBrowserSettingEnabled](#defaultbrowsersettingenabled)|設定 Microsoft Edge 為預設瀏覽器|
|[DeveloperToolsAvailability](#developertoolsavailability)|控制可在哪使用開發人員工具|
|[DirectInvokeEnabled](#directinvokeenabled)|允許使用者透過 DirectInvoke 協定打開檔案|
|[Disable3DAPIs](#disable3dapis)|停用 3D 圖形 Api 支援|
|[DisableScreenshots](#disablescreenshots)|停用取得螢幕擷取畫面功能|
|[DiskCacheDir](#diskcachedir)|設定磁碟快取目錄|
|[DiskCacheSize](#diskcachesize)|設定磁碟快取大小，以位元組為單位|
|[DownloadDirectory](#downloaddirectory)|設定下載目錄|
|[DownloadRestrictions](#downloadrestrictions)|允許下載限制|
|[EdgeCollectionsEnabled](#edgecollectionsenabled)|啟用 [集錦] 功能|
|[EditFavoritesEnabled](#editfavoritesenabled)|允許使用者編輯我的最愛|
|[EnableDeprecatedWebPlatformFeatures](#enabledeprecatedwebplatformfeatures)|在限定時間內重新啟用已取代的網頁平台功能|
|[EnableDomainActionsDownload](#enabledomainactionsdownload)|啟用從 Microsoft 進行網域動作下載|
|[EnableOnlineRevocationChecks](#enableonlinerevocationchecks)|啟用線上 OCSP/CRL 檢查|
|[EnterpriseHardwarePlatformAPIEnabled](#enterprisehardwareplatformapienabled)|允許受管理的擴充程式使用企業硬體平台 API|
|[ExperimentationAndConfigurationServiceControl](#experimentationandconfigurationservicecontrol)|透過 [實驗] 和 [設定服務] 控制通訊|
|[ExternalProtocolDialogShowAlwaysOpenCheckbox](#externalprotocoldialogshowalwaysopencheckbox)|在外部通訊協定對話方塊中顯示「一律開啟」核取方塊。|
|[FavoritesBarEnabled](#favoritesbarenabled)|啟用 [我的最愛] 列|
|[ForceBingSafeSearch](#forcebingsafesearch)|強制執行 Bing 安全搜尋|
|[ForceEphemeralProfiles](#forceephemeralprofiles)|啟用使用暫時設定檔|
|[ForceGoogleSafeSearch](#forcegooglesafesearch)|強制執行 Google 安全搜尋|
|[ForceNetworkInProcess](#forcenetworkinprocess)|強制網路程式碼在瀏覽器處理程序中執行|
|[ForceYouTubeRestrict](#forceyoutuberestrict)|強制最小 YouTube 限制模式|
|[FullscreenAllowed](#fullscreenallowed)|允許全螢幕模式|
|[GoToIntranetSiteForSingleWordEntryInAddressBar](#gotointranetsiteforsinglewordentryinaddressbar)|強制直接進行內部網路網站導航，而非在 [網址列] 中搜尋單字項目。|
|[HSTSPolicyBypassList](#hstspolicybypasslist)|設定會略過 HSTS 原則檢查的名稱清單|
|[HardwareAccelerationModeEnabled](#hardwareaccelerationmodeenabled)|可用時便使用硬體加速|
|[ImportAutofillFormData](#importautofillformdata)|允許匯入自動填滿表單資料|
|[ImportBrowserSettings](#importbrowsersettings)|允許匯入瀏覽器設定|
|[ImportFavorites](#importfavorites)|允許匯入 [我的最愛]|
|[ImportHistory](#importhistory)|允許匯入瀏覽歷程記錄|
|[ImportHomepage](#importhomepage)|允許匯入首頁設定|
|[ImportOpenTabs](#importopentabs)|允許匯入已開啟的索引標籤|
|[ImportPaymentInfo](#importpaymentinfo)|允許匯入付款資訊|
|[ImportSavedPasswords](#importsavedpasswords)|允許匯入已儲存的密碼|
|[ImportSearchEngine](#importsearchengine)|允許匯入搜尋引擎設定|
|[InPrivateModeAvailability](#inprivatemodeavailability)|設定 InPrivate 模式可用性|
|[InternetExplorerIntegrationLevel](#internetexplorerintegrationlevel)|設定 Internet Explorer 整合|
|[InternetExplorerIntegrationSiteList](#internetexplorerintegrationsitelist)|設定 [企業模式網站清單]|
|[IsolateOrigins](#isolateorigins)|為特定來源啟用網站隔離|
|[ManagedFavorites](#managedfavorites)|設定我的最愛|
|[ManagedSearchEngines](#managedsearchengines)|管理搜索引擎|
|[MaxConnectionsPerProxy](#maxconnectionsperproxy)|同時連線到 Proxy 伺服器的最大數目|
|[MediaRouterCastAllowAllIPs](#mediaroutercastallowallips)|允許 Google Cast 連線至所有 IP 位址上的 Cast 裝置|
|[MetricsReportingEnabled](#metricsreportingenabled)|啟用使用量及當機相關資料報告|
|[NetworkPredictionOptions](#networkpredictionoptions)|啟用網路預測|
|[NonRemovableProfileEnabled](#nonremovableprofileenabled)|設定使用者是否一律擁有其公司或學校帳戶自動登入的預設設定檔|
|[OverrideSecurityRestrictionsOnInsecureOrigin](#overridesecurityrestrictionsoninsecureorigin)|控制不安全來源中安全性限制套用的地方|
|[PinningWizardAllowed](#pinningwizardallowed)|允許 [釘選到工作列精靈]|
|[ProactiveAuthEnabled](#proactiveauthenabled)|啟用主動式驗證|
|[PromotionalTabsEnabled](#promotionaltabsenabled)|啟用全分頁促銷內容|
|[PromptForDownloadLocation](#promptfordownloadlocation)|詢問下載檔案的儲存位置|
|[QuicAllowed](#quicallowed)|允許 QUIC 通訊協定|
|[RelaunchNotification](#relaunchnotification)|通知使用者建議或需要重新啟動瀏覽器，以套用擱置中的更新|
|[RelaunchNotificationPeriod](#relaunchnotificationperiod)|設定更新通知的時間週期|
|[RendererCodeIntegrityEnabled](#renderercodeintegrityenabled)|啟用轉譯器程式碼完整性|
|[RequireOnlineRevocationChecksForLocalAnchors](#requireonlinerevocationchecksforlocalanchors)|指定本機信賴起點是否需要線上 OCSP / CRL 檢查|
|[ResolveNavigationErrorsUseWebService](#resolvenavigationerrorsusewebservice)|透過網頁服務啟用瀏覽錯誤解析度|
|[RestrictSigninToPattern](#restrictsignintopattern)|限制哪些帳戶可用為 Microsoft Edge 主要帳戶|
|[RunAllFlashInAllowMode](#runallflashinallowmode)|將 Adobe Flash 內容設定延伸至所有內容|
|[SSLErrorOverrideAllowed](#sslerroroverrideallowed)|允許使用者從 HTTPS 警告頁面繼續|
|[SSLVersionMin](#sslversionmin)|已啟用最低 TLS 版本|
|[SavingBrowserHistoryDisabled](#savingbrowserhistorydisabled)|停用儲存瀏覽器歷程記錄|
|[SearchSuggestEnabled](#searchsuggestenabled)|啟用搜尋建議|
|[SecurityKeyPermitAttestation](#securitykeypermitattestation)|不需要權限即可使用直接存取 [安全性金鑰] 證明的網站或網域|
|[SendIntranetToInternetExplorer](#sendintranettointernetexplorer)|將所有內部網路網站傳送到 Internet Explorer|
|[SendSiteInfoToImproveServices](#sendsiteinfotoimproveservices)|傳送網站資訊來改善 Microsoft 服務|
|[ShowOfficeShortcutInFavoritesBar](#showofficeshortcutinfavoritesbar)|在 [我的最愛] 列中顯示 Microsoft Office 捷徑|
|[SignedHTTPExchangeEnabled](#signedhttpexchangeenabled)|啟用簽署 HTTP Exchange (SXG) 支援|
|[SitePerProcess](#siteperprocess)|在所有網站中啟用網站隔離|
|[SpellcheckEnabled](#spellcheckenabled)|啟用拼字檢查|
|[SpellcheckLanguage](#spellchecklanguage)|啟用特定拼字檢查語言|
|[SpellcheckLanguageBlocklist](#spellchecklanguageblocklist)|強制停用拼字檢查語言|
|[SuppressUnsupportedOSWarning](#suppressunsupportedoswarning)|隱藏不支援的 OS 警告|
|[SyncDisabled](#syncdisabled)|透過 Microsoft 同步服務停用資料同步處理|
|[TabFreezingEnabled](#tabfreezingenabled)|允許凍結背景索引標籤|
|[TaskManagerEndProcessEnabled](#taskmanagerendprocessenabled)|在瀏覽器工作管理員中啟用結束處理程序|
|[TrackingPrevention](#trackingprevention)|封鎖使用者的網頁瀏覽活動追蹤|
|[TranslateEnabled](#translateenabled)|啟用翻譯|
|[URLAllowlist](#urlallowlist)|定義受允許的 URL 清單|
|[URLBlocklist](#urlblocklist)|封鎖存取 URL 清單|
|[UserDataDir](#userdatadir)|設定使用者資料目錄|
|[UserFeedbackAllowed](#userfeedbackallowed)|允許使用者意見反應|
|[VideoCaptureAllowed](#videocaptureallowed)|允許或封鎖視訊擷取|
|[VideoCaptureAllowedUrls](#videocaptureallowedurls)|無需請求權限即可存取視訊擷取裝置的網站|
|[WPADQuickCheckEnabled](#wpadquickcheckenabled)|設定 WPAD 最佳化|
|[WebAppInstallForceList](#webappinstallforcelist)|設定強制安裝 Web 應用程式的清單|
|[WebDriverOverridesIncompatiblePolicies](#webdriveroverridesincompatiblepolicies)|允許 WebDriver 覆寫不相容原則|
|[WebRtcLocalIpsAllowedUrls](#webrtclocalipsallowedurls)|Manage exposure of local IP addressess by WebRTC|
|[WebRtcLocalhostIpHandling](#webrtclocalhostiphandling)|Restrict exposure of local IP address by WebRTC|
|[WebRtcUdpPortRange](#webrtcudpportrange)|限制 WebRTC 所使用的本機 UDP 連接埠範圍|




  ## Cast policies

  [回到頂端](#microsoft-edge---原則)

  ### EnableMediaRouter
  #### 啟用 Google Cast
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  啟用此原則以啟用 Google Cast。使用者將可以從應用程式功能表、網頁操作功能表、已啟用 Cast 的網站上的媒體控制項和 (如有顯示) Cast 工具列圖示啟動 Google Cast。

停用此原則以停用 Google Cast。

根據預設，Google Cast 將會啟用。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 否 - 需要重新啟動瀏覽器

  #### 資料類型:
  布林值

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: EnableMediaRouter
  - GP 名稱: 啟用 Google Cast
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/Cast
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: EnableMediaRouter
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000001
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: EnableMediaRouter
  - 範例值:
``` xml
<true/>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### ShowCastIconInToolbar
  #### 在工具列中顯示轉換圖示
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  將此原則設定為 true 即可在工具列或溢位 (overflow) 功能表顯示投射工具列圖示。

如果未設定或停用此原則，使用者可使用圖示的特色選單釘選或移除圖示。

如果也將 [EnableMediaRouter](#enablemediarouter) 原則設定為 false，則會忽略此原則，且不會顯示工具列。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 否 - 需要重新啟動瀏覽器

  #### 資料類型:
  布林值

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: ShowCastIconInToolbar
  - GP 名稱: 在工具列中顯示轉換圖示
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/Cast
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: ShowCastIconInToolbar
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000000
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: ShowCastIconInToolbar
  - 範例值:
``` xml
<false/>
```
  

  [回到頂端](#microsoft-edge---原則)

  ## HTTP 驗證 policies

  [回到頂端](#microsoft-edge---原則)

  ### AllowCrossOriginAuthPrompt
  #### 允許跨原始來源 HTTP Basic Auth 提示
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  控制頁面上的第三方子內容是否可以開啟 HTTP 基本驗證對話方塊。

一般而言，這會作為網路釣魚防護停用。如果您未設定此原則，此原則將停用，且第三方子內容無法開啟 HTTP 基本驗證對話方塊。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  布林值

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: AllowCrossOriginAuthPrompt
  - GP 名稱: 允許跨原始來源 HTTP Basic Auth 提示
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/HTTP 驗證
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: AllowCrossOriginAuthPrompt
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000000
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: AllowCrossOriginAuthPrompt
  - 範例值:
``` xml
<false/>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### AuthNegotiateDelegateAllowlist
  #### 指定 Microsoft Edge 可以委派使用者認證的伺服器清單
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  設定 Microsoft Edge 可以委派的伺服器清單。

以逗號分隔多個伺服器名稱。允許使用萬用字元 (*)。

如果您未設定此原則 Microsoft Edge，即使伺服器偵測到內部網路，也不會委派使用者認證。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 否 - 需要重新啟動瀏覽器

  #### 資料類型:
  字串

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: AuthNegotiateDelegateAllowlist
  - GP 名稱: 指定 Microsoft Edge 可以委派使用者認證的伺服器清單
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/HTTP 驗證
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: AuthNegotiateDelegateAllowlist
  - 數值類型: REG_SZ
  ##### 範例值:
```
"contoso.com"
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: AuthNegotiateDelegateAllowlist
  - 範例值:
``` xml
<string>contoso.com</string>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### AuthSchemes
  #### 支援的驗證配置
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  指定支援的 HTTP 驗證配置。

您可以使用以下值來設定原則: [基本]，[摘要]，[ntlm] 和 [交涉]。以逗點分隔多個值。

如果不設定此原則，則全部四種配置皆會使用。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 否 - 需要重新啟動瀏覽器

  #### 資料類型:
  字串

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: AuthSchemes
  - GP 名稱: 支援的驗證配置
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/HTTP 驗證
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: AuthSchemes
  - 數值類型: REG_SZ
  ##### 範例值:
```
"basic,digest,ntlm,negotiate"
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: AuthSchemes
  - 範例值:
``` xml
<string>basic,digest,ntlm,negotiate</string>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### AuthServerAllowlist
  #### 設定允許驗證伺服器的清單
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  指定啟用整合式驗證的伺服器。只有當 Microsoft Edge 接收來自清單中的 Proxy 或伺服器的驗證要求時，整合式驗證才會啟用。

以逗號分隔多個伺服器名稱。允許使用萬用字元 (*)。

如果您未設定此原則， Microsoft Edge  會嘗試偵測伺服器是否在內部網路 - 只有這樣才會回應 IWA 請求。如果伺服器位於網際網路上，Microsoft Edge 會忽略來自 IWA 的請求。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 否 - 需要重新啟動瀏覽器

  #### 資料類型:
  字串

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: AuthServerAllowlist
  - GP 名稱: 設定允許驗證伺服器的清單
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/HTTP 驗證
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: AuthServerAllowlist
  - 數值類型: REG_SZ
  ##### 範例值:
```
"*contoso.com,contoso.com"
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: AuthServerAllowlist
  - 範例值:
``` xml
<string>*contoso.com,contoso.com</string>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### DisableAuthNegotiateCnameLookup
  #### 當協調 Kerberos 驗證時停用 CNAME 查閱
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  決定產生的 Kerberos SPN 是根據正式的 DNS 名稱 (CNAME) 或輸入的原始名稱。

如果您啟用此原則，則會略過 CNAME 查閱並使用伺服器名稱 (如輸入內容)。

如果您停用此原則或未設定，會使用伺服器的正式名稱。透過 CNAME 查閱決定。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 否 - 需要重新啟動瀏覽器

  #### 資料類型:
  布林值

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: DisableAuthNegotiateCnameLookup
  - GP 名稱: 當協調 Kerberos 驗證時停用 CNAME 查閱
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/HTTP 驗證
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: DisableAuthNegotiateCnameLookup
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000000
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: DisableAuthNegotiateCnameLookup
  - 範例值:
``` xml
<false/>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### EnableAuthNegotiatePort
  #### Kerberos SPN 中包含非標準連接埠
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  指定生成的 Kerberos SPN 是否應該包含一個非標準的連接埠。

如果您啟用此原則，使用者會在 URL 中包含非標準的連接埠 (80 或 443 以外的連接埠)，該連接埠包含於生成的 Kerberos SPN 中。

如果您未設定或停用此原則，生成的 Kerberos SPN 在任何情況下均不會包含連接埠。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 否 - 需要重新啟動瀏覽器

  #### 資料類型:
  布林值

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: EnableAuthNegotiatePort
  - GP 名稱: Kerberos SPN 中包含非標準連接埠
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/HTTP 驗證
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: EnableAuthNegotiatePort
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000000
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: EnableAuthNegotiatePort
  - 範例值:
``` xml
<false/>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### NtlmV2Enabled
  #### 控制是否要啟用 NTLMv2 驗證
  >支援的版本: Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  控制是否啟用 NTLMv2。

Samba 和 Windows 伺服器的所有新版本都支援 NTLMv2。因為 NTLMv2 會降低驗證安全性，您應該僅停用 NTLMv2 以解決回溯相容性問題。

如果您未設定此原則，預設會啟用 NTLMv2。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  布林值

  

  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: NtlmV2Enabled
  - 範例值:
``` xml
<true/>
```
  

  [回到頂端](#microsoft-edge---原則)

  ## Proxy 伺服器 policies

  [回到頂端](#microsoft-edge---原則)

  ### ProxyBypassList
  #### 設定 Proxy 許可規則
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  定義 Microsoft Edge 略過所有 Proxy 的主機清單。

只有當您在 [ProxyMode](#proxymode) 原則中選取 'Use fixed proxy servers' 時套用此原則。如果您選取了任何其他設定 Proxy 原則的模式時，不要啟用或設定此原則。

如果您啟用此原則，則您可以建立未使用 Proxy 的 Microsoft Edge 主機清單。

如果您未設定此原則，則會為其建立所有略過 Proxy 的 Microsoft Edge 主機清單。如果您已指定其他設定 Proxy 原則的方法，請取消設定此原則。

如需詳細範例，請前往 [https://go.microsoft.com/fwlink/?linkid=2094936](https://go.microsoft.com/fwlink/?linkid=2094936)。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  字串

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: ProxyBypassList
  - GP 名稱: 設定 Proxy 許可規則
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/Proxy 伺服器
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: ProxyBypassList
  - 數值類型: REG_SZ
  ##### 範例值:
```
"https://www.contoso.com, https://www.fabrikam.com"
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: ProxyBypassList
  - 範例值:
``` xml
<string>https://www.contoso.com, https://www.fabrikam.com</string>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### ProxyMode
  #### 設定 proxy 伺服器設定
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  指定 Microsoft Edge 使用的 Proxy 伺服器設定。如果啟用此原則，則使用者無法變更 Proxy 設定。

如果您選擇永不使用 Proxy 伺服器並一律直接連線，則會忽略所有其他選項。

如果選擇使用系統 Proxy 設定，則會忽略所有其他選項。

如果選擇自動偵測 Proxy 伺服器，則會忽略所有其他選項。

如果選擇固定伺服器 Proxy 模式，則可以在 [ProxyServer](#proxyserver) 和 'Comma-separated list of proxy bypass rules' 中指定更多選項。

如果選擇使用 .pac Proxy 指令碼，則必須在 'URL to a proxy .pac file' 中，指定指令碼的URL。

如需詳細的範例，請前往 [https://go.microsoft.com/fwlink/?linkid=2094936](https://go.microsoft.com/fwlink/?linkid=2094936)。如果啟用此原則，則 Microsoft Edge 將忽略從命令列指定的所有與 Proxy 相關的選項。

如果不設定此原則，則使用者可以選擇自己的 Proxy 設定。

* "dir ect" =永不使用 Proxy

* "auto_detect" =自動偵測 Proxy 伺服器

* "pac_script" = 使用 .pac Proxy 指令碼

* "fixed_servers" = 使用固定 Proxy 伺服器

* "system" = 使用系統 Proxy 設定

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  字串

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: ProxyMode
  - GP 名稱: 設定 proxy 伺服器設定
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/Proxy 伺服器
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: ProxyMode
  - 數值類型: REG_SZ
  ##### 範例值:
```
"direct"
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: ProxyMode
  - 範例值:
``` xml
<string>direct</string>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### ProxyPacUrl
  #### 設定 Proxy .pac 檔案 URL
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  指定 Proxy 自動設定 (PAC) 檔案的 URL。

只有當您在 [ProxyMode](#proxymode) 原則中選取 [使用 .pac Proxy 指令碼] 時，此原則才會套用。如果您選取任何其他模式進行 Proxy 原則設定時，不要啟用或設定此原則。

  如果您啟用此原則，您可以指定 PAC 檔案，這會定義瀏覽器自動選擇適當的 Proxy 伺服器以取得特定網站的 URL 的方式。

  如果您停用或未設定此原則，則不會指定任何 PAC 檔案。如果已指定任何其他方法來設定 Proxy 原則，請不要設定此原則。

  如需詳細範例，請參閱 [https://go.microsoft.com/fwlink/?linkid=2094936](https://go.microsoft.com/fwlink/?linkid=2094936)。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  字串

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: ProxyPacUrl
  - GP 名稱: 設定 Proxy .pac 檔案 URL
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/Proxy 伺服器
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: ProxyPacUrl
  - 數值類型: REG_SZ
  ##### 範例值:
```
"https://internal.contoso.com/example.pac"
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: ProxyPacUrl
  - 範例值:
``` xml
<string>https://internal.contoso.com/example.pac</string>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### ProxyServer
  #### 設定 Proxy 伺服器的地址或 URL
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  指定 Proxy 伺服器的 URL。

只有當您在 [ProxyMode](#proxymode) 原則中選取 [使用固定的 proxy 伺服器] 時，才會套用這個原則。如果您選取了任何其他模式來設定 Proxy 原則，不要啟用或設定此原則。

如果您啟用這個原則，這個原則設定的 Proxy 伺服器將用於所有 URL。

如果您停用或未設定此原則，使用者可以在這個 Proxy 模式中選擇自己的 Proxy 設定。如果您已指定任何其他方法來設定 Proxy 原則，請不要設定此原則。

如需其他選項以及詳細的範例，請參閱 [https://go.microsoft.com/fwlink/?linkid=2094936](https://go.microsoft.com/fwlink/?linkid=2094936)。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  字串

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: ProxyServer
  - GP 名稱: 設定 Proxy 伺服器的地址或 URL
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/Proxy 伺服器
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: ProxyServer
  - 數值類型: REG_SZ
  ##### 範例值:
```
"123.123.123.123:8080"
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: ProxyServer
  - 範例值:
``` xml
<string>123.123.123.123:8080</string>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### ProxySettings
  #### Proxy 設定
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  設定 Microsoft Edge 的 Proxy 設定。

 如果您啟用此原則，Microsoft Edge 會略過從命令列指定的所有與 Proxy 相關的選項。

 如果您未設定此原則，使用者可以選擇自己的 Proxy 設定。

 此原則會覆寫下列的個別原則:

   [ProxyMode](#proxymode)
   [ProxyPacUrl](#proxypacurl)
   [ProxyServer](#proxyserver)
   [ProxyBypassList](#proxybypasslist)

   ProxyMode 欄位可讓您指定 Microsoft Edge 使用的 proxy 伺服器並防止使用者變更 Proxy 設定。

ProxyPacUrl 欄位是連至 proxy.pac 檔案的 URL。

 ProxyServer 欄位是 proxy 伺服器的 URL。

 ProxyBypassList 的欄位是 Microsoft Edge 略過的 Proxy 主機清單。

 如果您選擇的 'direct' 值為 'ProxyMode' 時，永遠不會使用 Proxy，且會忽略所有其他欄位。

 如果您選擇的 'system' 值為 'ProxyMode' 時，將會使用 Proxy，且會忽略所有其他欄位。

 如果您選擇的 'auto_detect' 值為 'ProxyMode' 時，會忽略所有其他欄位。

 如果您選擇的 'fixed_server' 值為 'ProxyMode' 時，則會使用 'ProxyServer' 和 'ProxyBypassList' 欄位。

 如果您選擇的 'pac_script' 值為 'ProxyMode' 時，則會使用 'ProxyPacUrl' 和 'ProxyBypassList' 欄位。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  字典

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: ProxySettings
  - GP 名稱: Proxy 設定
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/Proxy 伺服器
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: ProxySettings
  - 數值類型: REG_SZ
  ##### 範例值:
```
SOFTWARE\Policies\Microsoft\Edge\ProxySettings = {
  "ProxyBypassList": "https://www.example1.com,https://www.example2.com,https://internalsite/", 
  "ProxyMode": "direct", 
  "ProxyPacUrl": "https://internal.site/example.pac", 
  "ProxyServer": "123.123.123.123:8080"
}
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: ProxySettings
  - 範例值:
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
  

  [回到頂端](#microsoft-edge---原則)

  ## SmartScreen 設定 policies

  [回到頂端](#microsoft-edge---原則)

  ### PreventSmartScreenPromptOverride
  #### 防止略過 [Microsoft Defender SmartScreen] 提示網站
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  此原則可讓您確認使用者是否可以覆寫有關潛在惡意網站的 Microsoft Defender SmartScreen 警告。

如果啟用此設定，則使用者將無法忽略 Microsoft Defender SmartScreen 警告，且會讓使用者無法繼續瀏覽網站。

如果停用或未設定此設定，則使用者可以忽略 Microsoft Defender SmartScreen 警告，並繼續瀏覽網站。

此原則僅適用於已加入 Microsoft Active Directory 網域的 Windows 執行個體; 或已註冊裝置管理的 Windows 10 專業版或企業版執行個體。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  布林值

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: PreventSmartScreenPromptOverride
  - GP 名稱: 防止略過 [Microsoft Defender SmartScreen] 提示網站
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/SmartScreen 設定
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: PreventSmartScreenPromptOverride
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000001
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: PreventSmartScreenPromptOverride
  - 範例值:
``` xml
<true/>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### PreventSmartScreenPromptOverrideForFiles
  #### 防止略過關於下載項目的 Microsoft Defender SmartScreen 警告
  >支援的版本: Windows 上的 Microsoft Edge (77 版或更新版本)，以及 Mac 上的 Microsoft Edge (79 版或更新版本)

  #### 描述
  此原則可讓您確認使用者是否可以覆寫有關未驗證下載的 Microsoft Defender SmartScreen 警告。

如果啟用此原則，則您組織中的使用者將無法忽略 Microsoft Defender SmartScreen 警告，且會讓使用者無法完成未驗證的下載。

如果停用或未設定此原則，則使用者可以忽略 Microsoft Defender SmartScreen 警告，並完成未驗證的下載。

此原則僅適用於已加入 Microsoft Active Directory 網域的 Windows 執行個體; 或已註冊裝置管理的 Windows 10 專業版或企業版執行個體。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  布林值

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: PreventSmartScreenPromptOverrideForFiles
  - GP 名稱: 防止略過關於下載項目的 Microsoft Defender SmartScreen 警告
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/SmartScreen 設定
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: PreventSmartScreenPromptOverrideForFiles
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000001
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: PreventSmartScreenPromptOverrideForFiles
  - 範例值:
``` xml
<true/>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### SmartScreenAllowListDomains
  #### 設定的網域的 Microsoft Defender SmartScreen 篩選工具將不會觸發警告的清單
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  設定 Microsoft Defender SmartScreen 受信任網域的清單。這表示:
如果來源 URL 符合這些網域，Microsoft Defender SmartScreen 將不會檢查潛在的惡意資源，例如網路釣魚軟體與其他惡意程式碼。
Microsoft Defender SmartScreen 下載防護服務將不會檢查這些網域上裝載的下載內容。

  如果啟用此原則，則 Microsoft Defender SmartScreen 會信任這些網域。
如果停用或未設定此原則，預設 Microsoft Defender SmartScreen 保護會套用到所有資源。

此原則僅適用於已加入 Microsoft Active Directory 網域的 Windows 執行個體; 或已註冊裝置管理的 Windows 10 專業版或企業版執行個體。
請注意，如果您的組織已啟用 Microsoft Defender 進階威脅防護，則不適用此原則。您必須先在 Microsoft Defender 資訊安全中心設定允許及封鎖清單。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  字串的清單

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: SmartScreenAllowListDomains
  - GP 名稱: 設定的網域的 Microsoft Defender SmartScreen 篩選工具將不會觸發警告的清單
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/SmartScreen 設定
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge\SmartScreenAllowListDomains
  - 路徑 (推薦項目): N/A
  - 值名稱: 1, 2, 3, ...
  - 數值類型: REG_SZ 的清單
  ##### 範例值:
```
SOFTWARE\Policies\Microsoft\Edge\SmartScreenAllowListDomains\0 = "mydomain.com"
SOFTWARE\Policies\Microsoft\Edge\SmartScreenAllowListDomains\1 = "myuniversity.edu"

```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: SmartScreenAllowListDomains
  - 範例值:
``` xml
<array>
  <string>mydomain.com</string>
  <string>myuniversity.edu</string>
</array>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### SmartScreenEnabled
  #### 設定 Microsoft Defender SmartScreen
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  此原則設定可讓您設定是否要開啟 Microsoft Defender SmartScreen。Microsoft Defender SmartScreen 可提供警告訊息，以協助保護您的使用者從潛在網路釣魚詐騙與惡意軟體。根據預設，Microsoft Defender SmartScreen 已開啟。

如果您啟用這個設定，Microsoft Defender SmartScreen 已開啟，使用者無法關閉。

如果您停用這個設定，Microsoft Defender SmartScreen 已關閉，且使用者無法開啟它。

如果您未設定這個設定，使用者可以選擇是否要使用 Microsoft Defender SmartScreen。

這個原則僅適用於已加入的 Windows 執行個體 Microsoft Active Directory 網域; 或在 Windows 10 專業版或企業的執行個體上的已註冊裝置管理。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 是
  - 動態原則重新整理: 是

  #### 資料類型:
  布林值

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: SmartScreenEnabled
  - GP 名稱: 設定 Microsoft Defender SmartScreen
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/SmartScreen 設定
  - GP 路徑 (推薦項目): 系統管理範本/Microsoft Edge - 預設設定 (使用者可以覆寫)/SmartScreen 設定
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): SOFTWARE\Policies\Microsoft\Edge\推薦項目
  - 值名稱: SmartScreenEnabled
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000001
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: SmartScreenEnabled
  - 範例值:
``` xml
<true/>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### SmartScreenForTrustedDownloadsEnabled
  #### 強制 Microsoft Defender SmartScreen 檢查來自受信任來源的下載
  >支援的版本: Windows 上的 Microsoft Edge (78 版或更新版本)

  #### 描述
  此原則設定可讓您設定 Microsoft Defender SmartScreen 是否檢查來自受信任來源的下載評價。

如果您啟用或未設定此設定，Microsoft Defender SmartScreen 會無視來源檢查下載評價。

如果您停用此設定，從受信任來源下載時，Microsoft Defender SmartScreen 篩選工具並不會檢查下載評價。

此原則是僅適用於已加入 Windows 執行個體的 Microsoft Active Directory 網域中; 或在 Windows 10 專業版或企業版已註冊裝置管理的執行個體上。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 是
  - 動態原則重新整理: 是

  #### 資料類型:
  布林值

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: SmartScreenForTrustedDownloadsEnabled
  - GP 名稱: 強制 Microsoft Defender SmartScreen 檢查來自受信任來源的下載
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/SmartScreen 設定
  - GP 路徑 (推薦項目): 系統管理範本/Microsoft Edge - 預設設定 (使用者可以覆寫)/SmartScreen 設定
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): SOFTWARE\Policies\Microsoft\Edge\推薦項目
  - 值名稱: SmartScreenForTrustedDownloadsEnabled
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000000
```


  

  [回到頂端](#microsoft-edge---原則)

  ### SmartScreenPuaEnabled
  #### 設定 Microsoft Defender SmartScreen 以封鎖潛在不需要的應用程式
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (80 版或更新版本)

  #### 描述
  此原則設定可讓您設定是否要在 Microsoft Defender SmartScreen 開啟封鎖潛在垃圾應用程式。Microsoft Defender SmartScreen 中的潛在垃圾應用程式封鎖功能會針對廣告軟體、挖礦程式、混入軟體和其他網站提供的低評價應用程式，提供警告訊息以幫助保護用戶。根據預設，Microsoft Defender SmartScreen 已關閉。

如果您啟用這個設定，Microsoft Defender SmartScreen 內的垃圾應用程式封鎖功能將會開啟。

如果您停用這個設定，Microsoft Defender SmartScreen 內的垃圾應用程式封鎖功能將會關閉。

如果您未設定這個設定，使用者可以選擇是否要使用 Microsoft Defender SmartScreen 內的垃圾應用程式封鎖功能。

此原則僅適用於已加入的 Windows 執行個體 Microsoft Active Directory 網域; 或在 Windows 10 專業版或企業的執行個體上的已註冊裝置管理。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 是
  - 動態原則重新整理: 是

  #### 資料類型:
  布林值

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: SmartScreenPuaEnabled
  - GP 名稱: 設定 Microsoft Defender SmartScreen 以封鎖潛在不需要的應用程式
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/SmartScreen 設定
  - GP 路徑 (推薦項目): 系統管理範本/Microsoft Edge - 預設設定 (使用者可以覆寫)/SmartScreen 設定
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): SOFTWARE\Policies\Microsoft\Edge\推薦項目
  - 值名稱: SmartScreenPuaEnabled
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000001
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: SmartScreenPuaEnabled
  - 範例值:
``` xml
<true/>
```
  

  [回到頂端](#microsoft-edge---原則)

  ## 內容設定 policies

  [回到頂端](#microsoft-edge---原則)

  ### AutoSelectCertificateForUrls
  #### 自動選取這些網站的用戶端憑證
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  根據 URL 模式指定網站清單，如果網站請求，Microsoft Edge 應為其自動選擇用戶端憑證。

該值必須是 JSON 字典字串化的陣列。每個字典的格式必須為 { "pattern": "$URL_PATTERN", "filter" : $FILTER }，其中 $URL_PATTERN 是內容設定模式。$FILTER 限制瀏覽器要自動選擇哪個用戶端憑證。與篩選器無關，僅選擇與伺服器憑證要求相符的憑證。例如，如果 $FILTER 的格式為 { "ISSUER": { "CN": "$ISSUER_CN" } }，則僅選擇由具有 CommonName $ISSUER_CN 的憑證所發布的用戶端憑證。如果 $FILTER 包含"ISSUER" 和 "SUBJECT" 部分，用戶端憑證必須同時滿足兩個要選擇的條件。如果 $FILTER 指定一個組織 ("O")，則憑證必須具有至少一個與要選擇的指定值相符的組織。如果 $FILTER 指定組織單位 ("OU")，則憑證必須具有至少一個與要選擇的指定值相符的組織單位。已選擇。如果 $FILTER 為空字典 {}，則用戶端憑證的選擇沒有任何其他限制。

如果未設定此原則，則所有網站皆不會進行自動選擇。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  字串的清單

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: AutoSelectCertificateForUrls
  - GP 名稱: 自動選取這些網站的用戶端憑證
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/內容設定
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge\AutoSelectCertificateForUrls
  - 路徑 (推薦項目): N/A
  - 值名稱: 1, 2, 3, ...
  - 數值類型: REG_SZ 的清單
  ##### 範例值:
```
SOFTWARE\Policies\Microsoft\Edge\AutoSelectCertificateForUrls\0 = "{"pattern":"https://www.contoso.com","filter":{"ISSUER":{"CN":"certificate issuer name", "L": "certificate issuer location", "O": "certificate issuer org", "OU": "certificate issuer org unit"}, "SUBJECT":{"CN":"certificate subject name", "L": "certificate subject location", "O": "certificate subject org", "OU": "certificate subject org unit"}}}"

```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: AutoSelectCertificateForUrls
  - 範例值:
``` xml
<array>
  <string>{"pattern":"https://www.contoso.com","filter":{"ISSUER":{"CN":"certificate issuer name", "L": "certificate issuer location", "O": "certificate issuer org", "OU": "certificate issuer org unit"}, "SUBJECT":{"CN":"certificate subject name", "L": "certificate subject location", "O": "certificate subject org", "OU": "certificate subject org unit"}}}</string>
</array>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### CookiesAllowedForUrls
  #### 允許在特定網站上的 Cookie
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  根據 URL 的規則，定義不允許設定 Cookie 的網站清單。

如果您未設定此原則，所有網站都將使用來自 [DefaultCookiesSetting](#defaultcookiessetting) 原則 (如有設定) 或使用者個人設定的全域預設值。

請查看 [CookiesBlockedForUrls](#cookiesblockedforurls) 和 [CookiesSessionOnlyForUrls](#cookiessessiononlyforurls) 原則，了解更多資訊。

請注意這三個原則之間不可有衝突的 URL 模式設定:

- [CookiesBlockedForUrls](#cookiesblockedforurls)

- CookiesAllowedForUrls

- [CookiesSessionOnlyForUrls](#cookiessessiononlyforurls)

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  字串的清單

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: CookiesAllowedForUrls
  - GP 名稱: 允許在特定網站上的 Cookie
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/內容設定
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge\CookiesAllowedForUrls
  - 路徑 (推薦項目): N/A
  - 值名稱: 1, 2, 3, ...
  - 數值類型: REG_SZ 的清單
  ##### 範例值:
```
SOFTWARE\Policies\Microsoft\Edge\CookiesAllowedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\CookiesAllowedForUrls\1 = "[*.]contoso.edu"

```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: CookiesAllowedForUrls
  - 範例值:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### CookiesBlockedForUrls
  #### 封鎖特定網站上的 Cookie
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  根據 URL 的規則，定義不允許設定 Cookie 的網站清單。

如果您未設定此原則，所有網站都將使用來自 [DefaultCookiesSetting](#defaultcookiessetting) 原則 (如有設定) 或使用者個人設定的全域預設值。

 請查看 [CookiesAllowedForUrls](#cookiesallowedforurls) 和[CookiesSessionOnlyForUrls](#cookiessessiononlyforurls) 原則，了解更多資訊。請注意這三個原則之間不可有衝突的 URL 模式設定:

 - CookiesBlockedForUrls

 - [CookiesAllowedForUrls](#cookiesallowedforurls)

 - [CookiesSessionOnlyForUrls](#cookiessessiononlyforurls)



  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  字串的清單

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: CookiesBlockedForUrls
  - GP 名稱: 封鎖特定網站上的 Cookie
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/內容設定
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge\CookiesBlockedForUrls
  - 路徑 (推薦項目): N/A
  - 值名稱: 1, 2, 3, ...
  - 數值類型: REG_SZ 的清單
  ##### 範例值:
```
SOFTWARE\Policies\Microsoft\Edge\CookiesBlockedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\CookiesBlockedForUrls\1 = "[*.]contoso.edu"

```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: CookiesBlockedForUrls
  - 範例值:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### CookiesSessionOnlyForUrls
  #### 限制來自特定網站的 Cookie 匯入目前的工作階段
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  工作階段結束 (關閉視窗) 時，會刪除由符合您所定義的 URL 模式的網站的 Cookie。

建立者不符合模式的網站的 Cookie 由 [DefaultCookiesSetting](#defaultcookiessetting) 原則 (如果設定) 或使用者的個人設定。如果您未設定這個原則，這是預設行為。

如果 Microsoft Edge 正以背景模式工作階段可能關閉時執行的上一個視窗會關閉，這表示視窗關閉時，將不會清除 Cookie。如需 Microsoft Edge 以背景模式執行時所會發生情形的詳細資訊，請查看 [BackgroundModeEnabled](#backgroundmodeenabled) 原則。n
您也可以使用 [CookiesAllowedForUrls](#cookiesallowedforurls) 和 [CookiesBlockedForUrls](#cookiesblockedforurls) 原則來控制哪些網站可以建立 Cookie。

附註有不可以是介於這些三個原則設定衝突的 URL 模式:

- [CookiesBlockedForUrls](#cookiesblockedforurls)

- [CookiesAllowedForUrls](#cookiesallowedforurls)

- CookiesSessionOnlyForUrls

如果您設定 [RestoreOnStartup](#restoreonstartup) 原則為從先前的工作階段還原 URL，就會忽略此原則，並為這些網站永久儲存 Cookie。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  字串的清單

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: CookiesSessionOnlyForUrls
  - GP 名稱: 限制來自特定網站的 Cookie 匯入目前的工作階段
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/內容設定
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge\CookiesSessionOnlyForUrls
  - 路徑 (推薦項目): N/A
  - 值名稱: 1, 2, 3, ...
  - 數值類型: REG_SZ 的清單
  ##### 範例值:
```
SOFTWARE\Policies\Microsoft\Edge\CookiesSessionOnlyForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\CookiesSessionOnlyForUrls\1 = "[*.]contoso.edu"

```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: CookiesSessionOnlyForUrls
  - 範例值:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### DefaultCookiesSetting
  #### 設定 Cookie
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  控制網站是否可以能在使用者裝置上建立 Cookie。此原則為可以或完全不行 - 您可以讓所有網站建立 Cookie，或不讓任何網站建立 Cookie。您無法使用此原則啟用來自特定網站的 Cookie。

設定原則為 'SessionOnly' (4)，當工作階段結束時清除 Cookie。如果 Microsoft Edge 正以背景模式運行，當最後一個視窗關閉時，則工作階段可能會停止執行，這表示視窗關閉時將不會清除 Cookie。[BackgroundModeEnabled](#backgroundmodeenabled) 原則會設定當 Microsoft Edge 以背景模式執行時，會發生什麼情況的相關資訊。

如果您未設定此原則，將使用預設 'AllowCookies' (1)，且使用者可以變更此設定中的 Microsoft Edge 設定。(如果您不希望使用者變更此設定，請設定原則)。

* 1 = 讓所有網站建立 Cookie        * 2 = 不要讓任何網站建立 Cookie

* 4 = 保留工作階段持續時間的 Cookie

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  整數

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: DefaultCookiesSetting
  - GP 名稱: 設定 Cookie
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/內容設定
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: DefaultCookiesSetting
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000001
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: DefaultCookiesSetting
  - 範例值:
``` xml
<integer>1</integer>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### DefaultGeolocationSetting
  #### 預設地理位置設定值
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  設定網站是否可以追蹤使用者的實體位置。您可以設定預設 (1) 允許追蹤，設定預設 (2) 拒絕追蹤，或者每次網站請求其位置時詢問使用者 (3)。

如果不設定此原則，則會使用 [AskGeolocation] 原則，且使用者可以變更此

* 1 =允許網站追蹤使用者的實體位置

* 2 =不允許任何網站追蹤使用者的實體位置

* 3 =在網站想要使用者的實體位置時詢問

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  整數

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: DefaultGeolocationSetting
  - GP 名稱: 預設地理位置設定值
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/內容設定
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: DefaultGeolocationSetting
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000001
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: DefaultGeolocationSetting
  - 範例值:
``` xml
<integer>1</integer>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### DefaultImagesSetting
  #### 設定影像設定
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  設定網站是否可以顯示影像。您可以允許所有網站 (1) 上的影像顯示，或封鎖所有網站 (2) 上的影像。

如果您未設定此原則，預設為允許顯示影像，使用者可以變更此設定。

* 1 = 允許所有網站顯示所有影像

* 2 = 不允許所有網站顯示影像

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  整數

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: DefaultImagesSetting
  - GP 名稱: 設定影像設定
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/內容設定
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: DefaultImagesSetting
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000001
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: DefaultImagesSetting
  - 範例值:
``` xml
<integer>1</integer>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### DefaultInsecureContentSetting
  #### Control use of insecure content exceptions
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (80 版或更新版本)

  #### 描述
  Allows you to set whether users can add exceptions to allow mixed content for specific sites.

This policy can be overridden for specific URL patterns using the [InsecureContentAllowedForUrls](#insecurecontentallowedforurls) and [InsecureContentBlockedForUrls](#insecurecontentblockedforurls) policies.

If this policy is left unset, users will be allowed to add exceptions to allow blockable mixed content.

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  整數

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: DefaultInsecureContentSetting
  - GP 名稱: Control use of insecure content exceptions
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/內容設定
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: DefaultInsecureContentSetting
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000002
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: DefaultInsecureContentSetting
  - 範例值:
``` xml
<integer>2</integer>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### DefaultJavaScriptSetting
  #### 預設 JavaScript 設定
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  設定網站是否可以執行 JavaScript。您可以允許所有網站 (1) 執行 JavaScript，或所有網站 (2) 皆不得執行 JavaScript。

如果不設定此原則，則預設為所有網站皆可執行 JavaScript，且使用者可以變更此設定。

* 1 = 允許所有網站執行 JavaScript

* 2 =不允許任何網站執行 JavaScript

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  整數

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: DefaultJavaScriptSetting
  - GP 名稱: 預設 JavaScript 設定
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/內容設定
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: DefaultJavaScriptSetting
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000001
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: DefaultJavaScriptSetting
  - 範例值:
``` xml
<integer>1</integer>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### DefaultNotificationsSetting
  #### 預設通知設定
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  設定網站是否可以顯示桌面通知。您可以預設為允許顯示 (1)、拒絕顯示 (2)，或每次網站想要顯示通知時都詢問使用者 (3)。

如果不設定此原則，預設為允許選是通知，且使用者可以變更此原則。

* 1 =允許網站顯示桌面通知

* 2 =不允許任何網站顯示桌面通知

* 3 =每次網站想要顯示桌面通知時詢問

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  整數

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: DefaultNotificationsSetting
  - GP 名稱: 預設通知設定
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/內容設定
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: DefaultNotificationsSetting
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000002
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: DefaultNotificationsSetting
  - 範例值:
``` xml
<integer>2</integer>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### DefaultPluginsSetting
  #### 預設 Adobe Flash 設定
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  決定 [PluginsAllowedForUrls](#pluginsallowedforurls) 或 [PluginsBlockedForUrls](#pluginsblockedforurls) 未涵蓋的網站是否可以自動執行 Adobe Flash 外掛程式。您可以在所有網站上選取 [BlockPlugins] (2) 來封鎖 Adobe Flash，您也可以選擇 [ClickToPlay] (3) 讓 Adobe Flash 執行，但需要使用者點選預留位置才能啟動。在任何情況下，[PluginsAllowedForUrls](#pluginsallowedforurls) 和 [PluginsBlockedForUrls](#pluginsblockedforurls) 原則皆優先於 'DefaultPluginsSetting'。

僅允許在 [PluginsAllowedForUrls](#pluginsallowedforurls) 原則中明確列出的網域能自動播放。如果要在所有網站上啟用自動播放，請考慮將 http://* 和 https://* 新增到此清單中。

如果未設定此原則，則使用者可以手動變更此設定。

* 2 = 封鎖 Adobe Flash 外掛程式

* 3 = 點擊播放

前者 [1] 選項設定為允許所有，但此功能現在僅由 [PluginsAllowedForUrls](#pluginsallowedforurls) 處理。使用 [1] 的現有原則將在 [點選播放] 模式下執行。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  整數

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: DefaultPluginsSetting
  - GP 名稱: 預設 Adobe Flash 設定
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/內容設定
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: DefaultPluginsSetting
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000002
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: DefaultPluginsSetting
  - 範例值:
``` xml
<integer>2</integer>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### DefaultPopupsSetting
  #### 預設快顯視窗設定
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  設定網站是否可以顯示快顯視窗。您可以允許快顯視窗在所有網站 (1) 上顯示，或在所有網站 (2) 上封鎖。

如果您未設定此原則，預設會封鎖快顯視窗，且使用者可以變更此設定。

* 1 = 允許所有網站顯示快顯視窗

* 2 = 不允許任何網站顯示快顯視窗

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  整數

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: DefaultPopupsSetting
  - GP 名稱: 預設快顯視窗設定
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/內容設定
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: DefaultPopupsSetting
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000001
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: DefaultPopupsSetting
  - 範例值:
``` xml
<integer>1</integer>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### DefaultWebBluetoothGuardSetting
  #### 控制 Web 藍牙 API 的使用
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  控制網站是否可以存取附近的藍牙裝置。您可以完全封鎖存取，或在每次想存取藍牙裝置時要求網站詢問使用者。

如果您未設定此原則，則會使用預設值 (3，這代表每次都會詢問使用者)，而且使用者可以變更預設值。

* 2 = 不允許任何網站利用 Web 藍牙 API 要求存取藍牙裝置

* 3 = 允許網站要求使用者授與存取附近藍牙裝置的權限

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  整數

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: DefaultWebBluetoothGuardSetting
  - GP 名稱: 控制 Web 藍牙 API 的使用
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/內容設定
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: DefaultWebBluetoothGuardSetting
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000002
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: DefaultWebBluetoothGuardSetting
  - 範例值:
``` xml
<integer>2</integer>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### DefaultWebUsbGuardSetting
  #### 控制 WebUSB API 的使用
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  設定網站是否可存取連線的 USB 裝置。每次網站想要存取連線的 USB 裝置時，您都可以完全封鎖存取或詢問使用者。

您可以使用 [WebUsbAskForUrls](#webusbaskforurls) 和 [WebUsbBlockedForUrls](#webusbblockedforurls) 原則覆寫此原則的特定 URL 模式。

如果不設定此原則，網站將根據預設詢問使用者，是否可以存取連線的 USB 裝置 (3)，且使用者可以變更此設定。

* 2 =不允許任何網站透過 WebUSB API 要求存取 USB 裝置

* 3 =允許網站要求使用者授與權限存取連線的 USB 裝置

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  整數

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: DefaultWebUsbGuardSetting
  - GP 名稱: 控制 WebUSB API 的使用
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/內容設定
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: DefaultWebUsbGuardSetting
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000002
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: DefaultWebUsbGuardSetting
  - 範例值:
``` xml
<integer>2</integer>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### ImagesAllowedForUrls
  #### 允許這些網站上的影像
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  根據 URL 模式，定義可以顯示影像的網站清單。

如果您未設定這個原則，所有網站都將使用來自 [DefaultImagesSetting](#defaultimagessetting) 原則 (如有設定) 或使用者個人設定的全域預設值。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  字串的清單

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: ImagesAllowedForUrls
  - GP 名稱: 允許這些網站上的影像
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/內容設定
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge\ImagesAllowedForUrls
  - 路徑 (推薦項目): N/A
  - 值名稱: 1, 2, 3, ...
  - 數值類型: REG_SZ 的清單
  ##### 範例值:
```
SOFTWARE\Policies\Microsoft\Edge\ImagesAllowedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\ImagesAllowedForUrls\1 = "[*.]contoso.edu"

```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: ImagesAllowedForUrls
  - 範例值:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### ImagesBlockedForUrls
  #### 特定網站上的封鎖影像
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  根據 URL 模式，定義不允許顯示影像的網站。

如果您未設定此原則，所有網站都將使用來自 [DefaultImagesSetting](#defaultimagessetting) 原則 (如有設定) 或使用者個人設定的全域預設值。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  字串的清單

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: ImagesBlockedForUrls
  - GP 名稱: 特定網站上的封鎖影像
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/內容設定
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge\ImagesBlockedForUrls
  - 路徑 (推薦項目): N/A
  - 值名稱: 1, 2, 3, ...
  - 數值類型: REG_SZ 的清單
  ##### 範例值:
```
SOFTWARE\Policies\Microsoft\Edge\ImagesBlockedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\ImagesBlockedForUrls\1 = "[*.]contoso.edu"

```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: ImagesBlockedForUrls
  - 範例值:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### InsecureContentAllowedForUrls
  #### Allow insecure content on specified sites
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (80 版或更新版本)

  #### 描述
  Create a list of URL patterns to specify sites that can display insecure mixed content (that is, HTTP content on HTTPS sites.)

If this policy isn’t set, insecure mixed content will be blocked. However, users can set exceptions to allow insecure mixed content for specific sites.

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  字串的清單

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: InsecureContentAllowedForUrls
  - GP 名稱: Allow insecure content on specified sites
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/內容設定
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge\InsecureContentAllowedForUrls
  - 路徑 (推薦項目): N/A
  - 值名稱: 1, 2, 3, ...
  - 數值類型: REG_SZ 的清單
  ##### 範例值:
```
SOFTWARE\Policies\Microsoft\Edge\InsecureContentAllowedForUrls\0 = "https://www.example.com"
SOFTWARE\Policies\Microsoft\Edge\InsecureContentAllowedForUrls\1 = "[*.]example.edu"

```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: InsecureContentAllowedForUrls
  - 範例值:
``` xml
<array>
  <string>https://www.example.com</string>
  <string>[*.]example.edu</string>
</array>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### InsecureContentBlockedForUrls
  #### Block insecure content on specified sites
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (80 版或更新版本)

  #### 描述
  Create a list of URL patterns to specify sites that aren’t allowed to display insecure mixed content (that is, HTTP content on HTTPS sites.)

If this policy isn’t set, insecure mixed content will be blocked. However, users can set exceptions to allow insecure mixed content for specific sites.

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  字串的清單

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: InsecureContentBlockedForUrls
  - GP 名稱: Block insecure content on specified sites
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/內容設定
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge\InsecureContentBlockedForUrls
  - 路徑 (推薦項目): N/A
  - 值名稱: 1, 2, 3, ...
  - 數值類型: REG_SZ 的清單
  ##### 範例值:
```
SOFTWARE\Policies\Microsoft\Edge\InsecureContentBlockedForUrls\0 = "https://www.example.com"
SOFTWARE\Policies\Microsoft\Edge\InsecureContentBlockedForUrls\1 = "[*.]example.edu"

```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: InsecureContentBlockedForUrls
  - 範例值:
``` xml
<array>
  <string>https://www.example.com</string>
  <string>[*.]example.edu</string>
</array>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### JavaScriptAllowedForUrls
  #### 允許特定網站上的 JavaScript
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  根據 URL 的規則，定義允許執行 JavaScript 的網站清單。

如果您未設定此原則，所有網站都將使用來自 [DefaultJavaScriptSetting](#defaultjavascriptsetting) 原則 (如有設定) 或使用者個人設定的全域預設值。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  字串的清單

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: JavaScriptAllowedForUrls
  - GP 名稱: 允許特定網站上的 JavaScript
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/內容設定
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge\JavaScriptAllowedForUrls
  - 路徑 (推薦項目): N/A
  - 值名稱: 1, 2, 3, ...
  - 數值類型: REG_SZ 的清單
  ##### 範例值:
```
SOFTWARE\Policies\Microsoft\Edge\JavaScriptAllowedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\JavaScriptAllowedForUrls\1 = "[*.]contoso.edu"

```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: JavaScriptAllowedForUrls
  - 範例值:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### JavaScriptBlockedForUrls
  #### 封鎖特定網站上的 JavaScript
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  根據 URL 模式，定義不允許執行 JavaScript 的網站。

如果您未設定此原則，所有網站都將使用來自 [DefaultJavaScriptSetting](#defaultjavascriptsetting) 原則 (如有設定) 或使用者個人設定的全域預設值。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  字串的清單

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: JavaScriptBlockedForUrls
  - GP 名稱: 封鎖特定網站上的 JavaScript
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/內容設定
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge\JavaScriptBlockedForUrls
  - 路徑 (推薦項目): N/A
  - 值名稱: 1, 2, 3, ...
  - 數值類型: REG_SZ 的清單
  ##### 範例值:
```
SOFTWARE\Policies\Microsoft\Edge\JavaScriptBlockedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\JavaScriptBlockedForUrls\1 = "[*.]contoso.edu"

```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: JavaScriptBlockedForUrls
  - 範例值:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### LegacySameSiteCookieBehaviorEnabled
  #### 啟用預設舊版 SameSite Cookie 行為設定
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (80 版或更新版本)

  #### 描述
  讓您可以將所有 Cookie 恢復為舊版 SameSite 行為。恢復至舊行為會導致未指定 SameSite 屬性的 Cookie 被視為 [SameSite=None]，並刪除對 [SameSite=None] Cookie 的要求，以具有 [Secure] 屬性。

您可以為此原則設定下列值：

* 1 = 所有網站上的 Cookie 均恢復為舊版 SameSite 行為

* 2 = 所有網站上的 Cookie 使用 SameSite-by-default 行為

如果未設定此原則，則未指定 SameSite 屬性的 Cookie，其預設行為將取決於 SameSite-by-default 功能的其他設定資源。此功能可能透過現場試驗來設定，也可以透過啟用 edge://flags 中的 same-site-by-default-cookies 旗標來設定。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  整數

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: LegacySameSiteCookieBehaviorEnabled
  - GP 名稱: 啟用預設舊版 SameSite Cookie 行為設定
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/內容設定
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: LegacySameSiteCookieBehaviorEnabled
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000001
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: LegacySameSiteCookieBehaviorEnabled
  - 範例值:
``` xml
<integer>1</integer>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### LegacySameSiteCookieBehaviorEnabledForDomainList
  #### 將指定網站上的 Cookie 恢復至舊版 SameSite 行為
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (80 版或更新版本)

  #### 描述
  符合指定模式的網域所設定的 Cookie 將恢復為舊版 SameSite 行為。

恢復至舊行為會導致未指定 SameSite 屬性的 Cookie 被視為 [SameSite=None]，並刪除對 [SameSite=None] Cookie 的要求，以具有 [Secure] 屬性。

如果未設定此原則，則將使用全域預設值。全域預設值也將用於未涵蓋於您指定模式的網域的 Cookie。

可使用 [LegacySameSiteCookieBehaviorEnabled](#legacysamesitecookiebehaviorenabled) 原則來設定全域預設值。如果未設定 [LegacySameSiteCookieBehaviorEnabled](#legacysamesitecookiebehaviorenabled)，則全域預設值將回到其他設定源。

請注意，在此原則中列出的模式將視為網域而不是 URL，因此不應指定配置或連接埠。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  字串的清單

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: LegacySameSiteCookieBehaviorEnabledForDomainList
  - GP 名稱: 將指定網站上的 Cookie 恢復至舊版 SameSite 行為
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/內容設定
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge\LegacySameSiteCookieBehaviorEnabledForDomainList
  - 路徑 (推薦項目): N/A
  - 值名稱: 1, 2, 3, ...
  - 數值類型: REG_SZ 的清單
  ##### 範例值:
```
SOFTWARE\Policies\Microsoft\Edge\LegacySameSiteCookieBehaviorEnabledForDomainList\0 = "www.example.com"
SOFTWARE\Policies\Microsoft\Edge\LegacySameSiteCookieBehaviorEnabledForDomainList\1 = "[*.]example.edu"

```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: LegacySameSiteCookieBehaviorEnabledForDomainList
  - 範例值:
``` xml
<array>
  <string>www.example.com</string>
  <string>[*.]example.edu</string>
</array>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### NotificationsAllowedForUrls
  #### 允許特定網站上的通知
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  根據 URL 模式，定義可以顯示通知的網站。

如果您未設定此原則，所有網站都將使用來自 [DefaultNotificationsSetting](#defaultnotificationssetting) 原則 (如有設定) 或使用者個人設定的全域預設值。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  字串的清單

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: NotificationsAllowedForUrls
  - GP 名稱: 允許特定網站上的通知
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/內容設定
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge\NotificationsAllowedForUrls
  - 路徑 (推薦項目): N/A
  - 值名稱: 1, 2, 3, ...
  - 數值類型: REG_SZ 的清單
  ##### 範例值:
```
SOFTWARE\Policies\Microsoft\Edge\NotificationsAllowedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\NotificationsAllowedForUrls\1 = "[*.]contoso.edu"

```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: NotificationsAllowedForUrls
  - 範例值:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### NotificationsBlockedForUrls
  #### 封鎖特定網站上的通知
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  根據 URL 模式，定義封鎖顯示通知的網站清單。

如果您未設定此原則，來自 [DefaultNotificationsSetting](#defaultnotificationssetting) 原則 (如有設定) 的全域預設值或使用者的個人設定將用於所有網站。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  字串的清單

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: NotificationsBlockedForUrls
  - GP 名稱: 封鎖特定網站上的通知
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/內容設定
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge\NotificationsBlockedForUrls
  - 路徑 (推薦項目): N/A
  - 值名稱: 1, 2, 3, ...
  - 數值類型: REG_SZ 的清單
  ##### 範例值:
```
SOFTWARE\Policies\Microsoft\Edge\NotificationsBlockedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\NotificationsBlockedForUrls\1 = "[*.]contoso.edu"

```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: NotificationsBlockedForUrls
  - 範例值:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### PluginsAllowedForUrls
  #### 允許特定網站上的 Adobe Flash 外掛程式
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  根據 URL 模式定義網站清單，這些網站可執行 Adobe Flash 外掛程式。

如果未設定此原則，則所有網站將使用 [DefaultPluginsSetting](#defaultpluginssetting) 原則 (如果有設定) 的全域預設值或使用者的個人設定。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  字串的清單

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: PluginsAllowedForUrls
  - GP 名稱: 允許特定網站上的 Adobe Flash 外掛程式
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/內容設定
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge\PluginsAllowedForUrls
  - 路徑 (推薦項目): N/A
  - 值名稱: 1, 2, 3, ...
  - 數值類型: REG_SZ 的清單
  ##### 範例值:
```
SOFTWARE\Policies\Microsoft\Edge\PluginsAllowedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\PluginsAllowedForUrls\1 = "[*.]contoso.edu"

```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: PluginsAllowedForUrls
  - 範例值:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### PluginsBlockedForUrls
  #### 封鎖特定網站上的 Adobe Flash 外掛程式
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  根據 URL 模式定義網站清單，這些網站模式已封鎖執行 Adobe Flash。

如果未設定此原則，則所有網站將使用 [DefaultPluginsSetting](#defaultpluginssetting) 原則 (如果有設定) 的全域預設值或使用者的個人設定。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  字串的清單

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: PluginsBlockedForUrls
  - GP 名稱: 封鎖特定網站上的 Adobe Flash 外掛程式
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/內容設定
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge\PluginsBlockedForUrls
  - 路徑 (推薦項目): N/A
  - 值名稱: 1, 2, 3, ...
  - 數值類型: REG_SZ 的清單
  ##### 範例值:
```
SOFTWARE\Policies\Microsoft\Edge\PluginsBlockedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\PluginsBlockedForUrls\1 = "[*.]contoso.edu"

```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: PluginsBlockedForUrls
  - 範例值:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### PopupsAllowedForUrls
  #### 允許特定站台上的快顯視窗
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  根據 URL 模式，定義可以開始快顯視窗的網站清單。

如果您未設定這個原則，所有網站都將使用來自 [DefaultPopupsSetting](#defaultpopupssetting) 原則 (如有設定) 或使用者個人設定的全域預設值。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  字串的清單

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: PopupsAllowedForUrls
  - GP 名稱: 允許特定站台上的快顯視窗
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/內容設定
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge\PopupsAllowedForUrls
  - 路徑 (推薦項目): N/A
  - 值名稱: 1, 2, 3, ...
  - 數值類型: REG_SZ 的清單
  ##### 範例值:
```
SOFTWARE\Policies\Microsoft\Edge\PopupsAllowedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\PopupsAllowedForUrls\1 = "[*.]contoso.edu"

```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: PopupsAllowedForUrls
  - 範例值:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### PopupsBlockedForUrls
  #### 封鎖特定網站上的快顯視窗
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  根據 URL 模式，定義開啟快顯視窗功能受封鎖的網站清單。

如果您未設定這個原則，所有網站都將使用來自 [DefaultPopupsSetting](#defaultpopupssetting) 原則 (如有設定) 或使用者個人設定的全域預設值。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  字串的清單

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: PopupsBlockedForUrls
  - GP 名稱: 封鎖特定網站上的快顯視窗
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/內容設定
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge\PopupsBlockedForUrls
  - 路徑 (推薦項目): N/A
  - 值名稱: 1, 2, 3, ...
  - 數值類型: REG_SZ 的清單
  ##### 範例值:
```
SOFTWARE\Policies\Microsoft\Edge\PopupsBlockedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\PopupsBlockedForUrls\1 = "[*.]contoso.edu"

```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: PopupsBlockedForUrls
  - 範例值:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### RegisteredProtocolHandlers
  #### 登錄通訊協定處理常式
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  登錄通訊協定處理常式清單。將協定屬性設定為配置 (如 [mailto])，將 URL 屬性設定為處理該配置的 URL 應用程式模式。該模式可包含 [%s]，其可由處理過的 URL 替換。

您可以為此原則推薦特定值，但不能要求使用者使用其值。

由原則登錄的處理常式可與由使用者登錄的任何處理常式合併，且兩者皆可使用。使用者可以透過安裝新的預設處理常式來覆寫原則安裝的協定處理常式，但無法移除原則登錄的協定處理常式。

  #### 支援功能:
  - 可以是強制: 否
  - 可以建議: 是
  - 動態原則重新整理: 否 - 需要重新啟動瀏覽器

  #### 資料類型:
  字典

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: RegisteredProtocolHandlers
  - GP 名稱: 登錄通訊協定處理常式
  - GP 路徑 (強制): N/A
  - GP 路徑 (推薦項目): 系統管理範本/Microsoft Edge - 預設設定 (使用者可以覆寫)/內容設定
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): N/A
  - 路徑 (推薦項目): SOFTWARE\Policies\Microsoft\Edge\推薦項目
  - 值名稱: RegisteredProtocolHandlers
  - 數值類型: REG_SZ
  ##### 範例值:
```
SOFTWARE\Policies\Microsoft\Edge\RegisteredProtocolHandlers = [
  {
    "default": true, 
    "protocol": "mailto", 
    "url": "https://mail.contoso.com/mail/?extsrc=mailto&url=%s"
  }
]
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: RegisteredProtocolHandlers
  - 範例值:
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
  

  [回到頂端](#microsoft-edge---原則)

  ### WebUsbAllowDevicesForUrls
  #### 授與特定網站連線到特定 USB 裝置的存取權
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  可讓您設定一組 URL，指定會自動獲得具指定廠商和產品識別碼之 USB 裝置存取權的站台。清單中的所有項目都必須包含裝置和 URL，原則才會有像。裝置中的所有項目都能包含廠商識別碼和產品識別碼欄位。受到忽略的所有識別碼都會視作萬用字元，但有一個例外: 如果未指定廠商識別碼，就無法指定產品識別碼。否則，原則將不會生效且會受到忽略。

USB 權限模型會使用要求站台的 URL (要求 URL) 和頂層框架站台的 URL (內嵌 URL) 來授與要求 URL 存取 USB 裝置的權限。在 iframe 中載入要求站台時，要求 URL 可能和內嵌 URL 不同。因此，[urls] 欄位最多可包含兩個以逗點分隔的 URL 來分別指定要求與內嵌 URL。如果只有指定一個 URL，則會在要求站台的 URL 符合此 URL 時授與對應 USB 裝置的存取權，而不考慮內嵌狀態。[urls] 中的 URL 必須為有效的 URL，否則原則會受到忽略。

如果未設定此原則，則會對所有站台使用 [DefaultWebUsbGuardSetting](#defaultwebusbguardsetting) 原則 (如有設定) 或使用者個人設定 (如未設定前者) 的全域預設值。

這個原則中的 URL 模式不應與透過 [WebUsbBlockedForUrls](#webusbblockedforurls) 設定的 URL 模式衝突。如果發生衝突，此原則將優先於 [WebUsbBlockedForUrls](#webusbblockedforurls) 和 [WebUsbAskForUrls](#webusbaskforurls)。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  字典

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: WebUsbAllowDevicesForUrls
  - GP 名稱: 授與特定網站連線到特定 USB 裝置的存取權
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/內容設定
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: WebUsbAllowDevicesForUrls
  - 數值類型: REG_SZ
  ##### 範例值:
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


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: WebUsbAllowDevicesForUrls
  - 範例值:
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
  

  [回到頂端](#microsoft-edge---原則)

  ### WebUsbAskForUrls
  #### 在特定站台上允許 WebUSB
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  根據 URL 模式，定義可以要求使用者存取 USB 裝置的網站清單。

如果您未設定這個原則，所有網站都將使用來自 [DefaultWebUsbGuardSetting](#defaultwebusbguardsetting) 原則 (如有設定) 或使用者個人設定的全域預設值。

URL 模式在此原則中的定義不會與 [WebUsbBlockedForUrls](#webusbblockedforurls) 原則中的設定相衝突 - 您不能同時允許和封鎖一個 URL。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  字串的清單

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: WebUsbAskForUrls
  - GP 名稱: 在特定站台上允許 WebUSB
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/內容設定
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge\WebUsbAskForUrls
  - 路徑 (推薦項目): N/A
  - 值名稱: 1, 2, 3, ...
  - 數值類型: REG_SZ 的清單
  ##### 範例值:
```
SOFTWARE\Policies\Microsoft\Edge\WebUsbAskForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\WebUsbAskForUrls\1 = "[*.]contoso.edu"

```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: WebUsbAskForUrls
  - 範例值:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### WebUsbBlockedForUrls
  #### 封鎖特定網站上的 WebUSB
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  根據 URL 模式，定義無法要求使用者授予 USB 裝置存取權限的網站清單。

如果您未設定這個原則，所有網站都將使用來自 [DefaultWebUsbGuardSetting](#defaultwebusbguardsetting) 原則 (如有設定) 或使用者個人設定的全域預設值。

URL 模式在此原則中的定義不會與 [WebUsbAskForUrls](#webusbaskforurls) 原則中的設定相衝突。您不能同時允許和封鎖一個 URL。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  字串的清單

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: WebUsbBlockedForUrls
  - GP 名稱: 封鎖特定網站上的 WebUSB
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/內容設定
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge\WebUsbBlockedForUrls
  - 路徑 (推薦項目): N/A
  - 值名稱: 1, 2, 3, ...
  - 數值類型: REG_SZ 的清單
  ##### 範例值:
```
SOFTWARE\Policies\Microsoft\Edge\WebUsbBlockedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\WebUsbBlockedForUrls\1 = "[*.]contoso.edu"

```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: WebUsbBlockedForUrls
  - 範例值:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [回到頂端](#microsoft-edge---原則)

  ## 列印 policies

  [回到頂端](#microsoft-edge---原則)

  ### DefaultPrinterSelection
  #### 預設印表機選取規則
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  覆寫 Microsoft Edge 預設印表機選取規則。此原則會決定 Microsoft Edge 中預設印表機的選取規則，當使用者嘗試列印網頁時將會第一次發生。

此原則設定時，Microsoft Edge 會嘗試尋找所有符合指定屬性的印表機，並將其作為預設印表機。如果沒有多台符合條件的印表機，則會使用第一個符合的印表機。

如果您未設定此原則，或在逾時內找不到任何相符的印表機，印表機將預設為內建 PDF 印表機，如果 PDF 印表機無法使用，則會設定為沒有印表機。

數值剖析為 JSON 物件，確認下列結構描述: { "type": "object", "properties": { "idPattern": { "description": "Regular expression to match printer id.", "type": "string" }, "namePattern": { "description": "Regular expression to match printer display name.", "type": "string" } } }

省略欄位則表示所有值都符合;例如如果未指定連線，[列印預覽] 將開始探索所有類型的本機印表機。規則運算式模式必須遵守 JavaScript RegExp 語法，且配對會區分大小寫。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  字串

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: DefaultPrinterSelection
  - GP 名稱: 預設印表機選取規則
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/列印
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: DefaultPrinterSelection
  - 數值類型: REG_SZ
  ##### 範例值:
```
"{ "idPattern": ".*public", "namePattern": ".*Color" }"
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: DefaultPrinterSelection
  - 範例值:
``` xml
<string>{ "idPattern": ".*public", "namePattern": ".*Color" }</string>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### PrintHeaderFooter
  #### 列印頁首與頁尾
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  在列印對話方塊中強制打開或關閉 [頁首與頁尾]。

如果不設定此原則，使用者可以決定是否列頁首與頁尾。

如果停用此原則，則使用者無法列頁首與頁尾。

如果啟用此原則，使用者一律列印頁首和頁尾。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 是
  - 動態原則重新整理: 是

  #### 資料類型:
  布林值

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: PrintHeaderFooter
  - GP 名稱: 列印頁首與頁尾
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/列印
  - GP 路徑 (推薦項目): 系統管理範本/Microsoft Edge - 預設設定 (使用者可以覆寫)/列印
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): SOFTWARE\Policies\Microsoft\Edge\推薦項目
  - 值名稱: PrintHeaderFooter
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000000
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: PrintHeaderFooter
  - 範例值:
``` xml
<false/>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### PrintPreviewUseSystemDefaultPrinter
  #### 將系統預設的印表機設定為預設印表機
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  要求 Microsoft Edge 使用系統預設印表機作為 [列印預覽] 預設選擇，而非最近使用的印表機。

如果您停用此原則或未設定，[列印預覽] 會使用最近使用的印表機作為預設目的地選項。

如果您啟用此原則，[列印預覽] 使用 OS 系統預設印表機作為預設目的地選項。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 是
  - 動態原則重新整理: 是

  #### 資料類型:
  布林值

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: PrintPreviewUseSystemDefaultPrinter
  - GP 名稱: 將系統預設的印表機設定為預設印表機
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/列印
  - GP 路徑 (推薦項目): 系統管理範本/Microsoft Edge - 預設設定 (使用者可以覆寫)/列印
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): SOFTWARE\Policies\Microsoft\Edge\推薦項目
  - 值名稱: PrintPreviewUseSystemDefaultPrinter
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000000
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: PrintPreviewUseSystemDefaultPrinter
  - 範例值:
``` xml
<false/>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### PrintingEnabled
  #### 啟用列印
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  啟用 Microsoft Edge  中的列印功能，並防止使用者變更此設定。

如果您啟用此原則或未設定，使用者將可以列印。

如果您停用此原則，則使用者無法從 Microsoft Edge 列印。列印功能已於扳手功能表、擴充功能、JavaScript 應用程式等功能中停用。使用者仍可以從略過的 Microsoft Edge 外掛程式列印。例如，特定 Adobe Flash 應用程式已在其內容功能表中，此原則不涵蓋。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  布林值

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: PrintingEnabled
  - GP 名稱: 啟用列印
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/列印
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: PrintingEnabled
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000001
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: PrintingEnabled
  - 範例值:
``` xml
<true/>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### UseSystemPrintDialog
  #### 列印使用系統列印對話方塊
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  顯示系統列印對話方塊，而非預覽列印。

如果您啟用此原則，當使用者列印網頁時 Microsoft Edge 會開啟，而非內建預覽。

如果您未設定或停用此原則，列印命令會造成 Microsoft Edge 列印預覽畫面顯示。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 否 - 需要重新啟動瀏覽器

  #### 資料類型:
  布林值

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: UseSystemPrintDialog
  - GP 名稱: 列印使用系統列印對話方塊
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/列印
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: UseSystemPrintDialog
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000000
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: UseSystemPrintDialog
  - 範例值:
``` xml
<false/>
```
  

  [回到頂端](#microsoft-edge---原則)

  ## 原生訊息 policies

  [回到頂端](#microsoft-edge---原則)

  ### NativeMessagingAllowlist
  #### 原生訊息中心裝載使用者可以使用的控制項
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  列出使用者可在 Microsoft Edge 中使用的特定原生訊息主機。

根據預設，允許所有原生訊息的主機。如果您設定 [NativeMessagingBlocklist](#nativemessagingblocklist) 原則為 *，將會封鎖所有原生訊息的主機，而且會載入列在這裡的原生傳訊主機。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  字串的清單

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: NativeMessagingAllowlist
  - GP 名稱: 原生訊息中心裝載使用者可以使用的控制項
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/原生訊息
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge\NativeMessagingAllowlist
  - 路徑 (推薦項目): N/A
  - 值名稱: 1, 2, 3, ...
  - 數值類型: REG_SZ 的清單
  ##### 範例值:
```
SOFTWARE\Policies\Microsoft\Edge\NativeMessagingAllowlist\0 = "com.native.messaging.host.name1"
SOFTWARE\Policies\Microsoft\Edge\NativeMessagingAllowlist\1 = "com.native.messaging.host.name2"

```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: NativeMessagingAllowlist
  - 範例值:
``` xml
<array>
  <string>com.native.messaging.host.name1</string>
  <string>com.native.messaging.host.name2</string>
</array>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### NativeMessagingBlocklist
  #### 設定原生訊息中心的封鎖清單
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  指定不該使用哪一個原生傳訊主機。

除非明確列入允許清單，否則使用 [*] 封鎖所有原生訊息的主機。

如果您未設定此原則，Microsoft Edge 將載入所有已安裝的原生訊息主機。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  字串的清單

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: NativeMessagingBlocklist
  - GP 名稱: 設定原生訊息中心的封鎖清單
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/原生訊息
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge\NativeMessagingBlocklist
  - 路徑 (推薦項目): N/A
  - 值名稱: 1, 2, 3, ...
  - 數值類型: REG_SZ 的清單
  ##### 範例值:
```
SOFTWARE\Policies\Microsoft\Edge\NativeMessagingBlocklist\0 = "com.native.messaging.host.name1"
SOFTWARE\Policies\Microsoft\Edge\NativeMessagingBlocklist\1 = "com.native.messaging.host.name2"

```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: NativeMessagingBlocklist
  - 範例值:
``` xml
<array>
  <string>com.native.messaging.host.name1</string>
  <string>com.native.messaging.host.name2</string>
</array>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### NativeMessagingUserLevelHosts
  #### 允許使用者層級的原生訊息中心主機 (無需系統管理員權限即可安裝)
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  啟用原生訊息主機的使用者層級安裝。

如果您停用此原則，Microsoft Edge 將只會使用安裝於系統層級上的原生傳訊主機。

根據預設，如果您未設定此原則，Microsoft Edge 將允許使用者層級的原生傳訊主機的使用方式。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  布林值

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: NativeMessagingUserLevelHosts
  - GP 名稱: 允許使用者層級的原生訊息中心主機 (無需系統管理員權限即可安裝)
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/原生訊息
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: NativeMessagingUserLevelHosts
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000000
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: NativeMessagingUserLevelHosts
  - 範例值:
``` xml
<false/>
```
  

  [回到頂端](#microsoft-edge---原則)

  ## 啟動、首頁和新索引標籤頁面 policies

  [回到頂端](#microsoft-edge---原則)

  ### HomepageIsNewTabPage
  #### 將新的索引標籤頁面設定為 [首頁]
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  設定 Microsoft Edge 中的預設首頁。您可以將首頁頁面設定為 URL 或新索引標籤頁面。

如果您啟用此原則，則 首頁頁面將永遠使用新的索引標籤頁面，將會忽略首頁頁面的 URL 位置。

如果您停用此原則，使用者首頁頁面不可為新索引標籤頁面，除非 URL 設定為 [edge://newtab]。

如果未設定，則使用者可以選擇新索引標籤頁面是否為自己的首頁。

此原則僅適用於已加入至 Microsoft Active Directory 網域的 Windows 執行個體，或已註冊為裝置管理的 Windows 10 專業版或企業的執行個體。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 是
  - 動態原則重新整理: 是

  #### 資料類型:
  布林值

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: HomepageIsNewTabPage
  - GP 名稱: 將新的索引標籤頁面設定為 [首頁]
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/啟動、首頁和新索引標籤頁面
  - GP 路徑 (推薦項目): 系統管理範本/Microsoft Edge - 預設設定 (使用者可以覆寫)/啟動、首頁和新索引標籤頁面
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): SOFTWARE\Policies\Microsoft\Edge\推薦項目
  - 值名稱: HomepageIsNewTabPage
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000001
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: HomepageIsNewTabPage
  - 範例值:
``` xml
<true/>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### HomepageLocation
  #### 設定首頁頁面 URL
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  在 Microsoft Edge 中設定預設首頁 URL。

首頁可透過 [首頁] 按鈕開啟。在啟動時開啟的網頁受 [RestoreOnStartup](#restoreonstartup) 原則控制。

您可以在此處設定 URL 或設定首頁，以開啟新索引標籤頁面。如果您選擇開啟新索引標籤頁面，此原則將不會生效。

如果您啟用此原則，則使用者無法變更其首頁的 URL，但可以選擇使用新索引標籤頁作為首頁。

如果您停用或未設定此原則，只要 [HomepageIsNewTabPage](#homepageisnewtabpage) 原則未啟用，使用者可以自行選擇首頁頁面。

這個原則僅適用於已加入 Microsoft Active Directory 網域或已註冊裝置管理的 Windows 10 專業版或企業版的 Windows 執行個體。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 是
  - 動態原則重新整理: 是

  #### 資料類型:
  字串

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: HomepageLocation
  - GP 名稱: 設定首頁頁面 URL
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/啟動、首頁和新索引標籤頁面
  - GP 路徑 (推薦項目): 系統管理範本/Microsoft Edge - 預設設定 (使用者可以覆寫)/啟動、首頁和新索引標籤頁面
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): SOFTWARE\Policies\Microsoft\Edge\推薦項目
  - 值名稱: HomepageLocation
  - 數值類型: REG_SZ
  ##### 範例值:
```
"https://www.contoso.com"
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: HomepageLocation
  - 範例值:
``` xml
<string>https://www.contoso.com</string>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### NewTabPageCompanyLogo
  #### 設定新索引標籤頁面公司標誌
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (79 版或更新版本)

  #### 描述
  指定要在 Microsoft Edge 中新索引標籤頁面上使用的公司標誌。

原則應設定為能在 JSON 格式中表示標誌的字串。範例: { "default_logo": { "url": "https://www.contoso.com/logo.png", "hash": "cd0aa9856147b6c5b4ff2b7dfee5da20aa38253099ef1b4a64aced233c9afe29" }, "light_logo": { "url": "https://www.contoso.com/light_logo.png", "hash": "517d286edb416bb2625ccfcba9de78296e90da8e32330d4c9c8275c4c1c33737" } }

您可以指定 Microsoft Edge 能下載標誌及其用於驗證下載完整性的加密編譯雜湊 (SHA-256)，來設定此原則。標誌必須為 PNG 或 SVG 格式，且大小不得超過 16 MB。系統會下載並快取標誌，並在 URL 或雜湊變更時重新下載。URL 必須能在不經任何驗證的情況下開放存取。

'default_logo' 為必要項，且會在沒有背景影像時使用。如果提供 'light_logo'，則會在使用者的新索引標籤頁面有背景影像時使用。建議使用具有向左對齊且垂直置中之透明背景的水平標誌。標誌的最低高度為 32 像素，外觀比例應介於 1:1 至 4:1。'default_logo' 應對白/黑背景有適當的對比，而 'light_logo' 應對背景影像有適當的對比。

如果啟用此原則，Microsoft Edge 就會在新的索引標籤頁面上下載並顯示指定的標誌。使用者無法覆寫或隱藏標誌。

如果停用或未設定此原則，Microsoft Edge 將不會在新的索引標籤頁面上顯示任何公司標誌或 Microsoft 標誌。

如需協助了解如何決定 SHA-256 雜湊，請參閱 https://docs.microsoft.com/powershell/module/microsoft.powershell.utility/get-filehash。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 否 - 需要重新啟動瀏覽器

  #### 資料類型:
  字典

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: NewTabPageCompanyLogo
  - GP 名稱: 設定新索引標籤頁面公司標誌
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/啟動、首頁和新索引標籤頁面
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: NewTabPageCompanyLogo
  - 數值類型: REG_SZ
  ##### 範例值:
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


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: NewTabPageCompanyLogo
  - 範例值:
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
  

  [回到頂端](#microsoft-edge---原則)

  ### NewTabPageHideDefaultTopSites
  #### 隱藏新索引標籤頁面中的預設熱門網站
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  從 Microsoft Edge 的新索引標籤頁面隱藏預設上層網站。

如果您設定這個原則為 Tue 時，會隱藏預設排名最前面的網站磚。

如果您將此原則設定為 False 或未設定，預設排名最前面的網站磚保持可見。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  布林值

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: NewTabPageHideDefaultTopSites
  - GP 名稱: 隱藏新索引標籤頁面中的預設熱門網站
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/啟動、首頁和新索引標籤頁面
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: NewTabPageHideDefaultTopSites
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000001
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: NewTabPageHideDefaultTopSites
  - 範例值:
``` xml
<true/>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### NewTabPageLocation
  #### 設定新索引標籤頁面 URL
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  設定新索引標籤頁面的預設 URL。

這個原則會決定在新的索引標籤建立後 (包含開啟新視窗) 會開啟的頁面。如果設定為開起至新的索引標籤頁面，則這也會影響啟動頁面。

這個原則不會決定啟動時要開啟的頁面，這將由 [RestoreOnStartup](#restoreonstartup) 原則決定。此外，如果此原則設定為開啟至新的索引標籤頁面，則不會影響首頁。

如果未設定此原則，則會使用預設新索引標籤頁面。

如果同時設定此原則 *與* [NewTabPageSetFeedType](#newtabpagesetfeedtype) 原則，則此原則優先。

如果提供的 URL 無效，新的索引標籤會開啟 about://blank。

這個原則僅適用於加入 Microsoft Active Directory 網域的 Windows 執行個體，或已註冊裝置管理的 Windows 10 專業版/企業版執行個體。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 是
  - 動態原則重新整理: 是

  #### 資料類型:
  字串

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: NewTabPageLocation
  - GP 名稱: 設定新索引標籤頁面 URL
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/啟動、首頁和新索引標籤頁面
  - GP 路徑 (推薦項目): 系統管理範本/Microsoft Edge - 預設設定 (使用者可以覆寫)/啟動、首頁和新索引標籤頁面
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): SOFTWARE\Policies\Microsoft\Edge\推薦項目
  - 值名稱: NewTabPageLocation
  - 數值類型: REG_SZ
  ##### 範例值:
```
"https://www.fabrikam.com"
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: NewTabPageLocation
  - 範例值:
``` xml
<string>https://www.fabrikam.com</string>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### NewTabPageManagedQuickLinks
  #### 設定新的索引標籤頁面快速連結
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (79 版或更新版本)

  #### 描述
  在預設情況下，Microsoft Edge 會根據瀏覽歷程記錄，在新索引標籤頁面上顯示使用者新增的捷徑和熱門網站的快速連結。使用此原則，您可以在新索引標籤頁面上最多設定三個快速連結磚，以 JSON 物件表示：

[ { "url": "https://www.contoso.com", "title": "Contoso Portal", "pinned": true/false }, ... ]

需填寫 [url] 欄；[標題] 和 [已釘選] 可選填。如果未提供 [標題]，則會使用 URL 作為預設標題。如果未提供 [已釘選]，則預設值為 False。

Microsoft Edge 會以列出的順序由左至右顯示這些內容，所有已釘選磚皆顯示在非釘選磚前方。

如果此原則設為必填，則忽略 [已釘選] 欄位，並釘選所有磚。使用者無法刪除這些磚，且這些磚將一律顯示在快速連結清單的前方。

如果按建議設定此原則，則已釘選磚將保留在清單中，但使用者可以進行編輯和刪除。未釘選的快速連結磚的功能類似於預設熱門網站，如果其他網站瀏覽得更頻繁，則快速連結磚將從清單中移除。透過此原則將非釘選連結套用至現有瀏覽器設定檔時，連結可能根本不會顯示，這取決於其與使用者瀏覽歷程記錄相比的排名。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 是
  - 動態原則重新整理: 否 - 需要重新啟動瀏覽器

  #### 資料類型:
  字典

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: NewTabPageManagedQuickLinks
  - GP 名稱: 設定新的索引標籤頁面快速連結
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/啟動、首頁和新索引標籤頁面
  - GP 路徑 (推薦項目): 系統管理範本/Microsoft Edge - 預設設定 (使用者可以覆寫)/啟動、首頁和新索引標籤頁面
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): SOFTWARE\Policies\Microsoft\Edge\推薦項目
  - 值名稱: NewTabPageManagedQuickLinks
  - 數值類型: REG_SZ
  ##### 範例值:
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


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: NewTabPageManagedQuickLinks
  - 範例值:
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
  

  [回到頂端](#microsoft-edge---原則)

  ### NewTabPageSetFeedType
  #### 設定 Microsoft Edge 的新索引標籤頁面體驗
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (79 版或更新版本)

  #### 描述
  可讓您為新索引標籤頁選擇 Microsoft News 或 Office 365 摘要體驗。

將此原則設定為 Microsoft News 摘要體驗 (0) 時，使用者將在新索引標籤頁上看到 Microsoft News 摘要體驗。

將此原則設定為 Office 365 摘要體驗 (1) 時，具有 Azure Active Directory 瀏覽器登入的使用者將在新索引標籤頁上看到 Office 365 摘要體驗。

如果停用或未設定此原則:

-具有 Azure Active Directory 瀏覽器登入的使用者能享有 Office 365 新索引標籤頁摘要體驗，以及標準的新索引標籤頁摘要體驗。

-沒有 Azure Active Directory 瀏覽器登入的使用者將看到標準新索引標籤頁摘要體驗。

如果設定此原則，*並且* [NewTabPageLocation](#newtabpagelocation) 原則，[NewTabPageLocation](#newtabpagelocation) 具有優先順序。

預設設定: 已停用或未設定。

* 0 = Microsoft News 摘要體驗

* 1 = Office 365 摘要體驗

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 是
  - 動態原則重新整理: 是

  #### 資料類型:
  整數

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: NewTabPageSetFeedType
  - GP 名稱: 設定 Microsoft Edge 的新索引標籤頁面體驗
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/啟動、首頁和新索引標籤頁面
  - GP 路徑 (推薦項目): 系統管理範本/Microsoft Edge - 預設設定 (使用者可以覆寫)/啟動、首頁和新索引標籤頁面
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): SOFTWARE\Policies\Microsoft\Edge\推薦項目
  - 值名稱: NewTabPageSetFeedType
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000000
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: NewTabPageSetFeedType
  - 範例值:
``` xml
<integer>0</integer>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### RestoreOnStartup
  #### 啟動時所採取的動作
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  指定開始時的 Microsoft Edge 行為。

如果您想要在啟動時永遠開啟，請選擇 [開啟新索引標籤] (5)。

如果您想要重新開啟上次 Microsoft Edge 關閉時的 URL，請選擇 [還原上次工作階段] (1)。瀏覽工作階段將會還原成原本的樣子。請注意，此選項會停用某些設定的依賴工作階段或結束時執行的動作 (例如在結束或專用工作階段 Cookie 清除瀏覽資料)。

如果您想要開啟一組特定 URL，選擇 [開啟 URL 清單] (4)。

停用此設定相當保持未設定。使用者將能在 Microsoft Edge 中變更。

此原則僅適用於已加入 Microsoft Active Directory 網域的 Windows 執行個體，或已註冊裝置管理的 Windows 10 專業版或企業版的執行個體。

* 5 = 開啟新索引標籤

* 1 = 還原上次的工作階段

* 4 = 開啟 URL 清單

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 是
  - 動態原則重新整理: 是

  #### 資料類型:
  整數

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: RestoreOnStartup
  - GP 名稱: 啟動時所採取的動作
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/啟動、首頁和新索引標籤頁面
  - GP 路徑 (推薦項目): 系統管理範本/Microsoft Edge - 預設設定 (使用者可以覆寫)/啟動、首頁和新索引標籤頁面
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): SOFTWARE\Policies\Microsoft\Edge\推薦項目
  - 值名稱: RestoreOnStartup
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000004
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: RestoreOnStartup
  - 範例值:
``` xml
<integer>4</integer>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### RestoreOnStartupURLs
  #### 瀏覽器啟動時開啟的網站
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  指定瀏覽器啟動時自動開啟的網站清單。如果不設定此原則，則啟動時不會開啟任何網站。

此原則僅在同時設定 'Open a list of URLs' (4) [RestoreOnStartup](#restoreonstartup) 原則時才有效。

此原則僅適用於加入 Microsoft Active Directory 網域的 Windows 執行個體、Windows 10 專業版或註冊裝置管理的企業版執行個體。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 是
  - 動態原則重新整理: 是

  #### 資料類型:
  字串的清單

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: RestoreOnStartupURLs
  - GP 名稱: 瀏覽器啟動時開啟的網站
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/啟動、首頁和新索引標籤頁面
  - GP 路徑 (推薦項目): 系統管理範本/Microsoft Edge - 預設設定 (使用者可以覆寫)/啟動、首頁和新索引標籤頁面
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge\RestoreOnStartupURLs
  - 路徑 (推薦項目): SOFTWARE\Policies\Microsoft\Edge\推薦項目\RestoreOnStartupURLs
  - 值名稱: 1, 2, 3, ...
  - 數值類型: REG_SZ 的清單
  ##### 範例值:
```
SOFTWARE\Policies\Microsoft\Edge\RestoreOnStartupURLs\0 = "https://contoso.com"
SOFTWARE\Policies\Microsoft\Edge\RestoreOnStartupURLs\1 = "https://www.fabrikam.com"

```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: RestoreOnStartupURLs
  - 範例值:
``` xml
<array>
  <string>https://contoso.com</string>
  <string>https://www.fabrikam.com</string>
</array>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### ShowHomeButton
  #### 在工具列上顯示 [首頁] 按鈕
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  在 Microsoft Edge 的工具列上顯示 [首頁] 按鈕。

啟用此原則，一律顯示 [首頁] 按鈕。停用後將永遠不會顯示該按鈕。

如果您未設定此原則，則使用者可以選擇是否要顯示首頁按鈕。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 是
  - 動態原則重新整理: 是

  #### 資料類型:
  布林值

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: ShowHomeButton
  - GP 名稱: 在工具列上顯示 [首頁] 按鈕
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/啟動、首頁和新索引標籤頁面
  - GP 路徑 (推薦項目): 系統管理範本/Microsoft Edge - 預設設定 (使用者可以覆寫)/啟動、首頁和新索引標籤頁面
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): SOFTWARE\Policies\Microsoft\Edge\推薦項目
  - 值名稱: ShowHomeButton
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000001
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: ShowHomeButton
  - 範例值:
``` xml
<true/>
```
  

  [回到頂端](#microsoft-edge---原則)

  ## 密碼管理員和防護 policies

  [回到頂端](#microsoft-edge---原則)

  ### PasswordManagerEnabled
  #### 啟用儲存密碼的密碼管理員
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  啟用 Microsoft Edge 以儲存使用者密碼。

如果您啟用這個原則，使用者將密碼儲存在 Microsoft Edge。下次您造訪網站時，Microsoft Edge 將會自動輸入密碼。

如果您停用此原則，則使用者無法儲存新密碼，但仍可以使用先前儲存的密碼。

如果您啟用或停用此原則，則使用者無法在 Microsoft Edge 變更或覆寫。如果您未設定，則使用者可以儲存密碼並關閉此功能。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 是
  - 動態原則重新整理: 是

  #### 資料類型:
  布林值

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: PasswordManagerEnabled
  - GP 名稱: 啟用儲存密碼的密碼管理員
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/密碼管理員和防護
  - GP 路徑 (推薦項目): 系統管理範本/Microsoft Edge - 預設設定 (使用者可以覆寫)/密碼管理員和防護
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): SOFTWARE\Policies\Microsoft\Edge\推薦項目
  - 值名稱: PasswordManagerEnabled
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000001
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: PasswordManagerEnabled
  - 範例值:
``` xml
<true/>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### PasswordProtectionChangePasswordURL
  #### 設定變更密碼 URL
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  設定變更密碼 URL (僅 HTTP 與 HTTPS 配置)。

在瀏覽器中看見警告後，密碼保護服務會傳送使用者至此 URL 變更其密碼。n
如果啟用此原則，則密碼保護服務會傳送使用者至此 URL 變更其密碼。

如果停用或未設定此原則，則密碼保護服務將不會將使用者重新導向至變更密碼 URL。

此原則僅適用於已加入 Microsoft Active Directory 網域的 Windows 執行個體，或已註冊裝置管理的 Windows 10 專業版或企業版執行個體。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  字串

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: PasswordProtectionChangePasswordURL
  - GP 名稱: 設定變更密碼 URL
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/密碼管理員和防護
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: PasswordProtectionChangePasswordURL
  - 數值類型: REG_SZ
  ##### 範例值:
```
"https://contoso.com/change_password.html"
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: PasswordProtectionChangePasswordURL
  - 範例值:
``` xml
<string>https://contoso.com/change_password.html</string>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### PasswordProtectionLoginURLs
  #### 設定密碼保護服務應擷取密碼指紋的企業登入 URL 清單
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  設定企業登入 URL (僅 HTTP 與 HTTPS 配置) 清單，其中 Microsoft Edge 應該擷取密碼指紋，並將其用於密碼重複使用偵測。如果啟用此原則，則密碼保護服務會擷取已定義 URL 上的密碼指紋。

如果停用或未設定此原則，則不會擷取任何密碼指紋。

此原則僅適用於已加入 Microsoft Active Directory 網域的 Windows 執行個體，或已註冊裝置管理的 Windows 10 專業版或企業版執行個體。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  字串的清單

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: PasswordProtectionLoginURLs
  - GP 名稱: 設定密碼保護服務應擷取密碼指紋的企業登入 URL 清單
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/密碼管理員和防護
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge\PasswordProtectionLoginURLs
  - 路徑 (推薦項目): N/A
  - 值名稱: 1, 2, 3, ...
  - 數值類型: REG_SZ 的清單
  ##### 範例值:
```
SOFTWARE\Policies\Microsoft\Edge\PasswordProtectionLoginURLs\0 = "https://contoso.com/login.html"
SOFTWARE\Policies\Microsoft\Edge\PasswordProtectionLoginURLs\1 = "https://login.contoso.com"

```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: PasswordProtectionLoginURLs
  - 範例值:
``` xml
<array>
  <string>https://contoso.com/login.html</string>
  <string>https://login.contoso.com</string>
</array>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### PasswordProtectionWarningTrigger
  #### 設定密碼保護警告觸發程序
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  可讓您控制何時觸發密碼保護警告。當使用者在潛在可疑的網站上，重複使用受保護的密碼時會警告使用者。

您可以使用 [PasswordProtectionLoginURLs](#passwordprotectionloginurls) 和 [PasswordProtectionChangePasswordURL](#passwordprotectionchangepasswordurl) 原則來設定要保護的密碼。

豁免: [PasswordProtectionLoginURLs](#passwordprotectionloginurls) 和 [PasswordProtectionChangePasswordURL](#passwordprotectionchangepasswordurl) 以及 [SmartScreenAllowListDomains](#smartscreenallowlistdomains) 中列出的網站不會觸發密碼保護警告。

設定為 'PasswordProtectionWarningOff' (0) 不顯示密碼保護警告。

設定為 'PasswordProtectionWarningOnPasswordReuse' (1) 當使用者於非列於允許清單的網站上，重複使用其受保護的密碼時，顯示密碼保護警告。

如果停用或未設定此原則，則不會顯示警告觸發程序。

* 0 =密碼保護警告已關閉。

* 1 = 重複使用密碼觸發密碼保護警告。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  整數

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: PasswordProtectionWarningTrigger
  - GP 名稱: 設定密碼保護警告觸發程序
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/密碼管理員和防護
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: PasswordProtectionWarningTrigger
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000001
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: PasswordProtectionWarningTrigger
  - 範例值:
``` xml
<integer>1</integer>
```
  

  [回到頂端](#microsoft-edge---原則)

  ## 擴充功能 policies

  [回到頂端](#microsoft-edge---原則)

  ### ExtensionAllowedTypes
  #### 設定允許的延伸模組類型
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  控制哪些延伸模組類型可以安裝，並會限制存取執行階段。

這個設定會定義的延伸模組和允許的類型可以互動的主機。值是字串的清單，其中每一個應該是下列其中一個清單: "extension"、"theme"、"user_script" 和 "hosted_app"。如需有關這些類型的延伸模組文件，請參閱 Microsoft Edge。

這個原則也會影響延伸模組為強制安裝使用的附註 [ExtensionInstallForcelist](#extensioninstallforcelist) 原則。

如果您啟用這個原則，就只會安裝清單中符合類型的延伸模組。

如果您未設定這個原則，會強制執行的可接受的延伸模組類型沒有限制。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  字串的清單

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: ExtensionAllowedTypes
  - GP 名稱: 設定允許的延伸模組類型
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/擴充功能
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge\ExtensionAllowedTypes
  - 路徑 (推薦項目): N/A
  - 值名稱: 1, 2, 3, ...
  - 數值類型: REG_SZ 的清單
  ##### 範例值:
```
SOFTWARE\Policies\Microsoft\Edge\ExtensionAllowedTypes\0 = "hosted_app"

```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: ExtensionAllowedTypes
  - 範例值:
``` xml
<array>
  <string>hosted_app</string>
</array>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### ExtensionInstallAllowlist
  #### 允許特定安裝擴充功能
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  根據預設，允許所有擴充功能。不過如果您透過設定 [ExtensionInstallBlockList] 原則為「*」封鎖所有擴充功能，則使用者只能安裝在此原則中定義的擴充功能。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  字串的清單

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: ExtensionInstallAllowlist
  - GP 名稱: 允許特定安裝擴充功能
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/擴充功能
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallAllowlist
  - 路徑 (推薦項目): N/A
  - 值名稱: 1, 2, 3, ...
  - 數值類型: REG_SZ 的清單
  ##### 範例值:
```
SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallAllowlist\0 = "extension_id1"
SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallAllowlist\1 = "extension_id2"

```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: ExtensionInstallAllowlist
  - 範例值:
``` xml
<array>
  <string>extension_id1</string>
  <string>extension_id2</string>
</array>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### ExtensionInstallBlocklist
  #### 控制不能安裝哪些擴充程式
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  列出使用者無法安裝於 Microsoft Edge 內的特定擴充功能。當您部署此原則時，將會停用此清單上曾安裝的所有擴充功能，而且使用者將無法啟用。如果您移除封鎖擴充功能清單中的項目，該擴充功能會於之前安裝的位置自動重新啟用。

使用「*」封鎖所有未明確列於允許清單中的擴充功能。

如果您未設定此原則，使用者可以在 Microsoft Edge 中安裝所有擴充功能。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  字串的清單

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: ExtensionInstallBlocklist
  - GP 名稱: 控制不能安裝哪些擴充程式
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/擴充功能
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallBlocklist
  - 路徑 (推薦項目): N/A
  - 值名稱: 1, 2, 3, ...
  - 數值類型: REG_SZ 的清單
  ##### 範例值:
```
SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallBlocklist\0 = "extension_id1"
SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallBlocklist\1 = "extension_id2"

```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: ExtensionInstallBlocklist
  - 範例值:
``` xml
<array>
  <string>extension_id1</string>
  <string>extension_id2</string>
</array>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### ExtensionInstallForcelist
  #### 控制哪些擴充功能會默默地安裝
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  指定不需使用者互動以無訊息模式且已安裝的延伸模組，而且使用者無法解除安裝，或停用 ("force-installed")。所有延伸模組請求的權限皆為隱含式授與，且無需使用者互動，包括其他任何延伸模組的未來版本所要求的權限。此外，將為 enterprise.deviceAttributes 和 enterprise.platformKeys 延伸模組 API 授予權限。(這兩個 Api 僅適用於強制安裝的延伸模組)。

此原則的優先順序高於潛在衝突的 [ExtensionInstallBlocklist](#extensioninstallblocklist) 原則。當您從強制安裝清單中移除延伸模組時，其會由 Microsoft Edge 自動解除安裝。

未加入 Windows 裝置的 Microsoft Active Directory 網域，強制安裝僅限 Microsoft Store 中可用的延伸模組。

請注意，使用者將能夠使用開發人員工具，修改任何延伸模組的原始碼，這可能導致延伸模組異常。若會產生此問題，請設定 [DeveloperToolsAvailability](#developertoolsavailability) 原則。

透過下列格式將延伸模組新增到清單中:

[extensionID];[updateURL]



[extensionID];[updateURL]

- extensionID - 在 edge://extensions 上找到的 32 個字母字串。

-updateURL (可省略) 為在 [https://go.microsoft.com/fwlink/?linkid=2095043](https://go.microsoft.com/fwlink/?linkid=2095043) 所述的應用程式或延伸模組更新資訊清單 XML 文件位址。如果未設定 updateURL，則使用 Microsoft Store 更新 URL (目前為 https://edge.microsoft.com/extensionwebstorebase/v1/crx)。請注意，此原則中設定的更新 URL 僅用於初始安裝。延伸模組的後續更新將使用延伸模組資訊清單中指示的更新 URL。

例如，gggmmkjegpiggikcnhidnjjhmicpibll;https://edge.microsoft.com/extensionwebstorebase/v1/crx 從 Microsoft Store [更新] URL 安裝 Microsoft Online 應用程式。有關裝載延伸模組的詳細資訊，請參閱: [https://go.microsoft.com/fwlink/?linkid=2095044](https://go.microsoft.com/fwlink/?linkid=2095044)。

如果未設定此原則，則不會自動安裝任何延伸模組，且使用者可以在 Microsoft Edge 中解除安裝任何延伸模組。

請注意，這個原則不適用於 InPrivate 模式。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  字串的清單

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: ExtensionInstallForcelist
  - GP 名稱: 控制哪些擴充功能會默默地安裝
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/擴充功能
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallForcelist
  - 路徑 (推薦項目): N/A
  - 值名稱: 1, 2, 3, ...
  - 數值類型: REG_SZ 的清單
  ##### 範例值:
```
SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallForcelist\0 = "gbchcmhmhahfdphkhkmpfmihenigjmpp;https://edge.microsoft.com/extensionwebstorebase/v1/crx"
SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallForcelist\1 = "abcdefghijklmnopabcdefghijklmnop"

```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: ExtensionInstallForcelist
  - 範例值:
``` xml
<array>
  <string>gbchcmhmhahfdphkhkmpfmihenigjmpp;https://edge.microsoft.com/extensionwebstorebase/v1/crx</string>
  <string>abcdefghijklmnopabcdefghijklmnop</string>
</array>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### ExtensionInstallSources
  #### 設定擴充功能與使用者指令碼安裝來源
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  定義可以安裝延伸模組和佈景主題的 Url。

根據預設，使用者必須為想要安裝的每個延伸模組或指令碼下載 *.crx 檔案，並將其拖曳至 Microsoft Edge 設定頁面。這個原則可讓特定的 Url 使用安裝的延伸模組或使用者的指令碼。

在這個清單中的每個項目是延伸樣式比對模式 (請參閱 [https://go.microsoft.com/fwlink/?linkid=2095039](https://go.microsoft.com/fwlink/?linkid=2095039))。使用者可以輕鬆從符合此清單內項目的 URL 安裝項目。*.crx 檔案與下載開始頁面 (即轉介者) 的位置，都必須有這些模式的允許。

[ExtensionInstallBlocklist](#extensioninstallblocklist) 原則的優先順序高於這個原則。將不會安裝封鎖清單的任何延伸模組，即使它來自此清單上的網站也一樣。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  字串的清單

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: ExtensionInstallSources
  - GP 名稱: 設定擴充功能與使用者指令碼安裝來源
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/擴充功能
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallSources
  - 路徑 (推薦項目): N/A
  - 值名稱: 1, 2, 3, ...
  - 數值類型: REG_SZ 的清單
  ##### 範例值:
```
SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallSources\0 = "https://corp.contoso.com/*"

```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: ExtensionInstallSources
  - 範例值:
``` xml
<array>
  <string>https://corp.contoso.com/*</string>
</array>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### ExtensionSettings
  #### 設定擴充功能管理設定
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  設定 Microsoft Edge 的擴充功能管理設定。

此原則可控制多個設定，其中包含由所有現有的擴充功能相關原則所控制的設定。如果同時設定此原將會覆寫所有舊版原則。

此原則對應擴充功能識別碼或更新 URL 至其設定。透過擴充功能識別碼，設定將只會套用至指定括功能。設定特殊識別碼「*」的預設設定，套用到所有未特別列出原則的擴充功能。使用更新 URL，設定將用於所有擴充功能，而且此擴充功能在功能清單中帶有明確的更新內容，如 [https://go.microsoft.com/fwlink/?linkid=2095043](https://go.microsoft.com/fwlink/?linkid=2095043) 所述。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  字典

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: ExtensionSettings
  - GP 名稱: 設定擴充功能管理設定
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/擴充功能
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: ExtensionSettings
  - 數值類型: REG_SZ
  ##### 範例值:
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


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: ExtensionSettings
  - 範例值:
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
  

  [回到頂端](#microsoft-edge---原則)

  ## 預設搜尋提供者 policies

  [回到頂端](#microsoft-edge---原則)

  ### DefaultSearchProviderEnabled
  #### 啟用預設搜尋提供者
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  允許使用預設搜尋提供者。

如果啟用此原則，使用者可以在網址列中輸入字詞進行搜尋 (只要輸入的內容不是 URL)。

您可以透過啟用其餘預設搜尋原則來指定要使用的預設搜尋提供者。如果保留空白 (不設定)，則使用者可以選擇預設提供者。

如果停用此原則，則使用者無法從網址列進行搜尋。

如果啟用或停用此原則，則使用者將無法進行變更或覆寫。

如果不設定此原則，則啟用預設搜尋提供者，使用者可以選擇預設搜尋提供者並設定搜尋提供者列表。

此原則僅適用於已加入 Microsoft Active Directory 網域的 Windows 執行個體，或已註冊裝置管理的 Windows 10 專業版及 Windows 10 企業版執行個體。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  布林值

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: DefaultSearchProviderEnabled
  - GP 名稱: 啟用預設搜尋提供者
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/預設搜尋提供者
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: DefaultSearchProviderEnabled
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000001
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: DefaultSearchProviderEnabled
  - 範例值:
``` xml
<true/>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### DefaultSearchProviderEncodings
  #### 預設搜尋提供者編碼
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  指定的搜尋提供者所支援的字元編碼方式。編碼是字碼頁名稱，如 UTF-8、GB2312 和 ISO-8859-1。這些編碼會按提供的順序進行嘗試。

此原則是選擇性的。如果未設定，則使用預設值 UTF-8。

僅在啟用 [DefaultSearchProviderEnabled](#defaultsearchproviderenabled) 和 [DefaultSearchProviderSearchURL](#defaultsearchprovidersearchurl) 原則時，才能套用此原則。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  字串的清單

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: DefaultSearchProviderEncodings
  - GP 名稱: 預設搜尋提供者編碼
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/預設搜尋提供者
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge\DefaultSearchProviderEncodings
  - 路徑 (推薦項目): N/A
  - 值名稱: 1, 2, 3, ...
  - 數值類型: REG_SZ 的清單
  ##### 範例值:
```
SOFTWARE\Policies\Microsoft\Edge\DefaultSearchProviderEncodings\0 = "UTF-8"
SOFTWARE\Policies\Microsoft\Edge\DefaultSearchProviderEncodings\1 = "UTF-16"
SOFTWARE\Policies\Microsoft\Edge\DefaultSearchProviderEncodings\2 = "GB2312"
SOFTWARE\Policies\Microsoft\Edge\DefaultSearchProviderEncodings\3 = "ISO-8859-1"

```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: DefaultSearchProviderEncodings
  - 範例值:
``` xml
<array>
  <string>UTF-8</string>
  <string>UTF-16</string>
  <string>GB2312</string>
  <string>ISO-8859-1</string>
</array>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### DefaultSearchProviderImageURL
  #### 指定預設搜尋提供者的影像搜尋功能
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  指定用於影像搜尋的搜尋引擎 URL。將使用 GET 方法傳送搜尋要求。

此則是選擇性的。如果不設定此原則，則無法使用影像搜尋。

將 Bing 的影像搜尋 URL 指定為:
'{bing:baseURL}images/detail/search?iss=sbiupload&FORM=ANCMS1#enterInsights'。

將 Google 的影像搜尋 URL 指定為: '{google:baseURL}searchbyimage/upload'。

請參閱 [DefaultSearchProviderImageURLPostParams](#defaultsearchproviderimageurlpostparams) 原則以完成設定影像搜尋。

僅在啟用 [DefaultSearchProviderEnabled](#defaultsearchproviderenabled) 和 [DefaultSearchProviderSearchURL](#defaultsearchprovidersearchurl) 原則時，才能套用此原則。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  字串

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: DefaultSearchProviderImageURL
  - GP 名稱: 指定預設搜尋提供者的影像搜尋功能
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/預設搜尋提供者
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: DefaultSearchProviderImageURL
  - 數值類型: REG_SZ
  ##### 範例值:
```
"https://search.contoso.com/searchbyimage/upload"
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: DefaultSearchProviderImageURL
  - 範例值:
``` xml
<string>https://search.contoso.com/searchbyimage/upload</string>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### DefaultSearchProviderImageURLPostParams
  #### 使用 POST 的影像 URL 參數
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  如果啟用此原則，則會指定使用 POST 執行影像搜尋時使用的參數。該原則由逗號分隔的名稱/值組所組成。如果值是範本參數，如前面範例中的{imageThumbnail}，則會以實際影像縮圖資料替換。僅在啟用 [DefaultSearchProviderEnabled](#defaultsearchproviderenabled) 和 [DefaultSearchProviderSearchURL](#defaultsearchprovidersearchurl) 原則時，才能套用此原則。

將 Bing 的影像搜尋 URL Post 參數指定為:
'imageBin={google:imageThumbnailBase64}'。

將 Google 的影像搜尋 URL Post 參數指定為:
'encoded_image={google:imageThumbnail},image_url={google:imageURL},sbisrc={google:imageSearchSource},original_width={google:imageOriginalWidth},original_height={google:imageOriginalHeight}'。

如果未設定此原則，則會使用 GET 方法傳送影像搜尋要求。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  字串

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: DefaultSearchProviderImageURLPostParams
  - GP 名稱: 使用 POST 的影像 URL 參數
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/預設搜尋提供者
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: DefaultSearchProviderImageURLPostParams
  - 數值類型: REG_SZ
  ##### 範例值:
```
"content={imageThumbnail},url={imageURL},sbisrc={SearchSource}"
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: DefaultSearchProviderImageURLPostParams
  - 範例值:
``` xml
<string>content={imageThumbnail},url={imageURL},sbisrc={SearchSource}</string>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### DefaultSearchProviderKeyword
  #### 預設搜尋提供者關鍵字
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  指定關鍵字，也就是在網址列中用來觸發此提供者搜尋的捷徑。

此原則是選擇性的。如果未設定此原則，則不會有關鍵字啟動搜尋提供者。

僅在啟用 [DefaultSearchProviderEnabled](#defaultsearchproviderenabled) 和[DefaultSearchProviderSearchURL](#defaultsearchprovidersearchurl) 原則時，才能套用此原則。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  字串

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: DefaultSearchProviderKeyword
  - GP 名稱: 預設搜尋提供者關鍵字
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/預設搜尋提供者
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: DefaultSearchProviderKeyword
  - 數值類型: REG_SZ
  ##### 範例值:
```
"mis"
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: DefaultSearchProviderKeyword
  - 範例值:
``` xml
<string>mis</string>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### DefaultSearchProviderName
  #### 預設搜尋提供者名稱
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  指定預設搜尋提供者的名稱。

如果啟用此原則，則可以設定預設搜尋提供者的名稱。

如果未啟用此原則或將其保留空白，則使用搜尋 URL 指定的主機名稱。

'DefaultSearchProviderName' 應設定為組織批准的加密搜尋提供者，該提供者需對應至 DTBC 0008 中設定的加密搜尋提供者。僅在啟用 [DefaultSearchProviderEnabled](#defaultsearchproviderenabled) 和 [DefaultSearchProviderSearchURL](#defaultsearchprovidersearchurl) 原則時，才能套用此原則。


  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  字串

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: DefaultSearchProviderName
  - GP 名稱: 預設搜尋提供者名稱
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/預設搜尋提供者
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: DefaultSearchProviderName
  - 數值類型: REG_SZ
  ##### 範例值:
```
"My Intranet Search"
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: DefaultSearchProviderName
  - 範例值:
``` xml
<string>My Intranet Search</string>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### DefaultSearchProviderSearchURL
  #### 預設搜尋提供者搜尋 URL
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  指定用於預設搜尋的搜索引擎 URL。該 URL 包含字串 '{searchTerms}'，在查詢時由使用者的搜尋字詞替換。

指定 Bing 的搜尋 URL 為:

[{bing:baseURL}search?q={searchTerms}]。

指定 Google 的搜尋網址為: [{google:baseURL}search?q={searchTerms}&{google:RLZ}{google:originalQueryForSuggestion}{google:assistedQueryStats}{google:searchFieldtrialParameter}{google:searchClient}{google:sourceId}ie={inputEncoding}]。

當您啟用 [DefaultSearchProviderEnabled](#defaultsearchproviderenabled) 原則時，需有此原則; 如果您未啟用原則，則此原則將忽略。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  字串

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: DefaultSearchProviderSearchURL
  - GP 名稱: 預設搜尋提供者搜尋 URL
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/預設搜尋提供者
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: DefaultSearchProviderSearchURL
  - 數值類型: REG_SZ
  ##### 範例值:
```
"https://search.contoso.com/search?q={searchTerms}"
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: DefaultSearchProviderSearchURL
  - 範例值:
``` xml
<string>https://search.contoso.com/search?q={searchTerms}</string>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### DefaultSearchProviderSuggestURL
  #### 預設建議的搜尋提供者 URL
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  指定用於提供搜尋建議的搜索引擎的 URL。該 URL 包含字串 '{searchTerms}'，在查詢時由使用者輸入的文字替換。

此原則是選擇性的。如果未設定此原則，則使用者將看不見搜尋建議;他們會看到自己瀏覽歷程記錄和 [我的最愛] 中的建議。

Bing 的建議 URL 可以指定為:

'{bing:baseURL}qbox?query={searchTerms}'。

Google 的建議 URL 可以指定為: '{google:baseURL}complete/search?output=chrome&q={searchTerms}'。

僅在啟用 [DefaultSearchProviderEnabled](#defaultsearchproviderenabled) 和 [DefaultSearchProviderSearchURL](#defaultsearchprovidersearchurl) 原則時，才能套用此原則。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  字串

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: DefaultSearchProviderSuggestURL
  - GP 名稱: 預設建議的搜尋提供者 URL
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/預設搜尋提供者
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: DefaultSearchProviderSuggestURL
  - 數值類型: REG_SZ
  ##### 範例值:
```
"https://search.contoso.com/suggest?q={searchTerms}"
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: DefaultSearchProviderSuggestURL
  - 範例值:
``` xml
<string>https://search.contoso.com/suggest?q={searchTerms}</string>
```
  

  [回到頂端](#microsoft-edge---原則)

  ## Additional policies

  [回到頂端](#microsoft-edge---原則)

  ### AdsSettingForIntrusiveAdsSites
  #### 含有干擾廣告網站的廣告設定
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (78 版或更新版本)

  #### 描述
  控制干擾廣告與站台上是否會封鎖廣告。您可以設定這個原則為下列其中一個選項:

* 1 = 允許在所有網站的廣告。

* 2 = 網站上的區塊廣告與干擾廣告 (預設值)。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  整數

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: AdsSettingForIntrusiveAdsSites
  - GP 名稱: 含有干擾廣告網站的廣告設定
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: AdsSettingForIntrusiveAdsSites
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000001
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: AdsSettingForIntrusiveAdsSites
  - 範例值:
``` xml
<integer>1</integer>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### AllowDeletingBrowserHistory
  #### 啟用刪除瀏覽器和下載歷程記錄
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  啟用刪除瀏覽器歷程記錄並下載歷程記錄，並防止使用者變更此設定。

請注意，即使此原則已停用，瀏覽與下載歷程記錄並不保證保留: 使用者可以編輯或直接刪除歷程記錄資料庫檔案，而且瀏覽器本身可能會隨時移除 (根據到期時間) 或保存任何或所有歷程記錄。

如果您啟用此原則或未設定，則使用者可以刪除瀏覽和下載歷程記錄。

如果您停用此原則，則使用者無法刪除瀏覽和下載歷程記錄。

如果您啟用此原則，請不要啟用 [當 Microsoft Edge 關閉時清除瀏覽資料] 原則，因為它們都將刪除資料。如果您同時啟用兩者，無論此原則如何設定，[當 Microsoft Edge 關閉時清除瀏覽資料的] 原則優先順序較高，並於 Microsoft Edge 關閉時刪除所有資料。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  布林值

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: AllowDeletingBrowserHistory
  - GP 名稱: 啟用刪除瀏覽器和下載歷程記錄
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: AllowDeletingBrowserHistory
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000001
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: AllowDeletingBrowserHistory
  - 範例值:
``` xml
<true/>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### AllowFileSelectionDialogs
  #### 允許檔案選取項目對話方塊
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  讓 Microsoft Edge 顯示檔案選取項目對話方塊，允許存取本機檔案。

如果您啟用或未設定此原則，使用者可以像平常一樣開啟檔案選取項目對話方塊。

如果您停用此原則，當使用者執行會觸發檔案選取項目對話方塊的動作時 (例如匯入我的最愛、上傳檔案或儲存連結)，將會顯示訊息，且使用者會假設為已在檔案選取項目上按下 [取消]。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  布林值

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: AllowFileSelectionDialogs
  - GP 名稱: 允許檔案選取項目對話方塊
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: AllowFileSelectionDialogs
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000001
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: AllowFileSelectionDialogs
  - 範例值:
``` xml
<true/>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### AllowPopupsDuringPageUnload
  #### 允許在網頁卸載時顯示快顯視窗
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (78 版或更新版本)

  #### 描述
  此原則可讓系統管理員指定於卸載期間，能顯示的快顯頁面。

當此原則設定為啟用時，允許頁面在卸載時以快顯視窗顯示。

停用或未設定此原則，則不允許頁面在卸載時以快顯視窗顯示。這是根據規定： (https://html.spec.whatwg.org/#apis-for-creating-and-navigating-browsing-contexts-by-name)。

此原則將會在未來移除。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 否 - 需要重新啟動瀏覽器

  #### 資料類型:
  布林值

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: AllowPopupsDuringPageUnload
  - GP 名稱: 允許在網頁卸載時顯示快顯視窗
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: AllowPopupsDuringPageUnload
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000000
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: AllowPopupsDuringPageUnload
  - 範例值:
``` xml
<false/>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### AllowSyncXHRInPageDismissal
  #### 允許頁面在頁面關閉期間發送同步 XHR 請求
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (79 版或更新版本)

  #### 描述
  透過此原則，您可以指定在頁面關閉期間能發送同步 XHR 請求的頁面。

如果您啟用此原則，頁面可以在頁面關閉期間發送同步 XHR 請求。

若停用或未設定此原則，則不允許頁面在頁面關閉期間發送同步 XHR 請求。

此為臨時原則，並將在未來版本中移除。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 否 - 需要重新啟動瀏覽器

  #### 資料類型:
  布林值

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: AllowSyncXHRInPageDismissal
  - GP 名稱: 允許頁面在頁面關閉期間發送同步 XHR 請求
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: AllowSyncXHRInPageDismissal
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000000
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: AllowSyncXHRInPageDismissal
  - 範例值:
``` xml
<false/>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### AllowTrackingForUrls
  #### 設定特定網站的追蹤防止例外狀況
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (78 版或更新版本)

  #### 描述
  設定從追蹤防止排除的 URL 模式清單。

如果您設定此原則，則已設定為 URL 模式的清單會從追蹤防止中排除。

如果您未設定此原則，「封鎖使用者的網頁瀏覽活動的追蹤」原則 (如果設定) 的通用預設值 或使用者的個人設定將適用於所有網站。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  字串的清單

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: AllowTrackingForUrls
  - GP 名稱: 設定特定網站的追蹤防止例外狀況
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge\AllowTrackingForUrls
  - 路徑 (推薦項目): N/A
  - 值名稱: 1, 2, 3, ...
  - 數值類型: REG_SZ 的清單
  ##### 範例值:
```
SOFTWARE\Policies\Microsoft\Edge\AllowTrackingForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\AllowTrackingForUrls\1 = "[*.]contoso.edu"

```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: AllowTrackingForUrls
  - 範例值:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### AlwaysOpenPdfExternally
  #### 一律開啟外部 PDF 檔案
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  停用 Microsoft Edge 中的內部 PDF 檢視器。

如果啟用此原則，則 Microsoft Edge 會下載 PDF檔案，並允許使用者使用預設應用程式開啟。

如果未設定或停用此原則，則 Microsoft Edge 將開啟 PDF 檔案 (除非使用者停用)。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  布林值

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: AlwaysOpenPdfExternally
  - GP 名稱: 一律開啟外部 PDF 檔案
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: AlwaysOpenPdfExternally
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000001
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: AlwaysOpenPdfExternally
  - 範例值:
``` xml
<true/>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### ApplicationLocaleValue
  #### 設定應用程式地區設定
  >支援的版本: Windows 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  設定 Microsoft Edge 中的應用程式地區設定，並防止使用者變更地區設定。

如果您啟用此原則，Microsoft Edge 會使用指定的地區設定。如果設定地區設定不支援，請改為使用 [EN-US]。

如果您停用或未設置此設定，Microsoft Edge 會使用指定的使用者慣用地區設定 (若已設定) 或後援的地區設定 [EN-US]。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 是
  - 動態原則重新整理: 否 - 需要重新啟動瀏覽器

  #### 資料類型:
  字串

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: ApplicationLocaleValue
  - GP 名稱: 設定應用程式地區設定
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): 系統管理範本/Microsoft Edge - 預設設定 (使用者可以覆寫)/
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): SOFTWARE\Policies\Microsoft\Edge\推薦項目
  - 值名稱: ApplicationLocaleValue
  - 數值類型: REG_SZ
  ##### 範例值:
```
"en"
```


  

  [回到頂端](#microsoft-edge---原則)

  ### AudioCaptureAllowed
  #### 允許或封鎖音訊擷取
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  可讓您設定是否提示使用者授與網站存取其音訊擷取裝置的權限。除 [AudioCaptureAllowedUrls](#audiocaptureallowedurls) 清單中設定的 URL，此原則適用於所有 URL。

如果啟用或未設定此原則 (預設設定)，則除了 [AudioCaptureAllowedUrls](#audiocaptureallowedurls) 清單中的 URL，都會向使用者提示音訊擷取存取。清單中的 URL 會在沒有提示的情況下授與存取權限。

如果停用此原則，則不會提示使用者，且僅能對 [AudioCaptureAllowedUrls](#audiocaptureallowedurls) 中設定的 URL 音訊擷取進行存取。

此原則會影響所有類型的音訊輸入，而不僅是內建麥克風。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  布林值

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: AudioCaptureAllowed
  - GP 名稱: 允許或封鎖音訊擷取
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: AudioCaptureAllowed
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000000
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: AudioCaptureAllowed
  - 範例值:
``` xml
<false/>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### AudioCaptureAllowedUrls
  #### 無需請求權限即可存取音訊擷取裝置的網站
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  根據 URL 模式指定可使用音訊擷取裝置，且無需向使用者要求權限的網站。此清單中的模式與要求 URL 的安全性來源相符。如果相符，則會自動授與網站存取音訊擷取裝置的權限。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  字串的清單

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: AudioCaptureAllowedUrls
  - GP 名稱: 無需請求權限即可存取音訊擷取裝置的網站
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge\AudioCaptureAllowedUrls
  - 路徑 (推薦項目): N/A
  - 值名稱: 1, 2, 3, ...
  - 數值類型: REG_SZ 的清單
  ##### 範例值:
```
SOFTWARE\Policies\Microsoft\Edge\AudioCaptureAllowedUrls\0 = "https://www.contoso.com/"
SOFTWARE\Policies\Microsoft\Edge\AudioCaptureAllowedUrls\1 = "https://[*.]contoso.edu/"

```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: AudioCaptureAllowedUrls
  - 範例值:
``` xml
<array>
  <string>https://www.contoso.com/</string>
  <string>https://[*.]contoso.edu/</string>
</array>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### AutoImportAtFirstRun
  #### 在首次執行時，自動匯入其他瀏覽器的資料和設定
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  如果您啟用此原則，Microsoft Edge 會從預設瀏覽器或另一個指定的瀏覽器自動匯入所有支援資料型別與設定。這也會強制執行 Microsoft Edge 略過匯入區段的初次執行體驗。

如果您設定此原則為 [DisabledAutoImport] (4)，則初次執行體驗的匯入區段會完全略過，且 Microsoft Edge 的瀏覽器資料和設定將不會自動匯入。

* 0 = 從預設瀏覽器自動匯入所有支援的資料類型和設定

* 1 = 從 Internet Explorer 自動匯入所有支援的資料類型與設定

* 2 = 自動匯入所有支援的資料類型和 Google Chrome 設定

* 3= 自動從 Safari 匯入所有支援資料類型與設定

* 4 = 停用自動匯入，並已略過初次執行體驗的匯入區段

**注意**: 此原則目前支援從 Internet Explorer (Windows 7、8、10 和 macOS 上)、Google Chrome (Windows 7、8、10 和 macOS 上) 和 Apple Safari (macOS 上) 瀏覽器匯入。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 否 - 需要重新啟動瀏覽器

  #### 資料類型:
  整數

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: AutoImportAtFirstRun
  - GP 名稱: 在首次執行時，自動匯入其他瀏覽器的資料和設定
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: AutoImportAtFirstRun
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000002
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: AutoImportAtFirstRun
  - 範例值:
``` xml
<integer>2</integer>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### AutofillAddressEnabled
  #### 啟用 [自動填滿] 位址
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  啟用 [自動填寫] 功能，並在網頁表單使用先前儲存的資訊，讓使用者自動完成地址資訊。

如果您停用此原則，[自動填寫] 永遠不會向您建議或填入地址詳細資訊，也不會儲存使用者可能會在瀏覽網站時送出的其他地址資訊。

如果您啟用此原則或未設定，使用者可在使用者介面控制  [自動填寫]。

請注意，如果您停用此原則，也將停止所有網頁表單活動，除了付款與密碼表單之外。不會進一步儲存項目，且 Microsoft Edge 將無法建議或 [自動填寫] 任何先前的項目。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 是
  - 動態原則重新整理: 是

  #### 資料類型:
  布林值

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: AutofillAddressEnabled
  - GP 名稱: 啟用 [自動填滿] 位址
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): 系統管理範本/Microsoft Edge - 預設設定 (使用者可以覆寫)/
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): SOFTWARE\Policies\Microsoft\Edge\推薦項目
  - 值名稱: AutofillAddressEnabled
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000000
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: AutofillAddressEnabled
  - 範例值:
``` xml
<false/>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### AutofillCreditCardEnabled
  #### 啟用信用卡「自動填滿」功能
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  啟用 Microsoft Edge 的 [自動填寫] 功能，並讓使用者 使用先前儲存的網頁表格資訊，自動完成信用卡資訊。

如果您停用此原則，則不會建議 [自動填寫] 或填滿信用卡資訊，也不會儲存使用者可能在瀏覽網站時送出的其他信用卡資訊。

如果您啟用此原則或未設定，使用者可控制信用卡的 [自動填寫] 功能。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 是
  - 動態原則重新整理: 是

  #### 資料類型:
  布林值

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: AutofillCreditCardEnabled
  - GP 名稱: 啟用信用卡「自動填滿」功能
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): 系統管理範本/Microsoft Edge - 預設設定 (使用者可以覆寫)/
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): SOFTWARE\Policies\Microsoft\Edge\推薦項目
  - 值名稱: AutofillCreditCardEnabled
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000000
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: AutofillCreditCardEnabled
  - 範例值:
``` xml
<false/>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### AutoplayAllowed
  #### 允許網站自動播放媒體
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (78 版或更新版本)

  #### 描述
  此原則設定網站的媒體自動播放原則。

預設設定為「未設定」將尊重目前的媒體自動播放設定，並允許使用者設定其自動播放設定。

設定為「已啟用」會將媒體自動播放設定為「允許」。允許所有網站自動播放媒體。使用者無法覆寫此原則。

設定為「已停用」會將媒體自動播放設定為「封鎖」。不允許任何網站自動播放媒體。使用者無法覆寫此原則。

必須關閉並重新開啟索引標籤才能使此原則生效。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  布林值

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: AutoplayAllowed
  - GP 名稱: 允許網站自動播放媒體
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: AutoplayAllowed
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000001
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: AutoplayAllowed
  - 範例值:
``` xml
<true/>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### BackgroundModeEnabled
  #### 在 Microsoft Edge 關閉後繼續執行背景應用程式
  >支援的版本: Windows 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  允許在最近的瀏覽器視窗關閉後，Microsoft Edge 於 OS 登後入啟動。在此案例中，背景應用程式與目前的瀏覽工作階段持續使用中，包括所有工作階段 cookie。開啟式背景處理程序會以圖示顯示在系統匣中，並可能永遠從該處關閉。

如果您啟用此原則，則背景模式會開啟。

如果您停用此原則，則背景模式將會關閉。

如果您未設定此原則，背景模式從一開始就會關閉，而且使用者可以在 edge://settings/system 中設定行為。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 是
  - 動態原則重新整理: 是

  #### 資料類型:
  布林值

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: BackgroundModeEnabled
  - GP 名稱: 在 Microsoft Edge 關閉後繼續執行背景應用程式
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): 系統管理範本/Microsoft Edge - 預設設定 (使用者可以覆寫)/
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): SOFTWARE\Policies\Microsoft\Edge\推薦項目
  - 值名稱: BackgroundModeEnabled
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000001
```


  

  [回到頂端](#microsoft-edge---原則)

  ### BackgroundTemplateListUpdatesEnabled
  #### 對 [集合] 可用的範本清單和其他使用範本的功能啟用背景更新。
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (79 版或更新版本)

  #### 描述
  可讓您對 [集合] 可用範本清單，和使用範本的其他功能啟用或停用背景更新。將頁面儲存到集合時，範本可從網頁中擷取豐富的中繼資料。

如果啟用或未設定此設定，則每 24 小時就會從 Microsoft 服務的背景中下載可用的範本清單。

如果停用此設定，則會根據需要下載可用的範本清單。這種類型的下載可能會些微降低 [集合] 和其他功能的效能。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  布林值

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: BackgroundTemplateListUpdatesEnabled
  - GP 名稱: 對 [集合] 可用的範本清單和其他使用範本的功能啟用背景更新。
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: BackgroundTemplateListUpdatesEnabled
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000001
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: BackgroundTemplateListUpdatesEnabled
  - 範例值:
``` xml
<true/>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### BlockThirdPartyCookies
  #### 封鎖第三方 Cookie
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  禁止非來自網址列中網域的網頁項目設定 Cookie。

如果您啟用此原則，非來自網址列中網域的網頁項目無法設定 Cookie

如果您停用此原則，來自網址列外網域的網頁項目可以設定 Cookie。

如果您未設定此原則，即便第三方 Cookie 已啟用，但使用者仍可以變更此設定。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 是
  - 動態原則重新整理: 是

  #### 資料類型:
  布林值

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: BlockThirdPartyCookies
  - GP 名稱: 封鎖第三方 Cookie
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): 系統管理範本/Microsoft Edge - 預設設定 (使用者可以覆寫)/
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): SOFTWARE\Policies\Microsoft\Edge\推薦項目
  - 值名稱: BlockThirdPartyCookies
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000000
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: BlockThirdPartyCookies
  - 範例值:
``` xml
<false/>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### BrowserAddProfileEnabled
  #### 啟用從 [身分識別] 飛出視窗功能表或 [設定] 頁面建立設定檔
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  可讓使用者建立新設定檔，使用 **新增設定檔** 選項。
如果您啟用此原則或未設定，Microsoft Edge 可讓使用者使用 **新增設定檔** 辨識飛出視窗功能表或 [設定] 頁面，建立新的設定檔。

如果您停用此原則，則使用者無法從識別飛出視窗功能表或 [設定] 頁面新增新的設定檔。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  布林值

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: BrowserAddProfileEnabled
  - GP 名稱: 啟用從 [身分識別] 飛出視窗功能表或 [設定] 頁面建立設定檔
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: BrowserAddProfileEnabled
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000001
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: BrowserAddProfileEnabled
  - 範例值:
``` xml
<true/>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### BrowserGuestModeEnabled
  #### 啟用來賓模式
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  啟用在 Microsoft Edge 中讓使用訪客設定檔的選項。在訪客設定檔中，瀏覽器不會從現有的設定檔匯入瀏覽資料，並當所有訪客設定檔關閉時刪除所有瀏覽資料。

如果您啟用此原則或未設定，Microsoft Edge 可讓使用者在訪客設定檔中瀏覽。

如果您停用此原則，Microsoft Edge 不會在訪客設定檔中讓使用者瀏覽。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  布林值

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: BrowserGuestModeEnabled
  - GP 名稱: 啟用來賓模式
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: BrowserGuestModeEnabled
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000001
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: BrowserGuestModeEnabled
  - 範例值:
``` xml
<true/>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### BrowserNetworkTimeQueriesEnabled
  #### 允許查詢瀏覽器網路時間服務
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  防止 Microsoft Edge 發生有時無法將查詢傳送至瀏覽器網路時間服務以擷取精確時間戳記的情況。

如果您停用此原則，則 Microsoft Edge 將會停止將查詢內容傳送至瀏覽器網路時間服務。

如果您啟用此原則或未設定，Microsoft Edge 有時會傳送查詢內容至瀏覽器網路時間服務。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  布林值

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: BrowserNetworkTimeQueriesEnabled
  - GP 名稱: 允許查詢瀏覽器網路時間服務
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: BrowserNetworkTimeQueriesEnabled
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000001
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: BrowserNetworkTimeQueriesEnabled
  - 範例值:
``` xml
<true/>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### BrowserSignin
  #### 瀏覽器登入設定
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  指定使用者是否可以透過他們的帳戶登入 Microsoft Edge，並使用帳戶相關的服務，如同步處理和單一登入。若要控制同步處理的可用性，請改用 [SyncDisabled](#syncdisabled) 原則。

如果您已設定此原則為 [停用瀏覽器登入]，請確保同時停用 [NonRemovableProfileEnabled](#nonremovableprofileenabled) 原則，因為 [NonRemovableProfileEnabled](#nonremovableprofileenabled) 會禁止建立自動登入瀏覽器設定檔。如果同時設定了這兩個原則，則 Microsoft Edge 將使用 [停用瀏覽器登入] 原則，並表現出 [NonRemovableProfileEnabled](#nonremovableprofileenabled) 設為停用的狀態。如果將此原則設為 [啟用瀏覽器登入] (1)，則使用者可以登入瀏覽器。登入瀏覽器並不表示同步處理會根據預設值開啟; 使用者必須分別選擇加入以使用此功能。

如果將此原則設為 [強制瀏覽器登入] (2)，則使用者必須登入設定檔以使用瀏覽器。根據預設，這將允許使用者選擇是否要同步至他們的帳戶，除非網域系統管理員或已透過 [SyncDisabled](#syncdisabled) 原則停用同步處理。[BrowserGuestModeEnabled](#browserguestmodeenabled) 原則的預設值設定為 False。

如果未設定此原則，使用者可以決定是否要啟用瀏覽器登入選項，並於適當時使用。

* 0 = 停用瀏覽器登入



* 1 = 啟用瀏覽器登入

* 2 = 強制使用者登入以使用瀏覽器

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 否 - 需要重新啟動瀏覽器

  #### 資料類型:
  整數

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: BrowserSignin
  - GP 名稱: 瀏覽器登入設定
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: BrowserSignin
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000002
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: BrowserSignin
  - 範例值:
``` xml
<integer>2</integer>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### BuiltInDnsClientEnabled
  #### 使用內建 DNS 用戶端
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  Controls whether to use the built-in DNS client.

This does not affect which DNS servers are used; just the software stack which is used to communicate with them. For example if the operating system is configured to use an enterprise DNS server, that same server would be used by the built-in DNS client. It is however possible that the built-in DNS client will address servers in different ways by using more modern DNS-related protocols such as DNS-over-TLS.

If you enable this policy, the built-in DNS client is used, if it's available.

If you disable this policy, the client is never used.

If you don't configure this policy, the built-in DNS client is enabled by default on MacOS, and users can change whether to use the built-in DNS client by editing edge://flags or by specifying a command-line flag.

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  布林值

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: BuiltInDnsClientEnabled
  - GP 名稱: 使用內建 DNS 用戶端
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: BuiltInDnsClientEnabled
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000001
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: BuiltInDnsClientEnabled
  - 範例值:
``` xml
<true/>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### CertificateTransparencyEnforcementDisabledForCas
  #### 停用 subjectPublicKeyInfo 雜湊清單的憑證透明度強化
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  停用強制執行 subjectPublicKeyInfo 雜湊清單的 [憑證透明度] 要求。

此原則可讓您停用 [憑證透明度] 揭露對具有包含指定 subjectPublicKeyInfo 雜湊之一憑證的憑證鏈結要求。這會允許那些因未公開揭露而仍未用於 [企業] 主機而不受信任的憑證。

設定此原則時，若要停用 [憑證透明度] 強化，必須符合下列條件集合中的其中一個：
1. 雜湊屬於伺服器憑證的 subjectPublicKeyInfo。
2. 雜湊屬於憑證鏈結內 CA 憑證中出現的 subjectPublicKeyInfo，該CA 憑證會受到 X.509v3 nameConstraints 擴充功能限制，一或多個 directoryName nameConstraints 都存在於 permittedSubtrees 中，且 subjectPublicKeyInfo 和directoryName 均包含 organizationName 屬性。
3. 雜湊屬於憑證鏈結內 CA 憑證中出現的 subjectPublicKeyInfo，該 CA 憑證在憑證 [主體] 中有一或多個 organizationName 屬性，且伺服器的憑證包含相同數目的 organizationName 屬性，順序與位元組的值均相同。

您可以透過串連雜湊演算法名稱、「/」字元，與適用於指定憑證的 DER 編碼的 subjectPublicKeyInfo 雜湊演算法的 Base64 編碼指定 subjectPublicKeyInfo 雜湊。此 Base64 編碼與 [SPKI 指紋] 格式相同，定義與區段 2.4、RFC 7469 中相同。無法辨識的雜湊演算法會略過。目前唯一支援的雜湊演算法是「sha256」。

如果您停用此原則或未設定，且憑證未依照 [憑證透明度] 原則揭露，則任何要求由 [憑證透明度] 揭露的憑證會被視為不受信任。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  字串的清單

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: CertificateTransparencyEnforcementDisabledForCas
  - GP 名稱: 停用 subjectPublicKeyInfo 雜湊清單的憑證透明度強化
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge\CertificateTransparencyEnforcementDisabledForCas
  - 路徑 (推薦項目): N/A
  - 值名稱: 1, 2, 3, ...
  - 數值類型: REG_SZ 的清單
  ##### 範例值:
```
SOFTWARE\Policies\Microsoft\Edge\CertificateTransparencyEnforcementDisabledForCas\0 = "sha256/AAAAAAAAAAAAAAAAAAAAAA=="
SOFTWARE\Policies\Microsoft\Edge\CertificateTransparencyEnforcementDisabledForCas\1 = "sha256//////////////////////w=="

```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: CertificateTransparencyEnforcementDisabledForCas
  - 範例值:
``` xml
<array>
  <string>sha256/AAAAAAAAAAAAAAAAAAAAAA==</string>
  <string>sha256//////////////////////w==</string>
</array>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### CertificateTransparencyEnforcementDisabledForLegacyCas
  #### 停用舊版憑證授權單位清單的 [憑證透明度] 強化
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  停用強制執行舊版的憑證授權單位 (Cas) 的憑證透明度要求清單。

此原則可讓您停用包含具有指定 subjectPublicKeyInfo 雜湊的其中一個憑證的憑證鏈結的憑證透明度揭露需求。除非是不受信任的憑證，否則這會允許憑證，因為這些憑證是不正確公開揭露，且持續由企業主機使用。

為了讓 [憑證透明度強制執行] 停用，您必須設定 subjectPublicKeyInfo 出現在舊版的憑證授權單位 (CA) 可辨識 CA 憑證雜湊。傳統 CA 是由 Microsoft Edge 支援，是預設受到公開信任的一個或多個作業系統。

您可以指定 subjectPublicKeyInfo 雜湊串連雜湊演算法名稱、"/" 字元，以及套用至指定憑證 DER 編碼 subjectPublicKeyInfo 該雜湊演算法的 Base64 編碼。定義於 RFC 7469，區段 2.4 g h Base64 編碼方式是 SPKI 指紋，與相同的格式。無法辨識的雜湊演算法會略過。唯一支援的雜湊演算法此時是 "sha256"。

如果您未設定這個原則，已透過憑證透明度會透露所需的任何憑證將會被視為未受信任的未公開根據憑證透明度原則。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  字串的清單

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: CertificateTransparencyEnforcementDisabledForLegacyCas
  - GP 名稱: 停用舊版憑證授權單位清單的 [憑證透明度] 強化
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge\CertificateTransparencyEnforcementDisabledForLegacyCas
  - 路徑 (推薦項目): N/A
  - 值名稱: 1, 2, 3, ...
  - 數值類型: REG_SZ 的清單
  ##### 範例值:
```
SOFTWARE\Policies\Microsoft\Edge\CertificateTransparencyEnforcementDisabledForLegacyCas\0 = "sha256/AAAAAAAAAAAAAAAAAAAAAA=="
SOFTWARE\Policies\Microsoft\Edge\CertificateTransparencyEnforcementDisabledForLegacyCas\1 = "sha256//////////////////////w=="

```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: CertificateTransparencyEnforcementDisabledForLegacyCas
  - 範例值:
``` xml
<array>
  <string>sha256/AAAAAAAAAAAAAAAAAAAAAA==</string>
  <string>sha256//////////////////////w==</string>
</array>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### CertificateTransparencyEnforcementDisabledForUrls
  #### 停用針對特定 URL 的憑證透明度強化
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  停用強制執行憑證透明度需求列出的 url。

這個原則可讓您會進行中透過憑證透明度的指定 Url 的主機名稱的憑證。這可讓您使用的憑證，否則會是不受信任，因為它們未正確公開外洩，但它會使其他人更難來偵測這些主機卡簽發的憑證。

形成 [https://go.microsoft.com/fwlink/?linkid=2095322](https://go.microsoft.com/fwlink/?linkid=2095322) 根據您 URL 模式。因為指定的主機名稱的有效憑證，獨立於配置、 連接埠或路徑，只有 URL 的主機名稱部分被認為是。不支援萬用字元主機。

如果您未設定這個原則，應該會透露透過憑證透明度的任何憑證會被視為未受信任的如果未公開。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  字串的清單

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: CertificateTransparencyEnforcementDisabledForUrls
  - GP 名稱: 停用針對特定 URL 的憑證透明度強化
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge\CertificateTransparencyEnforcementDisabledForUrls
  - 路徑 (推薦項目): N/A
  - 值名稱: 1, 2, 3, ...
  - 數值類型: REG_SZ 的清單
  ##### 範例值:
```
SOFTWARE\Policies\Microsoft\Edge\CertificateTransparencyEnforcementDisabledForUrls\0 = "contoso.com"
SOFTWARE\Policies\Microsoft\Edge\CertificateTransparencyEnforcementDisabledForUrls\1 = ".contoso.com"

```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: CertificateTransparencyEnforcementDisabledForUrls
  - 範例值:
``` xml
<array>
  <string>contoso.com</string>
  <string>.contoso.com</string>
</array>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### ClearBrowsingDataOnExit
  #### 當 Microsoft Edge 關閉時清除瀏覽資料
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (78 版或更新版本)

  #### 描述
  依照預設，Microsoft Edge 關閉時不會清除瀏覽資料。瀏覽資料包含表格、密碼，甚至也包含曾瀏覽過的網站。

如果您啟用此原則，所有瀏覽資料會在每次 Microsoft Edge 關閉時刪除。

如果您停用或未設定此原則，使用者可以在 [設定] 中設定 [清除瀏覽資料] 選項。

如果您啟用此原則時，請不要啟用 [AllowDeletingBrowserHistory](#allowdeletingbrowserhistory) 原則，因為兩者均會刪除資料。如果您啟用兩者，此原則優先順序較高，而且不論您如何設定 [AllowDeletingBrowserHistory](#allowdeletingbrowserhistory)，當 Microsoft Edge 關閉時會刪除所有資料。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 是
  - 動態原則重新整理: 否 - 需要重新啟動瀏覽器

  #### 資料類型:
  布林值

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: ClearBrowsingDataOnExit
  - GP 名稱: 當 Microsoft Edge 關閉時清除瀏覽資料
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): 系統管理範本/Microsoft Edge - 預設設定 (使用者可以覆寫)/
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): SOFTWARE\Policies\Microsoft\Edge\推薦項目
  - 值名稱: ClearBrowsingDataOnExit
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000001
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: ClearBrowsingDataOnExit
  - 範例值:
``` xml
<true/>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### ClickOnceEnabled
  #### 允許使用者透過 ClickOnce 協定打開檔案
  >支援的版本: Windows 上的 Microsoft Edge (78 版或更新版本)

  #### 描述
  允許使用者使用 ClickOnce 通訊協定開啟檔案。ClickOnce 通訊協定可讓網站要求瀏覽器在使用者的電腦或裝置上使用 ClickOnce 檔案處理常式從特定 URL 開啟檔案。

允許使用者使用 ClickOnce 通訊協定開啟檔案。ClickOnce 通訊協定可讓網站要求瀏覽器在使用者的電腦或裝置上使用 ClickOnce 檔案處理常式從特定 URL 開啟檔案。
如果啟用此原則，使用者就能使用 ClickOnce 通訊協定開啟檔案。這個原則會覆寫使用者在 edge://flags/ 頁面中的 ClickOnce 設定。

如果停用此原則，使用者將無法使用 ClickOnce 開啟檔案。但是，檔案會儲存至使用瀏覽器的檔案系統。這個原則會覆寫使用者在 edge://flags/ 頁面中的 ClickOnce 設定。

如果未設定此原則，使用者就無法使用 ClickOnce 通訊協定開啟檔案。使用者可以選擇啟用 ClickOnce 通訊協定與 edge://flags/ 頁面的搭配使用。

停用 ClickOnce 可能會使 ClickOnce 應用程式 (.application 檔案) 無法正確啟動。

如需有關 ClickOnce 的詳細資訊，請參閱 [https://go.microsoft.com/fwlink/?linkid=2103872](https://go.microsoft.com/fwlink/?linkid=2103872) 與 [https://go.microsoft.com/fwlink/?linkid=2099880](https://go.microsoft.com/fwlink/?linkid=2099880)。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  布林值

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: ClickOnceEnabled
  - GP 名稱: 允許使用者透過 ClickOnce 協定打開檔案
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: ClickOnceEnabled
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000000
```


  

  [回到頂端](#microsoft-edge---原則)

  ### CommandLineFlagSecurityWarningsEnabled
  #### 啟用命令列旗標的安全性警告
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (78 版或更新版本)

  #### 描述
  若停用這個原則可防止安全性警告時，不要顯示 Microsoft Edge 已啟動具有潛在危險的命令列旗標。

 如果啟用或未設定，這些命令列旗標啟動時會顯示安全性警告 Microsoft Edge。

 例如，--disable-gpu-sandbox 旗標會產生此警告: 您正在使用不支援的命令列旗標: --disable-gpu-sandbox。這會造成穩定性與安全性風險。

在 Windows 中，此原則僅能使用已加入至 Microsoft Active Directory 網域的執行個體或已註冊裝置管理的 Windows 10 專業版 (或企業版) 的執行個體。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 否 - 需要重新啟動瀏覽器

  #### 資料類型:
  布林值

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: CommandLineFlagSecurityWarningsEnabled
  - GP 名稱: 啟用命令列旗標的安全性警告
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: CommandLineFlagSecurityWarningsEnabled
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000001
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: CommandLineFlagSecurityWarningsEnabled
  - 範例值:
``` xml
<true/>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### ComponentUpdatesEnabled
  #### 啟用 Microsoft Edge 中的元件更新
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  如果您啟用或未設定此原則，元件更新會在 Microsoft Edge 中啟用。

如果您停用此原則，或將其設定為 false，所有 Microsoft Edge 內的元件更新將會停用。

然而，有些元件已豁免於此原則。這包括未包含可執行程式碼的元件，這不會大幅變更瀏覽器行為或重大安全性。也就是說，即使您停用此原則，仍會套用視為「重大安全性」的更新。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 否 - 需要重新啟動瀏覽器

  #### 資料類型:
  布林值

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: ComponentUpdatesEnabled
  - GP 名稱: 啟用 Microsoft Edge 中的元件更新
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: ComponentUpdatesEnabled
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000001
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: ComponentUpdatesEnabled
  - 範例值:
``` xml
<true/>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### ConfigureDoNotTrack
  #### 設定 [不要追蹤]
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  指定是否要傳送 「 不要追蹤 」 要求到要求追蹤資訊的網站。不要追蹤 」 要求讓您瀏覽的網站，知道您不想要追蹤您瀏覽活動。根據預設， Microsoft Edge 不傳送 [不要追蹤要求]，但使用者可以開啟這項功能將它們傳送。

如果您啟用這個原則，會一律會傳送 Do Not Track 要求到要求追蹤資訊的網站。

如果您停用這個原則，將永遠不會傳送要求。

如果您未設定這個原則，使用者可以選擇是否要傳送這些要求。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  布林值

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: ConfigureDoNotTrack
  - GP 名稱: 設定 [不要追蹤]
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: ConfigureDoNotTrack
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000000
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: ConfigureDoNotTrack
  - 範例值:
``` xml
<false/>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### ConfigureOnlineTextToSpeech
  #### 設定線上文字轉語音
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  TX: 設定瀏覽器是否能利用 Azure 認知服務中的線上文字轉換語音的語音字型。這些語音字型的品質高於預先安裝的系統語音字型。

如果您啟用或未設定此原則，使用 SpeechSynthesis API 的網頁應用程式可以使用線上文字轉換語音的語音字型。

如果您停用此原則，語音字型便無法使用。

深入了解此功能:
SpeechSynthesis API: [https://go.microsoft.com/fwlink/?linkid=2110038](https://go.microsoft.com/fwlink/?linkid=2110038)
認知服務: [https://go.microsoft.com/fwlink/?linkid=2110141](https://go.microsoft.com/fwlink/?linkid=2110141)

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  布林值

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: ConfigureOnlineTextToSpeech
  - GP 名稱: 設定線上文字轉語音
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: ConfigureOnlineTextToSpeech
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000001
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: ConfigureOnlineTextToSpeech
  - 範例值:
``` xml
<true/>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### CustomHelpLink
  #### 指定自訂 [説明] 連結
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (79 版或更新版本)

  #### 描述
  指定 [説明] 功能表或按 F1 鍵的連結。

如果啟用此原則，則系統管理員可以為 [説明] 功能表或 F1 鍵指定連結。

如果停用或未設定此原則，則 [説明] 功能表或 F1 鍵將使用預設連結。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  字串

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: CustomHelpLink
  - GP 名稱: 指定自訂 [説明] 連結
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: CustomHelpLink
  - 數值類型: REG_SZ
  ##### 範例值:
```
"https://go.microsoft.com/fwlink/?linkid=2080734"
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: CustomHelpLink
  - 範例值:
``` xml
<string>https://go.microsoft.com/fwlink/?linkid=2080734</string>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### DefaultBrowserSettingEnabled
  #### 設定 Microsoft Edge 為預設瀏覽器
  >支援的版本: Windows 7 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  設定 Microsoft Edge 中的預設瀏覽器檢查，並防止使用者變更。

如果啟用此原則，則 Microsoft Edge 會在啟動時檢查其是否為預設瀏覽器，並在可能的情況下自動註冊。

如果停用此原則，則 Microsoft Edge 不會檢查和停用使用者控制項來設定此選項。

如果您未設定此原則，則 Microsoft Edge 允許使用者控制其是否為預設瀏覽器，以及在非為預設瀏覽器時，是否顯示使用者通知。

Windows 系統管理員注意事項：此原則僅適用於執行 Windows 7 的電腦。至於較新版本的 Windows，您必須部署一個「預設應用程式關聯」檔案，使 Microsoft Edge 成為 https 和http 通訊協定處理常式 (以及選擇性的ftp通訊協定和檔案格式，如 .html、.htm、.pdf、.svg、.webp)。如需詳細資訊，請參閱[https://go.microsoft.com/fwlink/?linkid=2094932](https://go.microsoft.com/fwlink/?linkid=2094932)。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  布林值

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: DefaultBrowserSettingEnabled
  - GP 名稱: 設定 Microsoft Edge 為預設瀏覽器
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: DefaultBrowserSettingEnabled
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000001
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: DefaultBrowserSettingEnabled
  - 範例值:
``` xml
<true/>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### DeveloperToolsAvailability
  #### 控制可在哪使用開發人員工具
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  控制開發人員工具使用的地方。

如果您設定原則為 [DeveloperToolsDisallowedForForceInstalledExtensions] (0，預設值)，使用者在一般情況下可以存取開發人員工具和 JavaScript 主控台，但不是在由企業原則安裝的擴充功能內容中。

如果您設定原則為 [DeveloperToolsAllowed] (1)，則使用者可以存取所有內容的開發人員工具和 JavaScript 主控台，包括由企業原則安裝的擴充功能。

如果您設定原則為 [DeveloperToolsDisallowed] (2)，使用者無法存取開發人員工具或檢查網站項目。鍵盤快速鍵和開啟開發人員工具或 JavaScript 主控台的功能表或操作功能表項目已停用。

* 0 = 允許其他內容中由企業原則所安裝的擴充功能上的開發人員工具

* 1 = 允許使用開發人員工具

* 2 = 不允許使用開發人員工具

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  整數

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: DeveloperToolsAvailability
  - GP 名稱: 控制可在哪使用開發人員工具
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: DeveloperToolsAvailability
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000002
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: DeveloperToolsAvailability
  - 範例值:
``` xml
<integer>2</integer>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### DirectInvokeEnabled
  #### 允許使用者透過 DirectInvoke 協定打開檔案
  >支援的版本: Windows 上的 Microsoft Edge (78 版或更新版本)

  #### 描述
  允許使用者使用 DirectInvoke 通訊協定開啟檔案。DirectInvoke 通訊協定可讓網站要求瀏覽器在使用者的電腦或裝置上使用 DirectInvoke 檔案處理常式從特定 URL 開啟檔案。

如果啟用或未設定此原則，使用者就能使用 DirectInvoke 通訊協定開啟檔案。

如果停用此原則，使用者將無法使用 DirectInvoke 開啟檔案。但是，檔案會儲存至檔案系統。

注意: 停用 DirectInvoke 可能會使部分 Microsoft Office SharePoint Online 功能無法正常運作。

如需有關 DirectInvoke 的詳細資訊，請參閱 [https://go.microsoft.com/fwlink/?linkid=2103872](https://go.microsoft.com/fwlink/?linkid=2103872) 和 [https://go.microsoft.com/fwlink/?linkid=2099871](https://go.microsoft.com/fwlink/?linkid=2099871)。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  布林值

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: DirectInvokeEnabled
  - GP 名稱: 允許使用者透過 DirectInvoke 協定打開檔案
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: DirectInvokeEnabled
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000000
```


  

  [回到頂端](#microsoft-edge---原則)

  ### Disable3DAPIs
  #### 停用 3D 圖形 Api 支援
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  防止網頁存取圖形處理器單元 (GPU)。具體而言，網頁無法存取 WebGL API，且外掛程式無法使用 Pepper 3D API。

如果您未設定或停用此原則，便可能會允許網頁設定使用 WebGL API 與外掛程式來使用 Pepper 3D API。根據預設，Microsoft Edge 可能會要求使用這些 Api 傳遞的命令列引數。

如果 [HardwareAccelerationModeEnabled](#hardwareaccelerationmodeenabled) 原則設定為 False，則會略過 'Disable3DAPIs' 原則設定 - 等同於 'Disable3DAPIs' 原則設定為 true。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  布林值

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: Disable3DAPIs
  - GP 名稱: 停用 3D 圖形 Api 支援
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: Disable3DAPIs
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000000
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: Disable3DAPIs
  - 範例值:
``` xml
<false/>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### DisableScreenshots
  #### 停用取得螢幕擷取畫面功能
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  控制使用者是否能取得瀏覽器頁面的螢幕擷取畫面。

啟用後，使用者將無法利用鍵盤快速鍵或延伸模組 API 取得螢幕擷取畫面。

如果停用或未設定此原則，使用者將能取得螢幕擷取畫面。

請注意，此原則可以控制自瀏覽器內取得的螢幕擷取畫面。即使您啟用此原則，使用者仍透過瀏覽器外的某些方式取得螢幕擷取畫面 (例如利用作業系統功能或其他應用程式)。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  布林值

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: DisableScreenshots
  - GP 名稱: 停用取得螢幕擷取畫面功能
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: DisableScreenshots
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000001
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: DisableScreenshots
  - 範例值:
``` xml
<true/>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### DiskCacheDir
  #### 設定磁碟快取目錄
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  設定用來存放快取檔案的目錄。

如果您啟用此原則，無論使用者是否已指定 [--disk-cache-dir] 旗標，Microsoft Edge 會使用提供的目錄。若要避免資料遺失或其他未預期錯誤，不要設定此原則至磁碟區根目錄或用於其他用途的目錄，因為 Microsoft Edge 可管理其內容。

請參閱 [https://go.microsoft.com/fwlink/?linkid=2095041](https://go.microsoft.com/fwlink/?linkid=2095041)，查看指定目錄及路徑時，您可以使用的變數清單。

如果您未設定此原則，會使用預設快取目錄，且使用者可以覆寫該預設 [--disk-cache-dir] 命令列旗標。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 否 - 需要重新啟動瀏覽器

  #### 資料類型:
  字串

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: DiskCacheDir
  - GP 名稱: 設定磁碟快取目錄
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: DiskCacheDir
  - 數值類型: REG_SZ
  ##### 範例值:
```
"${user_home}/Edge_cache"
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: DiskCacheDir
  - 範例值:
``` xml
<string>${user_home}/Edge_cache</string>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### DiskCacheSize
  #### 設定磁碟快取大小，以位元組為單位
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  設定快取的大小，以位元組為單位，用來儲存在磁碟上的檔案。

如果您啟用這個原則， Microsoft Edge時，使用提供的快取大小，無論使用者是否已指定 [--disk-cache-size] 旗標。此原則中指定的值不是固定的界限，但快取系統; 而建議下面是一些 mb 的任何值太小，而且會四捨五入至合理的最小值。

如果您設定這個原則的值為 0 時，要使用預設快取大小，和使用者無法變更它。

如果您未設定這個原則，就會使用預設大小，但是使用者可以覆寫它與 '-磁碟快取大小 ' 旗標。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 否 - 需要重新啟動瀏覽器

  #### 資料類型:
  整數

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: DiskCacheSize
  - GP 名稱: 設定磁碟快取大小，以位元組為單位
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: DiskCacheSize
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x06400000
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: DiskCacheSize
  - 範例值:
``` xml
<integer>104857600</integer>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### DownloadDirectory
  #### 設定下載目錄
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  設定下載檔案時使用的目錄。

如果您啟用此原則，無論使用者是否已指定一個，或每次選擇使用提示的下載位置，Microsoft Edge 都會使用提供的目錄。請參閱 [https://go.microsoft.com/fwlink/?linkid=2095041](https://go.microsoft.com/fwlink/?linkid=2095041) 的可用變數清單。

如果您停用或未設定此原則，請使用預設下載目錄，且使用者都可以變更。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 是
  - 動態原則重新整理: 是

  #### 資料類型:
  字串

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: DownloadDirectory
  - GP 名稱: 設定下載目錄
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): 系統管理範本/Microsoft Edge - 預設設定 (使用者可以覆寫)/
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): SOFTWARE\Policies\Microsoft\Edge\推薦項目
  - 值名稱: DownloadDirectory
  - 數值類型: REG_SZ
  ##### 範例值:
```
"/home/${user_name}/Downloads"
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: DownloadDirectory
  - 範例值:
``` xml
<string>/home/${user_name}/Downloads</string>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### DownloadRestrictions
  #### 允許下載限制
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  設定 Microsoft Edge 完全封鎖的下載類型，且不允許使用者覆寫安全性決策。

設定 [封鎖危險下載] (1) 允許所有下載項目，除了那些造成 Microsoft Defender SmartScreen 警告的項目。

設定 [封鎖具有潛在危險的下載項目] (2) 若要允許所有下載項目，除了那些具有潛在危險下載內容的 Microsoft Defender SmartScreen 警告的項目。

設定 [封鎖所有下載項目] (3) 會封鎖所有下載項目。

如果您不設定此原則，或設定為 [沒有特殊限制] (0) 選項，下載項目將移到根據 Microsoft Defender SmartScreen 分析結果的一般安全性限制。

請注意，這些限制會套用至網頁下載內容，以及 [下載連結...] 快顯功能表選項。這些限制不會套用至儲存或下載目前顯示的頁面，也不會套用至從列印選項另存為 PDF 選項。

如需更多 Microsoft Defender SmartScreen 的詳細資訊，請參閱 [https://go.microsoft.com/fwlink/?linkid=2094934](https://go.microsoft.com/fwlink/?linkid=2094934)。

* 0 = 沒有特殊限制

* 1 = 區塊危險下載

* 2 = 封鎖具有潛在危險的下載

* 3 = 封鎖所有下載

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 是
  - 動態原則重新整理: 是

  #### 資料類型:
  整數

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: DownloadRestrictions
  - GP 名稱: 允許下載限制
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): 系統管理範本/Microsoft Edge - 預設設定 (使用者可以覆寫)/
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): SOFTWARE\Policies\Microsoft\Edge\推薦項目
  - 值名稱: DownloadRestrictions
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000002
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: DownloadRestrictions
  - 範例值:
``` xml
<integer>2</integer>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### EdgeCollectionsEnabled
  #### 啟用 [集錦] 功能
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (78 版或更新版本)

  #### 描述
  可讓您允許使用者存取 [集錦] 功能，可以收集、組織、共用並且更有效率地匯出內容，並與 Office 整合。

如果您啟用或未設定此原則，使用者將能存取並使用 Microsoft Edge 中的集錦功能。

如果您停用此原則，則使用者無法存取與使用 Microsoft Edge 中的集錦。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 否 - 需要重新啟動瀏覽器

  #### 資料類型:
  布林值

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: EdgeCollectionsEnabled
  - GP 名稱: 啟用 [集錦] 功能
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: EdgeCollectionsEnabled
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000001
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: EdgeCollectionsEnabled
  - 範例值:
``` xml
<true/>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### EditFavoritesEnabled
  #### 允許使用者編輯我的最愛
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  啟用此原則讓使用者新增、移除和修改我的最愛。如果您未設定此原則，則為預設行為。

停用此原則禁止使用者新增、移除或修改我的最愛。他們仍可以使用現有的我的最愛。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  布林值

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: EditFavoritesEnabled
  - GP 名稱: 允許使用者編輯我的最愛
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: EditFavoritesEnabled
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000000
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: EditFavoritesEnabled
  - 範例值:
``` xml
<false/>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### EnableDeprecatedWebPlatformFeatures
  #### 在限定時間內重新啟用已取代的網頁平台功能
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  指定要暫時重新啟用的已取代的 Web 平台功能清單。

此原則允許在有限時間內重新啟用已取代的 Web 平台功能。功能由字串標記識別。

如果不設定此原則、清單為空，或功能與支援的字串標記之一不相符，則所有已取代的 Web 平台功能將維持停用狀態。

雖然上述平台支援該原則，但其啟用的功能可能無法在所有平台上使用。並非所有已取代的 Web 平台功能都能重新啟用。僅有下方明確列出的功能可在有限時間內重新啟用，每項功能的時間皆不同。您可以上 https://bit.ly/blinkintents 查看 Web 平台功能的變更用途。

 字串標記的一般格式為 [DeprecatedFeatureName]_EffectiveUntil[yyyymmdd]。

* "ExampleDeprecatedFeature_EffectiveUntil20080902" =啟用 ExampleDeprecatedFeature API 到 2008/09/02

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  字串的清單

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: EnableDeprecatedWebPlatformFeatures
  - GP 名稱: 在限定時間內重新啟用已取代的網頁平台功能
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge\EnableDeprecatedWebPlatformFeatures
  - 路徑 (推薦項目): N/A
  - 值名稱: 1, 2, 3, ...
  - 數值類型: REG_SZ 的清單
  ##### 範例值:
```
SOFTWARE\Policies\Microsoft\Edge\EnableDeprecatedWebPlatformFeatures\0 = "ExampleDeprecatedFeature_EffectiveUntil20080902"

```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: EnableDeprecatedWebPlatformFeatures
  - 範例值:
``` xml
<array>
  <string>ExampleDeprecatedFeature_EffectiveUntil20080902</string>
</array>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### EnableDomainActionsDownload
  #### 啟用從 Microsoft 進行網域動作下載
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  在 Microsoft Edge 中，[網域動作] 代表一系列的相容性功能，協助您的瀏覽器在網路上正確運作。

Microsoft 會基於相容性原因，保留特定網域中的動作清單。例如，如果網站因 Microsoft Edge 上的新 [使用者代理程式] 造成網站損毀，瀏覽器可能會覆寫網站上的使用者代理程式字串。當 Microsoft 嘗試解決網站擁有者的問題時，每個動作都是暫時性的。

瀏覽器啟動時並經過一定的時間後，將會聯繫 [實驗和設定服務]，其中包含最新的相容性以執行動作清單。此清單在第一次擷取後會儲存在本機，如果伺服器的複本已變更，讓後續的要求只需更新清單。

如果您啟用此原則，將會繼續從 [實驗和設定服務] 下載 [網域動作] 清單。

如果您停用此原則，將不會繼續從 [實驗和設定服務] 下載 [網域動作] 清單。

如果您未設定此原則，將繼續從 [實驗和設定服務] 下載網域動作清單。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  布林值

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: EnableDomainActionsDownload
  - GP 名稱: 啟用從 Microsoft 進行網域動作下載
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: EnableDomainActionsDownload
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000001
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: EnableDomainActionsDownload
  - 範例值:
``` xml
<true/>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### EnableOnlineRevocationChecks
  #### 啟用線上 OCSP/CRL 檢查
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  線上撤銷檢查並不會提供重大的安全性權益，且預設為停用。

如果啟用此原則，Microsoft Edge 將會執行非封鎖性失敗線上 OCSP/CRL 檢查。「非封鎖性」表示如果無法連線至撤銷伺服器，就會將憑證視作有效。

如果停用或未設定原則，Microsoft Edge 就不會執行線上撤銷檢查。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  布林值

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: EnableOnlineRevocationChecks
  - GP 名稱: 啟用線上 OCSP/CRL 檢查
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: EnableOnlineRevocationChecks
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000000
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: EnableOnlineRevocationChecks
  - 範例值:
``` xml
<false/>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### EnterpriseHardwarePlatformAPIEnabled
  #### 允許受管理的擴充程式使用企業硬體平台 API
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (78 版或更新版本)

  #### 描述
  當此原則設定為已啟用時，企業原則安裝的擴充功能允許使用企業硬體平台 API。
當設定為已停用或未設定時，沒有任何擴充功能可使用企業硬體平台 API。
此原則也適用於元件的擴充功能。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  布林值

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: EnterpriseHardwarePlatformAPIEnabled
  - GP 名稱: 允許受管理的擴充程式使用企業硬體平台 API
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: EnterpriseHardwarePlatformAPIEnabled
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000001
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: EnterpriseHardwarePlatformAPIEnabled
  - 範例值:
``` xml
<true/>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### ExperimentationAndConfigurationServiceControl
  #### 透過 [實驗] 和 [設定服務] 控制通訊
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  在 Microsoft Edge 中，測試和設定服務會用來部署測試和設定承載。

測試承載由一組 Microsoft 用於測試和收集意見反應的早期開發功能組成。

設定承載由一組 Microsoft 希望部署至 Microsoft Edge 以將使用者體驗最佳化的設定組成。舉例來說，設定承載可能會指定 Microsoft Edge 傳送要求至實驗和設定服務以擷取最新承載的頻率。

如果將此原則設定為「擷取設定和測試」模式，就會從測試和設定服務下載完整的承載。這同時包括測試和服務承載。

如果將此原則設定為「僅擷取設定」模式，則只會傳遞設定承載。

如果將此原則設定為「停用與測試和設定服務間的通訊」模式，則會完全停止與測試和設定服務間的通訊。

如果未設定此原則，則在穩定和搶鮮版 (Beta) 通道上的受控裝置，行為會等同「僅擷取設定」模式。

如果未設定此原則，則在非受控的裝置上，行為會等同「擷取設定和測試」模式。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  整數

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: ExperimentationAndConfigurationServiceControl
  - GP 名稱: 透過 [實驗] 和 [設定服務] 控制通訊
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: ExperimentationAndConfigurationServiceControl
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000002
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: ExperimentationAndConfigurationServiceControl
  - 範例值:
``` xml
<integer>2</integer>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### ExternalProtocolDialogShowAlwaysOpenCheckbox
  #### 在外部通訊協定對話方塊中顯示「一律開啟」核取方塊。
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (79 版或更新版本)

  #### 描述
  此原則控制是否在外部通訊協定啟動確認提示上顯示「一律開啟」核取方塊。

如果將此原則設為 True，則在顯示外部通訊協定確認提示時，使用者可以選擇「一律開啟」。該使用者以後將不會再收到此通訊協定的確認提示。

如果將此原則設為 False，或者未設定原則，則不會顯示「一律開啟」核取方塊。每次叫用外部通訊協定時，都會提示用戶進行確認。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 否 - 需要重新啟動瀏覽器

  #### 資料類型:
  布林值

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: ExternalProtocolDialogShowAlwaysOpenCheckbox
  - GP 名稱: 在外部通訊協定對話方塊中顯示「一律開啟」核取方塊。
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: ExternalProtocolDialogShowAlwaysOpenCheckbox
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000001
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: ExternalProtocolDialogShowAlwaysOpenCheckbox
  - 範例值:
``` xml
<true/>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### FavoritesBarEnabled
  #### 啟用 [我的最愛] 列
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  啟用或停用 [我的最愛] 列。

如果啟用此原則，使用者將能看到 [我的最愛] 列。

如果停用此原則，使用者將看不到 [我的最愛] 列。

如果未設定此原則，使用者可以決定是否使用 [我的最愛] 列。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 是
  - 動態原則重新整理: 是

  #### 資料類型:
  布林值

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: FavoritesBarEnabled
  - GP 名稱: 啟用 [我的最愛] 列
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): 系統管理範本/Microsoft Edge - 預設設定 (使用者可以覆寫)/
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): SOFTWARE\Policies\Microsoft\Edge\推薦項目
  - 值名稱: FavoritesBarEnabled
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000001
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: FavoritesBarEnabled
  - 範例值:
``` xml
<true/>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### ForceBingSafeSearch
  #### 強制執行 Bing 安全搜尋
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  請確認 Bing Web 搜尋中的查詢已完成，且安全搜尋設定為指定值。使用者無法變更此設定。

如果您設定此原則為「關閉」，Bing 搜尋中的安全搜尋會退回 bing.com 值。

如果您設定此原則為「中」時，則會使用安全搜尋的中等設定。中等設定會過濾成人影片和影像，但不會過濾搜尋結果的文字。

如果您設定此原則為「嚴格」則會使用安全搜尋的嚴格設定。嚴格設定會過濾成人文字、圖像及影片。

如果您停用此原則或未設定，則不會強制執行 Bing 搜尋中的安全搜尋，使用者可以在 bing.com 上設定他們要的值。

* 0 = 不要在 Bing 中設定搜尋限制

* 1 = 以 Bing 中設定中度搜尋限制

* 2 = 在 Bing 中設定嚴格搜尋限制

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  整數

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: ForceBingSafeSearch
  - GP 名稱: 強制執行 Bing 安全搜尋
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: ForceBingSafeSearch
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000000
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: ForceBingSafeSearch
  - 範例值:
``` xml
<integer>0</integer>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### ForceEphemeralProfiles
  #### 啟用使用暫時設定檔
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  控制使用者設定檔是否切換到暫時模式。工作階段開始時建立暫時設定檔，工作階段結束後刪除暫時設定檔，暫時設定檔與使用者原始設定檔相關聯。

如果啟用此原則，設定檔將以暫時模式執行。這能讓使用者在自己的裝置上工作，而無需將瀏覽資料儲存到裝置中。如果將此原則啟用為 OS 原則 (如在 Windows 上使用群組原則物件 (GPO))，則此原則將套用至系統上的所有設定檔。

 如果停用或不設定此原則，則使用者將在登入瀏覽器時，取得其慣常使用的設定檔。

   在暫時模式下，設定檔資料僅在使用者工作階段期間儲存於磁碟上。關閉瀏覽器後，將不會儲存瀏覽器歷程記錄、擴充功能和其資料等功能、Cookie 等網路資料和 Web 資料庫。這不會防止使用者以手動方式將任何資料下載到磁碟中，也不會防止使用者儲存或列印頁面。如果使用者已啟用同步處理，則所有資料都會保留在其同步帳戶中，就像一般設定檔一樣。除非明確停用此原則，否則使用者還可以在暫時模式下使用 InPrivate 瀏覽。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 否 - 需要重新啟動瀏覽器

  #### 資料類型:
  布林值

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: ForceEphemeralProfiles
  - GP 名稱: 啟用使用暫時設定檔
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: ForceEphemeralProfiles
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000001
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: ForceEphemeralProfiles
  - 範例值:
``` xml
<true/>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### ForceGoogleSafeSearch
  #### 強制執行 Google 安全搜尋
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  限制在啟用安全搜尋設定的 [Google 網頁搜尋] 中才能查詢，並防止使用者變更此設定。

如果您啟用此原則，[Google 搜尋] 中的安全搜尋將一律啟用。

如果您停用此原則或未設定，則不會強制執行 [Google 搜尋] 中的安全搜尋。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  布林值

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: ForceGoogleSafeSearch
  - GP 名稱: 強制執行 Google 安全搜尋
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: ForceGoogleSafeSearch
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000000
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: ForceGoogleSafeSearch
  - 範例值:
``` xml
<false/>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### ForceNetworkInProcess
  #### 強制網路程式碼在瀏覽器處理程序中執行
  >支援的版本: Windows 上的 Microsoft Edge (78 版或更新版本)

  #### 描述
  此原則會強制網路程式碼在瀏覽器處理程序中執行。

預設為停用此原則。如果啟用，則網路處理程序沙箱化時，使用者將開啟安全性問題。

  此原則旨在使企業有機會移轉至不依賴於連接網絡 API 的協力廠商。建議透過 LSP 及 Win32 API 填補 Proxy 伺服器。

  如果未設定此原則，網路程式可能會耗盡瀏覽器處理程序，具體取決於 NetworkService 實驗的現場試驗。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 否 - 需要重新啟動瀏覽器

  #### 資料類型:
  布林值

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: ForceNetworkInProcess
  - GP 名稱: 強制網路程式碼在瀏覽器處理程序中執行
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: ForceNetworkInProcess
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000000
```


  

  [回到頂端](#microsoft-edge---原則)

  ### ForceYouTubeRestrict
  #### 強制最小 YouTube 限制模式
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  在 YouTube 上強制執行最小限制模式，並防止使用者選擇限制較少的模式。

設定為 [嚴格](2)，則在 YouTube 上強制執行嚴格限制模式。

設定為 [中等](1)，則強制使用者在 YouTube 上僅使用中等限制模式和嚴格限制模式。使用者無法停用限制模式。

設定為關閉 (0) 或不設定此原則，則不在 YouTube 上強制執行受限模式。外部原則 (如 YouTube 原則) 可能仍然會強制執行限制模式。

* 0 = 不在 YouTube 上強制執行限制模式

* 1 = 在 YouTube 上強制執行至少中等限制模式

* 2 = 在 YouTube 上強制執行嚴格限制模式

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  整數

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: ForceYouTubeRestrict
  - GP 名稱: 強制最小 YouTube 限制模式
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: ForceYouTubeRestrict
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000000
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: ForceYouTubeRestrict
  - 範例值:
``` xml
<integer>0</integer>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### FullscreenAllowed
  #### 允許全螢幕模式
  >支援的版本: Windows 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  設定全螢幕模式的可用性 - 所有 Microsoft Edge 會隱藏 UI，且只會顯示網頁內容。

如果您啟用此原則或未設定，具有適當權限的使用者、應用程式與擴充功能可進入全螢幕模式。

如果您停用此原則，使用者、應用程式與擴充功能皆無法進入全螢幕模式。

當全螢幕模式停用時，使用命令列在 kiosk 模式中開啟 Microsoft Edge 的功能無法使用。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  布林值

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: FullscreenAllowed
  - GP 名稱: 允許全螢幕模式
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: FullscreenAllowed
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000001
```


  

  [回到頂端](#microsoft-edge---原則)

  ### GoToIntranetSiteForSingleWordEntryInAddressBar
  #### 強制直接進行內部網路網站導航，而非在 [網址列] 中搜尋單字項目。
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (78 版或更新版本)

  #### 描述
  如果啟用此原則，如果在網址列中輸入的文字是一個不帶標點符號的單字，則在網址列建議清單中排名最前面的自動建議結果，將巡覽至內部網路網站。

若輸入一個不帶標點符號的單字，則預設瀏覽將會連至與輸入文字相符的內部網路網站。

如果啟用此原則，則網址列建議清單中的第二個自動建議結果，將執行與輸入內容完全相同的 web 搜尋，前提輸入文字須為沒有標點符號的單字。除非還啟用了阻止 web 搜索的原則，否則將使用預設的搜尋提供者。

啟用此原則會有兩個效果：

將不再回應單字查詢 (通常會解析為歷程記錄項目) 巡覽至網站。瀏覽器將改為嘗試巡覽至可能不存在於組織內部網路網站中的網站。這將導致 404 錯誤。

熱門的單字搜尋詞彙將需要手動選擇搜尋建議才能進行正確的搜尋。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  布林值

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: GoToIntranetSiteForSingleWordEntryInAddressBar
  - GP 名稱: 強制直接進行內部網路網站導航，而非在 [網址列] 中搜尋單字項目。
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: GoToIntranetSiteForSingleWordEntryInAddressBar
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000000
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: GoToIntranetSiteForSingleWordEntryInAddressBar
  - 範例值:
``` xml
<false/>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### HSTSPolicyBypassList
  #### 設定會略過 HSTS 原則檢查的名稱清單
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (79 版或更新版本)

  #### 描述
  在此清單中指定的主機名稱不受 HSTS 原則檢查，該檢查可能會將請求從 [HTTP://] 升級到 [HTTPs://]。此原則僅允許使用單標籤主機名稱。主機名稱必須為正式名稱。任何 IDN 都必須轉換為其 A 標籤格式，且所有 ASCII 字母都必須為小寫。該原則僅適用於指定的特定主機名稱; 此原則無法套用到該清單中的子網域名稱。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 否 - 需要重新啟動瀏覽器

  #### 資料類型:
  字串的清單

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: HSTSPolicyBypassList
  - GP 名稱: 設定會略過 HSTS 原則檢查的名稱清單
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge\HSTSPolicyBypassList
  - 路徑 (推薦項目): N/A
  - 值名稱: 1, 2, 3, ...
  - 數值類型: REG_SZ 的清單
  ##### 範例值:
```
SOFTWARE\Policies\Microsoft\Edge\HSTSPolicyBypassList\0 = "meet"

```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: HSTSPolicyBypassList
  - 範例值:
``` xml
<array>
  <string>meet</string>
</array>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### HardwareAccelerationModeEnabled
  #### 可用時便使用硬體加速
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  如果可使用，請指定使用硬體加速。如果啟用或不設定此原則，除非明確封鎖 GPU 功能，否則便會啟用硬體加速。

如果停用此原則，則會停用硬體加速。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 否 - 需要重新啟動瀏覽器

  #### 資料類型:
  布林值

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: HardwareAccelerationModeEnabled
  - GP 名稱: 可用時便使用硬體加速
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: HardwareAccelerationModeEnabled
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000001
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: HardwareAccelerationModeEnabled
  - 範例值:
``` xml
<true/>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### ImportAutofillFormData
  #### 允許匯入自動填滿表單資料
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  允許使用者從另一個瀏覽器將自動填滿表格匯入 Microsoft Edge。

如果您啟用這個原則，將會自動選取手動匯入自動填滿表格設定。

如果您停用此原則，自動填滿表格將不會在第一次執行時匯入，且使用者無法手動匯入。

如果您未設定此原則，將會在第一次執行時匯入自動填滿表格，且使用者可以選擇是否要在稍後瀏覽工作階段期間將手動匯入。

您也可以設定此原則為建議值。這表示 Microsoft Edge 會在第一次執行時匯入自動填滿表格，但使用者可以在手動匯入期間選取或清除 **自動填滿資料** 選項。

**注意**: 此原則目前管理從 Google Chrome (Windows 7、8、10 和 macOS 上) 匯入。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 是
  - 動態原則重新整理: 是

  #### 資料類型:
  布林值

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: ImportAutofillFormData
  - GP 名稱: 允許匯入自動填滿表單資料
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): 系統管理範本/Microsoft Edge - 預設設定 (使用者可以覆寫)/
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): SOFTWARE\Policies\Microsoft\Edge\推薦項目
  - 值名稱: ImportAutofillFormData
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000001
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: ImportAutofillFormData
  - 範例值:
``` xml
<true/>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### ImportBrowserSettings
  #### 允許匯入瀏覽器設定
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (78 版或更新版本)

  #### 描述
  允許使用者將瀏覽器設定從其他瀏覽器匯入 Microsoft Edge。

如果啟用此原則，則 **瀏覽器設定** 核取方塊將自動在 [匯入瀏覽器資料] 對話方塊中選取。

如果停用此原則，瀏覽器設定在第一次執行時將不會匯入，且使用者無法手動匯入。

如果不設定此原則，瀏覽器設定在第一次執行時將會匯入，使用者可以選擇是否在稍後瀏覽工作階段中手動匯入。

您也可以將此策略設定為推薦。這代表 Microsoft Edge 將在第一次執行時匯入設定，但使用者可以在手動匯入期間選擇或清除 **瀏覽器設定** 選項。

**注意**: 此原則目前負責管理 Google Chrome (Windows 7、8、10 和 macOS) 的匯入資料。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 是
  - 動態原則重新整理: 是

  #### 資料類型:
  布林值

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: ImportBrowserSettings
  - GP 名稱: 允許匯入瀏覽器設定
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): 系統管理範本/Microsoft Edge - 預設設定 (使用者可以覆寫)/
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): SOFTWARE\Policies\Microsoft\Edge\推薦項目
  - 值名稱: ImportBrowserSettings
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000001
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: ImportBrowserSettings
  - 範例值:
``` xml
<true/>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### ImportFavorites
  #### 允許匯入 [我的最愛]
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  允許使用者從另一個瀏覽器將我的最愛匯入 Microsoft Edge。

如果您啟用這個原則，將會在 **匯入瀏覽器資料** 對話方塊中自動選取 **我的最愛** 核取方塊。

如果您停用此原則，我的最愛將不會在第一次執行時匯入，且使用者無法手動匯入。

如果您未設定此原則，將會在第一次執行時匯入我的最愛，且使用者可以選擇是否要在稍後瀏覽工作階段期間將手動匯入。

您也可以設定此原則為建議值。這表示 Microsoft Edge 會在第一次執行時匯入我的最愛，但使用者可以在手動匯入期間選取或清除 **我的最愛** 選項。

**注意**: 此原則目前管理從 Internet Explorer (Windows 7、8、10 和 macOS 上)、Google Chrome 線上應用程式 (Windows 7、8、10 和 macOS 上) 和 Apple Safari  (macOS 上) 瀏覽器匯入。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 是
  - 動態原則重新整理: 是

  #### 資料類型:
  布林值

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: ImportFavorites
  - GP 名稱: 允許匯入 [我的最愛]
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): 系統管理範本/Microsoft Edge - 預設設定 (使用者可以覆寫)/
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): SOFTWARE\Policies\Microsoft\Edge\推薦項目
  - 值名稱: ImportFavorites
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000001
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: ImportFavorites
  - 範例值:
``` xml
<true/>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### ImportHistory
  #### 允許匯入瀏覽歷程記錄
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  允許使用者從到另一個瀏覽器匯入其瀏覽歷程記錄至 Microsoft Edge。

如果您啟用此原則，**瀏覽歷程記錄** 核取方塊會自動選取 **匯入瀏覽器資料** 對話方塊。

如果您停用此原則，瀏覽歷程記錄資料在第一次執行時不會匯入，且使用者無法手動匯入此資料。

如果您未設定此原則，則瀏覽歷程記錄資料將在第一次執行時匯入，且使用者可以選擇是否要在稍後瀏覽工作階段期間手動匯入。

您也可以設定此原則為建議值。這表示 Microsoft Edge 會在第一次執行時匯入密碼，但使用者可以在手動匯入期間選取或清除 **歷史** 選項。

**注意**: 此原則目前管理來自 Internet Explorer (Windows 7、8 和 10 上) 與 Google Chrome (Windows 7、8、10 和 macOS 上) 和 Apple Safari (macOS) 瀏覽器的匯入內容。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 是
  - 動態原則重新整理: 是

  #### 資料類型:
  布林值

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: ImportHistory
  - GP 名稱: 允許匯入瀏覽歷程記錄
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): 系統管理範本/Microsoft Edge - 預設設定 (使用者可以覆寫)/
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): SOFTWARE\Policies\Microsoft\Edge\推薦項目
  - 值名稱: ImportHistory
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000001
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: ImportHistory
  - 範例值:
``` xml
<true/>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### ImportHomepage
  #### 允許匯入首頁設定
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  允許使用者從另一個瀏覽器將首頁設定匯入 Microsoft Edge。

如果您啟用這個原則，將會自動選取手動匯入首頁頁面設定。

如果您停用此原則，首頁頁面設定將不會在第一次執行時匯入，且使用者無法手動匯入。

如果您未設定此原則，將會在第一次執行時匯入首頁頁面設定，且使用者可以選擇是否要在稍後瀏覽工作階段期間將手動匯入。

您也可以設定此原則為建議值。這表示 Microsoft Edge 會在第一次執行時匯入首頁頁面設定，但使用者可以在手動匯入期間選取或清除 **首頁頁面設** 選項。

**注意**: 此原則目前管理從 Internet Explorer (Windows 7、8 和 10) 匯入。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  布林值

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: ImportHomepage
  - GP 名稱: 允許匯入首頁設定
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: ImportHomepage
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000001
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: ImportHomepage
  - 範例值:
``` xml
<true/>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### ImportOpenTabs
  #### 允許匯入已開啟的索引標籤
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (79 版或更新版本)

  #### 描述
  可讓使用者將已開啟和釘選的索引標籤從其他瀏覽器匯入 Microsoft Edge。

如果啟用此原則，則 **已開啟的索引標籤** 核取方塊將自動在 **匯入瀏覽器資料** 對話方塊中選取。

如果停用此原則，已開啟的索引標籤在第一次執行時將不會匯入，且使用者無法手動匯入。

如果不設定此原則，已開啟的索引標籤在第一次執行時將會匯入，使用者可以選擇是否在稍後瀏覽工作階段中手動匯入。

您也可以將此原則設為建議。這代表 Microsoft Edge 將在第一次執行時匯入已開啟的索引標籤，但使用者可以在手動匯入期間選擇或清除 **已開啟的索引標籤** 選項。

**注意**：此原則目前僅支援從 Google Chrome (Windows 7、8、10 和 macOS) 匯入資料。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 是
  - 動態原則重新整理: 是

  #### 資料類型:
  布林值

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: ImportOpenTabs
  - GP 名稱: 允許匯入已開啟的索引標籤
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): 系統管理範本/Microsoft Edge - 預設設定 (使用者可以覆寫)/
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): SOFTWARE\Policies\Microsoft\Edge\推薦項目
  - 值名稱: ImportOpenTabs
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000001
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: ImportOpenTabs
  - 範例值:
``` xml
<true/>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### ImportPaymentInfo
  #### 允許匯入付款資訊
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  允許使用者從另一個瀏覽器將付款資訊匯入 Microsoft Edge。

如果您啟用這個原則，將會在 **付款資訊** 對話方塊中自動選取 **匯入瀏覽器資料** 核取方塊。

如果您停用此原則，付款資訊將不會在第一次執行時匯入，且使用者無法手動匯入。

如果您未設定此原則，將會在第一次執行時匯入付款資訊，且使用者可以選擇是否要在稍後瀏覽工作階段期間將手動匯入。

您也可以設定此原則為建議值。這表示 Microsoft Edge 會在第一次執行時匯入付款資訊，但使用者可以在手動匯入期間選取或清除 **付款資訊** 選項。

**注意**: 此原則目前管理從 Google Chrome 線上應用程式 (Windows 7、8、10 和 macOS 上) 瀏覽器匯入。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 是
  - 動態原則重新整理: 是

  #### 資料類型:
  布林值

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: ImportPaymentInfo
  - GP 名稱: 允許匯入付款資訊
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): 系統管理範本/Microsoft Edge - 預設設定 (使用者可以覆寫)/
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): SOFTWARE\Policies\Microsoft\Edge\推薦項目
  - 值名稱: ImportPaymentInfo
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000001
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: ImportPaymentInfo
  - 範例值:
``` xml
<true/>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### ImportSavedPasswords
  #### 允許匯入已儲存的密碼
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  允許使用者將已儲存密碼從其他瀏覽器匯入到 Microsoft Edge。

如果您啟用此原則，則將會自動選取手動匯入儲存密碼的選項。

如果您停用此原則，則已儲存的密碼將不會在第一次執行時匯入，且使用者無法手動匯入。

如果您未設定此原則，密碼將會在第一次執行時匯入，且使用者可以選擇是否要在稍後瀏覽工作階段期間手動匯入。

您可以設定此原則為建議值。這表示 Microsoft Edge 會在第一次執行時匯入密碼，但使用者可以在手動匯入期間選取或清除 **密碼** 選項。

**注意**: 此原則目前管理來自 Internet Explorer (Windows 7、8 和 10 上) 與 Google Chrome (Windows 7、8、10 和 macOS 上) 瀏覽器的匯入內容。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 是
  - 動態原則重新整理: 是

  #### 資料類型:
  布林值

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: ImportSavedPasswords
  - GP 名稱: 允許匯入已儲存的密碼
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): 系統管理範本/Microsoft Edge - 預設設定 (使用者可以覆寫)/
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): SOFTWARE\Policies\Microsoft\Edge\推薦項目
  - 值名稱: ImportSavedPasswords
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000001
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: ImportSavedPasswords
  - 範例值:
``` xml
<true/>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### ImportSearchEngine
  #### 允許匯入搜尋引擎設定
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  允許使用者從到另一個瀏覽器匯入其搜尋引擎設定至 Microsoft Edge。

如果您啟用此原則，**瀏覽歷程記錄** 核取方塊會自動選取搜尋引擎設定。

如果您停用此原則，搜尋引擎設定在第一次執行時不會匯入，且使用者無法手動匯入此資料。

如果您未設定此原則，則搜尋引擎設定將在第一次執行時匯入，且使用者可以選擇是否要在稍後瀏覽工作階段期間手動匯入。

您也可以設定此原則為建議值。這表示 Microsoft Edge 會在第一次執行時匯入密碼，但使用者可以在手動匯入期間選取或清除 **搜尋引擎** 選項。

**注意**: 此原則目前管理來自 Internet Explorer (Windows 7、8 和 10 上) 的匯入內容。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 是
  - 動態原則重新整理: 是

  #### 資料類型:
  布林值

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: ImportSearchEngine
  - GP 名稱: 允許匯入搜尋引擎設定
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): 系統管理範本/Microsoft Edge - 預設設定 (使用者可以覆寫)/
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): SOFTWARE\Policies\Microsoft\Edge\推薦項目
  - 值名稱: ImportSearchEngine
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000001
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: ImportSearchEngine
  - 範例值:
``` xml
<true/>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### InPrivateModeAvailability
  #### 設定 InPrivate 模式可用性
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  指定使用者是否可以在 InPrivate 模式開啟頁面 Microsoft Edge。

如果您未設定這個原則，或將它設定為 'Enabled' (0)，則使用者可以開啟的網頁以 InPrivate 模式。

設定此原則，以 'Disable' (1) 若要停止使用者使用 InPrivate 模式。

設定此原則，以 '強制' (2) 若要一律使用 InPrivate 模式。

* 0 = InPrivate 模式

* 1 = InPrivate 模式已停用

* 2 = 強制 InPrivate 模式

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  整數

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: InPrivateModeAvailability
  - GP 名稱: 設定 InPrivate 模式可用性
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: InPrivateModeAvailability
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000001
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: InPrivateModeAvailability
  - 範例值:
``` xml
<integer>1</integer>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### InternetExplorerIntegrationLevel
  #### 設定 Internet Explorer 整合
  >支援的版本: Windows 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  如需設定 Internet Explorer 模式的最佳體驗教學，請參閱 [https://go.microsoft.com/fwlink/?linkid=2094210](https://go.microsoft.com/fwlink/?linkid=2094210)

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 否 - 需要重新啟動瀏覽器

  #### 資料類型:
  整數

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: InternetExplorerIntegrationLevel
  - GP 名稱: 設定 Internet Explorer 整合
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: InternetExplorerIntegrationLevel
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000001
```


  

  [回到頂端](#microsoft-edge---原則)

  ### InternetExplorerIntegrationSiteList
  #### 設定 [企業模式網站清單]
  >支援的版本: Windows 上的 Microsoft Edge (78 版或更新版本)

  #### 描述
  如需設定 Internet Explorer 模式的最佳體驗教學，請參閱 [https://go.microsoft.com/fwlink/?linkid=2094210](https://go.microsoft.com/fwlink/?linkid=2094210)

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 否 - 需要重新啟動瀏覽器

  #### 資料類型:
  字串

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: InternetExplorerIntegrationSiteList
  - GP 名稱: 設定 [企業模式網站清單]
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: InternetExplorerIntegrationSiteList
  - 數值類型: REG_SZ
  ##### 範例值:
```
"https://internal.contoso.com/sitelist.xml"
```


  

  [回到頂端](#microsoft-edge---原則)

  ### IsolateOrigins
  #### 為特定來源啟用網站隔離
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  指定來源在其處理程序中隔離執行。
此原則也會隔離子網域命名的來源 - 例如，指定 https://contoso.com/ 將導致 https://foo.contoso.com/ 隔離為 https://contoso.com/ 的一部分。
如果啟用此原則，則以逗點分隔清單中的每個命名來源，都將在其處理程序中執行。
如果停用此原則，則 'IsolateOrigins' 和 'SitePerProcess' 功能都將停用。使用者仍可以透過命令列旗標手動啟用 'IsolateOrigins' 原則。
如果不設定原則，使用者可以變更此原則。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 否 - 需要重新啟動瀏覽器

  #### 資料類型:
  字串

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: IsolateOrigins
  - GP 名稱: 為特定來源啟用網站隔離
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: IsolateOrigins
  - 數值類型: REG_SZ
  ##### 範例值:
```
"https://contoso.com/,https://fabrikam.com/"
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: IsolateOrigins
  - 範例值:
``` xml
<string>https://contoso.com/,https://fabrikam.com/</string>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### ManagedFavorites
  #### 設定我的最愛
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  設定受管理的我的最愛清單。

此原則會建立我的最愛清單。每個我的最愛項目均包含索引鍵 [名稱] 與 [url]，包含我的最愛名稱與目標。若要設定子資料夾，您可以無需使用「url」鍵，但而是透過其他「子系」鍵，像是上方曾定義過的我的最愛 (某些可能又是資料夾)。透過網址列提交時，Microsoft Edge 會修改不完整的 URL，像是「microsoft.com」變成「https://microsoft.com/」。

這些資料夾中的我的最愛無法由使用者修改 (但使用者可以選擇從我的最愛列隱藏)。預設的資料夾名稱是 「受管理的我的最愛」，但您可以透過想要的資料夾名稱值新增包含機碼「toplevel_name」的我的最愛清單，並加以變更。

受管理的我的最愛不會與使用者帳戶同步，且無法由擴充功能修改。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  字典

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: ManagedFavorites
  - GP 名稱: 設定我的最愛
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: ManagedFavorites
  - 數值類型: REG_SZ
  ##### 範例值:
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


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: ManagedFavorites
  - 範例值:
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
  

  [回到頂端](#microsoft-edge---原則)

  ### ManagedSearchEngines
  #### 管理搜索引擎
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  可讓您設定最多 10 個的搜尋引擎清單，其中一個必須標記為預設搜尋引擎。
您無需指定任何搜尋引擎編碼。

如果啟用此原則，則使用者無法新增、移除或變更清單中的任何搜尋引擎。使用者可將清單中的任一搜尋引擎設為預設搜尋引擎。

如果停用或未設定此原則，則使用者可視需要修改搜尋引擎清單。

如果設定了 [DefaultSearchProviderSearchURL](#defaultsearchprovidersearchurl) 原則，則會忽略此原則 (ManagedSearchEngines)。使用者必須重新啟動瀏覽器才能成功套用此原則。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 否 - 需要重新啟動瀏覽器

  #### 資料類型:
  字典

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: ManagedSearchEngines
  - GP 名稱: 管理搜索引擎
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: ManagedSearchEngines
  - 數值類型: REG_SZ
  ##### 範例值:
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


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: ManagedSearchEngines
  - 範例值:
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
  

  [回到頂端](#microsoft-edge---原則)

  ### MaxConnectionsPerProxy
  #### 同時連線到 Proxy 伺服器的最大數目
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  指定 Proxy 伺服器的同時連線數目上限。

某些 Proxy 伺服器可能無法處理每個用戶端大量的同時連線 - 您可以透過將此原則設定為較低的值，解決此問題。

此原則的值應小於 100 並高於 6。預設值為 32。

已知某些 Web App 會透過溢出 [GET] 耗用過多連線 -  如果開啟過多這些類型的 Web App，將最大連線數降至 32 以下可能會導致瀏覽器網路中斷。

如果您未設定此原則，則會使用預設值 (32)。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 否 - 需要重新啟動瀏覽器

  #### 資料類型:
  整數

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: MaxConnectionsPerProxy
  - GP 名稱: 同時連線到 Proxy 伺服器的最大數目
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: MaxConnectionsPerProxy
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000020
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: MaxConnectionsPerProxy
  - 範例值:
``` xml
<integer>32</integer>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### MediaRouterCastAllowAllIPs
  #### 允許 Google Cast 連線至所有 IP 位址上的 Cast 裝置
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  啟用此原則以允許 Google Cast 連線至所有 IP 位址上的 Cast 裝置，不只是 RFC1918/RFC4193 私人位址。

停用此原則以限制 Google Cast 連線至 RFC1918/RFC4193 私人位址上的 Cast 裝置。

如果您未設定此原則，除非啟用 CastAllowAllIPs 功能，Google Cast 僅會連線至 RFC1918/RFC4193 私人位址上的 Cast 裝置。

如果 [EnableMediaRouter](#enablemediarouter) 已停用此原則，則此原則將無效。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  布林值

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: MediaRouterCastAllowAllIPs
  - GP 名稱: 允許 Google Cast 連線至所有 IP 位址上的 Cast 裝置
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: MediaRouterCastAllowAllIPs
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000000
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: MediaRouterCastAllowAllIPs
  - 範例值:
``` xml
<false/>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### MetricsReportingEnabled
  #### 啟用使用量及當機相關資料報告
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  對於 Microsoft Edge 的 Windows 10 Beta 版與穩定版通道，此原則設定時將會覆寫 Windows 診斷資料集合設定或非集合 Microsoft Edge 使用量與損毀相關資料 ([https://go.microsoft.com/fwlink/?linkid=2099569](https://go.microsoft.com/fwlink/?linkid=2099569))。

此原則可將關於 Microsoft Edge 的使用量與損毀相關資料報告給 Microsoft，並防止使用者變更此設定。

啟用此原則以傳送使用量與損毀相資料的報告給 Microsoft。停用此原則即不會將資料傳送給 Microsoft。在此兩種情況下，使用者無法變更或覆寫設定。

在 Windows 10、Beta 版與穩定版通道上，此原則能控制使用量資料。與毀損相關的資料由 Windows 診斷資料設定決定。如果未設定此原則，Microsoft Edge 將預設為 Windows 診斷資料設定。

在 Windows 10、Canary 與 Dev 通道上，此原則可以控制使用量與損毀相關資料。如果未設定此原則，Microsoft Edge 將預設為使用者的喜好設定。

在 Windows 7、8 和 Mac 上，此原則可以控制使用量和損毀相關資料。如果未設定此原則，Microsoft Edge 將預設為使用者的喜好設定。

此原則僅適用於已加入 Microsoft Active Directory 網域的 Windows 執行個體，或已註冊裝置管理的 Windows 10 專業版或企業版執行個體。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 否 - 需要重新啟動瀏覽器

  #### 資料類型:
  布林值

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: MetricsReportingEnabled
  - GP 名稱: 啟用使用量及當機相關資料報告
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: MetricsReportingEnabled
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000001
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: MetricsReportingEnabled
  - 範例值:
``` xml
<true/>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### NetworkPredictionOptions
  #### 啟用網路預測
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  啟用網路預測，並防止使用者變更此設定。

這會控制 DNS 預先擷取、TCP 和 SSL 預先連線和預先轉譯網頁。

如果不設定此原則，即便已啟用網絡預測，使用者依然可以進行變更。

* 0 =預測任何網路連線上的網路動作

* 2 =不預測任何網路連線上的網路動作

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 是
  - 動態原則重新整理: 是

  #### 資料類型:
  整數

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: NetworkPredictionOptions
  - GP 名稱: 啟用網路預測
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): 系統管理範本/Microsoft Edge - 預設設定 (使用者可以覆寫)/
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): SOFTWARE\Policies\Microsoft\Edge\推薦項目
  - 值名稱: NetworkPredictionOptions
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000001
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: NetworkPredictionOptions
  - 範例值:
``` xml
<integer>1</integer>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### NonRemovableProfileEnabled
  #### 設定使用者是否一律擁有其公司或學校帳戶自動登入的預設設定檔
  >支援的版本: Windows 上的 Microsoft Edge (78 版或更新版本)

  #### 描述
  This policy determines if a user can remove the Microsoft Edge profile automatically signed in with a user's work or school account.

If you enable this policy, a non-removable profile will be created with the user's work or school account on Windows. This profile can't be signed out or removed.

If you disable or don't configure this policy, the profile automatically signed in with a user's work or school account on Windows can be signed out or removed by the user.

If you want to configure browser sign in, use the [BrowserSignin](#browsersignin) policy.

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  布林值

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: NonRemovableProfileEnabled
  - GP 名稱: 設定使用者是否一律擁有其公司或學校帳戶自動登入的預設設定檔
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: NonRemovableProfileEnabled
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000001
```


  

  [回到頂端](#microsoft-edge---原則)

  ### OverrideSecurityRestrictionsOnInsecureOrigin
  #### 控制不安全來源中安全性限制套用的地方
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  指定不適用非安全來源中安全性限制的來源 (URL) 或主機名稱模式 (例如「*.contoso.com」) 的列表。

此原則可讓您指定無法部署 TLS 或設定內部網頁程式開發的暫存伺服器的繼承應用程式的允許來源，讓開發人員可以測試需要安全內容功能，而不需在暫存伺服器上部署 TLS。此原則也會防止來源在 Omnibox 中標示為「不安全」。

此原則中 Url 的清單設定也會與將命令列旗標 [-unsafely-treat-insecure-origin-as-secure] 設定為以逗號分隔的相同 URL 清單有相同效果。如果您啟用此原則，則會覆寫命令列旗標。

如需有關安全內容的詳細資訊，請參閱 https://www.w3.org/TR/secure-contexts/。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 否 - 需要重新啟動瀏覽器

  #### 資料類型:
  字串的清單

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: OverrideSecurityRestrictionsOnInsecureOrigin
  - GP 名稱: 控制不安全來源中安全性限制套用的地方
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge\OverrideSecurityRestrictionsOnInsecureOrigin
  - 路徑 (推薦項目): N/A
  - 值名稱: 1, 2, 3, ...
  - 數值類型: REG_SZ 的清單
  ##### 範例值:
```
SOFTWARE\Policies\Microsoft\Edge\OverrideSecurityRestrictionsOnInsecureOrigin\0 = "http://testserver.contoso.com/"
SOFTWARE\Policies\Microsoft\Edge\OverrideSecurityRestrictionsOnInsecureOrigin\1 = "*.contoso.com"

```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: OverrideSecurityRestrictionsOnInsecureOrigin
  - 範例值:
``` xml
<array>
  <string>http://testserver.contoso.com/</string>
  <string>*.contoso.com</string>
</array>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### PinningWizardAllowed
  #### 允許 [釘選到工作列精靈]
  >支援的版本: Windows 上的 Microsoft Edge (80 版或更新版本)

  #### 描述
  Microsoft Edge 使用 [釘選到工作列精靈] 來幫助使用者將建議的網站釘選到工作列。在預設情況下，[釘選到工作列精靈] 的功能為啟用狀態，使用者可以透過 [設定和其他功能表] 進行設定。

如果啟用或未設定此原則，則使用者可以在 [設定和其他功能表] 中呼叫 [釘選到工作列精靈]。也可以透過啟動通訊協定來呼叫該精靈。

如果停用此原則，則功能表中的 [釘選到工作列精靈] 將會停用，並且無法透過啟動通訊協定來呼叫。

使用者無法設定啟用或停用 [釘選到工作列精靈]。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 否 - 需要重新啟動瀏覽器

  #### 資料類型:
  布林值

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: PinningWizardAllowed
  - GP 名稱: 允許 [釘選到工作列精靈]
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: PinningWizardAllowed
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000000
```


  

  [回到頂端](#microsoft-edge---原則)

  ### ProactiveAuthEnabled
  #### 啟用主動式驗證
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  讓您設定是否要開啟主動式驗證。

如果您啟用此原則，Microsoft Edge 會透過 Microsoft 服務嘗試主動驗證登入使用者。Microsoft Edge 會以固定間隔檢查含有負責控制如何執行此操作的線上更新資訊清單。

如果您停用此原則，Microsoft Edge 不會嘗試透過 Microsoft 服務主動驗證登入使用者。Microsoft Edge 不會再檢查含有負責控制如何執行此操作的線上更新資訊清單。

如果您未設定此原則，[主動式驗證] 將會開啟。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 否 - 需要重新啟動瀏覽器

  #### 資料類型:
  布林值

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: ProactiveAuthEnabled
  - GP 名稱: 啟用主動式驗證
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: ProactiveAuthEnabled
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000001
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: ProactiveAuthEnabled
  - 範例值:
``` xml
<true/>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### PromotionalTabsEnabled
  #### 啟用全分頁促銷內容
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  控制全分頁促銷或教育內容的呈現。此設定會控制協助使用者登入 Microsoft Edge 的歡迎頁面外觀，請選擇其預設瀏覽器，或深入了解產品功能。

如果您啟用此原則 (設定為 True) 或未設定，則 Microsoft Edge 可以顯示完整分頁內容給使用者，提供產品資訊。

如果您停用 (設為 False) 原則，Microsoft Edge 將無法顯示完整分頁內容給使用者。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  布林值

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: PromotionalTabsEnabled
  - GP 名稱: 啟用全分頁促銷內容
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: PromotionalTabsEnabled
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000000
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: PromotionalTabsEnabled
  - 範例值:
``` xml
<false/>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### PromptForDownloadLocation
  #### 詢問下載檔案的儲存位置
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  設定是否要在下載前詢問檔案的儲存位置。

如果您啟用此原則，則會在每個檔案下載前詢問儲存位置；如果您未設定，檔案會自動儲存到預設位置，而不會詢問使用者。

如果您未設定此原則，使用者將無法變更此設定。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  布林值

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: PromptForDownloadLocation
  - GP 名稱: 詢問下載檔案的儲存位置
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: PromptForDownloadLocation
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000000
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: PromptForDownloadLocation
  - 範例值:
``` xml
<false/>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### QuicAllowed
  #### 允許 QUIC 通訊協定
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  允許在 Microsoft Edge 中使用 QUIC 通訊協定。

如果您啟用這個原則或未設定，則允許 QUIC 通訊協定。

如果您停用此原則，便會封鎖 QUIC 通訊協定。

QUIC 是一種傳輸層網路協議，能提高目前使用 TCP 的網路應用程式效能。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 否 - 需要重新啟動瀏覽器

  #### 資料類型:
  布林值

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: QuicAllowed
  - GP 名稱: 允許 QUIC 通訊協定
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: QuicAllowed
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000001
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: QuicAllowed
  - 範例值:
``` xml
<true/>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### RelaunchNotification
  #### 通知使用者建議或需要重新啟動瀏覽器，以套用擱置中的更新
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  通知使用者他們需要重新啟動 Microsoft Edge 以套用暫止的更新。

如果您未設定這個原則，Microsoft Edge 會新增回收圖示最右邊的排名最前面的功能表列，以提示使用者重新啟動瀏覽器以套用更新。

如果您啟用此原則，並將其設定為 'Recommended' (1)，週期性警告會提示使用者建議重新啟動。使用者可以關閉此警告，並延後重新啟動的時間。

如果您設定這個原則為 'Required' (2) 時，警告會提示使用者的瀏覽器將會自動重新啟動盡通知期間週期性傳遞。預設的期間是七天。您可以設定這段期間的 [RelaunchNotificationPeriod](#relaunchnotificationperiod) 原則。

重新啟動瀏覽器時，會還原使用者的工作階段。

* Recommended (1) = 顯示使用者指出的週期性提示，建議您重新啟動

* Required (2) = 顯示週期性，向使用者提示必須重新啟動

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  整數

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: RelaunchNotification
  - GP 名稱: 通知使用者建議或需要重新啟動瀏覽器，以套用擱置中的更新
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: RelaunchNotification
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000001
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: RelaunchNotification
  - 範例值:
``` xml
<integer>1</integer>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### RelaunchNotificationPeriod
  #### 設定更新通知的時間週期
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  可讓您設定時間期限 (以毫秒為單位)，在該時間期限內，將通知使用者必須重新啟動 Microsoft Edge 或 Microsoft Edge OS 裝置才能套用擱置的更新。

在此時間段內，系統將反覆通知使用者需要更新。對於 Microsoft Edge OS 裝置，根據 RelaunchHeadsUpPeriod 原則，系統匣中會出現重新啟動通知。對於 Microsoft Edge 瀏覽器，應用程式功能表將改為一旦通知期限經過三分之一，則需要重新啟動。通知期限經過三分之二後，此通知將改變顏色，而整個通知期限結束後，此通知將再次變更顏色。[RelaunchNotification](#relaunchnotification) 原則啟用的其他通知也遵循此相同的設定。

如果未設定，則預設時間期限為 604800000 毫秒 (一周)。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  整數

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: RelaunchNotificationPeriod
  - GP 名稱: 設定更新通知的時間週期
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: RelaunchNotificationPeriod
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x240c8400
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: RelaunchNotificationPeriod
  - 範例值:
``` xml
<integer>604800000</integer>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### RendererCodeIntegrityEnabled
  #### 啟用轉譯器程式碼完整性
  >支援的版本: Windows 上的 Microsoft Edge (78 版或更新版本)

  #### 描述
  如果此原則已啟用或未設定，則轉譯器程式碼完整性就會啟用。除非與必須在 Microsoft Edge 轉譯器處理序中執行的協力廠商軟體發生相容性問題，否則不應停用此原則。

因為停用此原則會使未知和可能有惡意的程式碼能在 Microsoft Edge 的轉譯器處理序中載入，所以停用此原則會對 Microsoft Edge 的安全性與穩定性造成不利的影響。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 否 - 需要重新啟動瀏覽器

  #### 資料類型:
  布林值

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: RendererCodeIntegrityEnabled
  - GP 名稱: 啟用轉譯器程式碼完整性
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: RendererCodeIntegrityEnabled
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000000
```


  

  [回到頂端](#microsoft-edge---原則)

  ### RequireOnlineRevocationChecksForLocalAnchors
  #### 指定本機信賴起點是否需要線上 OCSP / CRL 檢查
  >支援的版本: Windows 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  控制是否需要線上撤銷檢查 （OCSP/CRL 檢查）。如果 Microsoft Edge 無法取得撤銷狀態的詳細資訊，這些憑證都會被視為撤銷 （"硬碟失敗"）。

如果您啟用這個原則， Microsoft Edge 一定會先執行撤銷檢查已成功驗證，由本機安裝 CA 憑證所簽署的伺服器憑證。

如果您未設定或停用這個原則，然後 Microsoft Edge 使用現有的線上撤銷檢查設定。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  布林值

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: RequireOnlineRevocationChecksForLocalAnchors
  - GP 名稱: 指定本機信賴起點是否需要線上 OCSP / CRL 檢查
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: RequireOnlineRevocationChecksForLocalAnchors
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000000
```


  

  [回到頂端](#microsoft-edge---原則)

  ### ResolveNavigationErrorsUseWebService
  #### 透過網頁服務啟用瀏覽錯誤解析度
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  允許 Microsoft Edge 發出無資料連線至 Web 服務，以探查網路連線狀況，例如旅館與機場 Wi-Fi。

如果您啟用此原則，Web 服務會用於網路連線能力測試。

  如果您停用此原則，Microsoft Edge 會使用原生 API 以嘗試解決網路連線狀態及瀏覽問題。

**注意**: 除了在 Windows 8 和更新版本 Windows，Microsoft Edge *一律* 使用原生 API 來解決連線問題。

如果您未設定此原則，Microsoft Edge 會遵循設定在 edge://settings/privacy 服務下的使用者喜好設定。
特別是 **使用 Web 服務協助解決瀏覽錯誤** 切換，使用者可以切換開啟或關閉。請注意，如果您啟用此原則 (ResolveNavigationErrorsUseWebService)，**使用以協助解決瀏覽錯誤** 設定會開啟，但使用者無法變更此設定進行切換。如果您停用此原則，**使用 Web 服務以協助解決瀏覽錯誤** 設定會關閉，而且使用者無法變更此設定來切換。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 是
  - 動態原則重新整理: 是

  #### 資料類型:
  布林值

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: ResolveNavigationErrorsUseWebService
  - GP 名稱: 透過網頁服務啟用瀏覽錯誤解析度
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): 系統管理範本/Microsoft Edge - 預設設定 (使用者可以覆寫)/
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): SOFTWARE\Policies\Microsoft\Edge\推薦項目
  - 值名稱: ResolveNavigationErrorsUseWebService
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000001
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: ResolveNavigationErrorsUseWebService
  - 範例值:
``` xml
<true/>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### RestrictSigninToPattern
  #### 限制哪些帳戶可用為 Microsoft Edge 主要帳戶
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  決定那些帳戶可以在 Microsoft Edge (在同步加入流程中選擇的帳戶) 中，設定為瀏覽器主要帳戶。

如果使用者嘗試使用與此模式不相符的使用者名稱設定瀏覽器主要帳戶，則會封鎖該帳戶並顯示相應的錯誤訊息。

如果您未設定此原則或將其留白，則使用者可以在 Microsoft Edge 中，將任何帳戶設定為瀏覽器主要帳戶。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  字串

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: RestrictSigninToPattern
  - GP 名稱: 限制哪些帳戶可用為 Microsoft Edge 主要帳戶
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: RestrictSigninToPattern
  - 數值類型: REG_SZ
  ##### 範例值:
```
".*@contoso.com"
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: RestrictSigninToPattern
  - 範例值:
``` xml
<string>.*@contoso.com</string>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### RunAllFlashInAllowMode
  #### 將 Adobe Flash 內容設定延伸至所有內容
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  如果啟用此原則，所有在內容設定中設為允許 Adobe Flash 的網站，無論是由使用者或企業原則設定，這些網站皆會執行內嵌的 Adobe Flash 內容的。這包括來自其他來源和/或小量內容的內容。

若要控制允許執行 Adobe Flash 的網站，請參閱 [DefaultPluginsSetting](#defaultpluginssetting)、[PluginsAllowedForUrls](#pluginsallowedforurls) 和 [PluginsBlockedForUrls](#pluginsblockedforurls) 原則中的詳細說明。

如果停用或未設定此原則，可能會封鎖來自其他來源 (上述的三個原則中未指定的網站) 或小量內容的 Adobe Flash。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  布林值

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: RunAllFlashInAllowMode
  - GP 名稱: 將 Adobe Flash 內容設定延伸至所有內容
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: RunAllFlashInAllowMode
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000001
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: RunAllFlashInAllowMode
  - 範例值:
``` xml
<true/>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### SSLErrorOverrideAllowed
  #### 允許使用者從 HTTPS 警告頁面繼續
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  Microsoft Edge使用者造訪的網站時，具有 SSL 錯誤時，會顯示警告頁面。

如果您啟用或未設定 (預設值) 此原則，使用者可以按一下透過這些警告的頁面。

如果您停用此原則，會防止使用者按下透過任何警告頁面。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  布林值

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: SSLErrorOverrideAllowed
  - GP 名稱: 允許使用者從 HTTPS 警告頁面繼續
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: SSLErrorOverrideAllowed
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000001
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: SSLErrorOverrideAllowed
  - 範例值:
``` xml
<true/>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### SSLVersionMin
  #### 已啟用最低 TLS 版本
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  設定 SSL 支援的最低版本。如果您未設定這個原則， Microsoft Edge會使用預設最小版本，TLS 1.0。

如果您啟用這個原則，您可以設定的最小版本為下列值之一:"tls1"，"tls1.1"或"tls1.2"。設定時， Microsoft Edge將不會使用 SSL/TLS 低於指定任何的版本版本。無法辨識的任何值會略過。

* "tls1" = TLS 1.0

* "tls1.1" = TLS 1.1

* "tls1.2" = TLS 1.2

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  字串

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: SSLVersionMin
  - GP 名稱: 已啟用最低 TLS 版本
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: SSLVersionMin
  - 數值類型: REG_SZ
  ##### 範例值:
```
"tls1"
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: SSLVersionMin
  - 範例值:
``` xml
<string>tls1</string>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### SavingBrowserHistoryDisabled
  #### 停用儲存瀏覽器歷程記錄
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  停用儲存瀏覽器歷程記錄並防止使用者變更此設定。

如果啟用此原則，則不會儲存瀏覽歷程記錄。同時也會停用同步索引標籤。

如果停用或不設定此原則，則會儲存瀏覽歷程記錄。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  布林值

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: SavingBrowserHistoryDisabled
  - GP 名稱: 停用儲存瀏覽器歷程記錄
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: SavingBrowserHistoryDisabled
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000001
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: SavingBrowserHistoryDisabled
  - 範例值:
``` xml
<true/>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### SearchSuggestEnabled
  #### 啟用搜尋建議
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  在 Microsoft Edge 的 [網址列] 與 [自動建議清單] 中啟用網頁搜尋建議，並防止使用者並更此原則。

如果您啟用此原則，則會使用網頁搜尋建議。

如果您停用此原則，則不會使用網頁建議，但本機歷史紀錄與本機最愛建議仍會顯示。如果您停用此原則，無論是已輸入字元或曾造訪的 URL 都將不會包含在傳送至 Microsoft 的遙測中。

如果此原則未設定，搜尋建議將會啟用，但使用者仍能變更。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 是
  - 動態原則重新整理: 是

  #### 資料類型:
  布林值

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: SearchSuggestEnabled
  - GP 名稱: 啟用搜尋建議
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): 系統管理範本/Microsoft Edge - 預設設定 (使用者可以覆寫)/
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): SOFTWARE\Policies\Microsoft\Edge\推薦項目
  - 值名稱: SearchSuggestEnabled
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000001
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: SearchSuggestEnabled
  - 範例值:
``` xml
<true/>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### SecurityKeyPermitAttestation
  #### 不需要權限即可使用直接存取 [安全性金鑰] 證明的網站或網域
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  當安全性金鑰要求證明憑證時，指定無需明確使用者權限的網站和網域。此外，訊號傳送至安全性金鑰，代表可以使用個別證明。若沒有這麼做，每次網站請求安全性金鑰證明時都會提示使用者。

網站 (例如 https://contoso.com/some/path) 僅符合為 U2F appID。網域 (like contoso.com) 僅符合為 RP 識別碼。若要在指定網站涵蓋 U2F 和 webauthn API，您必須列出 appID URL 和網域。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  字串的清單

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: SecurityKeyPermitAttestation
  - GP 名稱: 不需要權限即可使用直接存取 [安全性金鑰] 證明的網站或網域
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge\SecurityKeyPermitAttestation
  - 路徑 (推薦項目): N/A
  - 值名稱: 1, 2, 3, ...
  - 數值類型: REG_SZ 的清單
  ##### 範例值:
```
SOFTWARE\Policies\Microsoft\Edge\SecurityKeyPermitAttestation\0 = "https://contoso.com"

```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: SecurityKeyPermitAttestation
  - 範例值:
``` xml
<array>
  <string>https://contoso.com</string>
</array>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### SendIntranetToInternetExplorer
  #### 將所有內部網路網站傳送到 Internet Explorer
  >支援的版本: Windows 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  如需設定 Internet Explorer 模式的最佳體驗教學，請參閱 [https://go.microsoft.com/fwlink/?linkid=2094210](https://go.microsoft.com/fwlink/?linkid=2094210)

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 否 - 需要重新啟動瀏覽器

  #### 資料類型:
  布林值

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: SendIntranetToInternetExplorer
  - GP 名稱: 將所有內部網路網站傳送到 Internet Explorer
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: SendIntranetToInternetExplorer
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000001
```


  

  [回到頂端](#microsoft-edge---原則)

  ### SendSiteInfoToImproveServices
  #### 傳送網站資訊來改善 Microsoft 服務
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  對於 Microsoft Edge Windows 10 Beta 與穩定版的通道來說，此原則設定時將會覆寫 Microsoft Edge 網站瀏覽資訊 ([https://go.microsoft.com/fwlink/?linkid=2099569](https://go.microsoft.com/fwlink/?linkid=2099569)) 集合或非集合的 Windows 診斷資料。

此原則設定可讓您決定使用者是否可以傳送與 Microsoft Edge 中造訪網站有關的資訊給 Microsoft 以改善搜尋等服務。

如果您啟用此原則，在 Microsoft Edge 中瀏覽過的網站資訊將傳送至 Microsoft。

如果您停用此原則，在 Microsoft Edge 中瀏覽過的網站資訊將不會傳送至 Microsoft。

在 Windows 10 Beta 版與穩定版的通道上，此原則可以控制傳送網站使用者的瀏覽資訊。如果此原則未設定，則 Microsoft Edge 將預設為 Windows 診斷資料設定。

在 Windows 10、Canary 與 Dev 通道中，此原則可以控制傳送網站使用者的瀏覽資訊。如果此原則未設定，則 Microsoft Edge 將預設為使用者的偏好設定。

在 Windows 7、8  和 Mac 上，此原則可以控制傳送網站使用者的瀏覽資訊。如果此原則未設定，Microsoft Edge 將預設為使用者的偏好設定。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 否 - 需要重新啟動瀏覽器

  #### 資料類型:
  布林值

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: SendSiteInfoToImproveServices
  - GP 名稱: 傳送網站資訊來改善 Microsoft 服務
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: SendSiteInfoToImproveServices
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000000
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: SendSiteInfoToImproveServices
  - 範例值:
``` xml
<false/>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### ShowOfficeShortcutInFavoritesBar
  #### 在 [我的最愛] 列中顯示 Microsoft Office 捷徑
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  指定是否在 [我的最愛] 列中包含 Office.com 的捷徑。使用者登入 Microsoft Edge 捷徑會將使用者帶到他們的 Microsoft Office 應用程式與文件。

如果啟用或未設定這個原則，使用者可以選擇是否要藉由變更操作功能表列將 [我的最愛] 中的切換，請參閱快顯。

如果已停用這個原則，將不會顯示捷徑。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  布林值

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: ShowOfficeShortcutInFavoritesBar
  - GP 名稱: 在 [我的最愛] 列中顯示 Microsoft Office 捷徑
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: ShowOfficeShortcutInFavoritesBar
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000000
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: ShowOfficeShortcutInFavoritesBar
  - 範例值:
``` xml
<false/>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### SignedHTTPExchangeEnabled
  #### 啟用簽署 HTTP Exchange (SXG) 支援
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (78 版或更新版本)

  #### 描述
  啟用 Signed HTTP Exchange (SXG) 的支援。

如果此原則未設定或未啟用，則 Microsoft Edge 將會接受網頁內容作為 Signed HTTP Exchange。

如果此原則設定為停用，則無法載入 Signed HTTP Exchanges。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  布林值

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: SignedHTTPExchangeEnabled
  - GP 名稱: 啟用簽署 HTTP Exchange (SXG) 支援
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: SignedHTTPExchangeEnabled
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000001
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: SignedHTTPExchangeEnabled
  - 範例值:
``` xml
<true/>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### SitePerProcess
  #### 在所有網站中啟用網站隔離
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  'SitePerProcess' 原則可防止使用者選擇超出隔離的所有網站的預設行為。請注意，您也可以使用 [IsolateOrigins](#isolateorigins) 原則隔離其他更細微的原始原則。
如果您啟用此原則，則使用者無法選擇退出每個網站在工作程序中運行的預設行為。
如果您停用或未設定此原則，使用者可以選擇退出網站隔離。(例如透過 edge://flags 中的 "Disable site isolation" 項目。) 停用或未設定此原則不會關閉網站隔離。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 否 - 需要重新啟動瀏覽器

  #### 資料類型:
  布林值

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: SitePerProcess
  - GP 名稱: 在所有網站中啟用網站隔離
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: SitePerProcess
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000001
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: SitePerProcess
  - 範例值:
``` xml
<true/>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### SpellcheckEnabled
  #### 啟用拼字檢查
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  如果您啟用或未設定此原則，使用者可以使用拼字檢查。

如果您停用此原則，使用者將無法使用拼字檢查，[SpellcheckLanguage](#spellchecklanguage) 和 [SpellcheckLanguageBlocklist](#spellchecklanguageblocklist) 原則也會停用。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  布林值

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: SpellcheckEnabled
  - GP 名稱: 啟用拼字檢查
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: SpellcheckEnabled
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000000
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: SpellcheckEnabled
  - 範例值:
``` xml
<false/>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### SpellcheckLanguage
  #### 啟用特定拼字檢查語言
  >支援的版本: Windows 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  啟用拼字檢查語言。無法辨識的語言，該清單中將會被忽略。

如果您啟用這個原則，拼字檢查將會停用指定的語言。使用者仍然可以啟用或停用的語言不在清單中的拼字檢查。

如果您未設定這個原則，或停用它，將不會變更使用者的拼字檢查喜好設定。

如果 [SpellcheckEnabled](#spellcheckenabled) 原則設定為停用，則此原則將不會有任何效果。

如果 'SpellcheckLanguage' 和 [SpellcheckLanguageBlocklist](#spellchecklanguageblocklist) 原則中包含了一種語言，會啟用拼字檢查語言。

目前支援的語言為: af、bg、ca、cs、cy、da、de、el、en-AU、en-CA、en-GB、en-US、es、es-419、es-AR、es-ES、es-MX、es-US、et、fa、fo、fr、he、hi、hr、hu、id、it、ko、lt、lv、nb、nl、pl、pt-BR、pt-PT、ro、ru、sh、sk、sl、sq、sr、sv、ta、tg、tr、uk、vi。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  字串的清單

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: SpellcheckLanguage
  - GP 名稱: 啟用特定拼字檢查語言
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge\SpellcheckLanguage
  - 路徑 (推薦項目): N/A
  - 值名稱: 1, 2, 3, ...
  - 數值類型: REG_SZ 的清單
  ##### 範例值:
```
SOFTWARE\Policies\Microsoft\Edge\SpellcheckLanguage\0 = "fr"
SOFTWARE\Policies\Microsoft\Edge\SpellcheckLanguage\1 = "es"

```


  

  [回到頂端](#microsoft-edge---原則)

  ### SpellcheckLanguageBlocklist
  #### 強制停用拼字檢查語言
  >支援的版本: Windows 上的 Microsoft Edge (78 版或更新版本)

  #### 描述
  強制-停用拼字檢查語言。無法辨識的語言，該清單中將會被忽略。

如果您啟用這個原則，拼字檢查將會停用指定的語言。使用者仍然可以啟用或停用的語言不在清單中的拼字檢查。

如果您未設定這個原則，或停用它，將不會變更使用者的拼字檢查喜好設定。

如果 [SpellcheckEnabled](#spellcheckenabled) 原則設定為 [停用]，則此原則將不會有任何效果。

如果 [SpellcheckLanguage](#spellchecklanguage) 和 'SpellcheckLanguageBlocklist' 原則中包含了一種語言，會啟用拼字檢查語言。

目前支援的語言為: af、bg、ca、cs、da、de、el、en-AU、en-CA、en-GB、en-US、es、es-419、es-AR、es-ES、es-MX、es-US、et、fa、fo、fr、he、hi、hr、hu、id、it、ko、lt、lv、nb、nl、pl、pt-BR、pt-PT、ro、ru、sh、sk、sl、sq、sr、sv、ta、tg、tr、uk、vi。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  字串的清單

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: SpellcheckLanguageBlocklist
  - GP 名稱: 強制停用拼字檢查語言
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge\SpellcheckLanguageBlocklist
  - 路徑 (推薦項目): N/A
  - 值名稱: 1, 2, 3, ...
  - 數值類型: REG_SZ 的清單
  ##### 範例值:
```
SOFTWARE\Policies\Microsoft\Edge\SpellcheckLanguageBlocklist\0 = "fr"
SOFTWARE\Policies\Microsoft\Edge\SpellcheckLanguageBlocklist\1 = "es"

```


  

  [回到頂端](#microsoft-edge---原則)

  ### SuppressUnsupportedOSWarning
  #### 隱藏不支援的 OS 警告
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  Suppresses the warning that appears when Microsoft Edge is running on a computer or operating system that is no longer supported.

If this policy is false or unset, the warnings will appear on such unsupported computers or operating systems.

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 否 - 需要重新啟動瀏覽器

  #### 資料類型:
  布林值

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: SuppressUnsupportedOSWarning
  - GP 名稱: 隱藏不支援的 OS 警告
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: SuppressUnsupportedOSWarning
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000001
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: SuppressUnsupportedOSWarning
  - 範例值:
``` xml
<true/>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### SyncDisabled
  #### 透過 Microsoft 同步服務停用資料同步處理
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  在 Microsoft Edge 中停用資料同步處理，並防止使用者修改此設定。

如果未設定此原則，則使用者將無法開啟或關閉同步處理。

 當原則 'RoamingProfileSupportEnabled' 已啟用時不要啟用此原則，因為 'RoamingProfileSupportEnabled' 會複製同步功能。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 是
  - 動態原則重新整理: 是

  #### 資料類型:
  布林值

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: SyncDisabled
  - GP 名稱: 透過 Microsoft 同步服務停用資料同步處理
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): 系統管理範本/Microsoft Edge - 預設設定 (使用者可以覆寫)/
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): SOFTWARE\Policies\Microsoft\Edge\推薦項目
  - 值名稱: SyncDisabled
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000001
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: SyncDisabled
  - 範例值:
``` xml
<true/>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### TabFreezingEnabled
  #### 允許凍結背景索引標籤
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (79 版或更新版本)

  #### 描述
  控制 Microsoft Edge 是否可以將背景的索引標籤凍結至少 5 分鐘。

索引標籤凍結可降低 CPU、電池和記憶體使用量。Microsoft Edge 使用啟發學習法，來避免凍結在背景進行運作的索引標籤，例如顯示通知、播放音效和串流影片。

如果啟用或未設定此原則，則位於背景至少 5 分鐘的索引標籤將會凍結。

如果停用此原則，則不會凍結任何索引標籤。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  布林值

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: TabFreezingEnabled
  - GP 名稱: 允許凍結背景索引標籤
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: TabFreezingEnabled
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000000
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: TabFreezingEnabled
  - 範例值:
``` xml
<false/>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### TaskManagerEndProcessEnabled
  #### 在瀏覽器工作管理員中啟用結束處理程序
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  如果啟用或不設定此原則，則使用者可以在 [瀏覽器工作管理員] 中結束處理程序。如果停用此原則，使用者將無法結束處理程序，且在 [瀏覽器工作管理員] 中將停用 [結束處理程序] 按鈕。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  布林值

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: TaskManagerEndProcessEnabled
  - GP 名稱: 在瀏覽器工作管理員中啟用結束處理程序
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: TaskManagerEndProcessEnabled
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000001
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: TaskManagerEndProcessEnabled
  - 範例值:
``` xml
<true/>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### TrackingPrevention
  #### 封鎖使用者的網頁瀏覽活動追蹤
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (78 版或更新版本)

  #### 描述
  讓您決定是否要封鎖追蹤使用者網頁瀏覽活動的網站。

  如果您啟用此原則，您有下列的防止追蹤層級選項可供選擇:

0 = 關閉 (沒有追蹤防止)
1 = 基本 (個人化區塊有害追蹤器、內容及廣告)
2 = 平衡 (未造訪區塊有害追蹤器和站台使用者從追蹤器; 內容與廣告將較不個人化)
3 = 嚴格 (區塊有害追蹤器和大部分的網站; 內容與廣告將極不個人化。網站的某些功能可能無法運作)

如果您停用此原則或未設定，使用者可以設定自己的防止追蹤層級。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  整數

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: TrackingPrevention
  - GP 名稱: 封鎖使用者的網頁瀏覽活動追蹤
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: TrackingPrevention
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000002
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: TrackingPrevention
  - 範例值:
``` xml
<integer>2</integer>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### TranslateEnabled
  #### 啟用翻譯
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  在 Microsoft Edge 上啟用整合式的 Microsoft 翻譯服務。

如果您啟用此原則， Microsoft Edge 會提供翻譯功能給使用者，並在恰當的時機顯示整合式翻譯飛出視窗，並在右鍵內容功能表中顯示翻譯選項。

停用此原則以停用所有內建翻譯功能。

如果您未設定此原則，使用者可以選擇是否要使用翻譯功能。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 是
  - 動態原則重新整理: 是

  #### 資料類型:
  布林值

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: TranslateEnabled
  - GP 名稱: 啟用翻譯
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): 系統管理範本/Microsoft Edge - 預設設定 (使用者可以覆寫)/
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): SOFTWARE\Policies\Microsoft\Edge\推薦項目
  - 值名稱: TranslateEnabled
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000001
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: TranslateEnabled
  - 範例值:
``` xml
<true/>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### URLAllowlist
  #### 定義受允許的 URL 清單
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  允許存取列出的 URL，以存取 URL 封鎖清單中的例外狀況。

根據 [https://go.microsoft.com/fwlink/?linkid=2095322](https://go.microsoft.com/fwlink/?linkid=2095322) 格式化 URL 模式。

您可以使用此原則以開啟嚴格封鎖清單的例外狀況。例如，您可以包含 [*] 封鎖所有要求，然後使用此原則以允許存取限制 Url 的封鎖清單。您可以使用此原則開啟某些配置、其他子網域、連線埠或特定路徑的例外狀況。

最適合的篩選器會決定 URL 是否封鎖或允許。允許的清單優先於封鎖清單。

此原則僅限於 1000 個項目; 後續的項目均將忽略。

如果您未設定此原則，則 [URLBlocklist](#urlblocklist) 原則的封鎖清單中沒有任何例外。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  字串的清單

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: URLAllowlist
  - GP 名稱: 定義受允許的 URL 清單
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge\URLAllowlist
  - 路徑 (推薦項目): N/A
  - 值名稱: 1, 2, 3, ...
  - 數值類型: REG_SZ 的清單
  ##### 範例值:
```
SOFTWARE\Policies\Microsoft\Edge\URLAllowlist\0 = "contoso.com"
SOFTWARE\Policies\Microsoft\Edge\URLAllowlist\1 = "https://ssl.server.com"
SOFTWARE\Policies\Microsoft\Edge\URLAllowlist\2 = "hosting.com/good_path"
SOFTWARE\Policies\Microsoft\Edge\URLAllowlist\3 = "https://server:8080/path"
SOFTWARE\Policies\Microsoft\Edge\URLAllowlist\4 = ".exact.hostname.com"

```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: URLAllowlist
  - 範例值:
``` xml
<array>
  <string>contoso.com</string>
  <string>https://ssl.server.com</string>
  <string>hosting.com/good_path</string>
  <string>https://server:8080/path</string>
  <string>.exact.hostname.com</string>
</array>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### URLBlocklist
  #### 封鎖存取 URL 清單
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  根據 URL 模式定義遭封鎖的網站清單 (您的使用者無法載入這些網站)。

格式化 URL 模式將根據 [https://go.microsoft.com/fwlink/?linkid=2095322](https://go.microsoft.com/fwlink/?linkid=2095322)。

您可以在 [URLAllowlist](#urlallowlist) 原則中定義例外狀況。這些原則僅限於 1000 個項目; 將忽略後續項目。

請注意，不建議封鎖內部 [edge://*] URL - 這可能會導致未預期的錯誤。

此原則不會阻止頁面 JavaScript 透過動態更新。假設您封鎖 'contoso.com/abc'，只要不重新整理此頁面，使用者可能仍能瀏覽 'contoso.com'，然後按一下連結前往 'contoso.com/abc'。

如果您未設定此原則，則不會封鎖任何 URL。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  字串的清單

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: URLBlocklist
  - GP 名稱: 封鎖存取 URL 清單
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge\URLBlocklist
  - 路徑 (推薦項目): N/A
  - 值名稱: 1, 2, 3, ...
  - 數值類型: REG_SZ 的清單
  ##### 範例值:
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


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: URLBlocklist
  - 範例值:
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
  

  [回到頂端](#microsoft-edge---原則)

  ### UserDataDir
  #### 設定使用者資料目錄
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  設定用來儲存使用者資料的目錄。

如果您啟用此原則，無論使用者的設定是否會使用 [--user-data-dir] 命令列旗標，Microsoft Edge 會使用指定目錄。

如果您未啟用此原則，會使用預設的設定檔路徑，但使用者可以透過 [--user-data-dir] 旗標覆寫。使用者可以在 edge://version/ 的設定檔路徑下尋找設定檔目錄。

若要避免資料遺失或其他錯誤，請不要設定此原則的磁碟區根目錄或用於其他用途，因為 Microsoft Edge 會管理其內容。

請參閱 [https://go.microsoft.com/fwlink/?linkid=2095041](https://go.microsoft.com/fwlink/?linkid=2095041) 的可用變數清單。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 否 - 需要重新啟動瀏覽器

  #### 資料類型:
  字串

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: UserDataDir
  - GP 名稱: 設定使用者資料目錄
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: UserDataDir
  - 數值類型: REG_SZ
  ##### 範例值:
```
"${users}/${user_name}/Edge"
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: UserDataDir
  - 範例值:
``` xml
<string>${users}/${user_name}/Edge</string>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### UserFeedbackAllowed
  #### 允許使用者意見反應
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  Microsoft Edge 使用 Edge Feedback 功能 (依預設啟用) 允許使用者傳送意見反應、建議或客戶調查，回報任何瀏覽器的問題。此外，根據預設，使用者無法停用 (關閉) Edge Feedback 功能。

如果您啟用此原則或未設定，使用者可以叫用 Edge Feedback。

如果您停用此原則，則使用者無法叫用 Edge Feedback。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 否 - 需要重新啟動瀏覽器

  #### 資料類型:
  布林值

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: UserFeedbackAllowed
  - GP 名稱: 允許使用者意見反應
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: UserFeedbackAllowed
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000001
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: UserFeedbackAllowed
  - 範例值:
``` xml
<true/>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### VideoCaptureAllowed
  #### 允許或封鎖視訊擷取
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  控制網站是否可以擷取視訊。

如果已啟用或未設定 (預設)，會向使用者要求所有網站的視訊擷取存取權限，除了那些 URL 設定在 [VideoCaptureAllowedUrls](#videocaptureallowedurls) 原則清單中的網站。這些網站無須提示便可獲得存取權限。

如果您停用此原則，使用者將不會收到提示，影片擷取功能僅可用於設定在 [VideoCaptureAllowedUrls](#videocaptureallowedurls) 原則中的 URL。

此原則會影響所有類型的視訊輸入，不僅限於內建攝影機。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  布林值

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: VideoCaptureAllowed
  - GP 名稱: 允許或封鎖視訊擷取
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: VideoCaptureAllowed
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000000
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: VideoCaptureAllowed
  - 範例值:
``` xml
<false/>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### VideoCaptureAllowedUrls
  #### 無需請求權限即可存取視訊擷取裝置的網站
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  根據 URL 模式指定可使用視訊擷取裝置的網站，而無需向使用者要求權限。此清單中的模式與要求 URL 的安全性來源相符。如果相符，則會自動授與該網站存取視訊擷取裝置的權限。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  字串的清單

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: VideoCaptureAllowedUrls
  - GP 名稱: 無需請求權限即可存取視訊擷取裝置的網站
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge\VideoCaptureAllowedUrls
  - 路徑 (推薦項目): N/A
  - 值名稱: 1, 2, 3, ...
  - 數值類型: REG_SZ 的清單
  ##### 範例值:
```
SOFTWARE\Policies\Microsoft\Edge\VideoCaptureAllowedUrls\0 = "https://www.contoso.com/"
SOFTWARE\Policies\Microsoft\Edge\VideoCaptureAllowedUrls\1 = "https://[*.]contoso.edu/"

```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: VideoCaptureAllowedUrls
  - 範例值:
``` xml
<array>
  <string>https://www.contoso.com/</string>
  <string>https://[*.]contoso.edu/</string>
</array>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### WPADQuickCheckEnabled
  #### 設定 WPAD 最佳化
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  允許您關閉 Microsoft Edge 中的 WPAD (Web Proxy 自動探索) 最佳化。

如果您停用此原則，WPAD 最佳化將會停用，並會讓瀏覽器等候 DNS 性 WPAD 伺服器的時間更久。

如果您啟用或未設定此原則，則會啟用 WPAD 最佳化。

無論是否已啟用此原則，使用者均無法變更 WPAD 最佳化設定。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 否 - 需要重新啟動瀏覽器

  #### 資料類型:
  布林值

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: WPADQuickCheckEnabled
  - GP 名稱: 設定 WPAD 最佳化
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: WPADQuickCheckEnabled
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000001
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: WPADQuickCheckEnabled
  - 範例值:
``` xml
<true/>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### WebAppInstallForceList
  #### 設定強制安裝 Web 應用程式的清單
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (80 版或更新版本)

  #### 描述
  指定無需使用者互動、以無訊息模式安裝，且不可由使用者解除安裝或停用的網站清單。

原則的每個清單項目都具有包含下列成員的物件:
具有強制性的「url」。「url」應為網頁應用程式要安裝的 URL。

「launch_container」應為「視窗」或「分頁」，以表明網頁應用程式安裝後的開啟方式。
  -如果應在 Windows 上建立桌面捷徑，則「create_desktop_shortcut」應為 True。

如果「default_launch_container」已省略，則此應用程式預設會在分頁中開啟。不論「default_launch_container」的值為何，使用者都能變更應用程式的開啟容器。如果「create_desktop_shortcuts」已省略，則不會建立任何桌面捷徑。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 是

  #### 資料類型:
  字典

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: WebAppInstallForceList
  - GP 名稱: 設定強制安裝 Web 應用程式的清單
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: WebAppInstallForceList
  - 數值類型: REG_SZ
  ##### 範例值:
```
SOFTWARE\Policies\Microsoft\Edge\WebAppInstallForceList = [
  {
    "create_desktop_shortcut": true, 
    "default_launch_container": "window", 
    "url": "https://www.contoso.com/maps"
  }, 
  {
    "default_launch_container": "tab", 
    "url": "https://app.contoso.edu"
  }
]
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: WebAppInstallForceList
  - 範例值:
``` xml
<key>WebAppInstallForceList</key>
<array>
  <dict>
    <key>create_desktop_shortcut</key>
    <true/>
    <key>default_launch_container</key>
    <string>window</string>
    <key>url</key>
    <string>https://www.contoso.com/maps</string>
  </dict>
  <dict>
    <key>default_launch_container</key>
    <string>tab</string>
    <key>url</key>
    <string>https://app.contoso.edu</string>
  </dict>
</array>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### WebDriverOverridesIncompatiblePolicies
  #### 允許 WebDriver 覆寫不相容原則
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  由於 WebDriver 現與所有現有的原則相容，此原則不再必要，
因此已在 M80 中刪除此原則。

此原則允許 WebDriver 功能的使用者覆寫
可能干擾其作業的原則。

目前此原則停用 [SitePerProcess](#siteperprocess) 和 [IsolateOrigins](#isolateorigins) 原則。

如果啟用該原則，則 WebDriver 將能覆寫不相容的
原則。
如果停用或未設定該原則，則不允許 WebDriver
覆寫不相容的原則。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 否 - 需要重新啟動瀏覽器

  #### 資料類型:
  布林值

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: WebDriverOverridesIncompatiblePolicies
  - GP 名稱: 允許 WebDriver 覆寫不相容原則
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: WebDriverOverridesIncompatiblePolicies
  - 數值類型: REG_DWORD
  ##### 範例值:
```
0x00000001
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: WebDriverOverridesIncompatiblePolicies
  - 範例值:
``` xml
<true/>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### WebRtcLocalIpsAllowedUrls
  #### Manage exposure of local IP addressess by WebRTC
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (80 版或更新版本)

  #### 描述
  Specifies a list of origins (URLs) or hostname patterns (like "*contoso.com*") for which local IP address should be exposed by WebRTC.

If you enable this policy and set a list of origins (URLs) or hostname patterns, when edge://flags/#enable-webrtc-hide-local-ips-with-mdns is Enabled, WebRTC will expose the local IP address for cases that match patterns in the list.

If you disable or don't configure this policy, and edge://flags/#enable-webrtc-hide-local-ips-with-mdns is Enabled, WebRTC will not expose local IP addresses. The local IP address is concealed with an mDNS hostname.

If you enable, disable, or don't configure this policy, and edge://flags/#enable-webrtc-hide-local-ips-with-mdns is Disabled, WebRTC will expose local IP addresses.

Please note that this policy weakens the protection of local IP addresses that might be needed by administrators.

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 否 - 需要重新啟動瀏覽器

  #### 資料類型:
  字串的清單

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: WebRtcLocalIpsAllowedUrls
  - GP 名稱: Manage exposure of local IP addressess by WebRTC
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge\WebRtcLocalIpsAllowedUrls
  - 路徑 (推薦項目): N/A
  - 值名稱: 1, 2, 3, ...
  - 數值類型: REG_SZ 的清單
  ##### 範例值:
```
SOFTWARE\Policies\Microsoft\Edge\WebRtcLocalIpsAllowedUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\WebRtcLocalIpsAllowedUrls\1 = "*contoso.com*"

```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: WebRtcLocalIpsAllowedUrls
  - 範例值:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>*contoso.com*</string>
</array>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### WebRtcLocalhostIpHandling
  #### Restrict exposure of local IP address by WebRTC
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  Allows you to set whether or not WebRTC exposes the user's local IP address.

If you set this policy to "AllowAllInterfaces" ('default') or "AllowPublicAndPrivateInterfaces" ('default_public_and_private_interfaces'), WebRTC exposes the local IP address.

If you set this policy to "AllowPublicInterfaceOnly" ('default_public_interface_only') or "DisableNonProxiedUdp" ('disable_non_proxied_udp'), WebRTC doesn't expose the local IP address.

If you don't set this policy, or if you disable it, WebRTC exposes the local IP address.

  * 'default' = Allow all interfaces. This exposes the local IP address.
  * 'default_public_and_private_interfaces' = Allow public and private interfaces over http default route. This exposes the local IP address.
  * 'default_public_interface_only' = Allow public interface over http default route. This doesn't expose the local IP address.
  * 'disable_non_proxied_udp' = Use TCP unless proxy server supports UDP. This doesn't expose the local IP address.

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 否 - 需要重新啟動瀏覽器

  #### 資料類型:
  字串

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: WebRtcLocalhostIpHandling
  - GP 名稱: Restrict exposure of local IP address by WebRTC
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: WebRtcLocalhostIpHandling
  - 數值類型: REG_SZ
  ##### 範例值:
```
"default"
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: WebRtcLocalhostIpHandling
  - 範例值:
``` xml
<string>default</string>
```
  

  [回到頂端](#microsoft-edge---原則)

  ### WebRtcUdpPortRange
  #### 限制 WebRTC 所使用的本機 UDP 連接埠範圍
  >支援的版本: Windows 與 Mac 上的 Microsoft Edge (77 版或更新版本)

  #### 描述
  將 WebRTC 使用的 UDP 連接埠範圍限制為指定連接埠間隔 (包含端點)。

透過此原則設定，您可以指定本機 WebRTC 可使用的 UDP 連接埠範圍。

如果您未設定此原則，或將其設定為空字串或無效連接埠範圍，則 WebRTC 可使用所有可用的本機 UDP 連接埠。

  #### 支援功能:
  - 可以是強制: 是
  - 可以建議: 否
  - 動態原則重新整理: 否 - 需要重新啟動瀏覽器

  #### 資料類型:
  字串

  #### Windows 資訊和設定
  ##### 群組原則 (ADMX) 資訊
  - GP 唯一名稱: WebRtcUdpPortRange
  - GP 名稱: 限制 WebRTC 所使用的本機 UDP 連接埠範圍
  - GP 路徑 (強制): 系統管理範本/Microsoft Edge/
  - GP 路徑 (推薦項目): N/A
  - GP ADMX 檔案名稱: MSEdge.admx
  ##### Windows 登錄設定
  - 路徑 (強制): SOFTWARE\Policies\Microsoft\Edge
  - 路徑 (推薦項目): N/A
  - 值名稱: WebRtcUdpPortRange
  - 數值類型: REG_SZ
  ##### 範例值:
```
"10000-11999"
```


  #### Mac 資訊和設定
  - 喜好設定金鑰名稱: WebRtcUdpPortRange
  - 範例值:
``` xml
<string>10000-11999</string>
```
  

  [回到頂端](#microsoft-edge---原則)


## 也可參閱
- [正在設定 Microsoft Edge](configure-microsoft-edge.md)
- [Microsoft Edge 企業版登陸頁面](https://aka.ms/EdgeEnterprise)