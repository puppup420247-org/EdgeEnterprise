---
title: "Microsoft Edge Browser Policy Documentation"
ms.author: stmoody
author: brianalt-msft
manager: tahills
ms.date: 11/22/2019
audience: ITPro
ms.topic: reference
ms.prod: microsoft-edge
ms.localizationpriority: medium
ms.collection: M365-modern-desktop
ms.custom:
description: "Windows and Mac documentation for all policies supported by the Microsoft Edge Browser"
---

# Microsoft Edge - ポリシー
最新バージョンの Microsoft Edge には、次のポリシーが含まれています。これらのポリシーを使用して、組織での Microsoft Edge の実行方法を構成できます。

Microsoft Edge の更新方法と更新タイミングの制御に使用される他のポリシーについては、[Microsoft Edge 更新ポリシーのリファレンス](microsoft-edge-update-policies.md) を参照してください。

> [!注意]
> この記事は、Microsoft Edge バージョン 77 以降に適用されます。

## 利用可能なポリシー
これらの表には、Microsoft Edge のこのリリースで利用できるブラウザー関連のグループ ポリシーがすべて示されています。特定のポリシーの詳細を確認するには、表内のリンクを使用してください。

|||
|-|-|
|[Cast](#cast)|[HTTP 認証](#http-認証)|
|[SmartScreen の設定](#smartscreen-の設定)|[コンテンツの設定](#コンテンツの設定)|
|[スタートアップ、ホーム ページ、新しいタブ ページ](#スタートアップ、ホーム-ページ、新しいタブ-ページ)|[ネイティブ メッセージング](#ネイティブ-メッセージング)|
|[パスワード マネージャーと保護](#パスワード-マネージャーと保護)|[プロキシ サーバー](#プロキシ-サーバー)|
|[印刷](#印刷)|[拡張機能](#拡張機能)|
|[既定の検索プロバイダー](#既定の検索プロバイダー)|[Additional](#additional)|


### [*Cast*](#cast-policies)
|ポリシー名|キャプション|
|-|-|
|[EnableMediaRouter](#enablemediarouter)|Google Cast を有効にする|
|[ShowCastIconInToolbar](#showcasticonintoolbar)|ツール バーにキャスト アイコンを表示する|
### [*HTTP 認証*](#http-認証-policies)
|ポリシー名|キャプション|
|-|-|
|[AllowCrossOriginAuthPrompt](#allowcrossoriginauthprompt)|クロスオリジンでの HTTP 基本認証プロンプトを許可する|
|[AuthNegotiateDelegateAllowlist](#authnegotiatedelegateallowlist)|Microsoft Edge がユーザー資格情報を委任できるサーバーのリストを指定する|
|[AuthSchemes](#authschemes)|サポートされている認証スキーム|
|[AuthServerAllowlist](#authserverallowlist)|許可されている認証サーバーのリストを構成する|
|[DisableAuthNegotiateCnameLookup](#disableauthnegotiatecnamelookup)|Kerberos 認証をネゴシエートするときに CNAME 検索を無効にする|
|[EnableAuthNegotiatePort](#enableauthnegotiateport)|Kerberos SPN に非標準ポートを含める|
|[NtlmV2Enabled](#ntlmv2enabled)|NTLMv2 認証を有効にするかどうかを制御する|
### [*SmartScreen の設定*](#smartscreen-の設定-policies)
|ポリシー名|キャプション|
|-|-|
|[PreventSmartScreenPromptOverride](#preventsmartscreenpromptoverride)|サイトに関する Microsoft Defender SmartScreen プロンプトをバイパスしない|
|[PreventSmartScreenPromptOverrideForFiles](#preventsmartscreenpromptoverrideforfiles)|ダウンロードに関する Microsoft Defende SmartScreen の警告をバイパスしない|
|[SmartScreenAllowListDomains](#smartscreenallowlistdomains)|Microsoft Defender SmartScreen が警告をトリガーしないドメインのリストを構成する|
|[SmartScreenEnabled](#smartscreenenabled)|Microsoft Defender SmartScreen を構成する|
|[SmartScreenForTrustedDownloadsEnabled](#smartscreenfortrusteddownloadsenabled)|信頼された発行元からダウンロードするときに、Microsoft Defender SmartScreen のチェックを強制的に行う|
|[SmartScreenPuaEnabled](#smartscreenpuaenabled)|望ましくない可能性のあるアプリをブロックするように Microsoft Defender SmartScreen を構成する|
### [*コンテンツの設定*](#コンテンツの設定-policies)
|ポリシー名|キャプション|
|-|-|
|[AutoSelectCertificateForUrls](#autoselectcertificateforurls)|該当のサイトでクライアント証明書を自動的に選択する|
|[CookiesAllowedForUrls](#cookiesallowedforurls)|特定のサイトで Cookie を許可する|
|[CookiesBlockedForUrls](#cookiesblockedforurls)|特定のサイトで Cookie をブロックする|
|[CookiesSessionOnlyForUrls](#cookiessessiononlyforurls)|特定の Web サイトからの Cookie を現在のセッションに制限する|
|[DefaultCookiesSetting](#defaultcookiessetting)|Cookie を構成する|
|[DefaultGeolocationSetting](#defaultgeolocationsetting)|位置情報の既定の設定|
|[DefaultImagesSetting](#defaultimagessetting)|画像の既定の設定|
|[DefaultJavaScriptSetting](#defaultjavascriptsetting)|JavaScript の既定の設定|
|[DefaultNotificationsSetting](#defaultnotificationssetting)|通知の既定の設定|
|[DefaultPluginsSetting](#defaultpluginssetting)|Adobe Flash の既定の設定|
|[DefaultPopupsSetting](#defaultpopupssetting)|ポップアップ ウィンドウの既定の設定|
|[DefaultWebBluetoothGuardSetting](#defaultwebbluetoothguardsetting)|Web Bluetooth API の使用を制御する|
|[DefaultWebUsbGuardSetting](#defaultwebusbguardsetting)|WebUSB API の使用を制御する|
|[ImagesAllowedForUrls](#imagesallowedforurls)|これらのサイトでの画像表示を許可する|
|[ImagesBlockedForUrls](#imagesblockedforurls)|特定のサイトで画像をブロックする|
|[JavaScriptAllowedForUrls](#javascriptallowedforurls)|特定のサイトで JavaScript を許可する|
|[JavaScriptBlockedForUrls](#javascriptblockedforurls)|特定のサイトで JavaScript をブロックする|
|[LegacySameSiteCookieBehaviorEnabled](#legacysamesitecookiebehaviorenabled)|Enable default legacy SameSite cookie behavior setting|
|[LegacySameSiteCookieBehaviorEnabledForDomainList](#legacysamesitecookiebehaviorenabledfordomainlist)|Revert to legacy SameSite behavior for cookies on specified sites|
|[NotificationsAllowedForUrls](#notificationsallowedforurls)|特定のサイトで通知を許可する|
|[NotificationsBlockedForUrls](#notificationsblockedforurls)|特定のサイトで通知をブロックする|
|[PluginsAllowedForUrls](#pluginsallowedforurls)|特定のサイトで Adobe Flash プラグインを許可する|
|[PluginsBlockedForUrls](#pluginsblockedforurls)|特定のサイトで Adobe Flash プラグインをブロックする|
|[PopupsAllowedForUrls](#popupsallowedforurls)|特定のサイトでのポップアップ ウィンドウを許可する|
|[PopupsBlockedForUrls](#popupsblockedforurls)|特定のサイトでポップアップ ウィンドウをブロックする|
|[RegisteredProtocolHandlers](#registeredprotocolhandlers)|プロトコル ハンドラーを登録する|
|[WebUsbAllowDevicesForUrls](#webusballowdevicesforurls)|特定の USB デバイスに接続するために、特定のサイトへのアクセスを許可します|
|[WebUsbAskForUrls](#webusbaskforurls)|特定のサイトでの WebUSB を許可する|
|[WebUsbBlockedForUrls](#webusbblockedforurls)|特定のサイトでの WebUSB をブロックする|
### [*スタートアップ、ホーム ページ、新しいタブ ページ*](#スタートアップ、ホーム-ページ、新しいタブ-ページ-policies)
|ポリシー名|キャプション|
|-|-|
|[HomepageIsNewTabPage](#homepageisnewtabpage)|新しいタブ ページをホーム ページとして設定する|
|[HomepageLocation](#homepagelocation)|ホーム ページの URL を構成する|
|[NewTabPageCompanyLogo](#newtabpagecompanylogo)|新しいタブ ページでの会社のロゴを設定する|
|[NewTabPageHideDefaultTopSites](#newtabpagehidedefaulttopsites)|新しいタブ ページで既定のトップ サイトを非表示にする|
|[NewTabPageLocation](#newtabpagelocation)|新しいタブ ページの URL を構成する|
|[NewTabPageManagedQuickLinks](#newtabpagemanagedquicklinks)|新しいタブ ページのクイック リンクを設定する|
|[NewTabPageSetFeedType](#newtabpagesetfeedtype)|Microsoft Edge の新しいタブ ページ エクスペリエンスを構成する|
|[RestoreOnStartup](#restoreonstartup)|スタートアップ時に実行するアクション|
|[RestoreOnStartupURLs](#restoreonstartupurls)|ブラウザーの起動時に開くサイト|
|[ShowHomeButton](#showhomebutton)|ツール バーに [ホーム] ボタンを表示する|
### [*ネイティブ メッセージング*](#ネイティブ-メッセージング-policies)
|ポリシー名|キャプション|
|-|-|
|[NativeMessagingAllowlist](#nativemessagingallowlist)|ユーザーが使用できるネイティブ メッセージング ホストを制御する|
|[NativeMessagingBlocklist](#nativemessagingblocklist)|ネイティブ メッセージングの禁止リストを構成する|
|[NativeMessagingUserLevelHosts](#nativemessaginguserlevelhosts)|ユーザー レベルのネイティブ メッセージング ホスト (管理者のアクセス許可なしでインストールされるホスト) を許可する|
### [*パスワード マネージャーと保護*](#パスワード-マネージャーと保護-policies)
|ポリシー名|キャプション|
|-|-|
|[PasswordManagerEnabled](#passwordmanagerenabled)|パスワード マネージャーへのパスワードの保存を有効にする|
|[PasswordProtectionChangePasswordURL](#passwordprotectionchangepasswordurl)|パスワード変更 URL を構成する|
|[PasswordProtectionLoginURLs](#passwordprotectionloginurls)|パスワード保護サービスによってパスワードとしての指紋がキャプチャされるエンタープライズ ログイン URL のリストを構成する|
|[PasswordProtectionWarningTrigger](#passwordprotectionwarningtrigger)|パスワード保護の警告トリガーを構成する|
### [*プロキシ サーバー*](#プロキシ-サーバー-policies)
|ポリシー名|キャプション|
|-|-|
|[ProxyBypassList](#proxybypasslist)|プロキシバイパスの規則を構成する|
|[ProxyMode](#proxymode)|プロキシ サーバーの設定を構成する|
|[ProxyPacUrl](#proxypacurl)|プロキシ .pac ファイルの URL を設定する|
|[ProxyServer](#proxyserver)|プロキシ サーバーのアドレスまたは URL を構成する|
|[ProxySettings](#proxysettings)|プロキシの設定|
### [*印刷*](#印刷-policies)
|ポリシー名|キャプション|
|-|-|
|[DefaultPrinterSelection](#defaultprinterselection)|既定のプリンターの選択規則|
|[PrintHeaderFooter](#printheaderfooter)|ヘッダーとフッターを印刷する|
|[PrintPreviewUseSystemDefaultPrinter](#printpreviewusesystemdefaultprinter)|システム既定のプリンターを通常使用するプリンターとして設定する|
|[PrintingEnabled](#printingenabled)|印刷を有効にする|
|[UseSystemPrintDialog](#usesystemprintdialog)|システム印刷ダイアログを使用して印刷する|
### [*拡張機能*](#拡張機能-policies)
|ポリシー名|キャプション|
|-|-|
|[ExtensionAllowedTypes](#extensionallowedtypes)|許可される拡張機能の種類を構成する|
|[ExtensionInstallAllowlist](#extensioninstallallowlist)|特定の拡張機能のインストールを許可する|
|[ExtensionInstallBlocklist](#extensioninstallblocklist)|インストールできない拡張機能を制御する|
|[ExtensionInstallForcelist](#extensioninstallforcelist)|サイレント インストールされる拡張機能を制御する|
|[ExtensionInstallSources](#extensioninstallsources)|拡張機能およびユーザー スクリプトのインストール ソースを構成する|
|[ExtensionSettings](#extensionsettings)|拡張子の管理設定を構成する|
### [*既定の検索プロバイダー*](#既定の検索プロバイダー-policies)
|ポリシー名|キャプション|
|-|-|
|[DefaultSearchProviderEnabled](#defaultsearchproviderenabled)|既定の検索プロバイダーを有効にする|
|[DefaultSearchProviderEncodings](#defaultsearchproviderencodings)|既定の検索プロバイダーのエンコード|
|[DefaultSearchProviderImageURL](#defaultsearchproviderimageurl)|既定の検索プロバイダーの画像検索を指定する|
|[DefaultSearchProviderImageURLPostParams](#defaultsearchproviderimageurlpostparams)|POST を使用する画像の URL のパラメーター|
|[DefaultSearchProviderKeyword](#defaultsearchproviderkeyword)|既定の検索プロバイダーのキーワード|
|[DefaultSearchProviderName](#defaultsearchprovidername)|既定の検索プロバイダーの名前|
|[DefaultSearchProviderSearchURL](#defaultsearchprovidersearchurl)|既定の検索プロバイダーの検索 URL|
|[DefaultSearchProviderSuggestURL](#defaultsearchprovidersuggesturl)|検索候補を使用するための既定の検索プロバイダーの URL|
### [*Additional*](#additional-policies)
|ポリシー名|キャプション|
|-|-|
|[AdsSettingForIntrusiveAdsSites](#adssettingforintrusiveadssites)|押し付けがましい広告を表示するサイトに対する広告の設定|
|[AllowDeletingBrowserHistory](#allowdeletingbrowserhistory)|ブラウザーとダウンロードの履歴の削除を有効にする|
|[AllowFileSelectionDialogs](#allowfileselectiondialogs)|ファイルの選択ダイアログを許可する|
|[AllowPopupsDuringPageUnload](#allowpopupsduringpageunload)|ページのアンロード中にポップアップの表示を許可する|
|[AllowSyncXHRInPageDismissal](#allowsyncxhrinpagedismissal)|ページを閉じるときにページで同期 XHR 要求を送信することを許可する|
|[AllowTrackingForUrls](#allowtrackingforurls)|特定のサイトの追跡防止の例外を構成する|
|[AlwaysOpenPdfExternally](#alwaysopenpdfexternally)|PDF ファイルを常に外部で開く|
|[ApplicationLocaleValue](#applicationlocalevalue)|アプリケーションのロケールを設定する|
|[AudioCaptureAllowed](#audiocaptureallowed)|オーディオ キャプチャを許可または禁止する|
|[AudioCaptureAllowedUrls](#audiocaptureallowedurls)|アクセス許可を要求しなくてもオーディオ キャプチャ デバイスにアクセスできるサイト|
|[AutoImportAtFirstRun](#autoimportatfirstrun)|初回実行時に別のブラウザーのデータと設定を自動的にインポートする|
|[AutofillAddressEnabled](#autofilladdressenabled)|アドレスのオートフィルを有効にする|
|[AutofillCreditCardEnabled](#autofillcreditcardenabled)|クレジット カード情報についてオートフィルを有効にする|
|[AutoplayAllowed](#autoplayallowed)|Web サイトでのメディアの自動再生を許可する|
|[BackgroundModeEnabled](#backgroundmodeenabled)|Microsoft Edge が終了してもバックグラウンド アプリの実行を続行する|
|[BackgroundTemplateListUpdatesEnabled](#backgroundtemplatelistupdatesenabled)|利用可能なテンプレートの一覧に対するバックグラウンドでの更新を有効にします。このテンプレートとは、コレクションや、テンプレートを使用する他の機能で利用できるテンプレートです。|
|[BlockThirdPartyCookies](#blockthirdpartycookies)|サードパーティの Cookie をブロックする|
|[BrowserAddProfileEnabled](#browseraddprofileenabled)|ID ポップアップ メニューまたは [設定] ページでのプロファイル作成を有効にする|
|[BrowserGuestModeEnabled](#browserguestmodeenabled)|ゲスト モードを有効にする|
|[BrowserNetworkTimeQueriesEnabled](#browsernetworktimequeriesenabled)|ブラウザー ネットワーク タイム サービスへのクエリを許可する|
|[BrowserSignin](#browsersignin)|ブラウザー サインインの設定|
|[BuiltInDnsClientEnabled](#builtindnsclientenabled)|組み込みの DNS クライアントを使用する|
|[CertificateTransparencyEnforcementDisabledForCas](#certificatetransparencyenforcementdisabledforcas)|subjectPublicKeyInfo ハッシュのリストに対する証明書の透明性の適用を無効にする|
|[CertificateTransparencyEnforcementDisabledForLegacyCas](#certificatetransparencyenforcementdisabledforlegacycas)|レガシ証明機関のリストに対する証明書の透明性の適用を無効にする|
|[CertificateTransparencyEnforcementDisabledForUrls](#certificatetransparencyenforcementdisabledforurls)|特定の URL に対する証明書の透明性の適用を無効にする|
|[ClearBrowsingDataOnExit](#clearbrowsingdataonexit)|Microsoft Edge を閉じるときに閲覧データを消去する|
|[ClickOnceEnabled](#clickonceenabled)|ユーザーが ClickOnce プロトコルを使用してファイルを開くことを許可する|
|[CommandLineFlagSecurityWarningsEnabled](#commandlineflagsecuritywarningsenabled)|コマンドライン フラグのセキュリティ警告を有効にする|
|[ComponentUpdatesEnabled](#componentupdatesenabled)|Microsoft Edge でのコンポーネントの更新を有効にする|
|[ConfigureDoNotTrack](#configuredonottrack)|トラッキング拒否を構成する|
|[ConfigureOnlineTextToSpeech](#configureonlinetexttospeech)|オンライン音声合成を構成する|
|[CustomHelpLink](#customhelplink)|カスタム ヘルプのリンクを指定する|
|[DefaultBrowserSettingEnabled](#defaultbrowsersettingenabled)|Microsoft Edge を既定のブラウザーとして設定する|
|[DeveloperToolsAvailability](#developertoolsavailability)|開発者ツールを使用できる状況を制御する|
|[DirectInvokeEnabled](#directinvokeenabled)|ユーザーが DirectInvoke プロトコルを使用してファイルを開くことを許可する|
|[Disable3DAPIs](#disable3dapis)|3D グラフィックス API のサポートを無効にする|
|[DisableScreenshots](#disablescreenshots)|スクリーンショットの撮影を無効にする|
|[DiskCacheDir](#diskcachedir)|ディスク キャッシュ ディレクトリを設定する|
|[DiskCacheSize](#diskcachesize)|ディスク キャッシュ サイズをバイト単位で設定する|
|[DownloadDirectory](#downloaddirectory)|ディレクトリをダウンロードする|
|[DownloadRestrictions](#downloadrestrictions)|ダウンロードの制限を許可する|
|[EdgeCollectionsEnabled](#edgecollectionsenabled)|コレクション機能を有効にする|
|[EditFavoritesEnabled](#editfavoritesenabled)|ユーザーによるお気に入りの編集を許可する|
|[EnableDeprecatedWebPlatformFeatures](#enabledeprecatedwebplatformfeatures)|制限された期間、非推奨の Web プラットフォーム機能を再度有効にする|
|[EnableDomainActionsDownload](#enabledomainactionsdownload)|マイクロソフトからのドメイン アクションのダウンロードを有効にする|
|[EnableOnlineRevocationChecks](#enableonlinerevocationchecks)|オンライン OCSP/CRL チェックを有効にする|
|[EnterpriseHardwarePlatformAPIEnabled](#enterprisehardwareplatformapienabled)|管理された拡張機能を有効にして、エンタープライズ ハードウェア プラットフォーム API を使用する|
|[ExperimentationAndConfigurationServiceControl](#experimentationandconfigurationservicecontrol)|実験および構成サービスとの通信を制御する|
|[ExternalProtocolDialogShowAlwaysOpenCheckbox](#externalprotocoldialogshowalwaysopencheckbox)|外部プロトコルのダイアログで [常に開く] チェック ボックスを表示します。|
|[FavoritesBarEnabled](#favoritesbarenabled)|お気に入りバーを有効にする|
|[ForceBingSafeSearch](#forcebingsafesearch)|Bing セーフサーチを適用する|
|[ForceEphemeralProfiles](#forceephemeralprofiles)|一時プロファイルの使用を有効にする|
|[ForceGoogleSafeSearch](#forcegooglesafesearch)|Google セーフサーチを適用する|
|[ForceNetworkInProcess](#forcenetworkinprocess)|ブラウザー プロセスでネットワーク コードを強制的に実行する|
|[ForceYouTubeRestrict](#forceyoutuberestrict)|最小限の YouTube の制限モードを強制する|
|[FullscreenAllowed](#fullscreenallowed)|全画面表示モードを許可する|
|[GoToIntranetSiteForSingleWordEntryInAddressBar](#gotointranetsiteforsinglewordentryinaddressbar)|アドレス バーへの 1 単語の入力で検索するのではなく、ダイレクト イントラネット サイト ナビゲーションを強制します|
|[HSTSPolicyBypassList](#hstspolicybypasslist)|HSTS ポリシー チェックをバイパスする名前の一覧を構成します|
|[HardwareAccelerationModeEnabled](#hardwareaccelerationmodeenabled)|使用可能な場合はハードウェア アクセラレータを使用する|
|[ImportAutofillFormData](#importautofillformdata)|オートフィルのフォーム データのインポートを許可する|
|[ImportBrowserSettings](#importbrowsersettings)|ブラウザーの設定のインポートを許可する|
|[ImportFavorites](#importfavorites)|お気に入りのインポートを許可する|
|[ImportHistory](#importhistory)|閲覧の履歴のインポートを許可する|
|[ImportHomepage](#importhomepage)|ホーム ページの設定のインポートを許可する|
|[ImportOpenTabs](#importopentabs)|開いているタブのインポートを許可する|
|[ImportPaymentInfo](#importpaymentinfo)|支払情報のインポートを許可する|
|[ImportSavedPasswords](#importsavedpasswords)|保存したパスワードのインポートを許可する|
|[ImportSearchEngine](#importsearchengine)|検索エンジンの設定のインポートを許可する|
|[InPrivateModeAvailability](#inprivatemodeavailability)|InPrivate モードが利用できるかどうかを構成する|
|[InternetExplorerIntegrationLevel](#internetexplorerintegrationlevel)|Internet Explorer 統合を構成する|
|[InternetExplorerIntegrationSiteList](#internetexplorerintegrationsitelist)|エンタープライズ モード サイト一覧を構成する|
|[InternetExplorerIntegrationSiteRedirect](#internetexplorerintegrationsiteredirect)|Internet Explorer モードのページから開始した場合、未構成のサイトへの "ページ内" ナビゲーションがどのように動作するかを指定する|
|[IsolateOrigins](#isolateorigins)|特定の出所に対してサイトの分離を有効にする|
|[ManagedFavorites](#managedfavorites)|お気に入りを構成する|
|[ManagedSearchEngines](#managedsearchengines)|検索エンジンの管理|
|[MaxConnectionsPerProxy](#maxconnectionsperproxy)|プロキシ サーバーへの同時実行の最大接続数|
|[MediaRouterCastAllowAllIPs](#mediaroutercastallowallips)|すべての IP アドレスで Cast デバイスに接続することを Google Cast に許可する|
|[MetricsReportingEnabled](#metricsreportingenabled)|使用状況とクラッシュに関するデータのレポート送信を有効にする|
|[NetworkPredictionOptions](#networkpredictionoptions)|ネットワーク予測を有効にする|
|[NonRemovableProfileEnabled](#nonremovableprofileenabled)|職場または学校アカウントで自動的にサインインする既定のプロファイルを、ユーザーが常に持つ必要があるかどうかを構成する|
|[OverrideSecurityRestrictionsOnInsecureOrigin](#overridesecurityrestrictionsoninsecureorigin)|保護されていないオリジンに対するセキュリティ制限を適用する状況を制御する|
|[PinningWizardAllowed](#pinningwizardallowed)|Allow Pin to taskbar wizard|
|[ProactiveAuthEnabled](#proactiveauthenabled)|事前認証を有効にする|
|[PromotionalTabsEnabled](#promotionaltabsenabled)|タブ全体にプロモーション コンテンツを表示できるようにする|
|[PromptForDownloadLocation](#promptfordownloadlocation)|ダウンロードしたファイルの保存場所を確認する|
|[QuicAllowed](#quicallowed)|QUIC プロトコルを許可する|
|[RelaunchNotification](#relaunchnotification)|ブラウザーの再起動が推奨されるか、または必須であることをユーザーに通知する|
|[RelaunchNotificationPeriod](#relaunchnotificationperiod)|更新通知の期間を設定する|
|[RendererCodeIntegrityEnabled](#renderercodeintegrityenabled)|レンダラー コードの整合性を有効にする|
|[RequireOnlineRevocationChecksForLocalAnchors](#requireonlinerevocationchecksforlocalanchors)|トラスト アンカーに対してオンライン OCSP/CRL チェックが必要であるかどうかを指定する|
|[ResolveNavigationErrorsUseWebService](#resolvenavigationerrorsusewebservice)|Web サービスを使用してナビゲーション エラーを解決できるようにする|
|[RestrictSigninToPattern](#restrictsignintopattern)|Microsoft Edge プライマリ アカウントとして使用できるアカウントを制限する|
|[RunAllFlashInAllowMode](#runallflashinallowmode)|Adobe Flash コンテンツの設定をすべてのコンテンツに拡張する|
|[SSLErrorOverrideAllowed](#sslerroroverrideallowed)|ユーザーが HTTPS 警告ページから先に進むことを許可する|
|[SSLVersionMin](#sslversionmin)|有効な TLS バージョンを最小限に抑える|
|[SavingBrowserHistoryDisabled](#savingbrowserhistorydisabled)|ブラウザーの履歴の保存を無効にする|
|[SearchSuggestEnabled](#searchsuggestenabled)|検索候補を有効にする|
|[SecurityKeyPermitAttestation](#securitykeypermitattestation)|直接セキュリティ キー構成証明を使用するためのアクセス許可を必要としない Web サイトまたはドメイン|
|[SendIntranetToInternetExplorer](#sendintranettointernetexplorer)|すべてのイントラネット サイトを Internet Explorer に送る|
|[SendSiteInfoToImproveServices](#sendsiteinfotoimproveservices)|Microsoft サービスを改善するためにサイト情報を送信する|
|[ShowOfficeShortcutInFavoritesBar](#showofficeshortcutinfavoritesbar)|Microsoft Office のショートカットをお気に入りバーに表示する|
|[SignedHTTPExchangeEnabled](#signedhttpexchangeenabled)|Signed HTTP Exchange (SXG) のサポートを有効にする|
|[SitePerProcess](#siteperprocess)|すべてのサイトでサイト分離を有効にする|
|[SpellcheckEnabled](#spellcheckenabled)|スペルチェックを有効にする|
|[SpellcheckLanguage](#spellchecklanguage)|特定のスペルチェック言語を有効にする|
|[SpellcheckLanguageBlocklist](#spellchecklanguageblocklist)|スペルチェック言語を強制的に無効にする|
|[SuppressUnsupportedOSWarning](#suppressunsupportedoswarning)|サポートされていない OS の警告を表示しない|
|[SyncDisabled](#syncdisabled)|Microsoft 同期サービスを使用しているデータの同期を無効にする|
|[TabFreezingEnabled](#tabfreezingenabled)|バックグラウンド タブの固定を許可する|
|[TaskManagerEndProcessEnabled](#taskmanagerendprocessenabled)|ブラウザーのタスク マネージャーでプロセスの終了を有効にする|
|[TrackingPrevention](#trackingprevention)|ユーザーの Web 閲覧アクティビティの追跡をブロックする|
|[TranslateEnabled](#translateenabled)|翻訳を有効にする|
|[URLAllowlist](#urlallowlist)|許可されている URL のリストを定義する|
|[URLBlocklist](#urlblocklist)|URL のリストへのアクセスをブロックする|
|[UserDataDir](#userdatadir)|ユーザー データ ディレクトリを設定する|
|[UserFeedbackAllowed](#userfeedbackallowed)|ユーザー フィードバックを許可する|
|[VideoCaptureAllowed](#videocaptureallowed)|ビデオ キャプチャを許可または禁止する|
|[VideoCaptureAllowedUrls](#videocaptureallowedurls)|アクセス許可を要求しなくてもビデオ キャプチャ デバイスにアクセスできるサイト|
|[WPADQuickCheckEnabled](#wpadquickcheckenabled)|WPAD 最適化を設定する|
|[WebDriverOverridesIncompatiblePolicies](#webdriveroverridesincompatiblepolicies)|互換性のないポリシーのオーバーライドを WebDriver に許可する|
|[WebRtcLocalhostIpHandling](#webrtclocalhostiphandling)|WebRTC による localhost IP アドレスの公開を制限する|
|[WebRtcUdpPortRange](#webrtcudpportrange)|WebRTC で使用されるローカル UDP ポートの範囲を制限する|




  ## Cast policies

  [トップに戻る](#microsoft-edge---ポリシー)

  ### EnableMediaRouter
  #### Google Cast を有効にする
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  このポリシーを有効にした場合、Google Cast が有効になります。ユーザーは、アプリ メニュー、ページのコンテキスト メニュー、Cast 対応 Web サイトのメディア コントロール、および Cast ツール バー アイコン (表示されている場合) から、Google Cast を起動できます。

このポリシーを無効にした場合、Google Cast は無効になります。

既定では、Google Cast は有効になっています。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: いいえ - ブラウザーの再起動が必要です

  #### データ型:
  ブール値

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: EnableMediaRouter
  - GP の名前: Google Cast を有効にする
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/Cast
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: EnableMediaRouter
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000001
```


  #### Mac の情報と設定
  - 優先されるキーの名前: EnableMediaRouter
  - サンプル値:
``` xml
<true/>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### ShowCastIconInToolbar
  #### ツール バーにキャスト アイコンを表示する
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  このポリシーを true に設定すると、ツール バーまたはオーバーフロー メニューに Cast ツール バー アイコンが表示されます。ユーザーはこのアイコンを削除できません。

このポリシーを構成しなかった場合または無効にした場合、ユーザーは、コンテキスト メニューを使ってこのアイコンをピン留めしたり、削除したりすることができます。

[EnableMediaRouter](#enablemediarouter) ポリシーも false に設定されている場合、このポリシーは無視され、ツール バー アイコンは表示されません。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: いいえ - ブラウザーの再起動が必要です

  #### データ型:
  ブール値

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: ShowCastIconInToolbar
  - GP の名前: ツール バーにキャスト アイコンを表示する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/Cast
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: ShowCastIconInToolbar
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000000
```


  #### Mac の情報と設定
  - 優先されるキーの名前: ShowCastIconInToolbar
  - サンプル値:
``` xml
<false/>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ## HTTP 認証 policies

  [トップに戻る](#microsoft-edge---ポリシー)

  ### AllowCrossOriginAuthPrompt
  #### クロスオリジンでの HTTP 基本認証プロンプトを許可する
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  ページ上にあるサード パーティのサブコンテンツで [HTTP 基本認証] ダイアログ ボックスを開くことができるかどうかを制御します。

通常、これはフィッシング詐欺の防衛策として無効になっています。このポリシーを構成しなかった場合、ポリシーは無効になり、サード パーティのサブコンテンツで [HTTP 基本認証] ダイアログ ボックスを開くことはできません。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  ブール値

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: AllowCrossOriginAuthPrompt
  - GP の名前: クロスオリジンでの HTTP 基本認証プロンプトを許可する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/HTTP 認証
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: AllowCrossOriginAuthPrompt
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000000
```


  #### Mac の情報と設定
  - 優先されるキーの名前: AllowCrossOriginAuthPrompt
  - サンプル値:
``` xml
<false/>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### AuthNegotiateDelegateAllowlist
  #### Microsoft Edge がユーザー資格情報を委任できるサーバーのリストを指定する
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  Microsoft Edge が委任できるサーバーのリストを構成します。

複数のサーバー名を入力するときはコンマで区切ります。ワイルドカード（*）を使用できます。

このポリシーを構成しなかった場合、サーバーがイントラネット上で検出されても、Microsoft Edge はユーザー資格情報を委任しません。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: いいえ - ブラウザーの再起動が必要です

  #### データ型:
  文字列

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: AuthNegotiateDelegateAllowlist
  - GP の名前: Microsoft Edge がユーザー資格情報を委任できるサーバーのリストを指定する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/HTTP 認証
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: AuthNegotiateDelegateAllowlist
  - 値の種類: REG_SZ
  ##### サンプル値:
```
"contoso.com"
```


  #### Mac の情報と設定
  - 優先されるキーの名前: AuthNegotiateDelegateAllowlist
  - サンプル値:
``` xml
<string>contoso.com</string>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### AuthSchemes
  #### サポートされている認証スキーム
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  サポートされる HTTP 認証スキームを指定します。

このポリシーは、'basic'、'digest'、'ntlm'、'negotiate' の各値を使用して構成できます。値が複数ある場合はコンマで区切ります。

このポリシーを構成しなかった場合、4 つのスキームすべてが使用されます。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: いいえ - ブラウザーの再起動が必要です

  #### データ型:
  文字列

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: AuthSchemes
  - GP の名前: サポートされている認証スキーム
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/HTTP 認証
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: AuthSchemes
  - 値の種類: REG_SZ
  ##### サンプル値:
```
"basic,digest,ntlm,negotiate"
```


  #### Mac の情報と設定
  - 優先されるキーの名前: AuthSchemes
  - サンプル値:
``` xml
<string>basic,digest,ntlm,negotiate</string>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### AuthServerAllowlist
  #### 許可されている認証サーバーのリストを構成する
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  統合認証を有効にするサーバーを指定します。統合認証が有効になるのはMicrosoft Edge がこのリストに含まれているプロキシやサーバーから認証チャレンジを受信した場合のみです。

サーバー名を複数指定する場合はコンマで区切ります。ワイルドカード (*) を使用できます。

このポリシーを構成しなかった場合、Microsoft Edge はサーバーがイントラネット上にあるかどうかの検出を試行し、検出された場合にのみ、IWA 要求に応答します。サーバーがインターネット上にある場合は、そのサーバーからの IWA 要求は Microsoft Edge では無視されます。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: いいえ - ブラウザーの再起動が必要です

  #### データ型:
  文字列

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: AuthServerAllowlist
  - GP の名前: 許可されている認証サーバーのリストを構成する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/HTTP 認証
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: AuthServerAllowlist
  - 値の種類: REG_SZ
  ##### サンプル値:
```
"*contoso.com,contoso.com"
```


  #### Mac の情報と設定
  - 優先されるキーの名前: AuthServerAllowlist
  - サンプル値:
``` xml
<string>*contoso.com,contoso.com</string>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### DisableAuthNegotiateCnameLookup
  #### Kerberos 認証をネゴシエートするときに CNAME 検索を無効にする
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  正規の DNS 名 (CNAME) または入力された元の名前のどちらを基準にして Kerberos SPN を生成するかを決定します。

このポリシーを有効にした場合、CNAME 検索がスキップされ、入力したサーバー名がそのまま使用されます。

このポリシーを無効にした場合または構成しなかった場合、サーバーの正規名が使用されます。このサーバーの正規名は CNAME 検索によって決まります。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: いいえ - ブラウザーの再起動が必要です

  #### データ型:
  ブール値

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: DisableAuthNegotiateCnameLookup
  - GP の名前: Kerberos 認証をネゴシエートするときに CNAME 検索を無効にする
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/HTTP 認証
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: DisableAuthNegotiateCnameLookup
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000000
```


  #### Mac の情報と設定
  - 優先されるキーの名前: DisableAuthNegotiateCnameLookup
  - サンプル値:
``` xml
<false/>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### EnableAuthNegotiatePort
  #### Kerberos SPN に非標準ポートを含める
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  生成された Kerberos SPN に非標準ポートを含めるかどうかを指定します。

このポリシーを有効にした場合、ユーザーが非標準ポート (80 と 443 以外のポート) を URL に含めると、生成された Kerberos SPN にそのポートが含まれます。

このポリシーを構成しなかった場合または無効にした場合は、どのような状況でも、生成された Kerberos SPN にはポートは含まれません。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: いいえ - ブラウザーの再起動が必要です

  #### データ型:
  ブール値

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: EnableAuthNegotiatePort
  - GP の名前: Kerberos SPN に非標準ポートを含める
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/HTTP 認証
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: EnableAuthNegotiatePort
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000000
```


  #### Mac の情報と設定
  - 優先されるキーの名前: EnableAuthNegotiatePort
  - サンプル値:
``` xml
<false/>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### NtlmV2Enabled
  #### NTLMv2 認証を有効にするかどうかを制御する
  >サポートされているバージョン: Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  NTLMv2 を有効にするかどうかを指定します。

最新バージョンのすべての Samba サーバーと Windows サーバーでは、NTLMv2 がサポートされています。下位互換性の問題を解決する場合にのみ、NTLMv2 を無効にしてください。NTLMv2 を無効すると、認証のセキュリティが低下するためです。

このポリシーを構成しなかった場合、NTLMv2 は既定で有効になります。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  ブール値

  

  #### Mac の情報と設定
  - 優先されるキーの名前: NtlmV2Enabled
  - サンプル値:
``` xml
<true/>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ## SmartScreen の設定 policies

  [トップに戻る](#microsoft-edge---ポリシー)

  ### PreventSmartScreenPromptOverride
  #### サイトに関する Microsoft Defender SmartScreen プロンプトをバイパスしない
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  This policy setting lets you decide whether users can override the Microsoft Defender SmartScreen warnings about potentially malicious websites.

If you enable this setting, users can't ignore Microsoft Defender SmartScreen warnings and they are blocked from continuing to the site.

If you disable or don't configure this setting, users can ignore Microsoft Defender SmartScreen warnings and continue to the site.

This policy is available only on Windows instances that are joined to a Microsoft Active Directory domain; or on Windows 10 Pro or Enterprise instances that are enrolled for device management.

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  ブール値

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: PreventSmartScreenPromptOverride
  - GP の名前: サイトに関する Microsoft Defender SmartScreen プロンプトをバイパスしない
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/SmartScreen の設定
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: PreventSmartScreenPromptOverride
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000001
```


  #### Mac の情報と設定
  - 優先されるキーの名前: PreventSmartScreenPromptOverride
  - サンプル値:
``` xml
<true/>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### PreventSmartScreenPromptOverrideForFiles
  #### ダウンロードに関する Microsoft Defende SmartScreen の警告をバイパスしない
  >サポートされているバージョン: Windows (バージョン 77 以降)、および Mac (バージョン 79 以降) の Microsoft Edge

  #### 説明
  This policy lets you determine whether users can override Microsoft Defender SmartScreen warnings about unverified downloads.

If you enable this policy, users in your organization can't ignore Microsoft Defender SmartScreen warnings, and they're prevented from completing the unverified downloads.

If you disable or don't configure this policy, users can ignore Microsoft Defender SmartScreen warnings and complete unverified downloads.

This policy is available only on Windows instances that are joined to a Microsoft Active Directory domain; or on Windows 10 Pro or Enterprise instances that are enrolled for device management.

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  ブール値

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: PreventSmartScreenPromptOverrideForFiles
  - GP の名前: ダウンロードに関する Microsoft Defende SmartScreen の警告をバイパスしない
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/SmartScreen の設定
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: PreventSmartScreenPromptOverrideForFiles
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000001
```


  #### Mac の情報と設定
  - 優先されるキーの名前: PreventSmartScreenPromptOverrideForFiles
  - サンプル値:
``` xml
<true/>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### SmartScreenAllowListDomains
  #### Microsoft Defender SmartScreen が警告をトリガーしないドメインのリストを構成する
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  Configure the list of Microsoft Defender SmartScreen trusted domains. This means:
Microsoft Defender SmartScreen won't check for potentially malicious resources like phishing software and other malware if the source URLs match these domains.
The Microsoft Defender SmartScreen download protection service won't check downloads hosted on these domains.

If you enable this policy, Microsoft Defender SmartScreen trusts these domains.
If you disable or don't set this policy, default Microsoft Defender SmartScreen protection is applied to all resources.

This policy is available only on Windows instances that are joined to a Microsoft Active Directory domain; or on Windows 10 Pro or Enterprise instances that are enrolled for device management.
Also note that this policy does not apply if your organization has enabled Microsoft Defender Advanced Threat Protection. You must configure your allow and block lists in Microsoft Defender Security Center instead.

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  文字列の一覧

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: SmartScreenAllowListDomains
  - GP の名前: Microsoft Defender SmartScreen が警告をトリガーしないドメインのリストを構成する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/SmartScreen の設定
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge\SmartScreenAllowListDomains
  - パス (おすすめ): N/A
  - 値の名前: 1, 2, 3, ...
  - 値の種類: REG_SZ の一覧
  ##### サンプル値:
```
SOFTWARE\Policies\Microsoft\Edge\SmartScreenAllowListDomains\0 = "mydomain.com"
SOFTWARE\Policies\Microsoft\Edge\SmartScreenAllowListDomains\1 = "myuniversity.edu"

```


  #### Mac の情報と設定
  - 優先されるキーの名前: SmartScreenAllowListDomains
  - サンプル値:
``` xml
<array>
  <string>mydomain.com</string>
  <string>myuniversity.edu</string>
</array>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### SmartScreenEnabled
  #### Microsoft Defender SmartScreen を構成する
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  このポリシー設定では、Microsoft Defender SmartScreen を有効にするかどうかを構成できます。Microsoft Defender SmartScreen は、フィッシング詐欺や悪意のあるソフトウェアの可能性からユーザーを保護するための警告メッセージを提示します。既定では、Microsoft Defender SmartScreen は有効になります。

この設定を有効にした場合、Microsoft Defender SmartScreen が有効になります。

この設定を無効にした場合、Microsoft Defender SmartScreen が無効になります。

この設定を構成しなかった場合、Microsoft Defender SmartScreen を使用するかどうかをユーザーが選択できます。

このポリシーは、Microsoft Active Directory ドメインに参加している Windows インスタンス、またはデバイス管理に登録されている Windows 10 Pro インスタンスや Windows 10 Enterprise インスタンスでのみ利用できます。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: はい
  - 動的ポリシーの更新: はい

  #### データ型:
  ブール値

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: SmartScreenEnabled
  - GP の名前: Microsoft Defender SmartScreen を構成する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/SmartScreen の設定
  - GP パス (おすすめ): 管理用テンプレート/Microsoft Edge - 既定の設定 (ユーザーはオーバーライドできます)/SmartScreen の設定
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): SOFTWARE\Policies\Microsoft\Edge\おすすめ
  - 値の名前: SmartScreenEnabled
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000001
```


  #### Mac の情報と設定
  - 優先されるキーの名前: SmartScreenEnabled
  - サンプル値:
``` xml
<true/>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### SmartScreenForTrustedDownloadsEnabled
  #### 信頼された発行元からダウンロードするときに、Microsoft Defender SmartScreen のチェックを強制的に行う
  >サポートされているバージョン: Windows (バージョン 78 以降) の Microsoft Edge

  #### 説明
  このポリシー設定では、Microsoft Defender SmartScreen が信頼できる発行元からダウンロード評価を確認するかどうかを構成できます。

この設定を有効にした場合または構成しなかった場合は、Microsoft Defender SmartScreen は、発行元にかかわらずダウンロード評価を確認します。

この設定を無効にした場合、Microsoft Defender SmartScreen は、信頼できる発行元からダウンロードする際にダウンロード評価を確認しません。

このポリシーは、Microsoft Active Directory ドメインに参加している Windows インスタンス、またはデバイス管理用に登録されている Windows 10 Pro または Enterprise インスタンスにでのみ使用できます。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: はい
  - 動的ポリシーの更新: はい

  #### データ型:
  ブール値

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: SmartScreenForTrustedDownloadsEnabled
  - GP の名前: 信頼された発行元からダウンロードするときに、Microsoft Defender SmartScreen のチェックを強制的に行う
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/SmartScreen の設定
  - GP パス (おすすめ): 管理用テンプレート/Microsoft Edge - 既定の設定 (ユーザーはオーバーライドできます)/SmartScreen の設定
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): SOFTWARE\Policies\Microsoft\Edge\おすすめ
  - 値の名前: SmartScreenForTrustedDownloadsEnabled
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000000
```


  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### SmartScreenPuaEnabled
  #### 望ましくない可能性のあるアプリをブロックするように Microsoft Defender SmartScreen を構成する
  >サポートされているバージョン: Windows および Mac (バージョン 80 以降) の Microsoft Edge

  #### 説明
  このポリシー設定では、Microsoft Defender SmartScreen で望ましくない可能性のあるアプリのブロックを有効にするかどうかを構成できます。Microsoft Defender SmartScreen で望ましくない可能性のあるアプリをブロックすると、Web サイトでホストされているアドウェア、コイン マイナー、バンドルウェア、および他の低評価のアプリからユーザーを保護するための警告メッセージが提示されます。既定では、Microsoft Defender SmartScreen での望ましくない可能性のあるアプリのブロックは無効になります。

この設定を有効にした場合、Microsoft Defender SmartScreen での望ましくない可能性のあるアプリのブロックが有効になります。

この設定を無効にした場合、Microsoft Defender SmartScreen での望ましくない可能性のあるアプリのブロックが無効になります。

この設定を構成しなかった場合、Microsoft Defender SmartScreen で望ましくない可能性のあるアプリのブロックを使用するかどうかはユーザーが選択できます。

このポリシーは、Microsoft Active Directory ドメインに参加している Windows インスタンス、またはデバイス管理に登録されている Windows 10 Pro インスタンスや Windows 10 Enterprise インスタンスでのみ利用できます。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: はい
  - 動的ポリシーの更新: はい

  #### データ型:
  ブール値

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: SmartScreenPuaEnabled
  - GP の名前: 望ましくない可能性のあるアプリをブロックするように Microsoft Defender SmartScreen を構成する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/SmartScreen の設定
  - GP パス (おすすめ): 管理用テンプレート/Microsoft Edge - 既定の設定 (ユーザーはオーバーライドできます)/SmartScreen の設定
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): SOFTWARE\Policies\Microsoft\Edge\おすすめ
  - 値の名前: SmartScreenPuaEnabled
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000001
```


  #### Mac の情報と設定
  - 優先されるキーの名前: SmartScreenPuaEnabled
  - サンプル値:
``` xml
<true/>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ## コンテンツの設定 policies

  [トップに戻る](#microsoft-edge---ポリシー)

  ### AutoSelectCertificateForUrls
  #### 該当のサイトでクライアント証明書を自動的に選択する
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  サイトがクライアント証明書を要求している場合に Microsoft Edge でクライアント証明書を自動的に選択するサイトのリストを、URL パターンに基づいて定義します。

値は、文字列化した JSON 辞書の配列で指定する必要があります。各辞書の形式は、{ "pattern": "$URL_PATTERN", "filter" : $FILTER } になっている必要があります。$URL_PATTERN はコンテンツ設定パターンを表します。$FILTER によって、ブラウザーで自動的に選択されるクライアント証明書の発行元を絞り込みます。ただしフィルターの設定に関わらず、選択されるのは、サーバーの証明書の要求に一致する証明書のみです。たとえば、$FILTER を { "ISSUER": { "CN": "$ISSUER_CN" } } という形式で指定すると、CommonName $ISSUER_CN を持つ証明書によって発行されたクライアント証明書のみが選択されます。$FILTER に "ISSUER" と "SUBJECT" のセクションが含まれている場合、クライアント証明書は、選択対象となる両方の条件を満たしている必要があります。$FILTER に組織 ("O") が指定されている場合、証明書は、選択対象となる指定の値に一致する組織を 1 つ以上含んでいる必要があります。$FILTER に組織単位 ("OU") が指定されている場合、証明書は、選択対象となる指定の値に一致する組織単位を 1 つ以上含んでいる必要があります。$FILTER が空の辞書 {} の場合、クライアント証明書の選択は、こうした制限を受けません。

このポリシーを構成しなかった場合、どのサイトについても証明書の自動選択は行われません。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  文字列の一覧

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: AutoSelectCertificateForUrls
  - GP の名前: 該当のサイトでクライアント証明書を自動的に選択する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/コンテンツの設定
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge\AutoSelectCertificateForUrls
  - パス (おすすめ): N/A
  - 値の名前: 1, 2, 3, ...
  - 値の種類: REG_SZ の一覧
  ##### サンプル値:
```
SOFTWARE\Policies\Microsoft\Edge\AutoSelectCertificateForUrls\0 = "{"pattern":"https://www.contoso.com","filter":{"ISSUER":{"CN":"certificate issuer name", "L": "certificate issuer location", "O": "certificate issuer org", "OU": "certificate issuer org unit"}, "SUBJECT":{"CN":"certificate subject name", "L": "certificate subject location", "O": "certificate subject org", "OU": "certificate subject org unit"}}}"

```


  #### Mac の情報と設定
  - 優先されるキーの名前: AutoSelectCertificateForUrls
  - サンプル値:
``` xml
<array>
  <string>{"pattern":"https://www.contoso.com","filter":{"ISSUER":{"CN":"certificate issuer name", "L": "certificate issuer location", "O": "certificate issuer org", "OU": "certificate issuer org unit"}, "SUBJECT":{"CN":"certificate subject name", "L": "certificate subject location", "O": "certificate subject org", "OU": "certificate subject org unit"}}}</string>
</array>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### CookiesAllowedForUrls
  #### 特定のサイトで Cookie を許可する
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  Cookie の設定が許可されるサイトのリストを、URL パターンに基づいて定義します。

このポリシーを構成しなかった場合、すべてのサイトで、[DefaultCookiesSetting](#defaultcookiessetting) ポリシーのグローバル デフォルト値 (設定されている場合)、またはユーザーの個人用の構成が使用されます。

詳細については、[CookiesBlockedForUrls](#cookiesblockedforurls) ポリシーと [CookiesSessionOnlyForUrls](#cookiessessiononlyforurls) ポリシーを参照してください。

以下の 3 つのポリシーでは、URL パターンが競合しない必要があります。

- [CookiesBlockedForUrls](#cookiesblockedforurls)

- CookiesAllowedForUrls

- [CookiesSessionOnlyForUrls](#cookiessessiononlyforurls)

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  文字列の一覧

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: CookiesAllowedForUrls
  - GP の名前: 特定のサイトで Cookie を許可する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/コンテンツの設定
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge\CookiesAllowedForUrls
  - パス (おすすめ): N/A
  - 値の名前: 1, 2, 3, ...
  - 値の種類: REG_SZ の一覧
  ##### サンプル値:
```
SOFTWARE\Policies\Microsoft\Edge\CookiesAllowedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\CookiesAllowedForUrls\1 = "[*.]contoso.edu"

```


  #### Mac の情報と設定
  - 優先されるキーの名前: CookiesAllowedForUrls
  - サンプル値:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### CookiesBlockedForUrls
  #### 特定のサイトで Cookie をブロックする
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  Cookie を設定できないサイトのリストを、URL パターンに基づいて定義します。

このポリシーを構成しなかった場合、すべてのサイトで、[DefaultCookiesSetting](#defaultcookiessetting) ポリシーのグローバル デフォルト値 (設定されている場合)、またはユーザーの個人用の構成が使用されます。

詳細については、[CookiesAllowedForUrls](#cookiesallowedforurls) ポリシーと [CookiesSessionOnlyForUrls](#cookiessessiononlyforurls) ポリシーを参照してください。

以下の 3 つのポリシーでは、URL パターンが競合しない必要があります。

- CookiesBlockedForUrls

- [CookiesAllowedForUrls](#cookiesallowedforurls)

- [CookiesSessionOnlyForUrls](#cookiessessiononlyforurls)

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  文字列の一覧

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: CookiesBlockedForUrls
  - GP の名前: 特定のサイトで Cookie をブロックする
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/コンテンツの設定
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge\CookiesBlockedForUrls
  - パス (おすすめ): N/A
  - 値の名前: 1, 2, 3, ...
  - 値の種類: REG_SZ の一覧
  ##### サンプル値:
```
SOFTWARE\Policies\Microsoft\Edge\CookiesBlockedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\CookiesBlockedForUrls\1 = "[*.]contoso.edu"

```


  #### Mac の情報と設定
  - 優先されるキーの名前: CookiesBlockedForUrls
  - サンプル値:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### CookiesSessionOnlyForUrls
  #### 特定の Web サイトからの Cookie を現在のセッションに制限する
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  定義した URL パターンに一致する Web サイトで作成された Cookie は、セッションの終了時 (ウィンドウを閉じたとき) に削除されます。

パターンに一致しない Web サイトで作成された Cookie は、[DefaultCookiesSetting](#defaultcookiessetting) ポリシー (設定されている場合)、またはユーザーの個人用の構成によって制御されます。これは、このポリシーを構成しなかった場合の既定の動作でもあります。

Microsoft Edge がバックグラウンド モードで実行されていると、最後のウィンドウを閉じたときに、セッションが終了しない場合があります。この場合、ウィンドウを閉じても Cookie は消去されません。Microsoft Edge がバックグラウンド モードで実行されているときに、どのような処理を行うかを構成する方法の詳細については、[BackgroundModeEnabled](#backgroundmodeenabled) ポリシーを参照してください。

Cookie を作成できる Web サイトを制御する場合は、[CookiesAllowedForUrls](#cookiesallowedforurls) ポリシーと [CookiesBlockedForUrls](#cookiesblockedforurls) ポリシーを使用することもできます。

以下の 3 つのポリシーでは、URL パターンが競合しない必要があります。

- [CookiesBlockedForUrls](#cookiesblockedforurls)

- [CookiesAllowedForUrls](#cookiesallowedforurls)

- CookiesSessionOnlyForUrls

前のセッションから URL を復元するように [RestoreOnStartup](#restoreonstartup) ポリシーを設定した場合、このポリシーは無視され、それらのサイトでは Cookie が 永続的に保存されます。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  文字列の一覧

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: CookiesSessionOnlyForUrls
  - GP の名前: 特定の Web サイトからの Cookie を現在のセッションに制限する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/コンテンツの設定
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge\CookiesSessionOnlyForUrls
  - パス (おすすめ): N/A
  - 値の名前: 1, 2, 3, ...
  - 値の種類: REG_SZ の一覧
  ##### サンプル値:
```
SOFTWARE\Policies\Microsoft\Edge\CookiesSessionOnlyForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\CookiesSessionOnlyForUrls\1 = "[*.]contoso.edu"

```


  #### Mac の情報と設定
  - 優先されるキーの名前: CookiesSessionOnlyForUrls
  - サンプル値:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### DefaultCookiesSetting
  #### Cookie を構成する
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  Web サイトがユーザーのデバイスに Cookie を作成できるかどうかを制御します。このポリシーは、すべての Web サイトを対象とするか、対象としないかのいずれかです。つまり、すべての Web サイトで Cookie の作成を許可するか、許可しないかを制御できます。このポリシーを使用して、特定の Web サイトからの Cookie を有効にすることはできません。

ポリシーを 'SessionOnly' (4) に設定すると、セッションの終了時に Cookie が消去されます。Microsoft Edge がバックグラウンド モードで実行されていると、最後のウィンドウを閉じたときに、セッションが終了しない場合があります。この場合、ウィンドウを閉じても Cookie は消去されません。Microsoft Edge がバックグラウンド モードで実行されているときに、どのような処理を行うかを構成する方法の詳細については、[BackgroundModeEnabled](#backgroundmodeenabled) ポリシーを参照してください。

このポリシーを構成しなかった場合、既定の 'AllowCookies' (1) が使用され、ユーザーはこの設定を Microsoft Edge の [設定] で変更できます (ユーザーがこの設定を変更できないようにする場合は、ポリシーを構成してください)。

* 1 = すべてのサイトで Cookie の作成を許可する

* 2 = すべてのサイトで Cookie の作成を許可しない

* 4 = セッションの継続中は Cookie を保存する

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  整数

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: DefaultCookiesSetting
  - GP の名前: Cookie を構成する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/コンテンツの設定
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: DefaultCookiesSetting
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000001
```


  #### Mac の情報と設定
  - 優先されるキーの名前: DefaultCookiesSetting
  - サンプル値:
``` xml
<integer>1</integer>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### DefaultGeolocationSetting
  #### 位置情報の既定の設定
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  Web サイトでユーザーの物理的な場所を追跡できるかどうかを設定します。既定で追跡を許可 (1) したり、禁止 (2) したりすることができます。また、ユーザーの場所が Web サイトで必要になるたびにユーザーに確認 (3) することもできます。

このポリシーを構成しなかった場合、'AskGeolocation' ポリシーが使用され、ユーザーは 'AskGeolocation' ポリシーを変更できます。

* 1 = サイトに対してユーザーの物理的な場所の追跡を許可する

* 2 = すべてのサイトに対してユーザーの物理的な場所の追跡を許可しない

* 3 = サイトでユーザーの物理的な場所を追跡する場合は常に確認する

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  整数

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: DefaultGeolocationSetting
  - GP の名前: 位置情報の既定の設定
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/コンテンツの設定
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: DefaultGeolocationSetting
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000001
```


  #### Mac の情報と設定
  - 優先されるキーの名前: DefaultGeolocationSetting
  - サンプル値:
``` xml
<integer>1</integer>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### DefaultImagesSetting
  #### 画像の既定の設定
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  Web サイトで画像を表示できるかどうかを設定します。画像の表示は、すべてのサイトに対して許可 (1) したり、禁止 (2) したりすることができます。

このポリシーを構成しなかった場合、既定で画像の表示は許可されますが、ユーザーはこの設定を変更できます。

* 1 = すべてのサイトに対して画像の表示を許可する

* 2 = すべてのサイトに対して画像の表示を許可しない

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  整数

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: DefaultImagesSetting
  - GP の名前: 画像の既定の設定
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/コンテンツの設定
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: DefaultImagesSetting
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000001
```


  #### Mac の情報と設定
  - 優先されるキーの名前: DefaultImagesSetting
  - サンプル値:
``` xml
<integer>1</integer>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### DefaultJavaScriptSetting
  #### JavaScript の既定の設定
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  Web サイトで JavaScript を実行できるかどうかを設定します。JavaScript の実行は、すべてのサイトで許可したり (1)、すべてのサイトで禁止したり (2) することができます。

このポリシーを構成しなかった場合、既定ではすべてのサイトで JavaScript を実行できますが、ユーザーはこの設定を変更できます。

* 1 = すべてのサイトで JavaScript の実行を許可する

* 2 = すべてのサイトで JavaScript の実行を許可しない

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  整数

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: DefaultJavaScriptSetting
  - GP の名前: JavaScript の既定の設定
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/コンテンツの設定
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: DefaultJavaScriptSetting
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000001
```


  #### Mac の情報と設定
  - 優先されるキーの名前: DefaultJavaScriptSetting
  - サンプル値:
``` xml
<integer>1</integer>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### DefaultNotificationsSetting
  #### 通知の既定の設定
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  Web サイトがデスクトップ通知を表示できるかどうかを設定します。通知の表示を既定で許可 (1) したり、通知の表示を既定で禁止 (2) したりすることができます。また、Web サイトで通知の表示が必要になるたびにユーザーに確認することもできます (3)。

このポリシーを構成しなかった場合、通知の表示は既定で許可されますが、ユーザーはこの設定を変更できます。

* 1 = サイトに対してデスクトップ通知の表示を許可する

* 2 = どのサイトに対してもデスクトップ通知の表示を許可しない

* 3 = サイトでデスクトップ通知の表示が必要になった場合に毎回確認する

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  整数

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: DefaultNotificationsSetting
  - GP の名前: 通知の既定の設定
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/コンテンツの設定
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: DefaultNotificationsSetting
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000002
```


  #### Mac の情報と設定
  - 優先されるキーの名前: DefaultNotificationsSetting
  - サンプル値:
``` xml
<integer>2</integer>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### DefaultPluginsSetting
  #### Adobe Flash の既定の設定
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  [PluginsAllowedForUrls](#pluginsallowedforurls) や [PluginsBlockedForUrls](#pluginsblockedforurls) が適用されない Web サイトで、Adobe Flash プラグインを自動的に実行できるかどうかを設定します。すべてのサイトで Adobe Flash をブロックするには、'BlockPlugins' (2) を選択できます。Adobe Flash の実行を許可するには、'ClickToPlay' (3) を選択できますが、この場合、ユーザーはプレースホルダーをクリックしてプラグインを起動する必要があります。どちらの場合も、[PluginsAllowedForUrls](#pluginsallowedforurls) ポリシーと [PluginsBlockedForUrls](#pluginsblockedforurls) ポリシーは 'DefaultPluginsSetting' ポリシーよりも優先されます。

自動再生は、[PluginsAllowedForUrls](#pluginsallowedforurls) ポリシーでリストに明示的に指定されているドメインに対してのみ許可されます。すべてのサイトで自動再生を有効にする場合は、このリストに http://* や https://* を追加することを検討してください。

このポリシーを構成しなかった場合、ユーザーはこの設定を手動で変更できます。

* 2 = Adobe Flash プラグインをブロックする

* 3 = クリックして再生する

以前の '1' オプションではすべてのサイトで実行を許可するように設定していましたが、現在この機能は、[PluginsAllowedForUrls](#pluginsallowedforurls) ポリシーでのみ処理されます。'1' を使用している既存のポリシーは、クリックして再生モードで機能します。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  整数

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: DefaultPluginsSetting
  - GP の名前: Adobe Flash の既定の設定
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/コンテンツの設定
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: DefaultPluginsSetting
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000002
```


  #### Mac の情報と設定
  - 優先されるキーの名前: DefaultPluginsSetting
  - サンプル値:
``` xml
<integer>2</integer>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### DefaultPopupsSetting
  #### ポップアップ ウィンドウの既定の設定
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  Web サイトでポップアップ ウィンドウを表示できるかどうかを設定します。ポップアップ ウィンドウの表示は、すべての Web サイトに対して許可 (1) したり、禁止 (2) したりすることができます。

このポリシーを構成しなかった場合、既定でポップアップ ウィンドウはブロックされますが、ユーザーはこの設定を変更できます。

* 1 = すべてのサイトに対してポップアップ表示を許可する

* 2 = すべてのサイトに対してポップアップ表示を許可しない

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  整数

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: DefaultPopupsSetting
  - GP の名前: ポップアップ ウィンドウの既定の設定
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/コンテンツの設定
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: DefaultPopupsSetting
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000001
```


  #### Mac の情報と設定
  - 優先されるキーの名前: DefaultPopupsSetting
  - サンプル値:
``` xml
<integer>1</integer>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### DefaultWebBluetoothGuardSetting
  #### Web Bluetooth API の使用を制御する
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  Web サイトが近くにある Bluetooth デバイスにアクセスできるかどうかを制御します。アクセスを完全に禁止したり、Bluetooth デバイスにアクセスする必要がある場合は、サイトで毎回ユーザーに確認するように要求したりすることができます。

このポリシーを構成しなかった場合、既定値 (3、ユーザーは毎回確認されます) が使用されます、ユーザーはこの設定を変更できます。

* 2 = すべてのサイトに対して、Web Bluetooth API を使用した Bluetooth デバイスへのアクセスの要求を許可しない

* 3 = サイトでは、近くにある Bluetooth デバイスへのアクセスを許可するようにユーザーに確認することができる

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  整数

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: DefaultWebBluetoothGuardSetting
  - GP の名前: Web Bluetooth API の使用を制御する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/コンテンツの設定
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: DefaultWebBluetoothGuardSetting
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000002
```


  #### Mac の情報と設定
  - 優先されるキーの名前: DefaultWebBluetoothGuardSetting
  - サンプル値:
``` xml
<integer>2</integer>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### DefaultWebUsbGuardSetting
  #### WebUSB API の使用を制御する
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  Web サイトが、接続されている USB デバイスにアクセスできるかどうかを設定します。アクセスを完全にブロックしたり、接続されている USB デバイスへのアクセスが Web サイトで必要になるたびにユーザーに確認したりすることができます。

特定の URL パターンに対してこのポリシーをオーバーライドすることができます。そのためには、[WebUsbAskForUrls](#webusbaskforurls) ポリシーと [WebUsbBlockedForUrls](#webusbblockedforurls) ポリシーを使用します。

このポリシーを構成しなかった場合、既定では、接続されている USB デバイスにサイトがアクセスできるかどうかをユーザーに確認しますが (3)、ユーザーはこの設定を変更できます。

* 2 = すべてのサイトに対して、WebUSB API を使用した USB デバイスへのアクセスの要求を許可しない

* 3 = サイトに対して、接続されている USB デバイスへのアクセス権を付与するようユーザーに確認すること許可する

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  整数

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: DefaultWebUsbGuardSetting
  - GP の名前: WebUSB API の使用を制御する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/コンテンツの設定
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: DefaultWebUsbGuardSetting
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000002
```


  #### Mac の情報と設定
  - 優先されるキーの名前: DefaultWebUsbGuardSetting
  - サンプル値:
``` xml
<integer>2</integer>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### ImagesAllowedForUrls
  #### これらのサイトでの画像表示を許可する
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  画像の表示できるサイトのリストを、URL パターンに基づいて定義します。

このポリシーを構成しなかった場合、すべてのサイトで、[DefaultImagesSetting](#defaultimagessetting) ポリシーのグローバル デフォルト値 (設定されている場合)、またはユーザーの個人用の構成が使用されます。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  文字列の一覧

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: ImagesAllowedForUrls
  - GP の名前: これらのサイトでの画像表示を許可する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/コンテンツの設定
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge\ImagesAllowedForUrls
  - パス (おすすめ): N/A
  - 値の名前: 1, 2, 3, ...
  - 値の種類: REG_SZ の一覧
  ##### サンプル値:
```
SOFTWARE\Policies\Microsoft\Edge\ImagesAllowedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\ImagesAllowedForUrls\1 = "[*.]contoso.edu"

```


  #### Mac の情報と設定
  - 優先されるキーの名前: ImagesAllowedForUrls
  - サンプル値:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### ImagesBlockedForUrls
  #### 特定のサイトで画像をブロックする
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  画像の表示が禁止されるサイトのリストを、URL パターンに基づいて定義します。

このポリシーを構成しなかった場合、すべてのサイトで、[DefaultImagesSetting](#defaultimagessetting) ポリシーのグローバル デフォルト値 (設定されている場合)、またはユーザーの個人用の構成が使用されます。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  文字列の一覧

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: ImagesBlockedForUrls
  - GP の名前: 特定のサイトで画像をブロックする
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/コンテンツの設定
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge\ImagesBlockedForUrls
  - パス (おすすめ): N/A
  - 値の名前: 1, 2, 3, ...
  - 値の種類: REG_SZ の一覧
  ##### サンプル値:
```
SOFTWARE\Policies\Microsoft\Edge\ImagesBlockedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\ImagesBlockedForUrls\1 = "[*.]contoso.edu"

```


  #### Mac の情報と設定
  - 優先されるキーの名前: ImagesBlockedForUrls
  - サンプル値:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### JavaScriptAllowedForUrls
  #### 特定のサイトで JavaScript を許可する
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  JavaScript の実行が許可されるサイトのリストを、URL パターンに基づいて定義します。

このポリシーを構成しなかった場合、すべてのサイトで、[DefaultJavaScriptSetting](#defaultjavascriptsetting) ポリシーのグローバル デフォルト値 (設定されている場合)、またはユーザーの個人用の構成が使用されます。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  文字列の一覧

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: JavaScriptAllowedForUrls
  - GP の名前: 特定のサイトで JavaScript を許可する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/コンテンツの設定
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge\JavaScriptAllowedForUrls
  - パス (おすすめ): N/A
  - 値の名前: 1, 2, 3, ...
  - 値の種類: REG_SZ の一覧
  ##### サンプル値:
```
SOFTWARE\Policies\Microsoft\Edge\JavaScriptAllowedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\JavaScriptAllowedForUrls\1 = "[*.]contoso.edu"

```


  #### Mac の情報と設定
  - 優先されるキーの名前: JavaScriptAllowedForUrls
  - サンプル値:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### JavaScriptBlockedForUrls
  #### 特定のサイトで JavaScript をブロックする
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  JavaScript の実行が許可されないサイトのリストを、URL パターンに基づいて定義します。

このポリシーを構成しなかった場合、すべてのサイトで、[DefaultJavaScriptSetting](#defaultjavascriptsetting) ポリシーのグローバル デフォルト値 (設定されている場合)、またはユーザーの個人用の構成が使用されます。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  文字列の一覧

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: JavaScriptBlockedForUrls
  - GP の名前: 特定のサイトで JavaScript をブロックする
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/コンテンツの設定
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge\JavaScriptBlockedForUrls
  - パス (おすすめ): N/A
  - 値の名前: 1, 2, 3, ...
  - 値の種類: REG_SZ の一覧
  ##### サンプル値:
```
SOFTWARE\Policies\Microsoft\Edge\JavaScriptBlockedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\JavaScriptBlockedForUrls\1 = "[*.]contoso.edu"

```


  #### Mac の情報と設定
  - 優先されるキーの名前: JavaScriptBlockedForUrls
  - サンプル値:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### LegacySameSiteCookieBehaviorEnabled
  #### Enable default legacy SameSite cookie behavior setting
  >サポートされているバージョン: Windows および Mac (バージョン 80 以降) の Microsoft Edge

  #### 説明
  Lets you revert all cookies to legacy SameSite behavior. Reverting to legacy behavior causes cookies that don't specify a SameSite attribute to be treated as if they were "SameSite=None", and removes the requirement for "SameSite=None" cookies to carry the "Secure" attribute.

You can set the following values for this policy:

* 1 = Revert to legacy SameSite behavior for cookies on all sites

* 2 = Use SameSite-by-default behavior for cookies on all sites

If you don't set this policy, the default behavior for cookies that don't specify a SameSite attribute will depend on other configuration sources for the SameSite-by-default feature. This feature might be set by a field trial or by enabling the same-site-by-default-cookies flag in edge://flags.

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  整数

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: LegacySameSiteCookieBehaviorEnabled
  - GP の名前: Enable default legacy SameSite cookie behavior setting
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/コンテンツの設定
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: LegacySameSiteCookieBehaviorEnabled
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000001
```


  #### Mac の情報と設定
  - 優先されるキーの名前: LegacySameSiteCookieBehaviorEnabled
  - サンプル値:
``` xml
<integer>1</integer>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### LegacySameSiteCookieBehaviorEnabledForDomainList
  #### Revert to legacy SameSite behavior for cookies on specified sites
  >サポートされているバージョン: Windows および Mac (バージョン 80 以降) の Microsoft Edge

  #### 説明
  Cookies set for domains match specified patterns will revert to legacy SameSite behavior.

Reverting to legacy behavior causes cookies that don't specify a SameSite attribute to be treated as if they were "SameSite=None", and removes the requirement for "SameSite=None" cookies to carry the "Secure" attribute.

If you don't set this policy, the global default value will be used. The global default will also be used for cookies on domains not covered by the patterns you specify.

The global default value can be configured using the [LegacySameSiteCookieBehaviorEnabled](#legacysamesitecookiebehaviorenabled) policy. If [LegacySameSiteCookieBehaviorEnabled](#legacysamesitecookiebehaviorenabled) is unset, the global default value falls back to other configuration sources.

Note that patterns you list in this policy are treated as domains, not URLs, so you should not specify a scheme or port.

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  文字列の一覧

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: LegacySameSiteCookieBehaviorEnabledForDomainList
  - GP の名前: Revert to legacy SameSite behavior for cookies on specified sites
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/コンテンツの設定
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge\LegacySameSiteCookieBehaviorEnabledForDomainList
  - パス (おすすめ): N/A
  - 値の名前: 1, 2, 3, ...
  - 値の種類: REG_SZ の一覧
  ##### サンプル値:
```
SOFTWARE\Policies\Microsoft\Edge\LegacySameSiteCookieBehaviorEnabledForDomainList\0 = "www.example.com"
SOFTWARE\Policies\Microsoft\Edge\LegacySameSiteCookieBehaviorEnabledForDomainList\1 = "[*.]example.edu"

```


  #### Mac の情報と設定
  - 優先されるキーの名前: LegacySameSiteCookieBehaviorEnabledForDomainList
  - サンプル値:
``` xml
<array>
  <string>www.example.com</string>
  <string>[*.]example.edu</string>
</array>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### NotificationsAllowedForUrls
  #### 特定のサイトで通知を許可する
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  通知を表示できるサイトのリストを、URL パターンに基づいて定義します。

このポリシーを構成しなかった場合、すべてのサイトで、[DefaultNotificationsSetting](#defaultnotificationssetting) ポリシーのグローバル デフォルト値 (設定されている場合)、またはユーザーの個人用の構成が使用されます。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  文字列の一覧

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: NotificationsAllowedForUrls
  - GP の名前: 特定のサイトで通知を許可する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/コンテンツの設定
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge\NotificationsAllowedForUrls
  - パス (おすすめ): N/A
  - 値の名前: 1, 2, 3, ...
  - 値の種類: REG_SZ の一覧
  ##### サンプル値:
```
SOFTWARE\Policies\Microsoft\Edge\NotificationsAllowedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\NotificationsAllowedForUrls\1 = "[*.]contoso.edu"

```


  #### Mac の情報と設定
  - 優先されるキーの名前: NotificationsAllowedForUrls
  - サンプル値:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### NotificationsBlockedForUrls
  #### 特定のサイトで通知をブロックする
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  通知の表示が禁止されるサイトのリストを、URL パターンに基づいて定義します。

このポリシーを構成しなかった場合、すべてのサイトで、[DefaultNotificationsSetting](#defaultnotificationssetting) ポリシーのグローバル デフォルト値 (設定されている場合)、またはユーザーの個人用の構成が使用されます。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  文字列の一覧

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: NotificationsBlockedForUrls
  - GP の名前: 特定のサイトで通知をブロックする
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/コンテンツの設定
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge\NotificationsBlockedForUrls
  - パス (おすすめ): N/A
  - 値の名前: 1, 2, 3, ...
  - 値の種類: REG_SZ の一覧
  ##### サンプル値:
```
SOFTWARE\Policies\Microsoft\Edge\NotificationsBlockedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\NotificationsBlockedForUrls\1 = "[*.]contoso.edu"

```


  #### Mac の情報と設定
  - 優先されるキーの名前: NotificationsBlockedForUrls
  - サンプル値:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### PluginsAllowedForUrls
  #### 特定のサイトで Adobe Flash プラグインを許可する
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  Adobe Flash プラグインを実行できるサイトのリストを、URL パターンに基づいて定義します。

このポリシーを構成しなかった場合、すべてのサイトで、[DefaultPluginsSetting](#defaultpluginssetting) ポリシーのグローバル デフォルト値 (設定されている場合)、またはユーザーの個人用の構成が使用されます。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  文字列の一覧

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: PluginsAllowedForUrls
  - GP の名前: 特定のサイトで Adobe Flash プラグインを許可する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/コンテンツの設定
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge\PluginsAllowedForUrls
  - パス (おすすめ): N/A
  - 値の名前: 1, 2, 3, ...
  - 値の種類: REG_SZ の一覧
  ##### サンプル値:
```
SOFTWARE\Policies\Microsoft\Edge\PluginsAllowedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\PluginsAllowedForUrls\1 = "[*.]contoso.edu"

```


  #### Mac の情報と設定
  - 優先されるキーの名前: PluginsAllowedForUrls
  - サンプル値:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### PluginsBlockedForUrls
  #### 特定のサイトで Adobe Flash プラグインをブロックする
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  Adobe Flash の実行が禁止されるサイトのリストを、URL パターンに基づいて定義します。

このポリシーを構成しなかった場合、すべてのサイトで、[DefaultPluginsSetting](#defaultpluginssetting) ポリシーのグローバル デフォルト値 (設定されている場合)、またはユーザーの個人用の構成が使用されます。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  文字列の一覧

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: PluginsBlockedForUrls
  - GP の名前: 特定のサイトで Adobe Flash プラグインをブロックする
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/コンテンツの設定
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge\PluginsBlockedForUrls
  - パス (おすすめ): N/A
  - 値の名前: 1, 2, 3, ...
  - 値の種類: REG_SZ の一覧
  ##### サンプル値:
```
SOFTWARE\Policies\Microsoft\Edge\PluginsBlockedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\PluginsBlockedForUrls\1 = "[*.]contoso.edu"

```


  #### Mac の情報と設定
  - 優先されるキーの名前: PluginsBlockedForUrls
  - サンプル値:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### PopupsAllowedForUrls
  #### 特定のサイトでのポップアップ ウィンドウを許可する
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  ポップアップ ウィンドウを開くことができるサイトのリストを、URL パターンに基づいて定義します。

このポリシーを構成しなかった場合、すべてのサイトで、[DefaultPopupsSetting](#defaultpopupssetting) ポリシーのグローバル デフォルト値 (設定されている場合)、またはユーザーの個人用の構成が使用されます。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  文字列の一覧

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: PopupsAllowedForUrls
  - GP の名前: 特定のサイトでのポップアップ ウィンドウを許可する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/コンテンツの設定
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge\PopupsAllowedForUrls
  - パス (おすすめ): N/A
  - 値の名前: 1, 2, 3, ...
  - 値の種類: REG_SZ の一覧
  ##### サンプル値:
```
SOFTWARE\Policies\Microsoft\Edge\PopupsAllowedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\PopupsAllowedForUrls\1 = "[*.]contoso.edu"

```


  #### Mac の情報と設定
  - 優先されるキーの名前: PopupsAllowedForUrls
  - サンプル値:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### PopupsBlockedForUrls
  #### 特定のサイトでポップアップ ウィンドウをブロックする
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  ポップアップ ウィンドウを開くことが禁止されているサイトのリストを、URL パターンに基づいて定義します。

このポリシーを構成しなかった場合、すべてのサイトで、[DefaultPopupsSetting](#defaultpopupssetting) ポリシーのグローバル デフォルト値 (設定されている場合)、またはユーザーの個人用の構成が使用されます。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  文字列の一覧

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: PopupsBlockedForUrls
  - GP の名前: 特定のサイトでポップアップ ウィンドウをブロックする
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/コンテンツの設定
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge\PopupsBlockedForUrls
  - パス (おすすめ): N/A
  - 値の名前: 1, 2, 3, ...
  - 値の種類: REG_SZ の一覧
  ##### サンプル値:
```
SOFTWARE\Policies\Microsoft\Edge\PopupsBlockedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\PopupsBlockedForUrls\1 = "[*.]contoso.edu"

```


  #### Mac の情報と設定
  - 優先されるキーの名前: PopupsBlockedForUrls
  - サンプル値:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### RegisteredProtocolHandlers
  #### プロトコル ハンドラーを登録する
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  プロトコル ハンドラーの一覧を登録します。プロトコル プロパティをスキーム (「mailto」など) に設定し、URL プロパティをスキームを処理するアプリケーションの URL パターンに設定します。このパターンには「%s」を含めることができます。これは、処理される URL に置き換えられます。

このポリシーに対して特定の値を推奨することはできますが、ユーザーにその値を使用するよう要求することはできません。

ポリシーによって登録されたプロトコル ハンドラーは、ユーザーが登録したハンドラーと統合され、両方を使用できるようになります。ユーザーは新しい既定のハンドラーをインストールすることで、ポリシーによってインストールされたプロトコル ハンドラーを上書きできますが、ポリシーによって登録されたプロトコル ハンドラーを削除することはできません。

  #### サポートされている機能:
  - 必須になる場合があります: いいえ
  - 推奨される場合があります: はい
  - 動的ポリシーの更新: いいえ - ブラウザーの再起動が必要です

  #### データ型:
  辞書

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: RegisteredProtocolHandlers
  - GP の名前: プロトコル ハンドラーを登録する
  - GP パス (必須): N/A
  - GP パス (おすすめ): 管理用テンプレート/Microsoft Edge - 既定の設定 (ユーザーはオーバーライドできます)/コンテンツの設定
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): N/A
  - パス (おすすめ): SOFTWARE\Policies\Microsoft\Edge\おすすめ
  - 値の名前: RegisteredProtocolHandlers
  - 値の種類: REG_SZ
  ##### サンプル値:
```
SOFTWARE\Policies\Microsoft\Edge\RegisteredProtocolHandlers = [
  {
    "default": true, 
    "protocol": "mailto", 
    "url": "https://mail.contoso.com/mail/?extsrc=mailto&url=%s"
  }
]
```


  #### Mac の情報と設定
  - 優先されるキーの名前: RegisteredProtocolHandlers
  - サンプル値:
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
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### WebUsbAllowDevicesForUrls
  #### 特定の USB デバイスに接続するために、特定のサイトへのアクセスを許可します
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  URL のリストを設定して、特定のベンダー ID と製品 ID を持つ USB デバイスへのアクセス許可が自動的に付与されるサイトを指定することを許可します。ポリシーを有効にするには、リストの各項目にデバイスと URL の両方が含まれている必要があります。デバイスに関する各項目には、ベンダー ID と製品 ID のフィールドを含めることができます。省略された ID はすべて、ワイルドカードとして扱われます。ただし、製品 ID を指定するときはベンダー ID も指定する必要があるので、注意してください。ベンダー ID を指定しないで製品 ID を指定した場合、このポリシーは無効になり、無視されます。

USB アクセス許可モデルでは、要求元サイト ("要求元 URL") の URL とトップレベルのフレーム サイト ("埋め込み URL") の URL を使用して、要求元 URL に対して USB デバイスへのアクセス許可を付与します。要求元サイトが iframe に読み込まれる場合、要求元 URL は、埋め込み URL とは異なる可能性があります。このため、"urls" フィールドに最大 2 個までの URL 文字列を含めて (コンマで区切ります)、要求元 URL と埋め込み URL をそれぞれ指定することができます。URL を 1 つだけ指定した場合は、埋め込みの状態に関係なく、要求元サイトの URL がこの URL と一致すると、対応する USB デバイスへのアクセスが許可されます。"urls" 内の URL は有効な URL である必要があります。有効な URL でない場合は、ポリシーは無視されます。

このポリシーを設定しなかった場合、すべてのサイトで、[DefaultWebUsbGuardSetting](#defaultwebusbguardsetting) ポリシーのグローバル デフォルト値 (設定されている場合)、またはユーザーの個人用の構成が使用されます。

このポリシーでの URL パターンは、[WebUsbBlockedForUrls](#webusbblockedforurls) で構成されているパターンとは重複しないパターンを指定してください。パターンが重複する場合、このポリシーは [WebUsbBlockedForUrls](#webusbblockedforurls) および [WebUsbAskForUrls](#webusbaskforurls) よりも優先されます。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  辞書

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: WebUsbAllowDevicesForUrls
  - GP の名前: 特定の USB デバイスに接続するために、特定のサイトへのアクセスを許可します
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/コンテンツの設定
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: WebUsbAllowDevicesForUrls
  - 値の種類: REG_SZ
  ##### サンプル値:
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


  #### Mac の情報と設定
  - 優先されるキーの名前: WebUsbAllowDevicesForUrls
  - サンプル値:
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
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### WebUsbAskForUrls
  #### 特定のサイトでの WebUSB を許可する
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  USB デバイスへのアクセスをユーザーに確認できるサイトのリストを、URL パターンに基づいて定義します。

このポリシーを構成しなかった場合、すべてのサイトで、[DefaultWebUsbGuardSetting](#defaultwebusbguardsetting) ポリシーのグローバル デフォルト値 (設定されている場合)、またはユーザーの個人用の構成が使用されます。

このポリシーで定義する URL パターンは、[WebUsbBlockedForUrls](#webusbblockedforurls) ポリシーで構成されている URL パターンと競合しないようにする必要があります。URL の許可とブロックの両方を構成することはできません。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  文字列の一覧

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: WebUsbAskForUrls
  - GP の名前: 特定のサイトでの WebUSB を許可する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/コンテンツの設定
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge\WebUsbAskForUrls
  - パス (おすすめ): N/A
  - 値の名前: 1, 2, 3, ...
  - 値の種類: REG_SZ の一覧
  ##### サンプル値:
```
SOFTWARE\Policies\Microsoft\Edge\WebUsbAskForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\WebUsbAskForUrls\1 = "[*.]contoso.edu"

```


  #### Mac の情報と設定
  - 優先されるキーの名前: WebUsbAskForUrls
  - サンプル値:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### WebUsbBlockedForUrls
  #### 特定のサイトでの WebUSB をブロックする
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  USB デバイスへのアクセスの許可をユーザーに確認できないサイトのリストを、URL パターンに基づいて定義します。

このポリシーを構成しなかった場合、すべてのサイトで、[DefaultWebUsbGuardSetting](#defaultwebusbguardsetting) ポリシーのグローバル デフォルト値 (設定されている場合)、またはユーザーの個人用の構成が使用されます。

このポリシーで定義する URL パターンは、[WebUsbAskForUrls](#webusbaskforurls) ポリシーで構成されている URL パターンと競合しないようにする必要があります。URL の許可とブロックの両方を構成することはできません。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  文字列の一覧

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: WebUsbBlockedForUrls
  - GP の名前: 特定のサイトでの WebUSB をブロックする
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/コンテンツの設定
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge\WebUsbBlockedForUrls
  - パス (おすすめ): N/A
  - 値の名前: 1, 2, 3, ...
  - 値の種類: REG_SZ の一覧
  ##### サンプル値:
```
SOFTWARE\Policies\Microsoft\Edge\WebUsbBlockedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\WebUsbBlockedForUrls\1 = "[*.]contoso.edu"

```


  #### Mac の情報と設定
  - 優先されるキーの名前: WebUsbBlockedForUrls
  - サンプル値:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ## スタートアップ、ホーム ページ、新しいタブ ページ policies

  [トップに戻る](#microsoft-edge---ポリシー)

  ### HomepageIsNewTabPage
  #### 新しいタブ ページをホーム ページとして設定する
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  Microsoft Edge の既定のホームページを構成します。ホームページは、指定の URL に設定したり、新しいタブ ページに設定したりすることができます。

このポリシーを有効にした場合、新しいタブ ページが常にホームページに使用され、ホームページの URL の場所は無視されます。

このポリシーを無効にした場合、URL を 'edge://newtab' に設定しない限り、ユーザーのホームページは新しいタブ ページとして設定できません。

このポリシーを構成しなかった場合、ユーザーは新しいタブ ページをホーム ページにするかどうかを選択できます。

このポリシーは、Microsoft Active Directory ドメインに参加している Windows インスタンス、またはデバイス管理に登録されている Windows 10 Pro インスタンスや Windows 10 Enterprise インスタンスでのみ利用できます。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: はい
  - 動的ポリシーの更新: はい

  #### データ型:
  ブール値

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: HomepageIsNewTabPage
  - GP の名前: 新しいタブ ページをホーム ページとして設定する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/スタートアップ、ホーム ページ、新しいタブ ページ
  - GP パス (おすすめ): 管理用テンプレート/Microsoft Edge - 既定の設定 (ユーザーはオーバーライドできます)/スタートアップ、ホーム ページ、新しいタブ ページ
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): SOFTWARE\Policies\Microsoft\Edge\おすすめ
  - 値の名前: HomepageIsNewTabPage
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000001
```


  #### Mac の情報と設定
  - 優先されるキーの名前: HomepageIsNewTabPage
  - サンプル値:
``` xml
<true/>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### HomepageLocation
  #### ホーム ページの URL を構成する
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  Microsoft Edge での既定のホーム ページの URL を構成します。

ホーム ページは、[ホーム] ボタンで開くページです。スタートアップ時に開くページは、[RestoreOnStartup](#restoreonstartup) ポリシーで制御します。

ここで URL を設定することも、新しいタブ ページを開くようにホームページを設定することもできます。新しいタブ ページを開くように選択した場合、このポリシーは適用されません。

このポリシーを有効にすると、ユーザーはホームページの URL を変更できなくなりますが、新しいタブ ページをホームページとして選択することはできます。

このポリシーを無効にした場合または構成しなかった場合、[HomepageIsNewTabPage](#homepageisnewtabpage) ポリシーが有効になっていなければ、ユーザーは自分のホームページを選択できます。

このポリシーは、Microsoft Active Directory ドメインに参加している Windows インスタンス、またはデバイス管理に登録されている Windows 10 Pro インスタンスや Windows 10 Enterprise インスタンスでのみ利用できます。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: はい
  - 動的ポリシーの更新: はい

  #### データ型:
  文字列

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: HomepageLocation
  - GP の名前: ホーム ページの URL を構成する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/スタートアップ、ホーム ページ、新しいタブ ページ
  - GP パス (おすすめ): 管理用テンプレート/Microsoft Edge - 既定の設定 (ユーザーはオーバーライドできます)/スタートアップ、ホーム ページ、新しいタブ ページ
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): SOFTWARE\Policies\Microsoft\Edge\おすすめ
  - 値の名前: HomepageLocation
  - 値の種類: REG_SZ
  ##### サンプル値:
```
"https://www.contoso.com"
```


  #### Mac の情報と設定
  - 優先されるキーの名前: HomepageLocation
  - サンプル値:
``` xml
<string>https://www.contoso.com</string>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### NewTabPageCompanyLogo
  #### 新しいタブ ページでの会社のロゴを設定する
  >サポートされているバージョン: Windows および Mac (バージョン 79 以降) の Microsoft Edge

  #### 説明
  Specifies the company logo to use on the new tab page in Microsoft Edge.

The policy should be configured as a string that expresses the logo(s) in JSON format. For example: { "default_logo": { "url": "https://www.contoso.com/logo.png", "hash": "cd0aa9856147b6c5b4ff2b7dfee5da20aa38253099ef1b4a64aced233c9afe29" }, "light_logo": { "url": "https://www.contoso.com/light_logo.png", "hash": "517d286edb416bb2625ccfcba9de78296e90da8e32330d4c9c8275c4c1c33737" } }

You configure this policy by specifying the URL from which Microsoft Edge can download the logo and its cryptographic hash (SHA-256), which is used to verify the integrity of the download. The logo must be in PNG or SVG format, and its file size must not exceed 16 MB. The logo is downloaded and cached, and it will be redownloaded whenever the URL or the hash changes. The URL must be accessible without any authentication.

The 'default_logo' is required and will be used when there's no background image. If 'light_logo' is provided, it will be used when the user's new tab page has a background image. We recommend a horizontal logo with a transparent background that is left-aligned and vertically centered. The logo should have a minimum height of 32 pixels and an aspect ratio from 1:1 to 4:1. The 'default_logo' should have proper contrast against a white/black background while the 'light_logo' should have proper contrast against a background image.

If you enable this policy, Microsoft Edge downloads and shows the specified logo(s) on the new tab page. Users can't override or hide the logo(s).

If you disable or don't configure this policy, Microsoft Edge will show no company logo or a Microsoft logo on the new tab page.

For help with determining the SHA-256 hash, see https://docs.microsoft.com/powershell/module/microsoft.powershell.utility/get-filehash.

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: いいえ - ブラウザーの再起動が必要です

  #### データ型:
  辞書

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: NewTabPageCompanyLogo
  - GP の名前: 新しいタブ ページでの会社のロゴを設定する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/スタートアップ、ホーム ページ、新しいタブ ページ
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: NewTabPageCompanyLogo
  - 値の種類: REG_SZ
  ##### サンプル値:
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


  #### Mac の情報と設定
  - 優先されるキーの名前: NewTabPageCompanyLogo
  - サンプル値:
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
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### NewTabPageHideDefaultTopSites
  #### 新しいタブ ページで既定のトップ サイトを非表示にする
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  Microsoft Edge で、新しいタブ ページに既定のトップ サイトが表示されないようにします。

このポリシーを true に設定した場合、既定のトップ サイトのタイルが非表示になります。

このポリシーを false に設定した場合または構成しなかった場合は、既定のトップ サイトのタイルは表示されたままになります。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  ブール値

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: NewTabPageHideDefaultTopSites
  - GP の名前: 新しいタブ ページで既定のトップ サイトを非表示にする
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/スタートアップ、ホーム ページ、新しいタブ ページ
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: NewTabPageHideDefaultTopSites
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000001
```


  #### Mac の情報と設定
  - 優先されるキーの名前: NewTabPageHideDefaultTopSites
  - サンプル値:
``` xml
<true/>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### NewTabPageLocation
  #### 新しいタブ ページの URL を構成する
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  新しいタブ ページの既定の URL を構成します。

このポリシーは、新しいタブの作成時 (新しいウィンドウを開いた時も含む) に開くページを特定します。また、スタートアップ ページで新しいタブ ページを開くように設定している場合は、スタートアップ ページに対しても適用されます。

このポリシーでは、スタートアップ時に開くページは特定されません。このようなページは、[RestoreOnStartup](#restoreonstartup) ポリシーによって制御されます。またこのポリシーは、ホーム ページで新しいタブ ページを開くように設定している場合でも、ホーム ページに対しては適用されません。

このポリシーを構成しなかった場合、既定の新しいタブ ページが使用されます。

このポリシー*および* [NewTabPageSetFeedType](#newtabpagesetfeedtype) ポリシーを構成した場合は、このポリシーが優先されます。

無効な URL が指定された場合、新しいタブで about://blank が開きます。

このポリシーは、Microsoft Active Directory ドメインに参加している Windows インスタンス、またはデバイス管理に登録されている Windows 10 Pro インスタンスや Windows 10 Enterprise インスタンスでのみ利用できます。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: はい
  - 動的ポリシーの更新: はい

  #### データ型:
  文字列

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: NewTabPageLocation
  - GP の名前: 新しいタブ ページの URL を構成する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/スタートアップ、ホーム ページ、新しいタブ ページ
  - GP パス (おすすめ): 管理用テンプレート/Microsoft Edge - 既定の設定 (ユーザーはオーバーライドできます)/スタートアップ、ホーム ページ、新しいタブ ページ
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): SOFTWARE\Policies\Microsoft\Edge\おすすめ
  - 値の名前: NewTabPageLocation
  - 値の種類: REG_SZ
  ##### サンプル値:
```
"https://www.fabrikam.com"
```


  #### Mac の情報と設定
  - 優先されるキーの名前: NewTabPageLocation
  - サンプル値:
``` xml
<string>https://www.fabrikam.com</string>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### NewTabPageManagedQuickLinks
  #### 新しいタブ ページのクイック リンクを設定する
  >サポートされているバージョン: Windows および Mac (バージョン 79 以降) の Microsoft Edge

  #### 説明
  既定では、Microsoft Edge は、ユーザーが追加したショートカットや閲覧の履歴に基づくトップ サイトから開かれる新しいタブ ページにクイック リンクを表示します。このポリシーでは、新しいタブページにクイック リンクのタイルを 3 つまで構成できます。これらのタイルは JSON オブジェクトとして表します

[ { "url": "https://www.contoso.com", "title": "Contoso Portal", "pinned": true/false }, ... ]

'url' フィールドは必須です。'title' と 'pinned' はオプションです。'title' が指定されていない場合は、URL が既定のタイトルとして使用されます。'pinned' が指定されていない場合は、既定値は false になります。

Microsoft Edge では、これらのタイルがリスト指定された順に、左から右へ表示されます。また、ピン留めされたすべてのタイルは、ピン留めされていないタイルよりも前に表示されます。

ポリシーを必須として設定した場合、'pinned' (ピン留めされた) フィールドは無視され、すべてのタイルがピン留めされます。ユーザーはタイルを削除できません。また、タイルは常にクイック リンク リストの先頭に表示されます。

このポリシーを推奨として設定した場合、ピン留めされたタイルはリストに残りますが、ユーザーはタイルを編集したり削除したりすることができます。ピン留めされていないクイック リンクのタイルは、既定のトップ サイトように動作し、他の Web サイトが頻繁にアクセスされるとこのタイルはリストから除外されます。ピン留めされていないリンクを、このポリシーを利用して既存のブラウザー プロファイルに適用すると、リンクのランクとユーザーの閲覧履歴との比較方法によっては、リンクが完全に表示されなくなる場合があります。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: はい
  - 動的ポリシーの更新: いいえ - ブラウザーの再起動が必要です

  #### データ型:
  辞書

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: NewTabPageManagedQuickLinks
  - GP の名前: 新しいタブ ページのクイック リンクを設定する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/スタートアップ、ホーム ページ、新しいタブ ページ
  - GP パス (おすすめ): 管理用テンプレート/Microsoft Edge - 既定の設定 (ユーザーはオーバーライドできます)/スタートアップ、ホーム ページ、新しいタブ ページ
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): SOFTWARE\Policies\Microsoft\Edge\おすすめ
  - 値の名前: NewTabPageManagedQuickLinks
  - 値の種類: REG_SZ
  ##### サンプル値:
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


  #### Mac の情報と設定
  - 優先されるキーの名前: NewTabPageManagedQuickLinks
  - サンプル値:
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
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### NewTabPageSetFeedType
  #### Microsoft Edge の新しいタブ ページ エクスペリエンスを構成する
  >サポートされているバージョン: Windows および Mac (バージョン 79 以降) の Microsoft Edge

  #### 説明
  新しいタブページに対して、Microsoft News または Office 365 のいずれかのフィード エクスペリエンスを選択できます。

このポリシーを Microsoft News フィード エクスペリエンスに設定すると (0)、新しいタブ ページに Microsoft News フィード エクスペリエンスが表示されます。

このポリシーを Office 365 フィード エクスペリエンスに設定すると (1)、ユーザーが Azure Active Directory ブラウザー サインインを使用している場合は、新しいタブ ページに Office 365 フィード エクスペリエンスが表示されます。

このポリシーを無効にした場合または構成しなかった場合:

- ユーザーが Azure Active Directory ブラウザー サインインを使用している場合は、Office 365 の新しいタブ ページ フィード エクスペリエンス、および標準の新しいタブ ページ フィード エクスペリエンスが提供されます。

- ユーザーが Azure Active Directory ブラウザー サインインを使用していない場合は、標準の新しいタブ ページ エクスペリエンスが表示されます。

このポリシー*および* [NewTabPageLocation](#newtabpagelocation) ポリシーを構成した場合は、[NewTabPageLocation](#newtabpagelocation) が優先されます。

既定の設定: 無効または未構成。

* 0 = Microsoft News フィード エクスペリエンス

* 1 = Office 365 フィード エクスペリエンス

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: はい
  - 動的ポリシーの更新: はい

  #### データ型:
  整数

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: NewTabPageSetFeedType
  - GP の名前: Microsoft Edge の新しいタブ ページ エクスペリエンスを構成する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/スタートアップ、ホーム ページ、新しいタブ ページ
  - GP パス (おすすめ): 管理用テンプレート/Microsoft Edge - 既定の設定 (ユーザーはオーバーライドできます)/スタートアップ、ホーム ページ、新しいタブ ページ
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): SOFTWARE\Policies\Microsoft\Edge\おすすめ
  - 値の名前: NewTabPageSetFeedType
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000000
```


  #### Mac の情報と設定
  - 優先されるキーの名前: NewTabPageSetFeedType
  - サンプル値:
``` xml
<integer>0</integer>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### RestoreOnStartup
  #### スタートアップ時に実行するアクション
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  Microsoft Edge の起動時の動作を指定します。

起動時に常に新しいタブを開く場合は、'新しいタブを開く' (5) を選択します。

前回 Microsoft Edge の終了時に開いていた URL をもう一度開く場合は、'前回のセッションを復元する' (1) を選択します。閲覧セッションが前回と同様に復元されます。このオプションによって、セッションに依存する設定や終了時にアクションを実行する設定 (終了時の閲覧データの消去やセッション専用 Cookie の消去) など、一部の設定が無効になることに注意してください。

URL の特定のセットを開く場合は、'URL のリストを開く' (4) を選択します。

この設定を無効にした場合、設定を構成していない状態と同じになり、ユーザーは、Microsoft Edge で設定を変更できます。

このポリシーは、Microsoft Active Directory ドメインに参加している Windows インスタンス、またはデバイス管理に登録されている Windows 10 Pro インスタンスや Windows 10 Enterprise インスタンスでのみ利用できます。

* 5 = 新しいタブを開く

* 1 = 前回のセッションを復元する

* 4 = URL のリストを開く

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: はい
  - 動的ポリシーの更新: はい

  #### データ型:
  整数

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: RestoreOnStartup
  - GP の名前: スタートアップ時に実行するアクション
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/スタートアップ、ホーム ページ、新しいタブ ページ
  - GP パス (おすすめ): 管理用テンプレート/Microsoft Edge - 既定の設定 (ユーザーはオーバーライドできます)/スタートアップ、ホーム ページ、新しいタブ ページ
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): SOFTWARE\Policies\Microsoft\Edge\おすすめ
  - 値の名前: RestoreOnStartup
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000004
```


  #### Mac の情報と設定
  - 優先されるキーの名前: RestoreOnStartup
  - サンプル値:
``` xml
<integer>4</integer>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### RestoreOnStartupURLs
  #### ブラウザーの起動時に開くサイト
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  ブラウザーの起動時に自動的に表示する Web サイトのリストを指定します。このポリシーを構成しなかった場合、起動時にサイトは表示されません。

このポリシーは、[RestoreOnStartup](#restoreonstartup) ポリシーを 'URL のリストを開く' (4) に設定している場合にのみ適用されます。

このポリシーは、Microsoft Active Directory ドメインに参加している Windows インスタンス、またはデバイス管理に登録されている Windows 10 Pro インスタンスや Windows 10 Enterprise インスタンスでのみ利用できます。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: はい
  - 動的ポリシーの更新: はい

  #### データ型:
  文字列の一覧

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: RestoreOnStartupURLs
  - GP の名前: ブラウザーの起動時に開くサイト
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/スタートアップ、ホーム ページ、新しいタブ ページ
  - GP パス (おすすめ): 管理用テンプレート/Microsoft Edge - 既定の設定 (ユーザーはオーバーライドできます)/スタートアップ、ホーム ページ、新しいタブ ページ
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge\RestoreOnStartupURLs
  - パス (おすすめ): SOFTWARE\Policies\Microsoft\Edge\おすすめ\RestoreOnStartupURLs
  - 値の名前: 1, 2, 3, ...
  - 値の種類: REG_SZ の一覧
  ##### サンプル値:
```
SOFTWARE\Policies\Microsoft\Edge\RestoreOnStartupURLs\0 = "https://contoso.com"
SOFTWARE\Policies\Microsoft\Edge\RestoreOnStartupURLs\1 = "https://www.fabrikam.com"

```


  #### Mac の情報と設定
  - 優先されるキーの名前: RestoreOnStartupURLs
  - サンプル値:
``` xml
<array>
  <string>https://contoso.com</string>
  <string>https://www.fabrikam.com</string>
</array>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### ShowHomeButton
  #### ツール バーに [ホーム] ボタンを表示する
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  Microsoft Edge のツール バーに [ホーム] ボタンを表示します。

このポリシーを有効にすると、[ホーム] ボタンが常に表示されます。このポリシーを無効にすると、ホーム ボタンは表示されません。

このポリシーを構成しなかった場合、ユーザーは [ホーム] ボタンを表示するかどうかを選択できます。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: はい
  - 動的ポリシーの更新: はい

  #### データ型:
  ブール値

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: ShowHomeButton
  - GP の名前: ツール バーに [ホーム] ボタンを表示する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/スタートアップ、ホーム ページ、新しいタブ ページ
  - GP パス (おすすめ): 管理用テンプレート/Microsoft Edge - 既定の設定 (ユーザーはオーバーライドできます)/スタートアップ、ホーム ページ、新しいタブ ページ
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): SOFTWARE\Policies\Microsoft\Edge\おすすめ
  - 値の名前: ShowHomeButton
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000001
```


  #### Mac の情報と設定
  - 優先されるキーの名前: ShowHomeButton
  - サンプル値:
``` xml
<true/>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ## ネイティブ メッセージング policies

  [トップに戻る](#microsoft-edge---ポリシー)

  ### NativeMessagingAllowlist
  #### ユーザーが使用できるネイティブ メッセージング ホストを制御する
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  ユーザーが Microsoft Edge で使用できる特定のネイティブ メッセージング ホストのリストを指定します。

既定では、すべてのネイティブ メッセージング ホストが許可されます。[NativeMessagingBlocklist](#nativemessagingblocklist) ポリシーを * に設定すると、すべてのネイティブ メッセージング ホストがブロックされ、ここで指定されたネイティブ メッセージング ホストのみが読み込まれます。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  文字列の一覧

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: NativeMessagingAllowlist
  - GP の名前: ユーザーが使用できるネイティブ メッセージング ホストを制御する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/ネイティブ メッセージング
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge\NativeMessagingAllowlist
  - パス (おすすめ): N/A
  - 値の名前: 1, 2, 3, ...
  - 値の種類: REG_SZ の一覧
  ##### サンプル値:
```
SOFTWARE\Policies\Microsoft\Edge\NativeMessagingAllowlist\0 = "com.native.messaging.host.name1"
SOFTWARE\Policies\Microsoft\Edge\NativeMessagingAllowlist\1 = "com.native.messaging.host.name2"

```


  #### Mac の情報と設定
  - 優先されるキーの名前: NativeMessagingAllowlist
  - サンプル値:
``` xml
<array>
  <string>com.native.messaging.host.name1</string>
  <string>com.native.messaging.host.name2</string>
</array>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### NativeMessagingBlocklist
  #### ネイティブ メッセージングの禁止リストを構成する
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  使用を禁止するネイティブ メッセージング ホストを指定します。

ネイティブ メッセージング ホストが明示的に許可リストに登録されていない場合は、'*' を使用して、すべてのネイティブ メッセージング ホストをブロックできます。

このポリシーを構成しなかった場合、Microsoft Edge では、インストールされているすべてのネイティブ メッセージング ホストが読み込まれます。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  文字列の一覧

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: NativeMessagingBlocklist
  - GP の名前: ネイティブ メッセージングの禁止リストを構成する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/ネイティブ メッセージング
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge\NativeMessagingBlocklist
  - パス (おすすめ): N/A
  - 値の名前: 1, 2, 3, ...
  - 値の種類: REG_SZ の一覧
  ##### サンプル値:
```
SOFTWARE\Policies\Microsoft\Edge\NativeMessagingBlocklist\0 = "com.native.messaging.host.name1"
SOFTWARE\Policies\Microsoft\Edge\NativeMessagingBlocklist\1 = "com.native.messaging.host.name2"

```


  #### Mac の情報と設定
  - 優先されるキーの名前: NativeMessagingBlocklist
  - サンプル値:
``` xml
<array>
  <string>com.native.messaging.host.name1</string>
  <string>com.native.messaging.host.name2</string>
</array>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### NativeMessagingUserLevelHosts
  #### ユーザー レベルのネイティブ メッセージング ホスト (管理者のアクセス許可なしでインストールされるホスト) を許可する
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  ネイティブ メッセージング ホストのユーザー レベルのインストールを有効にします。

このポリシーを無効にした場合、Microsoft Edge では、システム レベルでインストールされたネイティブ メッセージング ホストのみが使用されます。

このポリシーを構成しなかった場合、Microsoft Edge では、既定でユーザー レベルのネイティブ メッセージング ホストを使用できます。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  ブール値

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: NativeMessagingUserLevelHosts
  - GP の名前: ユーザー レベルのネイティブ メッセージング ホスト (管理者のアクセス許可なしでインストールされるホスト) を許可する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/ネイティブ メッセージング
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: NativeMessagingUserLevelHosts
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000000
```


  #### Mac の情報と設定
  - 優先されるキーの名前: NativeMessagingUserLevelHosts
  - サンプル値:
``` xml
<false/>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ## パスワード マネージャーと保護 policies

  [トップに戻る](#microsoft-edge---ポリシー)

  ### PasswordManagerEnabled
  #### パスワード マネージャーへのパスワードの保存を有効にする
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  Microsoft Edge を有効にして、ユーザーのパスワードを保存します。

このポリシーを有効にすると、ユーザーは Microsoft Edge でパスワードを保存できます。次回サイトにアクセスしたときに、Microsoft Edge でパスワードが自動的に入力されます。

このポリシーを無効にした場合、ユーザーは新しいパスワードを保存できませんが、前回保存したパスワードを使用することができます。

このポリシーを有効または無効にした場合、ユーザーは Microsoft Edge でこの設定を変更または上書きすることはできません。このポリシーを構成しなかった場合は、ユーザーはパスワードを保存することができ、この機能をオフにすることもできます。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: はい
  - 動的ポリシーの更新: はい

  #### データ型:
  ブール値

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: PasswordManagerEnabled
  - GP の名前: パスワード マネージャーへのパスワードの保存を有効にする
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/パスワード マネージャーと保護
  - GP パス (おすすめ): 管理用テンプレート/Microsoft Edge - 既定の設定 (ユーザーはオーバーライドできます)/パスワード マネージャーと保護
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): SOFTWARE\Policies\Microsoft\Edge\おすすめ
  - 値の名前: PasswordManagerEnabled
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000001
```


  #### Mac の情報と設定
  - 優先されるキーの名前: PasswordManagerEnabled
  - サンプル値:
``` xml
<true/>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### PasswordProtectionChangePasswordURL
  #### パスワード変更 URL を構成する
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  パスワード変更 URL (HTTP スキームと HTTPS スキームのみ) を構成します。

パスワード保護サービスは、ブラウザーで警告が表示された後、パスワードを変更するためにユーザーをこの URL にアクセスさせます。

このポリシーを有効にした場合、パスワード保護サービスは、パスワードを変更するためにユーザーをこの URL にアクセスさせます。

このポリシーを無効にした場合または構成しなかった場合、パスワード保護サービスは、パスワード変更 URL にユーザーをリダイレクトしません。

このポリシーは、Microsoft Active Directory ドメインに参加している Windows インスタンス、またはデバイス管理に登録されている Windows 10 Pro インスタンスや Windows 10 Enterprise インスタンスでのみ利用できます。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  文字列

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: PasswordProtectionChangePasswordURL
  - GP の名前: パスワード変更 URL を構成する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/パスワード マネージャーと保護
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: PasswordProtectionChangePasswordURL
  - 値の種類: REG_SZ
  ##### サンプル値:
```
"https://contoso.com/change_password.html"
```


  #### Mac の情報と設定
  - 優先されるキーの名前: PasswordProtectionChangePasswordURL
  - サンプル値:
``` xml
<string>https://contoso.com/change_password.html</string>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### PasswordProtectionLoginURLs
  #### パスワード保護サービスによってパスワードとしての指紋がキャプチャされるエンタープライズ ログイン URL のリストを構成する
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  エンタープライズ ログイン URL (HTTP スキームと HTTPS スキームのみ) のリストを構成します。この URL では、Microsoft Edge によって、パスワードとしての指紋がキャプチャされ、パスワード再利用の検出を行う際に使用されます。

このポリシーを有効にした場合、パスワード保護サービスによって、既定の URL でパスワードとしての指紋がキャプチャされます。

このポリシーを無効にした場合または構成しなかった場合、パスワードとしての指紋はキャプチャされません。

このポリシーは、Microsoft Active Directory ドメインに参加している Windows インスタンス、またはデバイス管理に登録されている Windows 10 Pro インスタンスや Windows 10 Enterprise インスタンスでのみ利用できます。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  文字列の一覧

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: PasswordProtectionLoginURLs
  - GP の名前: パスワード保護サービスによってパスワードとしての指紋がキャプチャされるエンタープライズ ログイン URL のリストを構成する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/パスワード マネージャーと保護
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge\PasswordProtectionLoginURLs
  - パス (おすすめ): N/A
  - 値の名前: 1, 2, 3, ...
  - 値の種類: REG_SZ の一覧
  ##### サンプル値:
```
SOFTWARE\Policies\Microsoft\Edge\PasswordProtectionLoginURLs\0 = "https://contoso.com/login.html"
SOFTWARE\Policies\Microsoft\Edge\PasswordProtectionLoginURLs\1 = "https://login.contoso.com"

```


  #### Mac の情報と設定
  - 優先されるキーの名前: PasswordProtectionLoginURLs
  - サンプル値:
``` xml
<array>
  <string>https://contoso.com/login.html</string>
  <string>https://login.contoso.com</string>
</array>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### PasswordProtectionWarningTrigger
  #### パスワード保護の警告トリガーを構成する
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  パスワード保護の警告をトリガーするタイミングを制御できます。パスワード保護は、ユーザーが保護されたパスワードを不審な可能性があるサイトで再利用するときに、ユーザーに警告します。

保護するパスワードを構成するには、[PasswordProtectionLoginURLs](#passwordprotectionloginurls) ポリシーと [PasswordProtectionChangePasswordURL](#passwordprotectionchangepasswordurl) ポリシーを使用できます。

例外: [PasswordProtectionLoginURLs](#passwordprotectionloginurls) ポリシーと [PasswordProtectionChangePasswordURL](#passwordprotectionchangepasswordurl) ポリシーで指定されているサイト、および [SmartScreenAllowListDomains](#smartscreenallowlistdomains) ポリシーで指定されているサイトのパスワードは、パスワード保護の警告をトリガーしません。

'PasswordProtectionWarningOff' (0) に設定すると、パスワード保護の警告は表示されません。

'PasswordProtectionWarningOnPasswordReuse' (1) に設定すると、ホワイトリストに登録されていないサイトでユーザーがパスワードを再利用するときに、パスワード保護の警告が表示されます。

このポリシーを無効にした場合または構成しなかった場合、警告トリガーは表示されません。

* 0 = パスワード保護の警告は無効です。

* 1 = パスワードを再利用すると、パスワード保護の警告がトリガーされます。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  整数

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: PasswordProtectionWarningTrigger
  - GP の名前: パスワード保護の警告トリガーを構成する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/パスワード マネージャーと保護
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: PasswordProtectionWarningTrigger
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000001
```


  #### Mac の情報と設定
  - 優先されるキーの名前: PasswordProtectionWarningTrigger
  - サンプル値:
``` xml
<integer>1</integer>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ## プロキシ サーバー policies

  [トップに戻る](#microsoft-edge---ポリシー)

  ### ProxyBypassList
  #### プロキシバイパスの規則を構成する
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  Microsoft Edge がプロキシをバイパスするホストのリストを定義します。

このポリシーが適用されるのは、[ProxyMode](#proxymode) ポリシーで '固定プロキシ サーバーを使用する' を選択した場合のみです。プロキシ ポリシーの構成で他のモードを選択した場合は、このポリシーを有効にしたり、構成したりしないでください。

このポリシーを有効にした場合、Microsoft Edge がプロキシを使用しないホストのリストを作成できます。

このポリシーを構成しなかった場合、Microsoft Edge がプロキシをバイパスするホストのリストは作成されません。プロキシ ポリシーの設定で他の方法を指定した場合は、このポリシーを構成しないでください。

詳細な例については、[https://go.microsoft.com/fwlink/?linkid=2094936](https://go.microsoft.com/fwlink/?linkid=2094936) を参照してください。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  文字列

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: ProxyBypassList
  - GP の名前: プロキシバイパスの規則を構成する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/プロキシ サーバー
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: ProxyBypassList
  - 値の種類: REG_SZ
  ##### サンプル値:
```
"https://www.contoso.com, https://www.fabrikam.com"
```


  #### Mac の情報と設定
  - 優先されるキーの名前: ProxyBypassList
  - サンプル値:
``` xml
<string>https://www.contoso.com, https://www.fabrikam.com</string>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### ProxyMode
  #### プロキシ サーバーの設定を構成する
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  Microsoft Edge で使用されるプロキシ サーバーの設定を指定します。このポリシーを有効にした場合、ユーザーはプロキシ設定を変更できなくなります。

プロキシ サーバーを使用せず、常に直接接続することを選択すると、他のすべてのオプションは無視されます。

システム プロキシ設定を使用すると、他のすべてのオプションは無視されます。

プロキシ サーバーの自動検出を選択すると、他のすべてのオプションは無視されます。

固定サーバー プロキシ モードを選択すると、[ProxyServer](#proxyserver) や 'プロキシ バイパス規則のカンマ区切りのリスト' で追加のオプションを指定できます。

.pac プロキシ スクリプトの使用を選択すると、'プロキシ .pac ファイルの URL' でスクリプトへの URL を指定する必要があります。

詳細な例については、[https://go.microsoft.com/fwlink/?linkid=2094936](https://go.microsoft.com/fwlink/?linkid=2094936) を参照してください。

このポリシーを有効にした場合、Microsoft Edge では、コマンド ラインから指定したプロキシ関連のすべてのオプションが無視されます。

このポリシーを構成しなかった場合、ユーザーは独自のプロキシ設定を選択できます。

* "direct" = プロキシを使用しない

* "auto_detect" = プロキシ設定を自動検出する

* "pac_script" = .pac プロキシ スクリプトを使用する

* "fixed_servers" = 固定プロキシ サーバーを使用する

* "system" = システム プロキシ設定を使用する

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  文字列

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: ProxyMode
  - GP の名前: プロキシ サーバーの設定を構成する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/プロキシ サーバー
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: ProxyMode
  - 値の種類: REG_SZ
  ##### サンプル値:
```
"direct"
```


  #### Mac の情報と設定
  - 優先されるキーの名前: ProxyMode
  - サンプル値:
``` xml
<string>direct</string>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### ProxyPacUrl
  #### プロキシ .pac ファイルの URL を設定する
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  プロキシ自動構成 (PAC) ファイルの URL を指定します

このポリシーが適用されるのは、[ProxyMode](#proxymode) ポリシーで '.pac プロキシ スクリプトを使用する' を選択した場合のみです。プロキシ ポリシーの構成で他のモードを選択した場合は、このポリシーを有効にしたり、構成したりしないでください。

このポリシーを有効にした場合、PAC ファイルの URL を指定できます。このファイルでは、特定の Web サイトを取得するための適切なプロキシ サーバーをブラウザーで自動的に選択する方法が定義されています。

このポリシーを無効にした場合または構成しなかった場合、PAC ファイルは指定されません。プロキシ ポリシーの設定で他の方法を指定した場合は、このポリシーを構成しないでください。

詳細な例については、[https://go.microsoft.com/fwlink/?linkid=2094936](https://go.microsoft.com/fwlink/?linkid=2094936) を参照してください。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  文字列

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: ProxyPacUrl
  - GP の名前: プロキシ .pac ファイルの URL を設定する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/プロキシ サーバー
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: ProxyPacUrl
  - 値の種類: REG_SZ
  ##### サンプル値:
```
"https://internal.contoso.com/example.pac"
```


  #### Mac の情報と設定
  - 優先されるキーの名前: ProxyPacUrl
  - サンプル値:
``` xml
<string>https://internal.contoso.com/example.pac</string>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### ProxyServer
  #### プロキシ サーバーのアドレスまたは URL を構成する
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  プロキシ サーバーの URL を指定します。

このポリシーが適用されるのは、[ProxyMode](#proxymode) ポリシーで '固定プロキシ サーバーを使用する' を選択した場合のみです。プロキシ ポリシーの構成で他のモードを選択した場合は、このポリシーを有効にしたり、構成したりしないでください。

このポリシーを有効にした場合、このポリシーによって構成されるプロキシ サーバーが、すべての URL に対して使用されます。

このポリシーを無効にした場合または構成しなかった場合、このプロキシ モード (固定プロキシ サーバーを使用する) のときに、ユーザーは独自のプロキシ設定を選択できます。プロキシ ポリシーの設定で他の方法を指定した場合は、このポリシーを構成しないでください。

その他のオプションや詳細な例については、[https://go.microsoft.com/fwlink/?linkid=2094936](https://go.microsoft.com/fwlink/?linkid=2094936) を参照してください。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  文字列

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: ProxyServer
  - GP の名前: プロキシ サーバーのアドレスまたは URL を構成する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/プロキシ サーバー
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: ProxyServer
  - 値の種類: REG_SZ
  ##### サンプル値:
```
"123.123.123.123:8080"
```


  #### Mac の情報と設定
  - 優先されるキーの名前: ProxyServer
  - サンプル値:
``` xml
<string>123.123.123.123:8080</string>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### ProxySettings
  #### プロキシの設定
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  Microsoft Edge のプロキシ設定を構成します。

このポリシーを有効にした場合、Microsoft Edge では、コマンド ラインから指定したプロキシ関連のオプションがすべて無視されます。

このポリシーを設定しなかった場合、ユーザーは独自のプロキシ設定を選択できます。

このポリシーは、以下の各ポリシーをオーバーライドします。

[ProxyMode](#proxymode)
[ProxyPacUrl](#proxypacurl)
[ProxyServer](#proxyserver)
[ProxyBypassList](#proxybypasslist)

ProxyMode フィールドでは、Microsoft Edge で使用されるプロキシ サーバーを指定でき、ユーザーがプロキシ設定を変更できないようにします。

ProxyPacUrl フィールドには、プロキシ .pac ファイルへの URL を指定します。

ProxyServer フィールドには、プロキシ サーバーの URL を指定します。

ProxyBypassList フィールドには、Microsoft Edge がバイパスするプロキシ ホストのリストを指定します。

'ProxyMode' の値として 'direct' を選択した場合、プロキシは使用されず、他のフィールドはすべて無視されます。

'ProxyMode' の値として 'system' を選択した場合、システムのプロキシが使用され、他のフィールドはすべて無視されます。

'ProxyMode' の値として 'auto_detect' を選択した場合、他のフィールドはすべて無視されます。

'ProxyMode' の値として 'fixed_server' を選択した場合、'ProxyServer' フィールドと 'ProxyBypassList' フィールドが使用されます。

'ProxyMode' の値として 'pac_script' を選択した場合、'ProxyPacUrl' フィールドと 'ProxyBypassList' フィールドが使用されます。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  辞書

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: ProxySettings
  - GP の名前: プロキシの設定
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/プロキシ サーバー
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: ProxySettings
  - 値の種類: REG_SZ
  ##### サンプル値:
```
SOFTWARE\Policies\Microsoft\Edge\ProxySettings = {
  "ProxyBypassList": "https://www.example1.com,https://www.example2.com,https://internalsite/", 
  "ProxyMode": "direct", 
  "ProxyPacUrl": "https://internal.site/example.pac", 
  "ProxyServer": "123.123.123.123:8080"
}
```


  #### Mac の情報と設定
  - 優先されるキーの名前: ProxySettings
  - サンプル値:
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
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ## 印刷 policies

  [トップに戻る](#microsoft-edge---ポリシー)

  ### DefaultPrinterSelection
  #### 既定のプリンターの選択規則
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  Microsoft Edge で通常使うプリンター選択規則よりも優先されます。このポリシーでは、ユーザーが初めてページを印刷しようとしたときに、Microsoft Edge で通常使うプリンターを選択するための規則を決定します。

このポリシーが構成されている場合、Microsoft Edge では、指定されたすべての属性に一致するプリンターの検索を試行し、そのプリンターを通常使うプリンターとして使用します。条件を満たすプリンターが複数ある場合は、最初に一致したプリンターが使用されます。

このポリシーを構成しない場合、またはタイムアウト期間内に一致するプリンターが見つからなかった場合は、既定のプリンターは組み込み PDF プリンターとなりますが、PDF プリンターが利用できない場合はプリンターなしになります。

この値は JSON オブジェクトとして解析され、次のスキーマに準拠します。{ "type": "object", "properties": { "idPattern": { "description": "Regular expression to match printer id.", "type": "string" }, "namePattern": { "description": "Regular expression to match printer display name.", "type": "string" } } }

フィールドを省略すると、すべての値が一致することになります。たとえば、接続を指定しない場合、印刷プレビューではすべての種類のローカル プリンターの検出を開始します。正規表現パターンは JavaScript RegExp 構文に従う必要があります。また、一致では大文字と小文字が区別されます。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  文字列

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: DefaultPrinterSelection
  - GP の名前: 既定のプリンターの選択規則
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/印刷
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: DefaultPrinterSelection
  - 値の種類: REG_SZ
  ##### サンプル値:
```
"{ "idPattern": ".*public", "namePattern": ".*Color" }"
```


  #### Mac の情報と設定
  - 優先されるキーの名前: DefaultPrinterSelection
  - サンプル値:
``` xml
<string>{ "idPattern": ".*public", "namePattern": ".*Color" }</string>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### PrintHeaderFooter
  #### ヘッダーとフッターを印刷する
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  [印刷] ダイアログボックスで「ヘッダーとフッター」の入力をオンまたはオフにします。

このポリシーを構成しない場合は、ユーザーはヘッダーとフッターを印刷するかどうかを選択できます。

このポリシーを無効にした場合、ユーザーはヘッダーとフッターを印刷できません。

このポリシーを有効にした場合、ユーザーは常にヘッダーとフッターを印刷します。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: はい
  - 動的ポリシーの更新: はい

  #### データ型:
  ブール値

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: PrintHeaderFooter
  - GP の名前: ヘッダーとフッターを印刷する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/印刷
  - GP パス (おすすめ): 管理用テンプレート/Microsoft Edge - 既定の設定 (ユーザーはオーバーライドできます)/印刷
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): SOFTWARE\Policies\Microsoft\Edge\おすすめ
  - 値の名前: PrintHeaderFooter
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000000
```


  #### Mac の情報と設定
  - 優先されるキーの名前: PrintHeaderFooter
  - サンプル値:
``` xml
<false/>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### PrintPreviewUseSystemDefaultPrinter
  #### システム既定のプリンターを通常使用するプリンターとして設定する
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  Microsoft Edge に対して、[印刷プレビュー] で既定で選択されるプリンターとして、最近使用したプリンターではなく、システムの既定のプリンターを使用するように指示します。

このポリシーを無効にした場合または構成しなかった場合、[印刷プレビュー] では、最近使用したプリンターが既定の出力先として使用されます。

このポリシーを有効にした場合、[印刷プレビュー] では、OS のシステム既定のプリンターが既定の出力先として使用されます。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: はい
  - 動的ポリシーの更新: はい

  #### データ型:
  ブール値

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: PrintPreviewUseSystemDefaultPrinter
  - GP の名前: システム既定のプリンターを通常使用するプリンターとして設定する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/印刷
  - GP パス (おすすめ): 管理用テンプレート/Microsoft Edge - 既定の設定 (ユーザーはオーバーライドできます)/印刷
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): SOFTWARE\Policies\Microsoft\Edge\おすすめ
  - 値の名前: PrintPreviewUseSystemDefaultPrinter
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000000
```


  #### Mac の情報と設定
  - 優先されるキーの名前: PrintPreviewUseSystemDefaultPrinter
  - サンプル値:
``` xml
<false/>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### PrintingEnabled
  #### 印刷を有効にする
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  Microsoft Edge での印刷を有効にして、ユーザーがこの設定を変更できないようにします。

このポリシーを有効にした場合または構成しなかった場合、ユーザーは印刷することができます。

このポリシーを無効にした場合、ユーザーは Microsoft Edge から印刷できません。レンチ メニュー、拡張機能、JavaScript アプリケーションなどで印刷が無効になります。ただし、ユーザーは、印刷中に Microsoft Edge をバイパスするプラグインから印刷することができます。たとえば、Adobe Flash の一部のアプリケーションでは、コンテキスト メニューにこのポリシーが適用されない印刷オプションがあります。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  ブール値

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: PrintingEnabled
  - GP の名前: 印刷を有効にする
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/印刷
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: PrintingEnabled
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000001
```


  #### Mac の情報と設定
  - 優先されるキーの名前: PrintingEnabled
  - サンプル値:
``` xml
<true/>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### UseSystemPrintDialog
  #### システム印刷ダイアログを使用して印刷する
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  印刷プレビューの代わりにシステムの印刷ダイアログを表示します。

このポリシーを有効にした場合、ユーザーがページを印刷するとき、Microsoft Edge では組み込みの印刷プレビューではなくシステムの印刷ダイアログを開きます。

このポリシーを構成しなかった場合または無効にした場合、印刷コマンドによって、Microsoft Edge の印刷プレビュー画面がトリガーされます。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: いいえ - ブラウザーの再起動が必要です

  #### データ型:
  ブール値

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: UseSystemPrintDialog
  - GP の名前: システム印刷ダイアログを使用して印刷する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/印刷
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: UseSystemPrintDialog
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000000
```


  #### Mac の情報と設定
  - 優先されるキーの名前: UseSystemPrintDialog
  - サンプル値:
``` xml
<false/>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ## 拡張機能 policies

  [トップに戻る](#microsoft-edge---ポリシー)

  ### ExtensionAllowedTypes
  #### 許可される拡張機能の種類を構成する
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  インストールできる拡張機能の種類を制御し、ランタイム アクセスを制限します。

この設定では、許可される拡張機能の種類と、拡張機能とのやり取りができるホストを定義します。値は文字列のリストとして指定します。これらの文字列は、"extension"、"theme"、"user_script"、"hosted_app" のいずれかになります。これらの種類について詳しくは、Microsoft Edge の拡張機能に関するドキュメントをご覧ください。

このポリシーは、[ExtensionInstallForcelist](#extensioninstallforcelist) ポリシーを使用して強制的にインストールされる拡張機能にも影響します。

このポリシーを有効にした場合、リスト内の種類に一致する拡張機能のみがインストールされます。

このポリシーを構成しなかった場合、許可される拡張機能の種類に関する制限は適用されません。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  文字列の一覧

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: ExtensionAllowedTypes
  - GP の名前: 許可される拡張機能の種類を構成する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/拡張機能
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge\ExtensionAllowedTypes
  - パス (おすすめ): N/A
  - 値の名前: 1, 2, 3, ...
  - 値の種類: REG_SZ の一覧
  ##### サンプル値:
```
SOFTWARE\Policies\Microsoft\Edge\ExtensionAllowedTypes\0 = "hosted_app"

```


  #### Mac の情報と設定
  - 優先されるキーの名前: ExtensionAllowedTypes
  - サンプル値:
``` xml
<array>
  <string>hosted_app</string>
</array>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### ExtensionInstallAllowlist
  #### 特定の拡張機能のインストールを許可する
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  既定では、すべての拡張機能が許可されます。ただし、'ExtensionInstallBlockList' ポリシーを "*" に設定してすべての拡張機能をブロックすると、ユーザーがインストールできるのは、このポリシーに定義されている拡張機能のみになります。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  文字列の一覧

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: ExtensionInstallAllowlist
  - GP の名前: 特定の拡張機能のインストールを許可する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/拡張機能
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallAllowlist
  - パス (おすすめ): N/A
  - 値の名前: 1, 2, 3, ...
  - 値の種類: REG_SZ の一覧
  ##### サンプル値:
```
SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallAllowlist\0 = "extension_id1"
SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallAllowlist\1 = "extension_id2"

```


  #### Mac の情報と設定
  - 優先されるキーの名前: ExtensionInstallAllowlist
  - サンプル値:
``` xml
<array>
  <string>extension_id1</string>
  <string>extension_id2</string>
</array>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### ExtensionInstallBlocklist
  #### インストールできない拡張機能を制御する
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  ユーザーが Microsoft Edge でインストールできない特定の拡張子を一覧表示します。このポリシーを導入すると、この一覧にある拡張子で既にインストールされているものはすべて無効になり、ユーザーは再度有効にすることができません。ブロックする拡張子の一覧からアイテムを削除すると、その拡張子は以前インストールされた場所で自動的に再度有効になります。

許可リストに明示的に指定されていないすべての拡張子をブロックするには、「*」を使用します。

このポリシーを設定しない場合、ユーザーは Microsoft Edge で任意の拡張子をインストールできます。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  文字列の一覧

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: ExtensionInstallBlocklist
  - GP の名前: インストールできない拡張機能を制御する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/拡張機能
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallBlocklist
  - パス (おすすめ): N/A
  - 値の名前: 1, 2, 3, ...
  - 値の種類: REG_SZ の一覧
  ##### サンプル値:
```
SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallBlocklist\0 = "extension_id1"
SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallBlocklist\1 = "extension_id2"

```


  #### Mac の情報と設定
  - 優先されるキーの名前: ExtensionInstallBlocklist
  - サンプル値:
``` xml
<array>
  <string>extension_id1</string>
  <string>extension_id2</string>
</array>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### ExtensionInstallForcelist
  #### サイレント インストールされる拡張機能を制御する
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  ユーザーによる操作なしでサイレント インストールされる拡張機能を指定します。ユーザーは、これらの拡張機能をアンインストールしたり、無効にしたりすることはできません ("強制インストール")。拡張機能によって要求されるすべてのアクセス許可は、ユーザーが操作することなく暗黙的に付与されます。拡張機能の将来のバージョンによって要求される追加のアクセス許可も対象となります。また、アクセス許可は、enterprise.deviceAttributes 拡張機能 API や enterprise.platformKeys 拡張機能 API に対しても付与されます (これら 2 つの API は強制的にインストールされる拡張機能でのみ利用できます)。

このポリシーは、競合する可能性のある [ExtensionInstallBlocklist](#extensioninstallblocklist) ポリシーよりも優先されます。強制的にインストールされるリストから拡張機能を削除すると、その拡張機能は、Microsoft Edge によって自動的にアンインストールされます。

Microsoft Active Directory ドメインに参加していない Windows デバイスの場合、強制インストールは、Microsoft Store で提供されている拡張機能に限定されます。

ただし、ユーザーは開発者ツールを使用することで、どの拡張機能に対してもソース コードを変更できます (その場合、拡張機能が機能しなくなることがあります)。このようなユーザーによる変更を禁止する場合は、[DeveloperToolsAvailability](#developertoolsavailability) ポリシーを設定してください。

以下の形式で拡張機能をリストに追加してください:

[extensionID];[updateURL]

- extensionID は 32 文字の文字列です。デベロッパー モード で edge://extensions を開くと確認できます。

- updateURL (省略可能) は、アプリや拡張機能の更新マニフェスト XML ドキュメントのアドレスです。[https://go.microsoft.com/fwlink/?linkid=2095043](https://go.microsoft.com/fwlink/?linkid=2095043) の説明をご覧ください。updateURL を設定しなかった場合、Microsoft Store の更新 URL が使用されます (現在は、https://edge.microsoft.com/extensionwebstorebase/v1/crx)。このポリシーで設定された更新 URL は、初回のインストールでのみ使用され、その後の拡張機能の更新では、拡張機能のマニフェストで指定されている更新 URL が使用されます。

たとえば、gggmmkjegpiggikcnhidnjjhmicpibll;https://edge.microsoft.com/extensionwebstorebase/v1/crx では、Microsoft Store の "更新" URL から Microsoft Online アプリがインストールされます。拡張機能のホスティングについて詳しくは、[https://go.microsoft.com/fwlink/?linkid=2095044](https://go.microsoft.com/fwlink/?linkid=2095044) を参照してください。

このポリシーを構成しなかった場合、拡張機能は自動的にはインストールされず、ユーザーは Microsoft Edge のどの拡張機能でもアンインストールできます。

このポリシーは InPrivate モードには適用されないことに注意してください。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  文字列の一覧

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: ExtensionInstallForcelist
  - GP の名前: サイレント インストールされる拡張機能を制御する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/拡張機能
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallForcelist
  - パス (おすすめ): N/A
  - 値の名前: 1, 2, 3, ...
  - 値の種類: REG_SZ の一覧
  ##### サンプル値:
```
SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallForcelist\0 = "gbchcmhmhahfdphkhkmpfmihenigjmpp;https://edge.microsoft.com/extensionwebstorebase/v1/crx"
SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallForcelist\1 = "abcdefghijklmnopabcdefghijklmnop"

```


  #### Mac の情報と設定
  - 優先されるキーの名前: ExtensionInstallForcelist
  - サンプル値:
``` xml
<array>
  <string>gbchcmhmhahfdphkhkmpfmihenigjmpp;https://edge.microsoft.com/extensionwebstorebase/v1/crx</string>
  <string>abcdefghijklmnopabcdefghijklmnop</string>
</array>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### ExtensionInstallSources
  #### 拡張機能およびユーザー スクリプトのインストール ソースを構成する
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  拡張機能やテーマをインストールできる URL を定義します。

既定では、ユーザーはインストールする拡張機能やスクリプトそれぞれに対応した *.crx ファイルをダウンロードし、そのファイルを Microsoft Edge の設定ページにドラッグする必要があります。このポリシーでは、特定の URL を使用して、ユーザーに必要な拡張機能やスクリプトをインストールできるようにします。

このリストの各項目は、拡張機能スタイルの一致パターンに従っています ([https://go.microsoft.com/fwlink/?linkid=2095039](https://go.microsoft.com/fwlink/?linkid=2095039) を参照してください)。ユーザーは、このリストの項目に一致するどの URL からでも、アイテムを簡単にインストールできます。*.crx ファイルの場所およびダウンロードが開始されるページ (つまり、参照元) はどちらも、これらもパターンに基づいて許可されます。

[ExtensionInstallBlocklist](#extensioninstallblocklist) ポリシーは、このポリシーよりも優先されます。禁止リストで指定されている拡張機能は、このリストにあるサイトからの拡張機能であってもインストールされません。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  文字列の一覧

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: ExtensionInstallSources
  - GP の名前: 拡張機能およびユーザー スクリプトのインストール ソースを構成する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/拡張機能
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallSources
  - パス (おすすめ): N/A
  - 値の名前: 1, 2, 3, ...
  - 値の種類: REG_SZ の一覧
  ##### サンプル値:
```
SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallSources\0 = "https://corp.contoso.com/*"

```


  #### Mac の情報と設定
  - 優先されるキーの名前: ExtensionInstallSources
  - サンプル値:
``` xml
<array>
  <string>https://corp.contoso.com/*</string>
</array>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### ExtensionSettings
  #### 拡張子の管理設定を構成する
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  Microsoft Edge の拡張機能の管理設定を構成します。

このポリシーでは、拡張機能に関連する既存のポリシーで管理されている設定を含む、複数の設定を管理します。このポリシーとレガシ ポリシーの両方が設定されている場合は、このポリシーが優先されます。

このポリシーでは、拡張機能 ID または更新 URL をそれぞれの構成にマップします。拡張機能 ID を使用する場合、構成は特定の拡張機能にのみ適用されます。特別な ID "*" に対して既定の構成を設定すると、既定の構成が、このポリシーに明示されていないすべての拡張機能に適用されます。更新 URL を使用する場合、[https://go.microsoft.com/fwlink/?linkid=2095043](https://go.microsoft.com/fwlink/?linkid=2095043) で説明されているように、構成はこの拡張機能のマニフェストに示されている更新 URL を使用するすべての拡張機能に適用されます。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  辞書

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: ExtensionSettings
  - GP の名前: 拡張子の管理設定を構成する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/拡張機能
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: ExtensionSettings
  - 値の種類: REG_SZ
  ##### サンプル値:
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


  #### Mac の情報と設定
  - 優先されるキーの名前: ExtensionSettings
  - サンプル値:
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
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ## 既定の検索プロバイダー policies

  [トップに戻る](#microsoft-edge---ポリシー)

  ### DefaultSearchProviderEnabled
  #### 既定の検索プロバイダーを有効にする
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  既定の検索プロバイダーの使用を有効にします。

このポリシーを有効にした場合、ユーザーは、(入力する内容が URL でないかぎり) 用語をアドレス バーに入力して検索できます。

既定の検索ポリシーの残りの部分を有効にすることで、使用する既定の検索プロバイダーを指定できます。これらが空のまま (構成されていない場合)、ユーザーは既定のプロバイダーを選択できます。

このポリシーを無効にした場合、ユーザーはアドレス バーから検索できません。

このポリシーを有効または無効にした場合、ユーザーはこのポリシーを変更したり、上書きしたりすることはできません。

このポリシーを構成しなかった場合、既定の検索プロバイダーが有効になり、ユーザーは既定の検索プロバイダーを選択して、検索プロバイダーの一覧を設定できます。

このポリシーは、Microsoft Active Directory ドメインに参加している Windows インスタンス、または、デバイス管理用に登録されている Windows 10 Pro またはエンタープライズのインスタンスでのみ使用できます。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  ブール値

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: DefaultSearchProviderEnabled
  - GP の名前: 既定の検索プロバイダーを有効にする
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/既定の検索プロバイダー
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: DefaultSearchProviderEnabled
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000001
```


  #### Mac の情報と設定
  - 優先されるキーの名前: DefaultSearchProviderEnabled
  - サンプル値:
``` xml
<true/>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### DefaultSearchProviderEncodings
  #### 既定の検索プロバイダーのエンコード
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  検索プロバイダーでサポートされる文字エンコードを指定します。エンコードは、UTF-8、GB2312、ISO-8859-1 などのコード ページ名になります。これらは、指定された順序で適用が試行されます。

このポリシーは省略可能です。このポリシーを構成しなかった場合、既定では UTF-8 が使用されます。

このポリシーは、[DefaultSearchProviderEnabled](#defaultsearchproviderenabled) ポリシーと [DefaultSearchProviderSearchURL](#defaultsearchprovidersearchurl) ポリシーを有効にした場合にのみ適用されます。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  文字列の一覧

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: DefaultSearchProviderEncodings
  - GP の名前: 既定の検索プロバイダーのエンコード
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/既定の検索プロバイダー
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge\DefaultSearchProviderEncodings
  - パス (おすすめ): N/A
  - 値の名前: 1, 2, 3, ...
  - 値の種類: REG_SZ の一覧
  ##### サンプル値:
```
SOFTWARE\Policies\Microsoft\Edge\DefaultSearchProviderEncodings\0 = "UTF-8"
SOFTWARE\Policies\Microsoft\Edge\DefaultSearchProviderEncodings\1 = "UTF-16"
SOFTWARE\Policies\Microsoft\Edge\DefaultSearchProviderEncodings\2 = "GB2312"
SOFTWARE\Policies\Microsoft\Edge\DefaultSearchProviderEncodings\3 = "ISO-8859-1"

```


  #### Mac の情報と設定
  - 優先されるキーの名前: DefaultSearchProviderEncodings
  - サンプル値:
``` xml
<array>
  <string>UTF-8</string>
  <string>UTF-16</string>
  <string>GB2312</string>
  <string>ISO-8859-1</string>
</array>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### DefaultSearchProviderImageURL
  #### 既定の検索プロバイダーの画像検索を指定する
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  画像検索に使用する検索エンジンの URL を指定します。検索要求は GET メソッドを使用して送信されます。

このポリシーは省略可能です。このポリシーを構成しなかった場合、画像検索を利用することはできません。

Bing の画像検索 URL は次のように指定します:
'{bing:baseURL}images/detail/search?iss=sbiupload&FORM=ANCMS1#enterInsights'。

Google の画像検索 URL は次のように指定します: '{google:baseURL}searchbyimage/upload'。

画像検索の構成を完了するには、[DefaultSearchProviderImageURLPostParams](#defaultsearchproviderimageurlpostparams) ポリシーを参照してください。

このポリシーは、[DefaultSearchProviderEnabled](#defaultsearchproviderenabled) ポリシーと [DefaultSearchProviderSearchURL](#defaultsearchprovidersearchurl) ポリシーを有効にした場合にのみ適用されます。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  文字列

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: DefaultSearchProviderImageURL
  - GP の名前: 既定の検索プロバイダーの画像検索を指定する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/既定の検索プロバイダー
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: DefaultSearchProviderImageURL
  - 値の種類: REG_SZ
  ##### サンプル値:
```
"https://search.contoso.com/searchbyimage/upload"
```


  #### Mac の情報と設定
  - 優先されるキーの名前: DefaultSearchProviderImageURL
  - サンプル値:
``` xml
<string>https://search.contoso.com/searchbyimage/upload</string>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### DefaultSearchProviderImageURLPostParams
  #### POST を使用する画像の URL のパラメーター
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  このポリシーを有効にした場合、POST を使った画像検索の実行時に使用するパラメーターが指定されます。このポリシーには、コンマで区切られた名前と値のペアが含まれます。値がテンプレート パラメータ (上記の例の {imageThumbnail} など) の場合は、実際の画像サムネイルのデータに置き換えられます。このポリシーは、[DefaultSearchProviderEnabled](#defaultsearchproviderenabled) ポリシーと [DefaultSearchProviderSearchURL](#defaultsearchprovidersearchurl) ポリシーを有効にした場合にのみ適用されます。

Bing の画像検索 URL の POST パラメーターは次のように指定します:
'imageBin={google:imageThumbnailBase64}'.

Google の画像検索 URL の POST パラメーターは次のように指定します:
'encoded_image={google:imageThumbnail},image_url={google:imageURL},sbisrc={google:imageSearchSource},original_width={google:imageOriginalWidth},original_height={google:imageOriginalHeight}'.

このポリシーを設定しなかった場合、画像検索要求は GET メソッドを使用して送信されます。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  文字列

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: DefaultSearchProviderImageURLPostParams
  - GP の名前: POST を使用する画像の URL のパラメーター
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/既定の検索プロバイダー
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: DefaultSearchProviderImageURLPostParams
  - 値の種類: REG_SZ
  ##### サンプル値:
```
"content={imageThumbnail},url={imageURL},sbisrc={SearchSource}"
```


  #### Mac の情報と設定
  - 優先されるキーの名前: DefaultSearchProviderImageURLPostParams
  - サンプル値:
``` xml
<string>content={imageThumbnail},url={imageURL},sbisrc={SearchSource}</string>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### DefaultSearchProviderKeyword
  #### 既定の検索プロバイダーのキーワード
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  アドレス バーで使用するショートカットとして、このプロバイダーで検索をトリガーするためのキーワードを指定します。

このポリシーは省略可能です。このポリシーを構成しなかった場合、キーワードによって検索プロバイダーはアクティブになりません。

このポリシーは、[DefaultSearchProviderEnabled](#defaultsearchproviderenabled) ポリシーと [DefaultSearchProviderSearchURL](#defaultsearchprovidersearchurl) ポリシーを有効にした場合にのみ適用されます。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  文字列

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: DefaultSearchProviderKeyword
  - GP の名前: 既定の検索プロバイダーのキーワード
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/既定の検索プロバイダー
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: DefaultSearchProviderKeyword
  - 値の種類: REG_SZ
  ##### サンプル値:
```
"mis"
```


  #### Mac の情報と設定
  - 優先されるキーの名前: DefaultSearchProviderKeyword
  - サンプル値:
``` xml
<string>mis</string>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### DefaultSearchProviderName
  #### 既定の検索プロバイダーの名前
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  既定の検索プロバイダーの名前を指定します。

このポリシーを有効にした場合、既定の検索プロバイダーの名前を設定します。

このポリシーを有効にしなかった場合または空白のままにした場合、検索 URL で指定されたホスト名が使用されます。

'DefaultSearchProviderName' は、組織で承認されている暗号化された検索プロバイダーに設定する必要があります。これは、DTBC-0008 で設定されている暗号化された検索プロバイダーに対応します。このポリシーは、[DefaultSearchProviderEnabled](#defaultsearchproviderenabled) ポリシーと [DefaultSearchProviderSearchURL](#defaultsearchprovidersearchurl) ポリシーが有効になっている場合にのみ適用されます。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  文字列

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: DefaultSearchProviderName
  - GP の名前: 既定の検索プロバイダーの名前
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/既定の検索プロバイダー
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: DefaultSearchProviderName
  - 値の種類: REG_SZ
  ##### サンプル値:
```
"My Intranet Search"
```


  #### Mac の情報と設定
  - 優先されるキーの名前: DefaultSearchProviderName
  - サンプル値:
``` xml
<string>My Intranet Search</string>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### DefaultSearchProviderSearchURL
  #### 既定の検索プロバイダーの検索 URL
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  既定の検索で使用する検索エンジンの URL を指定します。URL には、文字列 '{searchTerms}' を含めます。クエリの実行時、この文字列はユーザーが検索する用語に置き換えられます。

Bing の検索 URL は次のように指定します。

'{bing:baseURL}search?q={searchTerms}'.

Google の検索 URL は、'{google:baseURL}search?q={searchTerms}&{google:RLZ}{google:originalQueryForSuggestion}{google:assistedQueryStats}{google:searchFieldtrialParameter}{google:searchClient}{google:sourceId}ie={inputEncoding}' のように指定します。

このポリシーは、[DefaultSearchProviderEnabled](#defaultsearchproviderenabled) ポリシーを有効にした場合に必要となります。'DefaultSearchProviderEnabled' ポリシーを有効にしなかった場合、このポリシーは無視されます。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  文字列

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: DefaultSearchProviderSearchURL
  - GP の名前: 既定の検索プロバイダーの検索 URL
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/既定の検索プロバイダー
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: DefaultSearchProviderSearchURL
  - 値の種類: REG_SZ
  ##### サンプル値:
```
"https://search.contoso.com/search?q={searchTerms}"
```


  #### Mac の情報と設定
  - 優先されるキーの名前: DefaultSearchProviderSearchURL
  - サンプル値:
``` xml
<string>https://search.contoso.com/search?q={searchTerms}</string>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### DefaultSearchProviderSuggestURL
  #### 検索候補を使用するための既定の検索プロバイダーの URL
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  検索候補の表示に使用する検索エンジンの URL を指定します。URL には文字列 '{searchTerms}' を含めます。クエリの実行時、この文字列はユーザーがこれまで入力したテキストに置き換えられます。

このポリシーは省略可能です。このポリシーを構成しなかった場合、ユーザーには検索候補は表示されません。閲覧の履歴とお気に入りに基づく候補が表示されます。

Bing での検索候補の URL は次のように指定できます。

'{bing:baseURL}qbox?query={searchTerms}'

Google での検索候補の URL は、'{google:baseURL}complete/search?output=chrome&q={searchTerms}' のように指定できます。

このポリシーは、[DefaultSearchProviderEnabled](#defaultsearchproviderenabled) ポリシーと [DefaultSearchProviderSearchURL](#defaultsearchprovidersearchurl) ポリシーを有効にした場合にのみ適用されます。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  文字列

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: DefaultSearchProviderSuggestURL
  - GP の名前: 検索候補を使用するための既定の検索プロバイダーの URL
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/既定の検索プロバイダー
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: DefaultSearchProviderSuggestURL
  - 値の種類: REG_SZ
  ##### サンプル値:
```
"https://search.contoso.com/suggest?q={searchTerms}"
```


  #### Mac の情報と設定
  - 優先されるキーの名前: DefaultSearchProviderSuggestURL
  - サンプル値:
``` xml
<string>https://search.contoso.com/suggest?q={searchTerms}</string>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ## Additional policies

  [トップに戻る](#microsoft-edge---ポリシー)

  ### AdsSettingForIntrusiveAdsSites
  #### 押し付けがましい広告を表示するサイトに対する広告の設定
  >サポートされているバージョン: Windows および Mac (バージョン 78 以降) の Microsoft Edge

  #### 説明
  押し付けがましい広告を表示するサイトで広告をブロックするかどうかを制御します。このポリシーを次のいずれかのオプションに設定できます。

* 1 = すべてのサイトで広告を許可する。

* 2 = 押し付けがましい広告を表示するサイトでは広告をブロックする (既定値)。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  整数

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: AdsSettingForIntrusiveAdsSites
  - GP の名前: 押し付けがましい広告を表示するサイトに対する広告の設定
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: AdsSettingForIntrusiveAdsSites
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000001
```


  #### Mac の情報と設定
  - 優先されるキーの名前: AdsSettingForIntrusiveAdsSites
  - サンプル値:
``` xml
<integer>1</integer>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### AllowDeletingBrowserHistory
  #### ブラウザーとダウンロードの履歴の削除を有効にする
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  ブラウザーの履歴とダウンロードの履歴の削除を有効にして、ユーザーがこの設定を変更できないようにします。

このポリシーを無効にしても、閲覧とダウンロードの履歴が保持されることは保証されない点に注意してください。ユーザーは履歴データベースのファイルを直接編集または削除できます。また、ブラウザー自体が任意の、あるいはすべての履歴項目を (有効期限に基づいて) 削除、またはいつでもアーカイブできます。

このポリシーを有効にした場合、または構成しなかった場合は、ユーザーは閲覧とダウンロードの履歴を削除できます。

このポリシーを無効にした場合、ユーザーは閲覧とダウンロードの履歴を削除できません。

このポリシーを有効にした場合、[Microsoft Edge が閉じられたときに閲覧データを消去する] ポリシーを有効にしないでください。これは、両方でデータの削除を処理することになるためです。両方を有効にした場合、[Microsoft Edge が閉じられたときに閲覧データを消去する] ポリシーが優先され、Microsoft Edge を閉じたときに、このポリシーの構成方法に関係なく、すべてのデータが削除されます。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  ブール値

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: AllowDeletingBrowserHistory
  - GP の名前: ブラウザーとダウンロードの履歴の削除を有効にする
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: AllowDeletingBrowserHistory
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000001
```


  #### Mac の情報と設定
  - 優先されるキーの名前: AllowDeletingBrowserHistory
  - サンプル値:
``` xml
<true/>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### AllowFileSelectionDialogs
  #### ファイルの選択ダイアログを許可する
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  Microsoft Edge でファイル選択ダイアログを表示できるようにすることで、ローカル ファイルへのアクセスを許可します。

このポリシーを有効にした場合または構成しなかった場合は、ユーザーは通常どおりにファイル選択ダイアログを開くことができます。

このポリシーを無効にした場合、ファイル選択ダイアログをトリガーする操作 (お気に入りのインポート、ファイルのアップロード、リンクの保存など) をユーザーが実行したとき、操作が実行される代わりにメッセージが常に表示され、ユーザーはファイル選択ダイアログで [キャンセル] をクリックしたと見なされます。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  ブール値

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: AllowFileSelectionDialogs
  - GP の名前: ファイルの選択ダイアログを許可する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: AllowFileSelectionDialogs
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000001
```


  #### Mac の情報と設定
  - 優先されるキーの名前: AllowFileSelectionDialogs
  - サンプル値:
``` xml
<true/>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### AllowPopupsDuringPageUnload
  #### ページのアンロード中にポップアップの表示を許可する
  >サポートされているバージョン: Windows および Mac (バージョン 78 以降) の Microsoft Edge

  #### 説明
  このポリシーを使用すると、管理者は、ページのアンロード中にページにポップアップが表示されるよう指定できます。

このポリシーを有効に設定した場合、ページをアンロードしているときに、ページにポップアップを表示することができます。

このポリシーを無効に設定した場合または設定しなかった場合、ページをアンロードしているときに、ページにポップアップを表示することはできません。これは、仕様 (https://html.spec.whatwg.org/#apis-for-creating-and-navigating-browsing-contexts-by-name) に従うためです。

このポリシーは将来削除される予定です。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: いいえ - ブラウザーの再起動が必要です

  #### データ型:
  ブール値

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: AllowPopupsDuringPageUnload
  - GP の名前: ページのアンロード中にポップアップの表示を許可する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: AllowPopupsDuringPageUnload
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000000
```


  #### Mac の情報と設定
  - 優先されるキーの名前: AllowPopupsDuringPageUnload
  - サンプル値:
``` xml
<false/>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### AllowSyncXHRInPageDismissal
  #### ページを閉じるときにページで同期 XHR 要求を送信することを許可する
  >サポートされているバージョン: Windows および Mac (バージョン 79 以降) の Microsoft Edge

  #### 説明
  このポリシーを使用すると、ページを閉じるときにページで同期 XHR 要求を送信できることを指定できます。

このポリシーを有効にした場合、ページを閉じるときにページで同期 XHR 要求を送信することができます。

このポリシーを無効にした場合または構成しなかった場合、ページを閉じるときにページで同期 XHR 要求を送信することはできません。

このポリシーは一時的なものであり、将来のリリースでは削除されます。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: いいえ - ブラウザーの再起動が必要です

  #### データ型:
  ブール値

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: AllowSyncXHRInPageDismissal
  - GP の名前: ページを閉じるときにページで同期 XHR 要求を送信することを許可する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: AllowSyncXHRInPageDismissal
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000000
```


  #### Mac の情報と設定
  - 優先されるキーの名前: AllowSyncXHRInPageDismissal
  - サンプル値:
``` xml
<false/>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### AllowTrackingForUrls
  #### 特定のサイトの追跡防止の例外を構成する
  >サポートされているバージョン: Windows および Mac (バージョン 78 以降) の Microsoft Edge

  #### 説明
  追跡防止の対象外とする URL パターンの一覧を構成します。

このポリシーを構成した場合、構成された URL パターンの一覧が追跡防止から除外されます。

このポリシーを構成しなかった場合、すべてのサイトで、"ユーザーの Web 閲覧アクティビティの追跡をブロックする" ポリシーのグローバル デフォルト値 (設定されている場合)、またはユーザーの個人用の構成が使用されます。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  文字列の一覧

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: AllowTrackingForUrls
  - GP の名前: 特定のサイトの追跡防止の例外を構成する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge\AllowTrackingForUrls
  - パス (おすすめ): N/A
  - 値の名前: 1, 2, 3, ...
  - 値の種類: REG_SZ の一覧
  ##### サンプル値:
```
SOFTWARE\Policies\Microsoft\Edge\AllowTrackingForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\AllowTrackingForUrls\1 = "[*.]contoso.edu"

```


  #### Mac の情報と設定
  - 優先されるキーの名前: AllowTrackingForUrls
  - サンプル値:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### AlwaysOpenPdfExternally
  #### PDF ファイルを常に外部で開く
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  Microsoft Edge の内部 PDF ビューアーを無効にします。

このポリシーを有効にした場合、Microsoft Edge では PDF ファイルがダウンロードとして扱われ、ユーザーは既定のアプリケーションでそれらのファイルを開くことができます。

このポリシーを構成しなかった場合、または無効にした場合は、Microsoft Edge は、(ユーザーが無効にしない限り) PDF ファイルを開きます。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  ブール値

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: AlwaysOpenPdfExternally
  - GP の名前: PDF ファイルを常に外部で開く
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: AlwaysOpenPdfExternally
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000001
```


  #### Mac の情報と設定
  - 優先されるキーの名前: AlwaysOpenPdfExternally
  - サンプル値:
``` xml
<true/>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### ApplicationLocaleValue
  #### アプリケーションのロケールを設定する
  >サポートされているバージョン: Windows (バージョン 77 以降) の Microsoft Edge

  #### 説明
  Microsoft Edge のアプリケーション ロケールを構成し、ユーザーがロケールを変更できないようにします。

このポリシーを有効にした場合、Microsoft Edge では指定されたロケールが使用されます。構成したロケールがサポートされていない場合、代わりに 'en-US' が使用されます。

この設定を無効にした場合または構成しなかった場合、Microsoft Edge では、ユーザー指定の優先されるロケール (構成されている場合)、または代替のロケール 'en-US' が使用されます。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: はい
  - 動的ポリシーの更新: いいえ - ブラウザーの再起動が必要です

  #### データ型:
  文字列

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: ApplicationLocaleValue
  - GP の名前: アプリケーションのロケールを設定する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): 管理用テンプレート/Microsoft Edge - 既定の設定 (ユーザーはオーバーライドできます)/
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): SOFTWARE\Policies\Microsoft\Edge\おすすめ
  - 値の名前: ApplicationLocaleValue
  - 値の種類: REG_SZ
  ##### サンプル値:
```
"en"
```


  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### AudioCaptureAllowed
  #### オーディオ キャプチャを許可または禁止する
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  オーディオ キャプチャ デバイスへの Web サイト アクセスの許可をユーザーに確認するかどうかを設定できます。このポリシーは、[AudioCaptureAllowedUrls](#audiocaptureallowedurls) のリストで構成されている URL を除くすべての URL に適用されます。

このポリシーを有効にした場合または構成しなかった場合 (既定の設定)、ユーザーは、[AudioCaptureAllowedUrls](#audiocaptureallowedurls) のリストに含まれていない URL からのオーディオ キャプチャへのアクセスを許可するように求められます。このリストに含まれている URL については、ユーザーへの確認なしでアクセスが許可されます。

この設定を無効にした場合、ユーザーへの確認は行われず、オーディオ キャプチャにアクセスできるのは、[AudioCaptureAllowedUrls](#audiocaptureallowedurls) で構成されている URL からのみになります。

このポリシーは、内蔵マイクだけでなく、すべての種類のオーディオ入力に影響します。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  ブール値

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: AudioCaptureAllowed
  - GP の名前: オーディオ キャプチャを許可または禁止する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: AudioCaptureAllowed
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000000
```


  #### Mac の情報と設定
  - 優先されるキーの名前: AudioCaptureAllowed
  - サンプル値:
``` xml
<false/>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### AudioCaptureAllowedUrls
  #### アクセス許可を要求しなくてもオーディオ キャプチャ デバイスにアクセスできるサイト
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  ユーザーに対してアクセス許可を要求しなくてもオーディオ キャプチャ デバイスを使用できる Web サイトを、URL パターンに基づいて定義します。このリスト内のパターンは、要求元 URL のセキュリティ オリジンと照合されます。パターンが一致すると、サイトに対して、オーディオ キャプチャ デバイスへのアクセスが自動的に許可されます。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  文字列の一覧

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: AudioCaptureAllowedUrls
  - GP の名前: アクセス許可を要求しなくてもオーディオ キャプチャ デバイスにアクセスできるサイト
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge\AudioCaptureAllowedUrls
  - パス (おすすめ): N/A
  - 値の名前: 1, 2, 3, ...
  - 値の種類: REG_SZ の一覧
  ##### サンプル値:
```
SOFTWARE\Policies\Microsoft\Edge\AudioCaptureAllowedUrls\0 = "https://www.contoso.com/"
SOFTWARE\Policies\Microsoft\Edge\AudioCaptureAllowedUrls\1 = "https://[*.]contoso.edu/"

```


  #### Mac の情報と設定
  - 優先されるキーの名前: AudioCaptureAllowedUrls
  - サンプル値:
``` xml
<array>
  <string>https://www.contoso.com/</string>
  <string>https://[*.]contoso.edu/</string>
</array>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### AutoImportAtFirstRun
  #### 初回実行時に別のブラウザーのデータと設定を自動的にインポートする
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  このポリシーを有効にした場合、 Microsoft Edge では、サポートされているすべてのデータ型と設定を既定のブラウザーまたは指定した別のブラウザーから自動的にインポートします。また、Microsoft Edge で、初回実行エクスペリエンスのインポート セクションをスキップさせることもできます。

このポリシーを 'DisabledAutoImport' (4) に設定した場合、初回実行エクスペリエンスのインポート セクションがすべてスキップされ、Microsoft Edge では、ブラウザー データや設定が自動的にインポートされなくなります。

* 0 = サポートされているすべてのデータ型と設定を既定のブラウザーから自動的にインポートする

* 1 = サポートされているすべてのデータ型と設定を Internet Explorer から自動的にインポートする

* 2 = サポートされているすべてのデータ型と設定を Google Chrome から自動的にインポートする

* 3 = サポートされているすべてのデータ型と設定を Safari から自動的にインポートする

* 4 = 自動インポートを無効にし、初回実行エクスペリエンスのインポート セクションをスキップする

**注意**: 現在このポリシーでは、Internet Explorer (Windows 7、8、10)、Google Chrome (Windows 7、8、10、および macOS)、Apple Safari (macOS) の各ブラウザーからのインポートをサポートします。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: いいえ - ブラウザーの再起動が必要です

  #### データ型:
  整数

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: AutoImportAtFirstRun
  - GP の名前: 初回実行時に別のブラウザーのデータと設定を自動的にインポートする
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: AutoImportAtFirstRun
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000002
```


  #### Mac の情報と設定
  - 優先されるキーの名前: AutoImportAtFirstRun
  - サンプル値:
``` xml
<integer>2</integer>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### AutofillAddressEnabled
  #### アドレスのオートフィルを有効にする
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  オートフィル機能を有効にし、以前に保存した情報を使用して Web フォームでの住所情報のオートコンプリートを有効にします。

このポリシーを無効にした場合、オートフィルによる住所情報の提案や入力が行われず、また、Web の閲覧中にユーザーが送信する可能性がある追加の住所情報も保存されません。

このポリシーを有効にした場合または構成しなかった場合、ユーザーはユーザー インターフェイスで住所のオートフィルを制御できます。

このポリシーを無効にした場合は、支払いとパスワードのフォームを除く、すべての Web フォームでアクティビティがすべて停止されることに注意してください。追加の入力内容は保存されず、Microsoft Edge では、以前の入力情報は候補として表示されず、オートフィルも実行されません。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: はい
  - 動的ポリシーの更新: はい

  #### データ型:
  ブール値

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: AutofillAddressEnabled
  - GP の名前: アドレスのオートフィルを有効にする
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): 管理用テンプレート/Microsoft Edge - 既定の設定 (ユーザーはオーバーライドできます)/
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): SOFTWARE\Policies\Microsoft\Edge\おすすめ
  - 値の名前: AutofillAddressEnabled
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000000
```


  #### Mac の情報と設定
  - 優先されるキーの名前: AutofillAddressEnabled
  - サンプル値:
``` xml
<false/>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### AutofillCreditCardEnabled
  #### クレジット カード情報についてオートフィルを有効にする
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  Microsoft Edge のオートフィル機能を有効にし、前回保存された情報を使用して Web フォームでクレジット カード情報の入力を自動的に完了できるようにします。

このポリシーを無効にした場合、オートフィルで、クレジット カード情報の候補が表示または入力されたり、ユーザーが Web を閲覧しているときに送信する可能性のある追加のクレジット カード情報が保存されることはありません。

このポリシーを有効にした場合、または構成しなかった場合は、ユーザーはクレジット カードのオートフィルを制御できます。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: はい
  - 動的ポリシーの更新: はい

  #### データ型:
  ブール値

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: AutofillCreditCardEnabled
  - GP の名前: クレジット カード情報についてオートフィルを有効にする
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): 管理用テンプレート/Microsoft Edge - 既定の設定 (ユーザーはオーバーライドできます)/
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): SOFTWARE\Policies\Microsoft\Edge\おすすめ
  - 値の名前: AutofillCreditCardEnabled
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000000
```


  #### Mac の情報と設定
  - 優先されるキーの名前: AutofillCreditCardEnabled
  - サンプル値:
``` xml
<false/>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### AutoplayAllowed
  #### Web サイトでのメディアの自動再生を許可する
  >サポートされているバージョン: Windows および Mac (バージョン 78 以降) の Microsoft Edge

  #### 説明
  このポリシーは、Web サイトでのメディアの自動再生のポリシーを設定します。

既定の設定では "未構成" となり、現在指定されているメディアの自動再生の設定が適用され、ユーザーは自動再生の設定を構成することができます。

"有効" に設定すると、メディアの自動再生が "許可" に設定されます。すべての Web サイトでメディアの自動再生が許可されます。ユーザーは、このポリシーをオーバーライドすることはできません。

"無効" に設定すると、メディアの自動再生が "禁止" に設定されます。どの Web サイトでもメディアの自動再生は許可されません。ユーザーは、このポリシーをオーバーライドすることはできません。

このポリシーを有効にするには、タブを閉じてからもう一度開く必要があります。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  ブール値

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: AutoplayAllowed
  - GP の名前: Web サイトでのメディアの自動再生を許可する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: AutoplayAllowed
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000001
```


  #### Mac の情報と設定
  - 優先されるキーの名前: AutoplayAllowed
  - サンプル値:
``` xml
<true/>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### BackgroundModeEnabled
  #### Microsoft Edge が終了してもバックグラウンド アプリの実行を続行する
  >サポートされているバージョン: Windows (バージョン 77 以降) の Microsoft Edge

  #### 説明
  Microsoft Edge プロセスを OS サインイン時に開始し、最後のブラウザー ウィンドウが閉じられた後でもプロセスを引き続き実行できるようにします。このシナリオでは、バックグラウンド アプリと現在の閲覧セッション (すべてのセッション Cookie を含む) はアクティブな状態のままになります。実行中のバックグラウンド プロセスのアイコンは、システム トレイに表示されるため、いつでもシステム トレイからプロセスを終了させることができます。

このポリシーを有効にした場合、バックグラウンド モードが有効になります。

このポリシーを無効にした場合、バックグラウンド モードが無効になります。

このポリシーを構成しなかった場合、最初はバックグラウンド モードが無効になっていますが、ユーザーは edge://settings/system でバックグラウンド モードの動作を構成できます。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: はい
  - 動的ポリシーの更新: はい

  #### データ型:
  ブール値

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: BackgroundModeEnabled
  - GP の名前: Microsoft Edge が終了してもバックグラウンド アプリの実行を続行する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): 管理用テンプレート/Microsoft Edge - 既定の設定 (ユーザーはオーバーライドできます)/
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): SOFTWARE\Policies\Microsoft\Edge\おすすめ
  - 値の名前: BackgroundModeEnabled
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000001
```


  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### BackgroundTemplateListUpdatesEnabled
  #### 利用可能なテンプレートの一覧に対するバックグラウンドでの更新を有効にします。このテンプレートとは、コレクションや、テンプレートを使用する他の機能で利用できるテンプレートです。
  >サポートされているバージョン: Windows および Mac (バージョン 79 以降) の Microsoft Edge

  #### 説明
  利用可能なテンプレートの一覧に対するバックグラウンドでの更新を有効または無効にすることができます。このテンプレートとは、コレクションや、テンプレートを使用する他の機能で利用できるテンプレートです。テンプレートは、ページがコレクションに保存されるときに、リッチ メタデータを Web ページから抽出するために使用されます。

この設定を有効にした場合または構成しなかった場合、利用可能なテンプレートの一覧が、24 時間ごとに Microsoft サービスからバックグラウンドでダウンロードされます。

この設定を無効にした場合、利用可能なテンプレートの一覧は要求に応じてダウンロードされます。この種類のダウンロードでは、コレクションやその他の機能について、若干のパフォーマンスの低下が発生する可能性があります。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  ブール値

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: BackgroundTemplateListUpdatesEnabled
  - GP の名前: 利用可能なテンプレートの一覧に対するバックグラウンドでの更新を有効にします。このテンプレートとは、コレクションや、テンプレートを使用する他の機能で利用できるテンプレートです。
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: BackgroundTemplateListUpdatesEnabled
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000001
```


  #### Mac の情報と設定
  - 優先されるキーの名前: BackgroundTemplateListUpdatesEnabled
  - サンプル値:
``` xml
<true/>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### BlockThirdPartyCookies
  #### サードパーティの Cookie をブロックする
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  Web ページの要素がアドレス バーに表示されているドメインからのものではない場合、この Web ページの要素による Cookie の設定を禁止します。

このポリシーを有効にした場合、アドレス バーに表示されているドメインからのものではない Web ページの要素は Cookie を設定できません。

このポリシーを無効にした場合、アドレス バーには表示されていないドメインからの Web ページの要素は Cookie を設定できます。

このポリシーを構成しなかった場合、サード パーティの Cookie が有効になりますが、ユーザーはこの設定を変更できます。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: はい
  - 動的ポリシーの更新: はい

  #### データ型:
  ブール値

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: BlockThirdPartyCookies
  - GP の名前: サードパーティの Cookie をブロックする
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): 管理用テンプレート/Microsoft Edge - 既定の設定 (ユーザーはオーバーライドできます)/
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): SOFTWARE\Policies\Microsoft\Edge\おすすめ
  - 値の名前: BlockThirdPartyCookies
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000000
```


  #### Mac の情報と設定
  - 優先されるキーの名前: BlockThirdPartyCookies
  - サンプル値:
``` xml
<false/>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### BrowserAddProfileEnabled
  #### ID ポップアップ メニューまたは [設定] ページでのプロファイル作成を有効にする
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  ユーザーは、**[プロファイルの追加]** オプションを使用して新しいプロファイルを作成できます。
このポリシーが有効になっている場合または構成されていない場合、ユーザーは Microsoft Edge の ID ポップアップ メニューまたは設定ページから **[プロファイルの追加]** を使用して新しいプロファイルを作成できます。

このポリシーが無効になっている場合、ユーザーは ID ポップアップ メニューまたは設定ページから新しいプロファイルを追加することができません。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  ブール値

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: BrowserAddProfileEnabled
  - GP の名前: ID ポップアップ メニューまたは [設定] ページでのプロファイル作成を有効にする
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: BrowserAddProfileEnabled
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000001
```


  #### Mac の情報と設定
  - 優先されるキーの名前: BrowserAddProfileEnabled
  - サンプル値:
``` xml
<true/>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### BrowserGuestModeEnabled
  #### ゲスト モードを有効にする
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  Microsoft Edge でゲスト プロファイルの使用を許可するためのオプションを有効にします。ゲスト プロファイルでは、ブラウザーは既存のプロファイルから閲覧データをインポートせず、すべてのゲスト プロファイルが閉じられたときに閲覧データを削除します。

このポリシーを有効にした場合または構成しなかった場合、Microsoft Edge では、ゲスト プロファイルでの閲覧がユーザーに許可されます。

このポリシーを無効にした場合、Microsoft Edge では、ゲスト プロファイルでの閲覧がユーザーに許可されません。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  ブール値

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: BrowserGuestModeEnabled
  - GP の名前: ゲスト モードを有効にする
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: BrowserGuestModeEnabled
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000001
```


  #### Mac の情報と設定
  - 優先されるキーの名前: BrowserGuestModeEnabled
  - サンプル値:
``` xml
<true/>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### BrowserNetworkTimeQueriesEnabled
  #### ブラウザー ネットワーク タイム サービスへのクエリを許可する
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  Microsoft Edge が正確なタイムスタンプを取得するために、ブラウザー ネットワーク タイム サービスに不定期にクエリを送信するのを防ぎます。

このポリシーを無効にした場合、Microsoft Edge によるブラウザー ネットワーク タイム サービスへのクエリの送信を停止します。

このポリシーを有効にした場合、または構成しなかった場合は、Microsoft Edge では、ブラウザー ネットワーク タイム サービスにクエリが不定期に送信されます。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  ブール値

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: BrowserNetworkTimeQueriesEnabled
  - GP の名前: ブラウザー ネットワーク タイム サービスへのクエリを許可する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: BrowserNetworkTimeQueriesEnabled
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000001
```


  #### Mac の情報と設定
  - 優先されるキーの名前: BrowserNetworkTimeQueriesEnabled
  - サンプル値:
``` xml
<true/>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### BrowserSignin
  #### ブラウザー サインインの設定
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  ユーザーが自分のアカウントで Microsoft Edge にサインインして、アカウントに関連するサービス (同期やシングル サインオンなど) を使用できるかどうかを指定します。同期を利用できるかどうかを制御するには、代わりに [SyncDisabled](#syncdisabled) ポリシーを使用します。

このポリシーを 'ブラウザー サインインを無効にする' に設定した場合、[NonRemovableProfileEnabled](#nonremovableprofileenabled) ポリシーも無効に設定していることを確認してください。これは、[NonRemovableProfileEnabled](#nonremovableprofileenabled) によって、自動的にサインインされるブラウザー プロファイルの作成が無効になるためです。両方のポリシーが設定されていると、Microsoft Edge では 'ブラウザー サインインを無効にする' ポリシーが使用され、[NonRemovableProfileEnabled](#nonremovableprofileenabled) が無効に設定されているものとして動作します。

このポリシーを 'ブラウザー サインインを有効にする' (1) に設定した場合、ユーザーはブラウザーにサインインすることができます。ブラウザーにサインインしても、同期が既定で有効になるというわけではありません。同期の機能を使用するには、ユーザーは個別にオプトインする必要があります。

このポリシーを 'ブラウザー サインインを強制する' (2) に設定した場合、ユーザーはブラウザーを使用するためにプロファイルにサインインする必要があります。既定では、ドメイン管理者や [SyncDisabled](#syncdisabled) ポリシーによって同期が無効になっていない限り、この設定よって、ユーザーは自分のアカウントと同期するかどうかを選択することができます。[BrowserGuestModeEnabled](#browserguestmodeenabled) ポリシーの既定値は false に設定されます。

このポリシーを構成しなかった場合、ユーザーは、ブラウザー サインイン オプションを有効にして、ブラウザーをユーザーに合った状態で使用できるようにするかどうかを指定できます。

* 0 = ブラウザー サインインを無効にする

* 1 = ブラウザー サインインを有効にする

* 2 = ユーザーにサインインしてブラウザーを使用するよう強制する

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: いいえ - ブラウザーの再起動が必要です

  #### データ型:
  整数

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: BrowserSignin
  - GP の名前: ブラウザー サインインの設定
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: BrowserSignin
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000002
```


  #### Mac の情報と設定
  - 優先されるキーの名前: BrowserSignin
  - サンプル値:
``` xml
<integer>2</integer>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### BuiltInDnsClientEnabled
  #### 組み込みの DNS クライアントを使用する
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  組み込みの DNS クライアントを使用するかどうかを制御します。

このポリシーを有効にした場合、組み込みの DNS クライアントが使用されます (使用可能な場合)。

このポリシーを無効にした場合、組み込みの DNS クライアントは使用されません。

このポリシーを構成しなかった場合、MacOS では組み込みの DNS クライアントが既定で有効になり、ユーザーは、edge://flags を編集するか、コマンド ライン フラグを指定することで、組み込みの DNS クライアントを使用するかどうかを変更できます。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  ブール値

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: BuiltInDnsClientEnabled
  - GP の名前: 組み込みの DNS クライアントを使用する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: BuiltInDnsClientEnabled
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000001
```


  #### Mac の情報と設定
  - 優先されるキーの名前: BuiltInDnsClientEnabled
  - サンプル値:
``` xml
<true/>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### CertificateTransparencyEnforcementDisabledForCas
  #### subjectPublicKeyInfo ハッシュのリストに対する証明書の透明性の適用を無効にする
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  subjectPublicKeyInfo ハッシュのリストに対する証明書の透明性に関する要件の適用を無効にします。

このポリシーでは、指定された subjectpublickeyinfo ハッシュのいずれかを持つ証明書を含む証明書チェーンに対して、証明書の透明性の公開要件を無効にできます。これにより証明書を、引き続きエンタープライズ ホストに使用することができます。このポリシーを設定しない場合は、適切に公開されないため信頼できない証明書となります。

このポリシーが設定されているときに証明書の透明性の適用を無効にするには、次の条件のいずれかを満たしている必要があります。
1. サーバー証明書の subjectPublicKeyInfo のハッシュである。
2. 証明書チェーンの CA 証明書に表示される subjectPublicKeyInfo のハッシュである (CA 証明書が X.509v3 nameConstraints 拡張機能で制限されており、1 つ以上の directoryName nameConstraints が permittedSubtrees にある。また directoryName には organizationName 属性が含まれている)。
3. 証明書チェーンの CA 証明書に表示される subjectPublicKeyInfo のハッシュである。CA 証明書には証明書のサブジェクトに 1 つ以上の organizationName 属性が含まれ、サーバーの証明書には同じ数の organizationName 属性がバイトごとに同一の値を持ち、同じ順序で含まれている。

subjectPublicKeyInfo ハッシュは、ハッシュ アルゴリズムの名前、"/" 文字、および指定された証明書の subjectPublicKeyInfo (DER でエンコードされています) に適用されるハッシュ アルゴリズムの Base64 エンコードを連結することによって指定されます。この Base64 エンコード形式は、RFC 7469 のセクション 2.4 で定義されているように、SPKI フィンガープリントと同じ形式になります。認識されないハッシュ アルゴリズムは無視されます。現時点でサポートされているハッシュ アルゴリズムは、"sha256" だけです。

このポリシーを無効にした場合または構成しなかった場合、証明書の透明性を介して公開する必要のある証明書は、証明書の透明性ポリシーに従って公開されていない場合、信頼できないものとして扱われます。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  文字列の一覧

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: CertificateTransparencyEnforcementDisabledForCas
  - GP の名前: subjectPublicKeyInfo ハッシュのリストに対する証明書の透明性の適用を無効にする
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge\CertificateTransparencyEnforcementDisabledForCas
  - パス (おすすめ): N/A
  - 値の名前: 1, 2, 3, ...
  - 値の種類: REG_SZ の一覧
  ##### サンプル値:
```
SOFTWARE\Policies\Microsoft\Edge\CertificateTransparencyEnforcementDisabledForCas\0 = "sha256/AAAAAAAAAAAAAAAAAAAAAA=="
SOFTWARE\Policies\Microsoft\Edge\CertificateTransparencyEnforcementDisabledForCas\1 = "sha256//////////////////////w=="

```


  #### Mac の情報と設定
  - 優先されるキーの名前: CertificateTransparencyEnforcementDisabledForCas
  - サンプル値:
``` xml
<array>
  <string>sha256/AAAAAAAAAAAAAAAAAAAAAA==</string>
  <string>sha256//////////////////////w==</string>
</array>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### CertificateTransparencyEnforcementDisabledForLegacyCas
  #### レガシ証明機関のリストに対する証明書の透明性の適用を無効にする
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  レガシ証明機関 (CA) のリストに対して、証明書の透明性に関する要件の適用を無効にします。

このポリシーを使用すると、指定された subjectPublicKeyInfo ハッシュのいずれかを持つ証明書が含まれた証明書チェーンに対して、証明書の透明性に関する開示要件を無効にできます。これにより、適切に公開されていないことを理由に通常であれば信頼できないものとして扱われる証明書を、企業のホストで引き続き使用できるようになります。

証明書の透明性の適用を無効にするには、レガシ証明機関 (CA) として認識されている CA 証明書に含まれる subjectPublicKeyInfo にハッシュを設定する必要があります。レガシ CA とは、Microsoft Edge でサポートされている 1 つ以上のオペレーティング システムで既に一般的に信頼されている CA です。

subjectPublicKeyInfo ハッシュを指定するには、ハッシュ アルゴリズム名、"/" 文字、およびこのハッシュ アルゴリズムの Base64 エンコード (指定された証明書の DER エンコード済み subjectPublicKeyInfo に適用されます) を連結します。この Base64 エンコードは、RFC 7469 のセクション 2.4 で規定されている SPKI フィンガープリントと同じ形式を使用します。認識できないハッシュ アルゴリズムは無視されます。現時点でサポートされているハッシュ アルゴリズムは、"sha256" のみです。

このポリシーを構成しなかった場合、証明書の透明性を介して開示する必要がある証明書はすべて、証明書の透明性ポリシーに従って開示されていない場合は、信頼できない証明書として扱われます。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  文字列の一覧

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: CertificateTransparencyEnforcementDisabledForLegacyCas
  - GP の名前: レガシ証明機関のリストに対する証明書の透明性の適用を無効にする
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge\CertificateTransparencyEnforcementDisabledForLegacyCas
  - パス (おすすめ): N/A
  - 値の名前: 1, 2, 3, ...
  - 値の種類: REG_SZ の一覧
  ##### サンプル値:
```
SOFTWARE\Policies\Microsoft\Edge\CertificateTransparencyEnforcementDisabledForLegacyCas\0 = "sha256/AAAAAAAAAAAAAAAAAAAAAA=="
SOFTWARE\Policies\Microsoft\Edge\CertificateTransparencyEnforcementDisabledForLegacyCas\1 = "sha256//////////////////////w=="

```


  #### Mac の情報と設定
  - 優先されるキーの名前: CertificateTransparencyEnforcementDisabledForLegacyCas
  - サンプル値:
``` xml
<array>
  <string>sha256/AAAAAAAAAAAAAAAAAAAAAA==</string>
  <string>sha256//////////////////////w==</string>
</array>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### CertificateTransparencyEnforcementDisabledForUrls
  #### 特定の URL に対する証明書の透明性の適用を無効にする
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  一覧表示された URL に対して証明書の透過性に関する要件の強制を無効にします。

このポリシーを使用すると、証明書の透過性を介して指定された URL 内のホスト名の証明書を非公開にできます。ポリシーを使用しない場合は適切に公開されないため信頼されない証明書となります。このポリシーによって証明書を使用できますが、これらのホストに対して不正に発行された証明書の検出が困難になります。

[https://go.microsoft.com/fwlink/?linkid=2095322](https://go.microsoft.com/fwlink/?linkid=2095322) に従って URL パターンを形成します。証明書は、スキーム、ポート、またはパスに関係なく、指定されたホスト名に対して有効であるため、URL のホスト名部分のみが考慮されます。ワイルドカード ホストはサポートされていません。

このポリシーを設定しない場合、証明書の透過性を介して公開する必要のあるすべての証明書は、公開されていない場合には信頼できない証明書として処理されます。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  文字列の一覧

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: CertificateTransparencyEnforcementDisabledForUrls
  - GP の名前: 特定の URL に対する証明書の透明性の適用を無効にする
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge\CertificateTransparencyEnforcementDisabledForUrls
  - パス (おすすめ): N/A
  - 値の名前: 1, 2, 3, ...
  - 値の種類: REG_SZ の一覧
  ##### サンプル値:
```
SOFTWARE\Policies\Microsoft\Edge\CertificateTransparencyEnforcementDisabledForUrls\0 = "contoso.com"
SOFTWARE\Policies\Microsoft\Edge\CertificateTransparencyEnforcementDisabledForUrls\1 = ".contoso.com"

```


  #### Mac の情報と設定
  - 優先されるキーの名前: CertificateTransparencyEnforcementDisabledForUrls
  - サンプル値:
``` xml
<array>
  <string>contoso.com</string>
  <string>.contoso.com</string>
</array>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### ClearBrowsingDataOnExit
  #### Microsoft Edge を閉じるときに閲覧データを消去する
  >サポートされているバージョン: Windows および Mac (バージョン 78 以降) の Microsoft Edge

  #### 説明
  Microsoft Edge は、既定では終了時に閲覧データを消去しません。閲覧データには、フォームやパスワードに入力した情報が含まれています。またアクセスした Web サイトで入力した情報も含まれています。

このポリシーを有効にした場合、Microsoft Edge を終了するたびにすべての閲覧データが削除されます。

このポリシーを無効にした場合または構成しなかった場合、ユーザーは [設定] で [閲覧データの消去] オプションを構成できます。

このポリシーを有効にした場合は、[AllowDeletingBrowserHistory](#allowdeletingbrowserhistory) ポリシーを有効にしないでください。どちらのポリシーもデータの削除を扱うためです。両方のポリシーを有効にした場合、このポリシーが優先され、[AllowDeletingBrowserHistory](#allowdeletingbrowserhistory) の構成方法に関係なく、Microsoft Edge の終了時には、すべてのデータが削除されます。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: はい
  - 動的ポリシーの更新: いいえ - ブラウザーの再起動が必要です

  #### データ型:
  ブール値

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: ClearBrowsingDataOnExit
  - GP の名前: Microsoft Edge を閉じるときに閲覧データを消去する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): 管理用テンプレート/Microsoft Edge - 既定の設定 (ユーザーはオーバーライドできます)/
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): SOFTWARE\Policies\Microsoft\Edge\おすすめ
  - 値の名前: ClearBrowsingDataOnExit
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000001
```


  #### Mac の情報と設定
  - 優先されるキーの名前: ClearBrowsingDataOnExit
  - サンプル値:
``` xml
<true/>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### ClickOnceEnabled
  #### ユーザーが ClickOnce プロトコルを使用してファイルを開くことを許可する
  >サポートされているバージョン: Windows (バージョン 78 以降) の Microsoft Edge

  #### 説明
  ユーザーが ClickOnce プロトコルを使用してファイルを開くことを許可します。ClickOnce プロトコルを使用すると、ユーザーのコンピューターまたはデバイス上の ClickOnce ファイル ハンドラーを使用して特定の URL からファイルをブラウザーで開くように、Web サイトから要求できます。

このポリシーを有効にした場合、ユーザーは ClickOnce プロトコルを使用してファイルを開くことができます。このポリシーは、edge://flags/ ページのユーザーの ClickOnce 設定をオーバーライドします。

このポリシーを無効にした場合、ユーザーは ClickOnce プロトコルを使用してファイルを開くことはできません。代わりに、ファイルはブラウザーを使用してファイル システムに保存されます。 このポリシーは、edge://flags/ ページのユーザーの ClickOnce 設定をオーバーライドします。

このポリシーを構成しなかった場合、ユーザーは ClickOnce プロトコルを使用してファイルを開くことはできません。 ユーザーは、edge://flags/ ページで ClickOnce プロトコルの使用できるようにするオプションを利用できます。

ClickOnce を無効にすると、ClickOnce アプリケーション (.application ファイル) が正常に起動されなくなる可能性があります。

ClickOnce の詳細については、[https://go.microsoft.com/fwlink/?linkid=2103872](https://go.microsoft.com/fwlink/?linkid=2103872) および [https://go.microsoft.com/fwlink/?linkid=2099880](https://go.microsoft.com/fwlink/?linkid=2099880) を参照してください。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  ブール値

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: ClickOnceEnabled
  - GP の名前: ユーザーが ClickOnce プロトコルを使用してファイルを開くことを許可する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: ClickOnceEnabled
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000000
```


  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### CommandLineFlagSecurityWarningsEnabled
  #### コマンドライン フラグのセキュリティ警告を有効にする
  >サポートされているバージョン: Windows および Mac (バージョン 78 以降) の Microsoft Edge

  #### 説明
  無効にすると、危険性があるコマンドライン フラグで Microsoft Edge が起動されると、このポリシーはセキュリティ警告が表示されないようにします。

有効にするか設定しない場合、これらのコマンドライン フラグが Microsoft Edge に対して使用されると、セキュリティ警告は表示されます。

たとえば、--disable-gpu-sandbox フラグは次の警告を生成します: サポートされていないコマンドライン フラグ: --disable-gpu-sandbox を使用しています。これにより、安定性およびセキュリティに関するリスクが生じます。

Windows では、このポリシーは、Microsoft Active Directory ドメインに参加しているインスタンス、またはデバイス管理用に登録されている Windows 10 Pro (または Enterprise) インスタンスでのみ使用できます。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: いいえ - ブラウザーの再起動が必要です

  #### データ型:
  ブール値

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: CommandLineFlagSecurityWarningsEnabled
  - GP の名前: コマンドライン フラグのセキュリティ警告を有効にする
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: CommandLineFlagSecurityWarningsEnabled
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000001
```


  #### Mac の情報と設定
  - 優先されるキーの名前: CommandLineFlagSecurityWarningsEnabled
  - サンプル値:
``` xml
<true/>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### ComponentUpdatesEnabled
  #### Microsoft Edge でのコンポーネントの更新を有効にする
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  このポリシーを有効にした場合または構成しなかった場合、Microsoft Edge でコンポーネントの更新が有効になります。

この設定を無効にした場合または false に設定した場合、Microsoft Edge のすべてのコンポーネントに対してコンポーネントの更新が無効になります。

ただし、一部のコンポーネントはこのポリシーの適用対象外となります。このようなコンポーネントには、実行可能コードが含まれていないコンポーネント、ブラウザーの動作を大幅に変更しないコンポーネント、またはセキュリティ上重要なコンポーネントなどがあります。つまり、"セキュリティ上重要" と見なされる更新は、このポリシーを無効にした場合でも適用されます。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: いいえ - ブラウザーの再起動が必要です

  #### データ型:
  ブール値

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: ComponentUpdatesEnabled
  - GP の名前: Microsoft Edge でのコンポーネントの更新を有効にする
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: ComponentUpdatesEnabled
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000001
```


  #### Mac の情報と設定
  - 優先されるキーの名前: ComponentUpdatesEnabled
  - サンプル値:
``` xml
<true/>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### ConfigureDoNotTrack
  #### トラッキング拒否を構成する
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  トラッキング拒否要求を、トラッキング情報を要求する Web サイトに送信するかどうかを指定します。トラッキング拒否要求を使用すると、ユーザーが閲覧アクティビティの追跡を希望していないこと、アクセスした Web サイトに伝えることができます。既定では、Microsoft Edge はトラッキング拒否要求を送信しませんが、ユーザーはこの機能を有効にして、トラッキング拒否要求を送信することができます。

この設定を有効にした場合、トラッキング拒否要求は、トラッキング情報を要求する Web サイトに常に送信されます。

この設定を無効にした場合、要求は送信されません。

このポリシーを構成しなかった場合、ユーザーはこれらの要求を送信するかどうかを選択できます。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  ブール値

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: ConfigureDoNotTrack
  - GP の名前: トラッキング拒否を構成する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: ConfigureDoNotTrack
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000000
```


  #### Mac の情報と設定
  - 優先されるキーの名前: ConfigureDoNotTrack
  - サンプル値:
``` xml
<false/>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### ConfigureOnlineTextToSpeech
  #### オンライン音声合成を構成する
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  ブラウザーでオンライン音声合成の音声フォント (Azure Cognitive Services の一部) を活用できるかどうかを設定します。これらの音声フォントは、プレインストールされているシステム音声フォントよりも品質が高くなっています。

このポリシーを有効にした場合または構成しなかった場合、SpeechSynthesis API を使用する Web ベースのアプリケーションは、オンライン音声合成の音声フォントを利用できます。

このポリシーを無効にした場合、音声フォントは利用できなくなります。

この機能の詳細については以下をご覧ください:
SpeechSynthesis API: [https://go.microsoft.com/fwlink/?linkid=2110038](https://go.microsoft.com/fwlink/?linkid=2110038)
Cognitive Services: [https://go.microsoft.com/fwlink/?linkid=2110141](https://go.microsoft.com/fwlink/?linkid=2110141)

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  ブール値

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: ConfigureOnlineTextToSpeech
  - GP の名前: オンライン音声合成を構成する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: ConfigureOnlineTextToSpeech
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000001
```


  #### Mac の情報と設定
  - 優先されるキーの名前: ConfigureOnlineTextToSpeech
  - サンプル値:
``` xml
<true/>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### CustomHelpLink
  #### カスタム ヘルプのリンクを指定する
  >サポートされているバージョン: Windows および Mac (バージョン 79 以降) の Microsoft Edge

  #### 説明
  [ヘルプ] メニューまたは F1 キーのリンクを指定します。

このポリシーを有効にした場合、管理者は [ヘルプ] メニューや F1 キーのリンクを指定できます。

このポリシーを無効にした場合または構成しなかった場合、[ヘルプ] メニューや F1 キーの既定のリンクが使用されます。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  文字列

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: CustomHelpLink
  - GP の名前: カスタム ヘルプのリンクを指定する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: CustomHelpLink
  - 値の種類: REG_SZ
  ##### サンプル値:
```
"https://go.microsoft.com/fwlink/?linkid=2080734"
```


  #### Mac の情報と設定
  - 優先されるキーの名前: CustomHelpLink
  - サンプル値:
``` xml
<string>https://go.microsoft.com/fwlink/?linkid=2080734</string>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### DefaultBrowserSettingEnabled
  #### Microsoft Edge を既定のブラウザーとして設定する
  >サポートされているバージョン: Windows 7 および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  Microsoft Edge での通常使用するブラウザーの確認を構成し、ユーザーがこの構成を変更できないようにします。

このポリシーを有効にした場合、Microsoft Edge では、通常使用するブラウザーであるかどうかが常にスタートアップ時に確認され、必要に応じて自動登録を行います。

このポリシーを無効にした場合、Microsoft Edge では、通常使用するブラウザーの確認は行われず、このオプションを設定するためのユーザー コントロールが無効になります。

このポリシーを構成しなかった場合、Microsoft Edge が通常使用するブラウザであるかどうか、および通常使用するブラウザでない場合にユーザー通知を表示するかどうかをユーザーが制御できます。

Windows 管理者向け注意事項: このポリシーは、Windows 7 を実行している PC に対してのみ有効です。それよりも後のバージョンの Windows については、"既定のアプリケーションの関連付け" ファイルを展開する必要があります。このファイルによって、Microsoft Edge を https プロトコルや http プロトコルのハンドラーにすることができます (オプションで ftp プロトコルや、.html、.htm、.pdf、.svg、.webp などのファイル形式のハンドラーにすることもできます)。詳細については、[https://go.microsoft.com/fwlink/?linkid=2094932](https://go.microsoft.com/fwlink/?linkid=2094932) を参照してください。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  ブール値

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: DefaultBrowserSettingEnabled
  - GP の名前: Microsoft Edge を既定のブラウザーとして設定する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: DefaultBrowserSettingEnabled
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000001
```


  #### Mac の情報と設定
  - 優先されるキーの名前: DefaultBrowserSettingEnabled
  - サンプル値:
``` xml
<true/>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### DeveloperToolsAvailability
  #### 開発者ツールを使用できる状況を制御する
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  開発者ツールを使用できる状況を制御します。

このポリシーを 'DeveloperToolsDisallowedForForceInstalledExtensions' (0、既定) に設定した場合、基本的には、ユーザーは開発者ツールや JavaScript コンソールにアクセスできますが、エンタープライズ ポリシーによってインストールされた拡張機能では、開発者ツールや JavaScript コンソールにはアクセスできません。

このポリシーを 'DeveloperToolsAllowed' (1) に設定した場合、エンタープライズ ポリシーによってインストールされた拡張機能を含むすべての状況で、ユーザーは開発者ツールや JavaScript コンソールにアクセスできます。

このポリシーを 'DeveloperToolsDisallowed' (2) に設定した場合、ユーザーは開発者ツールにアクセスしたり、Web サイトの要素を検査したりすることはできません。開発者ツールや JavaScript コンソールを開くキーボード ショートカット、メニュー、コンテキスト メニューの各エントリは、無効になります。

* 0 = エンタープライズ ポリシーによってインストールされた拡張機能での開発者ツールの使用を禁止するが、他の状況における開発者ツールの使用は許可する

* 1 = 開発者ツールの使用を許可する

* 2 = 開発者ツールの使用は許可しない

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  整数

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: DeveloperToolsAvailability
  - GP の名前: 開発者ツールを使用できる状況を制御する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: DeveloperToolsAvailability
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000002
```


  #### Mac の情報と設定
  - 優先されるキーの名前: DeveloperToolsAvailability
  - サンプル値:
``` xml
<integer>2</integer>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### DirectInvokeEnabled
  #### ユーザーが DirectInvoke プロトコルを使用してファイルを開くことを許可する
  >サポートされているバージョン: Windows (バージョン 78 以降) の Microsoft Edge

  #### 説明
  ユーザーが DirectInvoke プロトコルを使用してファイルを開くことを許可します。DirectInvoke プロトコルを使用すると、ユーザーのコンピューターまたはデバイス上の特定のファイル ハンドラーを使用して特定の URL からファイルをブラウザーで開くように、Web サイトから要求できます。

このポリシーを有効にした場合または構成しなかった場合、ユーザーは DirectInvoke プロトコルを使用してファイルを開くことができます。

このポリシーを無効にした場合、ユーザーは DirectInvoke プロトコルを使用してファイルを開くことはできません。代わりに、ファイルはファイル システムに保存されます。

注意: DirectInvoke を無効にすると、一部の Microsoft Office SharePoint Online 機能が予期したとおりに機能しなくなる場合があります。

DirectInvoke の詳細については、[https://go.microsoft.com/fwlink/?linkid=2103872](https://go.microsoft.com/fwlink/?linkid=2103872) および [https://go.microsoft.com/fwlink/?linkid=2099871](https://go.microsoft.com/fwlink/?linkid=2099871) を参照してください。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  ブール値

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: DirectInvokeEnabled
  - GP の名前: ユーザーが DirectInvoke プロトコルを使用してファイルを開くことを許可する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: DirectInvokeEnabled
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000000
```


  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### Disable3DAPIs
  #### 3D グラフィックス API のサポートを無効にする
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  Web ページがグラフィック プロセッシング ユニット (GPU) にアクセスできないようにします。具体的には、Web ページは WebGL API にアクセスできず、プラグインでは Pepper 3D API を使用できなくなります。

このポリシーを構成しなかった場合または無効にした場合は、Web ページで WebGL API とプラグインを使用して、Pepper 3D API を使用することができます。Microsoft Edge では、既定でこれらの API を使用するためにコマンド ラインの引数を渡すことが必要になる場合があります。

[HardwareAccelerationModeEnabled](#hardwareaccelerationmodeenabled) ポリシーが false に設定されている場合、'Disable3DAPIs' ポリシーの設定は無視されます。これは、'Disable3DAPIs' ポリシーを true に設定することと同じです。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  ブール値

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: Disable3DAPIs
  - GP の名前: 3D グラフィックス API のサポートを無効にする
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: Disable3DAPIs
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000000
```


  #### Mac の情報と設定
  - 優先されるキーの名前: Disable3DAPIs
  - サンプル値:
``` xml
<false/>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### DisableScreenshots
  #### スクリーンショットの撮影を無効にする
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  ユーザーがブラウザー ページのスクリーンショットを撮ることができるかどうかを制御します。

このポリシーを有効にした場合、ユーザーはキーボード ショートカットや、拡張機能 API を使ってスクリーンショットを撮ることはできません。

このポリシーを無効にした場合または構成しなかった場合、ユーザーはスクリーンショットを撮ることができます。

このポリシーは、ブラウザー内から撮るスクリーンショットを制御することに注意してください。このポリシーを有効にしても、ユーザーはブラウザー外部の方法 (オペレーティング システムの機能や他のアプリケーションなど) を使用して、スクリーンショットを撮ることができる場合があります。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  ブール値

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: DisableScreenshots
  - GP の名前: スクリーンショットの撮影を無効にする
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: DisableScreenshots
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000001
```


  #### Mac の情報と設定
  - 優先されるキーの名前: DisableScreenshots
  - サンプル値:
``` xml
<true/>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### DiskCacheDir
  #### ディスク キャッシュ ディレクトリを設定する
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  キャッシュ ファイルを保存するために使用するディレクトリを構成します。

このポリシーを有効にした場合、Microsoft Edge では、ユーザーが '--disk-cache-dir' フラグを設定したかどうかに関係なく、ポリシーで指定されたディレクトリを使用します。データの損失や他の予期しないエラーを回避するために、このポリシーの構成では、ボリュームのルート ディレクトリまたは他の用途に使用されるディレクトリを指定しないでください。Microsoft Edge で、こうしたディレクトリのコンテンツを管理しているためです。

ディレクトリとパスを指定するときに使用できる変数のリストについては、[https://go.microsoft.com/fwlink/?linkid=2095041](https://go.microsoft.com/fwlink/?linkid=2095041) を参照してください。

このポリシーを構成しなかった場合、既定のキャッシュ ディレクトリが使用されます。ユーザーは、'--disk-cache-dir' コマンド ライン フラグを使用して、既定のキャッシュ ディレクトリをオーバーライドできます。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: いいえ - ブラウザーの再起動が必要です

  #### データ型:
  文字列

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: DiskCacheDir
  - GP の名前: ディスク キャッシュ ディレクトリを設定する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: DiskCacheDir
  - 値の種類: REG_SZ
  ##### サンプル値:
```
"${user_home}/Edge_cache"
```


  #### Mac の情報と設定
  - 優先されるキーの名前: DiskCacheDir
  - サンプル値:
``` xml
<string>${user_home}/Edge_cache</string>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### DiskCacheSize
  #### ディスク キャッシュ サイズをバイト単位で設定する
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  ファイルをディスク上に保存する場合に使用するキャッシュのサイズをバイト単位で構成します。

このポリシーを有効にした場合、Microsoft Edge では、ユーザーが '--disk-cache-size' フラグを指定したかどうかに関係なく、ポリシーで指定されたキャッシュ サイズを使用します。このポリシーで指定される値は、絶対的な境界値を示すものではなく、キャッシュ システム向けの推奨値を示すものです。数メガバイトを下回る値は小さすぎ、適正な最小値に引き上げられます。

このポリシーの値を 0 に設定した場合、既定のキャッシュ サイズが使用されます。ユーザーはこのサイズを変更できません。

このポリシーを構成しなかった場合、既定のサイズが使用されます。ユーザーは '--disk-cache-size' フラグを使用してこのサイズをオーバーライドできます。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: いいえ - ブラウザーの再起動が必要です

  #### データ型:
  整数

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: DiskCacheSize
  - GP の名前: ディスク キャッシュ サイズをバイト単位で設定する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: DiskCacheSize
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x06400000
```


  #### Mac の情報と設定
  - 優先されるキーの名前: DiskCacheSize
  - サンプル値:
``` xml
<integer>104857600</integer>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### DownloadDirectory
  #### ディレクトリをダウンロードする
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  ファイルをダウンロードするときに使用するディレクトリを構成します。

このポリシーを有効にした場合、Microsoft Edge では、ユーザーが既にディレクトリを設定しているかどうか、またはユーザーに対して毎回ダウンロードの場所を要求するように選択したかどうかに関係なく、ポリシーで指定されたディレクトリを使用します。使用できる変数のリストについては、[https://go.microsoft.com/fwlink/?linkid=2095041](https://go.microsoft.com/fwlink/?linkid=2095041) を参照してください。

このポリシーを無効にした場合または構成しなかった場合、既定のダウンロード ディレクトリが使用されます。ユーザーはこの既定のディレクトリを変更できます。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: はい
  - 動的ポリシーの更新: はい

  #### データ型:
  文字列

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: DownloadDirectory
  - GP の名前: ディレクトリをダウンロードする
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): 管理用テンプレート/Microsoft Edge - 既定の設定 (ユーザーはオーバーライドできます)/
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): SOFTWARE\Policies\Microsoft\Edge\おすすめ
  - 値の名前: DownloadDirectory
  - 値の種類: REG_SZ
  ##### サンプル値:
```
"/home/${user_name}/Downloads"
```


  #### Mac の情報と設定
  - 優先されるキーの名前: DownloadDirectory
  - サンプル値:
``` xml
<string>/home/${user_name}/Downloads</string>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### DownloadRestrictions
  #### ダウンロードの制限を許可する
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  Microsoft Edge で完全にブロックするダウンロードの種類を構成します。ユーザーは、セキュリティの判定結果をオーバーライドすることはできません。

  '危険なダウンロードをブロックする' (1) に設定すると、Microsoft Defender SmartScreen の警告が表示される場合にダウンロードがブロックされ、それ以外の場合はすべてのダウンロードが許可されます。

'危険性があるダウンロードをブロックする' (2) に設定すると、危険の可能性があるダウンロードを示す Microsoft Defender SmartScreen の警告が表示される場合にダウンロードがブロックされ、それ以外の場合はすべてのダウンロードが許可されます。

.すべてのダウンロードをブロックする' (3) に設定すると、すべてのダウンロードがブロックされます。

このポリシーを構成しなかった場合または '特別な制限なし' (0) オプションに設定した場合、Microsoft Defender SmartScreen の分析結果に基づいて、ダウンロードでは通常のセキュリティ制限が適用されます。

こうした制限は、Web ページのコンテンツや [ダウンロード リンク...] コンテキスト メニュー オプションからのダウンロードに適用されます。ただし、現在表示されているページの保存やダウンロードには適用されません。また、印刷オプションの [PDF として保存] オプションにも適用されません。

Microsoft Defender SmartScreen の詳細については、[https://go.microsoft.com/fwlink/?linkid=2094934](https://go.microsoft.com/fwlink/?linkid=2094934) を参照してください。

* 0 = 特別な制限なし

* 1 = 危険なダウンロードをブロックする

* 2 = 危険性があるダウンロードをブロックする

* 3 = すべてのダウンロードをブロックする

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: はい
  - 動的ポリシーの更新: はい

  #### データ型:
  整数

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: DownloadRestrictions
  - GP の名前: ダウンロードの制限を許可する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): 管理用テンプレート/Microsoft Edge - 既定の設定 (ユーザーはオーバーライドできます)/
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): SOFTWARE\Policies\Microsoft\Edge\おすすめ
  - 値の名前: DownloadRestrictions
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000002
```


  #### Mac の情報と設定
  - 優先されるキーの名前: DownloadRestrictions
  - サンプル値:
``` xml
<integer>2</integer>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### EdgeCollectionsEnabled
  #### コレクション機能を有効にする
  >サポートされているバージョン: Windows および Mac (バージョン 78 以降) の Microsoft Edge

  #### 説明
  ユーザーがコレクション機能にアクセスして、コンテンツの収集、整理、共有、およびエクスポートをより効率的に Office 統合を使用して行うことができるようになります。

このポリシーを有効にした場合、または構成しなかった場合、ユーザーは Microsoft Edge のコレクション機能にアクセスして使用することができます。

このポリシーを無効にした場合は、ユーザーは Microsoft Edge のコレクション機能にアクセスして使用できません。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: いいえ - ブラウザーの再起動が必要です

  #### データ型:
  ブール値

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: EdgeCollectionsEnabled
  - GP の名前: コレクション機能を有効にする
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: EdgeCollectionsEnabled
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000001
```


  #### Mac の情報と設定
  - 優先されるキーの名前: EdgeCollectionsEnabled
  - サンプル値:
``` xml
<true/>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### EditFavoritesEnabled
  #### ユーザーによるお気に入りの編集を許可する
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  このポリシーを有効にした場合、ユーザーはお気に入りの追加、削除、変更を行うことができます。これは、ポリシーを構成しなかった場合の既定の動作です。

このポリシーを無効にした場合、ユーザーはお気に入りの追加、削除、変更を行うことができなくなります。ただし、既存のお気に入りは引き続き使用できます。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  ブール値

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: EditFavoritesEnabled
  - GP の名前: ユーザーによるお気に入りの編集を許可する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: EditFavoritesEnabled
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000000
```


  #### Mac の情報と設定
  - 優先されるキーの名前: EditFavoritesEnabled
  - サンプル値:
``` xml
<false/>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### EnableDeprecatedWebPlatformFeatures
  #### 制限された期間、非推奨の Web プラットフォーム機能を再度有効にする
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  一時的にもう一度有効にすることができる、非推奨の Web プラットフォーム機能のリストを指定します。

このポリシーを使用すると、限定された期間内であれば非推奨の Web プラットフォーム機能をもう一度有効にできます。機能は文字列タグで識別されます。

このポリシーを構成しないと、リストが空の場合、またはサポートされる文字列タグのいずれにも機能が一致しない場合は、すべての非推奨の Web プラットフォーム機能は無効のままとなります。

ポリシー自体は上記のプラットフォームでサポートされますが、このポリシーで有効になる機能は、一部のプラットフォームでは利用できない場合があります。一部の非推奨の Web プラットフォーム機能は、もう一度有効にすることはできません。もう一度有効にできるのは、下記のリストに明示的に指定されている機能のみで、有効にできる期間は限定されています。この期間は機能によって異なります。Web プラットフォーム機能の変更の背景にある目的については、https://bit.ly/blinkintents で確認できます。

文字列タグの一般的な形式は [DeprecatedFeatureName]_EffectiveUntil[yyyymmdd] です。

* "ExampleDeprecatedFeature_EffectiveUntil20080902" = ExampleDeprecatedFeature API は 2008 年 9 月 2 日まで有効にできます

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  文字列の一覧

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: EnableDeprecatedWebPlatformFeatures
  - GP の名前: 制限された期間、非推奨の Web プラットフォーム機能を再度有効にする
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge\EnableDeprecatedWebPlatformFeatures
  - パス (おすすめ): N/A
  - 値の名前: 1, 2, 3, ...
  - 値の種類: REG_SZ の一覧
  ##### サンプル値:
```
SOFTWARE\Policies\Microsoft\Edge\EnableDeprecatedWebPlatformFeatures\0 = "ExampleDeprecatedFeature_EffectiveUntil20080902"

```


  #### Mac の情報と設定
  - 優先されるキーの名前: EnableDeprecatedWebPlatformFeatures
  - サンプル値:
``` xml
<array>
  <string>ExampleDeprecatedFeature_EffectiveUntil20080902</string>
</array>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### EnableDomainActionsDownload
  #### マイクロソフトからのドメイン アクションのダウンロードを有効にする
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  Microsoft Edge では、ドメイン アクションとは、ブラウザーが Web 上で正常に動作するのに役立つ一連の互換性機能です。

マイクロソフトでは、互換性の理由から、特定のドメインで実行するアクションの一覧を保持しています。たとえば、ブラウザーは Microsoft Edge での新しいユーザー エージェント文字列によって Web サイトが破損した場合、Web サイト上のユーザー エージェント文字列を上書きする場合があります。これらの操作は一時的なものであり、この間にマイクロソフトではサイト所有者と問題解決に当たります。

ブラウザーが起動し、その後定期的に実行されると、ブラウザーは、実行する互換性操作の最新の一覧がある [実験および構成サービス] に接続します。この一覧は、最初に取得された後、サーバーのコピーが変更された場合にのみ後続の要求で一覧が更新されるように、ローカルで保存されます。

このポリシーを有効にした場合、ドメイン アクションの一覧は引き続き [実験および構成サービス] からダウンロードされます。

このポリシーを無効にすると、ドメイン アクションの一覧は [実験および構成サービス] からダウンロードされなくなります。

このポリシーを構成しなかった場合、ドメイン アクションの一覧は引き続き [実験および構成サービス] からダウンロードされます。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  ブール値

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: EnableDomainActionsDownload
  - GP の名前: マイクロソフトからのドメイン アクションのダウンロードを有効にする
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: EnableDomainActionsDownload
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000001
```


  #### Mac の情報と設定
  - 優先されるキーの名前: EnableDomainActionsDownload
  - サンプル値:
``` xml
<true/>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### EnableOnlineRevocationChecks
  #### オンライン OCSP/CRL チェックを有効にする
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  オンライン失効チェックでは、セキュリティ上の重要なメリットが実現されず、既定では無効になっています。

このポリシーを有効にした場合、Microsoft Edge ではソフト フェイルのオンライン OCSP/CRL チェックが実行されます。"ソフト フェイル" とは、失効サーバーにアクセスできない場合に、証明書が有効と見なされることを意味します。

このポリシーを無効にした場合または構成しなかった場合、Microsoft Edge ではオンライン失効チェックが実行されません。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  ブール値

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: EnableOnlineRevocationChecks
  - GP の名前: オンライン OCSP/CRL チェックを有効にする
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: EnableOnlineRevocationChecks
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000000
```


  #### Mac の情報と設定
  - 優先されるキーの名前: EnableOnlineRevocationChecks
  - サンプル値:
``` xml
<false/>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### EnterpriseHardwarePlatformAPIEnabled
  #### 管理された拡張機能を有効にして、エンタープライズ ハードウェア プラットフォーム API を使用する
  >サポートされているバージョン: Windows および Mac (バージョン 78 以降) の Microsoft Edge

  #### 説明
  このポリシーが有効に設定されていると、エンタープライズ ポリシーによってインストールされた拡張機能では、エンタープライズ ハードウェア プラットフォーム API を使用できます。
このポリシーが無効に設定されているか、設定されていない場合、どの拡張機能もエンタープライズ ハードウェア プラットフォーム API を使用できません。
このポリシーは、コンポーネント拡張機能にも適用されます。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  ブール値

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: EnterpriseHardwarePlatformAPIEnabled
  - GP の名前: 管理された拡張機能を有効にして、エンタープライズ ハードウェア プラットフォーム API を使用する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: EnterpriseHardwarePlatformAPIEnabled
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000001
```


  #### Mac の情報と設定
  - 優先されるキーの名前: EnterpriseHardwarePlatformAPIEnabled
  - サンプル値:
``` xml
<true/>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### ExperimentationAndConfigurationServiceControl
  #### 実験および構成サービスとの通信を制御する
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  Microsoft Edge では、実験および構成サービスを使用して実験および構成ペイロードを展開します。

実験ペイロードは、Microsoft がテストおよびフィードバックを有効にしている新しい開発機能のリストで構成されています。

構成ペイロードは、ユーザー エクスペリエンスを最適化するために Microsoft が Microsoft Edge に展開する設定のリストで構成されています。たとえば、構成ペイロードは、最新のペイロードを取得するために Microsoft Edge が実験および構成サービスに要求を送信する頻度を指定できます。

このポリシーを "構成と実験の取得" モードに設定した場合、ペイロード全体は実験および構成サービスからダウンロードされます。これには、実験ペイロードと構成ペイロードの両方が含まれます。

このポリシーを "構成のみを取得する" モードに設定した場合、構成ペイロードのみが提供されます。

このポリシーを "実験および構成サービスとの通信を無効にする" モードに設定した場合、実験および構成サービスとの通信は完全に停止します。

このポリシーを構成しなかった場合、安定版のチャネルとベータ版のチャネルのマネージド デバイスでは、動作が "構成のみを取得する" モードと同じになります。

このポリシーを構成しなかった場合、アンマネージド デバイスでは、動作が "構成と実験の取得" モードと同じになります。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  整数

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: ExperimentationAndConfigurationServiceControl
  - GP の名前: 実験および構成サービスとの通信を制御する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: ExperimentationAndConfigurationServiceControl
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000002
```


  #### Mac の情報と設定
  - 優先されるキーの名前: ExperimentationAndConfigurationServiceControl
  - サンプル値:
``` xml
<integer>2</integer>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### ExternalProtocolDialogShowAlwaysOpenCheckbox
  #### 外部プロトコルのダイアログで [常に開く] チェック ボックスを表示します。
  >サポートされているバージョン: Windows および Mac (バージョン 79 以降) の Microsoft Edge

  #### 説明
  このポリシーでは、外部プロトコルの起動確認プロンプトに [常に開く] チェック ボックスを表示するかどうかを制御します。

このポリシーを True に設定した場合、外部プロトコルの確認プロンプトが表示されたときに、ユーザーは [常に開く] を選択できます。今後、ユーザーに対してこのプロトコルの確認プロンプトは表示されなくなります。

このポリシーを False に設定した場合またはこのポリシーを設定しなかった場合、[常に開く] チェック ボックスは表示されません。外部プロトコルを呼び出すたびに、ユーザーは確認を求められます。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: いいえ - ブラウザーの再起動が必要です

  #### データ型:
  ブール値

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: ExternalProtocolDialogShowAlwaysOpenCheckbox
  - GP の名前: 外部プロトコルのダイアログで [常に開く] チェック ボックスを表示します。
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: ExternalProtocolDialogShowAlwaysOpenCheckbox
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000001
```


  #### Mac の情報と設定
  - 優先されるキーの名前: ExternalProtocolDialogShowAlwaysOpenCheckbox
  - サンプル値:
``` xml
<true/>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### FavoritesBarEnabled
  #### お気に入りバーを有効にする
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  お気に入りバーを有効または無効にします。

このポリシーを有効にすると、ユーザーにはお気に入りバーが表示されます。

このポリシーを無効にした場合、お気に入りバーはユーザーに表示されません。

このポリシーが構成されていない場合、ユーザーはお気に入りバーを使用するかどうかを選択できます。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: はい
  - 動的ポリシーの更新: はい

  #### データ型:
  ブール値

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: FavoritesBarEnabled
  - GP の名前: お気に入りバーを有効にする
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): 管理用テンプレート/Microsoft Edge - 既定の設定 (ユーザーはオーバーライドできます)/
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): SOFTWARE\Policies\Microsoft\Edge\おすすめ
  - 値の名前: FavoritesBarEnabled
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000001
```


  #### Mac の情報と設定
  - 優先されるキーの名前: FavoritesBarEnabled
  - サンプル値:
``` xml
<true/>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### ForceBingSafeSearch
  #### Bing セーフサーチを適用する
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  Bing Web Search でのクエリが、指定された値に設定されたセーフサーチに基づいて実行されるようにします。ユーザーはこの設定を変更できません。

このポリシーを "オフ" に構成すると、Bing Search のセーフサーチは Bing.com の値に戻ります。

このポリシーを "中程度" に構成すると、セーフサーチで中程度の設定が使用されます。中程度の設定では、検索結果で成人向けのビデオと画像がフィルターされますが、テキストはフィルターされません。

このポリシーを "厳密" に構成すると、セーフサーチで厳密な設定が使用されます。厳密な設定では、成人向けのテキスト、画像、ビデオがフィルターされます。

このポリシーを無効にした場合または構成しなかった場合、Bing Search のセーフサーチは適用されず、ユーザーは Bing.com で必要な値を設定できます。

* 0 = Bing で検索制限を構成しない

* 1 = Bing で中程度の検索制限を構成する

* 2 = Bing で厳密な検索制限を構成する

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  整数

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: ForceBingSafeSearch
  - GP の名前: Bing セーフサーチを適用する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: ForceBingSafeSearch
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000000
```


  #### Mac の情報と設定
  - 優先されるキーの名前: ForceBingSafeSearch
  - サンプル値:
``` xml
<integer>0</integer>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### ForceEphemeralProfiles
  #### 一時プロファイルの使用を有効にする
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  ユーザー プロファイルを 一時モードに切り替えるかどうかを制御します。一時プロファイルは、セッションの開始時に作成され、セッションの終了時に削除されます。

このポリシーを有効にした場合、プロファイルは一時モードで実行されます。これにより、ユーザーはデバイスに閲覧データを保存しなくても、使用しているデバイスから作業を行うことができます。このポリシーを (Windows の GPO を使用するなどして) OS ポリシーとして有効にすると、システム上のすべてのプロファイルに適用されます。

このポリシーを無効にした場合、または構成しなかった場合、ユーザーにはブラウザーへのサインイン時に標準プロファイルが適用されます。

一時モードでは、ユーザー セッションの間のみプロファイル データがディスクに保存されます。ブラウザーの履歴、拡張機能とそのデータ、Cookie のような Web データ、また Web データベースなどの機能は、ブラウザーを閉じた後には保存されません。ユーザーはディスクに手動でデータをダウンロードしたり、ページを保存または印刷したりすることはできます。ユーザーが同期を有効にしている場合は、標準プロファイルと同様に、すべてのデータが同期アカウントに保持されます。明示的に無効にしていない限り、ユーザーは InPrivate ブラウズを一時モードで使用することもできます。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: いいえ - ブラウザーの再起動が必要です

  #### データ型:
  ブール値

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: ForceEphemeralProfiles
  - GP の名前: 一時プロファイルの使用を有効にする
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: ForceEphemeralProfiles
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000001
```


  #### Mac の情報と設定
  - 優先されるキーの名前: ForceEphemeralProfiles
  - サンプル値:
``` xml
<true/>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### ForceGoogleSafeSearch
  #### Google セーフサーチを適用する
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  セーフサーチをアクティブに設定して実行される Google Web 検索でクエリを適用し、ユーザーがこの設定を変更できないようにします。

このポリシーを有効にした場合、Google 検索のセーフサーチは常にアクティブになります。

この設定を無効にした場合または構成しなかった場合、Google 検索のセーフサーチは適用されません。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  ブール値

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: ForceGoogleSafeSearch
  - GP の名前: Google セーフサーチを適用する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: ForceGoogleSafeSearch
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000000
```


  #### Mac の情報と設定
  - 優先されるキーの名前: ForceGoogleSafeSearch
  - サンプル値:
``` xml
<false/>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### ForceNetworkInProcess
  #### ブラウザー プロセスでネットワーク コードを強制的に実行する
  >サポートされているバージョン: Windows (バージョン 78 以降) の Microsoft Edge

  #### 説明
  このポリシーは、ブラウザー プロセスでネットワーク コードを強制的に実行します。

既定では、このポリシーは無効になっています。有効にした場合、ネットワーク プロセスがサンドボックス化されると、ユーザーがセキュリティの問題さらされる可能性があります。

このポリシーの目的は、企業がネットワーク API のフックに依存しないサード パーティのソフトウェアへ移行できるようにすることです。プロキシ サーバーは、LSP および Win32 API パッチ経由にすることをお勧めします。

このポリシーを設定しなかった場合、ネットワーク コードは、NetworkService 実験のフィールド トライアルに応じて、ブラウザー プロセスの外部で実行される可能性があります。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: いいえ - ブラウザーの再起動が必要です

  #### データ型:
  ブール値

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: ForceNetworkInProcess
  - GP の名前: ブラウザー プロセスでネットワーク コードを強制的に実行する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: ForceNetworkInProcess
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000000
```


  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### ForceYouTubeRestrict
  #### 最小限の YouTube の制限モードを強制する
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  YouTube に最小限の制限モードを強制し、それより制限の少ないモードをユーザーが選択できないようにします。

[制限 (2)] に設定すると、YouTube で厳格な制限モードを強制します。

[中 (1)] に設定すると、YouTube で中程度の制限モードと厳格な制限モードのみの使用をユーザーに強制します。ユーザーは制限モードを無効にすることはできません。

このポリシーが [オフ (0)] に設定されているか、構成していない場合は、YouTube で制限モードを強制しません。YouTube ポリシーなどの外部ポリシーで、制限モードが引き続き適用される場合があります。

* 0 = YouTube で制限モードを強制しない

* 1 = YouTube で少なくとも中程度の制限モードを強制する

* 2 = YouTube で厳格な制限モードを強制する

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  整数

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: ForceYouTubeRestrict
  - GP の名前: 最小限の YouTube の制限モードを強制する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: ForceYouTubeRestrict
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000000
```


  #### Mac の情報と設定
  - 優先されるキーの名前: ForceYouTubeRestrict
  - サンプル値:
``` xml
<integer>0</integer>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### FullscreenAllowed
  #### 全画面表示モードを許可する
  >サポートされているバージョン: Windows (バージョン 77 以降) の Microsoft Edge

  #### 説明
  全画面表示モードを使用できるかどうかを設定します。この表示モードでは、すべての Microsoft Edge の UI が非表示になり、Web コンテンツのみが表示されます。

このポリシーを有効にした場合または構成しなかった場合、適切なアクセス許可を持つユーザー、アプリ、拡張機能を全画面表示モードに切り替えることができます。

このポリシーを無効にした場合、ユーザー、アプリ、拡張機能は全画面表示モードに切り替えることはできません。

全画面表示モードが無効になっていると、コマンド ラインを使用してMicrosoft Edge をキオスク モードで開くことはできません。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  ブール値

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: FullscreenAllowed
  - GP の名前: 全画面表示モードを許可する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: FullscreenAllowed
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000001
```


  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### GoToIntranetSiteForSingleWordEntryInAddressBar
  #### アドレス バーへの 1 単語の入力で検索するのではなく、ダイレクト イントラネット サイト ナビゲーションを強制します
  >サポートされているバージョン: Windows および Mac (バージョン 78 以降) の Microsoft Edge

  #### 説明
  このポリシーを有効にした場合、アドレス バーの候補リストで先頭に示される自動提案の結果によって、イントラネット サイトに移動されます (アドレス バーに入力されたテキストが句読点を含まない 1 単語であるとき)。

句読点を含まない 1 単語を入力したときの既定のナビゲーションでは、入力したテキストに一致するイントラネット サイトへの移動が実施されます。

このポリシーを有効にした場合、アドレス バーの候補リストに示される自動提案の 2 番目の結果によって、入力されたとおりに Web 検索が実施されます (入力されたテキストが句読点を含まない 1 単語であるとき)。Web 検索を禁止するポリシーが有効になっている場合を除き、既定の検索プロバイダーが使用されます。

このポリシーを有効にした場合の 2 つの効果は次のとおりです。

履歴の項目に通常解決される 1 単語のクエリに対応するサイトへのナビゲーションは、実施されなくなります。代わりに、ブラウザーは、組織のイントラネットに存在しない可能性がある内部サイトへ移動しようとします。この結果、404 エラーが発生します。

よく使用される 1 単語の検索語句では、検索を適切に実行するために検索候補の手動選択が必要になります。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  ブール値

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: GoToIntranetSiteForSingleWordEntryInAddressBar
  - GP の名前: アドレス バーへの 1 単語の入力で検索するのではなく、ダイレクト イントラネット サイト ナビゲーションを強制します
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: GoToIntranetSiteForSingleWordEntryInAddressBar
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000000
```


  #### Mac の情報と設定
  - 優先されるキーの名前: GoToIntranetSiteForSingleWordEntryInAddressBar
  - サンプル値:
``` xml
<false/>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### HSTSPolicyBypassList
  #### HSTS ポリシー チェックをバイパスする名前の一覧を構成します
  >サポートされているバージョン: Windows および Mac (バージョン 79 以降) の Microsoft Edge

  #### 説明
  この一覧に指定されたホスト名は、"http://" からの要求を "https://" にアップグレードする可能性がある HSTS ポリシー チェックから除外されます。このポリシーでは、単一ラベルのホスト名のみが許可されます。ホスト名は正規化する必要があります。IDN は A-ラベル形式に変換する必要があり、ASCII 文字はすべて小文字にする必要があります。このポリシーは指定された特定のホスト名にのみ適用され、一覧に含まれる名前のサブドメインには適用されません。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: いいえ - ブラウザーの再起動が必要です

  #### データ型:
  文字列の一覧

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: HSTSPolicyBypassList
  - GP の名前: HSTS ポリシー チェックをバイパスする名前の一覧を構成します
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge\HSTSPolicyBypassList
  - パス (おすすめ): N/A
  - 値の名前: 1, 2, 3, ...
  - 値の種類: REG_SZ の一覧
  ##### サンプル値:
```
SOFTWARE\Policies\Microsoft\Edge\HSTSPolicyBypassList\0 = "meet"

```


  #### Mac の情報と設定
  - 優先されるキーの名前: HSTSPolicyBypassList
  - サンプル値:
``` xml
<array>
  <string>meet</string>
</array>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### HardwareAccelerationModeEnabled
  #### 使用可能な場合はハードウェア アクセラレータを使用する
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  ハードウェア アクセラレータが使用可能な場合は、これを使用するように指定します。このポリシーを有効にした場合または構成しなかった場合、GPU 機能が明示的にブロックされていない限り、ハードウェア アクセラレータが有効になります。

このポリシーを無効にした場合、ハードウェア アクセラレータは無効になります。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: いいえ - ブラウザーの再起動が必要です

  #### データ型:
  ブール値

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: HardwareAccelerationModeEnabled
  - GP の名前: 使用可能な場合はハードウェア アクセラレータを使用する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: HardwareAccelerationModeEnabled
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000001
```


  #### Mac の情報と設定
  - 優先されるキーの名前: HardwareAccelerationModeEnabled
  - サンプル値:
``` xml
<true/>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### ImportAutofillFormData
  #### オートフィルのフォーム データのインポートを許可する
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  ユーザーは、オートフィルのフォーム データを別のブラウザーから Microsoft Edge にインポートできます。

このポリシーを有効にした場合、オートフィルのフォーム データを手動でインポートするオプションが自動的に選択されます。

このポリシーを無効にした場合、オートフィルのフォーム データは初回実行時にインポートされず、またユーザーは手動でインポートすることもできません。

このポリシーを構成しなかった場合、オートフィルのデータは初回実行時にインポートされます。ユーザーは、後で閲覧セッションを実行しているときに、このデータを手動でインポートするかどうかを選択できます。

このポリシーは推奨事項として設定できます。つまり、Microsoft Edge では、初回起動時にオートフィルのデータがインポートされますが、ユーザーは、手動でインポートする際に **オートフィルのデータ** に関するオプションを選択したり、クリアしたりすることができます。

**注意**: 現在このポリシーでは、Google Chrome (Windows 7、8、10、および macOS) からのインポートを管理します。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: はい
  - 動的ポリシーの更新: はい

  #### データ型:
  ブール値

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: ImportAutofillFormData
  - GP の名前: オートフィルのフォーム データのインポートを許可する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): 管理用テンプレート/Microsoft Edge - 既定の設定 (ユーザーはオーバーライドできます)/
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): SOFTWARE\Policies\Microsoft\Edge\おすすめ
  - 値の名前: ImportAutofillFormData
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000001
```


  #### Mac の情報と設定
  - 優先されるキーの名前: ImportAutofillFormData
  - サンプル値:
``` xml
<true/>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### ImportBrowserSettings
  #### ブラウザーの設定のインポートを許可する
  >サポートされているバージョン: Windows および Mac (バージョン 78 以降) の Microsoft Edge

  #### 説明
  ユーザーは、ブラウザーの設定を別のブラウザーから Microsoft Edge にインポートできます。

このポリシーを有効にした場合、**[ブラウザー データのインポート]** ダイアログ ボックスにある **[ブラウザーの設定]** チェック ボックスが自動的に選択されます。

このポリシーを無効にした場合、ブラウザーの設定は初回実行時にインポートされず、またユーザーは手動でインポートすることもできません。

このポリシーを構成しなかった場合、ブラウザーの設定は初回実行時にインポートされます。ユーザーは、後で閲覧セッションを実行しているときに、ブラウザーの設定を手動でインポートするかどうかを選択できます。

このポリシーは推奨事項として設定できます。つまり、Microsoft Edge では、初回起動時にブラウザーの設定がインポートされますが、ユーザーは、手動でインポートする際に**ブラウザーの設定**に関するオプションを選択したり、クリアしたりすることができます。

**注意:** 現在このポリシーでは、Google Chrome (Windows 7、8、10、および macOS) からのインポートを管理します。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: はい
  - 動的ポリシーの更新: はい

  #### データ型:
  ブール値

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: ImportBrowserSettings
  - GP の名前: ブラウザーの設定のインポートを許可する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): 管理用テンプレート/Microsoft Edge - 既定の設定 (ユーザーはオーバーライドできます)/
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): SOFTWARE\Policies\Microsoft\Edge\おすすめ
  - 値の名前: ImportBrowserSettings
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000001
```


  #### Mac の情報と設定
  - 優先されるキーの名前: ImportBrowserSettings
  - サンプル値:
``` xml
<true/>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### ImportFavorites
  #### お気に入りのインポートを許可する
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  ユーザーは、お気に入りを別のブラウザーから Microsoft Edge にインポートできます。

このポリシーを有効にした場合、**[ブラウザー データのインポート]** ダイアログ ボックスの **[お気に入り]** チェック ボックスが自動的にオンになります。

このポリシーを無効にした場合、初回実行時にお気に入りはインポートされず、またユーザーはお気に入りを手動でインポートすることもできません。

このポリシーを構成しなかった場合、初回実行時にお気に入りがインポートされます。ユーザーは、後で閲覧セッションを実行しているときに、お気に入りを手動でインポートするかどうかを選択できます。

このポリシーは推奨事項として設定できます。つまり、Microsoft Edge では、初回起動時にお気に入りがインポートされますが、ユーザーは、手動でインポートする際に **お気に入り** に関するオプションを選択したり、クリアしたりすることができます。

**注意**: 現在このポリシーでは、Internet Explorer (Windows 7、8、10)、Google Chrome (Windows 7、8、10、および macOS)、Apple Safari (macOS) の各ブラウザーからのインポートを管理します。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: はい
  - 動的ポリシーの更新: はい

  #### データ型:
  ブール値

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: ImportFavorites
  - GP の名前: お気に入りのインポートを許可する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): 管理用テンプレート/Microsoft Edge - 既定の設定 (ユーザーはオーバーライドできます)/
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): SOFTWARE\Policies\Microsoft\Edge\おすすめ
  - 値の名前: ImportFavorites
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000001
```


  #### Mac の情報と設定
  - 優先されるキーの名前: ImportFavorites
  - サンプル値:
``` xml
<true/>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### ImportHistory
  #### 閲覧の履歴のインポートを許可する
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  ユーザーは、閲覧の履歴を別のブラウザーから Microsoft Edge にインポートできます。

このポリシーを有効にした場合、**[ブラウザー データのインポート]** ダイアログ ボックスの **[閲覧の履歴]** チェック ボックスが自動的にオンになります。

このポリシーを無効にした場合、初回実行時に閲覧の履歴データはインポートされず、またユーザーはこのデータを手動でインポートすることもできません。

このポリシーを構成しなかった場合、初回実行時に閲覧の履歴データがインポートされます。ユーザーは、後で閲覧セッションを実行しているときに、このデータを手動でインポートするかどうかを選択できます

このポリシーは推奨事項として設定できます。つまり、Microsoft Edge では、初回起動時に閲覧の履歴がインポートされますが、ユーザーは、手動でインポートする際に **履歴** に関するオプションを選択したり、クリアしたりすることができます。

**注意**: 現在このポリシーでは、Internet Explorer (Windows 7、8、10)、Google Chrome (Windows 7、8、10、および macOS)、Apple Safari (macOS) の各ブラウザーからのインポートを管理します。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: はい
  - 動的ポリシーの更新: はい

  #### データ型:
  ブール値

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: ImportHistory
  - GP の名前: 閲覧の履歴のインポートを許可する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): 管理用テンプレート/Microsoft Edge - 既定の設定 (ユーザーはオーバーライドできます)/
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): SOFTWARE\Policies\Microsoft\Edge\おすすめ
  - 値の名前: ImportHistory
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000001
```


  #### Mac の情報と設定
  - 優先されるキーの名前: ImportHistory
  - サンプル値:
``` xml
<true/>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### ImportHomepage
  #### ホーム ページの設定のインポートを許可する
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  ユーザーは、ホーム ページの設定を別のブラウザーから Microsoft Edge にインポートできます。

このポリシーを有効にした場合、ホーム ページの設定を手動でインポートするオプションが自動的に選択されます。

このポリシーを無効にした場合、ホーム ページの設定は初回実行時にインポートされず、またユーザーは手動でインポートすることもできません。

このポリシーを構成しなかった場合、ホーム ページの設定は初回実行時にインポートされます。ユーザーは、後で閲覧セッションを実行しているときに、このデータを手動でインポートするかどうかを選択できます。

このポリシーは推奨事項として設定できます。つまり、Microsoft Edge では、初回起動時にホーム ページの設定がインポートされますが、ユーザーは、手動でインポートする際に **ホーム ページ** に関するオプションを選択したり、クリアしたりすることができます。

**注意**: 現在このポリシーでは、Internet Explorer (Windows 7、8、10) からのインポートを管理します。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  ブール値

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: ImportHomepage
  - GP の名前: ホーム ページの設定のインポートを許可する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: ImportHomepage
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000001
```


  #### Mac の情報と設定
  - 優先されるキーの名前: ImportHomepage
  - サンプル値:
``` xml
<true/>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### ImportOpenTabs
  #### 開いているタブのインポートを許可する
  >サポートされているバージョン: Windows および Mac (バージョン 79 以降) の Microsoft Edge

  #### 説明
  ユーザーは、開いているタブやピン留めされたタブを別のブラウザーから Microsoft Edge にインポートできます。

このポリシーを有効にした場合、**[ブラウザー データのインポート]** ダイアログ ボックスにある **[開いているタブ]** チェック ボックスが自動的にオンになります。

このポリシーを無効にした場合、開いているタブは初回実行時にインポートされず、またユーザーは手動でインポートすることもできません。

このポリシーを構成しなかった場合、開いているタブは初回実行時にインポートされます。ユーザーは、後で閲覧セッションを実行しているときに、開いているタブを手動でインポートするかどうかを選択できます。

このポリシーは推奨事項として設定できます。つまり、Microsoft Edge では、開いているタブが初回起動時にインポートされますが、ユーザーは、手動でインポートする際に **[開いているタブ]** オプションをオンにしたり、オフにしたりすることができます。

**注意:** 現在このポリシーでは、Google Chrome (Windows 7、8、10、および macOS) からのインポートのみをサポートします。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: はい
  - 動的ポリシーの更新: はい

  #### データ型:
  ブール値

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: ImportOpenTabs
  - GP の名前: 開いているタブのインポートを許可する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): 管理用テンプレート/Microsoft Edge - 既定の設定 (ユーザーはオーバーライドできます)/
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): SOFTWARE\Policies\Microsoft\Edge\おすすめ
  - 値の名前: ImportOpenTabs
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000001
```


  #### Mac の情報と設定
  - 優先されるキーの名前: ImportOpenTabs
  - サンプル値:
``` xml
<true/>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### ImportPaymentInfo
  #### 支払情報のインポートを許可する
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  ユーザーは、支払情報を別のブラウザーから Microsoft Edge にインポートできます。

このポリシーを有効にした場合、**[ブラウザー データのインポート]** ダイアログ ボックスにある **[支払情報]** チェック ボックスが自動的に選択されます。

このポリシーを無効にした場合、支払情報は初回実行時にインポートされず、またユーザーは手動でインポートすることもできません。

このポリシーを構成しなかった場合、支払情報は初回実行時にインポートされます。ユーザーは、後で閲覧セッションを実行しているときに、支払情報を手動でインポートするかどうかを選択できます。

このポリシーは推奨事項として設定できます。つまり、Microsoft Edge では、初回起動時に支払情報がインポートされますが、ユーザーは、手動でインポートする際に **支払情報** に関するオプションを選択したり、クリアしたりすることができます。

**注意:** 現在このポリシーでは、Google Chrome (Windows 7、8、10、および macOS) からのインポートを管理します。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: はい
  - 動的ポリシーの更新: はい

  #### データ型:
  ブール値

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: ImportPaymentInfo
  - GP の名前: 支払情報のインポートを許可する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): 管理用テンプレート/Microsoft Edge - 既定の設定 (ユーザーはオーバーライドできます)/
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): SOFTWARE\Policies\Microsoft\Edge\おすすめ
  - 値の名前: ImportPaymentInfo
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000001
```


  #### Mac の情報と設定
  - 優先されるキーの名前: ImportPaymentInfo
  - サンプル値:
``` xml
<true/>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### ImportSavedPasswords
  #### 保存したパスワードのインポートを許可する
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  ユーザーは、保存したパスワードを別のブラウザーから Microsoft Edge にインポートできます。

このポリシーを有効にした場合、保存したパスワードを手動でインポートするオプションが自動的に選択されます。

このポリシーを無効にした場合、保存したパスワードは初回実行時にインポートされず、またユーザーは手動でインポートすることもできません。

このポリシーを構成しなかった場合、パスワードは初回実行時にインポートされます。ユーザーは、後で閲覧セッションを実行しているときに、パスワードを手動でインポートするかどうかを選択できます

このポリシーは推奨事項として設定できます。つまり、Microsoft Edge では、初回起動時にパスワードがインポートされますが、ユーザーは、手動でインポートする際に **パスワード** に関するオプションを選択したり、クリアしたりすることができます。

**注意**: 現在このポリシーでは、Internet Explorer (Windows 7、8、10) と Google Chrome (Windows 7、8、10、および macOS) の各ブラウザーからのインポートを管理します。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: はい
  - 動的ポリシーの更新: はい

  #### データ型:
  ブール値

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: ImportSavedPasswords
  - GP の名前: 保存したパスワードのインポートを許可する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): 管理用テンプレート/Microsoft Edge - 既定の設定 (ユーザーはオーバーライドできます)/
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): SOFTWARE\Policies\Microsoft\Edge\おすすめ
  - 値の名前: ImportSavedPasswords
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000001
```


  #### Mac の情報と設定
  - 優先されるキーの名前: ImportSavedPasswords
  - サンプル値:
``` xml
<true/>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### ImportSearchEngine
  #### 検索エンジンの設定のインポートを許可する
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  ユーザーは、検索エンジンの設定を別のブラウザーから Microsoft Edge にインポートできます。

このポリシーを有効にした場合、検索エンジンの設定を手動でインポートするオプションが自動的に選択されます。

このポリシーを無効にした場合、検索エンジンの設定は初回実行時にインポートされず、またユーザーは手動でインポートすることもできません。

このポリシーを構成しなかった場合、検索エンジンの設定は初回実行時にインポートされます。ユーザーは、後で閲覧セッションを実行しているときに、このデータを手動でインポートするかどうかを選択できます。

このポリシーは推奨事項として設定できます。つまり、Microsoft Edge では、初回起動時に検索エンジンの設定がインポートされますが、ユーザーは、手動でインポートする際に **検索エンジンの設定** に関するオプションを選択したり、クリアしたりすることができます。

**注意**: 現在このポリシーでは、Internet Explorer (Windows 7、8、10) からのインポートを管理します。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: はい
  - 動的ポリシーの更新: はい

  #### データ型:
  ブール値

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: ImportSearchEngine
  - GP の名前: 検索エンジンの設定のインポートを許可する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): 管理用テンプレート/Microsoft Edge - 既定の設定 (ユーザーはオーバーライドできます)/
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): SOFTWARE\Policies\Microsoft\Edge\おすすめ
  - 値の名前: ImportSearchEngine
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000001
```


  #### Mac の情報と設定
  - 優先されるキーの名前: ImportSearchEngine
  - サンプル値:
``` xml
<true/>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### InPrivateModeAvailability
  #### InPrivate モードが利用できるかどうかを構成する
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  ユーザーが Microsoft Edge で InPrivate モードを使用してページを開くことができるかどうかを指定します。

このポリシーを構成しなかった場合または '有効' (0) に設定した場合、ユーザーは InPrivate モードでページを開くことができます。

このポリシーを '無効' (1) に設定した場合、ユーザーは InPrivate モードを使用できません。

このポリシーを '強制' (2) に設定した場合、常に InPrivate モードが使用されます。

* 0 = InPrivate モードを利用可能にする

* 1 = InPrivate モードを無効にする

* 2 = InPrivate モードを強制的に適用する

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  整数

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: InPrivateModeAvailability
  - GP の名前: InPrivate モードが利用できるかどうかを構成する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: InPrivateModeAvailability
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000001
```


  #### Mac の情報と設定
  - 優先されるキーの名前: InPrivateModeAvailability
  - サンプル値:
``` xml
<integer>1</integer>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### InternetExplorerIntegrationLevel
  #### Internet Explorer 統合を構成する
  >サポートされているバージョン: Windows (バージョン 77 以降) の Microsoft Edge

  #### 説明
  Internet Explorer モードに最適なエクスペリエンスを構成するガイダンスについては、[https://go.microsoft.com/fwlink/?linkid=2094210](https://go.microsoft.com/fwlink/?linkid=2094210) を参照してください

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: いいえ - ブラウザーの再起動が必要です

  #### データ型:
  整数

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: InternetExplorerIntegrationLevel
  - GP の名前: Internet Explorer 統合を構成する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: InternetExplorerIntegrationLevel
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000001
```


  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### InternetExplorerIntegrationSiteList
  #### エンタープライズ モード サイト一覧を構成する
  >サポートされているバージョン: Windows (バージョン 78 以降) の Microsoft Edge

  #### 説明
  Internet Explorer モードに最適なエクスペリエンスを構成するガイダンスについては、[https://go.microsoft.com/fwlink/?linkid=2094210](https://go.microsoft.com/fwlink/?linkid=2094210) を参照してください

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: いいえ - ブラウザーの再起動が必要です

  #### データ型:
  文字列

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: InternetExplorerIntegrationSiteList
  - GP の名前: エンタープライズ モード サイト一覧を構成する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: InternetExplorerIntegrationSiteList
  - 値の種類: REG_SZ
  ##### サンプル値:
```
"https://internal.contoso.com/sitelist.xml"
```


  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### InternetExplorerIntegrationSiteRedirect
  #### Internet Explorer モードのページから開始した場合、未構成のサイトへの "ページ内" ナビゲーションがどのように動作するかを指定する
  >サポートされているバージョン: Windows (バージョン 79 以降) の Microsoft Edge

  #### 説明
  "ページ内" ナビゲーションは、現在のページ上にあるリンク、スクリプト、またはフォームから始まります。また "ページ内" ナビゲーションが、前回行った "ページ内" ナビゲーションのサーバー側リダイレクトになる場合もあります。これに対して、ユーザーは、ブラウザー コントロールを使用したいくつかの方法で、現在のページに依存しない "ページ内" 以外のナビゲーションを開始することができます。たとえば、アドレス バー、[戻る] ボタン、またはお気に入りのリンクを使用します。

この設定では、Internet Explorer モードで読み込まれたページから未構成のサイト (エンタープライズ モード サイト一覧に構成されていないサイト) へのナビゲーションを Microsoft Edge に戻すか、Internet Explorer モードのままにしておくかどうかを指定できます。

この設定は、以下の操作と連動して機能します:
[InternetExplorerIntegrationLevel](#internetexplorerintegrationlevel) を "Internet Explorer モード" (1) に設定する
および
エンタープライズ モード サイト一覧に少なくとも 1 つのエントリが含まれるように、[InternetExplorerIntegrationSiteList](#internetexplorerintegrationsitelist) ポリシーを構成する

このポリシーを無効にした場合または構成しなかった場合、Internet Explorer モードで開くように構成されたサイトのみが、そのモードで開きます。Internet Explorer モードで開くように構成されていないサイトは、Microsoft Edge にリダイレクトされます。

このポリシーを有効にした場合、次のいずれかのナビゲーション オプションを選択できます。
0 - 既定値。Internet Explorer モードで開くように構成されたサイトのみが、そのモードで開きます。Internet Explorer モードで開くように構成されていないサイトは、Microsoft Edge にリダイレクトされます。
1 - 自動ナビゲーションのみが Internet Explorer モードで維持されます。既定のエクスペリエンスを Internet Explorer モードで維持する場合は、このオプションを使用します。ただし、未構成のサイトへの自動ナビゲーション (302 リダイレクトなど) はすべて、このオプションの対象外となります。
2 - すべてのページ内ナビゲーション が Internet Explorer モードで維持されます (ほとんどの場合に推奨されません)。IE モードで読み込まれたページから未構成のサイトへのすべてのナビゲーションが Internet Explorer モードで維持されます。

Internet Explorer モードの詳細については、[https://go.microsoft.com/fwlink/?linkid=2105106](https://go.microsoft.com/fwlink/?linkid=2105106) をご覧ください

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: いいえ - ブラウザーの再起動が必要です

  #### データ型:
  整数

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: InternetExplorerIntegrationSiteRedirect
  - GP の名前: Internet Explorer モードのページから開始した場合、未構成のサイトへの "ページ内" ナビゲーションがどのように動作するかを指定する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: InternetExplorerIntegrationSiteRedirect
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000000
```


  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### IsolateOrigins
  #### 特定の出所に対してサイトの分離を有効にする
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  独自のプロセスで分離して実行されるオリジンを指定します。
またこのポリシーでは、サブドメインによって指定されたオリジンも分離されます。たとえば、https://contoso.com/ と指定すると、https://foo.contoso.com/ が https://contoso.com/ サイトの一部として 分離されます。
このポリシーを有効にした場合、コンマ区切りのリスト内にある指定のオリジンは、それぞれ独自のプロセスで実行されます。
このポリシーを無効にした場合、'IsolateOrigins' 機能と 'SitePerProcess' 機能はどちらも無効になります。ただしユーザーは、コマンド ライン フラグを使用して、手動で 'IsolateOrigins' ポリシーを有効にすることができます。
このポリシーを構成しなかった場合、ユーザーはこの設定を変更できます。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: いいえ - ブラウザーの再起動が必要です

  #### データ型:
  文字列

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: IsolateOrigins
  - GP の名前: 特定の出所に対してサイトの分離を有効にする
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: IsolateOrigins
  - 値の種類: REG_SZ
  ##### サンプル値:
```
"https://contoso.com/,https://fabrikam.com/"
```


  #### Mac の情報と設定
  - 優先されるキーの名前: IsolateOrigins
  - サンプル値:
``` xml
<string>https://contoso.com/,https://fabrikam.com/</string>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### ManagedFavorites
  #### お気に入りを構成する
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  管理対象のお気に入りのリストを構成します。

このポリシーによって、お気に入りのリストが作成されます。各お気に入りには、キーとなる "name" と "url" が含まれており、これらのキーはお気に入りの名前とターゲットを保持します。"url" キーを使用せずに、追加の "children" キーを使用してお気に入りを定義することによって、サブフォルダーを構成できます。"children" キーには、上で定義したお気に入りのリストが含まれています (これらのお気に入りの一部は再度フォルダーとして含まれる場合があります)。Microsoft Edge は、不完全な URL をアドレス バーから送信された URL のように修正します。たとえば、"microsoft.com" は "https://microsoft.com/" となります。

これらのお気に入りは、ユーザーが変更できないフォルダーに配置されます (ただし、お気に入りバーでこのフォルダーが非表示になるように選択することはできます)。既定では、フォルダー名は "Managed favorites" ですが、必要なフォルダー名を値として持つ "toplevel_name" キーを含んでいるディクショナリをお気に入りのリストに追加することで、フォルダー名を変更できます。

管理対象のお気に入りは、ユーザー アカウントとは同期されず、拡張機能によって変更することはできません。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  辞書

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: ManagedFavorites
  - GP の名前: お気に入りを構成する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: ManagedFavorites
  - 値の種類: REG_SZ
  ##### サンプル値:
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


  #### Mac の情報と設定
  - 優先されるキーの名前: ManagedFavorites
  - サンプル値:
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
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### ManagedSearchEngines
  #### 検索エンジンの管理
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  最大 10 個の検索エンジンが含まれるリストを構成できます。検索エンジンのいずれか一つは、既定の検索エンジンとしてマークする必要があります。
検索エンジンのエンコードを指定する必要はありません。

このポリシーを有効にした場合、ユーザーはリスト内の検索エンジンを追加、削除、または変更できません。ユーザーは、リスト内のどの検索エンジンでも既定の検索エンジンとして設定できます。

このポリシーを無効にした場合または構成しなかった場合、ユーザーは検索エンジンのリストを必要に応じて変更できます。

[DefaultSearchProviderSearchURL](#defaultsearchprovidersearchurl) ポリシーを設定した場合、このポリシー (ManagedSearchEngines) は無視されます。このポリシーの適用を完了するには、ユーザーはブラウザーを再起動する必要があります。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: いいえ - ブラウザーの再起動が必要です

  #### データ型:
  辞書

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: ManagedSearchEngines
  - GP の名前: 検索エンジンの管理
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: ManagedSearchEngines
  - 値の種類: REG_SZ
  ##### サンプル値:
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


  #### Mac の情報と設定
  - 優先されるキーの名前: ManagedSearchEngines
  - サンプル値:
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
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### MaxConnectionsPerProxy
  #### プロキシ サーバーへの同時実行の最大接続数
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  プロキシ サーバーへの最大同時接続数を指定します。

プロキシ サーバーによっては 1 つのクライアントに対して多数の同時接続を処理できない場合がありますが、このポリシーの値を小さく設定することによって、この問題を解決できます。

このポリシーの値は、7 以上 100 未満の間で設定する必要があります。既定値は 32 です。

一部の Web アプリでは、ハンギング GET で多数の接続が使用されることがわかっています。そのため、最大接続数を 32 未満の小さい値に設定すると、このような Web アプリを多く開きすぎた場合に、ブラウザー ネットワークが停止します。

このポリシーを構成しなかった場合、既定値 (32) が使用されます。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: いいえ - ブラウザーの再起動が必要です

  #### データ型:
  整数

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: MaxConnectionsPerProxy
  - GP の名前: プロキシ サーバーへの同時実行の最大接続数
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: MaxConnectionsPerProxy
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000020
```


  #### Mac の情報と設定
  - 優先されるキーの名前: MaxConnectionsPerProxy
  - サンプル値:
``` xml
<integer>32</integer>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### MediaRouterCastAllowAllIPs
  #### すべての IP アドレスで Cast デバイスに接続することを Google Cast に許可する
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  このポリシーを有効にした場合、Google Cast は、RFC1918/RFC4193 のプライベート アドレスだけでなく、すべての IP アドレスの Cast デバイスに接続できます。

このポリシーを無効にした場合、Google Cast は、RFC1918/RFC4193 のプライベート アドレスの Cast デバイスにのみ接続できます。

このポリシーを構成しなかった場合、CastAllowAllIPs 機能が有効になっていなければ、Google Cast は RFC1918/RFC4193 のプライベート アドレスの Cast デバイスにのみ接続できます。

[EnableMediaRouter](#enablemediarouter) ポリシーを無効にした場合、このポリシーは適用されません。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  ブール値

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: MediaRouterCastAllowAllIPs
  - GP の名前: すべての IP アドレスで Cast デバイスに接続することを Google Cast に許可する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: MediaRouterCastAllowAllIPs
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000000
```


  #### Mac の情報と設定
  - 優先されるキーの名前: MediaRouterCastAllowAllIPs
  - サンプル値:
``` xml
<false/>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### MetricsReportingEnabled
  #### 使用状況とクラッシュに関するデータのレポート送信を有効にする
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  For Windows 10 Beta and Stable channels of Microsoft Edge, this policy when configured will override the Windows diagnostic data setting for collection or non-collection of Microsoft Edge usage and crash related data ([https://go.microsoft.com/fwlink/?linkid=2099569](https://go.microsoft.com/fwlink/?linkid=2099569)).

This policy enables reporting of usage and crash-related data about Microsoft Edge to Microsoft and prevents users from changing this setting.

Enable this policy to send reporting of usage and crash-related data to Microsoft. Disable this policy to not send the data to Microsoft. In both cases, users can't change or override the setting.

On Windows 10, Beta and Stable channels, this policy controls usage data. Crash-related data is determined by the Windows diagnostic data setting. If this policy is not configured, Microsoft Edge will default to the Windows diagnostic data setting.

On Windows 10, Canary and Dev channels, this policy controls usage and crash related data. If this policy is not configured, Microsoft Edge will default to the user's preference.

On Windows 7, 8, and Mac this policy controls usage and crash related data. If this policy is not configured, Microsoft Edge will default to the user's preference.

This policy is available only on Windows instances that are joined to a Microsoft Active Directory domain or Windows 10 Pro or Enterprise instances enrolled for device management.

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: いいえ - ブラウザーの再起動が必要です

  #### データ型:
  ブール値

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: MetricsReportingEnabled
  - GP の名前: 使用状況とクラッシュに関するデータのレポート送信を有効にする
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: MetricsReportingEnabled
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000001
```


  #### Mac の情報と設定
  - 優先されるキーの名前: MetricsReportingEnabled
  - サンプル値:
``` xml
<true/>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### NetworkPredictionOptions
  #### ネットワーク予測を有効にする
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  ネットワーク予測を有効にして、ユーザーがこの設定を変更できないようにします。

これにより、DNS プリフェッチ、TCP と SSL の接続数、および Web ページのプリレンダリングが制御されます。

このポリシーを構成しなかった場合は、ネットワーク予測が有効になりますが、ユーザーはこの設定を変更できます。

* 0 = 任意のネットワーク接続でネットワーク操作を予測する

* 2 = 任意のネットワーク接続でネットワーク操作を予測しない

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: はい
  - 動的ポリシーの更新: はい

  #### データ型:
  整数

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: NetworkPredictionOptions
  - GP の名前: ネットワーク予測を有効にする
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): 管理用テンプレート/Microsoft Edge - 既定の設定 (ユーザーはオーバーライドできます)/
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): SOFTWARE\Policies\Microsoft\Edge\おすすめ
  - 値の名前: NetworkPredictionOptions
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000001
```


  #### Mac の情報と設定
  - 優先されるキーの名前: NetworkPredictionOptions
  - サンプル値:
``` xml
<integer>1</integer>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### NonRemovableProfileEnabled
  #### 職場または学校アカウントで自動的にサインインする既定のプロファイルを、ユーザーが常に持つ必要があるかどうかを構成する
  >サポートされているバージョン: Windows (バージョン 78 以降) の Microsoft Edge

  #### 説明
  このポリシーでは、ユーザーの職場または学校アカウントを使用して自動的にサインインされる Microsoft Edge のプロファイルが削除可能であるかどうかを決定します。

このポリシーを有効にした場合または構成しなかった場合、Windows におけるユーザーの職場または学校アカウントを使用して、削除不可能なプロファイルが作成されます。このプロファイルからサインアウトしたり、このプロファイルを削除したりすることはできません。

このポリシーを無効にした場合、Windows におけるユーザーの職場または学校アカウントを使用して自動的にサインインされるプロファイルについては、ユーザーはサインアウトしたり、削除したりすることができます。

ブラウザー サインインを完全に無効する場合は、'BrowserSignIn' ポリシーを使用します。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  ブール値

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: NonRemovableProfileEnabled
  - GP の名前: 職場または学校アカウントで自動的にサインインする既定のプロファイルを、ユーザーが常に持つ必要があるかどうかを構成する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: NonRemovableProfileEnabled
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000001
```


  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### OverrideSecurityRestrictionsOnInsecureOrigin
  #### 保護されていないオリジンに対するセキュリティ制限を適用する状況を制御する
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  保護されていないオリジンに対してセキュリティ制限を適用しない場合に、そのオリジン (URL) やホスト名パターン ("*.contoso.com"など) のリストを指定します。

このポリシーを使用すると、TLS を展開できないまたは内部の Web 開発についてステージング サーバーをセットアップできないレガシ アプリケーションに対して、オリジンを許可するように指定できます。これにより開発者は、TLS をステージング サーバーに展開しなくても、セキュリティで保護されたコンテキストが必要となる機能をテストすることができます。このポリシーでは、omnibox で "セキュリティ保護なし" というラベルがオリジンに付くのを回避することもできます。

このポリシーで URL のリストを設定すると、同じ URL が指定されたコンマ区切りのリストに対してコマンド ライン フラグ '--unsafely-treat-insecure-origin-as-secure' を設定した場合と同じ効果があります。このポリシーを有効にした場合、コマンド ライン フラグはオーバーライドされます。

セキュリティで保護されたコンテキストの詳細については、https://www.w3.org/TR/secure-contexts/ を参照してください。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: いいえ - ブラウザーの再起動が必要です

  #### データ型:
  文字列の一覧

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: OverrideSecurityRestrictionsOnInsecureOrigin
  - GP の名前: 保護されていないオリジンに対するセキュリティ制限を適用する状況を制御する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge\OverrideSecurityRestrictionsOnInsecureOrigin
  - パス (おすすめ): N/A
  - 値の名前: 1, 2, 3, ...
  - 値の種類: REG_SZ の一覧
  ##### サンプル値:
```
SOFTWARE\Policies\Microsoft\Edge\OverrideSecurityRestrictionsOnInsecureOrigin\0 = "http://testserver.contoso.com/"
SOFTWARE\Policies\Microsoft\Edge\OverrideSecurityRestrictionsOnInsecureOrigin\1 = "*.contoso.com"

```


  #### Mac の情報と設定
  - 優先されるキーの名前: OverrideSecurityRestrictionsOnInsecureOrigin
  - サンプル値:
``` xml
<array>
  <string>http://testserver.contoso.com/</string>
  <string>*.contoso.com</string>
</array>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### PinningWizardAllowed
  #### Allow Pin to taskbar wizard
  >サポートされているバージョン: Windows (バージョン 80 以降) の Microsoft Edge

  #### 説明
  Microsoft Edge uses the Pin to taskbar wizard to help users pin suggested sites to the taskbar. The Pin to taskbar wizard feature is enabled by default and accessible to the user through the Settings and more menu.

If you enable this policy or don't configure it, users can call the Pin to taskbar wizard from the Settings and More menu. The wizard can also be called via a protocol launch.

If you disable this policy, the Pin to taskbar wizard is disabled in the menu and cannot be called via a protocol launch.

User settings to enable or disable the Pin to taskbar wizard aren't available.

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: いいえ - ブラウザーの再起動が必要です

  #### データ型:
  ブール値

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: PinningWizardAllowed
  - GP の名前: Allow Pin to taskbar wizard
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: PinningWizardAllowed
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000000
```


  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### ProactiveAuthEnabled
  #### 事前認証を有効にする
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  事前認証を有効にするかどうかを構成できます。

このポリシーを有効にした場合、Microsoft Edge では、Microsoft サービスにサインインしているユーザーの事前認証を試行します。Microsoft Edge では、定期的にオンライン サービスを調べて、事前認証の方法を規定する構成が含まれているマニフェストが更新されているかどうかを確認します。

このポリシーを無効にした場合、Microsoft Edge では、Microsoft サービスにサインインしているユーザーの事前認証を試行しません。Microsoft Edge では、オンライン サービスを調べて、事前認証を行うための構成が含まれているマニフェストが更新されているかどうかを確認することはありません。

このポリシーを構成しなかった場合、事前認証が有効になります。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: いいえ - ブラウザーの再起動が必要です

  #### データ型:
  ブール値

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: ProactiveAuthEnabled
  - GP の名前: 事前認証を有効にする
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: ProactiveAuthEnabled
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000001
```


  #### Mac の情報と設定
  - 優先されるキーの名前: ProactiveAuthEnabled
  - サンプル値:
``` xml
<true/>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### PromotionalTabsEnabled
  #### タブ全体にプロモーション コンテンツを表示できるようにする
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  フルタブのプロモーション用コンテンツや教育用コンテンツの表示を制御します。この設定は、Microsoft Edge へのサインインのサポート、既定のブラウザーの選択、製品の機能の説明を行うウェルカム ページの表示を制御します。

Iこのポリシーを有効にした場合 (true に設定) または構成しなかった場合、Microsoft Edge では、ユーザーに対してフルタブのコンテンツを表示し、製品情報が提示されます。

Iこの設定を無効にした場合 (false に設定)、Microsoft Edge では、ユーザーに対してフルタブのコンテンツを表示しません。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  ブール値

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: PromotionalTabsEnabled
  - GP の名前: タブ全体にプロモーション コンテンツを表示できるようにする
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: PromotionalTabsEnabled
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000000
```


  #### Mac の情報と設定
  - 優先されるキーの名前: PromotionalTabsEnabled
  - サンプル値:
``` xml
<false/>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### PromptForDownloadLocation
  #### ダウンロードしたファイルの保存場所を確認する
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  ダウンロードする前にファイルの保存場所を確認するかどうかを設定します。

この設定を有効にした場合、ユーザーはダウンロードする前にファイルの保存場所を確認されます。このポリシーを構成しなかった場合、ファイルは既定の場所に自動的に保存され、ユーザーへの確認はありません。

このポリシーを構成しなかった場合、ユーザーはこの設定を変更できます。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  ブール値

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: PromptForDownloadLocation
  - GP の名前: ダウンロードしたファイルの保存場所を確認する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: PromptForDownloadLocation
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000000
```


  #### Mac の情報と設定
  - 優先されるキーの名前: PromptForDownloadLocation
  - サンプル値:
``` xml
<false/>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### QuicAllowed
  #### QUIC プロトコルを許可する
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  Microsoft Edge での QUIC プロトコルの使用を許可します。

このポリシーを有効にした場合または構成しなかった場合、QUIC プロトコルが許可されます。

このポリシーを無効にした場合、QUIC プロトコルはブロックされます。

QUIC とは、トランスポート層ネットワーク プロトコルで、現在 TCP を使用している Web アプリケーションのパフォーマンスを向上させることができます。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: いいえ - ブラウザーの再起動が必要です

  #### データ型:
  ブール値

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: QuicAllowed
  - GP の名前: QUIC プロトコルを許可する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: QuicAllowed
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000001
```


  #### Mac の情報と設定
  - 優先されるキーの名前: QuicAllowed
  - サンプル値:
``` xml
<true/>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### RelaunchNotification
  #### ブラウザーの再起動が推奨されるか、または必須であることをユーザーに通知する
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  保留中の更新プログラムを適用するには Microsoft Edge を再起動する必要があることをユーザーに通知します。

このポリシーを構成しなかった場合、Microsoft Edge では、上部のメニュー バーの右端に [リサイクル] アイコンが追加され、ブラウザーを再起動して更新プログラムを適用するようにユーザーに通知します。

このポリシーを有効にして、'推奨' (1) に設定した場合、再起動が推奨されることをユーザーに通知する警告が定期的に表示されます。ユーザーはこの警告を無視して、再起動を延期できます。

ポリシーを '必須' (2) に設定した場合は、通知期間が経過するとすぐにブラウザーが自動的に再起動されることをユーザーに通知する定期的な警告が表示されます。既定の期間は 7 日間です。この期間は [RelaunchNotificationPeriod](#relaunchnotificationperiod) ポリシーで構成できます。

ユーザーのセッションは、ブラウザーの再起動時に復元されます。

* 推奨 (1) = 再起動が推奨されることを示す定期的なプロンプトをユーザーに表示する

* 必須 (2) = 再起動が必須であることを示す定期的なプロンプトをユーザーに表示する

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  整数

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: RelaunchNotification
  - GP の名前: ブラウザーの再起動が推奨されるか、または必須であることをユーザーに通知する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: RelaunchNotification
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000001
```


  #### Mac の情報と設定
  - 優先されるキーの名前: RelaunchNotification
  - サンプル値:
``` xml
<integer>1</integer>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### RelaunchNotificationPeriod
  #### 更新通知の期間を設定する
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  Allows you to set the time period, in milliseconds, over which users are notified that Microsoft Edge must be relaunched or that a Microsoft Edge OS device must be restarted to apply a pending update.

Over this time period, the user will be repeatedly informed of the need for an update. For Microsoft Edge OS devices, a restart notification appears in the system tray according to the RelaunchHeadsUpPeriod policy. For Microsoft Edge browsers, the app menu changes to indicate that a relaunch is needed once one third of the notification period passes. This notification changes color once two thirds of the notification period passes, and again once the full notification period has passed. The additional notifications enabled by the RelaunchNotification policy follow this same schedule.

If not set, the default period of 604800000 milliseconds (one week) is used.

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  整数

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: RelaunchNotificationPeriod
  - GP の名前: 更新通知の期間を設定する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: RelaunchNotificationPeriod
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x240c8400
```


  #### Mac の情報と設定
  - 優先されるキーの名前: RelaunchNotificationPeriod
  - サンプル値:
``` xml
<integer>604800000</integer>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### RendererCodeIntegrityEnabled
  #### レンダラー コードの整合性を有効にする
  >サポートされているバージョン: Windows (バージョン 78 以降) の Microsoft Edge

  #### 説明
  このポリシーを有効にした場合または設定しなかった場合、レンダラー コードの整合性が有効になります。このポリシーを無効にするには、Microsoft Edge のレンダラー プロセス内で実行する必要があるサード パーティのソフトウェアとの間で互換性の問題が発生する場合のみにしてください。

このポリシーを無効にすると、Microsoft Edge のセキュリティや安定性が悪影響を受けます。これは、悪意を持つ可能性がある不明なコードが、Microsoft Edge のレンダラー プロセス内で読み込まれるためです。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: いいえ - ブラウザーの再起動が必要です

  #### データ型:
  ブール値

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: RendererCodeIntegrityEnabled
  - GP の名前: レンダラー コードの整合性を有効にする
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: RendererCodeIntegrityEnabled
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000000
```


  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### RequireOnlineRevocationChecksForLocalAnchors
  #### トラスト アンカーに対してオンライン OCSP/CRL チェックが必要であるかどうかを指定する
  >サポートされているバージョン: Windows (バージョン 77 以降) の Microsoft Edge

  #### 説明
  オンライン失効確認 (OCSP/CRL チェック) が必要かどうかを制御します。Microsoft Edge が失効状態の情報を取得できない場合、該当の証明書は失効したものとして扱われます (ハード フェイル)。

このポリシーを有効にした場合、Microsoft Edge では、正常に確認されローカルにインストールされている CA 証明書によって署名されたサーバー証明書に対して、常に失効確認を実行します。

このポリシーを構成しなかった場合または無効にした場合、Microsoft Edge では、既存のオンライン失効確認の設定が使用されます。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  ブール値

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: RequireOnlineRevocationChecksForLocalAnchors
  - GP の名前: トラスト アンカーに対してオンライン OCSP/CRL チェックが必要であるかどうかを指定する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: RequireOnlineRevocationChecksForLocalAnchors
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000000
```


  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### ResolveNavigationErrorsUseWebService
  #### Web サービスを使用してナビゲーション エラーを解決できるようにする
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  Microsoft Edge で、データレス接続を Web サービスに対して発行し、ホテルや空港の Wi-Fi などを利用する場合にネットワークの接続性を調べることができるようにします。

このポリシーを有効にした場合、ネットワーク接続のテストで Web サービスが使用されます。

このポリシーを無効にした場合、Microsoft Edge ではネイティブ API を使用して、ネットワーク接続とナビゲーションに関する問題の解決を試行します。

** 注意 **: Windows 8 およびそれ以降のバージョンの Windows を除き、Microsoft Edge では、*常に*ネイティブ API を使用して、接続の問題を解決します。

このポリシーを構成しなかった場合、Microsoft Edge では、edge://settings/privacy の [サービス] で設定されているユーザーの基本設定に従います。
具体的には **[ナビゲーションエラーを解決するために Web サービスを使用する]** というトグルが使用されます。ユーザーはこのトグルのオン/オフを切り替えることができます。ただし、このポリシー (ResolveNavigationErrorsUseWebService) を有効にした場合は、 **[ナビゲーションエラーを解決するために Web サービスを使用する]** の設定がオンになりますが、ユーザーはこのトグルを使用して設定を変更することができなくなります。このポリシーを無効にした場合は、**[ナビゲーションエラーを解決するために Web サービスを使用する]** の設定がオフになり、この場合もユーザーはこのトグルを使用して設定を変更することができなくなります。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: はい
  - 動的ポリシーの更新: はい

  #### データ型:
  ブール値

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: ResolveNavigationErrorsUseWebService
  - GP の名前: Web サービスを使用してナビゲーション エラーを解決できるようにする
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): 管理用テンプレート/Microsoft Edge - 既定の設定 (ユーザーはオーバーライドできます)/
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): SOFTWARE\Policies\Microsoft\Edge\おすすめ
  - 値の名前: ResolveNavigationErrorsUseWebService
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000001
```


  #### Mac の情報と設定
  - 優先されるキーの名前: ResolveNavigationErrorsUseWebService
  - サンプル値:
``` xml
<true/>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### RestrictSigninToPattern
  #### Microsoft Edge プライマリ アカウントとして使用できるアカウントを制限する
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  Microsoft Edge でのブラウザー プライマリ アカウントとして設定できるアカウントを決定します (同期のオプトイン フローで選択されるアカウント)。

ユーザーがこのパターンに一致しないユーザー名でブラウザー プライマリ アカウントを設定しようとすると、設定がブロックされ、適切なエラー メッセージが表示されます。

このポリシーを構成しなかった場合または空のままにした場合、ユーザーは、どのアカウントでも Microsoft Edge でのブラウザー プライマリ アカウントとして設定できます。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  文字列

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: RestrictSigninToPattern
  - GP の名前: Microsoft Edge プライマリ アカウントとして使用できるアカウントを制限する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: RestrictSigninToPattern
  - 値の種類: REG_SZ
  ##### サンプル値:
```
".*@contoso.com"
```


  #### Mac の情報と設定
  - 優先されるキーの名前: RestrictSigninToPattern
  - サンプル値:
``` xml
<string>.*@contoso.com</string>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### RunAllFlashInAllowMode
  #### Adobe Flash コンテンツの設定をすべてのコンテンツに拡張する
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  このポリシーを有効にした場合、コンテンツの設定で Adobe Flash が許可されている Web サイトでは (この許可はユーザーまたはエンタープライズ ポリシーによって指定されます)、埋め込まれているすべての Adobe Flash コンテンツが実行されます。こうしたコンテンツには、他のオリジンからのコンテンツや小さなコンテンツも含まれます。

Adobe Flash の実行を許可する Web サイトを制御するには、[DefaultPluginsSetting](#defaultpluginssetting)、[PluginsAllowedForUrls](#pluginsallowedforurls)、[PluginsBlockedForUrls](#pluginsblockedforurls) の各ポリシーの仕様を参照してください。

このポリシーを無効にした場合または構成しなかった場合、他のオリジン (上に示した 3 つのポリシーで指定されていないサイト) からの Adobe Flash コンテンツや小さなコンテンツはブロックされる可能性があります。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  ブール値

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: RunAllFlashInAllowMode
  - GP の名前: Adobe Flash コンテンツの設定をすべてのコンテンツに拡張する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: RunAllFlashInAllowMode
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000001
```


  #### Mac の情報と設定
  - 優先されるキーの名前: RunAllFlashInAllowMode
  - サンプル値:
``` xml
<true/>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### SSLErrorOverrideAllowed
  #### ユーザーが HTTPS 警告ページから先に進むことを許可する
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  ユーザーが SSL エラーのあるサイトにアクセスしたときに、Microsoft Edge で警告ページが表示されます。

このポリシーを有効にした場合または構成しなかった場合 (既定)、ユーザーはこうした警告ページをクリック スルーすることができます。

このポリシーを無効にした場合、ユーザーはどのような警告ページもクリック スルーすることはできません。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  ブール値

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: SSLErrorOverrideAllowed
  - GP の名前: ユーザーが HTTPS 警告ページから先に進むことを許可する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: SSLErrorOverrideAllowed
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000001
```


  #### Mac の情報と設定
  - 優先されるキーの名前: SSLErrorOverrideAllowed
  - サンプル値:
``` xml
<true/>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### SSLVersionMin
  #### 有効な TLS バージョンを最小限に抑える
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  サポートされる SSL の最小バージョンを設定します。このポリシーを構成しなかった場合、Microsoft Edge では既定の最小バージョン (TLS 1.0) が使用されます。

この設定を有効にした場合、最小バージョンを "tls1"、"tls1.1"、"tls1.2" のいずれかの値に設定できます。設定すると、Microsoft Edge では、指定されたバージョンより小さい SSL/TLS のバージョンは使用されません。認識されない値は無視されます。

* "tls1" = TLS 1.0

* "tls1.1" = TLS 1.1

* "tls1.2" = TLS 1.2

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  文字列

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: SSLVersionMin
  - GP の名前: 有効な TLS バージョンを最小限に抑える
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: SSLVersionMin
  - 値の種類: REG_SZ
  ##### サンプル値:
```
"tls1"
```


  #### Mac の情報と設定
  - 優先されるキーの名前: SSLVersionMin
  - サンプル値:
``` xml
<string>tls1</string>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### SavingBrowserHistoryDisabled
  #### ブラウザーの履歴の保存を無効にする
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  閲覧の履歴の保存を無効にして、ユーザーがこの設定を変更できないようにします。

このポリシーを有効にした場合、閲覧の履歴は保存されません。これにより、タブの同期も無効になります。

このポリシーを無効にした場合、または構成しなかった場合は、閲覧の履歴が保存されます。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  ブール値

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: SavingBrowserHistoryDisabled
  - GP の名前: ブラウザーの履歴の保存を無効にする
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: SavingBrowserHistoryDisabled
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000001
```


  #### Mac の情報と設定
  - 優先されるキーの名前: SavingBrowserHistoryDisabled
  - サンプル値:
``` xml
<true/>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### SearchSuggestEnabled
  #### 検索候補を有効にする
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  Microsoft Edge のアドレスバーおよび自動提案リストの Web 検索候補を有効にして、ユーザーがこのポリシーを変更できないようにします。

このポリシーを有効にした場合、Web 検索候補が使用されます。

このポリシーを無効にした場合、Web 検索候補は使用されませんが、ローカルの履歴とお気に入りの候補が表示されます。また、入力した文字やアクセスした URL は、マイクロソフトに送信される利用統計情報には含まれません。

このポリシーの構成を行わない場合、検索候補は有効になりますが、ユーザーはこれを変更できます。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: はい
  - 動的ポリシーの更新: はい

  #### データ型:
  ブール値

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: SearchSuggestEnabled
  - GP の名前: 検索候補を有効にする
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): 管理用テンプレート/Microsoft Edge - 既定の設定 (ユーザーはオーバーライドできます)/
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): SOFTWARE\Policies\Microsoft\Edge\おすすめ
  - 値の名前: SearchSuggestEnabled
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000001
```


  #### Mac の情報と設定
  - 優先されるキーの名前: SearchSuggestEnabled
  - サンプル値:
``` xml
<true/>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### SecurityKeyPermitAttestation
  #### 直接セキュリティ キー構成証明を使用するためのアクセス許可を必要としない Web サイトまたはドメイン
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  セキュリティ キーからの構成証明書が要求されたときに明示的なユーザー アクセス許可を必要としない Web サイトやドメインを指定します。また、個人の構成証明を使用できることを示す信号がセキュリティ キーに送信されます。このポリシーを指定しなかった場合、サイトがセキュリティ キーの構成証明を要求するたびに、ユーザーに対して確認メッセージが表示されます。

サイト (https://contoso.com/some/path など) は U2F の appID としてのみ照合されます。ドメイン (contoso.com など) は webauthn の RP ID としてのみ照合されます。指定のサイトについて、U2F と webauthn の両方の API に対応するには、appID URL とドメインの両方をリストに指定する必要があります。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  文字列の一覧

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: SecurityKeyPermitAttestation
  - GP の名前: 直接セキュリティ キー構成証明を使用するためのアクセス許可を必要としない Web サイトまたはドメイン
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge\SecurityKeyPermitAttestation
  - パス (おすすめ): N/A
  - 値の名前: 1, 2, 3, ...
  - 値の種類: REG_SZ の一覧
  ##### サンプル値:
```
SOFTWARE\Policies\Microsoft\Edge\SecurityKeyPermitAttestation\0 = "https://contoso.com"

```


  #### Mac の情報と設定
  - 優先されるキーの名前: SecurityKeyPermitAttestation
  - サンプル値:
``` xml
<array>
  <string>https://contoso.com</string>
</array>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### SendIntranetToInternetExplorer
  #### すべてのイントラネット サイトを Internet Explorer に送る
  >サポートされているバージョン: Windows (バージョン 77 以降) の Microsoft Edge

  #### 説明
  Internet Explorer モードに最適なエクスペリエンスを構成するガイダンスについては、[https://go.microsoft.com/fwlink/?linkid=2094210](https://go.microsoft.com/fwlink/?linkid=2094210) を参照してください

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: いいえ - ブラウザーの再起動が必要です

  #### データ型:
  ブール値

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: SendIntranetToInternetExplorer
  - GP の名前: すべてのイントラネット サイトを Internet Explorer に送る
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: SendIntranetToInternetExplorer
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000001
```


  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### SendSiteInfoToImproveServices
  #### Microsoft サービスを改善するためにサイト情報を送信する
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  Microsoft Edge の Windows 10 Beta および Stable チャネルについては、このポリシーが構成されると、Microsoft Edge Web サイト閲覧情報 ([https://go.microsoft.com/fwlink/?linkid=2099569](https://go.microsoft.com/fwlink/?linkid=2099569)) のコレクションまたは非コレクションに設定された Windows 診断データが上書きされます。

このポリシー設定では、ユーザーが Microsoft Edge でアクセスした Web サイトに関する情報を Microsoft に送信できるかどうかを指定できます。

このポリシーを有効にした場合、Microsoft Edge でアクセスした Web サイトに関する情報は、Microsoft に送信されます。

このポリシーを無効にした場合、Microsoft Edge でアクセスした Web サイトに関する情報は、Microsoft に送信されません。

Windows 10、Beta、および Stable チャネルでは、このポリシーがユーザーがアクセスする Web サイトに関する情報の送信を制御します。このポリシーが構成されていなかった場合、Microsoft Edge は Windows 診断データ設定を既定値に設定します。

Windows 10、Canary および Dev チャネルでは、このポリシーがユーザーがアクセスする Web サイトに関する情報の送信を制御します。このポリシーが構成されていなかった場合、Microsoft Edge はユーザー設定を既定値に設定します。

Windows 7、8、および Mac では、このポリシーがユーザーがアクセスする Web サイトに関する情報の送信を制御します。このポリシーが構成されていなかった場合、Microsoft Edge はユーザー設定を既定値に設定します。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: いいえ - ブラウザーの再起動が必要です

  #### データ型:
  ブール値

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: SendSiteInfoToImproveServices
  - GP の名前: Microsoft サービスを改善するためにサイト情報を送信する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: SendSiteInfoToImproveServices
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000000
```


  #### Mac の情報と設定
  - 優先されるキーの名前: SendSiteInfoToImproveServices
  - サンプル値:
``` xml
<false/>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### ShowOfficeShortcutInFavoritesBar
  #### Microsoft Office のショートカットをお気に入りバーに表示する
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  Office.com へのショートカットをお気に入りバーに含めるかどうかを指定します。ユーザーが Microsoft Edge にサインインしている場合、ユーザーはショートカットによって Microsoft Office のアプリやドキュメントにアクセスすることができます。

このポリシーを有効にした場合または構成しなかった場合、ユーザーは、お気に入りバーのコンテキスト メニューで表示/非表示を切り替えることによって、ショートカットを表示するかどうかを選択できます。

この設定を無効にした場合、ショートカットは表示されません。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  ブール値

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: ShowOfficeShortcutInFavoritesBar
  - GP の名前: Microsoft Office のショートカットをお気に入りバーに表示する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: ShowOfficeShortcutInFavoritesBar
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000000
```


  #### Mac の情報と設定
  - 優先されるキーの名前: ShowOfficeShortcutInFavoritesBar
  - サンプル値:
``` xml
<false/>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### SignedHTTPExchangeEnabled
  #### Signed HTTP Exchange (SXG) のサポートを有効にする
  >サポートされているバージョン: Windows および Mac (バージョン 78 以降) の Microsoft Edge

  #### 説明
  Signed HTTP Exchange (SXG) のサポートを有効にします。

このポリシーが設定されていないか、有効にされている場合、Microsoft Edge では、Signed HTTP Exchanges として提供される Web コンテンツを承認します。

このポリシーが無効に設定されている場合、Signed HTTP Exchanges を読み込むことができません。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  ブール値

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: SignedHTTPExchangeEnabled
  - GP の名前: Signed HTTP Exchange (SXG) のサポートを有効にする
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: SignedHTTPExchangeEnabled
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000001
```


  #### Mac の情報と設定
  - 優先されるキーの名前: SignedHTTPExchangeEnabled
  - サンプル値:
``` xml
<true/>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### SitePerProcess
  #### すべてのサイトでサイト分離を有効にする
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  'SitePerProcess' ポリシーを使用すると、すべてのサイトを分離する既定の動作をユーザーがオプトアウトするのを防ぐことができます。[IsolateOrigins](#isolateorigins) ポリシーを使用して、より細かいオリジンをさらに分離することもできます。
このポリシーを有効にした場合、ユーザーは既定の動作をオプトアウトできず、各サイトは独自のプロセスで実行されます。
このポリシーを無効にした場合またはこのポリシーを構成しなかった場合、ユーザーはサイトの分離をオプトアウトできます (たとえは、edge://flags で "Disable site isolation" (サイトの分離を無効にする) エントリを使用)。このポリシーを無効にした場合または構成しなかった場合でも、サイトの分離は無効になりません。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: いいえ - ブラウザーの再起動が必要です

  #### データ型:
  ブール値

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: SitePerProcess
  - GP の名前: すべてのサイトでサイト分離を有効にする
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: SitePerProcess
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000001
```


  #### Mac の情報と設定
  - 優先されるキーの名前: SitePerProcess
  - サンプル値:
``` xml
<true/>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### SpellcheckEnabled
  #### スペルチェックを有効にする
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  このポリシーを有効にした場合または構成しなかった場合、ユーザーはスペルチェックを使用できます。

このポリシーを無効にした場合、ユーザーはスペルチェックを使用できなくなり、[SpellcheckLanguage](#spellchecklanguage) ポリシーと [SpellcheckLanguageBlocklist](#spellchecklanguageblocklist) ポリシーも無効になります。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  ブール値

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: SpellcheckEnabled
  - GP の名前: スペルチェックを有効にする
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: SpellcheckEnabled
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000000
```


  #### Mac の情報と設定
  - 優先されるキーの名前: SpellcheckEnabled
  - サンプル値:
``` xml
<false/>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### SpellcheckLanguage
  #### 特定のスペルチェック言語を有効にする
  >サポートされているバージョン: Windows (バージョン 77 以降) の Microsoft Edge

  #### 説明
  スペルチェックでさまざまな言語が利用できるようにします。指定した言語が認識されない場合は無視されます。

このポリシーを有効にした場合、ポリシーで指定した言語およびユーザーが有効にしたすべての言語でスペルチェックを利用できるようになります。

このポリシーを構成しなかった場合または無効にした場合、ユーザーのスペルチェックの設定は変更されません。

[SpellcheckEnabled](#spellcheckenabled) ポリシーを無効にした場合、このポリシーは適用されません。

言語が 'SpellcheckLanguage' ポリシーと [SpellcheckLanguageBlocklist](#spellchecklanguageblocklist) ポリシーの両方に含まれている場合、そのスペルチェック言語は有効なものとして扱われます。

次の言語がサポートされています: af、bg、ca、cs、cy、da、de、el、en-AU、en-CA、en-GB、en-US、es、es-419、es-AR、es-ES、es-MX、es-US、et、fa、fo、fr、he、hi、hr、hu、id、it、ko、lt、lv、nb、nl、pl、pt-BR、pt-PT、ro、ru、sh、sk、sl、sq、sr、sv、ta、tg、tr、uk、vi。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  文字列の一覧

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: SpellcheckLanguage
  - GP の名前: 特定のスペルチェック言語を有効にする
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge\SpellcheckLanguage
  - パス (おすすめ): N/A
  - 値の名前: 1, 2, 3, ...
  - 値の種類: REG_SZ の一覧
  ##### サンプル値:
```
SOFTWARE\Policies\Microsoft\Edge\SpellcheckLanguage\0 = "fr"
SOFTWARE\Policies\Microsoft\Edge\SpellcheckLanguage\1 = "es"

```


  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### SpellcheckLanguageBlocklist
  #### スペルチェック言語を強制的に無効にする
  >サポートされているバージョン: Windows (バージョン 78 以降) の Microsoft Edge

  #### 説明
  スペルチェック言語を強制的に無効にします。このリストにある認識されない言語は、無視されます。

このポリシーを有効にした場合、指定した言語のスペルチェックが無効になります。ただしユーザーは、リストにない言語に対してスペルチェックを有効または無効にすることができます。

このポリシーを設定しなかった場合または無効にした場合、ユーザーのスペルチェックの設定は変更されません。

[SpellcheckEnabled](#spellcheckenabled) ポリシーを無効に設定した場合、このポリシーは適用されません。

[SpellcheckLanguage](#spellchecklanguage) ポリシーと 'SpellcheckLanguageBlocklist' ポリシーの両方に言語が含まれている場合、そのスペルチェック言語は有効なものとして扱われます。

現在、次の言語がサポートされています: af、bg、ca、cs、da、de、el、en-AU、en-CA、en-GB、en-US、es、es-419、es-AR、es-ES、es-MX、es-US、et、fa、fo、fr、he、hi、hr、hu、id、it、ko、lt、lv、nb、nl、pl、pt-BR、pt-PT、ro、ru、sh、sk、sl、sq、sr、sv、ta、tg、tr、uk、vi。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  文字列の一覧

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: SpellcheckLanguageBlocklist
  - GP の名前: スペルチェック言語を強制的に無効にする
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge\SpellcheckLanguageBlocklist
  - パス (おすすめ): N/A
  - 値の名前: 1, 2, 3, ...
  - 値の種類: REG_SZ の一覧
  ##### サンプル値:
```
SOFTWARE\Policies\Microsoft\Edge\SpellcheckLanguageBlocklist\0 = "fr"
SOFTWARE\Policies\Microsoft\Edge\SpellcheckLanguageBlocklist\1 = "es"

```


  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### SuppressUnsupportedOSWarning
  #### サポートされていない OS の警告を表示しない
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  現在サポートされていないコンピューターやオペレーティング システムで Microsoft Edge が実行されている場合に表示される警告が表示されなくなります。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: いいえ - ブラウザーの再起動が必要です

  #### データ型:
  ブール値

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: SuppressUnsupportedOSWarning
  - GP の名前: サポートされていない OS の警告を表示しない
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: SuppressUnsupportedOSWarning
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000001
```


  #### Mac の情報と設定
  - 優先されるキーの名前: SuppressUnsupportedOSWarning
  - サンプル値:
``` xml
<true/>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### SyncDisabled
  #### Microsoft 同期サービスを使用しているデータの同期を無効にする
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  Microsoft Edge でデータ同期を無効にして、ユーザーがこの設定を変更できないようにします。

このポリシーを設定しなかった場合、ユーザーは同期を有効にしたり無効にしたりすることができます。

'RoamingProfileSupportEnabled' ポリシーが有効になっているときは、このポリシーを有効にしないでください。'RoamingProfileSupportEnabled' と同期機能が重複するためです。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: はい
  - 動的ポリシーの更新: はい

  #### データ型:
  ブール値

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: SyncDisabled
  - GP の名前: Microsoft 同期サービスを使用しているデータの同期を無効にする
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): 管理用テンプレート/Microsoft Edge - 既定の設定 (ユーザーはオーバーライドできます)/
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): SOFTWARE\Policies\Microsoft\Edge\おすすめ
  - 値の名前: SyncDisabled
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000001
```


  #### Mac の情報と設定
  - 優先されるキーの名前: SyncDisabled
  - サンプル値:
``` xml
<true/>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### TabFreezingEnabled
  #### バックグラウンド タブの固定を許可する
  >サポートされているバージョン: Windows および Mac (バージョン 79 以降) の Microsoft Edge

  #### 説明
  Microsoft Edge で、5 分以上バックグラウンドで開かれるタブを固定できるかどうかを制御します。

タブを固定すると、CPU、バッテリ、およびメモリの使用量を減らすことができます。Microsoft Edge では、ヒューリスティックを使用して、重要な処理 (通知の表示、サウンドの再生、動画のストリーム配信など) をバックグラウンドで実行するタブが固定されるのを回避します。

このポリシーを有効にした場合または構成しなかった場合、5 分以上バックグラウンドで表示されていたタブが固定される可能性があります。

このポリシーを無効にした場合、タブは固定されません。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  ブール値

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: TabFreezingEnabled
  - GP の名前: バックグラウンド タブの固定を許可する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: TabFreezingEnabled
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000000
```


  #### Mac の情報と設定
  - 優先されるキーの名前: TabFreezingEnabled
  - サンプル値:
``` xml
<false/>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### TaskManagerEndProcessEnabled
  #### ブラウザーのタスク マネージャーでプロセスの終了を有効にする
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  このポリシーを有効にした場合、または構成しなかった場合、ユーザーは、ブラウザーのタスク マネージャーでプロセスを終了できます。この設定を無効にした場合、ユーザーはプロセスを終了できなくなり、ブラウザーのタスク マネージャーの [プロセスの終了] ボタンが無効になります。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  ブール値

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: TaskManagerEndProcessEnabled
  - GP の名前: ブラウザーのタスク マネージャーでプロセスの終了を有効にする
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: TaskManagerEndProcessEnabled
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000001
```


  #### Mac の情報と設定
  - 優先されるキーの名前: TaskManagerEndProcessEnabled
  - サンプル値:
``` xml
<true/>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### TrackingPrevention
  #### ユーザーの Web 閲覧アクティビティの追跡をブロックする
  >サポートされているバージョン: Windows および Mac (バージョン 78 以降) の Microsoft Edge

  #### 説明
  ユーザーの Web 閲覧アクティビティの追跡から Web サイトをブロックするかどうかを指定できます。

このポリシーを有効にした場合、追跡防止のレベルを設定する次のオプションを使用できます。

0 = オフ (追跡防止なし)
1 = 基本 (有害なトラッカーをブロックし、コンテンツと広告はパーソナル設定されます)
2 = バランス (有害なトラッカーとユーザーがアクセスしていないサイトのトラッカーをブロックします。コンテンツと広告はほとんどパーソナル設定されません)
3 = 厳密 (有害なトラッカーとすべてのサイトの大部分のトラッカーをブロックします。コンテンツと広告のパーソナル設定を最小限に抑えます。サイトの一部が機能しない場合があります)

このポリシーを無効にした場合、または構成しなかった場合、ユーザーは追跡防止の独自のレベルを設定できます。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  整数

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: TrackingPrevention
  - GP の名前: ユーザーの Web 閲覧アクティビティの追跡をブロックする
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: TrackingPrevention
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000002
```


  #### Mac の情報と設定
  - 優先されるキーの名前: TrackingPrevention
  - サンプル値:
``` xml
<integer>2</integer>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### TranslateEnabled
  #### 翻訳を有効にする
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  Microsoft Edge で統合された Microsoft 翻訳サービスを有効にします。

このポリシーを有効にすると、Microsoft Edge では、(該当する場合) 統合された翻訳ポップアップと右クリックコンテキスト メニューの翻訳オプションを表示して、ユーザーに翻訳機能を提供します。

組み込みの翻訳機能をすべて無効にするには、このポリシーを無効にしてください。

ポリシーを構成しない場合、ユーザーは翻訳機能を使用するかどうかを選択できます。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: はい
  - 動的ポリシーの更新: はい

  #### データ型:
  ブール値

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: TranslateEnabled
  - GP の名前: 翻訳を有効にする
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): 管理用テンプレート/Microsoft Edge - 既定の設定 (ユーザーはオーバーライドできます)/
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): SOFTWARE\Policies\Microsoft\Edge\おすすめ
  - 値の名前: TranslateEnabled
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000001
```


  #### Mac の情報と設定
  - 優先されるキーの名前: TranslateEnabled
  - サンプル値:
``` xml
<true/>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### URLAllowlist
  #### 許可されている URL のリストを定義する
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  URL 禁止リストの例外として、リストに登録された URL へのアクセスを許可します。

URL パターンの形式は、[https://go.microsoft.com/fwlink/?linkid=2095322](https://go.microsoft.com/fwlink/?linkid=2095322) に従って指定してください。

このポリシーを使用すると、アクセスを制限する禁止リストに対して例外を適用できます。たとえば、禁止リストに '*' を含めて、すべての要求をブロックしてから、このポリシーを使用し、リストに登録されている限定された URL へのアクセスを許可することができます。このポリシーを使用して、特定のスキーム、他のドメインのサブドメイン、ポート、特定のパスに対して例外を適用することができます。

具体的に指定されたフィルターによって、URL がブロックされるか許可されるかが決定されます。許可リストは、禁止リストよりも優先されます。

このポリシーに登録できるエントリは 1000 件までです。それ以降のエントリは無視されます。

このポリシーを構成しなかった場合、[URLBlocklist](#urlblocklist) ポリシーの禁止リストに対して例外は設定されません。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  文字列の一覧

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: URLAllowlist
  - GP の名前: 許可されている URL のリストを定義する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge\URLAllowlist
  - パス (おすすめ): N/A
  - 値の名前: 1, 2, 3, ...
  - 値の種類: REG_SZ の一覧
  ##### サンプル値:
```
SOFTWARE\Policies\Microsoft\Edge\URLAllowlist\0 = "contoso.com"
SOFTWARE\Policies\Microsoft\Edge\URLAllowlist\1 = "https://ssl.server.com"
SOFTWARE\Policies\Microsoft\Edge\URLAllowlist\2 = "hosting.com/good_path"
SOFTWARE\Policies\Microsoft\Edge\URLAllowlist\3 = "https://server:8080/path"
SOFTWARE\Policies\Microsoft\Edge\URLAllowlist\4 = ".exact.hostname.com"

```


  #### Mac の情報と設定
  - 優先されるキーの名前: URLAllowlist
  - サンプル値:
``` xml
<array>
  <string>contoso.com</string>
  <string>https://ssl.server.com</string>
  <string>hosting.com/good_path</string>
  <string>https://server:8080/path</string>
  <string>.exact.hostname.com</string>
</array>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### URLBlocklist
  #### URL のリストへのアクセスをブロックする
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  ブロックされるサイトのリストを、URL パターンに基づいて定義します (ユーザーはこれらのサイトを読み込むことはできません)。

URL パターンの形式は、[https://go.microsoft.com/fwlink/?linkid=2095322](https://go.microsoft.com/fwlink/?linkid=2095322) に従って指定します。

例外は [URLAllowlist](#urlallowlist) ポリシーで定義できます。これらのポリシーに登録できるエントリは 1000 件までです。それ以降のエントリは無視されます。

内部 URL である 'edge://*' をブロックすることはお勧めしません。こうした URL をブロックすると、予期しないエラーが発生する可能性があります。

このポリシーは、JavaScript を使用した動的なページの更新を妨げるものではありません。たとえば、'contoso.com/abc' をブロックした場合、ユーザーは 'contoso.com' にアクセスし、'contoso.com/abc' のページが更新されていなければ、このページへアクセスするためのリンクをクリックすることはできます。

このポリシーを構成しなかった場合、どの URL もブロックされません。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  文字列の一覧

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: URLBlocklist
  - GP の名前: URL のリストへのアクセスをブロックする
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge\URLBlocklist
  - パス (おすすめ): N/A
  - 値の名前: 1, 2, 3, ...
  - 値の種類: REG_SZ の一覧
  ##### サンプル値:
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


  #### Mac の情報と設定
  - 優先されるキーの名前: URLBlocklist
  - サンプル値:
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
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### UserDataDir
  #### ユーザー データ ディレクトリを設定する
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  ユーザー データの保存に使用するディレクトリを設定します。

このポリシーを有効にした場合、Microsoft Edge では、ユーザーが '--user-data-dir' コマンド ライン フラグを設定したかどうかに関係なく、ポリシーで指定されたディレクトリを使用します。

このポリシーを有効にしなかった場合、既定のプロファイル パスが使用されますが、ユーザーは '--user-data-dir' フラグを使用して、既定のプロファイル パスをオーバーライドできます。プロファイルのディレクトリは、edge://version/ のプロファイル パスで見つけることができます。

データの損失や他のエラーを回避するために、このポリシーの構成では、ボリュームのルート ディレクトリまたは他の用途に使用されるディレクトリを指定しないでください。Microsoft Edge で、こうしたディレクトリのコンテンツを管理しているためです。

使用できる変数のリストについては、[https://go.microsoft.com/fwlink/?linkid=2095041](https://go.microsoft.com/fwlink/?linkid=2095041) を参照してください。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: いいえ - ブラウザーの再起動が必要です

  #### データ型:
  文字列

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: UserDataDir
  - GP の名前: ユーザー データ ディレクトリを設定する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: UserDataDir
  - 値の種類: REG_SZ
  ##### サンプル値:
```
"${users}/${user_name}/Edge"
```


  #### Mac の情報と設定
  - 優先されるキーの名前: UserDataDir
  - サンプル値:
``` xml
<string>${users}/${user_name}/Edge</string>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### UserFeedbackAllowed
  #### ユーザー フィードバックを許可する
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  Microsoft Edge では、Edge フィードバック機能 (既定で有効) を使用することで、ユーザーがフィードバック、提案、または顧客アンケートを送信したり、ブラウザーに関する問題を報告したりすることができます。また既定では、ユーザーは Edge フィードバック機能を無効にする (オフにする) ことができません。

このポリシーを有効にした場合または構成しなかった場合、ユーザーは Edge フィードバックを呼び出すことができます。

このポリシーを無効にした場合、ユーザーは Edge フィードバックを呼び出すことはできません。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: いいえ - ブラウザーの再起動が必要です

  #### データ型:
  ブール値

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: UserFeedbackAllowed
  - GP の名前: ユーザー フィードバックを許可する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: UserFeedbackAllowed
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000001
```


  #### Mac の情報と設定
  - 優先されるキーの名前: UserFeedbackAllowed
  - サンプル値:
``` xml
<true/>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### VideoCaptureAllowed
  #### ビデオ キャプチャを許可または禁止する
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  サイトがビデオをキャプチャできるかどうかを制御します。

このポリシーを有効にした場合または構成しなかった場合 (既定)、ユーザーは、すべてのサイトでビデオ キャプチャのアクセスを確認するよう要求されます。ただし、[VideoCaptureAllowedUrls](#videocaptureallowedurls) ポリシーのリストで構成されている URL を持つサイトは除外されます。こうしたサイトでは、ユーザーへの確認を要求せずにアクセスが許可されます。

このポリシーを無効にした場合、ユーザーに対する確認の要求は行われず、ビデオ キャプチャは、[VideoCaptureAllowedUrls](#videocaptureallowedurls) ポリシーで構成されている URL でのみ利用できます。

このポリシーは、内蔵カメラだけでなく、すべての種類のビデオ入力に影響します。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  ブール値

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: VideoCaptureAllowed
  - GP の名前: ビデオ キャプチャを許可または禁止する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: VideoCaptureAllowed
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000000
```


  #### Mac の情報と設定
  - 優先されるキーの名前: VideoCaptureAllowed
  - サンプル値:
``` xml
<false/>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### VideoCaptureAllowedUrls
  #### アクセス許可を要求しなくてもビデオ キャプチャ デバイスにアクセスできるサイト
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  ユーザーに対してアクセス許可を要求しなくてもビデオ キャプチャ デバイスを使用できる Web サイトを、URL パターンに基づいて定義します。このリスト内のパターンは、要求元 URL のセキュリティ オリジンと照合されます。パターンが一致すると、サイトに対して、ビデオ キャプチャ デバイスへのアクセスが自動的に許可されます。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: はい

  #### データ型:
  文字列の一覧

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: VideoCaptureAllowedUrls
  - GP の名前: アクセス許可を要求しなくてもビデオ キャプチャ デバイスにアクセスできるサイト
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge\VideoCaptureAllowedUrls
  - パス (おすすめ): N/A
  - 値の名前: 1, 2, 3, ...
  - 値の種類: REG_SZ の一覧
  ##### サンプル値:
```
SOFTWARE\Policies\Microsoft\Edge\VideoCaptureAllowedUrls\0 = "https://www.contoso.com/"
SOFTWARE\Policies\Microsoft\Edge\VideoCaptureAllowedUrls\1 = "https://[*.]contoso.edu/"

```


  #### Mac の情報と設定
  - 優先されるキーの名前: VideoCaptureAllowedUrls
  - サンプル値:
``` xml
<array>
  <string>https://www.contoso.com/</string>
  <string>https://[*.]contoso.edu/</string>
</array>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### WPADQuickCheckEnabled
  #### WPAD 最適化を設定する
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  Microsoft Edge で WPAD (Web プロキシ自動検出) の最適化を無効にすることを許可します。

このポリシーを無効にした場合、WPAD の最適化が無効になり、DNS ベースの WPAD サーバーに対するブラウザーの待機間隔が長くなります。

このポリシーを有効にした場合または構成しなかった場合は、WPAD の最適化が有効になります。

このポリシーが有効かどうか、またはポリシーの設定方法に関係なく、ユーザーは WPAD の最適化設定を変更することはできません。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: いいえ - ブラウザーの再起動が必要です

  #### データ型:
  ブール値

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: WPADQuickCheckEnabled
  - GP の名前: WPAD 最適化を設定する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: WPADQuickCheckEnabled
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000001
```


  #### Mac の情報と設定
  - 優先されるキーの名前: WPADQuickCheckEnabled
  - サンプル値:
``` xml
<true/>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### WebDriverOverridesIncompatiblePolicies
  #### 互換性のないポリシーのオーバーライドを WebDriver に許可する
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  このポリシーは必要ではなくなったため、M80 で削除されました。
現在では、WebDriver が既存のすべてのポリシーと互換性を持っています。

このポリシーを使用すると、WebDriver 機能を使用するユーザーは、
動作を妨げる可能性のあるポリシーをオーバーライドできます。

現在、このポリシーによって無効になるのは [SitePerProcess](#siteperprocess) ポリシーと [IsolateOrigins](#isolateorigins) ポリシーです

このポリシーを有効にした場合、WebDriver では互換性のないポリシーを
オーバーライドできます。
このポリシーを無効にした場合または構成しなかった場合、WebDriver では互換性のないポリシーを
オーバーライドできません。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: いいえ - ブラウザーの再起動が必要です

  #### データ型:
  ブール値

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: WebDriverOverridesIncompatiblePolicies
  - GP の名前: 互換性のないポリシーのオーバーライドを WebDriver に許可する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: WebDriverOverridesIncompatiblePolicies
  - 値の種類: REG_DWORD
  ##### サンプル値:
```
0x00000001
```


  #### Mac の情報と設定
  - 優先されるキーの名前: WebDriverOverridesIncompatiblePolicies
  - サンプル値:
``` xml
<true/>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### WebRtcLocalhostIpHandling
  #### WebRTC による localhost IP アドレスの公開を制限する
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  WebRTC でユーザーの localhost IP アドレスを公開するかどうかを設定できます。

このポリシーを "AllowAllInterfaces" ('default') または "AllowPublicAndPrivateInterfaces" ('default_public_and_private_interfaces') に設定した場合、WebRTC は localhost IP アドレスを公開します。

このポリシーを "AllowPublicInterfaceOnly" ('default_public_interface_only') または "DisableNonProxiedUdp" ('disable_non_proxied_udp') に設定した場合、WebRTC は localhost IP アドレスを公開しません。

このポリシーを設定しなかった場合または無効にした場合、WebRTC は localhost IP アドレスを公開します。

  * 'default' = すべてのインターフェイスを許可します。この設定では localhost IP アドレスが公開されます。
  * 'default_public_and_private_interfaces' = http の既定ルートでパブリック インターフェイスやプライベート インターフェイスを許可します。この設定では localhost IP アドレスが公開されます。
  * 'default_public_interface_only' = http の既定ルートでパブリック インターフェイス許可します。この設定では localhost IP アドレスは公開されません。
  * 'disable_non_proxied_udp' = プロキシ サーバーが UDP をサポートしていない場合は TCP を使用します。この設定では localhost IP アドレスは公開されません。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: いいえ - ブラウザーの再起動が必要です

  #### データ型:
  文字列

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: WebRtcLocalhostIpHandling
  - GP の名前: WebRTC による localhost IP アドレスの公開を制限する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: WebRtcLocalhostIpHandling
  - 値の種類: REG_SZ
  ##### サンプル値:
```
"default"
```


  #### Mac の情報と設定
  - 優先されるキーの名前: WebRtcLocalhostIpHandling
  - サンプル値:
``` xml
<string>default</string>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)

  ### WebRtcUdpPortRange
  #### WebRTC で使用されるローカル UDP ポートの範囲を制限する
  >サポートされているバージョン: Windows および Mac (バージョン 77 以降) の Microsoft Edge

  #### 説明
  WebRTC で使用される UDP ポート範囲を、指定されたポート間隔 (エンドポイントも含む) に制限します。

このポリシー設定を構成することで、WebRTC で使用できるローカル UDP ポートの範囲を指定できます。

このポリシーを構成しなかった場合、または空の文字列あるいは無効なポート範囲に設定した場合、WebRTC では、利用可能な任意のローカル UDP ポートを使用できます。

  #### サポートされている機能:
  - 必須になる場合があります: はい
  - 推奨される場合があります: いいえ
  - 動的ポリシーの更新: いいえ - ブラウザーの再起動が必要です

  #### データ型:
  文字列

  #### Windows の情報と設定
  ##### グループ ポリシー (ADMX) 情報
  - GP 固有の名前: WebRtcUdpPortRange
  - GP の名前: WebRTC で使用されるローカル UDP ポートの範囲を制限する
  - GP パス (必須): 管理用テンプレート/Microsoft Edge/
  - GP パス (おすすめ): N/A
  - GP ADMX ファイル名: MSEdge.admx
  ##### Windows レジストリの設定
  - パス (必須): SOFTWARE\Policies\Microsoft\Edge
  - パス (おすすめ): N/A
  - 値の名前: WebRtcUdpPortRange
  - 値の種類: REG_SZ
  ##### サンプル値:
```
"10000-11999"
```


  #### Mac の情報と設定
  - 優先されるキーの名前: WebRtcUdpPortRange
  - サンプル値:
``` xml
<string>10000-11999</string>
```
  

  [トップに戻る](#microsoft-edge---ポリシー)


## 関連項目
- [Microsoft Edge の構成](configure-microsoft-edge.md)
- [Microsoft Edge Enterprise ランディング ページ](https://aka.ms/EdgeEnterprise)