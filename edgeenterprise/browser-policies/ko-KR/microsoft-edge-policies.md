---
title: "Microsoft Edge Browser Policy Documentation"
ms.author: stmoody
author: brianalt-msft
manager: tahills
ms.date: 11/07/2019
audience: ITPro
ms.topic: reference
ms.prod: microsoft-edge
ms.localizationpriority: medium
ms.collection: M365-modern-desktop
ms.custom:
description: "Windows and Mac documentation for all policies supported by the Microsoft Edge Browser"
---

# Microsoft Edge - 정책
최신 버전의 Microsoft Edge에는 다음 정책이 포함되어 있습니다. 이러한 정책을 사용하여 조직에서 Microsoft Edge가 실행되는 방식을 구성할 수 있습니다.

Microsoft Edge 업데이트 방법 및 시기를 제어하는 데 사용되는 추가 정책에 대한 자세한 내용은 [Microsoft Edge 업데이트 정책 참조](microsoft-edge-update-policies.md)을(를) 확인하세요.

> [!참고]
> 이 문서는 Microsoft Edge 버전 77 이상에 적용됩니다.

## 사용 가능한 정책
이 표에서는 이 Microsoft Edge 릴리스에서 사용 가능한 모든 브라우저 관련 그룹 정책을 나열합니다. 특정 정책에 대한 자세한 내용을 보려면 표의 링크를 사용하세요.

|||
|-|-|
|[Cast](#cast)|[HTTP 인증](#http-인증)|
|[SmartScreen 설정](#smartscreen-설정)|[기본 검색 공급자](#기본-검색-공급자)|
|[기본 메시지](#기본-메시지)|[시작, 홈 페이지 및 새 탭 페이지](#시작,-홈-페이지-및-새-탭-페이지)|
|[암호 관리자 및 보호](#암호-관리자-및-보호)|[인쇄 중](#인쇄-중)|
|[콘텐츠 설정](#콘텐츠-설정)|[프록시 서버](#프록시-서버)|
|[확장](#확장)|[Additional](#additional)|


### [*Cast*](#cast-policies)
|정책 이름|설명|
|-|-|
|[EnableMediaRouter](#enablemediarouter)|Google Cast 사용|
|[ShowCastIconInToolbar](#showcasticonintoolbar)|도구 모음에서 캐스트 아이콘 표시|
### [*HTTP 인증*](#http-인증-policies)
|정책 이름|설명|
|-|-|
|[AllowCrossOriginAuthPrompt](#allowcrossoriginauthprompt)|원본 간 HTTP 기본 인증 메시지 표시 허용|
|[AuthNegotiateDelegateAllowlist](#authnegotiatedelegateallowlist)|Microsoft Edge가 사용자 자격 증명을 위임할 수 있는 서버 목록을 지정합니다.|
|[AuthSchemes](#authschemes)|지원되는 인증 방식|
|[AuthServerAllowlist](#authserverallowlist)|허용된 인증 서버의 목록 구성|
|[DisableAuthNegotiateCnameLookup](#disableauthnegotiatecnamelookup)|Kerberos 인증을 협상할 때 CNAME 조회 사용 안 함|
|[EnableAuthNegotiatePort](#enableauthnegotiateport)|Kerberos SPN에 비표준 포트 포함|
|[NtlmV2Enabled](#ntlmv2enabled)|NTLMv2 인증을 사용할지 여부 제어|
### [*SmartScreen 설정*](#smartscreen-설정-policies)
|정책 이름|설명|
|-|-|
|[PreventSmartScreenPromptOverride](#preventsmartscreenpromptoverride)|사이트에 대한 Microsoft Defender SmartScreen 프롬프트 무시 허용 안 함|
|[PreventSmartScreenPromptOverrideForFiles](#preventsmartscreenpromptoverrideforfiles)|다운로드에 대한 Microsoft Defender SmartScreen 경고 무시 허용 안 함|
|[SmartScreenAllowListDomains](#smartscreenallowlistdomains)|Microsoft Defender SmartScreen이 경고를 트리거하지 않는 도메인 목록 구성|
|[SmartScreenEnabled](#smartscreenenabled)|Microsoft Defender SmartScreen 구성|
|[SmartScreenForTrustedDownloadsEnabled](#smartscreenfortrusteddownloadsenabled)|신뢰할 수 있는 원본의 다운로드에 대한 Microsoft Defender SmartScreen 검사 강제 적용|
|[SmartScreenPuaEnabled](#smartscreenpuaenabled)|Configure Microsoft Defender SmartScreen to block potentially unwanted apps|
### [*기본 검색 공급자*](#기본-검색-공급자-policies)
|정책 이름|설명|
|-|-|
|[DefaultSearchProviderEnabled](#defaultsearchproviderenabled)|기본 검색 공급자 사용|
|[DefaultSearchProviderEncodings](#defaultsearchproviderencodings)|기본 검색 공급자 인코딩|
|[DefaultSearchProviderImageURL](#defaultsearchproviderimageurl)|기본 검색 공급자에 대한 이미지로 검색하기 기능을 지정합니다.|
|[DefaultSearchProviderImageURLPostParams](#defaultsearchproviderimageurlpostparams)|POST를 사용하는 이미지 URL에 대한 매개 변수|
|[DefaultSearchProviderKeyword](#defaultsearchproviderkeyword)|기본 검색 공급자 키워드|
|[DefaultSearchProviderName](#defaultsearchprovidername)|기본 검색 공급자 이름|
|[DefaultSearchProviderSearchURL](#defaultsearchprovidersearchurl)|기본 검색 공급자 검색 URL|
|[DefaultSearchProviderSuggestURL](#defaultsearchprovidersuggesturl)|제안에 대한 기본 검색 공급자 URL|
### [*기본 메시지*](#기본-메시지-policies)
|정책 이름|설명|
|-|-|
|[NativeMessagingAllowlist](#nativemessagingallowlist)|사용자가 사용할 수 있는 기본 메시징 호스트 제어|
|[NativeMessagingBlocklist](#nativemessagingblocklist)|기본 메시지 차단 목록 구성|
|[NativeMessagingUserLevelHosts](#nativemessaginguserlevelhosts)|사용자 수준 기본 메시징 호스트 허용(관리자 권한 없이 설치됨)|
### [*시작&comma; 홈 페이지 및 새 탭 페이지*](#시작-홈-페이지-및-새-탭-페이지-policies)
|정책 이름|설명|
|-|-|
|[HomepageIsNewTabPage](#homepageisnewtabpage)|새 탭 페이지를 홈 페이지로 설정|
|[HomepageLocation](#homepagelocation)|홈 페이지 URL 구성|
|[NewTabPageCompanyLogo](#newtabpagecompanylogo)|새 탭 페이지 회사 로고 설정|
|[NewTabPageHideDefaultTopSites](#newtabpagehidedefaulttopsites)|새 탭 페이지에서 기본 상위 사이트 숨기기|
|[NewTabPageLocation](#newtabpagelocation)|새 탭 페이지 URL 구성|
|[NewTabPageManagedQuickLinks](#newtabpagemanagedquicklinks)|새 탭 페이지 빠른 연결 설정|
|[NewTabPageSetFeedType](#newtabpagesetfeedtype)|Configure the Microsoft Edge new tab page experience|
|[RestoreOnStartup](#restoreonstartup)|시작 시 수행할 작업|
|[RestoreOnStartupURLs](#restoreonstartupurls)|브라우저가 시작될 때 열 사이트|
|[ShowHomeButton](#showhomebutton)|도구 모음에 홈 버튼 표시|
### [*암호 관리자 및 보호*](#암호-관리자-및-보호-policies)
|정책 이름|설명|
|-|-|
|[PasswordManagerEnabled](#passwordmanagerenabled)|암호 관리자에 암호 저장 사용|
|[PasswordProtectionChangePasswordURL](#passwordprotectionchangepasswordurl)|암호 변경 URL 구성|
|[PasswordProtectionLoginURLs](#passwordprotectionloginurls)|암호 보호 서비스가 암호의 지문을 캡처해야 하는 엔터프라이즈 로그인 URL 목록 구성|
|[PasswordProtectionWarningTrigger](#passwordprotectionwarningtrigger)|암호 보호 경고 트리거 구성|
### [*인쇄 중*](#인쇄-중-policies)
|정책 이름|설명|
|-|-|
|[DefaultPrinterSelection](#defaultprinterselection)|기본 프린터 선택 규칙|
|[PrintHeaderFooter](#printheaderfooter)|머리글 및 바닥글 인쇄|
|[PrintPreviewUseSystemDefaultPrinter](#printpreviewusesystemdefaultprinter)|시스템 기본 프린터를 기본 프린터로 설정|
|[PrintingEnabled](#printingenabled)|인쇄 사용|
|[UseSystemPrintDialog](#usesystemprintdialog)|시스템 대화 상자를 사용하여 인쇄|
### [*콘텐츠 설정*](#콘텐츠-설정-policies)
|정책 이름|설명|
|-|-|
|[AutoSelectCertificateForUrls](#autoselectcertificateforurls)|이 사이트에 대한 클라이언트 인증서 자동 선택|
|[CookiesAllowedForUrls](#cookiesallowedforurls)|특정 사이트에서 쿠키 허용|
|[CookiesBlockedForUrls](#cookiesblockedforurls)|특정 사이트에서 쿠키 차단|
|[CookiesSessionOnlyForUrls](#cookiessessiononlyforurls)|특정 웹 사이트의 쿠키를 현재 세션으로 제한|
|[DefaultCookiesSetting](#defaultcookiessetting)|쿠키 구성|
|[DefaultGeolocationSetting](#defaultgeolocationsetting)|기본 지리적 위치 설정|
|[DefaultImagesSetting](#defaultimagessetting)|기본 이미지 설정|
|[DefaultJavaScriptSetting](#defaultjavascriptsetting)|기본 JavaScript 설정|
|[DefaultNotificationsSetting](#defaultnotificationssetting)|기본 알림 설정|
|[DefaultPluginsSetting](#defaultpluginssetting)|기본 Adobe Flash 설정|
|[DefaultPopupsSetting](#defaultpopupssetting)|기본 팝업 창 설정|
|[DefaultWebBluetoothGuardSetting](#defaultwebbluetoothguardsetting)|Bluetooth 웹 API의 사용 제어|
|[DefaultWebUsbGuardSetting](#defaultwebusbguardsetting)|WebUSB API의 사용 제어|
|[ImagesAllowedForUrls](#imagesallowedforurls)|이 사이트의 이미지 허용|
|[ImagesBlockedForUrls](#imagesblockedforurls)|특정 사이트에서 이미지 차단|
|[JavaScriptAllowedForUrls](#javascriptallowedforurls)|특정 사이트에서 JavaScript 허용|
|[JavaScriptBlockedForUrls](#javascriptblockedforurls)|특정 사이트에서 JavaScript 차단|
|[NotificationsAllowedForUrls](#notificationsallowedforurls)|특정 사이트에서 알림 허용|
|[NotificationsBlockedForUrls](#notificationsblockedforurls)|특정 사이트에서 알림 차단|
|[PluginsAllowedForUrls](#pluginsallowedforurls)|특정 사이트에서 Adobe Flash 플러그 인 허용|
|[PluginsBlockedForUrls](#pluginsblockedforurls)|특정 사이트에서 Adobe Flash 플러그 인 차단|
|[PopupsAllowedForUrls](#popupsallowedforurls)|특정 사이트에서 팝업 창 허용|
|[PopupsBlockedForUrls](#popupsblockedforurls)|특정 사이트에서 팝업 창 차단|
|[RegisteredProtocolHandlers](#registeredprotocolhandlers)|프로토콜 처리기 등록|
|[WebUsbAllowDevicesForUrls](#webusballowdevicesforurls)|특정 USB 장치에 연결하기 위해 특정 사이트에 대한 액세스 권한 부여|
|[WebUsbAskForUrls](#webusbaskforurls)|특정 사이트에서 WebUSB 허용|
|[WebUsbBlockedForUrls](#webusbblockedforurls)|특정 사이트에서 WebUSB 차단|
### [*프록시 서버*](#프록시-서버-policies)
|정책 이름|설명|
|-|-|
|[ProxyBypassList](#proxybypasslist)|프록시 바이패스 규칙 구성|
|[ProxyMode](#proxymode)|프록시 서버 설정 구성|
|[ProxyPacUrl](#proxypacurl)|프록시.pac 파일 URL 설정|
|[ProxyServer](#proxyserver)|프록시 서버의 주소 또는 URL 구성|
|[ProxySettings](#proxysettings)|프록시 설정|
### [*확장*](#확장-policies)
|정책 이름|설명|
|-|-|
|[ExtensionAllowedTypes](#extensionallowedtypes)|허용된 확장 유형 구성|
|[ExtensionInstallAllowlist](#extensioninstallallowlist)|특정 확장 설치 허용|
|[ExtensionInstallBlocklist](#extensioninstallblocklist)|설치될 수 없는 확장 제어|
|[ExtensionInstallForcelist](#extensioninstallforcelist)|자동으로 설치되는 확장 제어|
|[ExtensionInstallSources](#extensioninstallsources)|확장 및 사용자 스크립트 설치 원본 구성|
|[ExtensionSettings](#extensionsettings)|확장 관리 설정 구성|
### [*Additional*](#additional-policies)
|정책 이름|설명|
|-|-|
|[AdsSettingForIntrusiveAdsSites](#adssettingforintrusiveadssites)|침입적인 광고가 있는 사이트에 대한 광고 설정|
|[AllowDeletingBrowserHistory](#allowdeletingbrowserhistory)|브라우저 및 다운로드 기록 삭제 사용|
|[AllowFileSelectionDialogs](#allowfileselectiondialogs)|파일 선택 대화 상자 허용|
|[AllowPopupsDuringPageUnload](#allowpopupsduringpageunload)|언로드하는 동안 페이지에서 팝업을 표시하도록 허용|
|[AllowSyncXHRInPageDismissal](#allowsyncxhrinpagedismissal)|페이지 해제 중에 페이지에서 동기 XHR 요청을 보내도록 허용|
|[AllowTrackingForUrls](#allowtrackingforurls)|특정 사이트에 대한 추적 방지 예외 구성|
|[AlwaysOpenPdfExternally](#alwaysopenpdfexternally)|항상 외부에서 PDF 파일 열기|
|[ApplicationLocaleValue](#applicationlocalevalue)|응용 프로그램 로캘 설정|
|[AudioCaptureAllowed](#audiocaptureallowed)|오디오 캡처 허용 또는 차단|
|[AudioCaptureAllowedUrls](#audiocaptureallowedurls)|사용 권한을 요청하지 않고 오디오 캡처 장치에 액세스할 수 있는 사이트|
|[AutoImportAtFirstRun](#autoimportatfirstrun)|처음 실행 시 다른 브라우저의 데이터 및 설정 자동으로 가져오기|
|[AutofillAddressEnabled](#autofilladdressenabled)|주소 정보 자동 채우기 사용|
|[AutofillCreditCardEnabled](#autofillcreditcardenabled)|신용 카드 정보 자동 채우기 사용|
|[AutoplayAllowed](#autoplayallowed)|웹 사이트에 미디어 자동 재생 허용|
|[BackgroundModeEnabled](#backgroundmodeenabled)|Microsoft Edge가 닫힌 후 백그라운드 앱 계속 실행|
|[BackgroundTemplateListUpdatesEnabled](#backgroundtemplatelistupdatesenabled)|컬렉션 및 템플릿을 사용하는 기타 기능의 사용 가능한 템플릿 목록에 대한 백그라운드 업데이트를 사용하도록 설정합니다.|
|[BlockThirdPartyCookies](#blockthirdpartycookies)|타사 쿠키 차단|
|[BrowserAddProfileEnabled](#browseraddprofileenabled)|ID 플라이아웃 메뉴 또는 설정 페이지에서 프로필 만들기 사용|
|[BrowserGuestModeEnabled](#browserguestmodeenabled)|게스트 모드 사용|
|[BrowserNetworkTimeQueriesEnabled](#browsernetworktimequeriesenabled)|브라우저 네트워크 시간 서비스에 대한 쿼리 허용|
|[BrowserSignin](#browsersignin)|브라우저 로그인 설정|
|[BuiltInDnsClientEnabled](#builtindnsclientenabled)|기본 제공 DNS 클라이언트 사용|
|[CertificateTransparencyEnforcementDisabledForCas](#certificatetransparencyenforcementdisabledforcas)|subjectPublicKeyInfo 해시 목록에 대한 인증서 투명성 적용 사용 안 함|
|[CertificateTransparencyEnforcementDisabledForLegacyCas](#certificatetransparencyenforcementdisabledforlegacycas)|레거시 인증 기관 목록에 대 한 인증서 투명도 적용 사용 안 함|
|[CertificateTransparencyEnforcementDisabledForUrls](#certificatetransparencyenforcementdisabledforurls)|특정 URL에 대한 인증서 투명성 적용 사용 안 함|
|[ClearBrowsingDataOnExit](#clearbrowsingdataonexit)|Microsoft Edge가 닫힐 때 검색 데이터 지우기|
|[ClickOnceEnabled](#clickonceenabled)|사용자가 ClickOnce 프로토콜을 사용하여 파일을 열 수 있도록 허용|
|[CommandLineFlagSecurityWarningsEnabled](#commandlineflagsecuritywarningsenabled)|명령줄 플래그에 대한 보안 경고 사용|
|[ComponentUpdatesEnabled](#componentupdatesenabled)|Microsoft Edge에서 구성 요소 업데이트 사용|
|[ConfigureDoNotTrack](#configuredonottrack)|추적 안 함 구성|
|[ConfigureOnlineTextToSpeech](#configureonlinetexttospeech)|온라인 텍스트 음성 변환 구성|
|[CustomHelpLink](#customhelplink)|사용자 지정 도움말 링크 지정|
|[DefaultBrowserSettingEnabled](#defaultbrowsersettingenabled)|Microsoft Edge를 기본 브라우저로 설정|
|[DeveloperToolsAvailability](#developertoolsavailability)|개발자 도구를 사용할 수 있는 위치 제어|
|[DirectInvokeEnabled](#directinvokeenabled)|사용자가 DirectInvoke 프로토콜을 사용하여 파일을 열 수 있도록 허용|
|[Disable3DAPIs](#disable3dapis)|3D 그래픽 API에 대한 지원 사용 안 함|
|[DisableScreenshots](#disablescreenshots)|스크린샷 찍기 사용 안 함|
|[DiskCacheDir](#diskcachedir)|디스크 캐시 디렉터리 설정|
|[DiskCacheSize](#diskcachesize)|디스크 캐시 크기를 바이트 단위로 설정|
|[DownloadDirectory](#downloaddirectory)|다운로드 디렉터리 설정|
|[DownloadRestrictions](#downloadrestrictions)|다운로드 제한 허용|
|[EdgeCollectionsEnabled](#edgecollectionsenabled)|컬렉션 기능 사용|
|[EditFavoritesEnabled](#editfavoritesenabled)|사용자가 즐겨찾기를 편집할 수 있도록 허용|
|[EnableDeprecatedWebPlatformFeatures](#enabledeprecatedwebplatformfeatures)|제한된 기간 동안 사용되지 않은 웹 플랫폼 기능 다시 사용|
|[EnableDomainActionsDownload](#enabledomainactionsdownload)|Microsoft에서 도메인 작업 다운로드 사용|
|[EnableOnlineRevocationChecks](#enableonlinerevocationchecks)|온라인 OCSP/CRL 검사 사용|
|[EnterpriseHardwarePlatformAPIEnabled](#enterprisehardwareplatformapienabled)|관리되는 확장에서 엔터프라이즈 하드웨어 플랫폼 API를 사용하도록 허용|
|[ExperimentationAndConfigurationServiceControl](#experimentationandconfigurationservicecontrol)|실험 및 구성 서비스와의 통신 제어|
|[ExternalProtocolDialogShowAlwaysOpenCheckbox](#externalprotocoldialogshowalwaysopencheckbox)|Show an "Always open" checkbox in external protocol dialog.|
|[FavoritesBarEnabled](#favoritesbarenabled)|즐겨찾기 모음 사용|
|[ForceBingSafeSearch](#forcebingsafesearch)|Bing 유해 정보 차단 적용|
|[ForceEphemeralProfiles](#forceephemeralprofiles)|임시 프로필 사용 설정|
|[ForceGoogleSafeSearch](#forcegooglesafesearch)|Google 유해 정보 차단 적용|
|[ForceNetworkInProcess](#forcenetworkinprocess)|네트워킹 코드가 브라우저 프로세스에서 실행되도록 강제|
|[ForceYouTubeRestrict](#forceyoutuberestrict)|최소 YouTube 제한 모드 강제 적용|
|[FullscreenAllowed](#fullscreenallowed)|전체 화면 모드 허용|
|[GoToIntranetSiteForSingleWordEntryInAddressBar](#gotointranetsiteforsinglewordentryinaddressbar)|주소 표시줄에서 단일 단어 항목을 검색하는 대신 직접 인트라넷 사이트 탐색을 강제합니다.|
|[HSTSPolicyBypassList](#hstspolicybypasslist)|HSTS 정책 확인을 무시할 이름 목록 구성|
|[HardwareAccelerationModeEnabled](#hardwareaccelerationmodeenabled)|가능한 경우 하드웨어 가속 사용|
|[ImportAutofillFormData](#importautofillformdata)|자동 채우기 양식 데이터 가져오기 허용|
|[ImportBrowserSettings](#importbrowsersettings)|브라우저 설정 가져오기 허용|
|[ImportFavorites](#importfavorites)|즐겨찾기 가져오기 허용|
|[ImportHistory](#importhistory)|검색 기록 가져오기 허용|
|[ImportHomepage](#importhomepage)|홈 페이지 설정 가져오기 허용|
|[ImportOpenTabs](#importopentabs)|열린 탭 가져오기 허용|
|[ImportPaymentInfo](#importpaymentinfo)|결제 정보 가져오기 허용|
|[ImportSavedPasswords](#importsavedpasswords)|저장된 암호 가져오기 허용|
|[ImportSearchEngine](#importsearchengine)|검색 엔진 설정 가져오기 허용|
|[InPrivateModeAvailability](#inprivatemodeavailability)|InPrivate 모드 가용성 구성|
|[InternetExplorerIntegrationLevel](#internetexplorerintegrationlevel)|Internet Explorer 통합 구성|
|[InternetExplorerIntegrationSiteList](#internetexplorerintegrationsitelist)|엔터프라이즈 모드 사이트 목록 구성|
|[InternetExplorerIntegrationSiteRedirect](#internetexplorerintegrationsiteredirect)|Internet Explorer 모드 페이지에서 시작할 때 구성되지 않은 사이트에 대한 "페이지 내" 탐색 작동 방식 지정|
|[IsolateOrigins](#isolateorigins)|특정 원본에 대해 사이트 격리 사용|
|[ManagedFavorites](#managedfavorites)|즐겨찾기 구성|
|[ManagedSearchEngines](#managedsearchengines)|검색 엔진 관리|
|[MaxConnectionsPerProxy](#maxconnectionsperproxy)|프록시 서버에 대 한 동시 연결의 최대 수|
|[MediaRouterCastAllowAllIPs](#mediaroutercastallowallips)|Google Cast가 모든 IP 주소의 캐스트 장치에 연결하도록 허용|
|[MetricsReportingEnabled](#metricsreportingenabled)|사용 현황 및 크래시 관련 데이터 보고 사용|
|[NetworkPredictionOptions](#networkpredictionoptions)|네트워크 예측 사용|
|[NonRemovableProfileEnabled](#nonremovableprofileenabled)|사용자가 회사 또는 학교 계정으로 자동으로 로그인한 기본 프로필을 항상 가지고 있는지 여부를 구성합니다.|
|[OverrideSecurityRestrictionsOnInsecureOrigin](#overridesecurityrestrictionsoninsecureorigin)|안전하지 않은 원본에 대한 보안 제한이 적용되는 위치 제어|
|[ProactiveAuthEnabled](#proactiveauthenabled)|사전 인증 사용|
|[PromotionalTabsEnabled](#promotionaltabsenabled)|전체 탭 프로모션 콘텐츠 사용|
|[PromptForDownloadLocation](#promptfordownloadlocation)|다운로드한 파일을 저장할 위치 묻기|
|[QuicAllowed](#quicallowed)|QUIC 프로토콜 허용|
|[RelaunchNotification](#relaunchnotification)|보류 중인 업데이트에 대해 브라우저 다시 시작이 권장되거나 필요함을 사용자에게 알림|
|[RelaunchNotificationPeriod](#relaunchnotificationperiod)|업데이트 알림 기간 설정|
|[RendererCodeIntegrityEnabled](#renderercodeintegrityenabled)|렌더러 코드 무결성 사용|
|[RequireOnlineRevocationChecksForLocalAnchors](#requireonlinerevocationchecksforlocalanchors)|온라인 OCSP/CRL 검사가 로컬 트러스트 앵커에 필요한지 여부를 지정합니다.|
|[ResolveNavigationErrorsUseWebService](#resolvenavigationerrorsusewebservice)|웹 서비스를 사용하여 탐색 오류 해결 사용|
|[RestrictSigninToPattern](#restrictsignintopattern)|Microsoft Edge 기본 계정으로 사용할 수 있는 계정 제한|
|[RunAllFlashInAllowMode](#runallflashinallowmode)|Adobe Flash 콘텐츠 설정을 모든 콘텐츠로 확장|
|[SSLErrorOverrideAllowed](#sslerroroverrideallowed)|HTTPS 경고 페이지에서 사용자가 작업을 계속할 수 있도록 허용|
|[SSLVersionMin](#sslversionmin)|최소 TLS 버전 사용|
|[SavingBrowserHistoryDisabled](#savingbrowserhistorydisabled)|브라우저 기록 저장 사용 안 함|
|[SearchSuggestEnabled](#searchsuggestenabled)|검색 제안 사용|
|[SecurityKeyPermitAttestation](#securitykeypermitattestation)|직접 보안 키 증명 사용 권한이 필요하지 않은 웹 사이트 또는 도메인|
|[SendIntranetToInternetExplorer](#sendintranettointernetexplorer)|모든 인트라넷 사이트를 Internet Explorer로 보내기|
|[SendSiteInfoToImproveServices](#sendsiteinfotoimproveservices)|Microsoft 서비스 개선을 위해 사이트 정보 보내기|
|[ShowOfficeShortcutInFavoritesBar](#showofficeshortcutinfavoritesbar)|즐겨 찾기 모음에 Microsoft Office 바로 가기 표시|
|[SignedHTTPExchangeEnabled](#signedhttpexchangeenabled)|서명된 HTTP 교환(SXG) 지원 사용|
|[SitePerProcess](#siteperprocess)|모든 사이트에 대해 사이트 격리 사용|
|[SpellcheckEnabled](#spellcheckenabled)|맞춤법 검사 사용|
|[SpellcheckLanguage](#spellchecklanguage)|특정 맞춤법 검사 언어 사용|
|[SpellcheckLanguageBlocklist](#spellchecklanguageblocklist)|맞춤법 검사 언어 강제 사용 안 함|
|[SuppressUnsupportedOSWarning](#suppressunsupportedoswarning)|지원 되지 않는 OS 경고 표시 안 함|
|[SyncDisabled](#syncdisabled)|Microsoft 동기화 서비스를 사용한 데이터의 동기화 사용 안 함|
|[TabFreezingEnabled](#tabfreezingenabled)|Allow freezing of background tabs|
|[TaskManagerEndProcessEnabled](#taskmanagerendprocessenabled)|브라우저 작업 관리자에서 종료 프로세스 사용|
|[TrackingPrevention](#trackingprevention)|사용자의 웹 검색 활동 추적 차단|
|[TranslateEnabled](#translateenabled)|번역 사용|
|[URLAllowlist](#urlallowlist)|허용된 URL 목록을 정의|
|[URLBlocklist](#urlblocklist)|URL 목록에 대한 액세스 차단|
|[UserDataDir](#userdatadir)|사용자 데이터 디렉터리 설정|
|[UserFeedbackAllowed](#userfeedbackallowed)|사용자 피드백 허용|
|[VideoCaptureAllowed](#videocaptureallowed)|비디오 캡처 허용 또는 차단|
|[VideoCaptureAllowedUrls](#videocaptureallowedurls)|권한을 요청하지 않고 비디오 캡처 장치에 액세스할 수 있는 사이트|
|[WPADQuickCheckEnabled](#wpadquickcheckenabled)|WPAD 최적화 설정|
|[WebDriverOverridesIncompatiblePolicies](#webdriveroverridesincompatiblepolicies)|WebDriver가 호환되지 않는 정책을 재정의하도록 허용|
|[WebRtcLocalhostIpHandling](#webrtclocalhostiphandling)|WebRTC에 의한 로컬호스트 IP 주소 노출 제한|
|[WebRtcUdpPortRange](#webrtcudpportrange)|WebRTC에서 사용하는 로컬 UDP 포트 범위 제한|




  ## Cast policies

  [맨 위로 이동](#microsoft-edge---정책)

  ### EnableMediaRouter
  #### Google Cast 사용
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  이 정책을 사용하면 Google Cast를 사용하도록 설정할 수 있습니다. 사용자는 앱 메뉴, 페이지 상황에 맞는 메뉴, 캐스트 사용 웹 사이트의 미디어 컨트롤 및 캐스트 도구 모음 아이콘(표시되는 경우)에서 이를 시작할 수 있습니다.

Google 캐스트를 사용하지 않으려면 이 정책을 사용하지 않도록 설정하세요.

기본적으로 Google 캐스트를 사용하도록 설정되어 있습니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 아니요 - 브라우저 다시 시작 필요

  #### 데이터 형식:
  부울

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: EnableMediaRouter
  - GP 이름: Google Cast 사용
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/Cast
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: EnableMediaRouter
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000001
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: EnableMediaRouter
  - 예제 값:
``` xml
<true/>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### ShowCastIconInToolbar
  #### 도구 모음에서 캐스트 아이콘 표시
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  Set this policy to true to show the Cast toolbar icon on the toolbar or the overflow menu. Users won't be able to remove it.

If you don't configure this policy or if you disable it, users can pin or remove the icon by using its contextual menu.

If you've also set the [EnableMediaRouter](#enablemediarouter) policy to false, then this policy is ignored, and the toolbar icon isn't shown.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 아니요 - 브라우저 다시 시작 필요

  #### 데이터 형식:
  부울

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: ShowCastIconInToolbar
  - GP 이름: 도구 모음에서 캐스트 아이콘 표시
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/Cast
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: ShowCastIconInToolbar
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000000
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: ShowCastIconInToolbar
  - 예제 값:
``` xml
<false/>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ## HTTP 인증 policies

  [맨 위로 이동](#microsoft-edge---정책)

  ### AllowCrossOriginAuthPrompt
  #### 원본 간 HTTP 기본 인증 메시지 표시 허용
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  페이지의 타사 하위 콘텐츠가 HTTP 기본 인증 대화 상자를 열 수 있는지 여부를 제어합니다.

일반적으로 피싱 방어는 사용하지 않도록 설정되어 있습니다. 이 정책을 구성하지 않는 경우 사용하지 않도록 설정되고 타사 하위 콘텐츠는 HTTP 기본 인증 대화 상자를 열 수 없습니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  부울

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: AllowCrossOriginAuthPrompt
  - GP 이름: 원본 간 HTTP 기본 인증 메시지 표시 허용
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/HTTP 인증
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: AllowCrossOriginAuthPrompt
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000000
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: AllowCrossOriginAuthPrompt
  - 예제 값:
``` xml
<false/>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### AuthNegotiateDelegateAllowlist
  #### Microsoft Edge가 사용자 자격 증명을 위임할 수 있는 서버 목록을 지정합니다.
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  Microsoft Edge가 위임할 수 있는 서버 목록을 구성합니다.

여러 개의 서버 이름을 쉼표로 구분합니다. 와일드카드(*)는 허용됩니다.

이 정책을 구성하지 않으면 서버가 인트라넷으로 검색된 경우에도 Microsoft Edge는 사용자 자격 증명을 위임하지 않습니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 아니요 - 브라우저 다시 시작 필요

  #### 데이터 형식:
  문자열

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: AuthNegotiateDelegateAllowlist
  - GP 이름: Microsoft Edge가 사용자 자격 증명을 위임할 수 있는 서버 목록을 지정합니다.
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/HTTP 인증
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: AuthNegotiateDelegateAllowlist
  - 값 형식: REG_SZ
  ##### 예제 값:
```
"contoso.com"
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: AuthNegotiateDelegateAllowlist
  - 예제 값:
``` xml
<string>contoso.com</string>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### AuthSchemes
  #### 지원되는 인증 방식
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  지원되는 HTTP 인증 체계를 지정합니다.

'기본', '다이제스트', 'ntlm'및 '협상'과 같은 값을 사용하여 정책을 구성 할 수 있습니다. 값이 여러 개라면 쉼표로 구분하세요.

이 정책을 구성하지 않으면 네 가지 구성이 모두 사용됩니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 아니요 - 브라우저 다시 시작 필요

  #### 데이터 형식:
  문자열

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: AuthSchemes
  - GP 이름: 지원되는 인증 방식
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/HTTP 인증
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: AuthSchemes
  - 값 형식: REG_SZ
  ##### 예제 값:
```
"basic,digest,ntlm,negotiate"
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: AuthSchemes
  - 예제 값:
``` xml
<string>basic,digest,ntlm,negotiate</string>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### AuthServerAllowlist
  #### 허용된 인증 서버의 목록 구성
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  통합 인증을 위해 사용할 서버를 지정합니다. 통합 인증은 Microsoft Edge가 프록시 또는 이 목록의 서버로부터 인증 질문을 받는 경우에만 활성화됩니다.

여러 서버 이름은 쉼표로 구분합니다. 와일드 카드(*)를 사용할 수 있습니다.

이 정책을 구성하지 않으면 Microsoft Edge에서 서버가 인트라넷에 있는지 검색하려고 하고, 그런 다음에만 IWA 요청에 응답합니다. 서버가 인터넷에 연결되어 있으면 Microsoft Edge에 의해 IWA 요청이 무시됩니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 아니요 - 브라우저 다시 시작 필요

  #### 데이터 형식:
  문자열

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: AuthServerAllowlist
  - GP 이름: 허용된 인증 서버의 목록 구성
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/HTTP 인증
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: AuthServerAllowlist
  - 값 형식: REG_SZ
  ##### 예제 값:
```
"*contoso.com,contoso.com"
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: AuthServerAllowlist
  - 예제 값:
``` xml
<string>*contoso.com,contoso.com</string>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### DisableAuthNegotiateCnameLookup
  #### Kerberos 인증을 협상할 때 CNAME 조회 사용 안 함
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  생성된 Kerberos SPN이 정식 DNS 이름(CNAME)을 기반으로 하는지 아니면 원래 원본 이름에 기반으로 하는지 여부를 결정합니다.

이 정책을 사용하면 CNAME 조회를 건너뛰고 입력한 대로 서버 이름이 사용됩니다.

이 정책 설정을 사용하지 않거나 구성하지 않으면 서버의 정식 이름이 사용됩니다. CNAME 조회를 통해 결정 됩니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 아니요 - 브라우저 다시 시작 필요

  #### 데이터 형식:
  부울

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: DisableAuthNegotiateCnameLookup
  - GP 이름: Kerberos 인증을 협상할 때 CNAME 조회 사용 안 함
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/HTTP 인증
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: DisableAuthNegotiateCnameLookup
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000000
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: DisableAuthNegotiateCnameLookup
  - 예제 값:
``` xml
<false/>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### EnableAuthNegotiatePort
  #### Kerberos SPN에 비표준 포트 포함
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  생성 된 Kerberos SPN에 비표준 포트가 포함되어야 하는지 여부를 지정합니다.

이 정책을 사용하고 사용자가 URL에 비표준 포트 (80 또는 443 이외의 포트)를 포함하면 해당 포트가 생성 된 Kerberos SPN에 포함됩니다.

이 정책을 구성하거나 사용하지 않으면 생성된 Kerberos SPN에는 어떤 경우에도 포트가 포함되지 않습니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 아니요 - 브라우저 다시 시작 필요

  #### 데이터 형식:
  부울

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: EnableAuthNegotiatePort
  - GP 이름: Kerberos SPN에 비표준 포트 포함
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/HTTP 인증
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: EnableAuthNegotiatePort
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000000
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: EnableAuthNegotiatePort
  - 예제 값:
``` xml
<false/>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### NtlmV2Enabled
  #### NTLMv2 인증을 사용할지 여부 제어
  >지원되는 버전: Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  NTLMv2를 사용할지 여부를 제어합니다.

모든 최신 버전의 삼바 및 Windows 서버는 NTLMv2 지원합니다. NTLMv2를 사용하지 않도록 설정하면 인증 보안이 약화되기 때문에 이전 버전과의 호환성 문제를 해결하기 위해서만 NTLMv2를 사용하지 않도록 설정해야 합니다.

이 정책을 구성하지 않으면 NTLMv2는 기본적으로 사용하도록 설정됩니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  부울

  

  #### Mac 정보 및 설정
  - 기본 설정 키 이름: NtlmV2Enabled
  - 예제 값:
``` xml
<true/>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ## SmartScreen 설정 policies

  [맨 위로 이동](#microsoft-edge---정책)

  ### PreventSmartScreenPromptOverride
  #### 사이트에 대한 Microsoft Defender SmartScreen 프롬프트 무시 허용 안 함
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  이 정책 설정을 통해 사용자가 잠재적으로 악성 웹 사이트에 대한 Microsoft Defender SmartScreen 경고를 재정의할 수 있는지 여부를 결정할 수 있습니다.

이 설정을 사용하면 사용자가 Microsoft Defender SmartScreen 경고를 무시할 수 없으며 사이트로 이동하지 못합니다.

이 설정을 사용하지 않도록 설정하거나 구성하지 않으면 사용자가 Microsoft Defender SmartScreen 경고를 무시하고 사이트로 이동할 수 있습니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  부울

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: PreventSmartScreenPromptOverride
  - GP 이름: 사이트에 대한 Microsoft Defender SmartScreen 프롬프트 무시 허용 안 함
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/SmartScreen 설정
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: PreventSmartScreenPromptOverride
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000001
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: PreventSmartScreenPromptOverride
  - 예제 값:
``` xml
<true/>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### PreventSmartScreenPromptOverrideForFiles
  #### 다운로드에 대한 Microsoft Defender SmartScreen 경고 무시 허용 안 함
  >지원되는 버전: Windows의 Microsoft Edge, 버전 77 이상부터 및 Mac, 버전 79 이상부터

  #### 설명
  이 정책을 통해 확인되지 않은 다운로드에 대한 Microsoft Defender SmartScreen 경고를 무시할수 있는지 여부를 결정할 수 있습니다.

이 정책을 사용하면 조직의 사용자가 Microsoft Defender SmartScreen 경고를 무시할 수 없으며 확인되지 않은 다운로드를 완료할 수 없습니다.

이 정책을 사용하지 않거나 구성하지 않으면 사용자가 Microsoft Defender SmartScreen 경고를 무시하고 확인되지 않은 다운로드를 완료할 수 있습니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  부울

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: PreventSmartScreenPromptOverrideForFiles
  - GP 이름: 다운로드에 대한 Microsoft Defender SmartScreen 경고 무시 허용 안 함
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/SmartScreen 설정
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: PreventSmartScreenPromptOverrideForFiles
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000001
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: PreventSmartScreenPromptOverrideForFiles
  - 예제 값:
``` xml
<true/>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### SmartScreenAllowListDomains
  #### Microsoft Defender SmartScreen이 경고를 트리거하지 않는 도메인 목록 구성
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  Microsoft Defender SmartScreen에서 트러스트된 도메인 목록을 구성합니다. 즉,
원본 URL이 이 도메인과 일치하는 경우 Microsoft Defender SmartScreen은 피싱 소프트웨어 및 기타 맬웨어와 같은 잠재적 악성 리소스를 확인하지 않습니다.
Microsoft Defender SmartScreen 다운로드 보호 서비스는 해당 도메인에서 호스팅되는 다운로드를 확인하지 않습니다.

이 정책을 사용하면 Microsoft Defender SmartScreen에서 이러한 도메인을 신뢰합니다.
이 정책을 사용하지 않거나 설정하지 않으면 기본 Microsoft Defender SmartScreen 보호가 모든 리소스에 적용됩니다.
이 정책은 Microsoft Active Directory 도메인에 가입된 Windows 인스턴스 또는 장치 관리를 위해 등록된 Windows 10 Pro나 Enterprise 인스턴스에서만 사용할 수 있습니다.
또한 조직에서 Microsoft Defender Advanced Threat Protection을 사용하도록 설정한 경우에는 이 정책이 적용되지 않습니다. Microsoft Defender 보안 센터에서 허용 및 차단 목록을 구성해야 합니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  문자열 목록

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: SmartScreenAllowListDomains
  - GP 이름: Microsoft Defender SmartScreen이 경고를 트리거하지 않는 도메인 목록 구성
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/SmartScreen 설정
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge\SmartScreenAllowListDomains
  - 경로 (맞춤): 해당 없음
  - 값 이름: 1, 2, 3, ...
  - 값 형식: REG_SZ 목록
  ##### 예제 값:
```
SOFTWARE\Policies\Microsoft\Edge\SmartScreenAllowListDomains\0 = "mydomain.com"
SOFTWARE\Policies\Microsoft\Edge\SmartScreenAllowListDomains\1 = "myuniversity.edu"

```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: SmartScreenAllowListDomains
  - 예제 값:
``` xml
<array>
  <string>mydomain.com</string>
  <string>myuniversity.edu</string>
</array>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### SmartScreenEnabled
  #### Microsoft Defender SmartScreen 구성
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  This policy setting lets you configure whether to turn on Microsoft Defender SmartScreen. Microsoft Defender SmartScreen provides warning messages to help protect your users from potential phishing scams and malicious software. By default, Microsoft Defender SmartScreen is turned on.

If you enable this setting, Microsoft Defender SmartScreen is turned on.

If you disable this setting, Microsoft Defender SmartScreen is turned off.

If you don't configure this setting, users can choose whether to use Microsoft Defender SmartScreen.

This policy is available only on Windows instances that are joined to a Microsoft Active Directory domain; or on Windows 10 Pro or Enterprise instances that are enrolled for device management.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 예
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  부울

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: SmartScreenEnabled
  - GP 이름: Microsoft Defender SmartScreen 구성
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/SmartScreen 설정
  - GP 경로 (맞춤): 관리 템플릿/Microsoft Edge - 기본 설정(사용자가 재정의할 수 없음)/SmartScreen 설정
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): SOFTWARE\Policies\Microsoft\Edge\맞춤
  - 값 이름: SmartScreenEnabled
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000001
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: SmartScreenEnabled
  - 예제 값:
``` xml
<true/>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### SmartScreenForTrustedDownloadsEnabled
  #### 신뢰할 수 있는 원본의 다운로드에 대한 Microsoft Defender SmartScreen 검사 강제 적용
  >지원되는 버전: Windows의 Microsoft Edge, 버전 78 이상부터

  #### 설명
  이 정책 설정을 통해 Microsoft Defender SmartScreen이 신뢰할 수 있는 원본의 다운로드 신뢰도를 확인할 지 여부를 구성할 수 있습니다.

이 설정을 사용하거나 구성하지 않으면 Microsoft Defender SmartScreen이 원본에 관계 없이 다운로드의 신뢰도를 확인합니다.

이 설정을 사용하지 않으면 Microsoft Defender SmartScreen이 신뢰할 수 있는 원본에서 다운로드할 때 다운로드의 신뢰도를 확인하지 않습니다.

이 정책은 Microsoft Active Directory 도메인에 가입된 Windows 인스턴스 또는 장치 관리를 위해 등록된 Windows 10 Pro나 Enterprise 인스턴스에서만 사용할 수 있습니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 예
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  부울

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: SmartScreenForTrustedDownloadsEnabled
  - GP 이름: 신뢰할 수 있는 원본의 다운로드에 대한 Microsoft Defender SmartScreen 검사 강제 적용
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/SmartScreen 설정
  - GP 경로 (맞춤): 관리 템플릿/Microsoft Edge - 기본 설정(사용자가 재정의할 수 없음)/SmartScreen 설정
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): SOFTWARE\Policies\Microsoft\Edge\맞춤
  - 값 이름: SmartScreenForTrustedDownloadsEnabled
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000000
```


  

  [맨 위로 이동](#microsoft-edge---정책)

  ### SmartScreenPuaEnabled
  #### Configure Microsoft Defender SmartScreen to block potentially unwanted apps
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 80 이상부터

  #### 설명
  This policy setting lets you configure whether to turn on blocking for potentially unwanted apps in Microsoft Defender SmartScreen. Potentially unwanted app blocking in Microsoft Defender SmartScreen provides warning messages to help protect users from adware, coin miners, bundleware, and other low-reputation apps that are hosted by websites. Potentially unwanted app blocking in Microsoft Defender SmartScreen is turned off by default.

If you enable this setting, potentially unwanted app blocking in Microsoft Defender SmartScreen is turned on.

If you disable this setting, potentially unwanted app blocking in Microsoft Defender SmartScreen is turned off.

If you don't configure this setting, users can choose whether to use potentially unwanted app blocking in Microsoft Defender SmartScreen.

This policy is available only on Windows instances that are joined to a Microsoft Active Directory domain; or on Windows 10 Pro or Enterprise instances that are enrolled for device management.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 예
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  부울

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: SmartScreenPuaEnabled
  - GP 이름: Configure Microsoft Defender SmartScreen to block potentially unwanted apps
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/SmartScreen 설정
  - GP 경로 (맞춤): 관리 템플릿/Microsoft Edge - 기본 설정(사용자가 재정의할 수 없음)/SmartScreen 설정
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): SOFTWARE\Policies\Microsoft\Edge\맞춤
  - 값 이름: SmartScreenPuaEnabled
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000001
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: SmartScreenPuaEnabled
  - 예제 값:
``` xml
<true/>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ## 기본 검색 공급자 policies

  [맨 위로 이동](#microsoft-edge---정책)

  ### DefaultSearchProviderEnabled
  #### 기본 검색 공급자 사용
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  기본 검색 공급자를 사용하도록 설정합니다.

이 정책을 사용하면 (입력한 내용이 URL이 아닌 한) 사용자가 주소 표시줄에 검색어를 입력하여 검색할 수 있습니다.

기본 검색 정책의 나머지 부분을 사용하도록 설정하여 사용할 기본 검색 공급자를 지정할 수 있습니다. 이 항목을 비워두면(구성되지 않음) 사용자는 기본 공급자를 선택할 수 있습니다.

이 정책을 사용하지 않으면 사용자가 주소 표시줄에서 검색할 수 없습니다.

이 정책을 사용하거나 사용하지 않도록 설정하면 사용자가 변경하거나 재정의할 수 없습니다.

이 정책을 구성하지 않으면 기본 검색 공급자가 사용하도록 설정되며 사용자가 기본 검색 공급자를 선택하고 검색 공급자 목록을 설정할 수입니다.

이 정책은 Microsoft Active Directory 도메인에 가입된 Windows 인스턴스 또는 장치 관리를 위해 등록된 Windows 10 Pro나 엔터프라이즈 인스턴스에서만 사용할 수 있습니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  부울

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: DefaultSearchProviderEnabled
  - GP 이름: 기본 검색 공급자 사용
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/기본 검색 공급자
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: DefaultSearchProviderEnabled
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000001
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: DefaultSearchProviderEnabled
  - 예제 값:
``` xml
<true/>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### DefaultSearchProviderEncodings
  #### 기본 검색 공급자 인코딩
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  Specify the character encodings supported by the search provider. Encodings are code page names like UTF-8, GB2312, and ISO-8859-1. They are tried in the order provided.

This policy is optional. If not configured, the default, UTF-8, is used.

This policy is applied only if you enable the [DefaultSearchProviderEnabled](#defaultsearchproviderenabled) and [DefaultSearchProviderSearchURL](#defaultsearchprovidersearchurl) policies.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  문자열 목록

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: DefaultSearchProviderEncodings
  - GP 이름: 기본 검색 공급자 인코딩
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/기본 검색 공급자
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge\DefaultSearchProviderEncodings
  - 경로 (맞춤): 해당 없음
  - 값 이름: 1, 2, 3, ...
  - 값 형식: REG_SZ 목록
  ##### 예제 값:
```
SOFTWARE\Policies\Microsoft\Edge\DefaultSearchProviderEncodings\0 = "UTF-8"
SOFTWARE\Policies\Microsoft\Edge\DefaultSearchProviderEncodings\1 = "UTF-16"
SOFTWARE\Policies\Microsoft\Edge\DefaultSearchProviderEncodings\2 = "GB2312"
SOFTWARE\Policies\Microsoft\Edge\DefaultSearchProviderEncodings\3 = "ISO-8859-1"

```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: DefaultSearchProviderEncodings
  - 예제 값:
``` xml
<array>
  <string>UTF-8</string>
  <string>UTF-16</string>
  <string>GB2312</string>
  <string>ISO-8859-1</string>
</array>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### DefaultSearchProviderImageURL
  #### 기본 검색 공급자에 대한 이미지로 검색하기 기능을 지정합니다.
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  Specifies the URL to the search engine used for image search. Search requests are sent using the GET method.

This policy is optional. If you don't configure it, image search isn't available.

Specify Bing's Image Search URL as:
'{bing:baseURL}images/detail/search?iss=sbiupload&FORM=ANCMS1#enterInsights'.

Specify Google's Image Search URL as: '{google:baseURL}searchbyimage/upload'.

See [DefaultSearchProviderImageURLPostParams](#defaultsearchproviderimageurlpostparams) policy to finish configuring image search.

This policy is applied only if you enable the [DefaultSearchProviderEnabled](#defaultsearchproviderenabled) and [DefaultSearchProviderSearchURL](#defaultsearchprovidersearchurl) policies.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  문자열

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: DefaultSearchProviderImageURL
  - GP 이름: 기본 검색 공급자에 대한 이미지로 검색하기 기능을 지정합니다.
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/기본 검색 공급자
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: DefaultSearchProviderImageURL
  - 값 형식: REG_SZ
  ##### 예제 값:
```
"https://search.contoso.com/searchbyimage/upload"
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: DefaultSearchProviderImageURL
  - 예제 값:
``` xml
<string>https://search.contoso.com/searchbyimage/upload</string>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### DefaultSearchProviderImageURLPostParams
  #### POST를 사용하는 이미지 URL에 대한 매개 변수
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  If you enable this policy, it specifies the parameters used when an image search that uses POST is performed. The policy consists of comma-separated name/value pairs. If a value is a template parameter, like {imageThumbnail} in the preceding example, it’s replaced with real image thumbnail data. This policy is applied only if you enable the [DefaultSearchProviderEnabled](#defaultsearchproviderenabled) and [DefaultSearchProviderSearchURL](#defaultsearchprovidersearchurl) policies.

Specify Bing's Image Search URL Post Params as:
'imageBin={google:imageThumbnailBase64}'.

Specify Google's Image Search URL Post Params as:
'encoded_image={google:imageThumbnail},image_url={google:imageURL},sbisrc={google:imageSearchSource},original_width={google:imageOriginalWidth},original_height={google:imageOriginalHeight}'.

If you don’t set this policy, image search requests are sent using the GET method.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  문자열

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: DefaultSearchProviderImageURLPostParams
  - GP 이름: POST를 사용하는 이미지 URL에 대한 매개 변수
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/기본 검색 공급자
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: DefaultSearchProviderImageURLPostParams
  - 값 형식: REG_SZ
  ##### 예제 값:
```
"content={imageThumbnail},url={imageURL},sbisrc={SearchSource}"
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: DefaultSearchProviderImageURLPostParams
  - 예제 값:
``` xml
<string>content={imageThumbnail},url={imageURL},sbisrc={SearchSource}</string>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### DefaultSearchProviderKeyword
  #### 기본 검색 공급자 키워드
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  Specifies the keyword, which is the shortcut used in the Address Bar to trigger the search for this provider.

This policy is optional. If you don't configure it, no keyword activates the search provider.

This policy is applied only if you enable the [DefaultSearchProviderEnabled](#defaultsearchproviderenabled) and [DefaultSearchProviderSearchURL](#defaultsearchprovidersearchurl) policies.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  문자열

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: DefaultSearchProviderKeyword
  - GP 이름: 기본 검색 공급자 키워드
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/기본 검색 공급자
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: DefaultSearchProviderKeyword
  - 값 형식: REG_SZ
  ##### 예제 값:
```
"mis"
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: DefaultSearchProviderKeyword
  - 예제 값:
``` xml
<string>mis</string>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### DefaultSearchProviderName
  #### 기본 검색 공급자 이름
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  Specifies the name of the default search provider.

If you enable this policy, you set the name of the default search provider.

If you don't enable this policy or if you leave it empty, the host name specified by the search URL is used.

'DefaultSearchProviderName' should be set to an organization-approved encrypted search provider that corresponds to the encrypted search provider set in DTBC-0008. This policy is applied only if you enable the [DefaultSearchProviderEnabled](#defaultsearchproviderenabled) and [DefaultSearchProviderSearchURL](#defaultsearchprovidersearchurl) policies.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  문자열

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: DefaultSearchProviderName
  - GP 이름: 기본 검색 공급자 이름
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/기본 검색 공급자
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: DefaultSearchProviderName
  - 값 형식: REG_SZ
  ##### 예제 값:
```
"My Intranet Search"
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: DefaultSearchProviderName
  - 예제 값:
``` xml
<string>My Intranet Search</string>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### DefaultSearchProviderSearchURL
  #### 기본 검색 공급자 검색 URL
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  Specifies the URL of the search engine used for a default search. The URL contains the string '{searchTerms}', which is replaced at query time by the terms the user is searching for.

Specify Bing's search URL as:

'{bing:baseURL}search?q={searchTerms}'.

Specify Google's search URL as: '{google:baseURL}search?q={searchTerms}&{google:RLZ}{google:originalQueryForSuggestion}{google:assistedQueryStats}{google:searchFieldtrialParameter}{google:searchClient}{google:sourceId}ie={inputEncoding}'.

This policy is required when you enable the [DefaultSearchProviderEnabled](#defaultsearchproviderenabled) policy; if you don't enable the latter policy, this policy is ignored.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  문자열

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: DefaultSearchProviderSearchURL
  - GP 이름: 기본 검색 공급자 검색 URL
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/기본 검색 공급자
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: DefaultSearchProviderSearchURL
  - 값 형식: REG_SZ
  ##### 예제 값:
```
"https://search.contoso.com/search?q={searchTerms}"
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: DefaultSearchProviderSearchURL
  - 예제 값:
``` xml
<string>https://search.contoso.com/search?q={searchTerms}</string>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### DefaultSearchProviderSuggestURL
  #### 제안에 대한 기본 검색 공급자 URL
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  Specifies the URL for the search engine used to provide search suggestions. The URL contains the string '{searchTerms}', which is replaced at query time by the text the user has entered so far.

This policy is optional. If you don't configure it, users won't see search suggestions; they will see suggestions from their browsing history and favorites.

Bing's suggest URL can be specified as:

'{bing:baseURL}qbox?query={searchTerms}'.

Google's suggest URL can be specified as: '{google:baseURL}complete/search?output=chrome&q={searchTerms}'.

This policy is applied only if you enable the [DefaultSearchProviderEnabled](#defaultsearchproviderenabled) and [DefaultSearchProviderSearchURL](#defaultsearchprovidersearchurl) policies.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  문자열

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: DefaultSearchProviderSuggestURL
  - GP 이름: 제안에 대한 기본 검색 공급자 URL
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/기본 검색 공급자
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: DefaultSearchProviderSuggestURL
  - 값 형식: REG_SZ
  ##### 예제 값:
```
"https://search.contoso.com/suggest?q={searchTerms}"
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: DefaultSearchProviderSuggestURL
  - 예제 값:
``` xml
<string>https://search.contoso.com/suggest?q={searchTerms}</string>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ## 기본 메시지 policies

  [맨 위로 이동](#microsoft-edge---정책)

  ### NativeMessagingAllowlist
  #### 사용자가 사용할 수 있는 기본 메시징 호스트 제어
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  List specific native messaging hosts that users can use in Microsoft Edge.

By default, all native messaging hosts are allowed. If you set the [NativeMessagingBlocklist](#nativemessagingblocklist) policy to *, all native messaging hosts are blocked, and only native messaging hosts listed in here are loaded.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  문자열 목록

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: NativeMessagingAllowlist
  - GP 이름: 사용자가 사용할 수 있는 기본 메시징 호스트 제어
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/기본 메시지
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge\NativeMessagingAllowlist
  - 경로 (맞춤): 해당 없음
  - 값 이름: 1, 2, 3, ...
  - 값 형식: REG_SZ 목록
  ##### 예제 값:
```
SOFTWARE\Policies\Microsoft\Edge\NativeMessagingAllowlist\0 = "com.native.messaging.host.name1"
SOFTWARE\Policies\Microsoft\Edge\NativeMessagingAllowlist\1 = "com.native.messaging.host.name2"

```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: NativeMessagingAllowlist
  - 예제 값:
``` xml
<array>
  <string>com.native.messaging.host.name1</string>
  <string>com.native.messaging.host.name2</string>
</array>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### NativeMessagingBlocklist
  #### 기본 메시지 차단 목록 구성
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  사용할 수 없는 기본 메시징 호스트를 지정합니다.

허용 목록에 명시적으로 나열되어 있지 않는 한 '*'를 사용하여 모든 기본 메시징 호스트를 차단합니다.

이 정책을 구성하지 않으면 Microsoft Edge 는 설치된 모든 기본 메시징 호스트를 로드합니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  문자열 목록

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: NativeMessagingBlocklist
  - GP 이름: 기본 메시지 차단 목록 구성
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/기본 메시지
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge\NativeMessagingBlocklist
  - 경로 (맞춤): 해당 없음
  - 값 이름: 1, 2, 3, ...
  - 값 형식: REG_SZ 목록
  ##### 예제 값:
```
SOFTWARE\Policies\Microsoft\Edge\NativeMessagingBlocklist\0 = "com.native.messaging.host.name1"
SOFTWARE\Policies\Microsoft\Edge\NativeMessagingBlocklist\1 = "com.native.messaging.host.name2"

```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: NativeMessagingBlocklist
  - 예제 값:
``` xml
<array>
  <string>com.native.messaging.host.name1</string>
  <string>com.native.messaging.host.name2</string>
</array>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### NativeMessagingUserLevelHosts
  #### 사용자 수준 기본 메시징 호스트 허용(관리자 권한 없이 설치됨)
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  기본 메시징 호스트의 사용자 수준 설치를 사용하도록 설정합니다.

이 정책을 사용하지 않으면 Microsoft Edge는 시스템 수준에 설치된 기본 메시징 호스트만 사용합니다.

기본적으로 이 정책을 구성하지 않으면 Microsoft Edge는 사용자 수준 기본 메시징 호스트의 사용을 허용합니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  부울

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: NativeMessagingUserLevelHosts
  - GP 이름: 사용자 수준 기본 메시징 호스트 허용(관리자 권한 없이 설치됨)
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/기본 메시지
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: NativeMessagingUserLevelHosts
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000000
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: NativeMessagingUserLevelHosts
  - 예제 값:
``` xml
<false/>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ## 시작&comma; 홈 페이지 및 새 탭 페이지 policies

  [맨 위로 이동](#microsoft-edge---정책)

  ### HomepageIsNewTabPage
  #### 새 탭 페이지를 홈 페이지로 설정
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  Microsoft Edge에서 기본 홈 페이지를 구성합니다. 지정한 URL 또는 새 탭 페이지를 홈 페이지를 설정할 수 있습니다.

이 정책을 사용하면 항상 새 탭 페이지가 홈 페이지에 사용되며 홈 페이지 URL 위치는 무시됩니다.

이 정책을 사용하지 않으면 'edge://newtab'으로 설정되어 있지 않는 한 사용자의 홈 페이지 URL는 새 탭 페이지가 될 수 없습니다.

구성하지 않으면 사용자는 새 탭 페이지가 자신의 홈 페이지인지 여부를 선택할 수 있습니다.

이 정책은 Microsoft Active Directory도메인에 가입된 Windows 인스턴스 장치 관리를 위해 등록된 Windows 10 Pro나 Enterprise 인스턴스에서만 사용할 수 있습니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 예
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  부울

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: HomepageIsNewTabPage
  - GP 이름: 새 탭 페이지를 홈 페이지로 설정
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/시작, 홈 페이지 및 새 탭 페이지
  - GP 경로 (맞춤): 관리 템플릿/Microsoft Edge - 기본 설정(사용자가 재정의할 수 없음)/시작, 홈 페이지 및 새 탭 페이지
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): SOFTWARE\Policies\Microsoft\Edge\맞춤
  - 값 이름: HomepageIsNewTabPage
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000001
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: HomepageIsNewTabPage
  - 예제 값:
``` xml
<true/>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### HomepageLocation
  #### 홈 페이지 URL 구성
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  Configures the default home page URL in Microsoft Edge.

The home page is the page opened by the Home button. The pages that open on startup are controlled by the [RestoreOnStartup](#restoreonstartup) policies.

You can either set a URL here or set the home page to open the new tab page. If you select to open the new tab page, then this policy doesn't take effect.

If you enable this policy, users can't change their home page URL, but they can choose to use the new tab page as their home page.

If you disable or don't configure this policy, users can choose their own home page, as long as the [HomepageIsNewTabPage](#homepageisnewtabpage) policy isn't enabled.

This policy is available only on Windows instances that are joined to a Microsoft Active Directory domain or Windows 10 Pro or Enterprise instances enrolled for device management.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 예
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  문자열

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: HomepageLocation
  - GP 이름: 홈 페이지 URL 구성
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/시작, 홈 페이지 및 새 탭 페이지
  - GP 경로 (맞춤): 관리 템플릿/Microsoft Edge - 기본 설정(사용자가 재정의할 수 없음)/시작, 홈 페이지 및 새 탭 페이지
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): SOFTWARE\Policies\Microsoft\Edge\맞춤
  - 값 이름: HomepageLocation
  - 값 형식: REG_SZ
  ##### 예제 값:
```
"https://www.contoso.com"
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: HomepageLocation
  - 예제 값:
``` xml
<string>https://www.contoso.com</string>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### NewTabPageCompanyLogo
  #### 새 탭 페이지 회사 로고 설정
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 79 이상부터

  #### 설명
  Microsoft Edge의 새 탭 페이지에서 사용할 회사 로고를 지정합니다.

정책은 로고를 JSON 형식으로 나타내는 문자열로 구성해야 합니다. 예: { "default_logo": { "url": "https://www.contoso.com/logo.png", "hash": "cd0aa9856147b6c5b4ff2b7dfee5da20aa38253099ef1b4a64aced233c9afe29" }, "light_logo": { "url": "https://www.contoso.com/light_logo.png", "hash": "517d286edb416bb2625ccfcba9de78296e90da8e32330d4c9c8275c4c1c33737" } }

Microsoft Edge에서 로고 및 해당 암호화 해시 (SHA-256)를 다운로드 할 수 있는 URL을 지정하여 이 정책을 구성합니다. 로고는 PNG 또는 SVG 형식이어야 하며 파일 크기는 16mb를 초과하지 않아야 합니다. 로고가 다운로드 및 캐시되며 URL 또는 해시가 변경될 때마다 다시 다운로드됩니다. URL은 인증없이 액세스할 수 있어야 합니다.

'default_logo'는 필수이며 배경 이미지가 없을 때 사용됩니다. 'light_logo'가 제공되면 사용자의 새 탭 페이지에 배경 이미지가 있을 때 사용됩니다. 투명 배경이 왼쪽 맞춤 및 세로 가운데에 배치되는 가로 로고를 사용하는 것이 좋습니다. 로고의 최소 높이는 32 픽셀이고 가로 세로 비율은 1:1에서 4:1 사이여야 합니다. 'default_logo'는 흰색/검은색 배경과의 대비가 있으며 'light_logo'는배경 이미지에 대해 적절하게 대비되어야 합니다.

이 정책을 사용하도록 설정하는 경우 Microsoft Edge는 새 탭 페이지에 지정된 로고를 다운로드하여 표시합니다. 사용자는 로고를 무시하거나 숨길 수 없습니다.

이 정책을 사용하지 않거나 구성하지 않으면 Microsoft Edge가 회사 로고나 Microsoft 로고를 새 탭 페이지에 표시하지 않습니다.

SHA-256 해시 결정에 대한 도움말은 https://docs.microsoft.com/en-us/powershell/module/microsoft.powershell.utility/get-filehash?view=powershell-6를 참조하세요.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 아니요 - 브라우저 다시 시작 필요

  #### 데이터 형식:
  사전

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: NewTabPageCompanyLogo
  - GP 이름: 새 탭 페이지 회사 로고 설정
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/시작, 홈 페이지 및 새 탭 페이지
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: NewTabPageCompanyLogo
  - 값 형식: REG_SZ
  ##### 예제 값:
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


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: NewTabPageCompanyLogo
  - 예제 값:
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
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### NewTabPageHideDefaultTopSites
  #### 새 탭 페이지에서 기본 상위 사이트 숨기기
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  Microsoft Edge의 새 탭 페이지에서 기본 상위 사이트를 숨깁니다.

이 정책을 true로 설정하면 기본 상위 사이트 타일이 숨겨집니다.

이 정책을 false로 설정하거나 구성하지 않으면 기본 상위 사이트 타일이 계속 표시됩니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  부울

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: NewTabPageHideDefaultTopSites
  - GP 이름: 새 탭 페이지에서 기본 상위 사이트 숨기기
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/시작, 홈 페이지 및 새 탭 페이지
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: NewTabPageHideDefaultTopSites
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000001
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: NewTabPageHideDefaultTopSites
  - 예제 값:
``` xml
<true/>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### NewTabPageLocation
  #### 새 탭 페이지 URL 구성
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  Configures the default URL for the new tab page.

This policy determines the page that's opened when new tabs are created (including when new windows are opened). It also affects the startup page if that's set to open to the new tab page.

This policy doesn't determine which page opens on startup; that's controlled by the [RestoreOnStartup](#restoreonstartup) policy. It also doesn’t affect the home page if that’s set to open to the new tab page.

If you don't configure this policy, the default new tab page is used.

If you configure this policy *and* the [NewTabPageSetFeedType](#newtabpagesetfeedtype) policy, this policy has precedence.

If an invalid URL is provided, new tabs will open about://blank.

This policy is available only on Windows instances that are joined to a Microsoft Active Directory domain or Windows 10 Pro or Enterprise instances that are enrolled for device management.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 예
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  문자열

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: NewTabPageLocation
  - GP 이름: 새 탭 페이지 URL 구성
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/시작, 홈 페이지 및 새 탭 페이지
  - GP 경로 (맞춤): 관리 템플릿/Microsoft Edge - 기본 설정(사용자가 재정의할 수 없음)/시작, 홈 페이지 및 새 탭 페이지
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): SOFTWARE\Policies\Microsoft\Edge\맞춤
  - 값 이름: NewTabPageLocation
  - 값 형식: REG_SZ
  ##### 예제 값:
```
"https://www.fabrikam.com"
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: NewTabPageLocation
  - 예제 값:
``` xml
<string>https://www.fabrikam.com</string>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### NewTabPageManagedQuickLinks
  #### 새 탭 페이지 빠른 연결 설정
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 79 이상부터

  #### 설명
  기본적으로 Microsoft Edge는 검색 기록을 기반으로 사용자가 추가한 바로 가기 및 상위 사이트의 새 탭 페이지에 빠른 링크를 표시합니다. 이 정책을 사용하여 새 탭 페이지에서 JSON 개체로 표시되는 빠른 링크 타일을 3개까지 구성할 수 있습니다.

[ { "url": "https://www.contoso.com", "title": "Contoso Portal", "pinned": true/false }, ... ]

'url' 필드는 필수입니다. 'title' 및 'pinned'는 선택 사항입니다. 'title'이 제공되지 않으면 URL이 기본 제목으로 사용됩니다. 'pinned'가 제공되지 않으면 기본값은 false입니다.

Microsoft Edge는 고정된 모든 타일이 고정되지 않은 타일보다 먼저 표시되는 순서대로 왼쪽에서 오른쪽으로 나열됩니다.

'pinned' 필드가 무시되고 모든 타일이 고정됩니다. 타일은 사용자가 삭제할 수 없으며 항상 빠른 링크 목록 맨 앞에 표시됩니다.

정책을 권장 사항으로 설정하면 고정된 타일은 목록에 남아 있지만 사용자는 이를 편집하고 삭제할 수 있습니다. 고정되지 않은 빠른 링크 타일은 기본 상위 사이트처럼 작동하며 다른 웹 사이트를 더 자주 방문하는 경우 목록에서 제거됩니다. 이 정책을 통해 고정되지 않은 링크를 기존 브라우저 프로필에 적용할 경우 해당 링크는 사용자의 검색 기록과 비교하여 순위에 따라 전혀 표시되지 않을 수도 있습니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 예
  - 동적 정책 새로 고침: 아니요 - 브라우저 다시 시작 필요

  #### 데이터 형식:
  사전

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: NewTabPageManagedQuickLinks
  - GP 이름: 새 탭 페이지 빠른 연결 설정
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/시작, 홈 페이지 및 새 탭 페이지
  - GP 경로 (맞춤): 관리 템플릿/Microsoft Edge - 기본 설정(사용자가 재정의할 수 없음)/시작, 홈 페이지 및 새 탭 페이지
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): SOFTWARE\Policies\Microsoft\Edge\맞춤
  - 값 이름: NewTabPageManagedQuickLinks
  - 값 형식: REG_SZ
  ##### 예제 값:
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


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: NewTabPageManagedQuickLinks
  - 예제 값:
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
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### NewTabPageSetFeedType
  #### Configure the Microsoft Edge new tab page experience
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 79 이상부터

  #### 설명
  Lets you choose either the Microsoft News or Office 365 feed experience for the new tab page.

When you set this policy to Microsoft News feed experience (0), users will see the Microsoft News feed experience on the new tab page.

When you set this policy to Office 365 feed experience (1), users with an Azure Active Directory browser sign-in will see the Office 365 feed experience on the new tab page.

If you disable or don't configure this policy:

- Users with an Azure Active Directory browser sign-in are offered the Office 365 new tab page feed experience, as well as the standard new tab page feed experience.

- Users without an Azure Active Directory browser sign-in will see the standard new tab page experience.

If you configure this policy *and* the [NewTabPageLocation](#newtabpagelocation) policy, [NewTabPageLocation](#newtabpagelocation) has precedence.

Default setting:  Disabled or not configured.

* 0 = Microsoft News feed experience

* 1 = Office 365 feed experience

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 예
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  정수

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: NewTabPageSetFeedType
  - GP 이름: Configure the Microsoft Edge new tab page experience
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/시작, 홈 페이지 및 새 탭 페이지
  - GP 경로 (맞춤): 관리 템플릿/Microsoft Edge - 기본 설정(사용자가 재정의할 수 없음)/시작, 홈 페이지 및 새 탭 페이지
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): SOFTWARE\Policies\Microsoft\Edge\맞춤
  - 값 이름: NewTabPageSetFeedType
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000000
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: NewTabPageSetFeedType
  - 예제 값:
``` xml
<integer>0</integer>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### RestoreOnStartup
  #### 시작 시 수행할 작업
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  시작 시 Microsoft Edge의 동작 방식을 지정합니다.

시작 시 항상 새 탭이 열리도록 하려면 '새 탭 열기'(5)를 선택하세요.

Microsoft Edge 마지막으로 열린 URL을 다시 열려면 '마지막 세션 복원' (1)을 선택하세요. 검색 세션이 그대로 복원됩니다. 이 옵션은 세션에 의존하거나 종료 시 작업을 수행하는 일부 설정(예: 종료 시 검색 데이터 지우기 또는 세션 전용 쿠키)을 사용 중지합니다.

특정 URL 집합을 열려면 'URL 목록 열기'(4)를 선택하세요.

이 설정을 사용하지 않으면 구성되지 않은 상태로 유지되는 것과 같습니다. 사용자는 Microsoft Edge에서 변경할 수 있습니다.

이 정책은 Microsoft Active Directory 도메인에 가입된 Windows 인스턴스 또는 장치 관리를 위해 등록된 Windows 10 Pro나 Enterprise 인스턴스에서만 사용할 수 있습니다.

* 5 = 새 탭 열기

* 1 = 마지막 세션 복원

* 4 = URL 목록 열기

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 예
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  정수

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: RestoreOnStartup
  - GP 이름: 시작 시 수행할 작업
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/시작, 홈 페이지 및 새 탭 페이지
  - GP 경로 (맞춤): 관리 템플릿/Microsoft Edge - 기본 설정(사용자가 재정의할 수 없음)/시작, 홈 페이지 및 새 탭 페이지
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): SOFTWARE\Policies\Microsoft\Edge\맞춤
  - 값 이름: RestoreOnStartup
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000004
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: RestoreOnStartup
  - 예제 값:
``` xml
<integer>4</integer>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### RestoreOnStartupURLs
  #### 브라우저가 시작될 때 열 사이트
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  Specify a list of websites to open automatically when the browser starts. If you don't configure this policy, no site is opened on startup.

This policy only works if you also set the [RestoreOnStartup](#restoreonstartup) policy to 'Open a list of URLs' (4).

This policy is only available on Windows instances that are joined to a Microsoft Active Directory domain or Windows 10 Pro or Enterprise instances that are enrolled for device management.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 예
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  문자열 목록

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: RestoreOnStartupURLs
  - GP 이름: 브라우저가 시작될 때 열 사이트
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/시작, 홈 페이지 및 새 탭 페이지
  - GP 경로 (맞춤): 관리 템플릿/Microsoft Edge - 기본 설정(사용자가 재정의할 수 없음)/시작, 홈 페이지 및 새 탭 페이지
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge\RestoreOnStartupURLs
  - 경로 (맞춤): SOFTWARE\Policies\Microsoft\Edge\맞춤\RestoreOnStartupURLs
  - 값 이름: 1, 2, 3, ...
  - 값 형식: REG_SZ 목록
  ##### 예제 값:
```
SOFTWARE\Policies\Microsoft\Edge\RestoreOnStartupURLs\0 = "https://contoso.com"
SOFTWARE\Policies\Microsoft\Edge\RestoreOnStartupURLs\1 = "https://www.fabrikam.com"

```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: RestoreOnStartupURLs
  - 예제 값:
``` xml
<array>
  <string>https://contoso.com</string>
  <string>https://www.fabrikam.com</string>
</array>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### ShowHomeButton
  #### 도구 모음에 홈 버튼 표시
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  Microsoft Edge의 도구 모음에 홈 버튼을 표시합니다.

항상 홈 버튼을 표시하려면 이 정책을 사용합니다. 버튼을 표시하지 않으려면 사용하지 않도록 설정화합니다.

정책을 구성하지 않으면 사용자가 홈 버튼을 표시할지 여부를 선택할 수 있습니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 예
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  부울

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: ShowHomeButton
  - GP 이름: 도구 모음에 홈 버튼 표시
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/시작, 홈 페이지 및 새 탭 페이지
  - GP 경로 (맞춤): 관리 템플릿/Microsoft Edge - 기본 설정(사용자가 재정의할 수 없음)/시작, 홈 페이지 및 새 탭 페이지
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): SOFTWARE\Policies\Microsoft\Edge\맞춤
  - 값 이름: ShowHomeButton
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000001
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: ShowHomeButton
  - 예제 값:
``` xml
<true/>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ## 암호 관리자 및 보호 policies

  [맨 위로 이동](#microsoft-edge---정책)

  ### PasswordManagerEnabled
  #### 암호 관리자에 암호 저장 사용
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  Microsoft Edge에서 사용자 암호를 저장하도록 설정합니다.

이 정책을 사용하면 사용자가 Microsoft Edge에서 암호를 저장할 수 있습니다. 다음에 사이트를 방문하면 Microsoft Edge에서 자동으로 암호를 입력합니다.

이 정책을 사용하지 않으면 사용자가 새 암호를 저장할 수 없지만 이전에 저장된 암호를 계속 사용할 수 있습니다.

이 정책을 사용하거나 사용하지 않도록 설정하면 Microsoft Edge에서 사용자가 변경하거나 재정의할 수 없습니다. 구성하지 않으면 사용자가 암호를 저장할 수 있을 뿐만 아니라 이 기능을 끌 수도 있습니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 예
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  부울

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: PasswordManagerEnabled
  - GP 이름: 암호 관리자에 암호 저장 사용
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/암호 관리자 및 보호
  - GP 경로 (맞춤): 관리 템플릿/Microsoft Edge - 기본 설정(사용자가 재정의할 수 없음)/암호 관리자 및 보호
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): SOFTWARE\Policies\Microsoft\Edge\맞춤
  - 값 이름: PasswordManagerEnabled
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000001
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: PasswordManagerEnabled
  - 예제 값:
``` xml
<true/>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### PasswordProtectionChangePasswordURL
  #### 암호 변경 URL 구성
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  암호 변경 URL을 구성합니다(HTTP 및 HTTPS 스키마만 해당).

암호 보호 서비스는 브라우저에서 경고가 표시된 후 사용자를 이 URL로 보내 암호를 변경합니다.

이 정책을 사용하면 암호 보호 서비스가 비밀번호를 변경하기 위해 사용자를 이 URL로 보냅니다.

이 정책을 사용하지 않거나 구성하지 않으면 암호 보호 서비스가 사용자를 암호 변경 URL로 리디렉션하지 않습니다.

이 정책은 Microsoft Active Directory 도메인에 가입된 Windows 인스턴스나 장치 관리를 위해 등록된 Windows 10 Pro 또는 Enterprise 인스턴스에서만 사용할 수 있습니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  문자열

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: PasswordProtectionChangePasswordURL
  - GP 이름: 암호 변경 URL 구성
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/암호 관리자 및 보호
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: PasswordProtectionChangePasswordURL
  - 값 형식: REG_SZ
  ##### 예제 값:
```
"https://contoso.com/change_password.html"
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: PasswordProtectionChangePasswordURL
  - 예제 값:
``` xml
<string>https://contoso.com/change_password.html</string>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### PasswordProtectionLoginURLs
  #### 암호 보호 서비스가 암호의 지문을 캡처해야 하는 엔터프라이즈 로그인 URL 목록 구성
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  Microsoft Edge가 암호의 지문을 캡처하여 암호 재사용 감지에 사용해야 하는 엔터프라이즈 로그인 URL 목록을 구성합니다(HTTP 및 HTTPS 스키마만 해당).

이 정책을 사용하면 암호 보호 서비스가 정의된 URL의 암호 지문을 캡처합니다.

이 정책을 사용하지 않거나 구성하지 않으면 암호 지문을 캡처하지 않습니다.

이 정책은 Microsoft Active Directory도메인에 가입된 Windows 인스턴스 또는 장치 관리를 위해 등록된 Windows 10 Pro나 Enterprise 인스턴스에서만 사용할 수 있습니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  문자열 목록

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: PasswordProtectionLoginURLs
  - GP 이름: 암호 보호 서비스가 암호의 지문을 캡처해야 하는 엔터프라이즈 로그인 URL 목록 구성
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/암호 관리자 및 보호
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge\PasswordProtectionLoginURLs
  - 경로 (맞춤): 해당 없음
  - 값 이름: 1, 2, 3, ...
  - 값 형식: REG_SZ 목록
  ##### 예제 값:
```
SOFTWARE\Policies\Microsoft\Edge\PasswordProtectionLoginURLs\0 = "https://contoso.com/login.html"
SOFTWARE\Policies\Microsoft\Edge\PasswordProtectionLoginURLs\1 = "https://login.contoso.com"

```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: PasswordProtectionLoginURLs
  - 예제 값:
``` xml
<array>
  <string>https://contoso.com/login.html</string>
  <string>https://login.contoso.com</string>
</array>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### PasswordProtectionWarningTrigger
  #### 암호 보호 경고 트리거 구성
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  Allows you to control when to trigger password protection warning. Password protection alerts users when they reuse their protected password on potentially suspicious sites.

You can use the [PasswordProtectionLoginURLs](#passwordprotectionloginurls) and [PasswordProtectionChangePasswordURL](#passwordprotectionchangepasswordurl) policies to configure which passwords to protect.

Exemptions: Passwords for the sites listed in [PasswordProtectionLoginURLs](#passwordprotectionloginurls) and [PasswordProtectionChangePasswordURL](#passwordprotectionchangepasswordurl), as well as for the sites listed in [SmartScreenAllowListDomains](#smartscreenallowlistdomains), will not trigger a password-protection warning.

Set to 'PasswordProtectionWarningOff' (0) to not show password protection warningss.

Set to 'PasswordProtectionWarningOnPasswordReuse' (1) to show password protection warnings when the user reuses their protected password on a non-whitelisted site.

If you disable or don't configure this policy, then the warning trigger is not shown.

* 0 = Password protection warning is off.

* 1 = Password protection warning is triggered by password reuse.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  정수

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: PasswordProtectionWarningTrigger
  - GP 이름: 암호 보호 경고 트리거 구성
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/암호 관리자 및 보호
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: PasswordProtectionWarningTrigger
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000001
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: PasswordProtectionWarningTrigger
  - 예제 값:
``` xml
<integer>1</integer>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ## 인쇄 중 policies

  [맨 위로 이동](#microsoft-edge---정책)

  ### DefaultPrinterSelection
  #### 기본 프린터 선택 규칙
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  Microsoft Edge 기본 프린터 선택 규칙을 재정의합니다. 이 정책은 Microsoft Edge에서 사용자가 페이지를 처음 인쇄하려고 할 때 발생하는 기본 프린터를 선택하는 규칙을 결정합니다.

이 정책을 설정하면 Microsoft Edge는 지정된 모든 특성과 일치하는 프린터를 찾으려고 시도하고 기본 프린터로 사용합니다. 기준을 충족하는 프린터가 여러 개인 경우에는 일치하는 첫 번째 프린터가 사용됩니다.

이 정책을 구성하지 않거나 제한 시간 내에 일치하는 프린터가 발견되지 않으면 기본 제공 PDF 프린터 또는 프린터 없음(PDF 프린터를 사용할 수 없는 경우)이 프린터의 기본값으로 설정됩니다.

값은 다음과 같은 스키마를 준수하는 JSON 개체로 구문 분석됩니다. - { "type": "object", "properties": { "idPattern": { "description": "Regular expression to match printer id.", "type": "string" }, "namePattern": { "description": "Regular expression to match printer display name.", "type": "string" } } }

필드를 생략하면 모든 값이 일치함을 의미합니다. 예를 들어 연결을 지정하지 않으면 인쇄 미리 보기가 모든 종류의 로컬 프린터를 검색하기 시작합니다. 정규식 패턴은 JavaScript RegExp 구문을 따라야 하며 일치하는 항목은 대/소문자를 구분합니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  문자열

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: DefaultPrinterSelection
  - GP 이름: 기본 프린터 선택 규칙
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/인쇄 중
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: DefaultPrinterSelection
  - 값 형식: REG_SZ
  ##### 예제 값:
```
"{ "idPattern": ".*public", "namePattern": ".*Color" }"
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: DefaultPrinterSelection
  - 예제 값:
``` xml
<string>{ "idPattern": ".*public", "namePattern": ".*Color" }</string>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### PrintHeaderFooter
  #### 머리글 및 바닥글 인쇄
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  인쇄 대화 상자에서 '머리글 및 바닥글'을 강제로 켜거나 끌 수 있습니다.

이 정책을 구성하지 않으면 사용자가 머리글 및 바닥글을 인쇄할지 여부를 결정할 수 있습니다.

이 정책을 사용하지 않으면 사용자가 머리글 및 바닥글을 인쇄할 수 없습니다.

이 정책을 사용하면 사용자가 머리글 및 바닥글을 항상 인쇄합니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 예
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  부울

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: PrintHeaderFooter
  - GP 이름: 머리글 및 바닥글 인쇄
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/인쇄 중
  - GP 경로 (맞춤): 관리 템플릿/Microsoft Edge - 기본 설정(사용자가 재정의할 수 없음)/인쇄 중
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): SOFTWARE\Policies\Microsoft\Edge\맞춤
  - 값 이름: PrintHeaderFooter
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000000
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: PrintHeaderFooter
  - 예제 값:
``` xml
<false/>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### PrintPreviewUseSystemDefaultPrinter
  #### 시스템 기본 프린터를 기본 프린터로 설정
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  Microsoft Edge가 가장 최근에 사용한 프린터 대신 인쇄 미리보기에서 시스템 기본 프린터를 기본 선택으로 사용하도록 지시합니다.

이 정책을 사용하지 않거나 구성하지 않으면 인쇄 미리보기에서 가장 최근에 사용한 프린터를 기본값으로 사용합니다.

이 정책을 사용하면 인쇄 미리보기에서 OS 시스템 기본 프린터를 기본 대상으로 선택합니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 예
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  부울

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: PrintPreviewUseSystemDefaultPrinter
  - GP 이름: 시스템 기본 프린터를 기본 프린터로 설정
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/인쇄 중
  - GP 경로 (맞춤): 관리 템플릿/Microsoft Edge - 기본 설정(사용자가 재정의할 수 없음)/인쇄 중
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): SOFTWARE\Policies\Microsoft\Edge\맞춤
  - 값 이름: PrintPreviewUseSystemDefaultPrinter
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000000
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: PrintPreviewUseSystemDefaultPrinter
  - 예제 값:
``` xml
<false/>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### PrintingEnabled
  #### 인쇄 사용
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  Microsoft Edge에서 인쇄를 사용하도록 설정하고 사용자가 이 설정을 변경할 수 없게 합니다.

이 정책을 사용하거나 구성하지 않으면 사용자가 인쇄할 수 있습니다.

이 정책을 사용하지 않으면 사용자가 Microsoft Edge에서 인쇄를 할 수 없습니다. 공구 모양 메뉴, 확장, JavaScript 응용 프로그램 등에서 인쇄 기능을 사용할 수 없습니다. 사용자는 인쇄하는 동안 Microsoft Edge를 무시하는 플러그 인에서 계속 인쇄할 수 있습니다. 예를 들어 특정 Adobe Flash 응용 프로그램은 상황에 맞는 메뉴에 이 정책에서 다루지 않는 인쇄 옵션이 있습니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  부울

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: PrintingEnabled
  - GP 이름: 인쇄 사용
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/인쇄 중
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: PrintingEnabled
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000001
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: PrintingEnabled
  - 예제 값:
``` xml
<true/>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### UseSystemPrintDialog
  #### 시스템 대화 상자를 사용하여 인쇄
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  인쇄 미리보기 대신 시스템 인쇄 대화 상자를 표시합니다.

이 정책을 사용하면 Microsoft Edge는 사용자가 페이지를 인쇄할 때 기본 제공되는 인쇄 미리 보기 대신 시스템 인쇄 대화 상자를 엽니다.

이 정책을 구성하지 않거나 사용하지 않으면 인쇄 명령이 Microsoft Edge 인쇄 미리 보기 화면을 트리거합니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 아니요 - 브라우저 다시 시작 필요

  #### 데이터 형식:
  부울

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: UseSystemPrintDialog
  - GP 이름: 시스템 대화 상자를 사용하여 인쇄
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/인쇄 중
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: UseSystemPrintDialog
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000000
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: UseSystemPrintDialog
  - 예제 값:
``` xml
<false/>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ## 콘텐츠 설정 policies

  [맨 위로 이동](#microsoft-edge---정책)

  ### AutoSelectCertificateForUrls
  #### 이 사이트에 대한 클라이언트 인증서 자동 선택
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  Specify a list of sites, based on URL patterns, for which Microsoft Edge should automatically select a client certificate, if the site requests one.

The value must be an array of stringified JSON dictionaries. Each dictionary must have the form { "pattern": "$URL_PATTERN", "filter" : $FILTER }, where $URL_PATTERN is a content setting pattern. $FILTER restricts from which client certificates the browser will automatically select. Independent of the filter, only certificates will be selected that match the server's certificate request. For example, if $FILTER has the form { "ISSUER": { "CN": "$ISSUER_CN" } }, additionally only client certificates are selected that are issued by a certificate with the CommonName $ISSUER_CN. If $FILTER contains an "ISSUER" and a "SUBJECT" section, a client certificate must satisfy both conditions to be selected. If $FILTER specifies an organization ("O"), a certificate must have at least one organization which matches the specified value to be selected. If $FILTER specifies an organization unit ("OU"), a certificate must have at least one organization unit which matches the specified value to be selected. If $FILTER is the empty dictionary {}, the selection of client certificates is not additionally restricted.

If you don't configure this policy, auto-selection isn't done for any site.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  문자열 목록

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: AutoSelectCertificateForUrls
  - GP 이름: 이 사이트에 대한 클라이언트 인증서 자동 선택
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/콘텐츠 설정
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge\AutoSelectCertificateForUrls
  - 경로 (맞춤): 해당 없음
  - 값 이름: 1, 2, 3, ...
  - 값 형식: REG_SZ 목록
  ##### 예제 값:
```
SOFTWARE\Policies\Microsoft\Edge\AutoSelectCertificateForUrls\0 = "{"pattern":"https://www.contoso.com","filter":{"ISSUER":{"CN":"certificate issuer name", "L": "certificate issuer location", "O": "certificate issuer org", "OU": "certificate issuer org unit"}, "SUBJECT":{"CN":"certificate subject name", "L": "certificate subject location", "O": "certificate subject org", "OU": "certificate subject org unit"}}}"

```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: AutoSelectCertificateForUrls
  - 예제 값:
``` xml
<array>
  <string>{"pattern":"https://www.contoso.com","filter":{"ISSUER":{"CN":"certificate issuer name", "L": "certificate issuer location", "O": "certificate issuer org", "OU": "certificate issuer org unit"}, "SUBJECT":{"CN":"certificate subject name", "L": "certificate subject location", "O": "certificate subject org", "OU": "certificate subject org unit"}}}</string>
</array>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### CookiesAllowedForUrls
  #### 특정 사이트에서 쿠키 허용
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  Define a list of sites, based on URL patterns, that are allowed to set cookies.

If you don't configure this policy, the global default value from the [DefaultCookiesSetting](#defaultcookiessetting) policy (if set) or the user's personal configuration is used for all sites.

See the [CookiesBlockedForUrls](#cookiesblockedforurls) and [CookiesSessionOnlyForUrls](#cookiessessiononlyforurls) policies for more information.

Note there cannot be conflicting URL patterns set between these three policies:

- [CookiesBlockedForUrls](#cookiesblockedforurls)

- CookiesAllowedForUrls

- [CookiesSessionOnlyForUrls](#cookiessessiononlyforurls)

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  문자열 목록

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: CookiesAllowedForUrls
  - GP 이름: 특정 사이트에서 쿠키 허용
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/콘텐츠 설정
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge\CookiesAllowedForUrls
  - 경로 (맞춤): 해당 없음
  - 값 이름: 1, 2, 3, ...
  - 값 형식: REG_SZ 목록
  ##### 예제 값:
```
SOFTWARE\Policies\Microsoft\Edge\CookiesAllowedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\CookiesAllowedForUrls\1 = "[*.]contoso.edu"

```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: CookiesAllowedForUrls
  - 예제 값:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### CookiesBlockedForUrls
  #### 특정 사이트에서 쿠키 차단
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  Define a list of sites, based on URL patterns, that can't set cookies.

If you don't configure this policy, the global default value from the [DefaultCookiesSetting](#defaultcookiessetting) policy (if set) or the user's personal configuration is used for all sites.

See the [CookiesAllowedForUrls](#cookiesallowedforurls) and [CookiesSessionOnlyForUrls](#cookiessessiononlyforurls) policies for more information.

Note there cannot be conflicting URL patterns set between these three policies:

- CookiesBlockedForUrls

- [CookiesAllowedForUrls](#cookiesallowedforurls)

- [CookiesSessionOnlyForUrls](#cookiessessiononlyforurls)

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  문자열 목록

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: CookiesBlockedForUrls
  - GP 이름: 특정 사이트에서 쿠키 차단
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/콘텐츠 설정
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge\CookiesBlockedForUrls
  - 경로 (맞춤): 해당 없음
  - 값 이름: 1, 2, 3, ...
  - 값 형식: REG_SZ 목록
  ##### 예제 값:
```
SOFTWARE\Policies\Microsoft\Edge\CookiesBlockedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\CookiesBlockedForUrls\1 = "[*.]contoso.edu"

```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: CookiesBlockedForUrls
  - 예제 값:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### CookiesSessionOnlyForUrls
  #### 특정 웹 사이트의 쿠키를 현재 세션으로 제한
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  Cookies created by websites that match a URL pattern you define are deleted when the session ends (when the window closes).

Cookies created by websites that don't match the pattern are controlled by the [DefaultCookiesSetting](#defaultcookiessetting) policy (if set) or by the user's personal configuration. This is also the default behavior if you don't configure this policy.

If Microsoft Edge is running in background mode, the session might not close when the last window is closed, meaning the cookies won't be cleared when the window closes. See the [BackgroundModeEnabled](#backgroundmodeenabled) policy for information about configuring what happens when Microsoft Edge runs in background mode.

You can also use the [CookiesAllowedForUrls](#cookiesallowedforurls) and [CookiesBlockedForUrls](#cookiesblockedforurls) policies to control which websites can create cookies.

Note there cannot be conflicting URL patterns set between these three policies:

- [CookiesBlockedForUrls](#cookiesblockedforurls)

- [CookiesAllowedForUrls](#cookiesallowedforurls)

- CookiesSessionOnlyForUrls

If you set the [RestoreOnStartup](#restoreonstartup) policy to restore URLs from previous sessions, this policy is ignored, and cookies are stored permanently for those sites.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  문자열 목록

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: CookiesSessionOnlyForUrls
  - GP 이름: 특정 웹 사이트의 쿠키를 현재 세션으로 제한
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/콘텐츠 설정
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge\CookiesSessionOnlyForUrls
  - 경로 (맞춤): 해당 없음
  - 값 이름: 1, 2, 3, ...
  - 값 형식: REG_SZ 목록
  ##### 예제 값:
```
SOFTWARE\Policies\Microsoft\Edge\CookiesSessionOnlyForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\CookiesSessionOnlyForUrls\1 = "[*.]contoso.edu"

```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: CookiesSessionOnlyForUrls
  - 예제 값:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### DefaultCookiesSetting
  #### 쿠키 구성
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  Control whether websites can create cookies on the user's device. This policy is all or nothing - you can let all websites create cookies, or no websites create cookies. You can't use this policy to enable cookies from specific websites.

Set the policy to 'SessionOnly' (4) to clear cookies when the session closes. If Microsoft Edge is running in background mode, the session might not close when the last window is closed, meaning the cookies won't be cleared when the window closes. See [BackgroundModeEnabled](#backgroundmodeenabled) policy for information about configuring what happens when Microsoft Edge runs in background mode.

If you don't configure this policy, the default 'AllowCookies' (1) is used, and users can change this setting in Microsoft Edge Settings. (If you don't want users to be able to change this setting, set the policy.)

* 1 = Let all sites create cookies

* 2 = Don't let any site create cookies

* 4 = Keep cookies for the duration of the session

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  정수

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: DefaultCookiesSetting
  - GP 이름: 쿠키 구성
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/콘텐츠 설정
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: DefaultCookiesSetting
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000001
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: DefaultCookiesSetting
  - 예제 값:
``` xml
<integer>1</integer>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### DefaultGeolocationSetting
  #### 기본 지리적 위치 설정
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  웹 사이트가 사용자의 실제 위치를 추적 할 수 있는지 여부를 설정합니다. 기본값으로 추적을 허용하거나 (1) 기본값으로 거부 (2)하거나 웹 사이트에서 위치를 요청할 때마다 사용자에게 물어볼 수 있습니다 (3).

이 정책을 구성하지 않으면 'AskGeolocation'정책이 사용되며 사용자가 정책을 변경할 수 있습니다.

* 1 = 사이트가 사용자의 실제 위치를 추적하도록 허용

* 2 = 모든 사이트가 사용자의 실제 위치를 추적하도록 허용 안 함

* 3 = 사이트에서 사용자의 실제 위치를 추적하려고 할 때마다 물어보기

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  정수

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: DefaultGeolocationSetting
  - GP 이름: 기본 지리적 위치 설정
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/콘텐츠 설정
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: DefaultGeolocationSetting
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000001
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: DefaultGeolocationSetting
  - 예제 값:
``` xml
<integer>1</integer>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### DefaultImagesSetting
  #### 기본 이미지 설정
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  웹 사이트에서 이미지를 표시 할 수 있는지 여부를 설정합니다. 모든 사이트에서 이미지를 허용하거나 (1) 모든 사이트에서 차단할 수 있습니다 (2).

이 정책을 구성하지 않으면 이미지가 기본값으로 허용되며 사용자가 이 설정을 변경할 수 있습니다.

* 1 = 모든 사이트에서 모든 이미지를 표시하도록 허용

* 2 = 모든 사이트에서 이미지를 표시하도록 허용 안 함

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  정수

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: DefaultImagesSetting
  - GP 이름: 기본 이미지 설정
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/콘텐츠 설정
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: DefaultImagesSetting
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000001
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: DefaultImagesSetting
  - 예제 값:
``` xml
<integer>1</integer>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### DefaultJavaScriptSetting
  #### 기본 JavaScript 설정
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  웹 사이트에서 JavaScript를 실행할 수 있는지 여부를 설정합니다. 모든 사이트에서 허용하거나 (1) 모든 사이트에서 차단할 수 있습니다 (2).

이 정책을 구성하지 않으면 모든 사이트에서 기본값으로 JavaScript를 실행할 수 있고 사용자는 이 설정을 변경할 수 있습니다.

* 1 = 모든 사이트에서 JavaScript 실행 허용

* 2 = 모든 사이트에서 JavaScript 실행 허용 안 함

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  정수

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: DefaultJavaScriptSetting
  - GP 이름: 기본 JavaScript 설정
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/콘텐츠 설정
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: DefaultJavaScriptSetting
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000001
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: DefaultJavaScriptSetting
  - 예제 값:
``` xml
<integer>1</integer>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### DefaultNotificationsSetting
  #### 기본 알림 설정
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  웹 사이트에서 바탕 화면 알림을 표시할 수 있는지 여부를 설정합니다. 기본값으로 허용 (1)하거나, 기본값으로 거부 (2)하거나, 웹 사이트에서 알림을 표시하려고 할 때마다 사용자에게 물어보도록(3) 할 수 있습니다.

이 정책을 구성하지 않으면 기본적으로 알림이 허용되며 사용자가 이 설정을 변경할 수 있습니다.

* 1 = 사이트에 바탕 화면 알림 표시 허용

* 2 = 사이트에 바탕 화면 알림 표시 안 함

* 3 = 사이트에서 바탕 화면 알림을 표시하려고 할 때마다 확인

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  정수

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: DefaultNotificationsSetting
  - GP 이름: 기본 알림 설정
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/콘텐츠 설정
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: DefaultNotificationsSetting
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000002
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: DefaultNotificationsSetting
  - 예제 값:
``` xml
<integer>2</integer>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### DefaultPluginsSetting
  #### 기본 Adobe Flash 설정
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  Determines whether websites that aren't covered by [PluginsAllowedForUrls](#pluginsallowedforurls) or [PluginsBlockedForUrls](#pluginsblockedforurls) can automatically run the Adobe Flash plug-in. You can select 'BlockPlugins' (2) to block Adobe Flash on all sites, or you can select 'ClickToPlay' (3) to let Adobe Flash run but require the user to click the placeholder to start it. In any case, the [PluginsAllowedForUrls](#pluginsallowedforurls) and [PluginsBlockedForUrls](#pluginsblockedforurls) policies take precedence over 'DefaultPluginsSetting'.

Automatic playback is only allowed for domains explicitly listed in the [PluginsAllowedForUrls](#pluginsallowedforurls) policy. If you want to enable automatic playback for all sites, consider adding http://* and https://* to this list.

If you don't configure this policy, the user can change this setting manually.

* 2 = Block the Adobe Flash plug-in

* 3 = Click to play

The former '1' option set allow-all, but this functionality is now only handled by the [PluginsAllowedForUrls](#pluginsallowedforurls) policy.  Existing policies using '1' will operate in Click-to-play mode.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  정수

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: DefaultPluginsSetting
  - GP 이름: 기본 Adobe Flash 설정
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/콘텐츠 설정
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: DefaultPluginsSetting
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000002
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: DefaultPluginsSetting
  - 예제 값:
``` xml
<integer>2</integer>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### DefaultPopupsSetting
  #### 기본 팝업 창 설정
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  웹 사이트에서 팝업 창을 표시 할 수 있는지 여부를 설정합니다. 모든 웹 사이트에서 허용하거나 (1) 모든 사이트에서 차단할 수 있습니다 (2).

정책을 구성하지 않으면 팝업 창이 기본적으로 차단되고 사용자가 이 설정을 변경할 수 있습니다.

* 1 = 모모든 사이트에 팝업 표시 허용

* 2 = 모든 사이트에 팝업 표시 허용

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  정수

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: DefaultPopupsSetting
  - GP 이름: 기본 팝업 창 설정
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/콘텐츠 설정
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: DefaultPopupsSetting
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000001
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: DefaultPopupsSetting
  - 예제 값:
``` xml
<integer>1</integer>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### DefaultWebBluetoothGuardSetting
  #### Bluetooth 웹 API의 사용 제어
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  웹 사이트에서 근처의 Bluetooth 장치에 액세스할 수 있는지 여부를 제어합니다. 액세스를 완전히 차단하거나 사이트에서 Bluetooth 장치에 액세스하려고 할 때마다 사용자에게 묻도록 요구할 수 있습니다.

이 정책을 구성하지 않으면 기본값(3, 매번 사용자에게 묻는 메시지를 표시함)이 사용되며 사용자가 변경할 수 있습니다.

* 2 = 모든 사이트에서 웹 Bluetooth API를 사용하여 Bluetooth 장치에 대한 액세스를 요청하는 것을 허용 안 함

* 3 = 사이트에서 근처의 Bluetooth 장치에 대한 액세스 권한을 사용자에게 요청하는 것을 허용

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  정수

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: DefaultWebBluetoothGuardSetting
  - GP 이름: Bluetooth 웹 API의 사용 제어
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/콘텐츠 설정
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: DefaultWebBluetoothGuardSetting
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000002
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: DefaultWebBluetoothGuardSetting
  - 예제 값:
``` xml
<integer>2</integer>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### DefaultWebUsbGuardSetting
  #### WebUSB API의 사용 제어
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  Set whether websites can access connected USB devices. You can completely block access or ask the user each time a website wants to get access to connected USB devices.

You can override this policy for specific URL patterns by using the [WebUsbAskForUrls](#webusbaskforurls) and [WebUsbBlockedForUrls](#webusbblockedforurls) policies.

If you don't configure this policy, sites can ask users whether they can access the connected USB devices (3) by default, and users can change this setting.

* 2 = Don't allow any site to request access to USB devices via the WebUSB API

* 3 = Allow sites to ask the user to grant access to a connected USB device

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  정수

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: DefaultWebUsbGuardSetting
  - GP 이름: WebUSB API의 사용 제어
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/콘텐츠 설정
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: DefaultWebUsbGuardSetting
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000002
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: DefaultWebUsbGuardSetting
  - 예제 값:
``` xml
<integer>2</integer>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### ImagesAllowedForUrls
  #### 이 사이트의 이미지 허용
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  Define a list of sites, based on URL patterns, that can display images.

If you don't configure this policy, the global default value is used for all sites either from the [DefaultImagesSetting](#defaultimagessetting) policy (if set) or the user's personal configuration.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  문자열 목록

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: ImagesAllowedForUrls
  - GP 이름: 이 사이트의 이미지 허용
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/콘텐츠 설정
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge\ImagesAllowedForUrls
  - 경로 (맞춤): 해당 없음
  - 값 이름: 1, 2, 3, ...
  - 값 형식: REG_SZ 목록
  ##### 예제 값:
```
SOFTWARE\Policies\Microsoft\Edge\ImagesAllowedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\ImagesAllowedForUrls\1 = "[*.]contoso.edu"

```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: ImagesAllowedForUrls
  - 예제 값:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### ImagesBlockedForUrls
  #### 특정 사이트에서 이미지 차단
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  Define a list of sites, based on URL patterns, that aren't allowed to display images.

If you don't configure this policy, the global default value from the [DefaultImagesSetting](#defaultimagessetting) policy (if set) or the user's personal configuration is used for all sites.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  문자열 목록

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: ImagesBlockedForUrls
  - GP 이름: 특정 사이트에서 이미지 차단
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/콘텐츠 설정
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge\ImagesBlockedForUrls
  - 경로 (맞춤): 해당 없음
  - 값 이름: 1, 2, 3, ...
  - 값 형식: REG_SZ 목록
  ##### 예제 값:
```
SOFTWARE\Policies\Microsoft\Edge\ImagesBlockedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\ImagesBlockedForUrls\1 = "[*.]contoso.edu"

```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: ImagesBlockedForUrls
  - 예제 값:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### JavaScriptAllowedForUrls
  #### 특정 사이트에서 JavaScript 허용
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  Define a list of sites, based on URL patterns, that are allowed to run JavaScript.

If you don't configure this policy, the global default value from the [DefaultJavaScriptSetting](#defaultjavascriptsetting) policy (if set) or the user's personal configuration is used for all sites.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  문자열 목록

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: JavaScriptAllowedForUrls
  - GP 이름: 특정 사이트에서 JavaScript 허용
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/콘텐츠 설정
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge\JavaScriptAllowedForUrls
  - 경로 (맞춤): 해당 없음
  - 값 이름: 1, 2, 3, ...
  - 값 형식: REG_SZ 목록
  ##### 예제 값:
```
SOFTWARE\Policies\Microsoft\Edge\JavaScriptAllowedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\JavaScriptAllowedForUrls\1 = "[*.]contoso.edu"

```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: JavaScriptAllowedForUrls
  - 예제 값:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### JavaScriptBlockedForUrls
  #### 특정 사이트에서 JavaScript 차단
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  Define a list of sites, based on URL patterns, that aren't allowed to run JavaScript.

If you don't configure this policy, the global default value from the [DefaultJavaScriptSetting](#defaultjavascriptsetting) policy (if set) or the user's personal configuration is used for all sites.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  문자열 목록

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: JavaScriptBlockedForUrls
  - GP 이름: 특정 사이트에서 JavaScript 차단
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/콘텐츠 설정
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge\JavaScriptBlockedForUrls
  - 경로 (맞춤): 해당 없음
  - 값 이름: 1, 2, 3, ...
  - 값 형식: REG_SZ 목록
  ##### 예제 값:
```
SOFTWARE\Policies\Microsoft\Edge\JavaScriptBlockedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\JavaScriptBlockedForUrls\1 = "[*.]contoso.edu"

```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: JavaScriptBlockedForUrls
  - 예제 값:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### NotificationsAllowedForUrls
  #### 특정 사이트에서 알림 허용
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  Define a list of sites, based on URL patterns, that can display notifications.

If you don't configure this policy, the global default value from the [DefaultNotificationsSetting](#defaultnotificationssetting) policy (if set) or the user's personal configuration is used for all sites.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  문자열 목록

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: NotificationsAllowedForUrls
  - GP 이름: 특정 사이트에서 알림 허용
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/콘텐츠 설정
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge\NotificationsAllowedForUrls
  - 경로 (맞춤): 해당 없음
  - 값 이름: 1, 2, 3, ...
  - 값 형식: REG_SZ 목록
  ##### 예제 값:
```
SOFTWARE\Policies\Microsoft\Edge\NotificationsAllowedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\NotificationsAllowedForUrls\1 = "[*.]contoso.edu"

```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: NotificationsAllowedForUrls
  - 예제 값:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### NotificationsBlockedForUrls
  #### 특정 사이트에서 알림 차단
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  Define a list of sites, based on URL patterns, that are blocked from displaying notifications.

If you don't configure this policy, the global default value from the [DefaultNotificationsSetting](#defaultnotificationssetting) policy (if set) or the user's personal configuration is used for all sites.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  문자열 목록

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: NotificationsBlockedForUrls
  - GP 이름: 특정 사이트에서 알림 차단
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/콘텐츠 설정
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge\NotificationsBlockedForUrls
  - 경로 (맞춤): 해당 없음
  - 값 이름: 1, 2, 3, ...
  - 값 형식: REG_SZ 목록
  ##### 예제 값:
```
SOFTWARE\Policies\Microsoft\Edge\NotificationsBlockedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\NotificationsBlockedForUrls\1 = "[*.]contoso.edu"

```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: NotificationsBlockedForUrls
  - 예제 값:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### PluginsAllowedForUrls
  #### 특정 사이트에서 Adobe Flash 플러그 인 허용
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  Define a list of sites, based on URL patterns, that can run the Adobe Flash plug-in.

If you don't configure this policy, the global default value from the [DefaultPluginsSetting](#defaultpluginssetting) policy (if set) or the user's personal configuration is used for all sites.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  문자열 목록

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: PluginsAllowedForUrls
  - GP 이름: 특정 사이트에서 Adobe Flash 플러그 인 허용
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/콘텐츠 설정
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge\PluginsAllowedForUrls
  - 경로 (맞춤): 해당 없음
  - 값 이름: 1, 2, 3, ...
  - 값 형식: REG_SZ 목록
  ##### 예제 값:
```
SOFTWARE\Policies\Microsoft\Edge\PluginsAllowedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\PluginsAllowedForUrls\1 = "[*.]contoso.edu"

```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: PluginsAllowedForUrls
  - 예제 값:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### PluginsBlockedForUrls
  #### 특정 사이트에서 Adobe Flash 플러그 인 차단
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  Define a list of sites, based on URL patterns, that are blocked from running Adobe Flash.

If you don't configure this policy, the global default value from the [DefaultPluginsSetting](#defaultpluginssetting) policy (if set) or the user's personal configuration is used for all sites.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  문자열 목록

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: PluginsBlockedForUrls
  - GP 이름: 특정 사이트에서 Adobe Flash 플러그 인 차단
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/콘텐츠 설정
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge\PluginsBlockedForUrls
  - 경로 (맞춤): 해당 없음
  - 값 이름: 1, 2, 3, ...
  - 값 형식: REG_SZ 목록
  ##### 예제 값:
```
SOFTWARE\Policies\Microsoft\Edge\PluginsBlockedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\PluginsBlockedForUrls\1 = "[*.]contoso.edu"

```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: PluginsBlockedForUrls
  - 예제 값:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### PopupsAllowedForUrls
  #### 특정 사이트에서 팝업 창 허용
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  Define a list of sites, based on URL patterns, that can open pop-up windows.

If you don't configure this policy, the global default value from the [DefaultPopupsSetting](#defaultpopupssetting) policy (if set) or the user's personal configuration is used for all sites.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  문자열 목록

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: PopupsAllowedForUrls
  - GP 이름: 특정 사이트에서 팝업 창 허용
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/콘텐츠 설정
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge\PopupsAllowedForUrls
  - 경로 (맞춤): 해당 없음
  - 값 이름: 1, 2, 3, ...
  - 값 형식: REG_SZ 목록
  ##### 예제 값:
```
SOFTWARE\Policies\Microsoft\Edge\PopupsAllowedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\PopupsAllowedForUrls\1 = "[*.]contoso.edu"

```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: PopupsAllowedForUrls
  - 예제 값:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### PopupsBlockedForUrls
  #### 특정 사이트에서 팝업 창 차단
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  Define a list of sites, based on URL patterns, that are blocked from opening pop-up windows.

If you don't configure this policy, the global default value from the [DefaultPopupsSetting](#defaultpopupssetting) policy (if set) or the user's personal configuration is used for all sites.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  문자열 목록

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: PopupsBlockedForUrls
  - GP 이름: 특정 사이트에서 팝업 창 차단
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/콘텐츠 설정
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge\PopupsBlockedForUrls
  - 경로 (맞춤): 해당 없음
  - 값 이름: 1, 2, 3, ...
  - 값 형식: REG_SZ 목록
  ##### 예제 값:
```
SOFTWARE\Policies\Microsoft\Edge\PopupsBlockedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\PopupsBlockedForUrls\1 = "[*.]contoso.edu"

```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: PopupsBlockedForUrls
  - 예제 값:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### RegisteredProtocolHandlers
  #### 프로토콜 처리기 등록
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  프로토콜 처리기 목록을 등록합니다. 프로토콜 속성을 스키마(예: 'mailto')로 설정하고 URL 속성을 스키마를 처리하는 응용 프로그램의 URL 패턴으로 설정합니다. 이 패턴에는 처리된 URL로 대체되는 '%s'이(가) 포함될 수 있습니다.

이 정책에 대해 특정 값을 권장할 수 있지만 사용자가 이를 사용하도록 요구할 수는 없습니다.

정책에 의해 등록된 프로토콜 처리기가 사용자가 등록한 처리기와 병합되며 둘 다 사용할 수 있습니다. 사용자는 새 기본 처리기를 설치하여 정책에 의해 등록된 프로토콜 처리기를 재정의할 수는 있지만 정책에 의해 등록된 프로토콜 처리기를 제거할 수는 없습니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 아니요
  - 권장될 수 있음: 예
  - 동적 정책 새로 고침: 아니요 - 브라우저 다시 시작 필요

  #### 데이터 형식:
  사전

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: RegisteredProtocolHandlers
  - GP 이름: 프로토콜 처리기 등록
  - GP 경로 (필수): 해당 없음
  - GP 경로 (맞춤): 관리 템플릿/Microsoft Edge - 기본 설정(사용자가 재정의할 수 없음)/콘텐츠 설정
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): 해당 없음
  - 경로 (맞춤): SOFTWARE\Policies\Microsoft\Edge\맞춤
  - 값 이름: RegisteredProtocolHandlers
  - 값 형식: REG_SZ
  ##### 예제 값:
```
SOFTWARE\Policies\Microsoft\Edge\RegisteredProtocolHandlers = [
  {
    "default": true, 
    "protocol": "mailto", 
    "url": "https://mail.contoso.com/mail/?extsrc=mailto&url=%s"
  }
]
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: RegisteredProtocolHandlers
  - 예제 값:
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
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### WebUsbAllowDevicesForUrls
  #### 특정 USB 장치에 연결하기 위해 특정 사이트에 대한 액세스 권한 부여
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  Allows you to set a list of urls that specify which sites will automatically be granted permission to access a USB device with the given vendor and product IDs. Each item in the list must contain both devices and urls in order for the policy to be valid. Each item in devices can contain a vendor ID and product ID field. Any ID that is omitted is treated as a wildcard with one exception, and that exception is that a product ID cannot be specified without a vendor ID also being specified. Otherwise, the policy will not be valid and will be ignored.

The USB permission model uses the URL of the requesting site ("requesting URL") and the URL of the top-level frame site ("embedding URL") to grant permission to the requesting URL to access the USB device. The requesting URL may be different than the embedding URL when the requesting site is loaded in an iframe. Therefore, the "urls" field can contain up to two URL strings delimited by a comma to specify the requesting and embedding URL respectively. If only one URL is specified, then access to the corresponding USB devices will be granted when the requesting site's URL matches this URL regardless of embedding status. The URLs in "urls" must be valid URLs, otherwise the policy will be ignored.

If this policy is left not set, the global default value will be used for all sites either from the [DefaultWebUsbGuardSetting](#defaultwebusbguardsetting) policy if it is set, or the user's personal configuration otherwise.

URL patterns in this policy should not clash with the ones configured via [WebUsbBlockedForUrls](#webusbblockedforurls). If there is a clash, this policy will take precedence over [WebUsbBlockedForUrls](#webusbblockedforurls) and [WebUsbAskForUrls](#webusbaskforurls).

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  사전

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: WebUsbAllowDevicesForUrls
  - GP 이름: 특정 USB 장치에 연결하기 위해 특정 사이트에 대한 액세스 권한 부여
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/콘텐츠 설정
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: WebUsbAllowDevicesForUrls
  - 값 형식: REG_SZ
  ##### 예제 값:
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


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: WebUsbAllowDevicesForUrls
  - 예제 값:
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
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### WebUsbAskForUrls
  #### 특정 사이트에서 WebUSB 허용
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  Define a list of sites, based on URL patterns, that can ask the user for access to a USB device.

If you don't configure this policy, the global default value from the [DefaultWebUsbGuardSetting](#defaultwebusbguardsetting) policy (if set) or the user's personal configuration is used for all sites.

The URL patterns defined in this policy can't conflict with those configured in the [WebUsbBlockedForUrls](#webusbblockedforurls) policy - you can't both allow and block a URL.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  문자열 목록

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: WebUsbAskForUrls
  - GP 이름: 특정 사이트에서 WebUSB 허용
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/콘텐츠 설정
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge\WebUsbAskForUrls
  - 경로 (맞춤): 해당 없음
  - 값 이름: 1, 2, 3, ...
  - 값 형식: REG_SZ 목록
  ##### 예제 값:
```
SOFTWARE\Policies\Microsoft\Edge\WebUsbAskForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\WebUsbAskForUrls\1 = "[*.]contoso.edu"

```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: WebUsbAskForUrls
  - 예제 값:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### WebUsbBlockedForUrls
  #### 특정 사이트에서 WebUSB 차단
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  Define a list of sites, based on URL patterns, that can't ask the user to grant them access to a USB device.

If you don't configure this policy, the global default value from the [DefaultWebUsbGuardSetting](#defaultwebusbguardsetting) policy (if set) or the user's personal configuration is used for all sites.

URL patterns in this policy can't conflict with those configured in the [WebUsbAskForUrls](#webusbaskforurls) policy. You can't both allow and block a URL.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  문자열 목록

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: WebUsbBlockedForUrls
  - GP 이름: 특정 사이트에서 WebUSB 차단
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/콘텐츠 설정
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge\WebUsbBlockedForUrls
  - 경로 (맞춤): 해당 없음
  - 값 이름: 1, 2, 3, ...
  - 값 형식: REG_SZ 목록
  ##### 예제 값:
```
SOFTWARE\Policies\Microsoft\Edge\WebUsbBlockedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\WebUsbBlockedForUrls\1 = "[*.]contoso.edu"

```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: WebUsbBlockedForUrls
  - 예제 값:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ## 프록시 서버 policies

  [맨 위로 이동](#microsoft-edge---정책)

  ### ProxyBypassList
  #### 프록시 바이패스 규칙 구성
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  Defines a list of hosts for which Microsoft Edge bypasses any proxy.

This policy is applied only if you have selected 'Use fixed proxy servers' in the [ProxyMode](#proxymode) policy. If you selected any other mode for configuring proxy policies, don't enable or configure this policy.

If you enable this policy, you can create a list of hosts for which Microsoft Edge doesn't use a proxy.

If you don't configure this policy, no list of hosts is created for which Microsoft Edge bypasses a proxy. Leave this policy unconfigured if you've specified any other method for setting proxy policies.

For more detailed examples go to [https://go.microsoft.com/fwlink/?linkid=2094936](https://go.microsoft.com/fwlink/?linkid=2094936).

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  문자열

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: ProxyBypassList
  - GP 이름: 프록시 바이패스 규칙 구성
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/프록시 서버
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: ProxyBypassList
  - 값 형식: REG_SZ
  ##### 예제 값:
```
"https://www.contoso.com, https://www.fabrikam.com"
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: ProxyBypassList
  - 예제 값:
``` xml
<string>https://www.contoso.com, https://www.fabrikam.com</string>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### ProxyMode
  #### 프록시 서버 설정 구성
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  Specify the proxy server settings used by Microsoft Edge. If you enable this policy, users can't change the proxy settings.

If you choose to never use a proxy server and to always connect directly, all other options are ignored.

If you choose to use system proxy settings, all other options are ignored.

If you choose to auto detect the proxy server, all other options are ignored.

If you choose fixed server proxy mode, you can specify further options in [ProxyServer](#proxyserver) and 'Comma-separated list of proxy bypass rules'.

If you choose to use a .pac proxy script, you must specify the URL to the script in 'URL to a proxy .pac file'.

For detailed examples, go to [https://go.microsoft.com/fwlink/?linkid=2094936](https://go.microsoft.com/fwlink/?linkid=2094936).

If you enable this policy, Microsoft Edge will ignore all proxy-related options specified from the command line.

If you don't configure this policy users can choose their own proxy settings.

* "direct" = Never use a proxy

* "auto_detect" = Auto detect proxy settings

* "pac_script" = Use a .pac proxy script

* "fixed_servers" = Use fixed proxy servers

* "system" = Use system proxy settings

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  문자열

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: ProxyMode
  - GP 이름: 프록시 서버 설정 구성
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/프록시 서버
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: ProxyMode
  - 값 형식: REG_SZ
  ##### 예제 값:
```
"direct"
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: ProxyMode
  - 예제 값:
``` xml
<string>direct</string>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### ProxyPacUrl
  #### 프록시.pac 파일 URL 설정
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  Specifies the URL for a proxy auto-config (PAC) file.

This policy is applied only if you selected 'Use a .pac proxy script' in the [ProxyMode](#proxymode) policy. If you selected any other mode for configuring proxy policies, don't enable or configure this policy.

If you enable this policy, you can specify the URL for a PAC file, which defines how the browser automatically chooses the appropriate proxy server for fetching a particular website.

If you disable or don't configure this policy, no PAC file is specified. Leave this policy unconfigured if you've specified any other method for setting proxy policies.

For detailed examples, see [https://go.microsoft.com/fwlink/?linkid=2094936](https://go.microsoft.com/fwlink/?linkid=2094936).

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  문자열

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: ProxyPacUrl
  - GP 이름: 프록시.pac 파일 URL 설정
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/프록시 서버
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: ProxyPacUrl
  - 값 형식: REG_SZ
  ##### 예제 값:
```
"https://internal.contoso.com/example.pac"
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: ProxyPacUrl
  - 예제 값:
``` xml
<string>https://internal.contoso.com/example.pac</string>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### ProxyServer
  #### 프록시 서버의 주소 또는 URL 구성
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  Specifies the URL of the proxy server.

This policy is applied only if you have selected 'Use fixed proxy servers' in the [ProxyMode](#proxymode) policy. If you selected any other mode for configuring proxy policies, don't enable or configure this policy.

If you enable this policy, the proxy server configured by this policy will be used for all URLs.

If you disable or don't configure this policy, users can choose their own proxy settings while in this proxy mode. Leave this policy unconfigured if you've specified any other method for setting proxy policies.

For more options and detailed examples, see [https://go.microsoft.com/fwlink/?linkid=2094936](https://go.microsoft.com/fwlink/?linkid=2094936).

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  문자열

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: ProxyServer
  - GP 이름: 프록시 서버의 주소 또는 URL 구성
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/프록시 서버
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: ProxyServer
  - 값 형식: REG_SZ
  ##### 예제 값:
```
"123.123.123.123:8080"
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: ProxyServer
  - 예제 값:
``` xml
<string>123.123.123.123:8080</string>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### ProxySettings
  #### 프록시 설정
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  Configures the proxy settings for Microsoft Edge.

If you enable this policy, Microsoft Edge ignores all proxy-related options specified from the command line.

If you don't configure this policy, users can choose their own proxy settings.

This policy overrides the following individual policies:

[ProxyMode](#proxymode)
[ProxyPacUrl](#proxypacurl)
[ProxyServer](#proxyserver)
[ProxyBypassList](#proxybypasslist)

The ProxyMode field lets you specify the proxy server used by Microsoft Edge and prevents users from changing proxy settings.

The ProxyPacUrl field is a URL to a proxy .pac file.

The ProxyServer field is a URL for the proxy server.

The ProxyBypassList field is a list of proxy hosts that Microsoft Edge bypasses.

If you choose the 'direct' value as 'ProxyMode', a proxy is never used and all other fields are ignored.

If you choose the 'system' value as 'ProxyMode', the systems's proxy is used and all other fields are ignored.

If you choose the 'auto_detect' value as 'ProxyMode', all other fields are ignored.

If you choose the 'fixed_server' value as 'ProxyMode', the 'ProxyServer' and 'ProxyBypassList' fields are used.

If you choose the 'pac_script' value as 'ProxyMode', the 'ProxyPacUrl' and 'ProxyBypassList' fields are used.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  사전

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: ProxySettings
  - GP 이름: 프록시 설정
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/프록시 서버
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: ProxySettings
  - 값 형식: REG_SZ
  ##### 예제 값:
```
SOFTWARE\Policies\Microsoft\Edge\ProxySettings = {
  "ProxyBypassList": "https://www.example1.com,https://www.example2.com,https://internalsite/", 
  "ProxyMode": "direct", 
  "ProxyPacUrl": "https://internal.site/example.pac", 
  "ProxyServer": "123.123.123.123:8080"
}
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: ProxySettings
  - 예제 값:
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
  

  [맨 위로 이동](#microsoft-edge---정책)

  ## 확장 policies

  [맨 위로 이동](#microsoft-edge---정책)

  ### ExtensionAllowedTypes
  #### 허용된 확장 유형 구성
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  Controls which extension types can be installed and limits runtime access.

This setting defines the allowed types of extensions and which hosts they can interact with. The value is a list of strings, each of which should be one of the following: "extension", "theme", "user_script", and "hosted_app". See the Microsoft Edge extensions documentation for more information on these types.

Note that this policy also affects extensions to be force-installed by using [ExtensionInstallForcelist](#extensioninstallforcelist) policy.

If you enable this policy, only extensions that match a type in the list are installed.

If you don't configure this policy, no restrictions on the acceptable extension types are enforced.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  문자열 목록

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: ExtensionAllowedTypes
  - GP 이름: 허용된 확장 유형 구성
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/확장
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge\ExtensionAllowedTypes
  - 경로 (맞춤): 해당 없음
  - 값 이름: 1, 2, 3, ...
  - 값 형식: REG_SZ 목록
  ##### 예제 값:
```
SOFTWARE\Policies\Microsoft\Edge\ExtensionAllowedTypes\0 = "hosted_app"

```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: ExtensionAllowedTypes
  - 예제 값:
``` xml
<array>
  <string>hosted_app</string>
</array>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### ExtensionInstallAllowlist
  #### 특정 확장 설치 허용
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  기본적으로 모든 확장이 허용됩니다. 그러나 'ExtensionInstallBlockList'정책을 "*"로 설정하여 모든 확장을 차단하는 경우 사용자는 이 정책에 정의된 확장만 설치할 수 있습니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  문자열 목록

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: ExtensionInstallAllowlist
  - GP 이름: 특정 확장 설치 허용
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/확장
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallAllowlist
  - 경로 (맞춤): 해당 없음
  - 값 이름: 1, 2, 3, ...
  - 값 형식: REG_SZ 목록
  ##### 예제 값:
```
SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallAllowlist\0 = "extension_id1"
SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallAllowlist\1 = "extension_id2"

```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: ExtensionInstallAllowlist
  - 예제 값:
``` xml
<array>
  <string>extension_id1</string>
  <string>extension_id2</string>
</array>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### ExtensionInstallBlocklist
  #### 설치될 수 없는 확장 제어
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  사용자가 Microsoft Edge에 설치할 수 없는 특정 확장을 나열합니다. 이 정책을 배포하면 이전에 설치된 이 목록의 확장을 사용할 수 없게 되며 사용자는 이러한 확장을 사용하도록 설정할 수 없습니다. 차단된 확장 목록에서 항목을 제거하면 해당 확장은 이전에 설치된 모든 위치에서 자동으로 다시 사용하도록 설정됩니다.

"*"를 사용하여 허용 목록에 명시적으로 나열되지 않은 모든 확장을 차단합니다.

이 정책을 구성하지 않으면 사용자가 Microsoft Edge에 확장을 설치할 수 있습니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  문자열 목록

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: ExtensionInstallBlocklist
  - GP 이름: 설치될 수 없는 확장 제어
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/확장
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallBlocklist
  - 경로 (맞춤): 해당 없음
  - 값 이름: 1, 2, 3, ...
  - 값 형식: REG_SZ 목록
  ##### 예제 값:
```
SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallBlocklist\0 = "extension_id1"
SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallBlocklist\1 = "extension_id2"

```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: ExtensionInstallBlocklist
  - 예제 값:
``` xml
<array>
  <string>extension_id1</string>
  <string>extension_id2</string>
</array>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### ExtensionInstallForcelist
  #### 자동으로 설치되는 확장 제어
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  Specifies extensions that are installed silently, without user interaction, and that the users can't uninstall or disable ("force-installed"). All permissions requested by the extensions are granted implicitly, without user interaction, including any additional permissions requested by future versions of the extension. Furthermore, permissions are granted for the enterprise.deviceAttributes and enterprise.platformKeys extension APIs. (These two APIs are only available to extensions that are force-installed.)

This policy takes precedence over a potentially conflicting [ExtensionInstallBlocklist](#extensioninstallblocklist) policy. When you take an extension off of the force-installed list it's automatically uninstalled by Microsoft Edge.

For Windows devices that aren't joined to a Microsoft Active Directory domain, forced installation is limited to extensions available in the Microsoft Store.

Note that users can modify the source code of any extension by using Developer Tools, potentially rendering the extension dysfunctional. If this is a concern, set the [DeveloperToolsAvailability](#developertoolsavailability) policy.

Use the following format to add an extension to the list:

[extensionID];[updateURL]

- extensionID - the 32-letter string found on edge://extensions when in developer mode.

- updateURL (optional) is the address of the Update Manifest XML document for the app or extension, as described at [https://go.microsoft.com/fwlink/?linkid=2095043](https://go.microsoft.com/fwlink/?linkid=2095043). If you don't set the updateURL, the Microsoft Store update URL is used (currently https://edge.microsoft.com/extensionwebstorebase/v1/crx).  Note that the update URL set in this policy is only used for the initial installation; subsequent updates of the extension use the update URL indicated in the extension's manifest.

For example, gggmmkjegpiggikcnhidnjjhmicpibll;https://edge.microsoft.com/extensionwebstorebase/v1/crx installs the Microsoft Online app from the Microsoft Store "update" URL. For more information about hosting extensions, see: [https://go.microsoft.com/fwlink/?linkid=2095044](https://go.microsoft.com/fwlink/?linkid=2095044).

If you don't configure this policy, no extensions are installed automatically, and users can uninstall any extension in Microsoft Edge.

Note that this policy doesn't apply to InPrivate mode.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  문자열 목록

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: ExtensionInstallForcelist
  - GP 이름: 자동으로 설치되는 확장 제어
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/확장
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallForcelist
  - 경로 (맞춤): 해당 없음
  - 값 이름: 1, 2, 3, ...
  - 값 형식: REG_SZ 목록
  ##### 예제 값:
```
SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallForcelist\0 = "gbchcmhmhahfdphkhkmpfmihenigjmpp;https://edge.microsoft.com/extensionwebstorebase/v1/crx"
SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallForcelist\1 = "abcdefghijklmnopabcdefghijklmnop"

```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: ExtensionInstallForcelist
  - 예제 값:
``` xml
<array>
  <string>gbchcmhmhahfdphkhkmpfmihenigjmpp;https://edge.microsoft.com/extensionwebstorebase/v1/crx</string>
  <string>abcdefghijklmnopabcdefghijklmnop</string>
</array>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### ExtensionInstallSources
  #### 확장 및 사용자 스크립트 설치 원본 구성
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  Define URLs that can install extensions and themes.

By default, users have to download a *.crx file for each extension or script they want to install, and then drag it onto the Microsoft Edge settings page. This policy lets specific URLs use install the extension or script for the user.

Each item in this list is an extension-style match pattern (see [https://go.microsoft.com/fwlink/?linkid=2095039](https://go.microsoft.com/fwlink/?linkid=2095039)). Users can easily install items from any URL that matches an item in this list. Both the location of the *.crx file and the page where the download is started from (in other words, the referrer) must be allowed by these patterns.

The [ExtensionInstallBlocklist](#extensioninstallblocklist) policy takes precedence over this policy. Any extensions that's on the block list won't be installed, even if it comes from a site on this list.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  문자열 목록

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: ExtensionInstallSources
  - GP 이름: 확장 및 사용자 스크립트 설치 원본 구성
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/확장
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallSources
  - 경로 (맞춤): 해당 없음
  - 값 이름: 1, 2, 3, ...
  - 값 형식: REG_SZ 목록
  ##### 예제 값:
```
SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallSources\0 = "https://corp.contoso.com/*"

```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: ExtensionInstallSources
  - 예제 값:
``` xml
<array>
  <string>https://corp.contoso.com/*</string>
</array>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### ExtensionSettings
  #### 확장 관리 설정 구성
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  Microsoft Edge에 대한 확장 관리 설정을 구성합니다.

이 정책은 기존의 확장 관련 정책에 의해 제어되는 설정을 포함하여 여러 설정을 제어합니다. 두 가지 모두가 설정된 경우 이 정책은 기존 정책보다 우선합니다.

이 정책은 확장 ID 또는 업데이트 URL을 해당 구성에 매핑합니다. 확장 ID를 사용하면 구성은 지정된 확장에만 적용됩니다. 특수 ID "*"에 대한 기본 구성을 설정하여 이 정책에 특별히 나열되지 않은 모든 확장에 적용합니다. 업데이트 URL을 사용하면 [https://go.microsoft.com/fwlink/?linkid=2095043](https://go.microsoft.com/fwlink/?linkid=2095043)에서 설명한 대로 이 확장의 매니페스트에 명시된 정확한 업데이트 URL을 가진 모든 확장에 구성이 적용됩니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  사전

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: ExtensionSettings
  - GP 이름: 확장 관리 설정 구성
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/확장
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: ExtensionSettings
  - 값 형식: REG_SZ
  ##### 예제 값:
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


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: ExtensionSettings
  - 예제 값:
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
  

  [맨 위로 이동](#microsoft-edge---정책)

  ## Additional policies

  [맨 위로 이동](#microsoft-edge---정책)

  ### AdsSettingForIntrusiveAdsSites
  #### 침입적인 광고가 있는 사이트에 대한 광고 설정
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 78 이상부터

  #### 설명
  침입적인 광고가 있는 사이트에서 광고를 차단할지 여부를 제어합니다. 이 정책을 다음 옵션 중 하나로 설정할 수 있습니다.

* 1 = 모든 사이트에서 광고 허용.

* 2 = 침입적인 광고가 있는 사이트에서 광고 차단(기본값).

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  정수

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: AdsSettingForIntrusiveAdsSites
  - GP 이름: 침입적인 광고가 있는 사이트에 대한 광고 설정
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: AdsSettingForIntrusiveAdsSites
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000001
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: AdsSettingForIntrusiveAdsSites
  - 예제 값:
``` xml
<integer>1</integer>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### AllowDeletingBrowserHistory
  #### 브라우저 및 다운로드 기록 삭제 사용
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  브라우저 기록 및 다운로드 기록을 삭제하고 사용자가 이 설정을 변경할 수 없도록 합니다.

참고: 이 정책을 사용하지 않도록 설정해도 검색 및 다운로드 기록은 유지되지 않을 수 있습니다. 즉, 사용자가 기록 데이터베이스 파일을 직접 편집하거나 삭제할 수 있으며 브라우저 자체에서 언제든지 일부 또는 전체 기록을 만료 기간에 따라 제거하거나 보관할 수 있습니다.

이 정책을 사용하거나 구성하지 않으면 사용자가 검색 및 다운로드 기록을 삭제할 수 있습니다.

이 정책을 사용하지 않으면 사용자가 검색 및 다운로드 기록을 삭제할 수 없습니다.

이 정책을 사용하도록 설정하는 경우에는 'Microsoft Edge가 닫힐 때 검색 데이터 지우기' 정책을 사용하도록 설정하지 마세요. 둘 다 사용하도록 설정하는 경우에는 이 정책이 어떻게 구성되는지에 관계 없이 'Microsoft Edge가 닫힐 때 검색 데이터 지우기' 정책이 우선하고 Microsoft Edge가 닫힐 때 모든 데이터가 삭제됩니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  부울

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: AllowDeletingBrowserHistory
  - GP 이름: 브라우저 및 다운로드 기록 삭제 사용
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: AllowDeletingBrowserHistory
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000001
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: AllowDeletingBrowserHistory
  - 예제 값:
``` xml
<true/>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### AllowFileSelectionDialogs
  #### 파일 선택 대화 상자 허용
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  Microsoft Edge에서 파일 선택 대화 상자를 표시하여 로컬 파일에 대한 액세스를 허용합니다.

이 정책을 사용하거나 구성하지 않으면 사용자가 파일 선택 대화 상자를 정상적으로 열 수 있습니다.

이 정책을 사용하지 않으면 사용자가 파일 선택 대화 상자(예: 즐겨찾기 가져 오기, 파일 업로드, 링크 저장 등)를 트리거하는 작업을 수행할 때마다 대신 메시지가 표시되고 사용자가 파일 선택 대화 상자에서 [취소]를 클릭한 것으로 간주됩니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  부울

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: AllowFileSelectionDialogs
  - GP 이름: 파일 선택 대화 상자 허용
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: AllowFileSelectionDialogs
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000001
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: AllowFileSelectionDialogs
  - 예제 값:
``` xml
<true/>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### AllowPopupsDuringPageUnload
  #### 언로드하는 동안 페이지에서 팝업을 표시하도록 허용
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 78 이상부터

  #### 설명
  이 정책을 통해 관리자는 페이지를 언로드하는 동안 팝업을 표시할 수 있도록 지정할 수 있습니다.

정책을 사용하도록 설정하면 페이지를 언로드하는 동안 팝업을 표시할 수 있습니다.

 정책을 사용 안 함 또는 설정 해제로 설정하면 페이지가 언로드되는 동안 팝업을 표시할 수 없습니다. 이는 사양(https://html.spec.whatwg.org/#apis-for-creating-and-navigating-browsing-contexts-by-name)에 따라 다릅니다.

 이 정책은 향후에 제거될 예정입니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 아니요 - 브라우저 다시 시작 필요

  #### 데이터 형식:
  부울

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: AllowPopupsDuringPageUnload
  - GP 이름: 언로드하는 동안 페이지에서 팝업을 표시하도록 허용
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: AllowPopupsDuringPageUnload
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000000
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: AllowPopupsDuringPageUnload
  - 예제 값:
``` xml
<false/>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### AllowSyncXHRInPageDismissal
  #### 페이지 해제 중에 페이지에서 동기 XHR 요청을 보내도록 허용
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 79 이상부터

  #### 설명
  이 정책을 사용하면 페이지 해제 중에 페이지에서 동기 XHR 요청을 보낼 수 있도록 지정할 수 있습니다.

이 정책을 사용하면 페이지 해제 중에 페이지에서 동기 XHR 요청을 보낼 수 있습니다.

이 정책 설정을 사용하지 않거나 이 정책을 구성하지 않으면 페이지 해제 중에 페이지에서 동기 XHR 요청을 보낼 수 없습니다.

이 정책은 일시적이며 향후 릴리스에서 제거될 예정입니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 아니요 - 브라우저 다시 시작 필요

  #### 데이터 형식:
  부울

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: AllowSyncXHRInPageDismissal
  - GP 이름: 페이지 해제 중에 페이지에서 동기 XHR 요청을 보내도록 허용
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: AllowSyncXHRInPageDismissal
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000000
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: AllowSyncXHRInPageDismissal
  - 예제 값:
``` xml
<false/>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### AllowTrackingForUrls
  #### 특정 사이트에 대한 추적 방지 예외 구성
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 78 이상부터

  #### 설명
  추적 방지에서 제외되는 URL 패턴의 목록을 구성합니다.

이 정책을 구성하는 경우 구성된 URL 패턴 목록은 추적 방지에서 제외됩니다.

이 정책을 구성하지 않는 경우 "사용자의 웹 검색 활동 추적 차단" 정책(설정된 경우)의 전역 기본값 또는 사용자의 개인 구성이 모든 사이트에 사용됩니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  문자열 목록

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: AllowTrackingForUrls
  - GP 이름: 특정 사이트에 대한 추적 방지 예외 구성
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge\AllowTrackingForUrls
  - 경로 (맞춤): 해당 없음
  - 값 이름: 1, 2, 3, ...
  - 값 형식: REG_SZ 목록
  ##### 예제 값:
```
SOFTWARE\Policies\Microsoft\Edge\AllowTrackingForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\AllowTrackingForUrls\1 = "[*.]contoso.edu"

```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: AllowTrackingForUrls
  - 예제 값:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### AlwaysOpenPdfExternally
  #### 항상 외부에서 PDF 파일 열기
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  Microsoft Edge에서 내부 PDF 뷰어를 사용하지 않도록 설정합니다.

이 정책을 사용하면 Microsoft Edge에서 PDF 파일을 다운로드 파일로 취급하고 사용자가 기본 응용 프로그램을 사용하여 해당 파일을 열 수 있습니다.

이 정책을 구성하지 않거나 사용하지 않도록 설정하면 Microsoft Edge에서 PDF 파일을 엽니다(사용자가 사용하지 않도록 설정하지 않는 한).

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  부울

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: AlwaysOpenPdfExternally
  - GP 이름: 항상 외부에서 PDF 파일 열기
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: AlwaysOpenPdfExternally
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000001
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: AlwaysOpenPdfExternally
  - 예제 값:
``` xml
<true/>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### ApplicationLocaleValue
  #### 응용 프로그램 로캘 설정
  >지원되는 버전: Windows의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  Microsoft Edge에서 응용 프로그램 로캘을 구성하고 사용자가 로캘을 변경하지 못하도록 합니다.

이 정책을 사용하면 Microsoft Edge가 지정된 로캘을 사용합니다. 구성된 로캘이 지원되지 않으면 'en-US'가 대신 사용됩니다.

이 설정을 사용하지 않거나 구성하지 않으면 Microsoft Edge는 사용자가 지정한 기본 설정 로캘(구성된 경우) 또는 대체 로캘 'en-US'를 사용합니다

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 예
  - 동적 정책 새로 고침: 아니요 - 브라우저 다시 시작 필요

  #### 데이터 형식:
  문자열

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: ApplicationLocaleValue
  - GP 이름: 응용 프로그램 로캘 설정
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 관리 템플릿/Microsoft Edge - 기본 설정(사용자가 재정의할 수 없음)/
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): SOFTWARE\Policies\Microsoft\Edge\맞춤
  - 값 이름: ApplicationLocaleValue
  - 값 형식: REG_SZ
  ##### 예제 값:
```
"en"
```


  

  [맨 위로 이동](#microsoft-edge---정책)

  ### AudioCaptureAllowed
  #### 오디오 캡처 허용 또는 차단
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  Allows you to set whether a user is prompted to grant a website access to their audio capture device. This policy applies to all URLs except for those configured in the [AudioCaptureAllowedUrls](#audiocaptureallowedurls) list.

If you enable this policy or don't configure it (the default setting), the user is prompted for audio capture access except from the URLs in the [AudioCaptureAllowedUrls](#audiocaptureallowedurls) list. These listed URLs are granted access without prompting.

If you disable this policy, the user is not prompted, and audio capture is accessible only to the URLs configured in [AudioCaptureAllowedUrls](#audiocaptureallowedurls).

This policy affects all types of audio inputs, not only the built-in microphone.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  부울

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: AudioCaptureAllowed
  - GP 이름: 오디오 캡처 허용 또는 차단
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: AudioCaptureAllowed
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000000
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: AudioCaptureAllowed
  - 예제 값:
``` xml
<false/>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### AudioCaptureAllowedUrls
  #### 사용 권한을 요청하지 않고 오디오 캡처 장치에 액세스할 수 있는 사이트
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  URL 패턴을 기반으로 사용자에게 사용 권한 요청을 하지 않고 오디오 캡처 장치를 사용할 수 있는 웹 사이트를 지정합니다. 이 목록의 패턴은 요청 URL의 보안 시작과 비교됩니다. 일치할 경우 사이트에 오디오 캡처 장치에 대한 액세스 사용 권한이 자동으로 부여됩니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  문자열 목록

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: AudioCaptureAllowedUrls
  - GP 이름: 사용 권한을 요청하지 않고 오디오 캡처 장치에 액세스할 수 있는 사이트
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge\AudioCaptureAllowedUrls
  - 경로 (맞춤): 해당 없음
  - 값 이름: 1, 2, 3, ...
  - 값 형식: REG_SZ 목록
  ##### 예제 값:
```
SOFTWARE\Policies\Microsoft\Edge\AudioCaptureAllowedUrls\0 = "https://www.contoso.com/"
SOFTWARE\Policies\Microsoft\Edge\AudioCaptureAllowedUrls\1 = "https://[*.]contoso.edu/"

```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: AudioCaptureAllowedUrls
  - 예제 값:
``` xml
<array>
  <string>https://www.contoso.com/</string>
  <string>https://[*.]contoso.edu/</string>
</array>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### AutoImportAtFirstRun
  #### 처음 실행 시 다른 브라우저의 데이터 및 설정 자동으로 가져오기
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  이 정책을 사용하면 Microsoft Edge는 기본 브라우저 또는 지정된 다른 브라우저에서 지원되는 모든 데이터 형식 및 설정을 자동으로 가져옵니다. 이 정책은 또한 Microsoft Edge가 첫 실행 경험의 가져오기 섹션을 건너뛰도록 합니다.

이 정책을 'DisabledAutoImport'(4)로 설정하면 첫 실행 환경의 가져오기 섹션이 완전히 건너뛰고 Microsoft Edge는 브라우저 데이터 및 설정을 자동으로 가져오지 않습니다.

* 0 = 기본 브라우저에서 지원되는 모든 데이터 형식 및 설정을 자동으로 가져오기

* 1 = Internet Explorer에서 지원되는 모든 데이터 형식 및 설정을 자동으로 가져오기

* 2 = Google Chrome에서 지원되는 모든 데이터 형식 및 설정을 자동으로 가져오기

* 3 = Safari에서 지원되는 모든 데이터 형식 및 설정을 자동으로 가져오기

* 4 = 자동 가져오기를 사용하지 않고, 첫 실행 경험의 가져오기 섹션을 건너뜀

**참고**: 이 정책은 현재 Internet Explorer(Windows 7, 8 및 10), Google Chrome(Windows 7, 8 및 10, macOS) 및 Apple Safari(macOS) 브라우저에서 가져오기를 지원합니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 아니요 - 브라우저 다시 시작 필요

  #### 데이터 형식:
  정수

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: AutoImportAtFirstRun
  - GP 이름: 처음 실행 시 다른 브라우저의 데이터 및 설정 자동으로 가져오기
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: AutoImportAtFirstRun
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000002
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: AutoImportAtFirstRun
  - 예제 값:
``` xml
<integer>2</integer>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### AutofillAddressEnabled
  #### 주소 정보 자동 채우기 사용
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  자동 채우기 기능을 사용하도록 설정하고 사용자가 이전에 저장된 정보를 사용하여 웹 양식에 주소 정보를 자동으로 완성하도록 허용합니다.

이 정책을 사용하지 않으면 자동 채우기 기능이 주소 정보를 제안하거나 채우지 않으며 사용자가 웹을 탐색할 때 제출할 수 있는 추가 주소 정보도 저장하지 않습니다.

이 정책을 사용하거나 구성하지 않으면 사용자는 사용자 인터페이스의 주소에 대한 자동 채우기를 제어할 수 있습니다.

참고: 이 정책을 사용하지 않으면 지불 및 암호 양식을 제외한 모든 웹 양식의 모든 활동도 중지됩니다. 더 이상 항목이 저장되지 않으며 Microsoft Edge는 이전 항목을 제안하거나 자동으로 채우지 않습니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 예
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  부울

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: AutofillAddressEnabled
  - GP 이름: 주소 정보 자동 채우기 사용
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 관리 템플릿/Microsoft Edge - 기본 설정(사용자가 재정의할 수 없음)/
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): SOFTWARE\Policies\Microsoft\Edge\맞춤
  - 값 이름: AutofillAddressEnabled
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000000
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: AutofillAddressEnabled
  - 예제 값:
``` xml
<false/>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### AutofillCreditCardEnabled
  #### 신용 카드 정보 자동 채우기 사용
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  Microsoft Edge의 자동 채우기 기능을 사용하도록 설정하고 사용자가 이전에 저장된 정보를 사용하여 웹 양식에 신용 카드 정보를 자동으로 완성할 수 있게 합니다.

이 정책을 사용하지 않으면 자동 채우기에서 신용 카드 정보를 제안하거나 채우지 않으며 사용자가 웹을 검색하는 동안 제출할 수 있는 추가 신용 카드 정보를 저장하지 않습니다.

이 정책을 사용하거나 구성하지 않으면 사용자가 신용 카드 정보 자동 채우기를 제어할 수 있습니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 예
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  부울

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: AutofillCreditCardEnabled
  - GP 이름: 신용 카드 정보 자동 채우기 사용
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 관리 템플릿/Microsoft Edge - 기본 설정(사용자가 재정의할 수 없음)/
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): SOFTWARE\Policies\Microsoft\Edge\맞춤
  - 값 이름: AutofillCreditCardEnabled
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000000
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: AutofillCreditCardEnabled
  - 예제 값:
``` xml
<false/>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### AutoplayAllowed
  #### 웹 사이트에 미디어 자동 재생 허용
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 78 이상부터

  #### 설명
  이 정책은 웹 사이트에 대한 미디어 자동 재생 정책을 설정합니다.

기본 설정인 "구성되지 않음"은 현재 미디어 자동 실행 설정을 고려하며 사용자가 자동 실행 설정을 구성할 수 있도록 합니다..

"사용"으로 설정하면 미디어 자동 실행이 "허용"으로 설정됩니다. 모든 웹 사이트는 자동으로 미디어를 재생할 수 있습니다. 사용자가 이 정책을 무시할 수 없습니다..

"사용 안 함"으로 설정하면 미디어 자동 실행이 "차단"으로 설정됩니다. 미디어에 자동 실행을 허용하는 웹 사이트가 없습니다. 사용자가 이 정책을 무시할 수 없습니다.

이 정책이 적용되려면 탭을 닫았다가 다시 열어야 합니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  부울

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: AutoplayAllowed
  - GP 이름: 웹 사이트에 미디어 자동 재생 허용
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: AutoplayAllowed
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000001
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: AutoplayAllowed
  - 예제 값:
``` xml
<true/>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### BackgroundModeEnabled
  #### Microsoft Edge가 닫힌 후 백그라운드 앱 계속 실행
  >지원되는 버전: Windows의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  OS 로그인 시 Microsoft Edge 프로세스가 시작되고 마지막 브라우저 창이 닫힌 후 계속 실행되도록 허용합니다. 이 시나리오에서는 백그라운드 앱과 현재 검색 세션이 세션 쿠키를 포함하여 활성 상태로 유지됩니다. 열려 있는 백그라운드 프로세스는 시스템 트레이에 아이콘을 표시하며 거기에서 언제든지 닫을 수 있습니다.

이 정책을 사용하면 백그라운드 모드가 켜집니다.

이 정책을 사용하지 않으면 백그라운드 모드가 꺼집니다.

이 정책을 구성하지 않으면 초기에 백그라운드 모드가 꺼지고 사용자가 edge://settings/system에서 동작을 구성할 수 있습니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 예
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  부울

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: BackgroundModeEnabled
  - GP 이름: Microsoft Edge가 닫힌 후 백그라운드 앱 계속 실행
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 관리 템플릿/Microsoft Edge - 기본 설정(사용자가 재정의할 수 없음)/
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): SOFTWARE\Policies\Microsoft\Edge\맞춤
  - 값 이름: BackgroundModeEnabled
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000001
```


  

  [맨 위로 이동](#microsoft-edge---정책)

  ### BackgroundTemplateListUpdatesEnabled
  #### 컬렉션 및 템플릿을 사용하는 기타 기능의 사용 가능한 템플릿 목록에 대한 백그라운드 업데이트를 사용하도록 설정합니다.
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 79 이상부터

  #### 설명
  컬렉션 템플릿을 사용하는 기타 기능에 사용 가능한 템플릿 목록에 대한 백그라운드 업데이트를 사용하거나 사용하지 않도록 설정할 수 있습니다. 템플릿은 페이지가 컬렉션에 저장되어 있을 때 웹 페이지에서 서식 있는 메타데이터를 추출하는 데 사용됩니다.

이 설정을 사용하거나 설정을 구성하지 않으면 사용 가능한 템플릿 목록이 24시간마다 Microsoft 서비스에서 백그라운드로 다운로드됩니다.

이 설정을 사용하지 않으면 필요할 때 사용 가능한 템플릿 목록이 다운로드됩니다. 이러한 유형의 다운로드는 컬렉션 및 기타 기능에 대한 성능 저하를 일으킬 수 있습니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  부울

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: BackgroundTemplateListUpdatesEnabled
  - GP 이름: 컬렉션 및 템플릿을 사용하는 기타 기능의 사용 가능한 템플릿 목록에 대한 백그라운드 업데이트를 사용하도록 설정합니다.
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: BackgroundTemplateListUpdatesEnabled
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000001
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: BackgroundTemplateListUpdatesEnabled
  - 예제 값:
``` xml
<true/>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### BlockThirdPartyCookies
  #### 타사 쿠키 차단
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  주소 표시줄에 있는도메인에서 비롯되지 않은 웹 페이지 요소가 쿠키를 설정하지 못하도록 차단합니다.

이 정책을 사용하면 주소 표시줄에 있는도메인에서 비롯되지 않은 웹 페이지 요소가 쿠키를 설정할 수 없습니다.

이 정책을 사용하지 않으면 주소 표시줄 이외의도메인에 있는 웹 페이지 요소에서 쿠키를 설정할 수 있습니다.

이 정책을 구성하지 않으면 타사 쿠키가 사용하도록 설정되지만 사용자가 이 설정을 변경할 수 있습니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 예
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  부울

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: BlockThirdPartyCookies
  - GP 이름: 타사 쿠키 차단
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 관리 템플릿/Microsoft Edge - 기본 설정(사용자가 재정의할 수 없음)/
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): SOFTWARE\Policies\Microsoft\Edge\맞춤
  - 값 이름: BlockThirdPartyCookies
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000000
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: BlockThirdPartyCookies
  - 예제 값:
``` xml
<false/>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### BrowserAddProfileEnabled
  #### ID 플라이아웃 메뉴 또는 설정 페이지에서 프로필 만들기 사용
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  **프로필 추가** 옵션을 사용하여 새 프로필을 만들 수 있도록 허용합니다.
이 정책을 사용하거나 구성하지 않으면 Microsoft Edge에서 사용자가 ID 플라이아웃 메뉴 또는 설정 페이지에서 **프로필 추가**를 사용하여 새 프로필을 만들 수 있습니다.

이 정책을 사용하지 않으면 사용자가 ID 플라이아웃 메뉴 또는 설정 페이지에서 새 프로필을 추가할 수 없습니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  부울

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: BrowserAddProfileEnabled
  - GP 이름: ID 플라이아웃 메뉴 또는 설정 페이지에서 프로필 만들기 사용
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: BrowserAddProfileEnabled
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000001
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: BrowserAddProfileEnabled
  - 예제 값:
``` xml
<true/>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### BrowserGuestModeEnabled
  #### 게스트 모드 사용
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  Microsoft Edge에서 게스트 프로필을 사용하도록 허용하는 옵션을 사용합니다. 게스트 프로필의 경우, 브라우저는 기존 프로필에서 검색 데이터를 가져오지 않으며 모든 게스트 프로필이 닫힐 때 검색 데이터를 삭제합니다.

이 정책 설정을 사용하거나 구성하지 않으면 Microsoft Edge에서 사용자가 게스트 프로필을 탐색할 수 있도록 허용합니다.

이 정책을 사용하지 않으면 Microsoft Edge에서 사용자가 게스트 프로필을 탐색할 수 없습니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  부울

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: BrowserGuestModeEnabled
  - GP 이름: 게스트 모드 사용
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: BrowserGuestModeEnabled
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000001
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: BrowserGuestModeEnabled
  - 예제 값:
``` xml
<true/>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### BrowserNetworkTimeQueriesEnabled
  #### 브라우저 네트워크 시간 서비스에 대한 쿼리 허용
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  정확한 타임스탬프를 검색하기 위해 Microsoft Edge에서 때때로 브라우저 네트워크 시간 서비스에 쿼리를 보낼 수 없게 합니다.

이 정책을 사용하지 않으면 Microsoft Edge에서 브라우저 네트워크 시간 서비스에 쿼리를 보내는 것이 중지됩니다.

이 정책을 사용하거나 구성하지 않으면 Microsoft Edge에서 때때로 브라우저 네트워크 시간 서비스에 쿼리를 보냅니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  부울

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: BrowserNetworkTimeQueriesEnabled
  - GP 이름: 브라우저 네트워크 시간 서비스에 대한 쿼리 허용
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: BrowserNetworkTimeQueriesEnabled
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000001
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: BrowserNetworkTimeQueriesEnabled
  - 예제 값:
``` xml
<true/>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### BrowserSignin
  #### 브라우저 로그인 설정
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  Specify whether a user can sign into Microsoft Edge with their account and use account-related services like sync and single sign on. To control the availability of sync, use the [SyncDisabled](#syncdisabled) policy instead.

If you set this policy to 'Disable browser sign-in', make sure that you also set the [NonRemovableProfileEnabled](#nonremovableprofileenabled) policy to disabled because [NonRemovableProfileEnabled](#nonremovableprofileenabled) disables the creation of an automatically signed in browser profile. If both policies are set, Microsoft Edge will use the 'Disable browser sign-in' policy and behave as if [NonRemovableProfileEnabled](#nonremovableprofileenabled) is set to disabled.

If you set this policy to 'Enable browser sign-in' (1), users can sign into the browser. Signing into the browser doesn't mean that sync is turned on by default; the user must separately opt-in to use this feature.

If you set this policy to 'Force browser sign-in' (2) users must sign into a profile to use the browser. By default, this will allow the user to choose whether they want to sync to their account, unless sync is disabled by the domain admin or with the [SyncDisabled](#syncdisabled) policy. The default value of [BrowserGuestModeEnabled](#browserguestmodeenabled) policy is set to false.

If you don't configure this policy users can decide if they want to enable the browser sign-in option and use it as they see fit.

* 0 = Disable browser sign-in

* 1 = Enable browser sign-in

* 2 = Force users to sign-in to use the browser

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 아니요 - 브라우저 다시 시작 필요

  #### 데이터 형식:
  정수

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: BrowserSignin
  - GP 이름: 브라우저 로그인 설정
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: BrowserSignin
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000002
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: BrowserSignin
  - 예제 값:
``` xml
<integer>2</integer>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### BuiltInDnsClientEnabled
  #### 기본 제공 DNS 클라이언트 사용
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  기본 제공 DNS 클라이언트를 사용할지 여부를 제어합니다.

이 정책을 사용하면 기본 DNS 클라이언트가 사용됩니다(사용 가능한 경우).

이 정책을 사용하지 않으면 클라이언트가 사용되지 않습니다.

이 정책을 구성하지 않으면 기본 제공 DNS 클라이언트가 MacOS에서 기본적으로 사용되며 사용자는 edge://flags를 편집하거나 명령줄 플래그를 지정하여 기본 제공 DNS 클라이언트를 사용할지 여부를 변경할 수 있습니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  부울

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: BuiltInDnsClientEnabled
  - GP 이름: 기본 제공 DNS 클라이언트 사용
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: BuiltInDnsClientEnabled
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000001
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: BuiltInDnsClientEnabled
  - 예제 값:
``` xml
<true/>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### CertificateTransparencyEnforcementDisabledForCas
  #### subjectPublicKeyInfo 해시 목록에 대한 인증서 투명성 적용 사용 안 함
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  subjectPublicKeyInfo 해시 목록에 대한 인증서 투명성 요구 사항의 적용을 사용하지 않도록 설정합니다.

이 정책은 지정된 subjectPublicKeyInfo 해시 중 하나를 사용하여 인증서를 포함하는 인증서 체인에 대한 인증서 투명성 공개 요구 사항을 사용하지 않도록 설정할 수 있습니다. 제대로 공개되지 않았기 때문에 이 정책을 사용하지 않으면 신뢰할 수 없는 것이 되는 인증서가 엔터프라이즈 호스트에 계속 사용될 수 있습니다.

이 정책을 설정할 때 인증서 투명성 적용을 사용하지 않으려면 다음 조건 집합 중 하나가 충족되어야 합니다.
1. 해시는 서버 인증서의 subjectPublicKeyInfo입니다.
2. 해시는 인증서 체인에 있는 CA 인증서에 표시되는 subjectPublicKeyInfo의 해시이며, 해당 CA 인증서는 X.509v3 nameConstraints 확장을 통해 제한되며, 하나 이상의 directoryName nameConstraints가 permittedSubtrees에 있고 directoryName에 organizationName 특성이 포함되어 있습니다.
3. 해시는 인증서 체인에 있는 CA 인증서에 표시되는 subjectPublicKeyInfo의 해시이며, CA 인증서에는 인증서 Subject에 하나 이상의 organizationName 특성이 있으며, 서버의 인증서에는 동일한 순서로 바이트 단위의 동일한 값인 동일한 수의 organizationName 특성이 포함되어 있습니다.

해시 알고리즘 이름, "/" 문자 및 지정된 인증서의 DER로 인코딩된 subjectPublicKeyInfo에 적용된 해당 해시 알고리즘의 Base64 인코딩을 연결하여 subjectPublicKeyInfo 해시를 지정합니다. 이 Base64 인코딩은 RFC 7469, 섹션 2.4에 정의된 SPKI 지문과 동일한 형식입니다. 인식할 수 없는 해시 알고리즘은 무시됩니다. 현재 지원되는 유일한 해시 알고리즘은 "sha256"입니다.

이 정책을 사용하지 않거나 구성하지 않으면 인증서 투명성 정책에 따라 공개되지 않으면 인증서 투명성을 통해 공개해야 하는 인증서는 신뢰할 수 없는 것으로 처리됩니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  문자열 목록

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: CertificateTransparencyEnforcementDisabledForCas
  - GP 이름: subjectPublicKeyInfo 해시 목록에 대한 인증서 투명성 적용 사용 안 함
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge\CertificateTransparencyEnforcementDisabledForCas
  - 경로 (맞춤): 해당 없음
  - 값 이름: 1, 2, 3, ...
  - 값 형식: REG_SZ 목록
  ##### 예제 값:
```
SOFTWARE\Policies\Microsoft\Edge\CertificateTransparencyEnforcementDisabledForCas\0 = "sha256/AAAAAAAAAAAAAAAAAAAAAA=="
SOFTWARE\Policies\Microsoft\Edge\CertificateTransparencyEnforcementDisabledForCas\1 = "sha256//////////////////////w=="

```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: CertificateTransparencyEnforcementDisabledForCas
  - 예제 값:
``` xml
<array>
  <string>sha256/AAAAAAAAAAAAAAAAAAAAAA==</string>
  <string>sha256//////////////////////w==</string>
</array>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### CertificateTransparencyEnforcementDisabledForLegacyCas
  #### 레거시 인증 기관 목록에 대 한 인증서 투명도 적용 사용 안 함
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  레거시 CA(인증 기관) 목록에 대한 인증서 투명성 요구 사항의 적용을 사용하지 않도록 설정합니다.

이 정책을 사용하면 지정된 subjectPublicKeyInfo 해시 중 하나를 사용하여 인증서를 포함하는 인증서 체인에 대한 인증서 투명성 공개 요구 사항을 사용하지 않도록 설정할 수 있습니다. 적절하게 공개되지 않았기 때문에 이 정책을 사용하지 않으면 신뢰할 수 없는 것이 되는 인증서가 엔터프라이즈 호스트에 계속 사용됩니다.

인증서 투명성 적용을 사용하지 않으려면 레거시 CA(인증 기관)로 인식되는 CA 인증서에 표시되는 subjectPublicKeyInfo 해시를 설정해야 합니다. 레거시 CA는 Microsoft Edge에서 지원하는 하나 이상의 운영 체제에서 기본값으로 공개적으로 신뢰할 수 있는 CA입니다.

해시 알고리즘 이름, "/" 문자 및 지정된 인증서의 DER로 인코딩된 subjectPublicKeyInfo에 적용된 해당 해시 알고리즘의 Base64 인코딩을 연결하여 subjectPublicKeyInfo 해시를 지정합니다. 이 Base64 인코딩은 RFC 7469, 섹션 2.4에 정의된 SPKI 지문과 동일한 형식입니다. 인식할 수 없는 해시 알고리즘은 무시됩니다. 현재 지원되는 유일한 해시 알고리즘은 "sha256"입니다.

이 정책을 구성하지 않으면, 인증서 투명성을 통해 공개해야 하는 인증서는 인증서 투명성 정책에 따라 공개되지 않으면 신뢰할 수 없는 것으로 인증서는 처리됩니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  문자열 목록

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: CertificateTransparencyEnforcementDisabledForLegacyCas
  - GP 이름: 레거시 인증 기관 목록에 대 한 인증서 투명도 적용 사용 안 함
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge\CertificateTransparencyEnforcementDisabledForLegacyCas
  - 경로 (맞춤): 해당 없음
  - 값 이름: 1, 2, 3, ...
  - 값 형식: REG_SZ 목록
  ##### 예제 값:
```
SOFTWARE\Policies\Microsoft\Edge\CertificateTransparencyEnforcementDisabledForLegacyCas\0 = "sha256/AAAAAAAAAAAAAAAAAAAAAA=="
SOFTWARE\Policies\Microsoft\Edge\CertificateTransparencyEnforcementDisabledForLegacyCas\1 = "sha256//////////////////////w=="

```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: CertificateTransparencyEnforcementDisabledForLegacyCas
  - 예제 값:
``` xml
<array>
  <string>sha256/AAAAAAAAAAAAAAAAAAAAAA==</string>
  <string>sha256//////////////////////w==</string>
</array>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### CertificateTransparencyEnforcementDisabledForUrls
  #### 특정 URL에 대한 인증서 투명성 적용 사용 안 함
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  나열된 URL에 대해 강제 인증서 투명성 요구 사항을 사용하지 않도록 설정합니다.

이 정책을 사용하면 인증서 투명성을 통해 지정한 URL의 호스트 이름에 대한 인증서를 공개하지 않을 수 있습니다. 따라서 적절하게 공개되지 않았기 때문에 이 정책을 사용하지 않으면 신뢰할 수 없는 것이 되는 인증서를 사용할 수 있지만 해당 호스트에 대해 잘못 발급된 인증서를 검색하기가 더 어려워집니다.

[https://go.microsoft.com/fwlink/?linkid=2095322](https://go.microsoft.com/fwlink/?linkid=2095322)에 따라 URL 패턴을 구성합니다. 인증서는 구성표, 포트 또는 경로와 관계없이 지정된 호스트 이름에 대해 유효하기 때문에 URL의 호스트 이름 부분만 고려됩니다. 와일드카드 호스트는 지원되지 않습니다.

이 정책을 구성하지 않으면 인증서 투명성을 통해 공개해야 하는 공개되지 않은 경우 신뢰할 수 없는 것으로 처리됩니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  문자열 목록

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: CertificateTransparencyEnforcementDisabledForUrls
  - GP 이름: 특정 URL에 대한 인증서 투명성 적용 사용 안 함
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge\CertificateTransparencyEnforcementDisabledForUrls
  - 경로 (맞춤): 해당 없음
  - 값 이름: 1, 2, 3, ...
  - 값 형식: REG_SZ 목록
  ##### 예제 값:
```
SOFTWARE\Policies\Microsoft\Edge\CertificateTransparencyEnforcementDisabledForUrls\0 = "contoso.com"
SOFTWARE\Policies\Microsoft\Edge\CertificateTransparencyEnforcementDisabledForUrls\1 = ".contoso.com"

```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: CertificateTransparencyEnforcementDisabledForUrls
  - 예제 값:
``` xml
<array>
  <string>contoso.com</string>
  <string>.contoso.com</string>
</array>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### ClearBrowsingDataOnExit
  #### Microsoft Edge가 닫힐 때 검색 데이터 지우기
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 78 이상부터

  #### 설명
  Microsoft Edge doesn't clear the browsing data by default when it closes. Browsing data includes information entered in forms, passwords, and even the websites visited.

If you enable this policy, all browsing data is deleted each time Microsoft Edge closes.

If you disable or don't configure this policy, users can configure the Clear browsing data option in Settings.

If you enable this policy, don't enable the [AllowDeletingBrowserHistory](#allowdeletingbrowserhistory) policy, because they both deal with deleting data. If you enable both, this policy takes precedence and deletes all data when Microsoft Edge closes, regardless of how you configured [AllowDeletingBrowserHistory](#allowdeletingbrowserhistory).

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 예
  - 동적 정책 새로 고침: 아니요 - 브라우저 다시 시작 필요

  #### 데이터 형식:
  부울

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: ClearBrowsingDataOnExit
  - GP 이름: Microsoft Edge가 닫힐 때 검색 데이터 지우기
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 관리 템플릿/Microsoft Edge - 기본 설정(사용자가 재정의할 수 없음)/
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): SOFTWARE\Policies\Microsoft\Edge\맞춤
  - 값 이름: ClearBrowsingDataOnExit
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000001
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: ClearBrowsingDataOnExit
  - 예제 값:
``` xml
<true/>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### ClickOnceEnabled
  #### 사용자가 ClickOnce 프로토콜을 사용하여 파일을 열 수 있도록 허용
  >지원되는 버전: Windows의 Microsoft Edge, 버전 78 이상부터

  #### 설명
  사용자가 ClickOnce 프로토콜을 사용하여 파일을 열 수 있도록 허용 합니다. ClickOnce 프로토콜을 사용하면 웹 사이트에서 사용자의 컴퓨터나 장치에 있는 ClickOnce 파일 처리기를 사용하여 특정 URL의 파일을 브라우저에서 열도록 요청할 수 있습니다.

이 정책을 사용하면 사용자는 ClickOnce 프로토콜을 사용하여 파일을 열 수 있습니다. 이 정책은 edge://flags/ 페이지에 있는 사용자의 ClickOnce 설정보다 우선시 됩니다.

이 정책을 사용하지 않으면 사용자가 ClickOnce 프로토콜을 사용하 여 파일을 열 수 없습니다. 대신 파일은 브라우저를 사용하여 파일 시스템에 저장됩니다. 이 정책은 edge://flags/ 페이지에 있는 사용자의 ClickOnce 설정보다 우선시 됩니다.

이 정책을 구성하지 않으면 사용자가 ClickOnce 프로토콜을 사용하여 파일을 열 수 없습니다. 사용자는 edge://flags/ 페이지에서 ClickOnce 프로토콜을 사용할 수 있도록 설정하는 옵션을 사용할 수 있습니다.

ClickOnce를 사용하지 않도록 설정하면 ClickOnce 응용 프로그램 (.application 파일)이 제대로 시작되지 않을 수 있습니다.

ClickOnce에 대한 자세한 내용은 [https://go.microsoft.com/fwlink/?linkid=2103872](https://go.microsoft.com/fwlink/?linkid=2103872) 및 [https://go.microsoft.com/fwlink/?linkid=2099880](https://go.microsoft.com/fwlink/?linkid=2099880)를 참조하세요.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  부울

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: ClickOnceEnabled
  - GP 이름: 사용자가 ClickOnce 프로토콜을 사용하여 파일을 열 수 있도록 허용
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: ClickOnceEnabled
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000000
```


  

  [맨 위로 이동](#microsoft-edge---정책)

  ### CommandLineFlagSecurityWarningsEnabled
  #### 명령줄 플래그에 대한 보안 경고 사용
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 78 이상부터

  #### 설명
  이 정책을 사용하지 않으면 잠재적으로 위험한 명령줄 플래그를 사용하여 Microsoft Edge를 시작할 보안 경고가 표시되지 않습니다.

사용하거나 설정하지 않으면 이러한 명령줄 플래그를 사용하여 Microsoft Edge를 시작할 때 보안 경고가 표시됩니다.

예를 들어, --disable-gpu-sandbox 플래그는 다음 경고를 생성합니다: 지원되지 않는 명령줄 플래그(--disable-gpu-sandbox)를 사용하고 있습니다. 이 플래그는 안전성과 보안 상을 위험을 초래합니다.

Windows에서 이 정책은 Microsoft Active Directory 도메인에 가입된 인스턴스 또는 장치 관리를 위해 등록된 Windows 10 Pro 또는 Enterprise 인스턴스에서만 사용할 수 있습니다

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 아니요 - 브라우저 다시 시작 필요

  #### 데이터 형식:
  부울

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: CommandLineFlagSecurityWarningsEnabled
  - GP 이름: 명령줄 플래그에 대한 보안 경고 사용
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: CommandLineFlagSecurityWarningsEnabled
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000001
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: CommandLineFlagSecurityWarningsEnabled
  - 예제 값:
``` xml
<true/>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### ComponentUpdatesEnabled
  #### Microsoft Edge에서 구성 요소 업데이트 사용
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  이 정책을 사용하거나 구성하지 않으면 Microsoft Edge에서 구성 요소 업데이트를 사용할 수 있습니다.

이 정책을 사용하지 않거나 false로 설정하면 Microsoft Edge의 모든 구성 요소에 대해 구성 요소 업데이트를 사용할 수 없습니다.

그러나 일부 구성 요소는 이 정책에서 제외됩니다. 여기에는 실행 코드를 포함하지 않거나 브라우저의 동작이 크게 변경되지 않거나 보안을 위해 중요한 구성 요소가 포함됩니다. 즉, "보안을 위해 중요한" 업데이트라고 간주되는 업데이트는 이 정책을 사용하지 않도록 설정한 경우에도 계속 적용됩니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 아니요 - 브라우저 다시 시작 필요

  #### 데이터 형식:
  부울

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: ComponentUpdatesEnabled
  - GP 이름: Microsoft Edge에서 구성 요소 업데이트 사용
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: ComponentUpdatesEnabled
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000001
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: ComponentUpdatesEnabled
  - 예제 값:
``` xml
<true/>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### ConfigureDoNotTrack
  #### 추적 안 함 구성
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  추적 정보를 요청하는 웹 사이트에 추적 안 함 요청을 보낼지 여부를 지정합니다. 추적 안 함 요청은 사용자가 방문하는 웹 사이트에 사용자의 검색 활동을 추적하지 못하도록 한다는 것을 알려줍니다. 기본적으로 Microsoft Edge는 추적 안 함 요청을 보내지 않지만 사용자는 이 기능을 사용하여 보낼 수 있습니다.

이 정책을 사용하면 항상 추적 안 함 요청이 추적 정보를 요청하는 웹 사이트로 전송됩니다.

이 정책을 사용하지 않으면 요청이 전송되지 않습니다.

이 정책을 구성하지 않으면 사용자가 이러한 요청을 보낼지 여부를 선택할 수 있습니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  부울

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: ConfigureDoNotTrack
  - GP 이름: 추적 안 함 구성
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: ConfigureDoNotTrack
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000000
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: ConfigureDoNotTrack
  - 예제 값:
``` xml
<false/>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### ConfigureOnlineTextToSpeech
  #### 온라인 텍스트 음성 변환 구성
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  Azure인식 서비스의 한 부분인 브라우저에서 온라인 텍스트 음성 변환 글꼴을 활용할 수 있는지 여부를 설정합니다.

이 정책을 사용하거나 구성하지 않으면 SpeechSynthesis API를 사용하는 웹 기반 응용 프로그램에서 온라인 텍스트 음성 변환 글꼴을 사용할 수 있습니다.

사이 정책을 사용하지 않으면 음성 글꼴을 사용할 수 없습니다.

이 기능에 대한 자세한 내용은 다음을 참조하세요:
SpeechSynthesis API: https://developer.mozilla.org/ko-KR/docs/Web/API/SpeechSynthesis
인식 서비스: https://azure.microsoft.com/ko-kr/services/cognitive-services/text-to-speech/

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  부울

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: ConfigureOnlineTextToSpeech
  - GP 이름: 온라인 텍스트 음성 변환 구성
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: ConfigureOnlineTextToSpeech
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000001
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: ConfigureOnlineTextToSpeech
  - 예제 값:
``` xml
<true/>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### CustomHelpLink
  #### 사용자 지정 도움말 링크 지정
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 79 이상부터

  #### 설명
  도움말 메뉴 또는 F1 키에 대한 링크를 지정합니다.

이 정책을 사용하면 관리자가 도움말 메뉴 또는 F1 키에 대한 링크를 지정할 수 있습니다.

이 정책을 사용하지 않도록 설정하거나 구성하지 않으면 도움말 메뉴 또는 F1 키에 대한 기본 링크가 사용됩니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  문자열

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: CustomHelpLink
  - GP 이름: 사용자 지정 도움말 링크 지정
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: CustomHelpLink
  - 값 형식: REG_SZ
  ##### 예제 값:
```
"https://go.microsoft.com/fwlink/?linkid=2080734"
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: CustomHelpLink
  - 예제 값:
``` xml
<string>https://go.microsoft.com/fwlink/?linkid=2080734</string>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### DefaultBrowserSettingEnabled
  #### Microsoft Edge를 기본 브라우저로 설정
  >지원되는 버전: Windows 7 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  Microsoft Edge에서 기본 브라우저 확인을 구성하고 사용자가 이를 변경할 수 없도록 합니다.

이 정책을 사용하면 Microsoft Edge는 시작할 때 항상 기본 브라우저인지 여부를 확인하고 가능한 경우 자동으로 자체 등록합니다.

이 정책을 사용하지 않으면 Microsoft Edge는 절대 확인하지 않으며 이 옵션을 설정할 수 있는 사용자 컨트롤을 사용하지 않도록 설정합니다.

이 정책을 구성하지 않으면 Microsoft Edge를 통해 사용자가 기본 브라우저인지 여부와 그렇지 않을 경우 사용자 알림을 표시할지 여부를 제어할 수 있습니다.

Windows 관리자 참고 사항: 정책은 Windows 7을 실행하는 PC에서만 작동합니다. 이후 버전의 Windows에서는 Microsoft Edge를 https 및 http 프로토콜 (및 선택적으로 .html, .htm, .pdf, .svg, .webp와 같은 ftp 프로토콜 및 파일 형식)에 대한 처리기로 만드는 "기본 응용 프로그램 연결" 파일을 배포해야 합니다. 자세한 내용은 [https://go.microsoft.com/fwlink/?linkid=2094932](https://go.microsoft.com/fwlink/?linkid=2094932)를 참조하세요.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  부울

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: DefaultBrowserSettingEnabled
  - GP 이름: Microsoft Edge를 기본 브라우저로 설정
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: DefaultBrowserSettingEnabled
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000001
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: DefaultBrowserSettingEnabled
  - 예제 값:
``` xml
<true/>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### DeveloperToolsAvailability
  #### 개발자 도구를 사용할 수 있는 위치 제어
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  개발자 도구를 사용할 수 있는 위치를 제어합니다.

이 정책을 'DeveloperToolsDisallowedForForceInstalledExtensions'(0, 기본값)로 설정하면 사용자가 개발자 도구와 JavaScript 콘솔에 일반적으로 액세스할 수 있지만 엔터프라이즈 정책에 의해 설치된 확장의 컨텍스트에서는 액세스할 수 없습니다.

이 정책을 'DeveloperToolsAllowed'(1)로 설정하면 사용자가 엔터프라이즈 정책에 의해 설치된 확장을 포함하여 모든 컨텍스트에서 개발자 도구와 JavaScript 콘솔에 액세스할 수 있습니다.

이 정책을 'DeveloperToolsDisallowed'(2)로 설정하면 사용자가 개발자 도구에 액세스하거나 웹 사이트 요소를 검사할 수 없습니다. 개발자 도구나 JavaScript 콘솔을 여는 바로 가기 키와 메뉴 또는 상황에 맞는 메뉴 항목을 사용할 수 없습니다.

* 0 = 엔터프라이즈 정책에 의해 설치된 확장에서 개발자 도구 차단, 다른 컨텍스트에서 허용

* 1 = 개발자 도구 사용 허용

* 2 = 개발자 도구 사용 허용 안 함

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  정수

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: DeveloperToolsAvailability
  - GP 이름: 개발자 도구를 사용할 수 있는 위치 제어
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: DeveloperToolsAvailability
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000002
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: DeveloperToolsAvailability
  - 예제 값:
``` xml
<integer>2</integer>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### DirectInvokeEnabled
  #### 사용자가 DirectInvoke 프로토콜을 사용하여 파일을 열 수 있도록 허용
  >지원되는 버전: Windows의 Microsoft Edge, 버전 78 이상부터

  #### 설명
  사용자가 DirectInvoke 프로토콜을 사용하여 파일을 열 수 있도록 허용합니다. DirectInvoke 프로토콜은 웹 사이트에서 사용자의 컴퓨터나 장치에 있는 특정 파일 처리기를 사용하여 특정 URL의 파일을 브라우저에서 열도록 요청할 수 있습니다.

이 정책을 사용하거나 구성하지 않으면 사용자는 DirectInvoke 프로토콜을 사용하여 파일을 열 수 있습니다.

이 정책을 사용하지 않으면 사용자는 DirectInvoke 프로토콜을 사용하여 파일을 열 수 없습니다. 대신 파일은 파일 시스템에 저장됩니다.

참고: DirectInvoke를 사용하지 않도록 설정하면 특정 Microsoft SharePoint Online 기능이 예상대로 작동하지 않을 수 있습니다.

DirectInvoke에 대한 자세한 내용은 [https://go.microsoft.com/fwlink/?linkid=2103872](https://go.microsoft.com/fwlink/?linkid=2103872) 및 [https://go.microsoft.com/fwlink/?linkid=2099871](https://go.microsoft.com/fwlink/?linkid=2099871)를 참조하세요.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  부울

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: DirectInvokeEnabled
  - GP 이름: 사용자가 DirectInvoke 프로토콜을 사용하여 파일을 열 수 있도록 허용
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: DirectInvokeEnabled
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000000
```


  

  [맨 위로 이동](#microsoft-edge---정책)

  ### Disable3DAPIs
  #### 3D 그래픽 API에 대한 지원 사용 안 함
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  Prevent web pages from accessing the graphics processing unit (GPU). Specifically, web pages can't access the WebGL API and plug-ins can't use the Pepper 3D API.

If you don't configure or disable this policy, it potentially allows web pages to use the WebGL API and plug-ins to use the Pepper 3D API. Microsoft Edge might, by default, still require command line arguments to be passed in order to use these APIs.

If [HardwareAccelerationModeEnabled](#hardwareaccelerationmodeenabled) policy is set to false, the setting for 'Disable3DAPIs' policy is ignored - it's the equivalent of setting 'Disable3DAPIs' policy to true.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  부울

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: Disable3DAPIs
  - GP 이름: 3D 그래픽 API에 대한 지원 사용 안 함
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: Disable3DAPIs
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000000
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: Disable3DAPIs
  - 예제 값:
``` xml
<false/>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### DisableScreenshots
  #### 스크린샷 찍기 사용 안 함
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  사용자가 브라우저 페이지의 스크린샷을 찍을 수 있는지 여부를 제어합니다.

이 정책을 사용하면 사용자가 바로 가기 키 또는 확장 API를 사용하여 스크린샷을 찍을 수 없습니다.

이 정책을 사용하지 않거나 구성하지 않으면 사용자가 스크린샷을 찍을 수 있습니다.

참고: 이 정책은 브라우저 자체에서 찍은 스크린샷을 제어합니다. 이 정책을 사용하도록 설정하는 경우에도 사용자는 운영 체제 기능이나 다른 응용 프로그램 사용하는 등의 일부 브라우저 외부의 방법을 사용하여 계속 스크린샷을 찍을 수 있습니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  부울

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: DisableScreenshots
  - GP 이름: 스크린샷 찍기 사용 안 함
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: DisableScreenshots
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000001
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: DisableScreenshots
  - 예제 값:
``` xml
<true/>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### DiskCacheDir
  #### 디스크 캐시 디렉터리 설정
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  캐시된 파일을 저장하는 데 사용할 디렉터리를 구성합니다.

이 정책을 사용하면 Microsoft Edge 는 사용자가 '--disk-cache-dir' 플래그를 지정했는지 여부에 관계 없이 제공된 디렉터리를 사용합니다. Microsoft Edge에서 콘텐츠를 관리하므로 데이터 손실이나 기타 예기치 않은 오류가 발생하지 않도록 하려면 볼륨의 루트 디렉터리 또는 다른 목적으로 사용되는 디렉터리에 이 정책을 구성하지 마세요.

디렉터리 및 경로를 지정할 때 사용할 수 있는 변수 목록은 [https://go.microsoft.com/fwlink/?linkid=2095041](https://go.microsoft.com/fwlink/?linkid=2095041)을 참조하세요.

이 정책을 구성하지 않으면 기본 캐시 디렉터리가 사용되며 사용자가 '--disk-cache-dir' 명령줄 플래그를 사용하여 해당 기본값을 재정의할 수 있습니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 아니요 - 브라우저 다시 시작 필요

  #### 데이터 형식:
  문자열

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: DiskCacheDir
  - GP 이름: 디스크 캐시 디렉터리 설정
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: DiskCacheDir
  - 값 형식: REG_SZ
  ##### 예제 값:
```
"${user_home}/Edge_cache"
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: DiskCacheDir
  - 예제 값:
``` xml
<string>${user_home}/Edge_cache</string>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### DiskCacheSize
  #### 디스크 캐시 크기를 바이트 단위로 설정
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  디스크에 파일을 저장하는 데 사용되는 캐시 크기(바이트)를 구성합니다.

이 정책을 사용하면 Microsoft Edge는 사용자가 '--disk-cache-size' 플래그를 지정했는지 여부에 관계 없이 제공된 캐시 크기를 사용합니다. 이 정책에 지정된 값은 하드 경계가 아니라 캐싱 시스템에 대한 제안 사항입니다. 메가바이트 이하의 값은 너무 작아서 합리적인 최소값으로 반올림됩니다.

이 정책의 값을 0으로 설정하면 기본 캐시 크기가 사용되며 사용자가 변경할 수 없습니다.

이 정책을 구성하지 않으면 기본 크기가 사용되지만 사용자가 '--disk-cache-size' 플래그를 사용하여 재정의할 수 있습니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 아니요 - 브라우저 다시 시작 필요

  #### 데이터 형식:
  정수

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: DiskCacheSize
  - GP 이름: 디스크 캐시 크기를 바이트 단위로 설정
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: DiskCacheSize
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x06400000
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: DiskCacheSize
  - 예제 값:
``` xml
<integer>104857600</integer>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### DownloadDirectory
  #### 다운로드 디렉터리 설정
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  파일을 다운로드할 때 사용할 디렉터리를 구성합니다.

이 정책을 사용하면 Microsoft Edge는 사용자가 디렉터리를 지정했거나 매번 다운로드 위치를 묻는 메시지가 표시되도록 선택했는지 여부에 관계 없이 제공된 디렉터리를 사용합니다. 사용할 수 있는 변수 목록은 [https://go.microsoft.com/fwlink/?linkid=2095041](https://go.microsoft.com/fwlink/?linkid=2095041)을 참조하세요.

이 정책 설정을 사용하지 않거나 구성하지 않으면 기본 다운로드 디렉터리가 사용되며 사용자가 변경할 수 있습니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 예
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  문자열

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: DownloadDirectory
  - GP 이름: 다운로드 디렉터리 설정
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 관리 템플릿/Microsoft Edge - 기본 설정(사용자가 재정의할 수 없음)/
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): SOFTWARE\Policies\Microsoft\Edge\맞춤
  - 값 이름: DownloadDirectory
  - 값 형식: REG_SZ
  ##### 예제 값:
```
"/home/${user_name}/Downloads"
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: DownloadDirectory
  - 예제 값:
``` xml
<string>/home/${user_name}/Downloads</string>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### DownloadRestrictions
  #### 다운로드 제한 허용
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  사용자가 보안 결정을 재정의할 수 없도록 하면서 Microsoft Edge가 완전히 차단하는 다운로드 유형을 구성합니다.

Microsoft Defender SmartScreen 경고가 있는 다운로드를 제외한 모든 다운로드를 허용하려면 '위험한 다운로드 차단'(1)을 설정하세요.

잠재적으로 위험한 다운로드에 대한 Microsoft Defender SmartScreen 경고가 있는 다운로드를 제외한 모든 다운로드를 허용하려면 '잠재적으로 위험한 다운로드 차단'(2)을 설정하세요.

모든 다운로드를 차단하려면 '모든 다운로드 차단'(3)을 설정하세요.

이 정책을 구성하지 않거나 '특별한 제한 없음'(0) 옵션을 설정하면 Microsoft Defender SmartScreen 분석 결과를 기반으로 하는 일반적인 보안 제한을 거쳐 다운로드가 수행됩니다.

참고: 이러한 제한은 웹 페이지 콘텐츠의 다운로드 뿐만 아니라 '다운로드 링크 ...' 상황에 맞는 메뉴 옵션에도 적용됩니다. 이러한 제한은 현재 표시된 페이지를 저장하거나 다운로드하는 데 적용되지 않으며 인쇄 옵션의 PDF로 저장 옵션에도 적용되지도 않습니다.

Microsoft Defender SmartScreen에 대한 자세한 내용은 [https://go.microsoft.com/fwlink/?linkid=2094934](https://go.microsoft.com/fwlink/?linkid=2094934)를 참조하세요.

* 0 = 특별한 제한 없음

* 1 = 위험한 다운로드 차단

* 2 = 잠재적으로 위험한 다운로드 차단

* 3 = 모든 다운로드 차단

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 예
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  정수

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: DownloadRestrictions
  - GP 이름: 다운로드 제한 허용
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 관리 템플릿/Microsoft Edge - 기본 설정(사용자가 재정의할 수 없음)/
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): SOFTWARE\Policies\Microsoft\Edge\맞춤
  - 값 이름: DownloadRestrictions
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000002
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: DownloadRestrictions
  - 예제 값:
``` xml
<integer>2</integer>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### EdgeCollectionsEnabled
  #### 컬렉션 기능 사용
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 78 이상부터

  #### 설명
  사용자가 Office 통합으로 콘텐츠를 보다 효율적으로 수집하고 구성하고 공유하고 내보낼 수 있는 컬렉션 기능에 액세스하도록 허용할 수 있습니다.

이 정책을 사용하거나 구성하지 않으면 사용자가 Microsoft Edge에서 컬렉션 기능에 액세스하여 사용할 수 있습니다.

이 정책을 사용하지 않으면 사용자가 Microsoft Edge에서 컬렉션에 액세스하여 사용할 수 없습니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 아니요 - 브라우저 다시 시작 필요

  #### 데이터 형식:
  부울

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: EdgeCollectionsEnabled
  - GP 이름: 컬렉션 기능 사용
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: EdgeCollectionsEnabled
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000001
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: EdgeCollectionsEnabled
  - 예제 값:
``` xml
<true/>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### EditFavoritesEnabled
  #### 사용자가 즐겨찾기를 편집할 수 있도록 허용
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  이 정책을 사용하도록 설정하면 사용자가 즐겨찾기를 추가, 제거 및 수정할 수 있습니다. 정책을 구성하지 않으면 이것이 기본 동작입니다.

이 정책을 사용하지 않도록 설정하면 사용자가 즐겨찾기를 추가, 제거 또는 수정할 수 없도록 중지합니다. 기존 즐겨찾기는 계속 사용할 수 있습니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  부울

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: EditFavoritesEnabled
  - GP 이름: 사용자가 즐겨찾기를 편집할 수 있도록 허용
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: EditFavoritesEnabled
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000000
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: EditFavoritesEnabled
  - 예제 값:
``` xml
<false/>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### EnableDeprecatedWebPlatformFeatures
  #### 제한된 기간 동안 사용되지 않은 웹 플랫폼 기능 다시 사용
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  일시적으로 다시 사용하도록 사용 중단된 기능을 일시적으로 다시 사용할 수 있게 웹 플랫폼 기능 목록을 지정합니다.

이 정책을 사용하면 제한된 기간 동안 사용 중단된 웹 플랫폼 기능을 다시 활성화할 수 있습니다.기능은 문자열 태그로 식별됩니다.

이 정책을 구성하지 않은 경우, 목록이 비어 있거나 또는 기능이 지원되는 문자열 태그 중 하나와 일치하지 않는 경우, 사용 중단된 웹 플랫폼 기능이 모두 사용 중지된 상태로 유지됩니다.

위의 플랫폼에서는 정책 자체가 지원되지만 모든 플랫폼에서 사용할 수는 없습니다. 사용 중단된 모든 웹 플랫폼 기능을 다시 사용할 수 있는 것은 아닙니다. 명시적으로 아래에 나열 된 기능만이, 기능에 따라 다른 제한된 시간동안 사용할 수 있습니다.https://bit.ly/blinkintents에서 웹 플랫폼 기능 변경의 의도를 검토 할 수 있습니다.

문자열 태그의 일반적인 형식은 [DeprecatedFeatureName]_EffectiveUntil[yyyymmdd]입니다.

* "ExampleDeprecatedFeature_EffectiveUntil20080902" = ExampleDeprecatedFeature API를 2008/09/02까지 사용하도록 설정

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  문자열 목록

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: EnableDeprecatedWebPlatformFeatures
  - GP 이름: 제한된 기간 동안 사용되지 않은 웹 플랫폼 기능 다시 사용
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge\EnableDeprecatedWebPlatformFeatures
  - 경로 (맞춤): 해당 없음
  - 값 이름: 1, 2, 3, ...
  - 값 형식: REG_SZ 목록
  ##### 예제 값:
```
SOFTWARE\Policies\Microsoft\Edge\EnableDeprecatedWebPlatformFeatures\0 = "ExampleDeprecatedFeature_EffectiveUntil20080902"

```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: EnableDeprecatedWebPlatformFeatures
  - 예제 값:
``` xml
<array>
  <string>ExampleDeprecatedFeature_EffectiveUntil20080902</string>
</array>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### EnableDomainActionsDownload
  #### Microsoft에서 도메인 작업 다운로드 사용
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  Microsoft Edge에서 도메인 작업은 브라우저가 웹에서 올바르게 작동 하는 데 도움이 되는 일련의 호환성 기능을 나타냅니다.

Microsoft는 호환성을 위해 특정 도메인에서 수행할 작업 목록을 유지합니다. 예를 들어, Microsoft Edge의 새 사용자 에이전트 문자열로 인해 브라우저가 손상된 경우 브라우저에서 웹 사이트의 사용자 에이전트 문자열을 재정의할 수 있습니다. 이러한 각 작업은 Microsoft가 사이트 소유자의 문제를 해결하려고 하는 동안 임시로 수행하기 위한 것입니다.

브라우저가 시작된 다음 주기적으로 실행되면 브라우저는 수행할 호환성 작업의 최신 목록까지 대부분이 포함된 실험 및 구성 서비스에 접속합니다. 이 목록은 서버의 복사본이 변경된 경우에만 후속 요청이 목록을 업데이트하도록 처음 검색된 후에 로컬로 저장됩니다.

이 정책을 사용하면 도메인 작업 목록이 실험 및 구성 서비스에서 계속 다운로드됩니다.

이 정책을 사용하지 않으면 도메인 작업 목록이 더 이상 실험 및 구성 서비스에서 다운로드되지 않습니다.

이 정책을 구성하지 않으면 도메인 작업 목록이 실험 및 구성 서비스에서 계속 다운로드됩니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  부울

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: EnableDomainActionsDownload
  - GP 이름: Microsoft에서 도메인 작업 다운로드 사용
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: EnableDomainActionsDownload
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000001
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: EnableDomainActionsDownload
  - 예제 값:
``` xml
<true/>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### EnableOnlineRevocationChecks
  #### 온라인 OCSP/CRL 검사 사용
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  온라인 해지 확인은 보안에 큰 이점을 제공하지 않으며 기본적으로 사용하지 않도록 설정되어 있습니다.

이 정책을 사용하면 Microsoft Edge가 소프트 오류, 온라인 OCSP/CRL 검사를 수행합니다. "소프트 오류"는 해지 서버에 연결할 수 없는 경우 인증서가 유효한 것으로 간주된다는 것을 의미합니다.

이 정책을 사용하지 않거나 구성하지 않으면 Microsoft Edge는 온라인 해지 검사를 수행하지 않습니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  부울

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: EnableOnlineRevocationChecks
  - GP 이름: 온라인 OCSP/CRL 검사 사용
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: EnableOnlineRevocationChecks
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000000
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: EnableOnlineRevocationChecks
  - 예제 값:
``` xml
<false/>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### EnterpriseHardwarePlatformAPIEnabled
  #### 관리되는 확장에서 엔터프라이즈 하드웨어 플랫폼 API를 사용하도록 허용
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 78 이상부터

  #### 설명
  이 정책을 사용하도록 설정하면 엔터프라이즈 정책에 의해 설치된 확장에서 엔터프라이즈 하드웨어 플랫폼 API를 사용할 수 있습니다.
이 정책을 사용하지 않도록 설정하거나 설정하지 않으면 확장이 엔터프라이즈 하드웨어 플랫폼 API를 사용할 수 없습니다.
이 정책은 구성 요소 확장에도 적용됩니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  부울

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: EnterpriseHardwarePlatformAPIEnabled
  - GP 이름: 관리되는 확장에서 엔터프라이즈 하드웨어 플랫폼 API를 사용하도록 허용
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: EnterpriseHardwarePlatformAPIEnabled
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000001
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: EnterpriseHardwarePlatformAPIEnabled
  - 예제 값:
``` xml
<true/>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### ExperimentationAndConfigurationServiceControl
  #### 실험 및 구성 서비스와의 통신 제어
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  Microsoft Edge에서 실험 및 구성 서비스는 실험 및 구성 페이로드를 배포하는 데 사용됩니다.

실험 페이로드는 Microsoft에서 테스트 및 피드백을 위해 사용하는 개발 기능의 초기 목록으로 구성 됩니다.

구성 페이로드는 Microsoft가 사용자 경험을 최적화하기 위해 Microsoft Edge에 배포하려는 설정 목록으로 구성됩니다. 예를 들어, 구성 페이로드는 Microsoft Edge가 새로운 페이로드를 검색하기 위해 실험 및 구성 서비스에 요청을 보내는 빈도를 지정할 수 있습니다.

이 정책을 "구성 및 실험 검색" 모드로 설정하면 실험 및 구성 서비스에서 전체 페이로드가 다운로드됩니다. 여기에는 실험 및 구성 페이로드가 모두 포함됩니다.

이 정책을 "구성만 검색" 모드로 설정하면 구성 페이로드만 전달됩니다.

이 정책을 "실험 및 구성 서비스와의 통신 사용 안 함" 모드로 설정하면 실험 및 구성 서비스와의 통신이 완전히 중지됩니다.

이 정책을 구성하지 않으면 안정적이 고 베타 채널의 관리되는 장치에서 "구성만 검색" 모드와 동일하게 작동합니다.

이 정책을 구성하지 않으면 관리되지 않는 장치에서 "구성 및 실험 검색" 모드의 동작과 같습니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  정수

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: ExperimentationAndConfigurationServiceControl
  - GP 이름: 실험 및 구성 서비스와의 통신 제어
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: ExperimentationAndConfigurationServiceControl
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000002
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: ExperimentationAndConfigurationServiceControl
  - 예제 값:
``` xml
<integer>2</integer>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### ExternalProtocolDialogShowAlwaysOpenCheckbox
  #### Show an "Always open" checkbox in external protocol dialog.
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 79 이상부터

  #### 설명
  This policy controls whether the "Always open" checkbox is shown on external protocol launch confirmation prompts.

If you set this policy to True, when an external protocol confirmation prompt is shown, the user can select "Always open". The user won’t get any future confirmation prompts for this protocol.

If you set this policy to False, or the policy is unset, the "Always open" checkbox isn’t displayed. The user will be prompted for confirmation every time an external protocol is invoked.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 아니요 - 브라우저 다시 시작 필요

  #### 데이터 형식:
  부울

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: ExternalProtocolDialogShowAlwaysOpenCheckbox
  - GP 이름: Show an "Always open" checkbox in external protocol dialog.
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: ExternalProtocolDialogShowAlwaysOpenCheckbox
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000001
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: ExternalProtocolDialogShowAlwaysOpenCheckbox
  - 예제 값:
``` xml
<true/>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### FavoritesBarEnabled
  #### 즐겨찾기 모음 사용
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  즐겨찾기 모음을 사용하거나 사용하지 않도록 설정합니다.

이 정책을 사용하면 즐겨찾기 모음이 표시됩니다.

이 정책을 사용하지 않으면 즐겨찾기 모음이 표시되지 않습니다.

이 정책이 구성되어 있지 않으면 사용자가 즐겨찾기 모음을 사용할지 여부를 결정할 수 있습니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 예
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  부울

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: FavoritesBarEnabled
  - GP 이름: 즐겨찾기 모음 사용
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 관리 템플릿/Microsoft Edge - 기본 설정(사용자가 재정의할 수 없음)/
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): SOFTWARE\Policies\Microsoft\Edge\맞춤
  - 값 이름: FavoritesBarEnabled
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000001
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: FavoritesBarEnabled
  - 예제 값:
``` xml
<true/>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### ForceBingSafeSearch
  #### Bing 유해 정보 차단 적용
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  Bing 웹 검색의 쿼리는 지정된 값으로 설정된 유해 정보 차단 설정으로 완료됩니다. 사용자는 이 설정을 변경할 수 없습니다.

이 정책을 "사용 안 함"으로 설정하면 Bing 검색의 유해 정보 차단이 bing.com 값으로 돌아갑니다.

이 정책을 "보통"으로 설정하면 유해 정보 차단에서 보통 설정이 사용됩니다. 보통 설정은 성인용 비디오 및 이미지를 필터링하지만 검색 결과에서 텍스트는 필터링하지 않습니다.

이 정책을 "엄격"으로 설정하면 유해 정보 차단의 엄격한 설정이 사용됩니다. 엄격한 설정은 성인용 텍스트, 이미지 및 비디오를 필터링합니다.

이 정책을 사용하지 않거나 구성하지 않으면 Bing 검색의 유해 정보 차단이 적용되지 않으며 사용자가 bing.com에서 원하는 값을 설정할 수 있습니다.

* 0 = Bing에서 검색 제한 구성 안 함

* 1 = Bing에서 보통 검색 제한 구성

* 2 = Bing에서 엄격한 검색 제한 구성

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  정수

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: ForceBingSafeSearch
  - GP 이름: Bing 유해 정보 차단 적용
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: ForceBingSafeSearch
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000000
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: ForceBingSafeSearch
  - 예제 값:
``` xml
<integer>0</integer>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### ForceEphemeralProfiles
  #### 임시 프로필 사용 설정
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  사용자 프로필이 임시 모드로 전환되는지 여부를 제어합니다. 임시 프로필은 세션이 시작될 때 만들어지고 세션이 끝날 때 삭제되며 사용자의 원래 프로필과 연결됩니다.

이 정책을 사용하면 프로필이 임시 모드로 실행됩니다. 이를 통해 사용자는 검색 데이터를 해당 장치에 저장하지 않고도 자신의 장치에서 작업할 수 있습니다. Windows에서 GPO를 사용하여 OS 정책으로 이 정책을 사용하면 시스템의 모든 프로필에 이 정책이 적용됩니다.

이 정책을 사용하지 않거나 구성하지 않으면 사용자가 브라우저에 로그인할 때 일반 프로필을 가져옵니다.

임시 모드에서는 프로필 데이터가 사용자 세션 동안에만 디스크에 저장됩니다. 브라우저 기록, 확장 및 해당 데이터, 쿠키와 같은 웹 데이터, 웹 데이터베이스 등의 기능은 브라우저를 닫은 후에 저장되지 않습니다. 이 경우 사용자가 수동으로 디스크에 데이터를 다운로드하거나 페이지를 저장하거나 인쇄하는 것을 막지 않습니다. 사용자가 동기화를 사용하도록 설정하면 일반 프로필과 마찬가지로 모든 데이터가 동기화 계정에 보존됩니다. 명시적으로 사용하지 않도록 설정하지 않는 한 사용자는 임시 모드에서 InPrivate 브라우징을 사용할 수도 있습니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 아니요 - 브라우저 다시 시작 필요

  #### 데이터 형식:
  부울

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: ForceEphemeralProfiles
  - GP 이름: 임시 프로필 사용 설정
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: ForceEphemeralProfiles
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000001
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: ForceEphemeralProfiles
  - 예제 값:
``` xml
<true/>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### ForceGoogleSafeSearch
  #### Google 유해 정보 차단 적용
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  유해 정보 차단이 활성으로 설정된 상태에서 수행되도록 Google 웹 검색의 쿼리를 강제로 적용하고 사용자가 이 설정을 변경하지 못하도록 합니다.

이 정책을 사용하면 Google 검색에서 유해 정보 차단이 항상 활성 상태입니다.

이 정책을 사용하지 않거나 구성하지 않으면 유해 정보 차단이 Google 검색에 적용되지 않습니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  부울

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: ForceGoogleSafeSearch
  - GP 이름: Google 유해 정보 차단 적용
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: ForceGoogleSafeSearch
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000000
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: ForceGoogleSafeSearch
  - 예제 값:
``` xml
<false/>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### ForceNetworkInProcess
  #### 네트워킹 코드가 브라우저 프로세스에서 실행되도록 강제
  >지원되는 버전: Windows의 Microsoft Edge, 버전 78 이상부터

  #### 설명
  이 정책은 네트워킹 코드가 브라우저 프로세스에서 실행되도록 강제합니다.

이 정책은 기본적으로 사용하지 않도록 설정되어 있으며 사용하도록 설정된 경우에는 네트워킹 프로세스가 샌드박스 처리될 때 사용자에게 보안 문제가 발생할 수 있습니다.

이 정책은 기업이 네트워킹 API 연결에 의존하지 않는 타사 소프트웨어로 마이그레이션 할 수 있는 기회를 제공하기 위한 것입니다. 프록시 서버는 LSP 및 Win32 API 패치보다 권장됩니다.

이 정책을 설정하지 않으면 NetworkService 실험의 필드 평가판에 따라 네트워킹 코드가 브라우저 프로세스에서 실행되지 않을 수 있습니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 아니요 - 브라우저 다시 시작 필요

  #### 데이터 형식:
  부울

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: ForceNetworkInProcess
  - GP 이름: 네트워킹 코드가 브라우저 프로세스에서 실행되도록 강제
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: ForceNetworkInProcess
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000000
```


  

  [맨 위로 이동](#microsoft-edge---정책)

  ### ForceYouTubeRestrict
  #### 최소 YouTube 제한 모드 강제 적용
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  YouTube에서 최소 제한 모드를 적용하고 사용자가 더 낮은 제한 모드를 선택할 수 없도록 합니다.

YouTube에서 엄격한 제한 모드를 적용하려면 엄격(2)으로 설정하세요.

사용자가 YouTube에서 보통 제한 모드 및 엄격한 제한 모드만 사용하도록 하려면 보통(1)으로 설정하세요. 제한 모드를 사용하지 않도록 설정할 수 없습니다.

YouTube에서 제한 모드를 적용하지 않도록 하려면 이 정책을 끄기(0)로 설정하거나 구성하지 마세요. YouTube 정책과 같은 외부 정책은 계속 제한 모드를 적용할 수 있습니다.

* 0 = YouTube에서 제한 모드 적용 안 함

* 1 = YouTube에서 보통 제한 모드 이상만 적용

* 2 = YouTube에서 엄격한 제한 모드 적용

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  정수

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: ForceYouTubeRestrict
  - GP 이름: 최소 YouTube 제한 모드 강제 적용
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: ForceYouTubeRestrict
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000000
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: ForceYouTubeRestrict
  - 예제 값:
``` xml
<integer>0</integer>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### FullscreenAllowed
  #### 전체 화면 모드 허용
  >지원되는 버전: Windows의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  전체 화면 모드의 사용 가능 여부를 설정합니다. 모든 Microsoft Edge UI가 숨겨지고 웹 콘텐츠만 표시됩니다.

이 정책을 사용하거나 구성하지 않으면 적절한 사용 권한이 있는 사용자, 앱 및 확장이 전체 화면 모드로 전환될 수 있습니다.

이 정책을 사용하지 않으면 사용자, 앱 및 확장이 전체 화면 모드로 전환될 수 없습니다.

전체 화면 모드를 사용하지 않으면 명령줄을 사용하여 키오스크 모드에서 Microsoft Edge를 열 수 없습니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  부울

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: FullscreenAllowed
  - GP 이름: 전체 화면 모드 허용
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: FullscreenAllowed
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000001
```


  

  [맨 위로 이동](#microsoft-edge---정책)

  ### GoToIntranetSiteForSingleWordEntryInAddressBar
  #### 주소 표시줄에서 단일 단어 항목을 검색하는 대신 직접 인트라넷 사이트 탐색을 강제합니다.
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 78 이상부터

  #### 설명
  이 정책을 사용하면 주소 표시줄에 입력한 텍스트가 문장 부호가 없는 단일 단어인 경우 주소 표시줄 추천 단어 목록에서 최상위 자동 추천 결과는 인트라넷 사이트로 이동합니다.

문장 부호 없이 단일 단어를 입력하면 기본 탐색은 입력한 텍스트와 일치하는 인트라넷 사이트를 탐색합니다.

이 정책을 사용하면 이 텍스트가 문장 부호 없는 단일 단어인 경우 주소 표시줄 추천 단어 목록의 두 번째 자동 추천 결과는 입력한 텍스트 그대로 웹 검색을 수행합니다. 웹 검색을 금지하는 정책도 사용하지 않도록 설정하지 않는 한 기본 검색 공급자가 사용됩니다.

이 정책을 사용하면 다음과 같은 두 가지 효과가 있습니다.

기록 항목으로 해석되는 단일 단어 쿼리에 대한 응답으로 사이트 탐색이 더 이상 사이트를 탐색하지 않습니다. 대신, 브라우저는 조직의 인트라넷에 없을 수 있는 내부 사이트를 탐색합니다. 이로 인해 404 오류가 발생합니다.

인기 있는 단일 단어 검색어는 검색을 올바르게 수행하려면 검색 추천을 수동으로 선택해야 합니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  부울

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: GoToIntranetSiteForSingleWordEntryInAddressBar
  - GP 이름: 주소 표시줄에서 단일 단어 항목을 검색하는 대신 직접 인트라넷 사이트 탐색을 강제합니다.
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: GoToIntranetSiteForSingleWordEntryInAddressBar
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000000
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: GoToIntranetSiteForSingleWordEntryInAddressBar
  - 예제 값:
``` xml
<false/>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### HSTSPolicyBypassList
  #### HSTS 정책 확인을 무시할 이름 목록 구성
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 79 이상부터

  #### 설명
  이 목록에 지정된 호스트 이름은 요청을 "http://"에서 "https://"로 업그레이드할 수 있는 HSTS 정책 확인에서 제외됩니다. 이 정책에서는 단일 레이블 호스트 이름만 허용됩니다. 호스트 이름은 정규화되어야 합니다. 모든 IDN은 A 레이블 형식으로 변환되어야 하며 모든 ASCII 문자는 소문자여야 합니다. 이 정책은 지정된 특정 호스트 이름에만 적용됩니다. 목록에 있는 이름의 하위 도메인에는 적용되지 않습니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 아니요 - 브라우저 다시 시작 필요

  #### 데이터 형식:
  문자열 목록

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: HSTSPolicyBypassList
  - GP 이름: HSTS 정책 확인을 무시할 이름 목록 구성
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge\HSTSPolicyBypassList
  - 경로 (맞춤): 해당 없음
  - 값 이름: 1, 2, 3, ...
  - 값 형식: REG_SZ 목록
  ##### 예제 값:
```
SOFTWARE\Policies\Microsoft\Edge\HSTSPolicyBypassList\0 = "meet"

```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: HSTSPolicyBypassList
  - 예제 값:
``` xml
<array>
  <string>meet</string>
</array>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### HardwareAccelerationModeEnabled
  #### 가능한 경우 하드웨어 가속 사용
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  사용 가능한 경우 하드웨어 가속을 사용하도록 지정합니다. 이 정책을 사용하거나 구성하지 않으면 GPU 기능이 명시적으로 차단되어 있지 않는 한 하드웨어 가속이 활성화됩니다.

이 정책을 사용하지 않으면 하드웨어 가속이 비활성화됩니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 아니요 - 브라우저 다시 시작 필요

  #### 데이터 형식:
  부울

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: HardwareAccelerationModeEnabled
  - GP 이름: 가능한 경우 하드웨어 가속 사용
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: HardwareAccelerationModeEnabled
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000001
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: HardwareAccelerationModeEnabled
  - 예제 값:
``` xml
<true/>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### ImportAutofillFormData
  #### 자동 채우기 양식 데이터 가져오기 허용
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  사용자가 다른 브라우저에서 자동 채우기 양식 데이터를 Microsoft Edge로 가져올 수 있도록 허용합니다.

이 정책을 사용하면 자동 채우기 양식 데이터를 수동으로 가져오는 옵션이 자동으로 선택됩니다.

이 정책을 사용하지 않으면 처음 실행 시 자동 채우기 양식 데이터를 가져오지 않으며 사용자가 수동으로 가져올 수 없습니다.

이 정책을 구성하지 않으면 처음 실행 시 자동 채우기 양식 데이터를 가져오고 사용자는 나중에 검색 세션 동안 이 데이터를 수동으로 가져올지 여부를 선택할 수 있습니다.

이 정책을 권장 사항으로 설정할 수 있습니다. 즉, Microsoft Edge가 처음 실행 시 자동 채우기 양식 데이터를 가져오지만 사용자가 수동 가져오기 중에 **자동 채우기 데이터** 옵션을 선택하거나 선택을 취소할 수 있습니다.

**참고**: 이 정책은 현재 Internet Explorer(Windows 7, 8 및 10, macOS의 경우)에서 가져오기를 관리합니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 예
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  부울

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: ImportAutofillFormData
  - GP 이름: 자동 채우기 양식 데이터 가져오기 허용
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 관리 템플릿/Microsoft Edge - 기본 설정(사용자가 재정의할 수 없음)/
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): SOFTWARE\Policies\Microsoft\Edge\맞춤
  - 값 이름: ImportAutofillFormData
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000001
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: ImportAutofillFormData
  - 예제 값:
``` xml
<true/>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### ImportBrowserSettings
  #### 브라우저 설정 가져오기 허용
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 78 이상부터

  #### 설명
  사용자가 다른 브라우저에서 Microsoft Edge에 대한 브라우저 설정을 가져올 수 있도록 허용합니다.

이 정책을 사용하면 **브라우저 데이터 가져오기** 대화 상자에서 **브라우저 설정** 확인란이 자동으로 선택됩니다.

이 정책을 사용하지 않으면 처음 실행 시 브라우저 설정을 가져오지 않으며 사용자가 수동으로 가져올 수 없습니다.

이 정책을 구성하지 않으면 처음 실행시 브라우저 설정을 가져오고 사용자는 나중에 검색 세션 동안 수동으로 가져올지 여부를 선택할 수 있습니다.

이 정책을 권장 사항으로 설정할 수도 있습니다. 즉, Microsoft Edge가 처음 실행될 때 설정을 가져오지만 용자는 수동 가져 오기 중에 ** 브라우저 설정 ** 옵션을 선택하거나 지울 수 있습니다.

**참고**:이 정책은 현재 Chrome (Windows 7, 8 및 10 및 macOS) 가져 오기를 관리합니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 예
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  부울

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: ImportBrowserSettings
  - GP 이름: 브라우저 설정 가져오기 허용
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 관리 템플릿/Microsoft Edge - 기본 설정(사용자가 재정의할 수 없음)/
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): SOFTWARE\Policies\Microsoft\Edge\맞춤
  - 값 이름: ImportBrowserSettings
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000001
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: ImportBrowserSettings
  - 예제 값:
``` xml
<true/>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### ImportFavorites
  #### 즐겨찾기 가져오기 허용
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  사용자가 다른 브라우저에서 즐겨찾기를 Microsoft Edge로 가져올 수 있도록 허용합니다.

이 정책을 사용하면 **브라우저 데이터 가져오기** 대화 상자에서 **즐겨찾기** 확인란이 자동으로 선택됩니다.

이 정책을 사용하지 않으면 처음 실행 시 즐겨찾기를 가져오지 않으며 사용자가 이 데이터를 수동으로 가져올 수 없습니다.

이 정책을 구성하지 않으면 처음 실행 시 즐겨찾기를 가져오고 사용자는 나중에 검색 세션 동안 수동으로 가져올지 여부를 선택할 수 있습니다.

이 정책을 권장 사항으로 설정할 수도 있습니다. 즉, Microsoft Edge가 처음 실행 시 즐겨찾기를 가져오지만 사용자가 수동 가져오기 중에 **즐겨찾기** 옵션을 선택하거나 선택을 취소할 수 있습니다.

**참고**: 이 정책은 현재 Internet Explorer(Windows 7, 8 및 10의 경우), Google Chrome(Windows 7, 8 및 10, macOS의 경우) 및 Apple Safari(macOS의 경우) 브라우저에서 가져오기를 관리합니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 예
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  부울

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: ImportFavorites
  - GP 이름: 즐겨찾기 가져오기 허용
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 관리 템플릿/Microsoft Edge - 기본 설정(사용자가 재정의할 수 없음)/
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): SOFTWARE\Policies\Microsoft\Edge\맞춤
  - 값 이름: ImportFavorites
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000001
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: ImportFavorites
  - 예제 값:
``` xml
<true/>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### ImportHistory
  #### 검색 기록 가져오기 허용
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  사용자가 다른 브라우저에서 검색 기록을 Microsoft Edge로 가져올 수 있도록 허용합니다.

이 정책을 사용하면 **브라우저 데이터 가져오기** 대화 상자에서 **검색 기록** 확인란이 자동으로 선택됩니다.

이 정책을 사용하지 않으면 처음 실행 시 검색 기록 데이터를 가져오지 않으며 사용자가 이 데이터를 수동으로 가져올 수 없습니다.

이 정책을 구성하지 않으면 처음 실행 시 검색 기록 데이터를 가져오고 사용자는 나중에 검색 세션 동안 수동으로 가져올지 여부를 선택할 수 있습니다.

이 정책을 권장 사항으로 설정할 수도 있습니다. 즉, Microsoft Edge가 처음 실행 시 검색 기록을 가져오지만 사용자가 수동 가져오기 중에 **검색 기록** 옵션을 선택하거나 선택을 취소할 수 있습니다.

**참고**: 이 정책은 현재 Internet Explorer(Windows 7, 8 및 10의 경우), Google Chrome(Windows 7, 8 및 10, macOS의 경우) 및 Apple Safari(macOS) 브라우저에서 가져오기를 관리합니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 예
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  부울

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: ImportHistory
  - GP 이름: 검색 기록 가져오기 허용
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 관리 템플릿/Microsoft Edge - 기본 설정(사용자가 재정의할 수 없음)/
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): SOFTWARE\Policies\Microsoft\Edge\맞춤
  - 값 이름: ImportHistory
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000001
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: ImportHistory
  - 예제 값:
``` xml
<true/>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### ImportHomepage
  #### 홈 페이지 설정 가져오기 허용
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  사용자가 다른 브라우저에서 홈 페이지 설정을 Microsoft Edge로 가져올 수 있도록 허용합니다.

이 정책을 사용하면 홈 페이지 설정을 수동으로 가져오는 옵션이 자동으로 선택됩니다.

이 정책을 사용하지 않으면 처음 실행 시 홈 페이지 설정을 가져오지 않으며 사용자가 수동으로 가져올 수 없습니다.

이 정책을 구성하지 않으면 처음 실행 시 홈 페이지 설정을 가져오고 사용자는 나중에 검색 세션 동안 이 데이터를 수동으로 가져올지 여부를 선택할 수 있습니다.

이 정책을 권장 사항으로 설정할 수 있습니다. 즉, Microsoft Edge가 처음 실행 시 홈 페이지 설정을 가져오지만 사용자가 수동 가져오기 중에 **홈 페이지** 옵션을 선택하거나 선택을 취소할 수 있습니다.

**참고**: 이 정책은 현재 Internet Explorer(Windows 7, 8 및 10의 경우)에서 가져오기를 관리합니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  부울

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: ImportHomepage
  - GP 이름: 홈 페이지 설정 가져오기 허용
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: ImportHomepage
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000001
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: ImportHomepage
  - 예제 값:
``` xml
<true/>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### ImportOpenTabs
  #### 열린 탭 가져오기 허용
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 79 이상부터

  #### 설명
  사용자가 다른 브라우저에서 열려 있고 고정된 탭을 Microsoft Edge로 가져올 수 있도록 허용합니다.

이 정책을 사용하면 **브라우저 데이터 가져 오기** 대화 상자에서 **열립 탭** 확인란이 자동으로 선택됩니다.

이 정책을 사용하지 않으면 처음 실행 시 브라우저 설정을 가져오지 않으며 사용자가 수동으로 가져올 수 없습니다.

이 정책을 구성하지 않으면 처음 실행 시 열린 탭을 가져오고 사용자는 나중에 검색 세션 동안 수동으로 가져올지 여부를 선택할 수 있습니다.

이 정책을 권장 사항으로 설정할 수도 있습니다. 즉, Microsoft Edge가 처음 실행될 때 열린 탭을 가져오지만 사용자는 수동 가져오기 중에 **열린 탭** 옵션을 선택하거나 지울 수 있습니다.

**참고**: 이 정책은 현재 Google Chrome(Windows 7, 8 및 10 및 macOS)에서 가져오기만 지원합니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 예
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  부울

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: ImportOpenTabs
  - GP 이름: 열린 탭 가져오기 허용
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 관리 템플릿/Microsoft Edge - 기본 설정(사용자가 재정의할 수 없음)/
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): SOFTWARE\Policies\Microsoft\Edge\맞춤
  - 값 이름: ImportOpenTabs
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000001
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: ImportOpenTabs
  - 예제 값:
``` xml
<true/>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### ImportPaymentInfo
  #### 결제 정보 가져오기 허용
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  사용자가 다른 브라우저에서 결제 정보를 Microsoft Edge로 가져올 수 있도록 허용합니다.

이 정책을 사용하면 **브라우저 데이터 가져오기** 대화 상자에서 **결제 정보** 확인란이 자동으로 선택됩니다.

이 정책을 사용하지 않으면 처음 실행 시 결제 정보를 가져오지 않으며 사용자가 수동으로 가져올 수 없습니다.

이 정책을 구성하지 않으면 처음 실행 시 결제 정보를 가져오고 사용자는 나중에 검색 세션 동안 수동으로 가져올지 여부를 선택할 수 있습니다.

이 정책을 권장 사항으로 설정할 수도 있습니다. 즉, Microsoft Edge가 처음 실행 시 결제 정보를 가져오지만 사용자가 수동 가져오기 중에 **결제 정보** 옵션을 선택하거나 선택을 취소할 수 있습니다.

**참고**: 이 정책은 현재 Google Chrome(Windows 7, 8 및 10, macOS)에서 가져오기를 관리합니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 예
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  부울

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: ImportPaymentInfo
  - GP 이름: 결제 정보 가져오기 허용
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 관리 템플릿/Microsoft Edge - 기본 설정(사용자가 재정의할 수 없음)/
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): SOFTWARE\Policies\Microsoft\Edge\맞춤
  - 값 이름: ImportPaymentInfo
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000001
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: ImportPaymentInfo
  - 예제 값:
``` xml
<true/>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### ImportSavedPasswords
  #### 저장된 암호 가져오기 허용
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  사용자가 다른 브라우저에서 저장된 암호를 Microsoft Edge로 가져올 수 있도록 허용합니다.

이 정책을 사용하면 저장된 암호를 수동으로 가져오는 옵션이 자동으로 선택됩니다.

이 정책을 사용하지 않으면 저장된 암호를 처음 실행 시 가져오지 않으며 사용자가 수동으로 가져올 수 없습니다.

이 정책을 구성하지 않으면 처음 실행 시 암호를 가져오고 사용자는 나중에 검색 세션 동안 수동으로 가져올지 여부를 선택할 수 있습니다.

이 정책을 권장 사항으로 설정할 수 있습니다. 즉, Microsoft Edge가 처음 실행 시 암호를 가져오지만 사용자가 수동 가져오기 동안 **암호** 옵션을 선택하거나 선택을 취소할 수 있습니다.

**참고**: 이 정책은 현재 Internet Explorer(Windows 7, 8 및 10의 경우) 및 Google Chrome(Windows 7, 8 및 10, macOS의 경우) 브라우저에서 가져오기를 관리합니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 예
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  부울

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: ImportSavedPasswords
  - GP 이름: 저장된 암호 가져오기 허용
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 관리 템플릿/Microsoft Edge - 기본 설정(사용자가 재정의할 수 없음)/
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): SOFTWARE\Policies\Microsoft\Edge\맞춤
  - 값 이름: ImportSavedPasswords
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000001
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: ImportSavedPasswords
  - 예제 값:
``` xml
<true/>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### ImportSearchEngine
  #### 검색 엔진 설정 가져오기 허용
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  사용자가 다른 브라우저에서 검색 엔진 설정을 Microsoft Edge로 가져올 수 있도록 허용합니다.

이 정책을 사용하면 검색 엔진 설정을 가져오는 옵션이 자동으로 선택됩니다.

이 정책을 사용하지 않으면 처음 실행 시 검색 엔진 설정을 가져오지 않으며 사용자가 수동으로 가져올 수 없습니다.

이 정책을 구성하지 않으면 처음 실행 시 검색 엔진 설정을 가져오고 사용자는 나중에 검색 세션 동안 이 데이터를 수동으로 가져올지 여부를 선택할 수 있습니다.

이 정책을 권장 사항으로 설정할 수 있습니다. 즉, Microsoft Edge가 처음 실행 시 검색 엔진 설정을 가져오지만 사용자가 수동 가져오기 중에 **검색 엔진** 옵션을 선택하거나 선택을 취소할 수 있습니다.

**참고**: 이 정책은 현재 Internet Explorer(Windows 7, 8 및 10의 경우)에서 가져오기를 관리합니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 예
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  부울

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: ImportSearchEngine
  - GP 이름: 검색 엔진 설정 가져오기 허용
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 관리 템플릿/Microsoft Edge - 기본 설정(사용자가 재정의할 수 없음)/
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): SOFTWARE\Policies\Microsoft\Edge\맞춤
  - 값 이름: ImportSearchEngine
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000001
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: ImportSearchEngine
  - 예제 값:
``` xml
<true/>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### InPrivateModeAvailability
  #### InPrivate 모드 가용성 구성
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  Microsoft Edge에서 사용자가 InPrivate 모드로 페이지를 열 수 있는지 여부를 지정합니다.

이 정책을 구성하지 않거나 '사용'(0)으로 설정하면 사용자가 InPrivate 모드로 페이지를 열 수 있습니다.

사용자가 InPrivate 모드를 사용하지 못하게 하려면 이 정책을 '사용 안 함'(1)으로 설정하세요.

항상 InPrivate 모드를 사용하려면 이 정책을 '강제'(2)로 설정하세요.

* 0 = InPrivate 모드 사용 가능

* 1 = InPrivate 모드 사용 안 함

* 2 = InPrivate 모드 강제

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  정수

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: InPrivateModeAvailability
  - GP 이름: InPrivate 모드 가용성 구성
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: InPrivateModeAvailability
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000001
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: InPrivateModeAvailability
  - 예제 값:
``` xml
<integer>1</integer>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### InternetExplorerIntegrationLevel
  #### Internet Explorer 통합 구성
  >지원되는 버전: Windows의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  Internet Explorer 모드를 위한 최적의 환경을 구성하는 방법에 대한 지침은 [https://go.microsoft.com/fwlink/?linkid=2094210](https://go.microsoft.com/fwlink/?linkid=2094210)를 참조하세요.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 아니요 - 브라우저 다시 시작 필요

  #### 데이터 형식:
  정수

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: InternetExplorerIntegrationLevel
  - GP 이름: Internet Explorer 통합 구성
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: InternetExplorerIntegrationLevel
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000001
```


  

  [맨 위로 이동](#microsoft-edge---정책)

  ### InternetExplorerIntegrationSiteList
  #### 엔터프라이즈 모드 사이트 목록 구성
  >지원되는 버전: Windows의 Microsoft Edge, 버전 78 이상부터

  #### 설명
  Internet Explorer 모드를 위한 최적의 환경을 구성하는 방법에 대한 지침은 [https://go.microsoft.com/fwlink/?linkid=2094210](https://go.microsoft.com/fwlink/?linkid=2094210)를 참조하세요.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 아니요 - 브라우저 다시 시작 필요

  #### 데이터 형식:
  문자열

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: InternetExplorerIntegrationSiteList
  - GP 이름: 엔터프라이즈 모드 사이트 목록 구성
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: InternetExplorerIntegrationSiteList
  - 값 형식: REG_SZ
  ##### 예제 값:
```
"https://internal.contoso.com/sitelist.xml"
```


  

  [맨 위로 이동](#microsoft-edge---정책)

  ### InternetExplorerIntegrationSiteRedirect
  #### Internet Explorer 모드 페이지에서 시작할 때 구성되지 않은 사이트에 대한 "페이지 내" 탐색 작동 방식 지정
  >지원되는 버전: Windows의 Microsoft Edge, 버전 79 이상부터

  #### 설명
  An "in-page" navigation is started from a link, a script, or a form on the current page. It can also be a server-side redirect of a previous "in-page" navigation attempt. Conversely, a user can start a navigation that isn't "in-page" that's independent of the current page in several ways by using the browser controls. For example, using the address bar, the back button, or a favorite link.

This setting lets you specify whether navigations from pages loaded in Internet Explorer mode to unconfigured sites (that are not configured in the Enterprise Mode Site List) switch back to Microsoft Edge or remain in Internet Explorer mode.

This setting works in conjunction with:
[InternetExplorerIntegrationLevel](#internetexplorerintegrationlevel) is set to "Internet Explorer mode" (1)
and
[InternetExplorerIntegrationSiteList](#internetexplorerintegrationsitelist) policy where the list has at least one entry.

If you disable or don’t configure this policy, only sites configured to open in Internet Explorer mode will open in that mode. Any site not configured to open in Internet Explorer mode will be redirected back to Microsoft Edge.

If you enable this policy, you can choose one of the following navigation options:
0 - Default. Only sites configured to open in Internet Explorer mode will open in that mode. Any site not configured to open in Internet Explorer mode will be redirected back to Microsoft Edge.
1 - Keep only automatic navigations in Internet Explorer mode. Use this option If you want the default experience except that all automatic navigations (such as 302 redirects) to unconfigured sites will be kept in Internet Explorer mode.
2 - Keep all in-page navigations in Internet Explorer mode (Least Recommended). All navigations from pages loaded in IE mode to unconfigured sites are kept in Internet Explorer mode.

To learn more about Internet Explorer mode, see [https://go.microsoft.com/fwlink/?linkid=2105106](https://go.microsoft.com/fwlink/?linkid=2105106)

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 아니요 - 브라우저 다시 시작 필요

  #### 데이터 형식:
  정수

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: InternetExplorerIntegrationSiteRedirect
  - GP 이름: Internet Explorer 모드 페이지에서 시작할 때 구성되지 않은 사이트에 대한 "페이지 내" 탐색 작동 방식 지정
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: InternetExplorerIntegrationSiteRedirect
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000000
```


  

  [맨 위로 이동](#microsoft-edge---정책)

  ### IsolateOrigins
  #### 특정 원본에 대해 사이트 격리 사용
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  Specify origins to run in isolation, in their own process.
This policy also isolates origins named by subdomains - for example, specifying https://contoso.com/ will cause https://foo.contoso.com/ to be isolated as part of the https://contoso.com/ site.
If the policy is enabled, each of the named origins in a comma-separated list will run in its own process.
If you disable this policy, then both the 'IsolateOrigins' and 'SitePerProcess' features are disabled. Users can still enable 'IsolateOrigins' policy manually, via command line flags.
If you don't configure the policy, the user can change this setting.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 아니요 - 브라우저 다시 시작 필요

  #### 데이터 형식:
  문자열

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: IsolateOrigins
  - GP 이름: 특정 원본에 대해 사이트 격리 사용
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: IsolateOrigins
  - 값 형식: REG_SZ
  ##### 예제 값:
```
"https://contoso.com/,https://fabrikam.com/"
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: IsolateOrigins
  - 예제 값:
``` xml
<string>https://contoso.com/,https://fabrikam.com/</string>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### ManagedFavorites
  #### 즐겨찾기 구성
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  관리되는 즐겨 찾기 목록을 구성합니다.

정책은 즐겨찾기 목록을 만듭니다. 각 즐겨찾기에는 즐겨찾기의 이름과 대상을 포함하는 "이름" 및 "URL" 키가 있습니다. "URL" 키는 없으나 위에 정의된 즐겨찾기 목록을 포함하는 추가 "자식" 키는 있는 즐겨찾기를 정의하여 하위 폴더를 구성할 수 있습니다(일부는 폴더일 수 있음). Microsoft Edge는 주소 표시줄을 통해 제출된 것처럼 불완전한 URL을 수정합니다. 예를 들어 "microsoft.com"은 "https://microsoft.com/"로 바뀝니다.

이러한 즐겨찾기는 사용자가 수정할 수 없는 폴더에 저장됩니다. 그러나 사용자가 즐겨찾기 모음에서 숨길 수 있습니다. 기본적으로 폴더 이름은 "관리되는 즐겨찾기"이지만 "toplevel_name" 키가 포함된 사전을 즐겨찾기 목록에 추가하여 원하는 폴더 이름을 값으로 변경할 수 있습니다.

관리되는 즐겨찾기는 사용자 계정에 동기화되지 않으며 확장에 의해 수정될 수 없습니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  사전

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: ManagedFavorites
  - GP 이름: 즐겨찾기 구성
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: ManagedFavorites
  - 값 형식: REG_SZ
  ##### 예제 값:
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


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: ManagedFavorites
  - 예제 값:
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
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### ManagedSearchEngines
  #### 검색 엔진 관리
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  Lets you configure a list of list of up to 10 search engines, one of which must be marked as the default search engine.
You do not need to specify the encoding for any search engine.

If you enable this policy, users can't add, remove, or change any search engine in the list. Users can set their default search engine to any search engine in the list.

If you disable or don't configure this policy, users can modify the search engines list as desired.

If the [DefaultSearchProviderSearchURL](#defaultsearchprovidersearchurl) policy is set, this policy (ManagedSearchEngines) is ignored. The user must restart their browser to finish applying this policy.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 아니요 - 브라우저 다시 시작 필요

  #### 데이터 형식:
  사전

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: ManagedSearchEngines
  - GP 이름: 검색 엔진 관리
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: ManagedSearchEngines
  - 값 형식: REG_SZ
  ##### 예제 값:
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


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: ManagedSearchEngines
  - 예제 값:
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
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### MaxConnectionsPerProxy
  #### 프록시 서버에 대 한 동시 연결의 최대 수
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  프록시 서버에 대한 최대 동시 연결 수를 지정합니다.

일부 프록시 서버는 클라이언트 당 많은 수의 동시 연결을 처리할 수 없으므로 이 정책을 더 낮은 값으로 설정하여 해당 문제를 해결할 수 있습니다.

이 정책의 값은 100보다 작고 6보다 커야 합니다. 기본값은 32입니다.

일부 웹 앱은 GET을 사용하여 많은 연결을 사용하는 것으로 알려져 있습니다. 최대 연결을 32개 아래로 낮추거나 이러한 종류의 웹 응용 프로그램이 너무 많이 열려 있으면 브라우저 네트워킹이 중단될 수 있습니다.

이 정책을 구성하지 않으면 기본값 (32)이 사용됩니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 아니요 - 브라우저 다시 시작 필요

  #### 데이터 형식:
  정수

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: MaxConnectionsPerProxy
  - GP 이름: 프록시 서버에 대 한 동시 연결의 최대 수
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: MaxConnectionsPerProxy
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000020
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: MaxConnectionsPerProxy
  - 예제 값:
``` xml
<integer>32</integer>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### MediaRouterCastAllowAllIPs
  #### Google Cast가 모든 IP 주소의 캐스트 장치에 연결하도록 허용
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  Enable this policy to let Google Cast connect to Cast devices on all IP addresses, not just RFC1918/RFC4193 private addresses.

Disable this policy to restrict Google Cast to Cast devices on RFC1918/RFC4193 private addresses.

If you don't configure this policy, Google Cast connects to Cast devices on RFC1918/RFC4193 private addresses only, unless you enable the CastAllowAllIPs feature.

If the [EnableMediaRouter](#enablemediarouter) policy is disabled, then this policy has no effect.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  부울

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: MediaRouterCastAllowAllIPs
  - GP 이름: Google Cast가 모든 IP 주소의 캐스트 장치에 연결하도록 허용
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: MediaRouterCastAllowAllIPs
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000000
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: MediaRouterCastAllowAllIPs
  - 예제 값:
``` xml
<false/>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### MetricsReportingEnabled
  #### 사용 현황 및 크래시 관련 데이터 보고 사용
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  Microsoft Edge의 Windows 10 Beta 및 Stable 채널의 경우 이 정책을 구성하면 컬렉션 또는 컬렉션이 아닌 Microsoft Edge 사용량 및 크래시 관련 데이터에 대한 Windows 진단 데이터 설정을 재정의합니다([https://go.microsoft.com/fwlink/?linkid=2099569](https://go.microsoft.com/fwlink/?linkid=2099569)).

이 정책은 Microsoft Edge에 대한 사용량 및 크래시 관련 데이터를 Microsoft에 보고하는 것을 사용하도록 설정하며 사용자가 이 설정을 변경할 수 없도록 합니다.

사용량 및 크래시 관련 데이터 보고를 Microsoft에 보내려면 이 정책을 사용하도록 설정하세요. 데이터를 Microsoft로 보내지 않으려면 이 정책을 사용하지 않도록 설정하세요. 두 경우 모두 사용자가 설정을 변경하거나 재정의할 수 없습니다.

Windows 10, Beta 및 Stable 채널에서 이 정책은 사용량 및 크래시 관련 데이터를 제어합니다. 이 정책을 구성하지 않으면 Microsoft Edge에서 Windows 진단 데이터 설정을 기본값으로 합니다.

Windows 10, Canary 및 Dev 채널에서 이 정책은 사용량 및 크래시 관련 데이터를 제어합니다. 이 정책을 구성하지 않으면 Microsoft Edge에서 사용자의 기본 설정을 기본값으로 합니다.

Windows 7, 8 및 Mac에서는 이 정책이 사용량 및 크래시 관련 데이터를 제어합니다. 이 정책을 구성하지 않으면 Microsoft Edge에서 사용자의 기본 설정을 기본값으로 합니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 아니요 - 브라우저 다시 시작 필요

  #### 데이터 형식:
  부울

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: MetricsReportingEnabled
  - GP 이름: 사용 현황 및 크래시 관련 데이터 보고 사용
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: MetricsReportingEnabled
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000001
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: MetricsReportingEnabled
  - 예제 값:
``` xml
<true/>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### NetworkPredictionOptions
  #### 네트워크 예측 사용
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  네트워크 예측을 사용하도록 설정하고 사용자가 이 설정을 변경할 수 없게 합니다.

이 기능은 DNS 프리페치, TCP 및 SSL 사전 연결 및 웹 페이지 사전 렌더링을 제어합니다.

이 정책을 구성하지 않으면 네트워크 예측은 사용하도록 설정되지만 사용자가 변경할 수 있습니다.

* 0 = 모든 네트워크 연결에서 네트워크 작업 예측

* 2 = 모든 네트워크 연결에서 네트워크 작업 예측 안 함

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 예
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  정수

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: NetworkPredictionOptions
  - GP 이름: 네트워크 예측 사용
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 관리 템플릿/Microsoft Edge - 기본 설정(사용자가 재정의할 수 없음)/
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): SOFTWARE\Policies\Microsoft\Edge\맞춤
  - 값 이름: NetworkPredictionOptions
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000001
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: NetworkPredictionOptions
  - 예제 값:
``` xml
<integer>1</integer>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### NonRemovableProfileEnabled
  #### 사용자가 회사 또는 학교 계정으로 자동으로 로그인한 기본 프로필을 항상 가지고 있는지 여부를 구성합니다.
  >지원되는 버전: Windows의 Microsoft Edge, 버전 78 이상부터

  #### 설명
  This policy determines if the Microsoft Edge profile automatically signed in with a user's work or school account is removable.

If you enable or don't configure this policy, a non-removable profile will be created with the user's work or school account on Windows. This profile can't be signed out or removed.

When you disable this policy, the profile automatically signed in with a user's work or school account from Windows can be signed out or removed by the user.

If you want to completely disable browser sign in, use the 'BrowserSignIn' policy.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  부울

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: NonRemovableProfileEnabled
  - GP 이름: 사용자가 회사 또는 학교 계정으로 자동으로 로그인한 기본 프로필을 항상 가지고 있는지 여부를 구성합니다.
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: NonRemovableProfileEnabled
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000001
```


  

  [맨 위로 이동](#microsoft-edge---정책)

  ### OverrideSecurityRestrictionsOnInsecureOrigin
  #### 안전하지 않은 원본에 대한 보안 제한이 적용되는 위치 제어
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  보안되지 않은 출처에 대한 보안 제한이 적용되지 않는 원본 (URL) 또는 호스트 이름 패턴 (예: "* .contoso.com") 목록을 지정합니다.

이 정책을 사용하면 TLS를 배포할 수 없는 레거시 응용 프로그램의 허용된 원본을 지정하거나 개발자가 준비 서버에서 TLS를 배포하지 않고도 보안 컨텍스트가 필요한 기능을 테스트할 수 있도록 내부 웹 개발을 위한 준비 서버를 설정할 수 있습니다.레거시 응용 프로그램에 대 한 원본을 사용할 수 있습니다. 이 정책은 또한 출처가 검색 주소창에서 "안전하지 않음"으로 표시되는 것을 방지합니다.

이 정책에서 URL 목록을 설정하면 명령줄 플래그 '--unsafely-treat-insecure-origin-as-secure'를 동일한 URL의 쉼표로 구분 된 목록으로 설정하는 것과 같은 효과가 있습니다. 이 정책을 사용하면 명령줄 플래그가 재정의됩니다.

보안 컨텍스트에 대한 자세한 내용은 https://www.w3.org/TR/secure-contexts/를 참조하세요.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 아니요 - 브라우저 다시 시작 필요

  #### 데이터 형식:
  문자열 목록

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: OverrideSecurityRestrictionsOnInsecureOrigin
  - GP 이름: 안전하지 않은 원본에 대한 보안 제한이 적용되는 위치 제어
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge\OverrideSecurityRestrictionsOnInsecureOrigin
  - 경로 (맞춤): 해당 없음
  - 값 이름: 1, 2, 3, ...
  - 값 형식: REG_SZ 목록
  ##### 예제 값:
```
SOFTWARE\Policies\Microsoft\Edge\OverrideSecurityRestrictionsOnInsecureOrigin\0 = "http://testserver.contoso.com/"
SOFTWARE\Policies\Microsoft\Edge\OverrideSecurityRestrictionsOnInsecureOrigin\1 = "*.contoso.com"

```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: OverrideSecurityRestrictionsOnInsecureOrigin
  - 예제 값:
``` xml
<array>
  <string>http://testserver.contoso.com/</string>
  <string>*.contoso.com</string>
</array>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### ProactiveAuthEnabled
  #### 사전 인증 사용
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  사전 인증을 사용할지 여부를 구성할 수 있습니다.

이 정책을 사용하면 Microsoft Edge는 Microsoft 서비스로 로그인한 사용자를 사전에 인증하려고 시도합니다. 정기적으로 Microsoft Edge는 온라인 서비스에서 이 작업을 수행하는 방법을 제어하는 구성을 포함하는 업데이트된 매니페스트에 대해 확인합니다.

이 정책을 사용하지 않으면 Microsoft Edge는 Microsoft 서비스로 로그인한 사용자를 사전에 인증하려고 시도하지 않습니다. Microsoft Edge는 더 이상 온라인 서비스에서 이 작업을 수행하기 위한 구성을 포함하는 업데이트된 매니페스트에 대해 확인하지 않습니다.

이 정책을 구성하지 않으면 사전 인증이 켜집니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 아니요 - 브라우저 다시 시작 필요

  #### 데이터 형식:
  부울

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: ProactiveAuthEnabled
  - GP 이름: 사전 인증 사용
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: ProactiveAuthEnabled
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000001
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: ProactiveAuthEnabled
  - 예제 값:
``` xml
<true/>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### PromotionalTabsEnabled
  #### 전체 탭 프로모션 콘텐츠 사용
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  전체 탭 프로모션 또는 교육 콘텐츠의 프레젠테이션을 제어합니다. 이 설정은 사용자가 Microsoft Edge에 로그인하거나 기본 브라우저를 선택하거나 제품 기능에 대한 정보를 알아보는 데 도움이 되는 시작 페이지의 프레젠테이션을 제어합니다.

이 정책을 사용(true로 설정)하거나 구성하지 않으면 Microsoft Edge가 사용자에게 전체 탭 콘텐츠를 표시하여 제품 정보를 제공할 수 있습니다.

이 정책을 사용하지 않으면(false로 설정) Microsoft Edge가 사용자에게 전체 탭 콘텐츠를 표시할 수 없습니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  부울

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: PromotionalTabsEnabled
  - GP 이름: 전체 탭 프로모션 콘텐츠 사용
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: PromotionalTabsEnabled
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000000
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: PromotionalTabsEnabled
  - 예제 값:
``` xml
<false/>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### PromptForDownloadLocation
  #### 다운로드한 파일을 저장할 위치 묻기
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  다운로드하기 전에 파일을 저장할 위치를 묻는 메시지를 표시할지의 여부를 설정합니다.

이 정책을 사용하면 다운로드하기 전에 각 파일을 저장할 위치를 묻는 메시지가 표시됩니다. 구성하지 않은 경우 사용자에게 묻지 않고 파일이 자동으로 기본 위치에 저장됩니다.

이 정책을 구성하지 않으면 사용자가 이 설정을 변경할 수 있습니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  부울

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: PromptForDownloadLocation
  - GP 이름: 다운로드한 파일을 저장할 위치 묻기
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: PromptForDownloadLocation
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000000
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: PromptForDownloadLocation
  - 예제 값:
``` xml
<false/>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### QuicAllowed
  #### QUIC 프로토콜 허용
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  Microsoft Edge에서 QUIC 프로토콜의 사용을 허용합니다.

이 정책을 사용하거나 구성하지 않으면 QUIC 프로토콜이 허용됩니다.

이 정책을 사용하지 않으면 QUIC 프로토콜이 차단됩니다.

QUIC는 현재 TCP를 사용하는 웹 응용 프로그램의 성능을 향상시킬 수 있는 전송 계층 네트워크 프로토콜입니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 아니요 - 브라우저 다시 시작 필요

  #### 데이터 형식:
  부울

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: QuicAllowed
  - GP 이름: QUIC 프로토콜 허용
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: QuicAllowed
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000001
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: QuicAllowed
  - 예제 값:
``` xml
<true/>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### RelaunchNotification
  #### 보류 중인 업데이트에 대해 브라우저 다시 시작이 권장되거나 필요함을 사용자에게 알림
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  Notify users that they need to restart Microsoft Edge to apply a pending update.

If you don't configure this policy, Microsoft Edge adds a recycle icon at the far right of the top menu bar to prompt users to restart the browser to apply the update.

If you enable this policy and set it to 'Recommended' (1), a recurring warning prompts users that a restart is recommended. Users can dismiss this warning and defer the restart.

If you set the policy to 'Required' (2), a recurring warning prompts users that the browser will be restarted automatically as soon as a notification period passes. The default period is seven days. You can configure this period with the [RelaunchNotificationPeriod](#relaunchnotificationperiod) policy.

The user's session is restored when the browser restarts.

* Recommended (1) = Show a recurring prompt to the user indicating that a restart is recommended

* Required (2) = Show a recurring prompt to the user indicating that a restart is required

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  정수

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: RelaunchNotification
  - GP 이름: 보류 중인 업데이트에 대해 브라우저 다시 시작이 권장되거나 필요함을 사용자에게 알림
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: RelaunchNotification
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000001
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: RelaunchNotification
  - 예제 값:
``` xml
<integer>1</integer>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### RelaunchNotificationPeriod
  #### 업데이트 알림 기간 설정
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  Sets the time period, in milliseconds, over which users are notified that Microsoft Edge must be restarted to apply a pending update.

During this time period, the user is repeatedly informed that they need to restart. The app menu changes to indicate that a restart is needed when one third of the notification period passes. When two thirds of the notification period passes, the notification changes color, and again when the full notification period has passed. Additional notifications enabled by the [RelaunchNotification](#relaunchnotification) policy follow this same schedule.

If you don't configure this policy, the default period is 604800000 milliseconds (one week).

Restrictions:

* Minimum:3600000

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  정수

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: RelaunchNotificationPeriod
  - GP 이름: 업데이트 알림 기간 설정
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: RelaunchNotificationPeriod
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x240c8400
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: RelaunchNotificationPeriod
  - 예제 값:
``` xml
<integer>604800000</integer>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### RendererCodeIntegrityEnabled
  #### 렌더러 코드 무결성 사용
  >지원되는 버전: Windows의 Microsoft Edge, 버전 78 이상부터

  #### 설명
  이 정책을 사용하거나 설정하지 않으면 렌더러 코드 무결성이 사용됩니다. 이 정책은 Microsoft Edge내에서 실행해야 하는 타사 소프트웨어에서 호환성 문제가 발생한 경우에만 사용하지 않도록 설정해야 합니다.

이 정책을 사용하지 않도록 설정하면 Microsoft Edge내에서 알 수 없는 잠재적으로 악의적인 코드가 로드될 수 있기 때문에 Microsoft Edge의 보안 및 안정성에 해로운 영향을 미칩니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 아니요 - 브라우저 다시 시작 필요

  #### 데이터 형식:
  부울

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: RendererCodeIntegrityEnabled
  - GP 이름: 렌더러 코드 무결성 사용
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: RendererCodeIntegrityEnabled
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000000
```


  

  [맨 위로 이동](#microsoft-edge---정책)

  ### RequireOnlineRevocationChecksForLocalAnchors
  #### 온라인 OCSP/CRL 검사가 로컬 트러스트 앵커에 필요한지 여부를 지정합니다.
  >지원되는 버전: Windows의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  온라인 해지 확인(OCSP/CRL 확인)이 필요한지 여부를 제어합니다. Microsoft Edge에서 해지 상태 정보를 가져올 수 없는 경우 이러한 인증서는 해지된 것으로 처리됩니다("하드 오류").

이 정책을 사용하면 Microsoft Edge는 성공적으로 유효성을 검사하고 로컬로 설치된 CA 인증서에 의해 서명된 서버 인증서에 대한 해지 확인을 항상 수행합니다.

이 정책을 구성하거나 사용하지 않으면 Microsoft Edge는 기존 온라인 해지 확인 설정을 사용합니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  부울

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: RequireOnlineRevocationChecksForLocalAnchors
  - GP 이름: 온라인 OCSP/CRL 검사가 로컬 트러스트 앵커에 필요한지 여부를 지정합니다.
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: RequireOnlineRevocationChecksForLocalAnchors
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000000
```


  

  [맨 위로 이동](#microsoft-edge---정책)

  ### ResolveNavigationErrorsUseWebService
  #### 웹 서비스를 사용하여 탐색 오류 해결 사용
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  Allow Microsoft Edge to issue a dataless connection to a web service to probe networks for connectivity in cases like hotel and airport Wi-Fi.

If you enable this policy, a web service is used for network connectivity tests.

If you disable this policy, Microsoft Edge uses native APIs to try to resolve network connectivity and navigation issues.

**Note**: Except on Windows 8 and later versions of Windows, Microsoft Edge *always* uses native APIs to resolve connectivity issues.

If you don't configure this policy, Microsoft Edge respects the user preference that's set under Services at edge://settings/privacy.
Specifically, there's a **Use a web service to help resolve navigation errors** toggle, which the user can switch on or off. Be aware that if you have enabled this policy (ResolveNavigationErrorsUseWebService), the **Use a web service to help resolve navigation errors** setting is turned on, but the user can't change the setting by using the toggle. If you have disabled this policy, the **Use a web service to help resolve navigation errors** setting is turned off, and the user can't change the setting by using the toggle.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 예
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  부울

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: ResolveNavigationErrorsUseWebService
  - GP 이름: 웹 서비스를 사용하여 탐색 오류 해결 사용
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 관리 템플릿/Microsoft Edge - 기본 설정(사용자가 재정의할 수 없음)/
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): SOFTWARE\Policies\Microsoft\Edge\맞춤
  - 값 이름: ResolveNavigationErrorsUseWebService
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000001
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: ResolveNavigationErrorsUseWebService
  - 예제 값:
``` xml
<true/>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### RestrictSigninToPattern
  #### Microsoft Edge 기본 계정으로 사용할 수 있는 계정 제한
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  브라우저에서 기본 계정으로 설정할 수 있는 계정을 결정 합니다. Microsoft Edge에서 브라우저 기본 계정으로 설정할 수 있는 계정(옵트인 흐름을 동기화하는 동안 선택된 계정)결정합니다.

사용자가 이 패턴과 일치하지 않는 사용자 이름으로 브라우저 기본 계정을 설정하려고 하면 차단되며 적절한 오류 메시지가 표시됩니다.

이 정책을 구성하지 않거나 비워 두면 사용자가 Microsoft Edge에서 브라우저 기본 계정으로 모든 계정을 설정할 수 있습니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  문자열

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: RestrictSigninToPattern
  - GP 이름: Microsoft Edge 기본 계정으로 사용할 수 있는 계정 제한
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: RestrictSigninToPattern
  - 값 형식: REG_SZ
  ##### 예제 값:
```
".*@contoso.com"
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: RestrictSigninToPattern
  - 예제 값:
``` xml
<string>.*@contoso.com</string>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### RunAllFlashInAllowMode
  #### Adobe Flash 콘텐츠 설정을 모든 콘텐츠로 확장
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  If you enable this policy, all Adobe Flash content embedded in websites that are set to allow Adobe Flash in the content settings -- either by the user or by enterprise policy -- will run. This includes content from other origins and/or small content.

To control which websites are allowed to run Adobe Flash, see the specifications in the [DefaultPluginsSetting](#defaultpluginssetting), [PluginsAllowedForUrls](#pluginsallowedforurls), and [PluginsBlockedForUrls](#pluginsblockedforurls) policies.

If you disable this policy or don't configure it, Adobe Flash content from other origins (from sites that aren't specified in the three policies mentioned immediately above) or small content might be blocked.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  부울

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: RunAllFlashInAllowMode
  - GP 이름: Adobe Flash 콘텐츠 설정을 모든 콘텐츠로 확장
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: RunAllFlashInAllowMode
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000001
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: RunAllFlashInAllowMode
  - 예제 값:
``` xml
<true/>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### SSLErrorOverrideAllowed
  #### HTTPS 경고 페이지에서 사용자가 작업을 계속할 수 있도록 허용
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  Microsoft Edge는 사용자가 SSL 오류가 있는 사이트를 방문할 때 경고 페이지를 표시합니다.

이 정책을 사용하거나 구성하지 않으면(기본값) 사용자가 이 경고 페이지에서 클릭하여 앞으로 나아갈 수 있습니다.

이 정책을 사용하지 않으면 사용자가 클릭하여 앞으로 나아가는 것이 모든 경고 페이지에서 차단됩니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  부울

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: SSLErrorOverrideAllowed
  - GP 이름: HTTPS 경고 페이지에서 사용자가 작업을 계속할 수 있도록 허용
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: SSLErrorOverrideAllowed
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000001
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: SSLErrorOverrideAllowed
  - 예제 값:
``` xml
<true/>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### SSLVersionMin
  #### 최소 TLS 버전 사용
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  지원되는 최소 SSL 버전을 설정합니다. 이 정책을 구성하지 않으면 Microsoft Edge가 기본 최소 버전인 TLS 1.0을 사용합니다.

이 정책을 사용하면 최소 버전을 "tls1", "tls1.1"또는 "tls1.2"값 중 하나로 설정할 수 있습니다. 설정 시 Microsoft Edge는 지정된 버전보다 낮은 SSL/TLS 버전을 사용하지 않습니다. 인식할 수 없는 값은 무시됩니다.

* "tls1" = TLS 1.0

* "tls1.1" = TLS 1.1

* "tls1.2" = TLS 1.2

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  문자열

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: SSLVersionMin
  - GP 이름: 최소 TLS 버전 사용
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: SSLVersionMin
  - 값 형식: REG_SZ
  ##### 예제 값:
```
"tls1"
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: SSLVersionMin
  - 예제 값:
``` xml
<string>tls1</string>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### SavingBrowserHistoryDisabled
  #### 브라우저 기록 저장 사용 안 함
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  브라우저 기록 저장을 사용하지 않도록 설정하고 사용자가 이 설정을 변경할 수 없게 합니다.

이 정책을 사용하면 검색 기록 저장되지 않습니다. 이렇게 하면 탭 동기화도 사용하지 않도록 설정됩니다.

이 정책을 사용하지 않거나 구성하지 않으면, 검색 기록이 저장됩니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  부울

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: SavingBrowserHistoryDisabled
  - GP 이름: 브라우저 기록 저장 사용 안 함
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: SavingBrowserHistoryDisabled
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000001
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: SavingBrowserHistoryDisabled
  - 예제 값:
``` xml
<true/>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### SearchSuggestEnabled
  #### 검색 제안 사용
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  Microsoft Edge의 주소 표시줄 및 자동 제안 목록에서 웹 검색 제안을 사용하도록 설정하고 사용자가 이 정책을 변경할 수 없도록 합니다.

이 정책을 사용하면 웹 검색 제안이 사용됩니다.

이 정책을 사용하지 않으면 웹 검색 제안은 절대 사용되지 않지만 로컬 검색 기록 및 로컬 즐겨찾기 제안은 계속 표시됩니다. 이 정책을 사용하지 않으면 입력한 문자나 방문한 URL이 모두 원격 분석에 포함되지 않습니다.

이 정책을 설정하지 않으면 검색 제안이 사용되지만 사용자가 변경할 수 있습니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 예
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  부울

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: SearchSuggestEnabled
  - GP 이름: 검색 제안 사용
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 관리 템플릿/Microsoft Edge - 기본 설정(사용자가 재정의할 수 없음)/
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): SOFTWARE\Policies\Microsoft\Edge\맞춤
  - 값 이름: SearchSuggestEnabled
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000001
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: SearchSuggestEnabled
  - 예제 값:
``` xml
<true/>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### SecurityKeyPermitAttestation
  #### 직접 보안 키 증명 사용 권한이 필요하지 않은 웹 사이트 또는 도메인
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  보안 키의 증명 인증서를 요청할 때 명시 적 사용자의 사용 권한이 필요하지 않은 웹 사이트 및 도메인을 지정합니다. 또한 개별 증명을 사용할 수 있음을 나타내는 신호가 보안 키로 전송됩니다. 이 옵션이 없으면 사이트에서 보안 키의 인증을 요청할 때마다 사용자에게 메시지가 표시됩니다.

사이트 (예: https://contoso.com/some/path)은(는) U2F appID로만 일치합니다. 도메인(예: contoso.com)은(는) webauthn RP ID로만 일치합니다. 특정 사이트에 대한 U2F 및 webauthn API를 모두 포괄하려면 appID URL과 도메인을 모두 나열해야 합니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  문자열 목록

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: SecurityKeyPermitAttestation
  - GP 이름: 직접 보안 키 증명 사용 권한이 필요하지 않은 웹 사이트 또는 도메인
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge\SecurityKeyPermitAttestation
  - 경로 (맞춤): 해당 없음
  - 값 이름: 1, 2, 3, ...
  - 값 형식: REG_SZ 목록
  ##### 예제 값:
```
SOFTWARE\Policies\Microsoft\Edge\SecurityKeyPermitAttestation\0 = "https://contoso.com"

```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: SecurityKeyPermitAttestation
  - 예제 값:
``` xml
<array>
  <string>https://contoso.com</string>
</array>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### SendIntranetToInternetExplorer
  #### 모든 인트라넷 사이트를 Internet Explorer로 보내기
  >지원되는 버전: Windows의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  Internet Explorer 모드를 위한 최적의 환경을 구성하는 방법에 대한 지침은 [https://go.microsoft.com/fwlink/?linkid=2094210](https://go.microsoft.com/fwlink/?linkid=2094210)를 참조하세요.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 아니요 - 브라우저 다시 시작 필요

  #### 데이터 형식:
  부울

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: SendIntranetToInternetExplorer
  - GP 이름: 모든 인트라넷 사이트를 Internet Explorer로 보내기
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: SendIntranetToInternetExplorer
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000001
```


  

  [맨 위로 이동](#microsoft-edge---정책)

  ### SendSiteInfoToImproveServices
  #### Microsoft 서비스 개선을 위해 사이트 정보 보내기
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  Microsoft Edge의 Windows 10 Beta 및 Stable 채널의 경우 이 정책을 구성하면 컬렉션 또는 컬렉션이 아닌 Microsoft Edge 웹 사이트 검색 정보에 대한 Windows 진단 데이터 설정을 재정의합니다([https://go.microsoft.com/fwlink/?linkid=2099569](https://go.microsoft.com/fwlink/?linkid=2099569)).

이 정책 설정을 통해 사용자가 Microsoft로 보내 검색과 같은 서비스를 개선하기 위해 Microsoft Edge에서 방문하는 웹 사이트에 대한 정보를 Microsoft에 보낼 수 있는지 여부를 결정할 수 있습니다.

이 정책을 사용하면 Microsoft Edge에서 방문하는 웹 사이트에 대한 정보가 Microsoft에 전송됩니다.

이 정책을 사용하지 않으면 Microsoft Edge에서 방문하는 웹 사이트에 대한 정보가 Microsoft에 전송되지 않습니다.

Windows 10, Beta 및 Stable 채널에서 이 정책은 사용자가 방문하는 웹 사이트에 대한 정보 전송을 제어합니다. 이 정책을 구성하지 않으면 Microsoft Edge에서 Windows 진단 데이터 설정을 기본값으로 합니다.

Windows 10, Canary 및 Dev 채널에서 이 정책은 사용자가 방문하는 웹 사이트에 대한 정보 전송을 제어합니다. 이 정책을 구성하지 않으면 Microsoft Edge에서 사용자의 기본 설정을 기본값으로 합니다.

Windows 7, 8 및 Mac에서는 이 정책이 사용자가 방문하는 웹 사이트에 대한 정보 전송을 제어합니다. 이 정책을 구성하지 않으면 Microsoft Edge에서 사용자의 기본 설정을 기본값으로 합니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 아니요 - 브라우저 다시 시작 필요

  #### 데이터 형식:
  부울

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: SendSiteInfoToImproveServices
  - GP 이름: Microsoft 서비스 개선을 위해 사이트 정보 보내기
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: SendSiteInfoToImproveServices
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000000
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: SendSiteInfoToImproveServices
  - 예제 값:
``` xml
<false/>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### ShowOfficeShortcutInFavoritesBar
  #### 즐겨 찾기 모음에 Microsoft Office 바로 가기 표시
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  즐겨 찾기 모음에 Office.com에 대한 바로 가기를 포함할지 여부를 지정합니다. Microsoft Edge에 로그인한 사용자는 바로 가기를 통해 Microsoft Office 앱 및 문서로 이동합니다.

이 정책을 사용하거나 설정하지 않은 경우 즐겨 찾기 모음 상황에 맞는 메뉴에서 토글을 변경하여 바로 가기를 표시할지 여부를 선택할 수 있습니다.

정책을 사용하지 않으면 바로 가기가 표시되지 않습니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  부울

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: ShowOfficeShortcutInFavoritesBar
  - GP 이름: 즐겨 찾기 모음에 Microsoft Office 바로 가기 표시
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: ShowOfficeShortcutInFavoritesBar
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000000
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: ShowOfficeShortcutInFavoritesBar
  - 예제 값:
``` xml
<false/>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### SignedHTTPExchangeEnabled
  #### 서명된 HTTP 교환(SXG) 지원 사용
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 78 이상부터

  #### 설명
  서명된 HTTP Exchange(SXG) 지원을 사용하도록 설정합니다.

이 정책을 설정하거나 사용하지 않으면 Microsoft Edge가 서명된 HTTP Exchange로 제공되는 웹 콘텐츠를 수락합니다.

이 정책을 사용하지 않도록 설정하면 서명된 HTTP Exchange를 로드할 수 없습니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  부울

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: SignedHTTPExchangeEnabled
  - GP 이름: 서명된 HTTP 교환(SXG) 지원 사용
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: SignedHTTPExchangeEnabled
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000001
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: SignedHTTPExchangeEnabled
  - 예제 값:
``` xml
<true/>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### SitePerProcess
  #### 모든 사이트에 대해 사이트 격리 사용
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  
The 'SitePerProcess' policy can be used to prevent users from opting out of the default behavior of isolating all sites. Note that you can also use the [IsolateOrigins](#isolateorigins) policy to isolate additional, finer-grained origins.
If you enable this policy, users can't opt out of the default behavior where each site runs in its own process.
If you disable or don’t configure this policy, a user can opt out of site isolation.  (For example, by using "Disable site isolation" entry in edge://flags.)  Disabling the policy or not configuring the policy doesn't turn off Site Isolation.


  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 아니요 - 브라우저 다시 시작 필요

  #### 데이터 형식:
  부울

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: SitePerProcess
  - GP 이름: 모든 사이트에 대해 사이트 격리 사용
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: SitePerProcess
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000001
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: SitePerProcess
  - 예제 값:
``` xml
<true/>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### SpellcheckEnabled
  #### 맞춤법 검사 사용
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  If you enable or don't configure this policy, the user can use spellcheck.

If you disable this policy, the user can't use spellcheck and the [SpellcheckLanguage](#spellchecklanguage) and [SpellcheckLanguageBlocklist](#spellchecklanguageblocklist) policies are also disabled.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  부울

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: SpellcheckEnabled
  - GP 이름: 맞춤법 검사 사용
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: SpellcheckEnabled
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000000
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: SpellcheckEnabled
  - 예제 값:
``` xml
<false/>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### SpellcheckLanguage
  #### 특정 맞춤법 검사 언어 사용
  >지원되는 버전: Windows의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  Enables different languages for spellcheck. Any language that you specify that isn't recognized is ignored.

If you enable this policy, spellcheck is enabled for the languages specified, as well as any languages the user has enabled.

If you don't configure or disable this policy, there's no change to the user's spellcheck preferences.

If the [SpellcheckEnabled](#spellcheckenabled) policy is disabled, this policy will have no effect.

If a language is included in both the 'SpellcheckLanguage' and the [SpellcheckLanguageBlocklist](#spellchecklanguageblocklist) policy, the spellcheck language is enabled.

The supported languages are: af, bg, ca, cs, cy, da, de, el, en-AU, en-CA, en-GB, en-US, es, es-419, es-AR, es-ES, es-MX, es-US, et, fa, fo, fr, he, hi, hr, hu, id, it, ko, lt, lv, nb, nl, pl, pt-BR, pt-PT, ro, ru, sh, sk, sl, sq, sr, sv, ta, tg, tr, uk, vi.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  문자열 목록

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: SpellcheckLanguage
  - GP 이름: 특정 맞춤법 검사 언어 사용
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge\SpellcheckLanguage
  - 경로 (맞춤): 해당 없음
  - 값 이름: 1, 2, 3, ...
  - 값 형식: REG_SZ 목록
  ##### 예제 값:
```
SOFTWARE\Policies\Microsoft\Edge\SpellcheckLanguage\0 = "fr"
SOFTWARE\Policies\Microsoft\Edge\SpellcheckLanguage\1 = "es"

```


  

  [맨 위로 이동](#microsoft-edge---정책)

  ### SpellcheckLanguageBlocklist
  #### 맞춤법 검사 언어 강제 사용 안 함
  >지원되는 버전: Windows의 Microsoft Edge, 버전 78 이상부터

  #### 설명
  Force-disables spellcheck languages. Unrecognized languages in that list will be ignored.

If you enable this policy, spellcheck will be disabled for the languages specified. The user can still enable or disable spellcheck for languages not in the list.

If you do not set this policy, or disable it, there will be no change to the user's spellcheck preferences.

If the [SpellcheckEnabled](#spellcheckenabled) policy is set to disabled, this policy will have no effect.

If a language is included in both the [SpellcheckLanguage](#spellchecklanguage) and the 'SpellcheckLanguageBlocklist' policy, the spellcheck language is enabled.

The currently supported languages are: af, bg, ca, cs, da, de, el, en-AU, en-CA, en-GB, en-US, es, es-419, es-AR, es-ES, es-MX, es-US, et, fa, fo, fr, he, hi, hr, hu, id, it, ko, lt, lv, nb, nl, pl, pt-BR, pt-PT, ro, ru, sh, sk, sl, sq, sr, sv, ta, tg, tr, uk, vi.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  문자열 목록

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: SpellcheckLanguageBlocklist
  - GP 이름: 맞춤법 검사 언어 강제 사용 안 함
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge\SpellcheckLanguageBlocklist
  - 경로 (맞춤): 해당 없음
  - 값 이름: 1, 2, 3, ...
  - 값 형식: REG_SZ 목록
  ##### 예제 값:
```
SOFTWARE\Policies\Microsoft\Edge\SpellcheckLanguageBlocklist\0 = "fr"
SOFTWARE\Policies\Microsoft\Edge\SpellcheckLanguageBlocklist\1 = "es"

```


  

  [맨 위로 이동](#microsoft-edge---정책)

  ### SuppressUnsupportedOSWarning
  #### 지원 되지 않는 OS 경고 표시 안 함
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  더 이상 지원되지 않는 컴퓨터 또는 운영 체제에서 Microsoft Edge가 실행될 때 나타나는 경고를 표시하지 않습니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 아니요 - 브라우저 다시 시작 필요

  #### 데이터 형식:
  부울

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: SuppressUnsupportedOSWarning
  - GP 이름: 지원 되지 않는 OS 경고 표시 안 함
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: SuppressUnsupportedOSWarning
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000001
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: SuppressUnsupportedOSWarning
  - 예제 값:
``` xml
<true/>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### SyncDisabled
  #### Microsoft 동기화 서비스를 사용한 데이터의 동기화 사용 안 함
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  Disables data synchronization in Microsoft Edge and prevents users from modifying this setting.

If this policy is not set, users will be able to either turn on or turn off sync.

Do not enable this policy when the policy 'RoamingProfileSupportEnabled' is enabled, as 'RoamingProfileSupportEnabled' duplicates the sync functionality.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 예
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  부울

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: SyncDisabled
  - GP 이름: Microsoft 동기화 서비스를 사용한 데이터의 동기화 사용 안 함
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 관리 템플릿/Microsoft Edge - 기본 설정(사용자가 재정의할 수 없음)/
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): SOFTWARE\Policies\Microsoft\Edge\맞춤
  - 값 이름: SyncDisabled
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000001
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: SyncDisabled
  - 예제 값:
``` xml
<true/>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### TabFreezingEnabled
  #### Allow freezing of background tabs
  >지원되는 버전: Windows의 Microsoft Edge, 버전 79 이상부터

  #### 설명
  Controls whether Microsoft Edge can freeze tabs that are in the background for at least 5 minutes.

Tab freezing reduces CPU, battery, and memory usage. Microsoft Edge uses heuristics to avoid freezing tabs that do useful work in the background, such as display notifications, play sound, and stream video.

If you enable or don't configure this policy, tabs that have been in the background for at least 5 minutes might be frozen.

If you disable this policy, no tabs will be frozen.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 아니요 - 브라우저 다시 시작 필요

  #### 데이터 형식:
  부울

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: TabFreezingEnabled
  - GP 이름: Allow freezing of background tabs
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: TabFreezingEnabled
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000000
```


  

  [맨 위로 이동](#microsoft-edge---정책)

  ### TaskManagerEndProcessEnabled
  #### 브라우저 작업 관리자에서 종료 프로세스 사용
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  이 정책을 사용하거나 사용하지 않도록 설정하면 사용자가 브라우저 작업 관리자에서 프로세스를 종료할 수 있습니다. 이 기능을 사용하지 않으면 사용자가 프로세스를 종료할 수 없으며 브라우저 작업 관리자에서 [프로세스 끝내기] 단추가 비활성화됩니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  부울

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: TaskManagerEndProcessEnabled
  - GP 이름: 브라우저 작업 관리자에서 종료 프로세스 사용
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: TaskManagerEndProcessEnabled
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000001
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: TaskManagerEndProcessEnabled
  - 예제 값:
``` xml
<true/>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### TrackingPrevention
  #### 사용자의 웹 검색 활동 추적 차단
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 78 이상부터

  #### 설명
  사용자의 웹 검색 활동을 추적하지 못하도록 웹 사이트를 차단할지 여부를 결정할 수 있습니다.

이 정책을 사용하면 다음과 같은 옵션을 통해 추적 방지 수준을 설정할 수 있습니다.

0 = 꺼짐(추적 방지 안 함)
1 = 기본(유해한 추적기 차단, 콘텐츠 및 광고가 개인 설정됨)
2 = 균형 조정(유해한 추적기 및 사용자가 방문하지 않은 사이트의 추적기 차단, 콘텐츠 및 광고의 개인 설정 수준이 낮아짐)
3 = 엄격(모든 사이트에서 유해한 추적기 및 대부분의 추적기 차단, 콘텐츠 및 광고의 개인 설정이 최소화됨, 사이트의 일부 부분이 작동하지 않을 수 있음)

이 정책을 사용하지 않거나 구성하지 않으면 사용자가 추적 방지 수준을 직접 설정할 수 있습니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  정수

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: TrackingPrevention
  - GP 이름: 사용자의 웹 검색 활동 추적 차단
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: TrackingPrevention
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000002
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: TrackingPrevention
  - 예제 값:
``` xml
<integer>2</integer>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### TranslateEnabled
  #### 번역 사용
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  Microsoft Edge에서 통합된 Microsoft 번역 서비스를 사용하도록 설정합니다.

이 정책을 사용하면 Microsoft Edge는 오른쪽 클릭 상황에 맞는 메뉴에서 통합된 번역 플라이아웃(해당되는 경우) 및 번역 옵션을 표시하여 사용자에게 번역 기능을 제공합니다.

이 정책을 사용하지 않으면 기본 제공 번역 기능이 모두 사용하지 않도록 설정됩니다.

정책을 구성하지 않으면 사용자가 변역 기능을 사용할지 여부를 선택할 수 있습니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 예
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  부울

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: TranslateEnabled
  - GP 이름: 번역 사용
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 관리 템플릿/Microsoft Edge - 기본 설정(사용자가 재정의할 수 없음)/
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): SOFTWARE\Policies\Microsoft\Edge\맞춤
  - 값 이름: TranslateEnabled
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000001
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: TranslateEnabled
  - 예제 값:
``` xml
<true/>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### URLAllowlist
  #### 허용된 URL 목록을 정의
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  Allow access to the listed URLs, as exceptions to the URL block list.

Format the URL pattern according to [https://go.microsoft.com/fwlink/?linkid=2095322](https://go.microsoft.com/fwlink/?linkid=2095322).

You can use this policy to open exceptions to restrictive block lists. For example, you can include '*' in the block list to block all requests, and then use this policy to allow access to a limited list of URLs. You can use this policy to open exceptions to certain schemes, subdomains of other domains, ports, or specific paths.

The most specific filter determines if a URL is blocked or allowed. The allowed list takes precedence over the block list.

This policy is limited to 1000 entries; subsequent entries are ignored.

If you don't configure this policy, there are no exceptions to the block list in the [URLBlocklist](#urlblocklist) policy.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  문자열 목록

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: URLAllowlist
  - GP 이름: 허용된 URL 목록을 정의
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge\URLAllowlist
  - 경로 (맞춤): 해당 없음
  - 값 이름: 1, 2, 3, ...
  - 값 형식: REG_SZ 목록
  ##### 예제 값:
```
SOFTWARE\Policies\Microsoft\Edge\URLAllowlist\0 = "contoso.com"
SOFTWARE\Policies\Microsoft\Edge\URLAllowlist\1 = "https://ssl.server.com"
SOFTWARE\Policies\Microsoft\Edge\URLAllowlist\2 = "hosting.com/good_path"
SOFTWARE\Policies\Microsoft\Edge\URLAllowlist\3 = "https://server:8080/path"
SOFTWARE\Policies\Microsoft\Edge\URLAllowlist\4 = ".exact.hostname.com"

```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: URLAllowlist
  - 예제 값:
``` xml
<array>
  <string>contoso.com</string>
  <string>https://ssl.server.com</string>
  <string>hosting.com/good_path</string>
  <string>https://server:8080/path</string>
  <string>.exact.hostname.com</string>
</array>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### URLBlocklist
  #### URL 목록에 대한 액세스 차단
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  Define a list of sites, based on URL patterns, that are blocked (your users can't load them).

Format the URL pattern according to [https://go.microsoft.com/fwlink/?linkid=2095322](https://go.microsoft.com/fwlink/?linkid=2095322).

You can define exceptions in the [URLAllowlist](#urlallowlist) policy. These policies are limited to 1000 entries; subsequent entries are ignored.

Note that blocking internal 'edge://*' URLs isn't recommended - this may lead to unexpected errors.

This policy doesn't prevent the page from updating dynamically through JavaScript. For example, if you block 'contoso.com/abc', users might still be able to visit 'contoso.com' and click on a link to visit 'contoso.com/abc', as long as the page doesn't refresh.

If you don't configure this policy, no URLs are blocked.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  문자열 목록

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: URLBlocklist
  - GP 이름: URL 목록에 대한 액세스 차단
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge\URLBlocklist
  - 경로 (맞춤): 해당 없음
  - 값 이름: 1, 2, 3, ...
  - 값 형식: REG_SZ 목록
  ##### 예제 값:
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


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: URLBlocklist
  - 예제 값:
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
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### UserDataDir
  #### 사용자 데이터 디렉터리 설정
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  사용자 데이터를 저장하는 데 사용할 디렉터리를 설정합니다.

이 정책을 사용하면 Microsoft Edge는 사용자가 '--user-data-dir' 명령줄 플래그를 설정했는지 여부에 관계 없이 지정된 디렉터리를 사용합니다.

이 정책을 사용하지 않으면 기본 프로필 경로가 사용되지만 사용자가 '--user-data-dir' 플래그를 사용하여 이 경로를 재정의할 수 있습니다. 사용자는 프로필 경로에 있는 edge://version/에서 프로필 디렉터리를 찾을 수 있습니다.

데이터 손실이나 기타 오류가 발생하지 않도록 하려면 Microsoft Edge에서 콘텐츠를 관리하므로 볼륨의 루트 디렉터리 또는 다른 용도로 사용되는 디렉터리에 이 정책을 구성하지 마세요.

사용할 수 있는 변수 목록은 [https://go.microsoft.com/fwlink/?linkid=2095041](https://go.microsoft.com/fwlink/?linkid=2095041)을 참조하세요.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 아니요 - 브라우저 다시 시작 필요

  #### 데이터 형식:
  문자열

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: UserDataDir
  - GP 이름: 사용자 데이터 디렉터리 설정
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: UserDataDir
  - 값 형식: REG_SZ
  ##### 예제 값:
```
"${users}/${user_name}/Edge"
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: UserDataDir
  - 예제 값:
``` xml
<string>${users}/${user_name}/Edge</string>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### UserFeedbackAllowed
  #### 사용자 피드백 허용
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  Microsoft Edge는 사용자가 피드백, 제안 또는 고객 설문 조사를 보내고 브라우저 관련 문제를 보고할 수 있도록 Microsoft Edge 피드백 기능(기본적으로 사용하도록 설정됨)을 사용합니다.

이 정책을 사용하거나 구성하지 않으면 사용자가 피드백 가장자리를 호출할 수 있습니다.

이 정책을 사용하지 않으면 사용자가 Microsoft Edge 피드백을 호출할 수 없습니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 아니요 - 브라우저 다시 시작 필요

  #### 데이터 형식:
  부울

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: UserFeedbackAllowed
  - GP 이름: 사용자 피드백 허용
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: UserFeedbackAllowed
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000001
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: UserFeedbackAllowed
  - 예제 값:
``` xml
<true/>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### VideoCaptureAllowed
  #### 비디오 캡처 허용 또는 차단
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  Control whether sites can capture video.

If enabled or not configured (default), the user will be asked about video capture access for all sites except those with URLs configured in the [VideoCaptureAllowedUrls](#videocaptureallowedurls) policy list, which will be granted access without prompting.

If you disable this policy, the user isn't prompted, and video capture is only available to URLs configured in [VideoCaptureAllowedUrls](#videocaptureallowedurls) policy.

This policy affects all types of video inputs, not only the built-in camera.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  부울

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: VideoCaptureAllowed
  - GP 이름: 비디오 캡처 허용 또는 차단
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: VideoCaptureAllowed
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000000
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: VideoCaptureAllowed
  - 예제 값:
``` xml
<false/>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### VideoCaptureAllowedUrls
  #### 권한을 요청하지 않고 비디오 캡처 장치에 액세스할 수 있는 사이트
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  URL 패턴을 기반으로 사용자의 사용 권한없이 비디오 캡처 장치를 사용할 수 있는 웹 사이트를 지정합니다. 목록의 패턴은 요청 URL의 보안 원점과 비교됩니다. 일치할 경우 사이트에 자동으로 비디오 캡처 장치에 대한 액세스 권한이 부여됩니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 예

  #### 데이터 형식:
  문자열 목록

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: VideoCaptureAllowedUrls
  - GP 이름: 권한을 요청하지 않고 비디오 캡처 장치에 액세스할 수 있는 사이트
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge\VideoCaptureAllowedUrls
  - 경로 (맞춤): 해당 없음
  - 값 이름: 1, 2, 3, ...
  - 값 형식: REG_SZ 목록
  ##### 예제 값:
```
SOFTWARE\Policies\Microsoft\Edge\VideoCaptureAllowedUrls\0 = "https://www.contoso.com/"
SOFTWARE\Policies\Microsoft\Edge\VideoCaptureAllowedUrls\1 = "https://[*.]contoso.edu/"

```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: VideoCaptureAllowedUrls
  - 예제 값:
``` xml
<array>
  <string>https://www.contoso.com/</string>
  <string>https://[*.]contoso.edu/</string>
</array>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### WPADQuickCheckEnabled
  #### WPAD 최적화 설정
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  Microsoft Edge에서 WPAD(웹 프록시 자동 검색) 최적화를 끌 수 있도록 허용합니다.

이 정책을 사용하지 않으면 WPAD 최적화가 사용하지 않도록 설정되므로 브라우저가 DNS 기반 WPAD 서버를 더 오래 기다립니다.

이 정책을 사용하거나 구성하지 않으면 WPAD 최적화가 사용하도록 설정됩니다.

이 정책의 사용 여부 또는 방법에 관계 없이 WPAD 최적화 설정은 사용자가 변경할 수 없습니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 아니요 - 브라우저 다시 시작 필요

  #### 데이터 형식:
  부울

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: WPADQuickCheckEnabled
  - GP 이름: WPAD 최적화 설정
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: WPADQuickCheckEnabled
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000001
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: WPADQuickCheckEnabled
  - 예제 값:
``` xml
<true/>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### WebDriverOverridesIncompatiblePolicies
  #### WebDriver가 호환되지 않는 정책을 재정의하도록 허용
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  
This policy was removed in M80, because it is not necessary anymore as
WebDriver is now compatible with all existing policies.

This policy allows users of the WebDriver feature to override
policies which can interfere with its operation.

Currently this policy disables [SitePerProcess](#siteperprocess) and [IsolateOrigins](#isolateorigins) policies.

If the policy is enabled, WebDriver will be able to override incomaptible
policies.
If the policy is disabled or not configured, WebDriver will not be allowed
to override incompatible policies.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 아니요 - 브라우저 다시 시작 필요

  #### 데이터 형식:
  부울

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: WebDriverOverridesIncompatiblePolicies
  - GP 이름: WebDriver가 호환되지 않는 정책을 재정의하도록 허용
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: WebDriverOverridesIncompatiblePolicies
  - 값 형식: REG_DWORD
  ##### 예제 값:
```
0x00000001
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: WebDriverOverridesIncompatiblePolicies
  - 예제 값:
``` xml
<true/>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### WebRtcLocalhostIpHandling
  #### WebRTC에 의한 로컬호스트 IP 주소 노출 제한
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  WebRTC가 사용자의 localhost IP 주소를 노출하는지 여부를 설정할 수 있습니다.

이 정책을 "AllowAllInterfaces"('기본값') 또는 "AllowPublicAndPrivateInterfaces"('default_public_and_private_interfaces')로 설정하면 WebRTC가 로컬 호스트 IP 주소를 노출합니다.

이 정책을 "AllowPublicInterfaceOnly"('default_public_interface_only') 또는 "DisableNonProxiedUdp"('disable_non_proxied_udp')로 설정하면 WebRTC는 localhost IP 주소를 노출하지 않습니다.

이 정책을 설정하지 않거나 정책을 사용하지 않으면 WebRTC가 localhost IP 주소를 노출합니다.

  * '기본값' = 모든 인터페이스를 허용합니다. localhost IP 주소를 노출합니다.
  * default_public_and_private_interfaces' = http 기본 경로를 통한 공개 및 비공개 인터페이스를 허용합니다. localhost IP 주소를 노출합니다.
  * 'default_public_interface_only' = http 기본 경로를 통한 공개 인터페이스를 허용합니다. localhost IP 주소를 노출하지 않습니다.
  * 'disable_non_proxied_udp' = 프록시 서버에서 UDP를 지원하지 않으면 TCP를 사용합니다. localhost IP 주소를 노출하지 않습니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 아니요 - 브라우저 다시 시작 필요

  #### 데이터 형식:
  문자열

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: WebRtcLocalhostIpHandling
  - GP 이름: WebRTC에 의한 로컬호스트 IP 주소 노출 제한
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: WebRtcLocalhostIpHandling
  - 값 형식: REG_SZ
  ##### 예제 값:
```
"default"
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: WebRtcLocalhostIpHandling
  - 예제 값:
``` xml
<string>default</string>
```
  

  [맨 위로 이동](#microsoft-edge---정책)

  ### WebRtcUdpPortRange
  #### WebRTC에서 사용하는 로컬 UDP 포트 범위 제한
  >지원되는 버전: Windows 및 Mac의 Microsoft Edge, 버전 77 이상부터

  #### 설명
  WebRTC에서 사용하는 UDP 포트 범위를 지정된 포트 간격(끝점 포함)으로 제한합니다.

이 정책을 구성하면 WebRTC에서 사용할 수 있는 로컬 UDP 포트의 범위를 지정할 수 있습니다.

이 정책을 구성하지 않거나 빈 문자열 또는 잘못된 포트 범위로 설정하면 WebRTC는 사용 가능한 모든 로컬 UDP 포트를 사용할 수 있습니다.

  #### 지원되는 기능:
  - 필수일 수 있음: 예
  - 권장될 수 있음: 아니요
  - 동적 정책 새로 고침: 아니요 - 브라우저 다시 시작 필요

  #### 데이터 형식:
  문자열

  #### Windows 정보 및 설정
  ##### 그룹 정책(ADMX) 정보
  - GP 고유 이름: WebRtcUdpPortRange
  - GP 이름: WebRTC에서 사용하는 로컬 UDP 포트 범위 제한
  - GP 경로 (필수): 관리 템플릿/Microsoft Edge/
  - GP 경로 (맞춤): 해당 없음
  - GP ADMX 파일 이름: MSEdge.admx
  ##### Windows 레지스트리 설정
  - 경로 (필수): SOFTWARE\Policies\Microsoft\Edge
  - 경로 (맞춤): 해당 없음
  - 값 이름: WebRtcUdpPortRange
  - 값 형식: REG_SZ
  ##### 예제 값:
```
"10000-11999"
```


  #### Mac 정보 및 설정
  - 기본 설정 키 이름: WebRtcUdpPortRange
  - 예제 값:
``` xml
<string>10000-11999</string>
```
  

  [맨 위로 이동](#microsoft-edge---정책)


## 참고 항목
- [Microsoft Edge를 구성하는 중](configure-microsoft-edge.md)
- [Microsoft Edge 엔터프라이즈 방문 페이지](https://aka.ms/EdgeEnterprise)