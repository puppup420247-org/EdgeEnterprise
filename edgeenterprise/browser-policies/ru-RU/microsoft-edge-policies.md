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

# Microsoft Edge: политики
Последняя версия Microsoft Edge включает в себя указанные далее политики. Их можно использовать для настройки работы Microsoft Edge в вашей организации.

Чтобы узнать о дополнительных политиках для определения способа и времени обновления Microsoft Edge, перейдите сюда: [Ссылка на политику обновления Microsoft Edge](microsoft-edge-update-policies.md)

> [!ПРИМЕЧАНИЕ]
> Эта статья относится к Microsoft Edge версии 77 или более поздней.

## Доступные политики
В этих таблицах перечислены все связанные с браузером групповые политики, доступные в данном выпуске Microsoft Edge. Используйте ссылки из таблицы для получения дополнительных сведений о конкретных политиках.

|||
|-|-|
|[Cast](#cast)|[Диспетчер паролей и защита](#диспетчер-паролей-и-защита)|
|[Запуск, домашняя страница и страница новой вкладки](#запуск-домашняя-страница-и-страница-новой-вкладки)|[Параметры SmartScreen](#параметры-smartscreen)|
|[Параметры содержимого](#параметры-содержимого)|[Печать](#печать)|
|[Проверка подлинности HTTP](#проверка-подлинности-http)|[Прокси-сервер](#прокси-сервер)|
|[Расширения](#расширения)|[Служба поиска по умолчанию](#служба-поиска-по-умолчанию)|
|[Собственный обмен сообщениями](#собственный-обмен-сообщениями)|[Additional](#additional)|


### [*Cast*](#cast-policies)
|Имя политики|Заголовок|
|-|-|
|[EnableMediaRouter](#enablemediarouter)|Включить Google Cast|
|[ShowCastIconInToolbar](#showcasticonintoolbar)|Показать на панели инструментов значок передачи на другие устройства|
### [*Диспетчер паролей и защита*](#диспетчер-паролей-и-защита-policies)
|Имя политики|Заголовок|
|-|-|
|[PasswordManagerEnabled](#passwordmanagerenabled)|Включить сохранение паролей в диспетчер паролей|
|[PasswordProtectionChangePasswordURL](#passwordprotectionchangepasswordurl)|Настройка URL-адреса изменения пароля|
|[PasswordProtectionLoginURLs](#passwordprotectionloginurls)|Настройте список корпоративных URL-адресов входа, на которых служба защиты пароля должна записывать отпечаток пароля|
|[PasswordProtectionWarningTrigger](#passwordprotectionwarningtrigger)|Настройка триггера предупреждения защиты паролей|
### [*Запуск&comma; домашняя страница и страница новой вкладки*](#запуск-домашняя-страница-и-страница-новой-вкладки-policies)
|Имя политики|Заголовок|
|-|-|
|[HomepageIsNewTabPage](#homepageisnewtabpage)|Назначить страницу новой вкладки домашней страницей|
|[HomepageLocation](#homepagelocation)|Настроить URL-адрес домашней страницы|
|[NewTabPageCompanyLogo](#newtabpagecompanylogo)|Настройка логотипа компании на странице новой вкладки|
|[NewTabPageHideDefaultTopSites](#newtabpagehidedefaulttopsites)|Скрыть популярные сайты по умолчанию со страницы новой вкладки|
|[NewTabPageLocation](#newtabpagelocation)|Настроить URL-адрес страницы новой вкладки|
|[NewTabPageManagedQuickLinks](#newtabpagemanagedquicklinks)|Настройка быстрых ссылок для страницы новой вкладки|
|[NewTabPageSetFeedType](#newtabpagesetfeedtype)|Configure the Microsoft Edge new tab page experience|
|[RestoreOnStartup](#restoreonstartup)|Действие, выполняемое при запуске|
|[RestoreOnStartupURLs](#restoreonstartupurls)|Сайты, которые открываются при запуске браузера|
|[ShowHomeButton](#showhomebutton)|Показать кнопку домашней страницы на панели инструментов|
### [*Параметры SmartScreen*](#параметры-smartscreen-policies)
|Имя политики|Заголовок|
|-|-|
|[PreventSmartScreenPromptOverride](#preventsmartscreenpromptoverride)|Запретить игнорирование сообщений фильтра SmartScreen в Microsoft Defender о сайтах|
|[PreventSmartScreenPromptOverrideForFiles](#preventsmartscreenpromptoverrideforfiles)|Запретить обход предупреждений о загрузках, отправляемых фильтром SmartScreen в Microsoft Defender|
|[SmartScreenAllowListDomains](#smartscreenallowlistdomains)|Настроить список доменов, для которых фильтр SmartScreen в Microsoft Defender не будет отправлять предупреждения|
|[SmartScreenEnabled](#smartscreenenabled)|Настроить фильтр SmartScreen в Microsoft Defender|
|[SmartScreenForTrustedDownloadsEnabled](#smartscreenfortrusteddownloadsenabled)|Принудительная проверка загрузок из надежных источников с помощью фильтра SmartScreen в Microsoft Defender|
|[SmartScreenPuaEnabled](#smartscreenpuaenabled)|Configure Microsoft Defender SmartScreen to block potentially unwanted apps|
### [*Параметры содержимого*](#параметры-содержимого-policies)
|Имя политики|Заголовок|
|-|-|
|[AutoSelectCertificateForUrls](#autoselectcertificateforurls)|Автоматический выбор сертификатов клиентов для этих узлов|
|[CookiesAllowedForUrls](#cookiesallowedforurls)|Разрешить использование файлов cookie на определенных сайтах|
|[CookiesBlockedForUrls](#cookiesblockedforurls)|Блокировать файлы cookie на определенных сайтах|
|[CookiesSessionOnlyForUrls](#cookiessessiononlyforurls)|Ограничить файлы cookie от определенных веб-сайтов для текущего сеанса|
|[DefaultCookiesSetting](#defaultcookiessetting)|Настройка файлов cookie|
|[DefaultGeolocationSetting](#defaultgeolocationsetting)|Настройка географического положения по умолчанию|
|[DefaultImagesSetting](#defaultimagessetting)|Настройка изображений по умолчанию|
|[DefaultJavaScriptSetting](#defaultjavascriptsetting)|Настройка скриптов JavaScript по умолчанию|
|[DefaultNotificationsSetting](#defaultnotificationssetting)|Настройка уведомлений по умолчанию|
|[DefaultPluginsSetting](#defaultpluginssetting)|Параметр Adobe Flash по умолчанию|
|[DefaultPopupsSetting](#defaultpopupssetting)|Настройка всплывающего окна по умолчанию|
|[DefaultWebBluetoothGuardSetting](#defaultwebbluetoothguardsetting)|Управление использованием веб-API Bluetooth|
|[DefaultWebUsbGuardSetting](#defaultwebusbguardsetting)|Управление использованием API WebUSB|
|[ImagesAllowedForUrls](#imagesallowedforurls)|Разрешить изображения на этих сайтах|
|[ImagesBlockedForUrls](#imagesblockedforurls)|Блокировать изображения на определенных сайтах|
|[JavaScriptAllowedForUrls](#javascriptallowedforurls)|Разрешить скрипты JavaScript на определенных сайтах|
|[JavaScriptBlockedForUrls](#javascriptblockedforurls)|Блокировать скрипты JavaScript на определенных сайтах|
|[NotificationsAllowedForUrls](#notificationsallowedforurls)|Разрешить уведомления на определенных сайтах|
|[NotificationsBlockedForUrls](#notificationsblockedforurls)|Блокировать уведомления на определенных сайтах|
|[PluginsAllowedForUrls](#pluginsallowedforurls)|Разрешить подключаемый модуль Adobe Flash на определенных сайтах|
|[PluginsBlockedForUrls](#pluginsblockedforurls)|Блокировать подключаемый модуль Adobe Flash на определенных сайтах|
|[PopupsAllowedForUrls](#popupsallowedforurls)|Разрешить всплывающие окна на определенных сайтах|
|[PopupsBlockedForUrls](#popupsblockedforurls)|Блокировать всплывающие окна на определенных сайтах|
|[RegisteredProtocolHandlers](#registeredprotocolhandlers)|Регистрация обработчиков протоколов|
|[WebUsbAllowDevicesForUrls](#webusballowdevicesforurls)|Разрешить для определенных сайтов доступ к определенным USB-устройствам|
|[WebUsbAskForUrls](#webusbaskforurls)|Разрешить WebUSB на определенных сайтах|
|[WebUsbBlockedForUrls](#webusbblockedforurls)|Блокировать WebUSB на определенных сайтах|
### [*Печать*](#печать-policies)
|Имя политики|Заголовок|
|-|-|
|[DefaultPrinterSelection](#defaultprinterselection)|Правила выбора принтера по умолчанию|
|[PrintHeaderFooter](#printheaderfooter)|Печать колонтитулов|
|[PrintPreviewUseSystemDefaultPrinter](#printpreviewusesystemdefaultprinter)|Задать системный принтер по умолчанию в качестве принтера по умолчанию|
|[PrintingEnabled](#printingenabled)|Включить печать|
|[UseSystemPrintDialog](#usesystemprintdialog)|Печать с помощью системного диалогового окна печати|
### [*Проверка подлинности HTTP*](#проверка-подлинности-http-policies)
|Имя политики|Заголовок|
|-|-|
|[AllowCrossOriginAuthPrompt](#allowcrossoriginauthprompt)|Разрешить запросы обычной проверки подлинности HTTP независимо от источника|
|[AuthNegotiateDelegateAllowlist](#authnegotiatedelegateallowlist)|Список серверов, которым Microsoft Edge может передавать учетные данные пользователя|
|[AuthSchemes](#authschemes)|Поддерживаемые схемы проверки подлинности|
|[AuthServerAllowlist](#authserverallowlist)|Настройка списка разрешенных серверов проверки подлинности|
|[DisableAuthNegotiateCnameLookup](#disableauthnegotiatecnamelookup)|Отключить поиск CNAME при согласовании проверки подлинности Kerberos|
|[EnableAuthNegotiatePort](#enableauthnegotiateport)|Включить нестандартный порт в SPN Kerberos|
|[NtlmV2Enabled](#ntlmv2enabled)|Управление включением и отключением проверки подлинности NTLMv2|
### [*Прокси-сервер*](#прокси-сервер-policies)
|Имя политики|Заголовок|
|-|-|
|[ProxyBypassList](#proxybypasslist)|Настройка правил обхода прокси-сервера|
|[ProxyMode](#proxymode)|Настройка параметров прокси-сервера|
|[ProxyPacUrl](#proxypacurl)|Настроить URL-адрес PAC-файла прокси-сервера|
|[ProxyServer](#proxyserver)|Настройка адреса или URL-адреса прокси-сервера|
|[ProxySettings](#proxysettings)|Параметры прокси-сервера|
### [*Расширения*](#расширения-policies)
|Имя политики|Заголовок|
|-|-|
|[ExtensionAllowedTypes](#extensionallowedtypes)|Настройка разрешенных типов расширений|
|[ExtensionInstallAllowlist](#extensioninstallallowlist)|Разрешить установку определенных расширений|
|[ExtensionInstallBlocklist](#extensioninstallblocklist)|Управление расширениями, которые нельзя устанавливать|
|[ExtensionInstallForcelist](#extensioninstallforcelist)|Определение автоматически устанавливаемых расширений|
|[ExtensionInstallSources](#extensioninstallsources)|Настройка источников установки расширений и пользовательских скриптов|
|[ExtensionSettings](#extensionsettings)|Настройка параметров управления расширениями|
### [*Служба поиска по умолчанию*](#служба-поиска-по-умолчанию-policies)
|Имя политики|Заголовок|
|-|-|
|[DefaultSearchProviderEnabled](#defaultsearchproviderenabled)|Включить службу поиска по умолчанию|
|[DefaultSearchProviderEncodings](#defaultsearchproviderencodings)|Кодировки службы поиска по умолчанию|
|[DefaultSearchProviderImageURL](#defaultsearchproviderimageurl)|Определяет функцию поиска по изображению для системы поиска по умолчанию|
|[DefaultSearchProviderImageURLPostParams](#defaultsearchproviderimageurlpostparams)|Параметры для URL-адреса изображения при использовании метода POST|
|[DefaultSearchProviderKeyword](#defaultsearchproviderkeyword)|Ключевое слово службы поиска по умолчанию|
|[DefaultSearchProviderName](#defaultsearchprovidername)|Имя службы поиска по умолчанию|
|[DefaultSearchProviderSearchURL](#defaultsearchprovidersearchurl)|Поисковый URL-адрес службы поиска по умолчанию|
|[DefaultSearchProviderSuggestURL](#defaultsearchprovidersuggesturl)|URL-адреса службы поиска по умолчанию для предложений|
### [*Собственный обмен сообщениями*](#собственный-обмен-сообщениями-policies)
|Имя политики|Заголовок|
|-|-|
|[NativeMessagingAllowlist](#nativemessagingallowlist)|Управление узлами собственного обмена сообщениями, которые могут использовать пользователи|
|[NativeMessagingBlocklist](#nativemessagingblocklist)|Настроить список блокировки для собственного обмена сообщениями|
|[NativeMessagingUserLevelHosts](#nativemessaginguserlevelhosts)|Разрешить узлы собственного обмена сообщениями на уровне пользователя (установленные без разрешений администратора)|
### [*Additional*](#additional-policies)
|Имя политики|Заголовок|
|-|-|
|[AdsSettingForIntrusiveAdsSites](#adssettingforintrusiveadssites)|Настройка рекламы для сайтов с навязчивой рекламой|
|[AllowDeletingBrowserHistory](#allowdeletingbrowserhistory)|Включить удаление журнала браузера и журнала загрузок|
|[AllowFileSelectionDialogs](#allowfileselectiondialogs)|Разрешить диалоговые окна выбора файлов|
|[AllowPopupsDuringPageUnload](#allowpopupsduringpageunload)|Позволяет странице отображать всплывающие окна во время ее выгрузки|
|[AllowSyncXHRInPageDismissal](#allowsyncxhrinpagedismissal)|Разрешить отправку синхронных запросов XHR при закрытии страницы|
|[AllowTrackingForUrls](#allowtrackingforurls)|Настроить исключения из блокировки отслеживания для определенных сайтов|
|[AlwaysOpenPdfExternally](#alwaysopenpdfexternally)|Всегда открывать PDF-файлы извне|
|[ApplicationLocaleValue](#applicationlocalevalue)|Настроить язык приложения|
|[AudioCaptureAllowed](#audiocaptureallowed)|Разрешить или запретить запись звука|
|[AudioCaptureAllowedUrls](#audiocaptureallowedurls)|Сайты, которые могут получать доступ к устройствам записи звука без запроса разрешения|
|[AutoImportAtFirstRun](#autoimportatfirstrun)|Автоматически импортировать данные и параметры другого браузера при первом запуске|
|[AutofillAddressEnabled](#autofilladdressenabled)|Включить автозаполнение для адресов|
|[AutofillCreditCardEnabled](#autofillcreditcardenabled)|Включить автозаполнение для кредитных карт|
|[AutoplayAllowed](#autoplayallowed)|Разрешить автозапуск мультимедиа для веб-сайтов|
|[BackgroundModeEnabled](#backgroundmodeenabled)|Разрешить фоновым приложениям продолжать работу после закрытия Microsoft Edge|
|[BackgroundTemplateListUpdatesEnabled](#backgroundtemplatelistupdatesenabled)|Включение фонового обновления списка доступных шаблонов для коллекций и других функций, использующих шаблоны.|
|[BlockThirdPartyCookies](#blockthirdpartycookies)|Блокировать сторонние файлы cookie|
|[BrowserAddProfileEnabled](#browseraddprofileenabled)|Разрешить создание профиля во всплывающем меню "Удостоверение" или на странице "Параметры"|
|[BrowserGuestModeEnabled](#browserguestmodeenabled)|Включить режим гостя|
|[BrowserNetworkTimeQueriesEnabled](#browsernetworktimequeriesenabled)|Разрешить запросы к сетевой службе времени браузера|
|[BrowserSignin](#browsersignin)|Параметры входа браузера|
|[BuiltInDnsClientEnabled](#builtindnsclientenabled)|Использовать встроенный DNS-клиент|
|[CertificateTransparencyEnforcementDisabledForCas](#certificatetransparencyenforcementdisabledforcas)|Отключить обязательную проверку прозрачности сертификатов для списка хэш-значений subjectPublicKeyInfo|
|[CertificateTransparencyEnforcementDisabledForLegacyCas](#certificatetransparencyenforcementdisabledforlegacycas)|Отключить обязательную проверку прозрачности сертификатов для списка устаревших центров сертификации|
|[CertificateTransparencyEnforcementDisabledForUrls](#certificatetransparencyenforcementdisabledforurls)|Отключить обязательную проверку прозрачности сертификатов для определенных URL-адресов|
|[ClearBrowsingDataOnExit](#clearbrowsingdataonexit)|Удалять данные о просмотре веб-страниц при закрытии Microsoft Edge|
|[ClickOnceEnabled](#clickonceenabled)|Разрешить пользователям открывать файлы с помощью протокола ClickOnce|
|[CommandLineFlagSecurityWarningsEnabled](#commandlineflagsecuritywarningsenabled)|Включить предупреждения системы безопасности для флагов командной строки|
|[ComponentUpdatesEnabled](#componentupdatesenabled)|Включить обновления компонентов в Microsoft Edge|
|[ConfigureDoNotTrack](#configuredonottrack)|Настроить запросы "Не отслеживать"|
|[ConfigureOnlineTextToSpeech](#configureonlinetexttospeech)|Настройка преобразования текста в речь в сети|
|[CustomHelpLink](#customhelplink)|Указание настраиваемой ссылки для справки|
|[DefaultBrowserSettingEnabled](#defaultbrowsersettingenabled)|Назначить Microsoft Edge стандартным браузером|
|[DeveloperToolsAvailability](#developertoolsavailability)|Определение места использования средств разработчика|
|[DirectInvokeEnabled](#directinvokeenabled)|Разрешить пользователям открывать файлы с помощью протокола DirectInvoke|
|[Disable3DAPIs](#disable3dapis)|Отключить поддержку API трехмерной графики|
|[DisableScreenshots](#disablescreenshots)|Отключить создание снимков экрана|
|[DiskCacheDir](#diskcachedir)|Задать каталог кэша на диске|
|[DiskCacheSize](#diskcachesize)|Задать размер кэша диска (в байтах)|
|[DownloadDirectory](#downloaddirectory)|Настроить каталог загрузки|
|[DownloadRestrictions](#downloadrestrictions)|Разрешить ограничения загрузки|
|[EdgeCollectionsEnabled](#edgecollectionsenabled)|Включить функцию "Коллекции"|
|[EditFavoritesEnabled](#editfavoritesenabled)|Позволяет пользователям редактировать "Избранное"|
|[EnableDeprecatedWebPlatformFeatures](#enabledeprecatedwebplatformfeatures)|Повторно включить устаревшие функции веб-платформы на ограниченное время|
|[EnableDomainActionsDownload](#enabledomainactionsdownload)|Включить загрузку действий домена с серверов корпорации Майкрософт|
|[EnableOnlineRevocationChecks](#enableonlinerevocationchecks)|Включить проверки OCSP/CRL в сети|
|[EnterpriseHardwarePlatformAPIEnabled](#enterprisehardwareplatformapienabled)|Разрешить управляемым расширениям использовать API платформы оборудования предприятия|
|[ExperimentationAndConfigurationServiceControl](#experimentationandconfigurationservicecontrol)|Управление связью со службой "Эксперименты и конфигурация"|
|[ExternalProtocolDialogShowAlwaysOpenCheckbox](#externalprotocoldialogshowalwaysopencheckbox)|Show an "Always open" checkbox in external protocol dialog.|
|[FavoritesBarEnabled](#favoritesbarenabled)|Включить панель "Избранное"|
|[ForceBingSafeSearch](#forcebingsafesearch)|Принудительно применить функцию "Безопасный поиск Bing"|
|[ForceEphemeralProfiles](#forceephemeralprofiles)|Разрешить использование временных профилей|
|[ForceGoogleSafeSearch](#forcegooglesafesearch)|Принудительно применить функцию "Безопасный поиск Google"|
|[ForceNetworkInProcess](#forcenetworkinprocess)|Принудительно выполнять сетевой код в процессе браузера|
|[ForceYouTubeRestrict](#forceyoutuberestrict)|Принудительное применение минимального режима ограниченного доступа на YouTube|
|[FullscreenAllowed](#fullscreenallowed)|Разрешить работу в полноэкранном режиме|
|[GoToIntranetSiteForSingleWordEntryInAddressBar](#gotointranetsiteforsinglewordentryinaddressbar)|При вводе одного слова в адресной строке не выполнять поиск, а перенаправлять пользователя на сайт интрасети.|
|[HSTSPolicyBypassList](#hstspolicybypasslist)|Настройка списка имен, которые будут обходить проверку политики HSTS|
|[HardwareAccelerationModeEnabled](#hardwareaccelerationmodeenabled)|Использовать аппаратное ускорение, если доступно|
|[ImportAutofillFormData](#importautofillformdata)|Разрешить импорт данных автозаполнения формы|
|[ImportBrowserSettings](#importbrowsersettings)|Разрешить импорт настроек браузера|
|[ImportFavorites](#importfavorites)|Разрешить импорт избранного|
|[ImportHistory](#importhistory)|Разрешить импорт журнала браузера|
|[ImportHomepage](#importhomepage)|Разрешить импорт параметров домашней страницы|
|[ImportOpenTabs](#importopentabs)|Разрешение импорта открытых вкладок|
|[ImportPaymentInfo](#importpaymentinfo)|Разрешить импорт платежных данных|
|[ImportSavedPasswords](#importsavedpasswords)|Разрешить импорт сохраненных паролей|
|[ImportSearchEngine](#importsearchengine)|Разрешить импортировать параметры поисковой системы|
|[InPrivateModeAvailability](#inprivatemodeavailability)|Настроить доступность режима InPrivate|
|[InternetExplorerIntegrationLevel](#internetexplorerintegrationlevel)|Настройка интеграции с Internet Explorer|
|[InternetExplorerIntegrationSiteList](#internetexplorerintegrationsitelist)|Настроить список сайтов для режима предприятия|
|[InternetExplorerIntegrationSiteRedirect](#internetexplorerintegrationsiteredirect)|Укажите способ обработки переходов "на странице" для ненастроенных сайтов, выполненных со страниц в режиме Internet Explorer|
|[IsolateOrigins](#isolateorigins)|Включить изоляцию сайта для определенных источников|
|[ManagedFavorites](#managedfavorites)|Настроить "Избранное"|
|[ManagedSearchEngines](#managedsearchengines)|Управление поисковыми системами|
|[MaxConnectionsPerProxy](#maxconnectionsperproxy)|Максимальное число одновременных подключений к прокси-серверу|
|[MediaRouterCastAllowAllIPs](#mediaroutercastallowallips)|Разрешить Google Cast подключаться к устройствам передачи с любыми IP-адресами|
|[MetricsReportingEnabled](#metricsreportingenabled)|Включить отправку отчетов об использовании и данных, относящихся к сбою|
|[NetworkPredictionOptions](#networkpredictionoptions)|Включить прогнозирование сети|
|[NonRemovableProfileEnabled](#nonremovableprofileenabled)|Настройка постоянного автоматического входа пользователя в стандартный профиль на основе рабочей или учебной учетной записи|
|[OverrideSecurityRestrictionsOnInsecureOrigin](#overridesecurityrestrictionsoninsecureorigin)|Управление применением ограничений доступа к небезопасным источникам|
|[ProactiveAuthEnabled](#proactiveauthenabled)|Включить упреждающую проверку подлинности|
|[PromotionalTabsEnabled](#promotionaltabsenabled)|Включить отображение полноширинной вкладки с рекламным содержимым|
|[PromptForDownloadLocation](#promptfordownloadlocation)|Спрашивать, куда сохранять загруженные файлы|
|[QuicAllowed](#quicallowed)|Разрешить протокол QUIC|
|[RelaunchNotification](#relaunchnotification)|Уведомлять пользователя о том, что рекомендуется или требуется перезапустить браузер для ожидающих обновлений|
|[RelaunchNotificationPeriod](#relaunchnotificationperiod)|Задать период времени для уведомлений об обновлении|
|[RendererCodeIntegrityEnabled](#renderercodeintegrityenabled)|Включить целостность кода визуализации|
|[RequireOnlineRevocationChecksForLocalAnchors](#requireonlinerevocationchecksforlocalanchors)|Укажите, требуются ли проверки OCSP и списка отзыва сертификатов через Интернет для локальных якорей доверия|
|[ResolveNavigationErrorsUseWebService](#resolvenavigationerrorsusewebservice)|Включить устранение ошибок навигации с помощью веб-службы|
|[RestrictSigninToPattern](#restrictsignintopattern)|Ограничить учетные записи, которые могут использоваться в качестве основных в Microsoft Edge|
|[RunAllFlashInAllowMode](#runallflashinallowmode)|Расширить параметр содержимого Adobe Flash на все содержимое|
|[SSLErrorOverrideAllowed](#sslerroroverrideallowed)|Разрешить пользователям продолжать работу со страницы предупреждения HTTPS|
|[SSLVersionMin](#sslversionmin)|Включена минимальная версия протокола TLS|
|[SavingBrowserHistoryDisabled](#savingbrowserhistorydisabled)|Отключить сохранение журнала браузера|
|[SearchSuggestEnabled](#searchsuggestenabled)|Включить варианты поиска|
|[SecurityKeyPermitAttestation](#securitykeypermitattestation)|Веб-сайты и домены, которые не требуют разрешения на использование прямой аттестации ключа безопасности|
|[SendIntranetToInternetExplorer](#sendintranettointernetexplorer)|Отправка всех сайтов интрасети в Internet Explorer|
|[SendSiteInfoToImproveServices](#sendsiteinfotoimproveservices)|Отправлять сведения о сайте для улучшения служб Майкрософт|
|[ShowOfficeShortcutInFavoritesBar](#showofficeshortcutinfavoritesbar)|Показать ярлык Microsoft Office на панели "Избранное"|
|[SignedHTTPExchangeEnabled](#signedhttpexchangeenabled)|Включить поддержку подписи HTTP exchange (SXG)|
|[SitePerProcess](#siteperprocess)|Включить изоляцию для каждого сайта|
|[SpellcheckEnabled](#spellcheckenabled)|Включить проверку орфографии|
|[SpellcheckLanguage](#spellchecklanguage)|Включить конкретные языки проверки орфографии|
|[SpellcheckLanguageBlocklist](#spellchecklanguageblocklist)|Принудительное отключение языков проверки орфографии|
|[SuppressUnsupportedOSWarning](#suppressunsupportedoswarning)|Отключить предупреждение о неподдерживаемой ОС|
|[SyncDisabled](#syncdisabled)|Отключить синхронизацию данных с помощью служб синхронизации Майкрософт|
|[TabFreezingEnabled](#tabfreezingenabled)|Allow freezing of background tabs|
|[TaskManagerEndProcessEnabled](#taskmanagerendprocessenabled)|Включить завершение процессов в диспетчере задач браузера|
|[TrackingPrevention](#trackingprevention)|Блокировка отслеживания просмотренных веб-страниц|
|[TranslateEnabled](#translateenabled)|Включить перевод|
|[URLAllowlist](#urlallowlist)|Определить список разрешенных URL-адресов|
|[URLBlocklist](#urlblocklist)|Запретить доступ к списку URL-адресов|
|[UserDataDir](#userdatadir)|Задать каталог данных пользователя|
|[UserFeedbackAllowed](#userfeedbackallowed)|Разрешить отзывы пользователей|
|[VideoCaptureAllowed](#videocaptureallowed)|Разрешить или запретить запись видео|
|[VideoCaptureAllowedUrls](#videocaptureallowedurls)|Сайты, которые могут получать доступ к устройствам записи видео без запроса разрешения|
|[WPADQuickCheckEnabled](#wpadquickcheckenabled)|Настроить оптимизацию WPAD|
|[WebDriverOverridesIncompatiblePolicies](#webdriveroverridesincompatiblepolicies)|Разрешить WebDriver переопределять несовместимые политики|
|[WebRtcLocalhostIpHandling](#webrtclocalhostiphandling)|Ограничить раскрытие IP-адреса localhost с помощью WebRTC|
|[WebRtcUdpPortRange](#webrtcudpportrange)|Ограничить диапазон локальных UDP-портов, используемых WebRTC|




  ## Cast policies

  [В начало](#microsoft-edge:-политики)

  ### EnableMediaRouter
  #### Включить Google Cast
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Включите этот параметр политики, чтобы активировать Google Cast. Пользователи смогут запустить эту функцию из меню приложения, контекстных меню страницы, с помощью элементов управления мультимедиа на веб-сайтах с поддержкой Cast и с помощью значка компонента Cast (если отображается) на панели инструментов.

Отключите этот параметр политики, чтобы отключить Google Cast.

По умолчанию функция Google Cast активирована.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Нет - Требуется перезапуск браузера

  #### Тип данных:
  Логическое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: EnableMediaRouter
  - Имя групповой политики: Включить Google Cast
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/Cast
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: EnableMediaRouter
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000001
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: EnableMediaRouter
  - Пример значения:
``` xml
<true/>
```
  

  [В начало](#microsoft-edge:-политики)

  ### ShowCastIconInToolbar
  #### Показать на панели инструментов значок передачи на другие устройства
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Set this policy to true to show the Cast toolbar icon on the toolbar or the overflow menu. Users won't be able to remove it.

If you don't configure this policy or if you disable it, users can pin or remove the icon by using its contextual menu.

If you've also set the [EnableMediaRouter](#enablemediarouter) policy to false, then this policy is ignored, and the toolbar icon isn't shown.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Нет - Требуется перезапуск браузера

  #### Тип данных:
  Логическое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: ShowCastIconInToolbar
  - Имя групповой политики: Показать на панели инструментов значок передачи на другие устройства
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/Cast
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: ShowCastIconInToolbar
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000000
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: ShowCastIconInToolbar
  - Пример значения:
``` xml
<false/>
```
  

  [В начало](#microsoft-edge:-политики)

  ## Диспетчер паролей и защита policies

  [В начало](#microsoft-edge:-политики)

  ### PasswordManagerEnabled
  #### Включить сохранение паролей в диспетчер паролей
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Сохранение паролей пользователя в Microsoft Edge.

Если этот параметр политики включен, пользователи могут сохранять свои пароли в Microsoft Edge. При последующих посещениях сайта Microsoft Edge автоматически вводит пароль.

Если этот параметр политики отключен, пользователи не могут сохранять новые пароли, но могут использовать ранее сохраненные пароли.

Если включить или отключить этот параметр политики, пользователи не смогут изменить или переопределить его в Microsoft Edge. Если этот параметр не задан, пользователи могут сохранять пароли, а также могут отключить эту функцию.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Да
  - Динамическое обновление политики: Да

  #### Тип данных:
  Логическое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: PasswordManagerEnabled
  - Имя групповой политики: Включить сохранение паролей в диспетчер паролей
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/Диспетчер паролей и защита
  - Путь групповой политики (Рекомендовано): Административные шаблоны/Microsoft Edge - Параметры по умолчанию (пользователи могут переопределять)/Диспетчер паролей и защита
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): SOFTWARE\Policies\Microsoft\Edge\Рекомендовано
  - Имя значения: PasswordManagerEnabled
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000001
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: PasswordManagerEnabled
  - Пример значения:
``` xml
<true/>
```
  

  [В начало](#microsoft-edge:-политики)

  ### PasswordProtectionChangePasswordURL
  #### Настройка URL-адреса изменения пароля
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Настройка URL-адреса для смены пароля (только схемы HTTP и HTTPS).

Служба защиты паролей будет отправлять пользователей на этот URL-адрес для смены пароля после появления предупреждения в браузере.

Если эта политика включена, служба защиты паролей отправляет пользователей на данный URL-адрес для смены пароля.

Если эта политика отключена или не настроена, служба защиты паролей не перенаправляет пользователей на URL-адрес для смены пароля.

Эта политика доступна только в экземплярах Windows, присоединенных к домену Microsoft Active Directory, либо в экземплярах Windows 10 Pro или Windows 10 Корпоративная, зарегистрированных для управления устройствами.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Строковое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: PasswordProtectionChangePasswordURL
  - Имя групповой политики: Настройка URL-адреса изменения пароля
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/Диспетчер паролей и защита
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: PasswordProtectionChangePasswordURL
  - Тип значения: REG_SZ
  ##### Пример значения:
```
"https://contoso.com/change_password.html"
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: PasswordProtectionChangePasswordURL
  - Пример значения:
``` xml
<string>https://contoso.com/change_password.html</string>
```
  

  [В начало](#microsoft-edge:-политики)

  ### PasswordProtectionLoginURLs
  #### Настройте список корпоративных URL-адресов входа, на которых служба защиты пароля должна записывать отпечаток пароля
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Настройка списка корпоративных URL-адресов входа (только схемы HTTP и HTTPS), на которых браузер Microsoft Edge должен записывать отпечаток паролей и использовать его для определения повторного использования паролей.

Если эта политика включена, служба защиты паролей записывает отпечатки паролей на определенных URL-адресах.

Если эта политика отключена или не настроена, отпечатки паролей не записываются.

Эта политика доступна только в экземплярах Windows, присоединенных к домену Microsoft Active Directory, либо в экземплярах Windows 10 Pro или Windows 10 Корпоративная, зарегистрированных для управления устройствами.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Список строк

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: PasswordProtectionLoginURLs
  - Имя групповой политики: Настройте список корпоративных URL-адресов входа, на которых служба защиты пароля должна записывать отпечаток пароля
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/Диспетчер паролей и защита
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge\PasswordProtectionLoginURLs
  - Путь (Рекомендовано): Н/Д
  - Имя значения: 1, 2, 3, ...
  - Тип значения: Список REG_SZ
  ##### Пример значения:
```
SOFTWARE\Policies\Microsoft\Edge\PasswordProtectionLoginURLs\0 = "https://contoso.com/login.html"
SOFTWARE\Policies\Microsoft\Edge\PasswordProtectionLoginURLs\1 = "https://login.contoso.com"

```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: PasswordProtectionLoginURLs
  - Пример значения:
``` xml
<array>
  <string>https://contoso.com/login.html</string>
  <string>https://login.contoso.com</string>
</array>
```
  

  [В начало](#microsoft-edge:-политики)

  ### PasswordProtectionWarningTrigger
  #### Настройка триггера предупреждения защиты паролей
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Allows you to control when to trigger password protection warning. Password protection alerts users when they reuse their protected password on potentially suspicious sites.

You can use the [PasswordProtectionLoginURLs](#passwordprotectionloginurls) and [PasswordProtectionChangePasswordURL](#passwordprotectionchangepasswordurl) policies to configure which passwords to protect.

Exemptions: Passwords for the sites listed in [PasswordProtectionLoginURLs](#passwordprotectionloginurls) and [PasswordProtectionChangePasswordURL](#passwordprotectionchangepasswordurl), as well as for the sites listed in [SmartScreenAllowListDomains](#smartscreenallowlistdomains), will not trigger a password-protection warning.

Set to 'PasswordProtectionWarningOff' (0) to not show password protection warningss.

Set to 'PasswordProtectionWarningOnPasswordReuse' (1) to show password protection warnings when the user reuses their protected password on a non-whitelisted site.

If you disable or don't configure this policy, then the warning trigger is not shown.

* 0 = Password protection warning is off.

* 1 = Password protection warning is triggered by password reuse.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Целое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: PasswordProtectionWarningTrigger
  - Имя групповой политики: Настройка триггера предупреждения защиты паролей
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/Диспетчер паролей и защита
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: PasswordProtectionWarningTrigger
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000001
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: PasswordProtectionWarningTrigger
  - Пример значения:
``` xml
<integer>1</integer>
```
  

  [В начало](#microsoft-edge:-политики)

  ## Запуск&comma; домашняя страница и страница новой вкладки policies

  [В начало](#microsoft-edge:-политики)

  ### HomepageIsNewTabPage
  #### Назначить страницу новой вкладки домашней страницей
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Настройка стандартной домашней страницы в Microsoft Edge. В качестве домашней страницы можно задать URL-адрес или страницу новой вкладки.

Когда этот параметр политики включен, страница новой вкладки всегда используется в качестве домашней страницы, а URL-адрес домашней страницы игнорируется.

Когда этот параметр политики выключен, домашняя страница пользователя не может быть страницей новой вкладки, если в качестве URL-адреса не указано "edge://newtab".

Когда этот параметр не настроен, пользователи могут выбирать, будет ли страница новой вкладки их домашней страницей.

Этот параметр политики доступен только в экземплярах Windows, присоединенных к домену Microsoft Active Directory, либо в экземплярах Windows 10 Pro или Windows 10 Корпоративная, зарегистрированных для управления устройствами.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Да
  - Динамическое обновление политики: Да

  #### Тип данных:
  Логическое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: HomepageIsNewTabPage
  - Имя групповой политики: Назначить страницу новой вкладки домашней страницей
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/Запуск, домашняя страница и страница новой вкладки
  - Путь групповой политики (Рекомендовано): Административные шаблоны/Microsoft Edge - Параметры по умолчанию (пользователи могут переопределять)/Запуск, домашняя страница и страница новой вкладки
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): SOFTWARE\Policies\Microsoft\Edge\Рекомендовано
  - Имя значения: HomepageIsNewTabPage
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000001
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: HomepageIsNewTabPage
  - Пример значения:
``` xml
<true/>
```
  

  [В начало](#microsoft-edge:-политики)

  ### HomepageLocation
  #### Настроить URL-адрес домашней страницы
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Configures the default home page URL in Microsoft Edge.

The home page is the page opened by the Home button. The pages that open on startup are controlled by the [RestoreOnStartup](#restoreonstartup) policies.

You can either set a URL here or set the home page to open the new tab page. If you select to open the new tab page, then this policy doesn't take effect.

If you enable this policy, users can't change their home page URL, but they can choose to use the new tab page as their home page.

If you disable or don't configure this policy, users can choose their own home page, as long as the [HomepageIsNewTabPage](#homepageisnewtabpage) policy isn't enabled.

This policy is available only on Windows instances that are joined to a Microsoft Active Directory domain or Windows 10 Pro or Enterprise instances enrolled for device management.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Да
  - Динамическое обновление политики: Да

  #### Тип данных:
  Строковое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: HomepageLocation
  - Имя групповой политики: Настроить URL-адрес домашней страницы
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/Запуск, домашняя страница и страница новой вкладки
  - Путь групповой политики (Рекомендовано): Административные шаблоны/Microsoft Edge - Параметры по умолчанию (пользователи могут переопределять)/Запуск, домашняя страница и страница новой вкладки
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): SOFTWARE\Policies\Microsoft\Edge\Рекомендовано
  - Имя значения: HomepageLocation
  - Тип значения: REG_SZ
  ##### Пример значения:
```
"https://www.contoso.com"
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: HomepageLocation
  - Пример значения:
``` xml
<string>https://www.contoso.com</string>
```
  

  [В начало](#microsoft-edge:-политики)

  ### NewTabPageCompanyLogo
  #### Настройка логотипа компании на странице новой вкладки
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 79 или более поздней версии

  #### Описание
  Определяет логотип компании, который будет использоваться на странице новой вкладки в Microsoft Edge.

Этот параметр политики должен быть настроен в виде строки, которая выражает логотип в формате JSON. Пример: { "default_logo": { "url": "https://www.contoso.com/logo.png", "hash": "cd0aa9856147b6c5b4ff2b7dfee5da20aa38253099ef1b4a64aced233c9afe29" }, "light_logo": { "url": "https://www.contoso.com/light_logo.png", "hash": "517d286edb416bb2625ccfcba9de78296e90da8e32330d4c9c8275c4c1c33737" } }

Этот параметр политики настраивается путем указания URL-адреса, с которого Microsoft Edge может загрузить требуемый логотип, и хэша шифрования (SHA-256), который используется для проверки целостности загрузки. Логотип должен быть сохранен в формате PNG или SVG, а размер файла логотипа не должен превышать 16 МБ. Логотип загружается и хэшируется, и будет повторно загружаться при каждом изменении URL-адреса или хэша. URL-адрес должен быть доступен без какой-либо проверки подлинности.

Элемент "default_logo" является обязательным. Он будет использоваться в случае отсутствия фонового изображения. Если предоставлен элемент "light_logo", он будет использоваться в случаях, когда у страницы новой вкладки пользователя есть фоновое изображение. Рекомендуется использовать горизонтальный логотип с прозрачным фоном, выровненный по левому краю и по вертикали выровненный по центру. Высота логотипа должна составлять не меньше 32 пикселей, а соотношение сторон от 1:1 до 4:1. Элемент "default_logo" должен быть достаточно контрастным на черном/белом фоне, а элемент "light_logo" должен выглядеть достаточно контрастным на фоновом изображении.

Если этот параметр политики включен, Microsoft Edge загружает и отображает указанный логотип на странице новой вкладки. Пользователи не могут скрыть или переопределить его.

Если отключить или не настроить этот параметр политики, Microsoft Edge не будет отображать логотип на странице новой вкладки или будет отображать логотип Microsoft.

Справку по определению хэша SHA-256 см. на странице https://docs.microsoft.com/en-us/powershell/module/microsoft.powershell.utility/get-filehash?view=powershell-6.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Нет - Требуется перезапуск браузера

  #### Тип данных:
  Словарь

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: NewTabPageCompanyLogo
  - Имя групповой политики: Настройка логотипа компании на странице новой вкладки
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/Запуск, домашняя страница и страница новой вкладки
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: NewTabPageCompanyLogo
  - Тип значения: REG_SZ
  ##### Пример значения:
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


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: NewTabPageCompanyLogo
  - Пример значения:
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
  

  [В начало](#microsoft-edge:-политики)

  ### NewTabPageHideDefaultTopSites
  #### Скрыть популярные сайты по умолчанию со страницы новой вкладки
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Удаление стандартных популярных сайтов со страницы новой вкладки в Microsoft Edge.

Если для этого параметра задано значение true, стандартные плитки популярных сайтов скрыты.

Если для этого параметра задано значение false или он не настроен, стандартные плитки популярных сайтов отображаются.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Логическое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: NewTabPageHideDefaultTopSites
  - Имя групповой политики: Скрыть популярные сайты по умолчанию со страницы новой вкладки
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/Запуск, домашняя страница и страница новой вкладки
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: NewTabPageHideDefaultTopSites
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000001
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: NewTabPageHideDefaultTopSites
  - Пример значения:
``` xml
<true/>
```
  

  [В начало](#microsoft-edge:-политики)

  ### NewTabPageLocation
  #### Настроить URL-адрес страницы новой вкладки
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Configures the default URL for the new tab page.

This policy determines the page that's opened when new tabs are created (including when new windows are opened). It also affects the startup page if that's set to open to the new tab page.

This policy doesn't determine which page opens on startup; that's controlled by the [RestoreOnStartup](#restoreonstartup) policy. It also doesn’t affect the home page if that’s set to open to the new tab page.

If you don't configure this policy, the default new tab page is used.

If you configure this policy *and* the [NewTabPageSetFeedType](#newtabpagesetfeedtype) policy, this policy has precedence.

If an invalid URL is provided, new tabs will open about://blank.

This policy is available only on Windows instances that are joined to a Microsoft Active Directory domain or Windows 10 Pro or Enterprise instances that are enrolled for device management.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Да
  - Динамическое обновление политики: Да

  #### Тип данных:
  Строковое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: NewTabPageLocation
  - Имя групповой политики: Настроить URL-адрес страницы новой вкладки
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/Запуск, домашняя страница и страница новой вкладки
  - Путь групповой политики (Рекомендовано): Административные шаблоны/Microsoft Edge - Параметры по умолчанию (пользователи могут переопределять)/Запуск, домашняя страница и страница новой вкладки
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): SOFTWARE\Policies\Microsoft\Edge\Рекомендовано
  - Имя значения: NewTabPageLocation
  - Тип значения: REG_SZ
  ##### Пример значения:
```
"https://www.fabrikam.com"
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: NewTabPageLocation
  - Пример значения:
``` xml
<string>https://www.fabrikam.com</string>
```
  

  [В начало](#microsoft-edge:-политики)

  ### NewTabPageManagedQuickLinks
  #### Настройка быстрых ссылок для страницы новой вкладки
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 79 или более поздней версии

  #### Описание
  По умолчанию в качестве быстрых ссылок на странице новой вкладки Microsoft Edge отображаются добавленные пользователем ярлыки и популярные сайты из журнала браузера. С помощью этого параметра политики можно настроить до трех плиток быстрых ссылок на странице новой вкладки в виде объектов JSON:

[ { "url": "https://www.contoso.com", "title": "Contoso Portal", "pinned": true/false }, ... ]

Поле "url" — обязательное, "title" и "pinned" — необязательные. Если в поле "title" не задано значение, по умолчанию используется URL-адрес. Если в поле "pinned" не задано значение, по умолчанию используется значение false.

Microsoft Edge отображает плитки в указанном порядке (слева направо), при этом все закрепленные плитки предшествуют незакрепленным.

Если этот параметр политики является обязательным, поле "pinned" будет пропущено и все плитки будут закреплены. Пользователь не сможет удалить плитки. Они всегда будут отображаться в передней части списка быстрых ссылок.

Если политика задана как рекомендуемая, закрепленные плитки останутся в списке, но пользователь сможет изменять и удалять их. Незакрепленные плитки быстрых ссылок, как и стандартные популярные сайты, сдвигаются вниз по списку, если другие веб-сайты используются чаще. Когда незакрепленные ссылки применяются с помощью этого параметра политики к существующему профилю браузера, они могут не появиться, если имеют более низкий приоритет, чем другие ссылки из журнала браузера данного пользователя.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Да
  - Динамическое обновление политики: Нет - Требуется перезапуск браузера

  #### Тип данных:
  Словарь

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: NewTabPageManagedQuickLinks
  - Имя групповой политики: Настройка быстрых ссылок для страницы новой вкладки
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/Запуск, домашняя страница и страница новой вкладки
  - Путь групповой политики (Рекомендовано): Административные шаблоны/Microsoft Edge - Параметры по умолчанию (пользователи могут переопределять)/Запуск, домашняя страница и страница новой вкладки
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): SOFTWARE\Policies\Microsoft\Edge\Рекомендовано
  - Имя значения: NewTabPageManagedQuickLinks
  - Тип значения: REG_SZ
  ##### Пример значения:
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


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: NewTabPageManagedQuickLinks
  - Пример значения:
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
  

  [В начало](#microsoft-edge:-политики)

  ### NewTabPageSetFeedType
  #### Configure the Microsoft Edge new tab page experience
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 79 или более поздней версии

  #### Описание
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

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Да
  - Динамическое обновление политики: Да

  #### Тип данных:
  Целое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: NewTabPageSetFeedType
  - Имя групповой политики: Configure the Microsoft Edge new tab page experience
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/Запуск, домашняя страница и страница новой вкладки
  - Путь групповой политики (Рекомендовано): Административные шаблоны/Microsoft Edge - Параметры по умолчанию (пользователи могут переопределять)/Запуск, домашняя страница и страница новой вкладки
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): SOFTWARE\Policies\Microsoft\Edge\Рекомендовано
  - Имя значения: NewTabPageSetFeedType
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000000
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: NewTabPageSetFeedType
  - Пример значения:
``` xml
<integer>0</integer>
```
  

  [В начало](#microsoft-edge:-политики)

  ### RestoreOnStartup
  #### Действие, выполняемое при запуске
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Действия в Microsoft Edge при запуске.

Если необходимо, чтобы при запуске всегда открывалась новая вкладка, выберите пункт "Открывать новую вкладку" (5).

Если необходимо открывать URL-адреса, которые были открыты перед последним закрытием Microsoft Edge, выберите пункт "Восстанавливать последний сеанс" (1). Сеанс просмотра будет восстановлен в том состоянии, в котором он был на момент закрытия. Обратите внимание: этот параметр отключает некоторые настройки, которые зависят от сеансов или выполняют действия при выходе (например, удаление данных о просмотре веб-страниц при выходе или использование файлов cookie только во время сеанса).

Если необходимо открывать определенный набор URL-адресов, выберите пункт "Открывать список URL-адресов" (4).

Отключенный параметр действует так же, как ненастроенный. Пользователи могут изменить этот параметр в Microsoft Edge.

Этот параметр политики доступен только в экземплярах Windows, присоединенных к домену Microsoft Active Directory, либо в экземплярах Windows 10 Pro или Windows 10 Корпоративная, зарегистрированных для управления устройствами.

* 5 = Открывать новую вкладку

* 1 = Восстанавливать последний сеанс

* 4 = Открывать список URL-адресов

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Да
  - Динамическое обновление политики: Да

  #### Тип данных:
  Целое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: RestoreOnStartup
  - Имя групповой политики: Действие, выполняемое при запуске
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/Запуск, домашняя страница и страница новой вкладки
  - Путь групповой политики (Рекомендовано): Административные шаблоны/Microsoft Edge - Параметры по умолчанию (пользователи могут переопределять)/Запуск, домашняя страница и страница новой вкладки
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): SOFTWARE\Policies\Microsoft\Edge\Рекомендовано
  - Имя значения: RestoreOnStartup
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000004
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: RestoreOnStartup
  - Пример значения:
``` xml
<integer>4</integer>
```
  

  [В начало](#microsoft-edge:-политики)

  ### RestoreOnStartupURLs
  #### Сайты, которые открываются при запуске браузера
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Specify a list of websites to open automatically when the browser starts. If you don't configure this policy, no site is opened on startup.

This policy only works if you also set the [RestoreOnStartup](#restoreonstartup) policy to 'Open a list of URLs' (4).

This policy is only available on Windows instances that are joined to a Microsoft Active Directory domain or Windows 10 Pro or Enterprise instances that are enrolled for device management.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Да
  - Динамическое обновление политики: Да

  #### Тип данных:
  Список строк

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: RestoreOnStartupURLs
  - Имя групповой политики: Сайты, которые открываются при запуске браузера
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/Запуск, домашняя страница и страница новой вкладки
  - Путь групповой политики (Рекомендовано): Административные шаблоны/Microsoft Edge - Параметры по умолчанию (пользователи могут переопределять)/Запуск, домашняя страница и страница новой вкладки
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge\RestoreOnStartupURLs
  - Путь (Рекомендовано): SOFTWARE\Policies\Microsoft\Edge\Рекомендовано\RestoreOnStartupURLs
  - Имя значения: 1, 2, 3, ...
  - Тип значения: Список REG_SZ
  ##### Пример значения:
```
SOFTWARE\Policies\Microsoft\Edge\RestoreOnStartupURLs\0 = "https://contoso.com"
SOFTWARE\Policies\Microsoft\Edge\RestoreOnStartupURLs\1 = "https://www.fabrikam.com"

```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: RestoreOnStartupURLs
  - Пример значения:
``` xml
<array>
  <string>https://contoso.com</string>
  <string>https://www.fabrikam.com</string>
</array>
```
  

  [В начало](#microsoft-edge:-политики)

  ### ShowHomeButton
  #### Показать кнопку домашней страницы на панели инструментов
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Отображение кнопки домашней страницы на панели инструментов Microsoft Edge.

Если этот параметр включен, кнопка домашней страницы всегда отображается. Если этот параметр выключен, кнопка никогда не отображается.

Если данный параметр не настроен, пользователи могут самостоятельно отобразить или скрыть эту кнопку.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Да
  - Динамическое обновление политики: Да

  #### Тип данных:
  Логическое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: ShowHomeButton
  - Имя групповой политики: Показать кнопку домашней страницы на панели инструментов
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/Запуск, домашняя страница и страница новой вкладки
  - Путь групповой политики (Рекомендовано): Административные шаблоны/Microsoft Edge - Параметры по умолчанию (пользователи могут переопределять)/Запуск, домашняя страница и страница новой вкладки
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): SOFTWARE\Policies\Microsoft\Edge\Рекомендовано
  - Имя значения: ShowHomeButton
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000001
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: ShowHomeButton
  - Пример значения:
``` xml
<true/>
```
  

  [В начало](#microsoft-edge:-политики)

  ## Параметры SmartScreen policies

  [В начало](#microsoft-edge:-политики)

  ### PreventSmartScreenPromptOverride
  #### Запретить игнорирование сообщений фильтра SmartScreen в Microsoft Defender о сайтах
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  С помощью этого параметра политики можно разрешить или запретить пользователям переопределять предупреждения фильтра SmartScreen в Microsoft Defender, касающиеся потенциально вредоносных веб-сайтов.

Если включить этот параметр, пользователи не смогут игнорировать предупреждения фильтра SmartScreen в Microsoft Defender и переходить на соответствующие веб-сайты.

Если отключить или не настроить этот параметр, пользователи смогут игнорировать предупреждения фильтра SmartScreen в Microsoft Defender и переходить на соответствующие веб-сайты.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Логическое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: PreventSmartScreenPromptOverride
  - Имя групповой политики: Запретить игнорирование сообщений фильтра SmartScreen в Microsoft Defender о сайтах
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/Параметры SmartScreen
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: PreventSmartScreenPromptOverride
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000001
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: PreventSmartScreenPromptOverride
  - Пример значения:
``` xml
<true/>
```
  

  [В начало](#microsoft-edge:-политики)

  ### PreventSmartScreenPromptOverrideForFiles
  #### Запретить обход предупреждений о загрузках, отправляемых фильтром SmartScreen в Microsoft Defender
  >Поддерживаемые версии: Microsoft Edge на Windows с 77 или более поздней версии, а также на Mac с 79 или более поздней версии

  #### Описание
  С помощью этого параметра политики можно разрешить или запретить сотрудникам переопределять предупреждения о непроверенных загрузках, отправляемые фильтром SmartScreen в Microsoft Defender.

Если включить этот параметр, сотрудники не смогут игнорировать предупреждения фильтра SmartScreen в Microsoft Defender и загружать непроверенные элементы.

Если отключить или не настроить этот параметр, сотрудники смогут игнорировать предупреждения фильтра SmartScreen в Microsoft Defender и загружать непроверенные элементы.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Логическое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: PreventSmartScreenPromptOverrideForFiles
  - Имя групповой политики: Запретить обход предупреждений о загрузках, отправляемых фильтром SmartScreen в Microsoft Defender
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/Параметры SmartScreen
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: PreventSmartScreenPromptOverrideForFiles
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000001
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: PreventSmartScreenPromptOverrideForFiles
  - Пример значения:
``` xml
<true/>
```
  

  [В начало](#microsoft-edge:-политики)

  ### SmartScreenAllowListDomains
  #### Настроить список доменов, для которых фильтр SmartScreen в Microsoft Defender не будет отправлять предупреждения
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Настройка списка доменов, которым доверяет фильтр SmartScreen в Microsoft Defender. Это означает следующее.
Фильтр SmartScreen в Microsoft Defender не будет проверять потенциально вредоносные ресурсы (например, программы для фишинга и другое вредоносное ПО), если исходные URL-адреса совпадают с этими доменами.
Служба защиты загрузок фильтра SmartScreen в Microsoft Defender не будет проверять загружаемые файлы, размещенные на этих доменах.

Если включить этот параметр политики, фильтр SmartScreen в Microsoft Defender будет доверять этим доменам.
Если отключить или не настроить этот параметр политики, ко всем ресурсам применяется стандартная защита фильтра SmartScreen в Microsoft Defender.
Этот параметр политики доступен только в экземплярах Windows, присоединенных к домену Microsoft Active Directory, либо экземплярах Windows 10 Pro или Windows 10 Корпоративная, зарегистрированных для управления устройствами.
Также обратите внимание: этот параметр политики не применяется, если ваша организация включила функцию Advanced Threat Protection в Microsoft Defender. В этом случае следует настроить списки разрешенных и запрещенных URL-адресов в Центре безопасности в Microsoft Defender.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Список строк

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: SmartScreenAllowListDomains
  - Имя групповой политики: Настроить список доменов, для которых фильтр SmartScreen в Microsoft Defender не будет отправлять предупреждения
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/Параметры SmartScreen
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge\SmartScreenAllowListDomains
  - Путь (Рекомендовано): Н/Д
  - Имя значения: 1, 2, 3, ...
  - Тип значения: Список REG_SZ
  ##### Пример значения:
```
SOFTWARE\Policies\Microsoft\Edge\SmartScreenAllowListDomains\0 = "mydomain.com"
SOFTWARE\Policies\Microsoft\Edge\SmartScreenAllowListDomains\1 = "myuniversity.edu"

```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: SmartScreenAllowListDomains
  - Пример значения:
``` xml
<array>
  <string>mydomain.com</string>
  <string>myuniversity.edu</string>
</array>
```
  

  [В начало](#microsoft-edge:-политики)

  ### SmartScreenEnabled
  #### Настроить фильтр SmartScreen в Microsoft Defender
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  This policy setting lets you configure whether to turn on Microsoft Defender SmartScreen. Microsoft Defender SmartScreen provides warning messages to help protect your users from potential phishing scams and malicious software. By default, Microsoft Defender SmartScreen is turned on.

If you enable this setting, Microsoft Defender SmartScreen is turned on.

If you disable this setting, Microsoft Defender SmartScreen is turned off.

If you don't configure this setting, users can choose whether to use Microsoft Defender SmartScreen.

This policy is available only on Windows instances that are joined to a Microsoft Active Directory domain; or on Windows 10 Pro or Enterprise instances that are enrolled for device management.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Да
  - Динамическое обновление политики: Да

  #### Тип данных:
  Логическое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: SmartScreenEnabled
  - Имя групповой политики: Настроить фильтр SmartScreen в Microsoft Defender
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/Параметры SmartScreen
  - Путь групповой политики (Рекомендовано): Административные шаблоны/Microsoft Edge - Параметры по умолчанию (пользователи могут переопределять)/Параметры SmartScreen
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): SOFTWARE\Policies\Microsoft\Edge\Рекомендовано
  - Имя значения: SmartScreenEnabled
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000001
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: SmartScreenEnabled
  - Пример значения:
``` xml
<true/>
```
  

  [В начало](#microsoft-edge:-политики)

  ### SmartScreenForTrustedDownloadsEnabled
  #### Принудительная проверка загрузок из надежных источников с помощью фильтра SmartScreen в Microsoft Defender
  >Поддерживаемые версии: Microsoft Edge на Windows с 78 или более поздней версии

  #### Описание
  Этот параметр политики позволяет указать, будет ли фильтр SmartScreen в Microsoft Defender проверять репутацию загрузки из надежного источника.

Если этот параметр включен или не настроен, фильтр SmartScreen в Microsoft Defender проверяет репутацию загрузки независимо от источника.

Если этот параметр выключен, фильтр SmartScreen в Microsoft Defender не проверяет репутацию загрузки, если она выполняется из надежного источника.

Этот параметр политики доступен только в экземплярах Windows, присоединенных к домену Microsoft Active Directory, либо в экземплярах Windows 10 Pro или Windows 10 Корпоративная, зарегистрированных для управления устройствами.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Да
  - Динамическое обновление политики: Да

  #### Тип данных:
  Логическое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: SmartScreenForTrustedDownloadsEnabled
  - Имя групповой политики: Принудительная проверка загрузок из надежных источников с помощью фильтра SmartScreen в Microsoft Defender
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/Параметры SmartScreen
  - Путь групповой политики (Рекомендовано): Административные шаблоны/Microsoft Edge - Параметры по умолчанию (пользователи могут переопределять)/Параметры SmartScreen
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): SOFTWARE\Policies\Microsoft\Edge\Рекомендовано
  - Имя значения: SmartScreenForTrustedDownloadsEnabled
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000000
```


  

  [В начало](#microsoft-edge:-политики)

  ### SmartScreenPuaEnabled
  #### Configure Microsoft Defender SmartScreen to block potentially unwanted apps
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 80 или более поздней версии

  #### Описание
  This policy setting lets you configure whether to turn on blocking for potentially unwanted apps in Microsoft Defender SmartScreen. Potentially unwanted app blocking in Microsoft Defender SmartScreen provides warning messages to help protect users from adware, coin miners, bundleware, and other low-reputation apps that are hosted by websites. Potentially unwanted app blocking in Microsoft Defender SmartScreen is turned off by default.

If you enable this setting, potentially unwanted app blocking in Microsoft Defender SmartScreen is turned on.

If you disable this setting, potentially unwanted app blocking in Microsoft Defender SmartScreen is turned off.

If you don't configure this setting, users can choose whether to use potentially unwanted app blocking in Microsoft Defender SmartScreen.

This policy is available only on Windows instances that are joined to a Microsoft Active Directory domain; or on Windows 10 Pro or Enterprise instances that are enrolled for device management.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Да
  - Динамическое обновление политики: Да

  #### Тип данных:
  Логическое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: SmartScreenPuaEnabled
  - Имя групповой политики: Configure Microsoft Defender SmartScreen to block potentially unwanted apps
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/Параметры SmartScreen
  - Путь групповой политики (Рекомендовано): Административные шаблоны/Microsoft Edge - Параметры по умолчанию (пользователи могут переопределять)/Параметры SmartScreen
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): SOFTWARE\Policies\Microsoft\Edge\Рекомендовано
  - Имя значения: SmartScreenPuaEnabled
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000001
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: SmartScreenPuaEnabled
  - Пример значения:
``` xml
<true/>
```
  

  [В начало](#microsoft-edge:-политики)

  ## Параметры содержимого policies

  [В начало](#microsoft-edge:-политики)

  ### AutoSelectCertificateForUrls
  #### Автоматический выбор сертификатов клиентов для этих узлов
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Specify a list of sites, based on URL patterns, for which Microsoft Edge should automatically select a client certificate, if the site requests one.

The value must be an array of stringified JSON dictionaries. Each dictionary must have the form { "pattern": "$URL_PATTERN", "filter" : $FILTER }, where $URL_PATTERN is a content setting pattern. $FILTER restricts from which client certificates the browser will automatically select. Independent of the filter, only certificates will be selected that match the server's certificate request. For example, if $FILTER has the form { "ISSUER": { "CN": "$ISSUER_CN" } }, additionally only client certificates are selected that are issued by a certificate with the CommonName $ISSUER_CN. If $FILTER contains an "ISSUER" and a "SUBJECT" section, a client certificate must satisfy both conditions to be selected. If $FILTER specifies an organization ("O"), a certificate must have at least one organization which matches the specified value to be selected. If $FILTER specifies an organization unit ("OU"), a certificate must have at least one organization unit which matches the specified value to be selected. If $FILTER is the empty dictionary {}, the selection of client certificates is not additionally restricted.

If you don't configure this policy, auto-selection isn't done for any site.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Список строк

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: AutoSelectCertificateForUrls
  - Имя групповой политики: Автоматический выбор сертификатов клиентов для этих узлов
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/Параметры содержимого
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge\AutoSelectCertificateForUrls
  - Путь (Рекомендовано): Н/Д
  - Имя значения: 1, 2, 3, ...
  - Тип значения: Список REG_SZ
  ##### Пример значения:
```
SOFTWARE\Policies\Microsoft\Edge\AutoSelectCertificateForUrls\0 = "{"pattern":"https://www.contoso.com","filter":{"ISSUER":{"CN":"certificate issuer name", "L": "certificate issuer location", "O": "certificate issuer org", "OU": "certificate issuer org unit"}, "SUBJECT":{"CN":"certificate subject name", "L": "certificate subject location", "O": "certificate subject org", "OU": "certificate subject org unit"}}}"

```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: AutoSelectCertificateForUrls
  - Пример значения:
``` xml
<array>
  <string>{"pattern":"https://www.contoso.com","filter":{"ISSUER":{"CN":"certificate issuer name", "L": "certificate issuer location", "O": "certificate issuer org", "OU": "certificate issuer org unit"}, "SUBJECT":{"CN":"certificate subject name", "L": "certificate subject location", "O": "certificate subject org", "OU": "certificate subject org unit"}}}</string>
</array>
```
  

  [В начало](#microsoft-edge:-политики)

  ### CookiesAllowedForUrls
  #### Разрешить использование файлов cookie на определенных сайтах
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Define a list of sites, based on URL patterns, that are allowed to set cookies.

If you don't configure this policy, the global default value from the [DefaultCookiesSetting](#defaultcookiessetting) policy (if set) or the user's personal configuration is used for all sites.

See the [CookiesBlockedForUrls](#cookiesblockedforurls) and [CookiesSessionOnlyForUrls](#cookiessessiononlyforurls) policies for more information.

Note there cannot be conflicting URL patterns set between these three policies:

- [CookiesBlockedForUrls](#cookiesblockedforurls)

- CookiesAllowedForUrls

- [CookiesSessionOnlyForUrls](#cookiessessiononlyforurls)

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Список строк

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: CookiesAllowedForUrls
  - Имя групповой политики: Разрешить использование файлов cookie на определенных сайтах
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/Параметры содержимого
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge\CookiesAllowedForUrls
  - Путь (Рекомендовано): Н/Д
  - Имя значения: 1, 2, 3, ...
  - Тип значения: Список REG_SZ
  ##### Пример значения:
```
SOFTWARE\Policies\Microsoft\Edge\CookiesAllowedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\CookiesAllowedForUrls\1 = "[*.]contoso.edu"

```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: CookiesAllowedForUrls
  - Пример значения:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [В начало](#microsoft-edge:-политики)

  ### CookiesBlockedForUrls
  #### Блокировать файлы cookie на определенных сайтах
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Define a list of sites, based on URL patterns, that can't set cookies.

If you don't configure this policy, the global default value from the [DefaultCookiesSetting](#defaultcookiessetting) policy (if set) or the user's personal configuration is used for all sites.

See the [CookiesAllowedForUrls](#cookiesallowedforurls) and [CookiesSessionOnlyForUrls](#cookiessessiononlyforurls) policies for more information.

Note there cannot be conflicting URL patterns set between these three policies:

- CookiesBlockedForUrls

- [CookiesAllowedForUrls](#cookiesallowedforurls)

- [CookiesSessionOnlyForUrls](#cookiessessiononlyforurls)

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Список строк

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: CookiesBlockedForUrls
  - Имя групповой политики: Блокировать файлы cookie на определенных сайтах
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/Параметры содержимого
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge\CookiesBlockedForUrls
  - Путь (Рекомендовано): Н/Д
  - Имя значения: 1, 2, 3, ...
  - Тип значения: Список REG_SZ
  ##### Пример значения:
```
SOFTWARE\Policies\Microsoft\Edge\CookiesBlockedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\CookiesBlockedForUrls\1 = "[*.]contoso.edu"

```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: CookiesBlockedForUrls
  - Пример значения:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [В начало](#microsoft-edge:-политики)

  ### CookiesSessionOnlyForUrls
  #### Ограничить файлы cookie от определенных веб-сайтов для текущего сеанса
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Cookies created by websites that match a URL pattern you define are deleted when the session ends (when the window closes).

Cookies created by websites that don't match the pattern are controlled by the [DefaultCookiesSetting](#defaultcookiessetting) policy (if set) or by the user's personal configuration. This is also the default behavior if you don't configure this policy.

If Microsoft Edge is running in background mode, the session might not close when the last window is closed, meaning the cookies won't be cleared when the window closes. See the [BackgroundModeEnabled](#backgroundmodeenabled) policy for information about configuring what happens when Microsoft Edge runs in background mode.

You can also use the [CookiesAllowedForUrls](#cookiesallowedforurls) and [CookiesBlockedForUrls](#cookiesblockedforurls) policies to control which websites can create cookies.

Note there cannot be conflicting URL patterns set between these three policies:

- [CookiesBlockedForUrls](#cookiesblockedforurls)

- [CookiesAllowedForUrls](#cookiesallowedforurls)

- CookiesSessionOnlyForUrls

If you set the [RestoreOnStartup](#restoreonstartup) policy to restore URLs from previous sessions, this policy is ignored, and cookies are stored permanently for those sites.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Список строк

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: CookiesSessionOnlyForUrls
  - Имя групповой политики: Ограничить файлы cookie от определенных веб-сайтов для текущего сеанса
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/Параметры содержимого
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge\CookiesSessionOnlyForUrls
  - Путь (Рекомендовано): Н/Д
  - Имя значения: 1, 2, 3, ...
  - Тип значения: Список REG_SZ
  ##### Пример значения:
```
SOFTWARE\Policies\Microsoft\Edge\CookiesSessionOnlyForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\CookiesSessionOnlyForUrls\1 = "[*.]contoso.edu"

```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: CookiesSessionOnlyForUrls
  - Пример значения:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [В начало](#microsoft-edge:-политики)

  ### DefaultCookiesSetting
  #### Настройка файлов cookie
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Control whether websites can create cookies on the user's device. This policy is all or nothing - you can let all websites create cookies, or no websites create cookies. You can't use this policy to enable cookies from specific websites.

Set the policy to 'SessionOnly' (4) to clear cookies when the session closes. If Microsoft Edge is running in background mode, the session might not close when the last window is closed, meaning the cookies won't be cleared when the window closes. See [BackgroundModeEnabled](#backgroundmodeenabled) policy for information about configuring what happens when Microsoft Edge runs in background mode.

If you don't configure this policy, the default 'AllowCookies' (1) is used, and users can change this setting in Microsoft Edge Settings. (If you don't want users to be able to change this setting, set the policy.)

* 1 = Let all sites create cookies

* 2 = Don't let any site create cookies

* 4 = Keep cookies for the duration of the session

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Целое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: DefaultCookiesSetting
  - Имя групповой политики: Настройка файлов cookie
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/Параметры содержимого
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: DefaultCookiesSetting
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000001
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: DefaultCookiesSetting
  - Пример значения:
``` xml
<integer>1</integer>
```
  

  [В начало](#microsoft-edge:-политики)

  ### DefaultGeolocationSetting
  #### Настройка географического положения по умолчанию
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Этот параметр политики позволяет указать, могут ли веб-сайты отслеживать физическое расположение пользователя. Можно либо разрешить отслеживание по умолчанию (1), либо запретить его по умолчанию (2), либо каждый раз запрашивать у пользователя соответствующее разрешение (3).

Если этот параметр политики не настроен, используется параметр AskGeolocation и пользователь может изменить данную настройку.

* 1 = Разрешить сайтам отслеживать физическое расположение пользователя

* 2 = Запретить сайтам отслеживать физическое расположение пользователя

* 3 = Запрашивать у пользователя разрешение при каждой попытке сайта отследить физическое расположение пользователя

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Целое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: DefaultGeolocationSetting
  - Имя групповой политики: Настройка географического положения по умолчанию
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/Параметры содержимого
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: DefaultGeolocationSetting
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000001
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: DefaultGeolocationSetting
  - Пример значения:
``` xml
<integer>1</integer>
```
  

  [В начало](#microsoft-edge:-политики)

  ### DefaultImagesSetting
  #### Настройка изображений по умолчанию
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Этот параметр политики позволяет разрешить или запретить использование изображений на веб-сайтах. Можно либо разрешить изображения на всех сайтах (1), либо заблокировать их на всех сайтах (2).

Если этот параметр политики не настроен, изображения разрешены по умолчанию и пользователь может изменить данную настройку.

* 1 = Разрешить любые изображения на всех сайтах

* 2 = Запретить изображения на всех сайтах

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Целое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: DefaultImagesSetting
  - Имя групповой политики: Настройка изображений по умолчанию
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/Параметры содержимого
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: DefaultImagesSetting
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000001
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: DefaultImagesSetting
  - Пример значения:
``` xml
<integer>1</integer>
```
  

  [В начало](#microsoft-edge:-политики)

  ### DefaultJavaScriptSetting
  #### Настройка скриптов JavaScript по умолчанию
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Этот параметр политики позволяет разрешить или запретить выполнение сценариев JavaScript на веб-сайтах. Можно либо разрешить сценарии JavaScript на всех сайтах (1), либо заблокировать их на всех сайтах (2).

Если этот параметр политики не настроен, на всех сайтах можно запускать сценарии JavaScript по умолчанию и пользователь может изменить данную настройку.

* 1 = Разрешить сценарии JavaScript на всех сайтах

* 2 = Запретить сценарии JavaScript на всех сайтах

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Целое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: DefaultJavaScriptSetting
  - Имя групповой политики: Настройка скриптов JavaScript по умолчанию
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/Параметры содержимого
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: DefaultJavaScriptSetting
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000001
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: DefaultJavaScriptSetting
  - Пример значения:
``` xml
<integer>1</integer>
```
  

  [В начало](#microsoft-edge:-политики)

  ### DefaultNotificationsSetting
  #### Настройка уведомлений по умолчанию
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Этот параметр политики позволяет указать, могут ли веб-сайты отображать уведомления на рабочем столе. Можно либо разрешить это делать по умолчанию (1), либо запретить это делать по умолчанию (2), либо каждый раз запрашивать у пользователя соответствующее разрешение (3).

Если этот параметр политики не настроен, уведомления разрешены по умолчанию и пользователь может изменить данную настройку.

* 1 = Разрешить сайтам отображать уведомления на рабочем столе

* 2 = Не разрешать сайтам отображать уведомления на рабочем столе

* 3 = Запрашивать у пользователя разрешение при каждой попытке веб-сайта отобразить уведомление на рабочем столе

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Целое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: DefaultNotificationsSetting
  - Имя групповой политики: Настройка уведомлений по умолчанию
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/Параметры содержимого
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: DefaultNotificationsSetting
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000002
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: DefaultNotificationsSetting
  - Пример значения:
``` xml
<integer>2</integer>
```
  

  [В начало](#microsoft-edge:-политики)

  ### DefaultPluginsSetting
  #### Параметр Adobe Flash по умолчанию
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Determines whether websites that aren't covered by [PluginsAllowedForUrls](#pluginsallowedforurls) or [PluginsBlockedForUrls](#pluginsblockedforurls) can automatically run the Adobe Flash plug-in. You can select 'BlockPlugins' (2) to block Adobe Flash on all sites, or you can select 'ClickToPlay' (3) to let Adobe Flash run but require the user to click the placeholder to start it. In any case, the [PluginsAllowedForUrls](#pluginsallowedforurls) and [PluginsBlockedForUrls](#pluginsblockedforurls) policies take precedence over 'DefaultPluginsSetting'.

Automatic playback is only allowed for domains explicitly listed in the [PluginsAllowedForUrls](#pluginsallowedforurls) policy. If you want to enable automatic playback for all sites, consider adding http://* and https://* to this list.

If you don't configure this policy, the user can change this setting manually.

* 2 = Block the Adobe Flash plug-in

* 3 = Click to play

The former '1' option set allow-all, but this functionality is now only handled by the [PluginsAllowedForUrls](#pluginsallowedforurls) policy.  Existing policies using '1' will operate in Click-to-play mode.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Целое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: DefaultPluginsSetting
  - Имя групповой политики: Параметр Adobe Flash по умолчанию
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/Параметры содержимого
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: DefaultPluginsSetting
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000002
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: DefaultPluginsSetting
  - Пример значения:
``` xml
<integer>2</integer>
```
  

  [В начало](#microsoft-edge:-политики)

  ### DefaultPopupsSetting
  #### Настройка всплывающего окна по умолчанию
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Этот параметр политики позволяет разрешить или запретить использование всплывающих окон на веб-сайтах. Можно либо разрешить всплывающие окна на всех сайтах (1), либо заблокировать их на всех сайтах (2).

Если этот параметр политики не настроен, всплывающие окна блокируются по умолчанию и пользователь может изменить данную настройку.

* 1 = Разрешить всплывающие окна на всех сайтах

* 2 = Запретить всплывающие окна на всех сайтах

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Целое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: DefaultPopupsSetting
  - Имя групповой политики: Настройка всплывающего окна по умолчанию
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/Параметры содержимого
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: DefaultPopupsSetting
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000001
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: DefaultPopupsSetting
  - Пример значения:
``` xml
<integer>1</integer>
```
  

  [В начало](#microsoft-edge:-политики)

  ### DefaultWebBluetoothGuardSetting
  #### Управление использованием веб-API Bluetooth
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Управление доступом веб-сайтов к близлежащим устройствам Bluetooth. Можно полностью заблокировать доступ или обязать сайт отправлять пользователю запрос каждый раз, когда он пытается получить доступ к устройству Bluetooth.

Если не настроить этот параметр политики, используется значение по умолчанию (3, что означает, что пользователь каждый раз получает запрос) и пользователи могут изменять его.

* 2 = Запретить всем сайтам запрашивать доступ к устройствам Bluetooth с помощью веб-интерфейса API Bluetooth

* 3 = Разрешить сайтам отправлять пользователю запрос на доступ к близлежащим устройствам Bluetooth

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Целое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: DefaultWebBluetoothGuardSetting
  - Имя групповой политики: Управление использованием веб-API Bluetooth
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/Параметры содержимого
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: DefaultWebBluetoothGuardSetting
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000002
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: DefaultWebBluetoothGuardSetting
  - Пример значения:
``` xml
<integer>2</integer>
```
  

  [В начало](#microsoft-edge:-политики)

  ### DefaultWebUsbGuardSetting
  #### Управление использованием API WebUSB
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Set whether websites can access connected USB devices. You can completely block access or ask the user each time a website wants to get access to connected USB devices.

You can override this policy for specific URL patterns by using the [WebUsbAskForUrls](#webusbaskforurls) and [WebUsbBlockedForUrls](#webusbblockedforurls) policies.

If you don't configure this policy, sites can ask users whether they can access the connected USB devices (3) by default, and users can change this setting.

* 2 = Don't allow any site to request access to USB devices via the WebUSB API

* 3 = Allow sites to ask the user to grant access to a connected USB device

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Целое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: DefaultWebUsbGuardSetting
  - Имя групповой политики: Управление использованием API WebUSB
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/Параметры содержимого
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: DefaultWebUsbGuardSetting
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000002
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: DefaultWebUsbGuardSetting
  - Пример значения:
``` xml
<integer>2</integer>
```
  

  [В начало](#microsoft-edge:-политики)

  ### ImagesAllowedForUrls
  #### Разрешить изображения на этих сайтах
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Define a list of sites, based on URL patterns, that can display images.

If you don't configure this policy, the global default value is used for all sites either from the [DefaultImagesSetting](#defaultimagessetting) policy (if set) or the user's personal configuration.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Список строк

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: ImagesAllowedForUrls
  - Имя групповой политики: Разрешить изображения на этих сайтах
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/Параметры содержимого
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge\ImagesAllowedForUrls
  - Путь (Рекомендовано): Н/Д
  - Имя значения: 1, 2, 3, ...
  - Тип значения: Список REG_SZ
  ##### Пример значения:
```
SOFTWARE\Policies\Microsoft\Edge\ImagesAllowedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\ImagesAllowedForUrls\1 = "[*.]contoso.edu"

```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: ImagesAllowedForUrls
  - Пример значения:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [В начало](#microsoft-edge:-политики)

  ### ImagesBlockedForUrls
  #### Блокировать изображения на определенных сайтах
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Define a list of sites, based on URL patterns, that aren't allowed to display images.

If you don't configure this policy, the global default value from the [DefaultImagesSetting](#defaultimagessetting) policy (if set) or the user's personal configuration is used for all sites.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Список строк

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: ImagesBlockedForUrls
  - Имя групповой политики: Блокировать изображения на определенных сайтах
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/Параметры содержимого
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge\ImagesBlockedForUrls
  - Путь (Рекомендовано): Н/Д
  - Имя значения: 1, 2, 3, ...
  - Тип значения: Список REG_SZ
  ##### Пример значения:
```
SOFTWARE\Policies\Microsoft\Edge\ImagesBlockedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\ImagesBlockedForUrls\1 = "[*.]contoso.edu"

```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: ImagesBlockedForUrls
  - Пример значения:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [В начало](#microsoft-edge:-политики)

  ### JavaScriptAllowedForUrls
  #### Разрешить скрипты JavaScript на определенных сайтах
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Define a list of sites, based on URL patterns, that are allowed to run JavaScript.

If you don't configure this policy, the global default value from the [DefaultJavaScriptSetting](#defaultjavascriptsetting) policy (if set) or the user's personal configuration is used for all sites.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Список строк

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: JavaScriptAllowedForUrls
  - Имя групповой политики: Разрешить скрипты JavaScript на определенных сайтах
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/Параметры содержимого
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge\JavaScriptAllowedForUrls
  - Путь (Рекомендовано): Н/Д
  - Имя значения: 1, 2, 3, ...
  - Тип значения: Список REG_SZ
  ##### Пример значения:
```
SOFTWARE\Policies\Microsoft\Edge\JavaScriptAllowedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\JavaScriptAllowedForUrls\1 = "[*.]contoso.edu"

```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: JavaScriptAllowedForUrls
  - Пример значения:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [В начало](#microsoft-edge:-политики)

  ### JavaScriptBlockedForUrls
  #### Блокировать скрипты JavaScript на определенных сайтах
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Define a list of sites, based on URL patterns, that aren't allowed to run JavaScript.

If you don't configure this policy, the global default value from the [DefaultJavaScriptSetting](#defaultjavascriptsetting) policy (if set) or the user's personal configuration is used for all sites.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Список строк

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: JavaScriptBlockedForUrls
  - Имя групповой политики: Блокировать скрипты JavaScript на определенных сайтах
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/Параметры содержимого
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge\JavaScriptBlockedForUrls
  - Путь (Рекомендовано): Н/Д
  - Имя значения: 1, 2, 3, ...
  - Тип значения: Список REG_SZ
  ##### Пример значения:
```
SOFTWARE\Policies\Microsoft\Edge\JavaScriptBlockedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\JavaScriptBlockedForUrls\1 = "[*.]contoso.edu"

```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: JavaScriptBlockedForUrls
  - Пример значения:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [В начало](#microsoft-edge:-политики)

  ### NotificationsAllowedForUrls
  #### Разрешить уведомления на определенных сайтах
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Define a list of sites, based on URL patterns, that can display notifications.

If you don't configure this policy, the global default value from the [DefaultNotificationsSetting](#defaultnotificationssetting) policy (if set) or the user's personal configuration is used for all sites.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Список строк

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: NotificationsAllowedForUrls
  - Имя групповой политики: Разрешить уведомления на определенных сайтах
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/Параметры содержимого
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge\NotificationsAllowedForUrls
  - Путь (Рекомендовано): Н/Д
  - Имя значения: 1, 2, 3, ...
  - Тип значения: Список REG_SZ
  ##### Пример значения:
```
SOFTWARE\Policies\Microsoft\Edge\NotificationsAllowedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\NotificationsAllowedForUrls\1 = "[*.]contoso.edu"

```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: NotificationsAllowedForUrls
  - Пример значения:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [В начало](#microsoft-edge:-политики)

  ### NotificationsBlockedForUrls
  #### Блокировать уведомления на определенных сайтах
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Define a list of sites, based on URL patterns, that are blocked from displaying notifications.

If you don't configure this policy, the global default value from the [DefaultNotificationsSetting](#defaultnotificationssetting) policy (if set) or the user's personal configuration is used for all sites.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Список строк

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: NotificationsBlockedForUrls
  - Имя групповой политики: Блокировать уведомления на определенных сайтах
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/Параметры содержимого
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge\NotificationsBlockedForUrls
  - Путь (Рекомендовано): Н/Д
  - Имя значения: 1, 2, 3, ...
  - Тип значения: Список REG_SZ
  ##### Пример значения:
```
SOFTWARE\Policies\Microsoft\Edge\NotificationsBlockedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\NotificationsBlockedForUrls\1 = "[*.]contoso.edu"

```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: NotificationsBlockedForUrls
  - Пример значения:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [В начало](#microsoft-edge:-политики)

  ### PluginsAllowedForUrls
  #### Разрешить подключаемый модуль Adobe Flash на определенных сайтах
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Define a list of sites, based on URL patterns, that can run the Adobe Flash plug-in.

If you don't configure this policy, the global default value from the [DefaultPluginsSetting](#defaultpluginssetting) policy (if set) or the user's personal configuration is used for all sites.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Список строк

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: PluginsAllowedForUrls
  - Имя групповой политики: Разрешить подключаемый модуль Adobe Flash на определенных сайтах
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/Параметры содержимого
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge\PluginsAllowedForUrls
  - Путь (Рекомендовано): Н/Д
  - Имя значения: 1, 2, 3, ...
  - Тип значения: Список REG_SZ
  ##### Пример значения:
```
SOFTWARE\Policies\Microsoft\Edge\PluginsAllowedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\PluginsAllowedForUrls\1 = "[*.]contoso.edu"

```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: PluginsAllowedForUrls
  - Пример значения:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [В начало](#microsoft-edge:-политики)

  ### PluginsBlockedForUrls
  #### Блокировать подключаемый модуль Adobe Flash на определенных сайтах
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Define a list of sites, based on URL patterns, that are blocked from running Adobe Flash.

If you don't configure this policy, the global default value from the [DefaultPluginsSetting](#defaultpluginssetting) policy (if set) or the user's personal configuration is used for all sites.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Список строк

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: PluginsBlockedForUrls
  - Имя групповой политики: Блокировать подключаемый модуль Adobe Flash на определенных сайтах
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/Параметры содержимого
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge\PluginsBlockedForUrls
  - Путь (Рекомендовано): Н/Д
  - Имя значения: 1, 2, 3, ...
  - Тип значения: Список REG_SZ
  ##### Пример значения:
```
SOFTWARE\Policies\Microsoft\Edge\PluginsBlockedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\PluginsBlockedForUrls\1 = "[*.]contoso.edu"

```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: PluginsBlockedForUrls
  - Пример значения:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [В начало](#microsoft-edge:-политики)

  ### PopupsAllowedForUrls
  #### Разрешить всплывающие окна на определенных сайтах
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Define a list of sites, based on URL patterns, that can open pop-up windows.

If you don't configure this policy, the global default value from the [DefaultPopupsSetting](#defaultpopupssetting) policy (if set) or the user's personal configuration is used for all sites.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Список строк

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: PopupsAllowedForUrls
  - Имя групповой политики: Разрешить всплывающие окна на определенных сайтах
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/Параметры содержимого
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge\PopupsAllowedForUrls
  - Путь (Рекомендовано): Н/Д
  - Имя значения: 1, 2, 3, ...
  - Тип значения: Список REG_SZ
  ##### Пример значения:
```
SOFTWARE\Policies\Microsoft\Edge\PopupsAllowedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\PopupsAllowedForUrls\1 = "[*.]contoso.edu"

```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: PopupsAllowedForUrls
  - Пример значения:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [В начало](#microsoft-edge:-политики)

  ### PopupsBlockedForUrls
  #### Блокировать всплывающие окна на определенных сайтах
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Define a list of sites, based on URL patterns, that are blocked from opening pop-up windows.

If you don't configure this policy, the global default value from the [DefaultPopupsSetting](#defaultpopupssetting) policy (if set) or the user's personal configuration is used for all sites.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Список строк

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: PopupsBlockedForUrls
  - Имя групповой политики: Блокировать всплывающие окна на определенных сайтах
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/Параметры содержимого
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge\PopupsBlockedForUrls
  - Путь (Рекомендовано): Н/Д
  - Имя значения: 1, 2, 3, ...
  - Тип значения: Список REG_SZ
  ##### Пример значения:
```
SOFTWARE\Policies\Microsoft\Edge\PopupsBlockedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\PopupsBlockedForUrls\1 = "[*.]contoso.edu"

```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: PopupsBlockedForUrls
  - Пример значения:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [В начало](#microsoft-edge:-политики)

  ### RegisteredProtocolHandlers
  #### Регистрация обработчиков протоколов
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Зарегистрируйте список обработчиков протоколов. Задайте свойство протокола для схемы (например, "mailto") и свойство "url" в шаблоне URL-адреса приложения, которое обрабатывает схему. Шаблон может содержать символ "%s", который будут заменен обработанным URL-адресом.

Вы можете рекомендовать конкретное значение для этого параметра политики, но не можете требовать, чтобы пользователи использовали его.

Обработчики протоколов, зарегистрированные с помощью политики, объединяются со всеми обработчиками, зарегистрированными пользователем, и оба типа доступны для использования. Пользователь может переопределить обработчики протокола, установленные политикой, установив новый обработчик по умолчанию, но они не могут удалять обработчики протокола, зарегистрированные в соответствии политикой.

  #### Поддерживаемые функции:
  - Может быть обязательной: Нет
  - Может быть рекомендованной: Да
  - Динамическое обновление политики: Нет - Требуется перезапуск браузера

  #### Тип данных:
  Словарь

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: RegisteredProtocolHandlers
  - Имя групповой политики: Регистрация обработчиков протоколов
  - Путь групповой политики (Обязательно): Н/Д
  - Путь групповой политики (Рекомендовано): Административные шаблоны/Microsoft Edge - Параметры по умолчанию (пользователи могут переопределять)/Параметры содержимого
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): Н/Д
  - Путь (Рекомендовано): SOFTWARE\Policies\Microsoft\Edge\Рекомендовано
  - Имя значения: RegisteredProtocolHandlers
  - Тип значения: REG_SZ
  ##### Пример значения:
```
SOFTWARE\Policies\Microsoft\Edge\RegisteredProtocolHandlers = [
  {
    "default": true, 
    "protocol": "mailto", 
    "url": "https://mail.contoso.com/mail/?extsrc=mailto&url=%s"
  }
]
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: RegisteredProtocolHandlers
  - Пример значения:
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
  

  [В начало](#microsoft-edge:-политики)

  ### WebUsbAllowDevicesForUrls
  #### Разрешить для определенных сайтов доступ к определенным USB-устройствам
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Allows you to set a list of urls that specify which sites will automatically be granted permission to access a USB device with the given vendor and product IDs. Each item in the list must contain both devices and urls in order for the policy to be valid. Each item in devices can contain a vendor ID and product ID field. Any ID that is omitted is treated as a wildcard with one exception, and that exception is that a product ID cannot be specified without a vendor ID also being specified. Otherwise, the policy will not be valid and will be ignored.

The USB permission model uses the URL of the requesting site ("requesting URL") and the URL of the top-level frame site ("embedding URL") to grant permission to the requesting URL to access the USB device. The requesting URL may be different than the embedding URL when the requesting site is loaded in an iframe. Therefore, the "urls" field can contain up to two URL strings delimited by a comma to specify the requesting and embedding URL respectively. If only one URL is specified, then access to the corresponding USB devices will be granted when the requesting site's URL matches this URL regardless of embedding status. The URLs in "urls" must be valid URLs, otherwise the policy will be ignored.

If this policy is left not set, the global default value will be used for all sites either from the [DefaultWebUsbGuardSetting](#defaultwebusbguardsetting) policy if it is set, or the user's personal configuration otherwise.

URL patterns in this policy should not clash with the ones configured via [WebUsbBlockedForUrls](#webusbblockedforurls). If there is a clash, this policy will take precedence over [WebUsbBlockedForUrls](#webusbblockedforurls) and [WebUsbAskForUrls](#webusbaskforurls).

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Словарь

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: WebUsbAllowDevicesForUrls
  - Имя групповой политики: Разрешить для определенных сайтов доступ к определенным USB-устройствам
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/Параметры содержимого
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: WebUsbAllowDevicesForUrls
  - Тип значения: REG_SZ
  ##### Пример значения:
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


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: WebUsbAllowDevicesForUrls
  - Пример значения:
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
  

  [В начало](#microsoft-edge:-политики)

  ### WebUsbAskForUrls
  #### Разрешить WebUSB на определенных сайтах
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Define a list of sites, based on URL patterns, that can ask the user for access to a USB device.

If you don't configure this policy, the global default value from the [DefaultWebUsbGuardSetting](#defaultwebusbguardsetting) policy (if set) or the user's personal configuration is used for all sites.

The URL patterns defined in this policy can't conflict with those configured in the [WebUsbBlockedForUrls](#webusbblockedforurls) policy - you can't both allow and block a URL.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Список строк

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: WebUsbAskForUrls
  - Имя групповой политики: Разрешить WebUSB на определенных сайтах
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/Параметры содержимого
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge\WebUsbAskForUrls
  - Путь (Рекомендовано): Н/Д
  - Имя значения: 1, 2, 3, ...
  - Тип значения: Список REG_SZ
  ##### Пример значения:
```
SOFTWARE\Policies\Microsoft\Edge\WebUsbAskForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\WebUsbAskForUrls\1 = "[*.]contoso.edu"

```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: WebUsbAskForUrls
  - Пример значения:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [В начало](#microsoft-edge:-политики)

  ### WebUsbBlockedForUrls
  #### Блокировать WebUSB на определенных сайтах
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Define a list of sites, based on URL patterns, that can't ask the user to grant them access to a USB device.

If you don't configure this policy, the global default value from the [DefaultWebUsbGuardSetting](#defaultwebusbguardsetting) policy (if set) or the user's personal configuration is used for all sites.

URL patterns in this policy can't conflict with those configured in the [WebUsbAskForUrls](#webusbaskforurls) policy. You can't both allow and block a URL.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Список строк

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: WebUsbBlockedForUrls
  - Имя групповой политики: Блокировать WebUSB на определенных сайтах
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/Параметры содержимого
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge\WebUsbBlockedForUrls
  - Путь (Рекомендовано): Н/Д
  - Имя значения: 1, 2, 3, ...
  - Тип значения: Список REG_SZ
  ##### Пример значения:
```
SOFTWARE\Policies\Microsoft\Edge\WebUsbBlockedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\WebUsbBlockedForUrls\1 = "[*.]contoso.edu"

```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: WebUsbBlockedForUrls
  - Пример значения:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [В начало](#microsoft-edge:-политики)

  ## Печать policies

  [В начало](#microsoft-edge:-политики)

  ### DefaultPrinterSelection
  #### Правила выбора принтера по умолчанию
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Переопределение правил выбора стандартного принтера в браузере Microsoft Edge. Этот параметр политики определяет правила выбора стандартного принтера в Microsoft Edge. Такой выбор происходит, когда пользователь в первый раз пытается напечатать страницу.

Если этот параметр политики задан, Microsoft Edge находит принтер, который соответствует всем указанным атрибутам, и использует его в качестве стандартного. При наличии нескольких принтеров, которые соответствуют критериям, используется первый подходящий принтер.

Если этот параметр политики не настроен или соответствующие критериям принтеры не найдены в течение заданного времени, стандартным назначается встроенный PDF-принтер или, если PDF-принтер недоступен, не назначается ни один принтер.

Это значение анализируется как объект JSON, соответствующий следующей схеме: { "type": "object", "properties": { "idPattern": { "description": "Regular expression to match printer id.", "type": "string" }, "namePattern": { "description": "Regular expression to match printer display name.", "type": "string" } } }

Пропуск поля означает, что все значения подходят. Например, если не указать подключение, функция предварительного просмотра начинает поиск всех типов локальных принтеров. Шаблоны регулярных выражений должны соответствовать синтаксису JavaScript RegExp. Совпадения определяются с учетом регистра.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Строковое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: DefaultPrinterSelection
  - Имя групповой политики: Правила выбора принтера по умолчанию
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/Печать
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: DefaultPrinterSelection
  - Тип значения: REG_SZ
  ##### Пример значения:
```
"{ "idPattern": ".*public", "namePattern": ".*Color" }"
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: DefaultPrinterSelection
  - Пример значения:
``` xml
<string>{ "idPattern": ".*public", "namePattern": ".*Color" }</string>
```
  

  [В начало](#microsoft-edge:-политики)

  ### PrintHeaderFooter
  #### Печать колонтитулов
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Принудительное включение или отключение колонтитулов в диалоговом окне печати.

Если не настроить этот параметр политики, пользователи смогут включать и отключать печать колонтитулов.

Если этот параметр политики отключен, пользователи не смогут печатать колонтитулы.

Если данный параметр политики включен, пользователи всегда будут печатать верхние и нижние колонтитулы.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Да
  - Динамическое обновление политики: Да

  #### Тип данных:
  Логическое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: PrintHeaderFooter
  - Имя групповой политики: Печать колонтитулов
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/Печать
  - Путь групповой политики (Рекомендовано): Административные шаблоны/Microsoft Edge - Параметры по умолчанию (пользователи могут переопределять)/Печать
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): SOFTWARE\Policies\Microsoft\Edge\Рекомендовано
  - Имя значения: PrintHeaderFooter
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000000
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: PrintHeaderFooter
  - Пример значения:
``` xml
<false/>
```
  

  [В начало](#microsoft-edge:-политики)

  ### PrintPreviewUseSystemDefaultPrinter
  #### Задать системный принтер по умолчанию в качестве принтера по умолчанию
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Назначение стандартного системного принтера в качестве стандартного принтера для предварительного просмотра в Microsoft Edge вместо последнего использованного принтера.

Если этот параметр отключен или не настроен, последний использованный принтер используется в качестве стандартного в режиме предварительного просмотра.

Если этот параметр политики включен, в режиме предварительного просмотра по умолчанию используется стандартный принтер операционной системы.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Да
  - Динамическое обновление политики: Да

  #### Тип данных:
  Логическое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: PrintPreviewUseSystemDefaultPrinter
  - Имя групповой политики: Задать системный принтер по умолчанию в качестве принтера по умолчанию
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/Печать
  - Путь групповой политики (Рекомендовано): Административные шаблоны/Microsoft Edge - Параметры по умолчанию (пользователи могут переопределять)/Печать
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): SOFTWARE\Policies\Microsoft\Edge\Рекомендовано
  - Имя значения: PrintPreviewUseSystemDefaultPrinter
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000000
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: PrintPreviewUseSystemDefaultPrinter
  - Пример значения:
``` xml
<false/>
```
  

  [В начало](#microsoft-edge:-политики)

  ### PrintingEnabled
  #### Включить печать
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Включение печати в Microsoft Edge без возможности для пользователей изменять этот параметр.

Если этот параметр включен или не настроен, пользователи могут печатать.

Если этот параметр политики отключен, пользователи не могут печатать из Microsoft Edge. Печать будет отключена в меню "гаечный ключ", расширениях, приложениях JavaScript и других элементах. Пользователи по-прежнему смогут печатать из подключаемых модулей, которые обходят Microsoft Edge во время печати. Например, некоторые приложения Adobe Flash будут иметь в своем контекстном меню команду печати, на которую не распространяется этот параметр.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Логическое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: PrintingEnabled
  - Имя групповой политики: Включить печать
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/Печать
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: PrintingEnabled
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000001
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: PrintingEnabled
  - Пример значения:
``` xml
<true/>
```
  

  [В начало](#microsoft-edge:-политики)

  ### UseSystemPrintDialog
  #### Печать с помощью системного диалогового окна печати
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Вывод системного диалогового окна печати вместо окна предварительного просмотра.

Если этот параметр включен, Microsoft Edge открывает системное диалоговое окно печати вместо собственного окна предварительного просмотра, когда пользователь пытается выполнить печать.

Если этот параметр выключен или не настроен, при выборе команды печати открывается окно предварительного просмотра Microsoft Edge.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Нет - Требуется перезапуск браузера

  #### Тип данных:
  Логическое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: UseSystemPrintDialog
  - Имя групповой политики: Печать с помощью системного диалогового окна печати
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/Печать
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: UseSystemPrintDialog
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000000
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: UseSystemPrintDialog
  - Пример значения:
``` xml
<false/>
```
  

  [В начало](#microsoft-edge:-политики)

  ## Проверка подлинности HTTP policies

  [В начало](#microsoft-edge:-политики)

  ### AllowCrossOriginAuthPrompt
  #### Разрешить запросы обычной проверки подлинности HTTP независимо от источника
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Определяет для стороннего вложенного содержимого на странице возможность открывать диалоговое окно для обычной проверки подлинности HTTP.

Обычно эта возможность отключена для защиты от фишинга. Если не настроить этот параметр политики, он будет отключен и стороннее вложенное содержимое не сможет открыть диалоговое окно обычной проверки подлинности HTTP.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Логическое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: AllowCrossOriginAuthPrompt
  - Имя групповой политики: Разрешить запросы обычной проверки подлинности HTTP независимо от источника
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/Проверка подлинности HTTP
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: AllowCrossOriginAuthPrompt
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000000
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: AllowCrossOriginAuthPrompt
  - Пример значения:
``` xml
<false/>
```
  

  [В начало](#microsoft-edge:-политики)

  ### AuthNegotiateDelegateAllowlist
  #### Список серверов, которым Microsoft Edge может передавать учетные данные пользователя
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Настройка списка серверов, которым Microsoft Edge может передавать данные.

Можно указать несколько имен серверов через запятую. Допускаются подстановочные знаки (*).

Если не настроить этот параметр политики, Microsoft Edge не будет передавать учетные данные пользователя, даже если сервер определен как входящий в интрасеть.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Нет - Требуется перезапуск браузера

  #### Тип данных:
  Строковое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: AuthNegotiateDelegateAllowlist
  - Имя групповой политики: Список серверов, которым Microsoft Edge может передавать учетные данные пользователя
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/Проверка подлинности HTTP
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: AuthNegotiateDelegateAllowlist
  - Тип значения: REG_SZ
  ##### Пример значения:
```
"contoso.com"
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: AuthNegotiateDelegateAllowlist
  - Пример значения:
``` xml
<string>contoso.com</string>
```
  

  [В начало](#microsoft-edge:-политики)

  ### AuthSchemes
  #### Поддерживаемые схемы проверки подлинности
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Определяет поддерживаемые схемы проверки подлинности HTTP.

Политики можно настроить с помощью следующих значений: "basic", "digest", "ntlm" и "negotiate". Несколько значений следует разделять запятыми.

Если не настроить этот параметр политики, используются все четыре схемы.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Нет - Требуется перезапуск браузера

  #### Тип данных:
  Строковое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: AuthSchemes
  - Имя групповой политики: Поддерживаемые схемы проверки подлинности
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/Проверка подлинности HTTP
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: AuthSchemes
  - Тип значения: REG_SZ
  ##### Пример значения:
```
"basic,digest,ntlm,negotiate"
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: AuthSchemes
  - Пример значения:
``` xml
<string>basic,digest,ntlm,negotiate</string>
```
  

  [В начало](#microsoft-edge:-политики)

  ### AuthServerAllowlist
  #### Настройка списка разрешенных серверов проверки подлинности
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Определение серверов, для которых необходимо включить встроенную проверку подлинности. Встроенная проверка подлинности включается только в том случае, если Microsoft Edge получает запрос проверки подлинности от прокси-сервера или от указанного здесь сервера.

Для разделения нескольких имен серверов используйте запятые. Допускаются подстановочные знаки (*).

Если этот параметр политики не настроен, Microsoft Edge пытается определить, находится ли сервер в интрасети — только в этом случае он будет отвечать на запросы IWA. Если сервер подключен к Интернету, Microsoft Edge будет игнорировать его запросы IWA.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Нет - Требуется перезапуск браузера

  #### Тип данных:
  Строковое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: AuthServerAllowlist
  - Имя групповой политики: Настройка списка разрешенных серверов проверки подлинности
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/Проверка подлинности HTTP
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: AuthServerAllowlist
  - Тип значения: REG_SZ
  ##### Пример значения:
```
"*contoso.com,contoso.com"
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: AuthServerAllowlist
  - Пример значения:
``` xml
<string>*contoso.com,contoso.com</string>
```
  

  [В начало](#microsoft-edge:-политики)

  ### DisableAuthNegotiateCnameLookup
  #### Отключить поиск CNAME при согласовании проверки подлинности Kerberos
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Определяется основа для создания SPN Kerberos — каноническое имя DNS (CNAME) или исходное введенное имя.

Если этот параметр включен, поиск CNAME пропускается и используется имя сервера (введенное).

Если этот параметр выключен или не настроен, используется каноническое имя сервера, определяемое с помощью поиска CNAME.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Нет - Требуется перезапуск браузера

  #### Тип данных:
  Логическое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: DisableAuthNegotiateCnameLookup
  - Имя групповой политики: Отключить поиск CNAME при согласовании проверки подлинности Kerberos
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/Проверка подлинности HTTP
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: DisableAuthNegotiateCnameLookup
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000000
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: DisableAuthNegotiateCnameLookup
  - Пример значения:
``` xml
<false/>
```
  

  [В начало](#microsoft-edge:-политики)

  ### EnableAuthNegotiatePort
  #### Включить нестандартный порт в SPN Kerberos
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Определяет, должен ли созданный SPN Kerberos включать нестандартный порт.

Если данный параметр политики включен, и пользователь включает в URL-адрес нестандартный порт (не порт 80 или 443), этот порт включается в созданный SPN Kerberos.

Если не настроить или отключить этот параметр политики, созданный SPN Kerberos не будет включать порт в любом случае.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Нет - Требуется перезапуск браузера

  #### Тип данных:
  Логическое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: EnableAuthNegotiatePort
  - Имя групповой политики: Включить нестандартный порт в SPN Kerberos
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/Проверка подлинности HTTP
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: EnableAuthNegotiatePort
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000000
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: EnableAuthNegotiatePort
  - Пример значения:
``` xml
<false/>
```
  

  [В начало](#microsoft-edge:-политики)

  ### NtlmV2Enabled
  #### Управление включением и отключением проверки подлинности NTLMv2
  >Поддерживаемые версии: Microsoft Edge на Mac с 77 или более поздней версии

  #### Описание
  Определяет, включен ли NTLMv2.

Все последние версии серверов Samba и Windows поддерживают NTLMv2. Отключать NTLMv2 следует только для устранения проблем с обратной совместимостью, так как это снизит безопасность проверки подлинности.

Если этот параметр политики не настроен, NTLMv2 включен по умолчанию.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Логическое

  

  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: NtlmV2Enabled
  - Пример значения:
``` xml
<true/>
```
  

  [В начало](#microsoft-edge:-политики)

  ## Прокси-сервер policies

  [В начало](#microsoft-edge:-политики)

  ### ProxyBypassList
  #### Настройка правил обхода прокси-сервера
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Defines a list of hosts for which Microsoft Edge bypasses any proxy.

This policy is applied only if you have selected 'Use fixed proxy servers' in the [ProxyMode](#proxymode) policy. If you selected any other mode for configuring proxy policies, don't enable or configure this policy.

If you enable this policy, you can create a list of hosts for which Microsoft Edge doesn't use a proxy.

If you don't configure this policy, no list of hosts is created for which Microsoft Edge bypasses a proxy. Leave this policy unconfigured if you've specified any other method for setting proxy policies.

For more detailed examples go to [https://go.microsoft.com/fwlink/?linkid=2094936](https://go.microsoft.com/fwlink/?linkid=2094936).

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Строковое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: ProxyBypassList
  - Имя групповой политики: Настройка правил обхода прокси-сервера
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/Прокси-сервер
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: ProxyBypassList
  - Тип значения: REG_SZ
  ##### Пример значения:
```
"https://www.contoso.com, https://www.fabrikam.com"
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: ProxyBypassList
  - Пример значения:
``` xml
<string>https://www.contoso.com, https://www.fabrikam.com</string>
```
  

  [В начало](#microsoft-edge:-политики)

  ### ProxyMode
  #### Настройка параметров прокси-сервера
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
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

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Строковое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: ProxyMode
  - Имя групповой политики: Настройка параметров прокси-сервера
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/Прокси-сервер
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: ProxyMode
  - Тип значения: REG_SZ
  ##### Пример значения:
```
"direct"
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: ProxyMode
  - Пример значения:
``` xml
<string>direct</string>
```
  

  [В начало](#microsoft-edge:-политики)

  ### ProxyPacUrl
  #### Настроить URL-адрес PAC-файла прокси-сервера
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Specifies the URL for a proxy auto-config (PAC) file.

This policy is applied only if you selected 'Use a .pac proxy script' in the [ProxyMode](#proxymode) policy. If you selected any other mode for configuring proxy policies, don't enable or configure this policy.

If you enable this policy, you can specify the URL for a PAC file, which defines how the browser automatically chooses the appropriate proxy server for fetching a particular website.

If you disable or don't configure this policy, no PAC file is specified. Leave this policy unconfigured if you've specified any other method for setting proxy policies.

For detailed examples, see [https://go.microsoft.com/fwlink/?linkid=2094936](https://go.microsoft.com/fwlink/?linkid=2094936).

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Строковое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: ProxyPacUrl
  - Имя групповой политики: Настроить URL-адрес PAC-файла прокси-сервера
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/Прокси-сервер
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: ProxyPacUrl
  - Тип значения: REG_SZ
  ##### Пример значения:
```
"https://internal.contoso.com/example.pac"
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: ProxyPacUrl
  - Пример значения:
``` xml
<string>https://internal.contoso.com/example.pac</string>
```
  

  [В начало](#microsoft-edge:-политики)

  ### ProxyServer
  #### Настройка адреса или URL-адреса прокси-сервера
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Specifies the URL of the proxy server.

This policy is applied only if you have selected 'Use fixed proxy servers' in the [ProxyMode](#proxymode) policy. If you selected any other mode for configuring proxy policies, don't enable or configure this policy.

If you enable this policy, the proxy server configured by this policy will be used for all URLs.

If you disable or don't configure this policy, users can choose their own proxy settings while in this proxy mode. Leave this policy unconfigured if you've specified any other method for setting proxy policies.

For more options and detailed examples, see [https://go.microsoft.com/fwlink/?linkid=2094936](https://go.microsoft.com/fwlink/?linkid=2094936).

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Строковое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: ProxyServer
  - Имя групповой политики: Настройка адреса или URL-адреса прокси-сервера
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/Прокси-сервер
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: ProxyServer
  - Тип значения: REG_SZ
  ##### Пример значения:
```
"123.123.123.123:8080"
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: ProxyServer
  - Пример значения:
``` xml
<string>123.123.123.123:8080</string>
```
  

  [В начало](#microsoft-edge:-политики)

  ### ProxySettings
  #### Параметры прокси-сервера
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
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

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Словарь

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: ProxySettings
  - Имя групповой политики: Параметры прокси-сервера
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/Прокси-сервер
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: ProxySettings
  - Тип значения: REG_SZ
  ##### Пример значения:
```
SOFTWARE\Policies\Microsoft\Edge\ProxySettings = {
  "ProxyBypassList": "https://www.example1.com,https://www.example2.com,https://internalsite/", 
  "ProxyMode": "direct", 
  "ProxyPacUrl": "https://internal.site/example.pac", 
  "ProxyServer": "123.123.123.123:8080"
}
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: ProxySettings
  - Пример значения:
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
  

  [В начало](#microsoft-edge:-политики)

  ## Расширения policies

  [В начало](#microsoft-edge:-политики)

  ### ExtensionAllowedTypes
  #### Настройка разрешенных типов расширений
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Controls which extension types can be installed and limits runtime access.

This setting defines the allowed types of extensions and which hosts they can interact with. The value is a list of strings, each of which should be one of the following: "extension", "theme", "user_script", and "hosted_app". See the Microsoft Edge extensions documentation for more information on these types.

Note that this policy also affects extensions to be force-installed by using [ExtensionInstallForcelist](#extensioninstallforcelist) policy.

If you enable this policy, only extensions that match a type in the list are installed.

If you don't configure this policy, no restrictions on the acceptable extension types are enforced.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Список строк

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: ExtensionAllowedTypes
  - Имя групповой политики: Настройка разрешенных типов расширений
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/Расширения
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge\ExtensionAllowedTypes
  - Путь (Рекомендовано): Н/Д
  - Имя значения: 1, 2, 3, ...
  - Тип значения: Список REG_SZ
  ##### Пример значения:
```
SOFTWARE\Policies\Microsoft\Edge\ExtensionAllowedTypes\0 = "hosted_app"

```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: ExtensionAllowedTypes
  - Пример значения:
``` xml
<array>
  <string>hosted_app</string>
</array>
```
  

  [В начало](#microsoft-edge:-политики)

  ### ExtensionInstallAllowlist
  #### Разрешить установку определенных расширений
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  По умолчанию разрешены все расширения. Тем не менее, если вы заблокируете все расширения, задав для параметра политики "ExtensionInstallBlockList" значение "*", пользователи смогут устанавливать только расширения, определенные в этой политике.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Список строк

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: ExtensionInstallAllowlist
  - Имя групповой политики: Разрешить установку определенных расширений
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/Расширения
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallAllowlist
  - Путь (Рекомендовано): Н/Д
  - Имя значения: 1, 2, 3, ...
  - Тип значения: Список REG_SZ
  ##### Пример значения:
```
SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallAllowlist\0 = "extension_id1"
SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallAllowlist\1 = "extension_id2"

```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: ExtensionInstallAllowlist
  - Пример значения:
``` xml
<array>
  <string>extension_id1</string>
  <string>extension_id2</string>
</array>
```
  

  [В начало](#microsoft-edge:-политики)

  ### ExtensionInstallBlocklist
  #### Управление расширениями, которые нельзя устанавливать
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Определение списка конкретных расширений, которые пользователи НЕ могут устанавливать в Microsoft Edge. При развертывании этого параметра все установленные ранее расширения из данного списка отключаются и пользователь не может их включить. Если удалить расширение из списка заблокированных, оно будет автоматически повторно включено в том месте, где было установлено ранее.

Используйте "*" для блокировки всех расширений, не указанных явным образом в списке разрешенных.

Если этот параметр не настроен, пользователи могут установить любое расширение в Microsoft Edge.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Список строк

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: ExtensionInstallBlocklist
  - Имя групповой политики: Управление расширениями, которые нельзя устанавливать
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/Расширения
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallBlocklist
  - Путь (Рекомендовано): Н/Д
  - Имя значения: 1, 2, 3, ...
  - Тип значения: Список REG_SZ
  ##### Пример значения:
```
SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallBlocklist\0 = "extension_id1"
SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallBlocklist\1 = "extension_id2"

```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: ExtensionInstallBlocklist
  - Пример значения:
``` xml
<array>
  <string>extension_id1</string>
  <string>extension_id2</string>
</array>
```
  

  [В начало](#microsoft-edge:-политики)

  ### ExtensionInstallForcelist
  #### Определение автоматически устанавливаемых расширений
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
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

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Список строк

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: ExtensionInstallForcelist
  - Имя групповой политики: Определение автоматически устанавливаемых расширений
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/Расширения
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallForcelist
  - Путь (Рекомендовано): Н/Д
  - Имя значения: 1, 2, 3, ...
  - Тип значения: Список REG_SZ
  ##### Пример значения:
```
SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallForcelist\0 = "gbchcmhmhahfdphkhkmpfmihenigjmpp;https://edge.microsoft.com/extensionwebstorebase/v1/crx"
SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallForcelist\1 = "abcdefghijklmnopabcdefghijklmnop"

```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: ExtensionInstallForcelist
  - Пример значения:
``` xml
<array>
  <string>gbchcmhmhahfdphkhkmpfmihenigjmpp;https://edge.microsoft.com/extensionwebstorebase/v1/crx</string>
  <string>abcdefghijklmnopabcdefghijklmnop</string>
</array>
```
  

  [В начало](#microsoft-edge:-политики)

  ### ExtensionInstallSources
  #### Настройка источников установки расширений и пользовательских скриптов
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Define URLs that can install extensions and themes.

By default, users have to download a *.crx file for each extension or script they want to install, and then drag it onto the Microsoft Edge settings page. This policy lets specific URLs use install the extension or script for the user.

Each item in this list is an extension-style match pattern (see [https://go.microsoft.com/fwlink/?linkid=2095039](https://go.microsoft.com/fwlink/?linkid=2095039)). Users can easily install items from any URL that matches an item in this list. Both the location of the *.crx file and the page where the download is started from (in other words, the referrer) must be allowed by these patterns.

The [ExtensionInstallBlocklist](#extensioninstallblocklist) policy takes precedence over this policy. Any extensions that's on the block list won't be installed, even if it comes from a site on this list.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Список строк

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: ExtensionInstallSources
  - Имя групповой политики: Настройка источников установки расширений и пользовательских скриптов
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/Расширения
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallSources
  - Путь (Рекомендовано): Н/Д
  - Имя значения: 1, 2, 3, ...
  - Тип значения: Список REG_SZ
  ##### Пример значения:
```
SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallSources\0 = "https://corp.contoso.com/*"

```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: ExtensionInstallSources
  - Пример значения:
``` xml
<array>
  <string>https://corp.contoso.com/*</string>
</array>
```
  

  [В начало](#microsoft-edge:-политики)

  ### ExtensionSettings
  #### Настройка параметров управления расширениями
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Настройка параметров управления расширениями для Microsoft Edge.

Этот параметр политики определяет множество настроек, включая настройки, управляемые любыми текущими политиками, связанными с расширениями. Он также переопределяет все устаревшие политики, если они еще настроены.

Этот параметр политики сопоставляет идентификатор расширения или URL-адрес обновления со своей настройкой. При использовании идентификатора расширения настройка применяется только к указанному расширению. Используйте стандартную настройку для специального идентификатора "*", чтобы применить ее ко всем расширениям, которые конкретно не указаны в этом параметре политики. При использовании URL-адреса обновления настройка применяется ко всем расширениям с точным URL-адресом обновления, указанном в манифесте этого расширения, как описано на странице [https://go.microsoft.com/fwlink/?linkid=2095043](https://go.microsoft.com/fwlink/?linkid=2095043).

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Словарь

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: ExtensionSettings
  - Имя групповой политики: Настройка параметров управления расширениями
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/Расширения
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: ExtensionSettings
  - Тип значения: REG_SZ
  ##### Пример значения:
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


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: ExtensionSettings
  - Пример значения:
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
  

  [В начало](#microsoft-edge:-политики)

  ## Служба поиска по умолчанию policies

  [В начало](#microsoft-edge:-политики)

  ### DefaultSearchProviderEnabled
  #### Включить службу поиска по умолчанию
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Включает использование поисковой системы по умолчанию.

Если данный параметр политики включен, пользователь может искать слово, введя его в адресной строке (при условии, что он не вводит URL-адрес).

Вы можете указать службу поиска по умолчанию для использования, включив остальные политики поиска по умолчанию. Если оставить эти значения пустыми (не настроенными), пользователь сможет выбрать поисковую систему по умолчанию.

Если этот параметр политики отключен, пользователи не смогут выполнять поиск из адресной строки.

Если этот параметр политики включен или отключен, пользователи не смогут переопределить его.

Если не настроить этот параметр политики, будет включена служба поиска по умолчанию, при этом пользователь сможет выбрать службу поиска по умолчанию и настроить список служб поиска.

Эта политика доступна только для экземпляров Windows, входящих в состав домена Microsoft Active Directory, Windows 10 Pro или экземпляров предприятия, зарегистрированных для управления устройствами.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Логическое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: DefaultSearchProviderEnabled
  - Имя групповой политики: Включить службу поиска по умолчанию
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/Служба поиска по умолчанию
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: DefaultSearchProviderEnabled
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000001
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: DefaultSearchProviderEnabled
  - Пример значения:
``` xml
<true/>
```
  

  [В начало](#microsoft-edge:-политики)

  ### DefaultSearchProviderEncodings
  #### Кодировки службы поиска по умолчанию
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Specify the character encodings supported by the search provider. Encodings are code page names like UTF-8, GB2312, and ISO-8859-1. They are tried in the order provided.

This policy is optional. If not configured, the default, UTF-8, is used.

This policy is applied only if you enable the [DefaultSearchProviderEnabled](#defaultsearchproviderenabled) and [DefaultSearchProviderSearchURL](#defaultsearchprovidersearchurl) policies.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Список строк

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: DefaultSearchProviderEncodings
  - Имя групповой политики: Кодировки службы поиска по умолчанию
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/Служба поиска по умолчанию
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge\DefaultSearchProviderEncodings
  - Путь (Рекомендовано): Н/Д
  - Имя значения: 1, 2, 3, ...
  - Тип значения: Список REG_SZ
  ##### Пример значения:
```
SOFTWARE\Policies\Microsoft\Edge\DefaultSearchProviderEncodings\0 = "UTF-8"
SOFTWARE\Policies\Microsoft\Edge\DefaultSearchProviderEncodings\1 = "UTF-16"
SOFTWARE\Policies\Microsoft\Edge\DefaultSearchProviderEncodings\2 = "GB2312"
SOFTWARE\Policies\Microsoft\Edge\DefaultSearchProviderEncodings\3 = "ISO-8859-1"

```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: DefaultSearchProviderEncodings
  - Пример значения:
``` xml
<array>
  <string>UTF-8</string>
  <string>UTF-16</string>
  <string>GB2312</string>
  <string>ISO-8859-1</string>
</array>
```
  

  [В начало](#microsoft-edge:-политики)

  ### DefaultSearchProviderImageURL
  #### Определяет функцию поиска по изображению для системы поиска по умолчанию
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Specifies the URL to the search engine used for image search. Search requests are sent using the GET method.

This policy is optional. If you don't configure it, image search isn't available.

Specify Bing's Image Search URL as:
'{bing:baseURL}images/detail/search?iss=sbiupload&FORM=ANCMS1#enterInsights'.

Specify Google's Image Search URL as: '{google:baseURL}searchbyimage/upload'.

See [DefaultSearchProviderImageURLPostParams](#defaultsearchproviderimageurlpostparams) policy to finish configuring image search.

This policy is applied only if you enable the [DefaultSearchProviderEnabled](#defaultsearchproviderenabled) and [DefaultSearchProviderSearchURL](#defaultsearchprovidersearchurl) policies.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Строковое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: DefaultSearchProviderImageURL
  - Имя групповой политики: Определяет функцию поиска по изображению для системы поиска по умолчанию
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/Служба поиска по умолчанию
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: DefaultSearchProviderImageURL
  - Тип значения: REG_SZ
  ##### Пример значения:
```
"https://search.contoso.com/searchbyimage/upload"
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: DefaultSearchProviderImageURL
  - Пример значения:
``` xml
<string>https://search.contoso.com/searchbyimage/upload</string>
```
  

  [В начало](#microsoft-edge:-политики)

  ### DefaultSearchProviderImageURLPostParams
  #### Параметры для URL-адреса изображения при использовании метода POST
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  If you enable this policy, it specifies the parameters used when an image search that uses POST is performed. The policy consists of comma-separated name/value pairs. If a value is a template parameter, like {imageThumbnail} in the preceding example, it’s replaced with real image thumbnail data. This policy is applied only if you enable the [DefaultSearchProviderEnabled](#defaultsearchproviderenabled) and [DefaultSearchProviderSearchURL](#defaultsearchprovidersearchurl) policies.

Specify Bing's Image Search URL Post Params as:
'imageBin={google:imageThumbnailBase64}'.

Specify Google's Image Search URL Post Params as:
'encoded_image={google:imageThumbnail},image_url={google:imageURL},sbisrc={google:imageSearchSource},original_width={google:imageOriginalWidth},original_height={google:imageOriginalHeight}'.

If you don’t set this policy, image search requests are sent using the GET method.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Строковое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: DefaultSearchProviderImageURLPostParams
  - Имя групповой политики: Параметры для URL-адреса изображения при использовании метода POST
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/Служба поиска по умолчанию
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: DefaultSearchProviderImageURLPostParams
  - Тип значения: REG_SZ
  ##### Пример значения:
```
"content={imageThumbnail},url={imageURL},sbisrc={SearchSource}"
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: DefaultSearchProviderImageURLPostParams
  - Пример значения:
``` xml
<string>content={imageThumbnail},url={imageURL},sbisrc={SearchSource}</string>
```
  

  [В начало](#microsoft-edge:-политики)

  ### DefaultSearchProviderKeyword
  #### Ключевое слово службы поиска по умолчанию
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Specifies the keyword, which is the shortcut used in the Address Bar to trigger the search for this provider.

This policy is optional. If you don't configure it, no keyword activates the search provider.

This policy is applied only if you enable the [DefaultSearchProviderEnabled](#defaultsearchproviderenabled) and [DefaultSearchProviderSearchURL](#defaultsearchprovidersearchurl) policies.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Строковое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: DefaultSearchProviderKeyword
  - Имя групповой политики: Ключевое слово службы поиска по умолчанию
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/Служба поиска по умолчанию
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: DefaultSearchProviderKeyword
  - Тип значения: REG_SZ
  ##### Пример значения:
```
"mis"
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: DefaultSearchProviderKeyword
  - Пример значения:
``` xml
<string>mis</string>
```
  

  [В начало](#microsoft-edge:-политики)

  ### DefaultSearchProviderName
  #### Имя службы поиска по умолчанию
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Specifies the name of the default search provider.

If you enable this policy, you set the name of the default search provider.

If you don't enable this policy or if you leave it empty, the host name specified by the search URL is used.

'DefaultSearchProviderName' should be set to an organization-approved encrypted search provider that corresponds to the encrypted search provider set in DTBC-0008. This policy is applied only if you enable the [DefaultSearchProviderEnabled](#defaultsearchproviderenabled) and [DefaultSearchProviderSearchURL](#defaultsearchprovidersearchurl) policies.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Строковое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: DefaultSearchProviderName
  - Имя групповой политики: Имя службы поиска по умолчанию
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/Служба поиска по умолчанию
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: DefaultSearchProviderName
  - Тип значения: REG_SZ
  ##### Пример значения:
```
"My Intranet Search"
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: DefaultSearchProviderName
  - Пример значения:
``` xml
<string>My Intranet Search</string>
```
  

  [В начало](#microsoft-edge:-политики)

  ### DefaultSearchProviderSearchURL
  #### Поисковый URL-адрес службы поиска по умолчанию
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Specifies the URL of the search engine used for a default search. The URL contains the string '{searchTerms}', which is replaced at query time by the terms the user is searching for.

Specify Bing's search URL as:

'{bing:baseURL}search?q={searchTerms}'.

Specify Google's search URL as: '{google:baseURL}search?q={searchTerms}&{google:RLZ}{google:originalQueryForSuggestion}{google:assistedQueryStats}{google:searchFieldtrialParameter}{google:searchClient}{google:sourceId}ie={inputEncoding}'.

This policy is required when you enable the [DefaultSearchProviderEnabled](#defaultsearchproviderenabled) policy; if you don't enable the latter policy, this policy is ignored.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Строковое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: DefaultSearchProviderSearchURL
  - Имя групповой политики: Поисковый URL-адрес службы поиска по умолчанию
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/Служба поиска по умолчанию
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: DefaultSearchProviderSearchURL
  - Тип значения: REG_SZ
  ##### Пример значения:
```
"https://search.contoso.com/search?q={searchTerms}"
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: DefaultSearchProviderSearchURL
  - Пример значения:
``` xml
<string>https://search.contoso.com/search?q={searchTerms}</string>
```
  

  [В начало](#microsoft-edge:-политики)

  ### DefaultSearchProviderSuggestURL
  #### URL-адреса службы поиска по умолчанию для предложений
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Specifies the URL for the search engine used to provide search suggestions. The URL contains the string '{searchTerms}', which is replaced at query time by the text the user has entered so far.

This policy is optional. If you don't configure it, users won't see search suggestions; they will see suggestions from their browsing history and favorites.

Bing's suggest URL can be specified as:

'{bing:baseURL}qbox?query={searchTerms}'.

Google's suggest URL can be specified as: '{google:baseURL}complete/search?output=chrome&q={searchTerms}'.

This policy is applied only if you enable the [DefaultSearchProviderEnabled](#defaultsearchproviderenabled) and [DefaultSearchProviderSearchURL](#defaultsearchprovidersearchurl) policies.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Строковое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: DefaultSearchProviderSuggestURL
  - Имя групповой политики: URL-адреса службы поиска по умолчанию для предложений
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/Служба поиска по умолчанию
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: DefaultSearchProviderSuggestURL
  - Тип значения: REG_SZ
  ##### Пример значения:
```
"https://search.contoso.com/suggest?q={searchTerms}"
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: DefaultSearchProviderSuggestURL
  - Пример значения:
``` xml
<string>https://search.contoso.com/suggest?q={searchTerms}</string>
```
  

  [В начало](#microsoft-edge:-политики)

  ## Собственный обмен сообщениями policies

  [В начало](#microsoft-edge:-политики)

  ### NativeMessagingAllowlist
  #### Управление узлами собственного обмена сообщениями, которые могут использовать пользователи
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  List specific native messaging hosts that users can use in Microsoft Edge.

By default, all native messaging hosts are allowed. If you set the [NativeMessagingBlocklist](#nativemessagingblocklist) policy to *, all native messaging hosts are blocked, and only native messaging hosts listed in here are loaded.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Список строк

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: NativeMessagingAllowlist
  - Имя групповой политики: Управление узлами собственного обмена сообщениями, которые могут использовать пользователи
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/Собственный обмен сообщениями
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge\NativeMessagingAllowlist
  - Путь (Рекомендовано): Н/Д
  - Имя значения: 1, 2, 3, ...
  - Тип значения: Список REG_SZ
  ##### Пример значения:
```
SOFTWARE\Policies\Microsoft\Edge\NativeMessagingAllowlist\0 = "com.native.messaging.host.name1"
SOFTWARE\Policies\Microsoft\Edge\NativeMessagingAllowlist\1 = "com.native.messaging.host.name2"

```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: NativeMessagingAllowlist
  - Пример значения:
``` xml
<array>
  <string>com.native.messaging.host.name1</string>
  <string>com.native.messaging.host.name2</string>
</array>
```
  

  [В начало](#microsoft-edge:-политики)

  ### NativeMessagingBlocklist
  #### Настроить список блокировки для собственного обмена сообщениями
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Определение запрещенных узлов собственного обмена сообщениями.

Символ "*" позволяет заблокировать все узлы собственного обмена сообщениями, не указанные явным образом в списке разрешенных узлов.

Если не настроить этот параметр политики, Microsoft Edge будет загружать все установленные узлы собственного обмена сообщениями.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Список строк

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: NativeMessagingBlocklist
  - Имя групповой политики: Настроить список блокировки для собственного обмена сообщениями
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/Собственный обмен сообщениями
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge\NativeMessagingBlocklist
  - Путь (Рекомендовано): Н/Д
  - Имя значения: 1, 2, 3, ...
  - Тип значения: Список REG_SZ
  ##### Пример значения:
```
SOFTWARE\Policies\Microsoft\Edge\NativeMessagingBlocklist\0 = "com.native.messaging.host.name1"
SOFTWARE\Policies\Microsoft\Edge\NativeMessagingBlocklist\1 = "com.native.messaging.host.name2"

```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: NativeMessagingBlocklist
  - Пример значения:
``` xml
<array>
  <string>com.native.messaging.host.name1</string>
  <string>com.native.messaging.host.name2</string>
</array>
```
  

  [В начало](#microsoft-edge:-политики)

  ### NativeMessagingUserLevelHosts
  #### Разрешить узлы собственного обмена сообщениями на уровне пользователя (установленные без разрешений администратора)
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Установка узлов собственного обмена сообщениями на уровне пользователя.

Если данный параметр политики отключен, Microsoft Edge использует только узлы собственного обмена сообщениями, установленные на уровне системы.

Если этот параметр политики не настроен, в Microsoft Edge по умолчанию разрешается использование узлов собственного обмена сообщениями на уровне пользователя.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Логическое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: NativeMessagingUserLevelHosts
  - Имя групповой политики: Разрешить узлы собственного обмена сообщениями на уровне пользователя (установленные без разрешений администратора)
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/Собственный обмен сообщениями
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: NativeMessagingUserLevelHosts
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000000
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: NativeMessagingUserLevelHosts
  - Пример значения:
``` xml
<false/>
```
  

  [В начало](#microsoft-edge:-политики)

  ## Additional policies

  [В начало](#microsoft-edge:-политики)

  ### AdsSettingForIntrusiveAdsSites
  #### Настройка рекламы для сайтов с навязчивой рекламой
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 78 или более поздней версии

  #### Описание
  Блокировка объявлений на сайтах с навязчивой рекламой. Для этого параметра политики можно задать один из следующих вариантов.

* 1 = Разрешить рекламу на всех сайтах.

* 2 = Блокировать объявления на сайтах с навязчивой рекламой (по умолчанию).

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Целое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: AdsSettingForIntrusiveAdsSites
  - Имя групповой политики: Настройка рекламы для сайтов с навязчивой рекламой
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: AdsSettingForIntrusiveAdsSites
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000001
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: AdsSettingForIntrusiveAdsSites
  - Пример значения:
``` xml
<integer>1</integer>
```
  

  [В начало](#microsoft-edge:-политики)

  ### AllowDeletingBrowserHistory
  #### Включить удаление журнала браузера и журнала загрузок
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Удаление журнала браузера и журнала скачиваний без возможности для пользователей изменять этот параметр.

Обратите внимание: даже если этот параметр политики отключен, журнал браузера и журнал скачиваний не обязательно будут сохраняться, так как пользователи могут изменить или удалить файлы базы данных журнала, а сам браузер может в любое время удалить (на основании срока действия) или заархивировать некоторые или все элементы журнала.

Если этот параметр включен или не настроен, пользователи могут удалять журнал браузера и журнал скачиваний.

Если этот параметр политики отключен, пользователи не могут удалять журнал браузера и журнал скачиваний.

Если этот параметр политики включен, не включайте параметр "Удалять данные о просмотре веб-страниц при закрытии Microsoft Edge", так как оба эти параметра связаны с удалением данных. В противном случае параметр "Удалять данные о просмотре веб-страниц при закрытии Microsoft Edge" будет иметь приоритет и все данные будут удаляться при закрытии Microsoft Edge независимо от настройки данного параметра.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Логическое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: AllowDeletingBrowserHistory
  - Имя групповой политики: Включить удаление журнала браузера и журнала загрузок
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: AllowDeletingBrowserHistory
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000001
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: AllowDeletingBrowserHistory
  - Пример значения:
``` xml
<true/>
```
  

  [В начало](#microsoft-edge:-политики)

  ### AllowFileSelectionDialogs
  #### Разрешить диалоговые окна выбора файлов
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Доступ к локальным файлам через диалоговые окна выбора файлов в Microsoft Edge.

Если включить или не настроить этот параметр политики, пользователи смогут открывать диалоговые окна выбора файлов в обычном режиме.

Если отключить этот параметр политики, при каждом действии пользователя, запускающем диалоговое окно выбора файлов (например, импорт избранного, загрузка файлов или сохранение ссылок), выводится сообщение и пользователь должен нажать кнопку "Отмена" в диалоговом окне выбора файлов.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Логическое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: AllowFileSelectionDialogs
  - Имя групповой политики: Разрешить диалоговые окна выбора файлов
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: AllowFileSelectionDialogs
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000001
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: AllowFileSelectionDialogs
  - Пример значения:
``` xml
<true/>
```
  

  [В начало](#microsoft-edge:-политики)

  ### AllowPopupsDuringPageUnload
  #### Позволяет странице отображать всплывающие окна во время ее выгрузки
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 78 или более поздней версии

  #### Описание
  Эта политика позволяет администратору указать, что страница может отображать всплывающие окна во время ее выгрузки.

Если этот параметр политики включен, страницам разрешено отображать всплывающие окна во время выгрузки.

Если этот параметр политики отключен или не определен, страницы не смогут отображать всплывающие окна во время выгрузки. Это относится к следующей спецификации: (https://html.spec.whatwg.org/#apis-for-creating-and-navigating-browsing-contexts-by-name).

Эта политика будет удалена в будущем.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Нет - Требуется перезапуск браузера

  #### Тип данных:
  Логическое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: AllowPopupsDuringPageUnload
  - Имя групповой политики: Позволяет странице отображать всплывающие окна во время ее выгрузки
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: AllowPopupsDuringPageUnload
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000000
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: AllowPopupsDuringPageUnload
  - Пример значения:
``` xml
<false/>
```
  

  [В начало](#microsoft-edge:-политики)

  ### AllowSyncXHRInPageDismissal
  #### Разрешить отправку синхронных запросов XHR при закрытии страницы
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 79 или более поздней версии

  #### Описание
  Эта политика позволяет разрешить отправку синхронных запросов XHR при закрытии страницы.

Если данный параметр политики включен, синхронные запросы XHR могут отправляться при закрытии страниц.

Если данный параметр политики отключен или не настроен, синхронные запросы XHR не могут отправляться при закрытии страниц.

Этот параметр политики является временным и будет удален в одном из будущих выпусков.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Нет - Требуется перезапуск браузера

  #### Тип данных:
  Логическое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: AllowSyncXHRInPageDismissal
  - Имя групповой политики: Разрешить отправку синхронных запросов XHR при закрытии страницы
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: AllowSyncXHRInPageDismissal
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000000
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: AllowSyncXHRInPageDismissal
  - Пример значения:
``` xml
<false/>
```
  

  [В начало](#microsoft-edge:-политики)

  ### AllowTrackingForUrls
  #### Настроить исключения из блокировки отслеживания для определенных сайтов
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 78 или более поздней версии

  #### Описание
  Настройка списка шаблонов URL-адресов, исключаемых из блокировки отслеживания.

Если этот параметр политики настроен, список заданных шаблонов URL-адресов исключается из блокировки отслеживания.

Если этот параметр политики не настроен, для всех сайтов используется глобальное стандартное значение параметра "Блокировка отслеживания просмотренных веб-страниц" (если установлено) или персональная настройка пользователя.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Список строк

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: AllowTrackingForUrls
  - Имя групповой политики: Настроить исключения из блокировки отслеживания для определенных сайтов
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge\AllowTrackingForUrls
  - Путь (Рекомендовано): Н/Д
  - Имя значения: 1, 2, 3, ...
  - Тип значения: Список REG_SZ
  ##### Пример значения:
```
SOFTWARE\Policies\Microsoft\Edge\AllowTrackingForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\AllowTrackingForUrls\1 = "[*.]contoso.edu"

```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: AllowTrackingForUrls
  - Пример значения:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [В начало](#microsoft-edge:-политики)

  ### AlwaysOpenPdfExternally
  #### Всегда открывать PDF-файлы извне
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Отключение встроенного средства просмотра PDF-файлов в Microsoft Edge.

Если данный параметр политики включен, Microsoft Edge рассматривает PDF-файлы как загрузки и пользователи могут открывать их с помощью стандартного приложения.

Если не настроить этот параметр политики или отключить его, Microsoft Edge будет открывать PDF-файлы (если пользователь не отключит эту функцию).

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Логическое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: AlwaysOpenPdfExternally
  - Имя групповой политики: Всегда открывать PDF-файлы извне
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: AlwaysOpenPdfExternally
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000001
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: AlwaysOpenPdfExternally
  - Пример значения:
``` xml
<true/>
```
  

  [В начало](#microsoft-edge:-политики)

  ### ApplicationLocaleValue
  #### Настроить язык приложения
  >Поддерживаемые версии: Microsoft Edge на Windows с 77 или более поздней версии

  #### Описание
  Определение языкового стандарта приложения в Microsoft Edge без возможности для пользователей изменять этот параметр.

Если данный параметр политики включен, Microsoft Edge использует указанный языковой стандарт. Если настроенный языковой стандарт не поддерживается, вместо него используется "en-US".

Если отключить или не настроить этот параметр, Microsoft Edge использует указанный пользователем предпочтительный языковой стандарт (если настроен) или базовый языковой стандарт "en-US".

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Да
  - Динамическое обновление политики: Нет - Требуется перезапуск браузера

  #### Тип данных:
  Строковое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: ApplicationLocaleValue
  - Имя групповой политики: Настроить язык приложения
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Административные шаблоны/Microsoft Edge - Параметры по умолчанию (пользователи могут переопределять)/
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): SOFTWARE\Policies\Microsoft\Edge\Рекомендовано
  - Имя значения: ApplicationLocaleValue
  - Тип значения: REG_SZ
  ##### Пример значения:
```
"en"
```


  

  [В начало](#microsoft-edge:-политики)

  ### AudioCaptureAllowed
  #### Разрешить или запретить запись звука
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Allows you to set whether a user is prompted to grant a website access to their audio capture device. This policy applies to all URLs except for those configured in the [AudioCaptureAllowedUrls](#audiocaptureallowedurls) list.

If you enable this policy or don't configure it (the default setting), the user is prompted for audio capture access except from the URLs in the [AudioCaptureAllowedUrls](#audiocaptureallowedurls) list. These listed URLs are granted access without prompting.

If you disable this policy, the user is not prompted, and audio capture is accessible only to the URLs configured in [AudioCaptureAllowedUrls](#audiocaptureallowedurls).

This policy affects all types of audio inputs, not only the built-in microphone.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Логическое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: AudioCaptureAllowed
  - Имя групповой политики: Разрешить или запретить запись звука
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: AudioCaptureAllowed
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000000
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: AudioCaptureAllowed
  - Пример значения:
``` xml
<false/>
```
  

  [В начало](#microsoft-edge:-политики)

  ### AudioCaptureAllowedUrls
  #### Сайты, которые могут получать доступ к устройствам записи звука без запроса разрешения
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  На основании шаблонов URL-адресов укажите веб-сайты, которые могут использовать устройства записи звука, без запроса разрешения пользователя. Шаблоны в этом списке сопоставляются с источником безопасности запрашивающего URL-адреса. Если они совпадают, сайту автоматически предоставляется доступ к устройствам записи звука.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Список строк

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: AudioCaptureAllowedUrls
  - Имя групповой политики: Сайты, которые могут получать доступ к устройствам записи звука без запроса разрешения
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge\AudioCaptureAllowedUrls
  - Путь (Рекомендовано): Н/Д
  - Имя значения: 1, 2, 3, ...
  - Тип значения: Список REG_SZ
  ##### Пример значения:
```
SOFTWARE\Policies\Microsoft\Edge\AudioCaptureAllowedUrls\0 = "https://www.contoso.com/"
SOFTWARE\Policies\Microsoft\Edge\AudioCaptureAllowedUrls\1 = "https://[*.]contoso.edu/"

```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: AudioCaptureAllowedUrls
  - Пример значения:
``` xml
<array>
  <string>https://www.contoso.com/</string>
  <string>https://[*.]contoso.edu/</string>
</array>
```
  

  [В начало](#microsoft-edge:-политики)

  ### AutoImportAtFirstRun
  #### Автоматически импортировать данные и параметры другого браузера при первом запуске
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Если данный параметр политики включен, Microsoft Edge автоматически импортирует все поддерживаемые типы данных и параметры из стандартного или другого указанного браузера. При этом Microsoft Edge пропускает пункт импорта при первом запуске.

Если для этого параметра политики задано значение DisabledAutoImport (4), пункт импорта при первом запуске пропускается полностью и Microsoft Edge не импортирует данные и параметры браузера автоматически.

* 0 = Автоматически импортирует все поддерживаемые типы данных и параметры из стандартного браузера

* 1 = Автоматически импортирует все поддерживаемые типы данных и параметры из Internet Explorer

* 2 = Автоматически импортирует все поддерживаемые типы данных и параметры из Google Chrome

* 3 = Автоматически импортирует все поддерживаемые типы данных и параметры из Safari

* 4 = Автоматический импорт отключается, и пункт импорта при первом запуске пропускается

**Примечание**. Сейчас этот параметр политики поддерживает импорт из браузеров Internet Explorer (в Windows 7, 8 и 10), Google Chrome (в Windows 7, 8, 10 и в macOS) и Apple Safari (в macOS).

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Нет - Требуется перезапуск браузера

  #### Тип данных:
  Целое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: AutoImportAtFirstRun
  - Имя групповой политики: Автоматически импортировать данные и параметры другого браузера при первом запуске
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: AutoImportAtFirstRun
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000002
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: AutoImportAtFirstRun
  - Пример значения:
``` xml
<integer>2</integer>
```
  

  [В начало](#microsoft-edge:-политики)

  ### AutofillAddressEnabled
  #### Включить автозаполнение для адресов
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Включение функции автозаполнения для автоматического ввода сохраненных адресов в веб-формах.

Если этот параметр политики отключен, функция автозаполнения никогда не предлагает и не вводит информацию об адресах, а также не сохраняет дополнительные сведения об адресе, которые пользователь может отправить при просмотре веб-страниц.

Если этот параметр включен или не настроен, пользователи могут управлять функцией автозаполнения адресов в пользовательском интерфейсе.

Примечание. Отключив этот параметр политики, вы также остановите все действия для любых веб-форм, за исключением форм оплаты и паролей. Дальнейшие записи не будут сохраняться, и Microsoft Edge не будет предлагать или автоматически вводить какие-либо предыдущие записи.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Да
  - Динамическое обновление политики: Да

  #### Тип данных:
  Логическое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: AutofillAddressEnabled
  - Имя групповой политики: Включить автозаполнение для адресов
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Административные шаблоны/Microsoft Edge - Параметры по умолчанию (пользователи могут переопределять)/
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): SOFTWARE\Policies\Microsoft\Edge\Рекомендовано
  - Имя значения: AutofillAddressEnabled
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000000
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: AutofillAddressEnabled
  - Пример значения:
``` xml
<false/>
```
  

  [В начало](#microsoft-edge:-политики)

  ### AutofillCreditCardEnabled
  #### Включить автозаполнение для кредитных карт
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Включение функции автозаполнения в Microsoft Edge, которая автоматически вносит данные кредитных карт в веб-формы, используя ранее сохраненные сведения.

Если этот параметр политики отключен, функция автозаполнения никогда не предлагает и не вносит данные кредитных карт, а также не сохраняет дополнительные сведения о кредитной карте, которые пользователи могут отправлять при просмотре веб-страниц.

Если этот параметр политики включен или не настроен, пользователи могут управлять функцией автозаполнения в отношении сведений о кредитных картах.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Да
  - Динамическое обновление политики: Да

  #### Тип данных:
  Логическое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: AutofillCreditCardEnabled
  - Имя групповой политики: Включить автозаполнение для кредитных карт
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Административные шаблоны/Microsoft Edge - Параметры по умолчанию (пользователи могут переопределять)/
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): SOFTWARE\Policies\Microsoft\Edge\Рекомендовано
  - Имя значения: AutofillCreditCardEnabled
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000000
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: AutofillCreditCardEnabled
  - Пример значения:
``` xml
<false/>
```
  

  [В начало](#microsoft-edge:-политики)

  ### AutoplayAllowed
  #### Разрешить автозапуск мультимедиа для веб-сайтов
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 78 или более поздней версии

  #### Описание
  Определение правил автозапуска мультимедиа для веб-сайтов.

Если выбран стандартный вариант "Не настроено", соблюдаются текущие настройки автозапуска мультимедиа, которые пользователь может изменить.

Если выбран вариант "Включено", для автозапуска устанавливается значение "Разрешить". Всем сайтам будет разрешено автоматически запускать мультимедиа, и пользователи не смогут переопределить этот параметр политики.

Если выбран вариант "Выключено", для автозапуска устанавливается значение "Запретить". Всем сайтам будет запрещено автоматически запускать мультимедиа, и пользователи не смогут переопределить этот параметр политики.

Чтобы параметр вступил в силу, необходимо закрыть и снова открыть вкладку.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Логическое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: AutoplayAllowed
  - Имя групповой политики: Разрешить автозапуск мультимедиа для веб-сайтов
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: AutoplayAllowed
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000001
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: AutoplayAllowed
  - Пример значения:
``` xml
<true/>
```
  

  [В начало](#microsoft-edge:-политики)

  ### BackgroundModeEnabled
  #### Разрешить фоновым приложениям продолжать работу после закрытия Microsoft Edge
  >Поддерживаемые версии: Microsoft Edge на Windows с 77 или более поздней версии

  #### Описание
  Процессы Microsoft Edge запускаются при входе в ОС и продолжают работу после закрытия последнего окна браузера. В этом сценарии фоновые приложения и текущий сеанс браузера остаются активными, включая все файлы cookie сеанса. На панели задач отображается значок выполняемого фонового процесса, с помощью которого этот процесс можно в любой момент остановить.

Если данный параметр политики включен, фоновый режим включен.

Если этот параметр политики отключен, фоновый режим отключен.

Если этот параметр политики не настроен, фоновый режим изначально отключен и пользователи могут управлять им в разделе edge://settings/system.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Да
  - Динамическое обновление политики: Да

  #### Тип данных:
  Логическое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: BackgroundModeEnabled
  - Имя групповой политики: Разрешить фоновым приложениям продолжать работу после закрытия Microsoft Edge
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Административные шаблоны/Microsoft Edge - Параметры по умолчанию (пользователи могут переопределять)/
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): SOFTWARE\Policies\Microsoft\Edge\Рекомендовано
  - Имя значения: BackgroundModeEnabled
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000001
```


  

  [В начало](#microsoft-edge:-политики)

  ### BackgroundTemplateListUpdatesEnabled
  #### Включение фонового обновления списка доступных шаблонов для коллекций и других функций, использующих шаблоны.
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 79 или более поздней версии

  #### Описание
  Включение или отключение фонового обновления списка доступных шаблонов для коллекций и других функций, использующих шаблоны. Шаблоны используются для извлечения многоформатных метаданных из веб-страницы при сохранении страницы в коллекции.

Если этот параметр включен или не настроен, список доступных шаблонов будет загружаться в фоновом режиме из службы Майкрософт каждые 24 часа.

Если этот параметр отключен, список доступных шаблонов будет загружаться по требованию. Этот тип загрузки может привести к снижению производительности коллекций и других функций.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Логическое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: BackgroundTemplateListUpdatesEnabled
  - Имя групповой политики: Включение фонового обновления списка доступных шаблонов для коллекций и других функций, использующих шаблоны.
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: BackgroundTemplateListUpdatesEnabled
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000001
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: BackgroundTemplateListUpdatesEnabled
  - Пример значения:
``` xml
<true/>
```
  

  [В начало](#microsoft-edge:-политики)

  ### BlockThirdPartyCookies
  #### Блокировать сторонние файлы cookie
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Блокировать задание файлов cookie элементами веб-страницы, не принадлежащими домену, который указан в адресной строке.

Если данный параметр политики включен, элементы веб-страницы, которые не принадлежат домену, указанному в адресной строке, не могут задавать файлы cookie

Если этот параметр политики отключен, элементы веб-страницы из доменов, не относящихся к домену, указанному в адресной строке, могут задавать файлы cookie.

Если не настроить этот параметр политики, будут включены сторонние файлы cookie, но пользователи смогут изменить этот параметр.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Да
  - Динамическое обновление политики: Да

  #### Тип данных:
  Логическое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: BlockThirdPartyCookies
  - Имя групповой политики: Блокировать сторонние файлы cookie
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Административные шаблоны/Microsoft Edge - Параметры по умолчанию (пользователи могут переопределять)/
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): SOFTWARE\Policies\Microsoft\Edge\Рекомендовано
  - Имя значения: BlockThirdPartyCookies
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000000
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: BlockThirdPartyCookies
  - Пример значения:
``` xml
<false/>
```
  

  [В начало](#microsoft-edge:-политики)

  ### BrowserAddProfileEnabled
  #### Разрешить создание профиля во всплывающем меню "Удостоверение" или на странице "Параметры"
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Создание новых профилей с помощью команды **Добавить профиль**.
Если этот параметр политики включен или не настроен, в Microsoft Edge можно создавать новые профили с помощью команды **Добавить профиль** во всплывающем меню "Удостоверение" или на странице "Параметры".

Если этот параметр политики отключен, пользователи не могут добавлять новые профили во всплывающем меню "Удостоверение" или на странице "Параметры".

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Логическое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: BrowserAddProfileEnabled
  - Имя групповой политики: Разрешить создание профиля во всплывающем меню "Удостоверение" или на странице "Параметры"
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: BrowserAddProfileEnabled
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000001
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: BrowserAddProfileEnabled
  - Пример значения:
``` xml
<true/>
```
  

  [В начало](#microsoft-edge:-политики)

  ### BrowserGuestModeEnabled
  #### Включить режим гостя
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Использование гостевых профилей в Microsoft Edge. При использовании такого профиля браузер не импортирует данные о просмотре веб-страниц из имеющихся профилей и удаляет эти данные после закрытия всех гостевых профилей.

Если этот параметр политики включен или не настроен, пользователи могут просматривать веб-страницы в Microsoft Edge в гостевых профилях.

Если этот параметр политики отключен, пользователи не могут просматривать веб-страницы в Microsoft Edge в гостевых профилях.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Логическое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: BrowserGuestModeEnabled
  - Имя групповой политики: Включить режим гостя
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: BrowserGuestModeEnabled
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000001
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: BrowserGuestModeEnabled
  - Пример значения:
``` xml
<true/>
```
  

  [В начало](#microsoft-edge:-политики)

  ### BrowserNetworkTimeQueriesEnabled
  #### Разрешить запросы к сетевой службе времени браузера
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Запрет периодической отправки запросов из Microsoft Edge в сетевую службу времени браузера для получения точной метки времени.

Если отключить этот параметр политики, Microsoft Edge прекратит отправку запросов в сетевую службу времени браузера.

Если этот параметр включен или не настроен, Microsoft Edge периодически отправляет запросы в сетевую службу времени браузера.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Логическое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: BrowserNetworkTimeQueriesEnabled
  - Имя групповой политики: Разрешить запросы к сетевой службе времени браузера
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: BrowserNetworkTimeQueriesEnabled
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000001
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: BrowserNetworkTimeQueriesEnabled
  - Пример значения:
``` xml
<true/>
```
  

  [В начало](#microsoft-edge:-политики)

  ### BrowserSignin
  #### Параметры входа браузера
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Specify whether a user can sign into Microsoft Edge with their account and use account-related services like sync and single sign on. To control the availability of sync, use the [SyncDisabled](#syncdisabled) policy instead.

If you set this policy to 'Disable browser sign-in', make sure that you also set the [NonRemovableProfileEnabled](#nonremovableprofileenabled) policy to disabled because [NonRemovableProfileEnabled](#nonremovableprofileenabled) disables the creation of an automatically signed in browser profile. If both policies are set, Microsoft Edge will use the 'Disable browser sign-in' policy and behave as if [NonRemovableProfileEnabled](#nonremovableprofileenabled) is set to disabled.

If you set this policy to 'Enable browser sign-in' (1), users can sign into the browser. Signing into the browser doesn't mean that sync is turned on by default; the user must separately opt-in to use this feature.

If you set this policy to 'Force browser sign-in' (2) users must sign into a profile to use the browser. By default, this will allow the user to choose whether they want to sync to their account, unless sync is disabled by the domain admin or with the [SyncDisabled](#syncdisabled) policy. The default value of [BrowserGuestModeEnabled](#browserguestmodeenabled) policy is set to false.

If you don't configure this policy users can decide if they want to enable the browser sign-in option and use it as they see fit.

* 0 = Disable browser sign-in

* 1 = Enable browser sign-in

* 2 = Force users to sign-in to use the browser

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Нет - Требуется перезапуск браузера

  #### Тип данных:
  Целое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: BrowserSignin
  - Имя групповой политики: Параметры входа браузера
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: BrowserSignin
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000002
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: BrowserSignin
  - Пример значения:
``` xml
<integer>2</integer>
```
  

  [В начало](#microsoft-edge:-политики)

  ### BuiltInDnsClientEnabled
  #### Использовать встроенный DNS-клиент
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Определяет, следует ли использовать встроенный DNS-клиент.

Если данный параметр политики включен, используется встроенный DNS-клиент, если он доступен.

Если этот параметр политики отключен, этот клиент никогда не используется.

Если не настроить этот параметр политики, встроенный DNS-клиент будет включен по умолчанию для MacOS, и пользователи смогут изменять возможности использования встроенного DNS-клиента, изменив edge://flags или указав флаг командной строки.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Логическое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: BuiltInDnsClientEnabled
  - Имя групповой политики: Использовать встроенный DNS-клиент
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: BuiltInDnsClientEnabled
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000001
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: BuiltInDnsClientEnabled
  - Пример значения:
``` xml
<true/>
```
  

  [В начало](#microsoft-edge:-политики)

  ### CertificateTransparencyEnforcementDisabledForCas
  #### Отключить обязательную проверку прозрачности сертификатов для списка хэш-значений subjectPublicKeyInfo
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Отключает принудительное применение требований к прозрачности сертификата для списка хэш-данных subjectPublicKeyInfo.

Этот параметр политики разрешает отключать требования к публикации с помощью функции прозрачности сертификата для цепочек сертификатов, которые содержат сертификаты с одним из указанных хэшей subjectPublicKeyInfo. Этот параметр разрешает и дальше использовать для узлов предприятия сертификаты, которые считались бы в противном случае недоверенными, так как они не были правильно опубликованы.

Чтобы отключить принудительное применение прозрачности сертификата, когда задан этот параметр политики, должен выполняться один из следующих наборов условий.
1. Хэш включен в сведения subjectPublicKeyInfo сертификата сервера.
2. Хэш включен в сведения subjectPublicKeyInfo, содержащиеся в сертификате ЦС в цепочке сертификатов; этот сертификат ЦС ограничен через расширение X.509v3 nameConstraints; один или несколько атрибутов directoryName nameConstraints присутствуют в permittedSubtrees; directoryName содержит атрибут organizationName.
3. Хэш включен в сведения subjectPublicKeyInfo, содержащиеся в сертификате ЦС цепочки сертификатов; этот сертификат ЦС содержит один или несколько атрибутов organizationName в поле субъекта сертификата; сертификат сервера содержит то же количество атрибутов organizationName с одинаковыми значениями по байтам и в том же порядке.

Хэш subjectPublicKeyInfo задается путем объединения имени алгоритма хэша, символа "/" и кодировки Base64 этого алгоритма хэша, примененной к сведениям subjectPublicKeyInfo в DER-кодировке в указанном сертификате. Кодировка Base64 имеет тот же формат, что и SPKI Fingerprint в соответствии с разделом 2.4 RFC 7469. Нераспознанные алгоритмы хэша игнорируются. Единственным поддерживаемым алгоритмом хэша в настоящее время является "sha256".

Если этот параметр политики отключен или не задан, любой сертификат, который должен быть опубликован с помощью функции прозрачности сертификата, будет считаться недоверенным, если он не опубликован в соответствии с политикой прозрачности сертификата.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Список строк

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: CertificateTransparencyEnforcementDisabledForCas
  - Имя групповой политики: Отключить обязательную проверку прозрачности сертификатов для списка хэш-значений subjectPublicKeyInfo
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge\CertificateTransparencyEnforcementDisabledForCas
  - Путь (Рекомендовано): Н/Д
  - Имя значения: 1, 2, 3, ...
  - Тип значения: Список REG_SZ
  ##### Пример значения:
```
SOFTWARE\Policies\Microsoft\Edge\CertificateTransparencyEnforcementDisabledForCas\0 = "sha256/AAAAAAAAAAAAAAAAAAAAAA=="
SOFTWARE\Policies\Microsoft\Edge\CertificateTransparencyEnforcementDisabledForCas\1 = "sha256//////////////////////w=="

```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: CertificateTransparencyEnforcementDisabledForCas
  - Пример значения:
``` xml
<array>
  <string>sha256/AAAAAAAAAAAAAAAAAAAAAA==</string>
  <string>sha256//////////////////////w==</string>
</array>
```
  

  [В начало](#microsoft-edge:-политики)

  ### CertificateTransparencyEnforcementDisabledForLegacyCas
  #### Отключить обязательную проверку прозрачности сертификатов для списка устаревших центров сертификации
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Отключение принудительного применения политики прозрачности сертификатов для списка устаревших центров сертификации (ЦС).

Этот параметр политики позволяет отключить требования к прозрачной отправке сертификатов для цепочек, содержащих сертификаты с одним из указанных хэшей subjectPublicKeyInfo. Благодаря этому для корпоративных узлов продолжают использоваться сертификаты, которые иначе считались бы недоверенными из-за неправильной отправки.

Чтобы отключить принудительное применение политики прозрачности сертификатов, необходимо присвоить хэшу значение subjectPublicKeyInfo, которое отображается в сертификате ЦС и распознается как устаревший Центр сертификации (ЦС). Устаревший ЦС — это общедоступный ЦС, которому по умолчанию доверяли одна или несколько операционных систем, совместимых с Microsoft Edge.

Хэш subjectPublicKeyInfo указывается путем объединения имени хэш-алгоритма, символа "/" и кодировки Base64 этого хэш-алгоритма, применяемого к значению subjectPublicKeyInfo в кодировке DER для указанного сертификата. Данная кодировка Base64 представляет тот же формат, что и отпечаток SPKI, согласно RFC 7469, раздел 2.4. Нераспознанные хэш-алгоритмы игнорируются. Единственным поддерживаемым хэш-алгоритмом в данный момент является "sha256".

Когда этот параметр не настроен, любой сертификат, который должен быть отправлен с применением политики прозрачности сертификатов, считается недоверенным, если он не был отправлен в соответствии с этой политикой.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Список строк

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: CertificateTransparencyEnforcementDisabledForLegacyCas
  - Имя групповой политики: Отключить обязательную проверку прозрачности сертификатов для списка устаревших центров сертификации
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge\CertificateTransparencyEnforcementDisabledForLegacyCas
  - Путь (Рекомендовано): Н/Д
  - Имя значения: 1, 2, 3, ...
  - Тип значения: Список REG_SZ
  ##### Пример значения:
```
SOFTWARE\Policies\Microsoft\Edge\CertificateTransparencyEnforcementDisabledForLegacyCas\0 = "sha256/AAAAAAAAAAAAAAAAAAAAAA=="
SOFTWARE\Policies\Microsoft\Edge\CertificateTransparencyEnforcementDisabledForLegacyCas\1 = "sha256//////////////////////w=="

```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: CertificateTransparencyEnforcementDisabledForLegacyCas
  - Пример значения:
``` xml
<array>
  <string>sha256/AAAAAAAAAAAAAAAAAAAAAA==</string>
  <string>sha256//////////////////////w==</string>
</array>
```
  

  [В начало](#microsoft-edge:-политики)

  ### CertificateTransparencyEnforcementDisabledForUrls
  #### Отключить обязательную проверку прозрачности сертификатов для определенных URL-адресов
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Отключение принудительного применения политики прозрачности сертификатов для заданных URL-адресов.

Этот параметр политики позволяет не передавать сертификаты для имен узлов на указанных URL-адресах с применением политики прозрачности сертификатов. Это означает, что вы можете использовать сертификаты, которые в противном случае считались бы недоверенными из-за неправильной передачи, однако при этом усложняется определение неправильно изданных сертификатов для таких узлов.

Сформируйте шаблон URL-адреса в соответствии с рекомендациями, изложенными на странице [https://go.microsoft.com/fwlink/?linkid=2095322](https://go.microsoft.com/fwlink/?linkid=2095322). Так как сертификаты являются действительными для заданного имени узла независимо от схемы, порта или пути, в URL-адресе учитывается только часть имени узла. Узлы с подстановочными знаками не поддерживаются.

Когда этот параметр политики не настроен, любой сертификат, который должен быть передан с применением политики прозрачности сертификатов, считается недоверенным, если он не был передан.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Список строк

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: CertificateTransparencyEnforcementDisabledForUrls
  - Имя групповой политики: Отключить обязательную проверку прозрачности сертификатов для определенных URL-адресов
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge\CertificateTransparencyEnforcementDisabledForUrls
  - Путь (Рекомендовано): Н/Д
  - Имя значения: 1, 2, 3, ...
  - Тип значения: Список REG_SZ
  ##### Пример значения:
```
SOFTWARE\Policies\Microsoft\Edge\CertificateTransparencyEnforcementDisabledForUrls\0 = "contoso.com"
SOFTWARE\Policies\Microsoft\Edge\CertificateTransparencyEnforcementDisabledForUrls\1 = ".contoso.com"

```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: CertificateTransparencyEnforcementDisabledForUrls
  - Пример значения:
``` xml
<array>
  <string>contoso.com</string>
  <string>.contoso.com</string>
</array>
```
  

  [В начало](#microsoft-edge:-политики)

  ### ClearBrowsingDataOnExit
  #### Удалять данные о просмотре веб-страниц при закрытии Microsoft Edge
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 78 или более поздней версии

  #### Описание
  Microsoft Edge doesn't clear the browsing data by default when it closes. Browsing data includes information entered in forms, passwords, and even the websites visited.

If you enable this policy, all browsing data is deleted each time Microsoft Edge closes.

If you disable or don't configure this policy, users can configure the Clear browsing data option in Settings.

If you enable this policy, don't enable the [AllowDeletingBrowserHistory](#allowdeletingbrowserhistory) policy, because they both deal with deleting data. If you enable both, this policy takes precedence and deletes all data when Microsoft Edge closes, regardless of how you configured [AllowDeletingBrowserHistory](#allowdeletingbrowserhistory).

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Да
  - Динамическое обновление политики: Нет - Требуется перезапуск браузера

  #### Тип данных:
  Логическое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: ClearBrowsingDataOnExit
  - Имя групповой политики: Удалять данные о просмотре веб-страниц при закрытии Microsoft Edge
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Административные шаблоны/Microsoft Edge - Параметры по умолчанию (пользователи могут переопределять)/
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): SOFTWARE\Policies\Microsoft\Edge\Рекомендовано
  - Имя значения: ClearBrowsingDataOnExit
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000001
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: ClearBrowsingDataOnExit
  - Пример значения:
``` xml
<true/>
```
  

  [В начало](#microsoft-edge:-политики)

  ### ClickOnceEnabled
  #### Разрешить пользователям открывать файлы с помощью протокола ClickOnce
  >Поддерживаемые версии: Microsoft Edge на Windows с 78 или более поздней версии

  #### Описание
  Разрешить пользователям открывать файлы с помощью протокола ClickOnce. Протокол ClickOnce позволяет веб-сайтам запрашивать открытие файлов в браузере с определенного URL-адреса с помощью обработчика файлов ClickOnce на компьютере или другом устройстве пользователя.

Если данный параметр политики включен, пользователи могут открывать файлы с помощью протокола ClickOnce. Этот параметр переопределяет настройку ClickOnce, заданную пользователем на странице edge://flags/.

Если данный параметр политики отключен, пользователи не могут открывать файлы с помощью протокола ClickOnce. В этом случае файл сохраняется в файловой системе через браузер. Этот параметр переопределяет настройку ClickOnce, заданную пользователем на странице edge://flags/.

Если не настроить этот параметр политики, пользователи не смогут открывать файлы с помощью протокола ClickOnce. Пользователи могут разрешить использование протокола ClickOnce на странице edge://flags/.

Запрет ClickOnce может препятствовать нормальному запуску приложений ClickOnce (файлов .application).

Дополнительные сведения о ClickOnce см. на страницах [https://go.microsoft.com/fwlink/?linkid=2103872](https://go.microsoft.com/fwlink/?linkid=2103872) и [https://go.microsoft.com/fwlink/?linkid=2099880](https://go.microsoft.com/fwlink/?linkid=2099880).

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Логическое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: ClickOnceEnabled
  - Имя групповой политики: Разрешить пользователям открывать файлы с помощью протокола ClickOnce
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: ClickOnceEnabled
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000000
```


  

  [В начало](#microsoft-edge:-политики)

  ### CommandLineFlagSecurityWarningsEnabled
  #### Включить предупреждения системы безопасности для флагов командной строки
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 78 или более поздней версии

  #### Описание
  Если этот параметр отключен, при запуске Microsoft Edge с потенциально опасными флагами командной строки предупреждения системы безопасности не отображаются.

Если этот параметр включен или не настроен, при запуске Microsoft Edge с такими флагами командной строки предупреждения системы безопасности отображаются.

Например, флаг "--disable-gpu-sandbox" вызывает такое предупреждение: "Вы используете неподдерживаемый флаг командной строки: --disable-gpu-sandbox. Это создает угрозу стабильности и безопасности".

В Windows этот параметр доступен только в экземплярах, присоединенных к домену Microsoft Active Directory, либо экземплярах Windows 10 Pro или Windows 10 Корпоративная, зарегистрированных для управления устройствами.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Нет - Требуется перезапуск браузера

  #### Тип данных:
  Логическое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: CommandLineFlagSecurityWarningsEnabled
  - Имя групповой политики: Включить предупреждения системы безопасности для флагов командной строки
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: CommandLineFlagSecurityWarningsEnabled
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000001
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: CommandLineFlagSecurityWarningsEnabled
  - Пример значения:
``` xml
<true/>
```
  

  [В начало](#microsoft-edge:-политики)

  ### ComponentUpdatesEnabled
  #### Включить обновления компонентов в Microsoft Edge
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Если включить или не настроить этот параметр политики, в Microsoft Edge будет выполняться обновление компонентов.

Если отключить этот параметр политики или задать для него значение false, обновление будет отключено для всех компонентов в Microsoft Edge.

Из этого параметра, однако, исключены некоторые компоненты, например все компоненты, которые не содержат исполняемый код, не имеют существенного влияния на поведение браузера или имеют важное значение для безопасности. Это означает, что обновления, которые считаются "критически важными для безопасности", будут применяться, даже если данный параметр будет отключен.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Нет - Требуется перезапуск браузера

  #### Тип данных:
  Логическое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: ComponentUpdatesEnabled
  - Имя групповой политики: Включить обновления компонентов в Microsoft Edge
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: ComponentUpdatesEnabled
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000001
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: ComponentUpdatesEnabled
  - Пример значения:
``` xml
<true/>
```
  

  [В начало](#microsoft-edge:-политики)

  ### ConfigureDoNotTrack
  #### Настроить запросы "Не отслеживать"
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Настройка запросов "Не отслеживать" для веб-сайтов, запрашивающих данные отслеживания. Запросы "Не отслеживать" сообщают веб-сайтам, которые вы посещаете, о том, что вы не хотите, чтобы ваши действия в сети отслеживались. По умолчанию Microsoft Edge не отправляет запросы "Не отслеживать", но пользователи могут включить данную функцию для отправки таких запросов.

Если этот параметр политики включен, запросы "Не отслеживать" всегда отправляются на веб-сайты, запрашивающие данные отслеживания.

Если отключить этот параметр политики, запросы не будут отправляться.

Если не настроить этот параметр политики, пользователи смогут разрешить или запретить отправку таких запросов.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Логическое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: ConfigureDoNotTrack
  - Имя групповой политики: Настроить запросы "Не отслеживать"
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: ConfigureDoNotTrack
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000000
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: ConfigureDoNotTrack
  - Пример значения:
``` xml
<false/>
```
  

  [В начало](#microsoft-edge:-политики)

  ### ConfigureOnlineTextToSpeech
  #### Настройка преобразования текста в речь в сети
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Этот параметр политики позволяет указать, можно ли в браузере использовать голоса веб-службы преобразования текста в речь (в рамках Azure Cognitive Services). Эти голоса имеют более высокое качество, чем предустановленные в системе голоса.

Если этот параметр политики включен или не настроен, веб-приложения, использующие API SpeechSynthesis, могут использовать голоса веб-службы преобразования текста в речь.

Если этот параметр политики выключен, такие голоса недоступны.

Ниже указано, где можно узнать больше об этой функции.
API SpeechSynthesis: https://developer.mozilla.org/en-US/docs/Web/API/SpeechSynthesis
Службы Cognitive Services: https://azure.microsoft.com/en-us/services/cognitive-services/text-to-speech/

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Логическое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: ConfigureOnlineTextToSpeech
  - Имя групповой политики: Настройка преобразования текста в речь в сети
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: ConfigureOnlineTextToSpeech
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000001
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: ConfigureOnlineTextToSpeech
  - Пример значения:
``` xml
<true/>
```
  

  [В начало](#microsoft-edge:-политики)

  ### CustomHelpLink
  #### Указание настраиваемой ссылки для справки
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 79 или более поздней версии

  #### Описание
  Указание ссылки для меню "Справка" или клавиши F1.

Если включить эту политику, администратор может указать ссылку для меню "Справка" или клавиши F1.

Если отключить или не настроить эту политику, для меню "Справка" или клавиши F1 используется стандартная ссылка.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Строковое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: CustomHelpLink
  - Имя групповой политики: Указание настраиваемой ссылки для справки
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: CustomHelpLink
  - Тип значения: REG_SZ
  ##### Пример значения:
```
"https://go.microsoft.com/fwlink/?linkid=2080734"
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: CustomHelpLink
  - Пример значения:
``` xml
<string>https://go.microsoft.com/fwlink/?linkid=2080734</string>
```
  

  [В начало](#microsoft-edge:-политики)

  ### DefaultBrowserSettingEnabled
  #### Назначить Microsoft Edge стандартным браузером
  >Поддерживаемые версии: Microsoft Edge на Windows 7 и Mac с 77 или более поздней версии

  #### Описание
  Настройка стандартных проверок браузера в Microsoft Edge без возможности для пользователей изменять этот параметр.

Если этот параметр включен, Microsoft Edge всегда проверяет при запуске, является ли он стандартным браузером, и автоматически регистрирует себя (если это возможно).

Если этот параметр отключен, Microsoft Edge никогда не выполняет проверку и отключает пользовательские элементы управления для настройки этого параметра.

Если этот параметр политики не настроен, пользователь может назначить Microsoft Edge стандартным браузером, а также включить или выключить уведомления для случаев, когда этот браузер не является стандартным.

Примечание для администраторов Windows. Этот параметр политики работает только для компьютеров под управлением Windows 7. В более поздних версиях Windows необходимо развернуть файл "сопоставления приложений по умолчанию", который назначает Microsoft Edge обработчиком протоколов HTTPS и HTTP (а также, дополнительно, протокола FTP и таких расширений файлов, как .html, .htm, .pdf, .svg, .webp). Дополнительные сведения см. на странице [https://go.microsoft.com/fwlink/?linkid=2094932](https://go.microsoft.com/fwlink/?linkid=2094932).

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Логическое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: DefaultBrowserSettingEnabled
  - Имя групповой политики: Назначить Microsoft Edge стандартным браузером
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: DefaultBrowserSettingEnabled
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000001
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: DefaultBrowserSettingEnabled
  - Пример значения:
``` xml
<true/>
```
  

  [В начало](#microsoft-edge:-политики)

  ### DeveloperToolsAvailability
  #### Определение места использования средств разработчика
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Определяет место, в котором можно использовать средства разработчика.

Если задать этом параметру политики значение "DeveloperToolsDisallowedForForceInstalledExtensions" (0, по умолчанию), пользователи смогут получать доступ к средствам разработчика и консоли JavaScript в общем, но не в контексте расширений, установленных политикой предприятия.

Если присвоить этому параметру политики значение "DeveloperToolsAllowed" (1), пользователи смогут получать доступ к средствам разработчика и консоли JavaScript во всех контекстах, включая расширения, установленные политикой предприятия.

Если присвоить этому параметру политики значение "DeveloperToolsDisallowed" (2), пользователи не смогут получать доступ к средствам разработчика или проверять элементы веб-сайтов. Сочетания клавиш и пункты меню или контекстных меню, которые открывают средства разработчика, или консоль JavaScript будут отключены.

* 0 = Блокировать средства разработчика в расширениях, установленных политикой предприятия, разрешить в других контекстах

* 1 = Разрешить использование средств разработчика

* 2 = Запретить использование средств разработчика

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Целое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: DeveloperToolsAvailability
  - Имя групповой политики: Определение места использования средств разработчика
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: DeveloperToolsAvailability
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000002
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: DeveloperToolsAvailability
  - Пример значения:
``` xml
<integer>2</integer>
```
  

  [В начало](#microsoft-edge:-политики)

  ### DirectInvokeEnabled
  #### Разрешить пользователям открывать файлы с помощью протокола DirectInvoke
  >Поддерживаемые версии: Microsoft Edge на Windows с 78 или более поздней версии

  #### Описание
  Разрешить пользователям открывать файлы с помощью протокола DirectInvoke. Протокол DirectInvoke позволяет веб-сайтам запрашивать открытие файлов в браузере с определенного URL-адреса с помощью специального обработчика файлов на компьютере или другом устройстве пользователя.

Если этот параметр политики включен или не настроен, пользователи могут открывать файлы с помощью протокола DirectInvoke.

Если данный параметр политики отключен, пользователи не могут открывать файлы с помощью протокола DirectInvoke. В этом случае файл сохраняется в файловой системе.

Примечание. Запрет DirectInvoke может привести к неправильной работе некоторых компонентов Microsoft Office SharePoint Online.

Дополнительные сведения о DirectInvoke см. на страницах [https://go.microsoft.com/fwlink/?linkid=2103872](https://go.microsoft.com/fwlink/?linkid=2103872) и [https://go.microsoft.com/fwlink/?linkid=2099871](https://go.microsoft.com/fwlink/?linkid=2099871).

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Логическое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: DirectInvokeEnabled
  - Имя групповой политики: Разрешить пользователям открывать файлы с помощью протокола DirectInvoke
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: DirectInvokeEnabled
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000000
```


  

  [В начало](#microsoft-edge:-политики)

  ### Disable3DAPIs
  #### Отключить поддержку API трехмерной графики
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Prevent web pages from accessing the graphics processing unit (GPU). Specifically, web pages can't access the WebGL API and plug-ins can't use the Pepper 3D API.

If you don't configure or disable this policy, it potentially allows web pages to use the WebGL API and plug-ins to use the Pepper 3D API. Microsoft Edge might, by default, still require command line arguments to be passed in order to use these APIs.

If [HardwareAccelerationModeEnabled](#hardwareaccelerationmodeenabled) policy is set to false, the setting for 'Disable3DAPIs' policy is ignored - it's the equivalent of setting 'Disable3DAPIs' policy to true.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Логическое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: Disable3DAPIs
  - Имя групповой политики: Отключить поддержку API трехмерной графики
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: Disable3DAPIs
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000000
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: Disable3DAPIs
  - Пример значения:
``` xml
<false/>
```
  

  [В начало](#microsoft-edge:-политики)

  ### DisableScreenshots
  #### Отключить создание снимков экрана
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Определяет, могут ли пользователи делать снимки экрана страницы браузера.

Если этот параметр включен, пользователь не может делать снимки экрана с помощью сочетания клавиш или API расширения.

Если отключить или не настроить этот параметр политики, пользователи смогут делать снимки экрана.

Обратите внимание, что этот параметр политики управляет снимками экрана, которые делаются из самого браузера. Даже если данный параметр политики включен, пользователи по-прежнему смогут делать снимки экрана с помощью любого метода вне браузера (например, с помощью функции операционной системы или другого приложения).

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Логическое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: DisableScreenshots
  - Имя групповой политики: Отключить создание снимков экрана
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: DisableScreenshots
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000001
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: DisableScreenshots
  - Пример значения:
``` xml
<true/>
```
  

  [В начало](#microsoft-edge:-политики)

  ### DiskCacheDir
  #### Задать каталог кэша на диске
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Выбор каталога для сохранения кэшированных файлов.

Если включить этот параметр политики, Microsoft Edge будет использовать заданный каталог независимо от того, указал ли пользователь флаг "--disk-cache-dir". Чтобы избежать потери данных или других непредвиденных ошибок, не задавайте в этом параметре политики корневой каталог тома или каталог, который используется для других целей, так как Microsoft Edge управляет его содержимым.

Список переменных, которые можно использовать при определении каталогов и путей, см. на странице [https://go.microsoft.com/fwlink/?linkid=2095041](https://go.microsoft.com/fwlink/?linkid=2095041).

Если не настроить этот параметр политики, будет использоваться стандартный каталог кэша и пользователь сможет переопределить это стандартное значение с помощью флага командной строки "--disk-cache-dir".

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Нет - Требуется перезапуск браузера

  #### Тип данных:
  Строковое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: DiskCacheDir
  - Имя групповой политики: Задать каталог кэша на диске
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: DiskCacheDir
  - Тип значения: REG_SZ
  ##### Пример значения:
```
"${user_home}/Edge_cache"
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: DiskCacheDir
  - Пример значения:
``` xml
<string>${user_home}/Edge_cache</string>
```
  

  [В начало](#microsoft-edge:-политики)

  ### DiskCacheSize
  #### Задать размер кэша диска (в байтах)
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Определение размера кэша (в байтах) для хранения файлов на диске.

Если этот параметр политики включен, в Microsoft Edge используется указанный размер кэша независимо от того, указал ли пользователь флаг "--disk-cache-size". Указанное в этом параметре значение является не жестким, а скорее рекомендованным ограничением для системы кэширования. Любое значение меньше нескольких мегабайт считается слишком маленьким и будет округлено до разумного минимума.

Если для данного параметра политики выбрано значение 0, используется стандартный размер кэша и пользователи не могут изменить эту настройку.

Если не настроить этот параметр политики, используется стандартный размер, но пользователи могут изменить его с помощью флага "--disk-cache-size".

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Нет - Требуется перезапуск браузера

  #### Тип данных:
  Целое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: DiskCacheSize
  - Имя групповой политики: Задать размер кэша диска (в байтах)
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: DiskCacheSize
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x06400000
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: DiskCacheSize
  - Пример значения:
``` xml
<integer>104857600</integer>
```
  

  [В начало](#microsoft-edge:-политики)

  ### DownloadDirectory
  #### Настроить каталог загрузки
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Определение каталога для загрузки файлов.

Если включить этот параметр политики, Microsoft Edge будет использовать указанный каталог независимо от того, указал пользователь такой каталог или настроил вывод запроса о расположении при каждой загрузке. Список переменных, которые можно использовать, см. на странице [https://go.microsoft.com/fwlink/?linkid=2095041](https://go.microsoft.com/fwlink/?linkid=2095041).

Если отключить или не настроить этот параметр политики, будет использоваться стандартный каталог и пользователь сможет изменить его.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Да
  - Динамическое обновление политики: Да

  #### Тип данных:
  Строковое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: DownloadDirectory
  - Имя групповой политики: Настроить каталог загрузки
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Административные шаблоны/Microsoft Edge - Параметры по умолчанию (пользователи могут переопределять)/
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): SOFTWARE\Policies\Microsoft\Edge\Рекомендовано
  - Имя значения: DownloadDirectory
  - Тип значения: REG_SZ
  ##### Пример значения:
```
"/home/${user_name}/Downloads"
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: DownloadDirectory
  - Пример значения:
``` xml
<string>/home/${user_name}/Downloads</string>
```
  

  [В начало](#microsoft-edge:-политики)

  ### DownloadRestrictions
  #### Разрешить ограничения загрузки
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Определение типа загрузок, которые Microsoft Edge полностью блокирует, без возможности для пользователей переопределять этот параметр безопасности.

Задайте значение "Блокировать опасные загрузки" (1), чтобы разрешить все загрузки, кроме тех, которые сопровождаются предупреждениями фильтра SmartScreen в Microsoft Defender.

Задайте значение "Блокировать потенциально опасные загрузки" (2), чтобы разрешить все загрузки, кроме тех, которые сопровождаются предупреждениями фильтра SmartScreen в Microsoft Defender о потенциально опасной загрузке.

Задайте значение "Блокировать все загрузки" (3), чтобы блокировать все загрузки.

Если не настроить этот параметр политики или выбрать для него значение "Нет специальных ограничений" (0), загрузки будут подпадать под обычные защитные ограничения на основе результатов анализа фильтра SmartScreen в Microsoft Defender.

Обратите внимание: эти ограничения применяются при загрузках из содержимого веб-страницы, а также пункта контекстного меню "ссылка для загрузки…". Эти ограничения не применяются при сохранении или загрузке страницы, отображаемой в данный момент, а также не применяются к пункту меню печати "Сохранить как PDF".

Дополнительные сведения о фильтре SmartScreen в Microsoft Defender см. на странице [https://go.microsoft.com/fwlink/?linkid=2094934](https://go.microsoft.com/fwlink/?linkid=2094934).

* 0 = Нет специальных ограничений

* 1 = Блокировать опасные загрузки

* 2 = Блокировать потенциально опасные загрузки

* 3 = Блокировать все загрузки

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Да
  - Динамическое обновление политики: Да

  #### Тип данных:
  Целое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: DownloadRestrictions
  - Имя групповой политики: Разрешить ограничения загрузки
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Административные шаблоны/Microsoft Edge - Параметры по умолчанию (пользователи могут переопределять)/
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): SOFTWARE\Policies\Microsoft\Edge\Рекомендовано
  - Имя значения: DownloadRestrictions
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000002
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: DownloadRestrictions
  - Пример значения:
``` xml
<integer>2</integer>
```
  

  [В начало](#microsoft-edge:-политики)

  ### EdgeCollectionsEnabled
  #### Включить функцию "Коллекции"
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 78 или более поздней версии

  #### Описание
  Настройка доступа к функции "Коллекции" для более эффективного сбора, упорядочивания, передачи и экспорта содержимого, в том числе с помощью встроенных инструментов Office.

Если включить или не настроить этот параметр политики, пользователи смогут получать доступ к функции "Коллекции" и использовать ее в Microsoft Edge.

Если данный параметр политики отключен, пользователи не могут получать доступ к функции "Коллекции" в Microsoft Edge.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Нет - Требуется перезапуск браузера

  #### Тип данных:
  Логическое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: EdgeCollectionsEnabled
  - Имя групповой политики: Включить функцию "Коллекции"
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: EdgeCollectionsEnabled
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000001
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: EdgeCollectionsEnabled
  - Пример значения:
``` xml
<true/>
```
  

  [В начало](#microsoft-edge:-политики)

  ### EditFavoritesEnabled
  #### Позволяет пользователям редактировать "Избранное"
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Включите эту политику, чтобы разрешить пользователям добавлять, удалять и изменять избранное. Это поведение по умолчанию, если параметр политики не настроен.

Отключите эту политику, чтобы запретить пользователям добавлять, удалять или изменять избранное. Они по-прежнему смогут использовать существующее избранное.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Логическое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: EditFavoritesEnabled
  - Имя групповой политики: Позволяет пользователям редактировать "Избранное"
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: EditFavoritesEnabled
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000000
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: EditFavoritesEnabled
  - Пример значения:
``` xml
<false/>
```
  

  [В начало](#microsoft-edge:-политики)

  ### EnableDeprecatedWebPlatformFeatures
  #### Повторно включить устаревшие функции веб-платформы на ограниченное время
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Укажите список устаревших функций веб-платформы, которые необходимо временно повторно включить.

Этот параметр политики позволяет пользователю повторно включить устаревшие функции веб-платформы на ограниченное время. Функции определяются тегом строки.

Если не настроить этот параметр политики, если список будет пустым или если функция не соответствует одному из поддерживаемых тегов строки, все устаревшие функции веб-платформы будут отключены.

Этот параметр политики поддерживается на вышеуказанных платформах, но функция, которую он включает, может быть недоступна на всех этих платформах. Не все устаревшие функции веб-платформы можно включить повторно. Только явно указанные ниже функции можно включить повторно и только на ограниченный период времени, который зависит от функции. Вы можете увидеть, как назначение функции веб-платформы меняется, на странице https://bit.ly/blinkintents.

Общий формат этой строки: [DeprecatedFeatureName]_EffectiveUntil[yyyymmdd].

* "ExampleDeprecatedFeature_EffectiveUntil20080902" = Enable ExampleDeprecatedFeature API through 2008/09/02

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Список строк

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: EnableDeprecatedWebPlatformFeatures
  - Имя групповой политики: Повторно включить устаревшие функции веб-платформы на ограниченное время
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge\EnableDeprecatedWebPlatformFeatures
  - Путь (Рекомендовано): Н/Д
  - Имя значения: 1, 2, 3, ...
  - Тип значения: Список REG_SZ
  ##### Пример значения:
```
SOFTWARE\Policies\Microsoft\Edge\EnableDeprecatedWebPlatformFeatures\0 = "ExampleDeprecatedFeature_EffectiveUntil20080902"

```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: EnableDeprecatedWebPlatformFeatures
  - Пример значения:
``` xml
<array>
  <string>ExampleDeprecatedFeature_EffectiveUntil20080902</string>
</array>
```
  

  [В начало](#microsoft-edge:-политики)

  ### EnableDomainActionsDownload
  #### Включить загрузку действий домена с серверов корпорации Майкрософт
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Действия домена в Microsoft Edge представляют собой ряд функций обеспечения совместимости, которые помогают браузеру правильно работать в Интернете.

Майкрософт сохраняет список действий, которые необходимо выполнить на некоторых доменах, в целях обеспечения совместимости. Например, браузер может переопределить строку "Агент пользователя" на веб-сайте, если этот веб-сайт не работает из-за новой строки "Агент пользователя" в Microsoft Edge. Каждое из этих действий применяется в течение ограниченного времени, пока Майкрософт пытается устранить проблему с владельцем сайта.

При запуске и периодически после него браузер будет подключаться к службе "Эксперименты и конфигурация", которая содержит наиболее актуальный список необходимых действий для обеспечения совместимости. Этот список сохраняется локально после первого получения, и последующие запросы только обновляют его, если серверная копия изменяется.

Если этот параметр политики включен, список действий домена и дальше будет загружаться из службы "Эксперименты и конфигурация".

Если этот параметр политики отключен, список действий домена больше не будет загружаться из службы "Эксперименты и конфигурация".

Если не настроить этот параметр политики, список действий домена и дальше будет загружаться из службы "Эксперименты и конфигурация".

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Логическое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: EnableDomainActionsDownload
  - Имя групповой политики: Включить загрузку действий домена с серверов корпорации Майкрософт
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: EnableDomainActionsDownload
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000001
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: EnableDomainActionsDownload
  - Пример значения:
``` xml
<true/>
```
  

  [В начало](#microsoft-edge:-политики)

  ### EnableOnlineRevocationChecks
  #### Включить проверки OCSP/CRL в сети
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Проверки отзыва через Интернет не обеспечивают существенного выигрыша в безопасности и по умолчанию отключены.

Если данный параметр политики включен, Microsoft Edge будет выполнять проверки OCSP/CRL через Интернет ("несерьезный сбой"). "Несерьезный сбой" означает, что если сервер отзыва сертификатов недоступен, сертификат считается действительным.

Если этот параметр политики отключен или не настроен, Microsoft Edge не будет выполнять проверки отзыва сертификатов через Интернет.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Логическое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: EnableOnlineRevocationChecks
  - Имя групповой политики: Включить проверки OCSP/CRL в сети
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: EnableOnlineRevocationChecks
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000000
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: EnableOnlineRevocationChecks
  - Пример значения:
``` xml
<false/>
```
  

  [В начало](#microsoft-edge:-политики)

  ### EnterpriseHardwarePlatformAPIEnabled
  #### Разрешить управляемым расширениям использовать API платформы оборудования предприятия
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 78 или более поздней версии

  #### Описание
  Если этот параметр политики включен, расширениям, установленным на основе корпоративной политики, разрешается использовать API платформы оборудования предприятия.
Если этот параметр политики отключен или не настроен, ни одному расширению не разрешается использовать API платформы оборудования предприятия.
Этот параметр политики также применяется для расширений компонентов.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Логическое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: EnterpriseHardwarePlatformAPIEnabled
  - Имя групповой политики: Разрешить управляемым расширениям использовать API платформы оборудования предприятия
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: EnterpriseHardwarePlatformAPIEnabled
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000001
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: EnterpriseHardwarePlatformAPIEnabled
  - Пример значения:
``` xml
<true/>
```
  

  [В начало](#microsoft-edge:-политики)

  ### ExperimentationAndConfigurationServiceControl
  #### Управление связью со службой "Эксперименты и конфигурация"
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  В Microsoft Edge для развертывания полезных данных экспериментов и конфигураций используется служба "Эксперименты и конфигурация".

Полезные данные экспериментов представляют собой список средств разработки, которые корпорация Майкрософт предоставляет для тестирования и обратной связи.

Полезные данные конфигурации представляют собой список параметров, которые Майкрософт желает реализовать в Microsoft Edge для оптимизации взаимодействия с пользователем. Например, полезные данные конфигурации могут сообщать о том, как часто Microsoft Edge отправляет запросы в службу "Эксперименты и конфигурация" для получения последних полезных данных.

Если для этого параметра политики задан режим "Получать конфигурации и эксперименты", из службы "Эксперименты и конфигурация" загружаются все полезные данные, относящиеся как к экспериментам, так и к конфигурации.

Если для этого параметра политики задан режим "Получать только конфигурации", загружаются только полезные данные конфигурации.

Если для этого параметра политики задан режим "Отключить связь со службой «Эксперименты и конфигурация»", обмен данными со службой "Эксперименты и конфигурация" полностью прекращается.

Если не настроить этот параметр политики, на управляемом устройстве в каналах Stable и Beta выполняется тот же сценарий, что и при режиме "Получать только конфигурации".

Если не настроить этот параметр политики на неуправляемом устройстве, выполняется тот же сценарий, что и при режиме "Получать конфигурации и эксперименты".

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Целое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: ExperimentationAndConfigurationServiceControl
  - Имя групповой политики: Управление связью со службой "Эксперименты и конфигурация"
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: ExperimentationAndConfigurationServiceControl
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000002
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: ExperimentationAndConfigurationServiceControl
  - Пример значения:
``` xml
<integer>2</integer>
```
  

  [В начало](#microsoft-edge:-политики)

  ### ExternalProtocolDialogShowAlwaysOpenCheckbox
  #### Show an "Always open" checkbox in external protocol dialog.
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 79 или более поздней версии

  #### Описание
  This policy controls whether the "Always open" checkbox is shown on external protocol launch confirmation prompts.

If you set this policy to True, when an external protocol confirmation prompt is shown, the user can select "Always open". The user won’t get any future confirmation prompts for this protocol.

If you set this policy to False, or the policy is unset, the "Always open" checkbox isn’t displayed. The user will be prompted for confirmation every time an external protocol is invoked.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Нет - Требуется перезапуск браузера

  #### Тип данных:
  Логическое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: ExternalProtocolDialogShowAlwaysOpenCheckbox
  - Имя групповой политики: Show an "Always open" checkbox in external protocol dialog.
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: ExternalProtocolDialogShowAlwaysOpenCheckbox
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000001
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: ExternalProtocolDialogShowAlwaysOpenCheckbox
  - Пример значения:
``` xml
<true/>
```
  

  [В начало](#microsoft-edge:-политики)

  ### FavoritesBarEnabled
  #### Включить панель "Избранное"
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Включает или выключает панель избранного.

Если данный параметр политики включен, пользователи будут видеть панель избранного.

Если этот параметр политики отключен, пользователи не смогут видеть панель избранного.

Если этот параметр политики не настроен, пользователи смогут решить, использовать панель избранного или нет.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Да
  - Динамическое обновление политики: Да

  #### Тип данных:
  Логическое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: FavoritesBarEnabled
  - Имя групповой политики: Включить панель "Избранное"
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Административные шаблоны/Microsoft Edge - Параметры по умолчанию (пользователи могут переопределять)/
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): SOFTWARE\Policies\Microsoft\Edge\Рекомендовано
  - Имя значения: FavoritesBarEnabled
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000001
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: FavoritesBarEnabled
  - Пример значения:
``` xml
<true/>
```
  

  [В начало](#microsoft-edge:-политики)

  ### ForceBingSafeSearch
  #### Принудительно применить функцию "Безопасный поиск Bing"
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Этот параметр политики обеспечивает выполнение запросов веб-поиска в Bing с помощью функции "Безопасный поиск", которой задано указанное значение. Пользователи не могут изменить этот параметр.

Если задать этому параметру политики значение "Отключено", функция "Безопасного поиска" в Bing применяет значение bing.com.

Если задать этому параметру политики значение "Умеренная", для функции "Безопасный поиск" будет использоваться умеренное значение параметра. Умеренное значение этого параметра отфильтровывает из результатов поиска видео и изображения для взрослых, но не текст.

Если задать этому параметру политики значение "Строгое", для функции "Безопасный поиск" будет использоваться строгое значение параметра. Строгое значение отфильтровывает текст, изображения и видео для взрослых.

Если отключить или не настроить этот параметр политики, функция "Безопасного поиска" в Bing не применяется принудительно, и пользователи могут задать этому параметру значение, которое они хотят, на bing.com.

* 0 = Не настраивать ограничения поиска в Bing

* 1 = Настроить умеренные ограничения поиска в Bing

* 2 = Настроить строгие ограничения поиска в Bing

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Целое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: ForceBingSafeSearch
  - Имя групповой политики: Принудительно применить функцию "Безопасный поиск Bing"
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: ForceBingSafeSearch
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000000
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: ForceBingSafeSearch
  - Пример значения:
``` xml
<integer>0</integer>
```
  

  [В начало](#microsoft-edge:-политики)

  ### ForceEphemeralProfiles
  #### Разрешить использование временных профилей
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Этот параметр политики контролирует переключение профилей пользователя во временный режим. Временный профиль создается, когда начинается сеанс, и удаляется после его завершения, при этом он привязывается к исходному профилю пользователя.

Если данный параметр политики включен, профили работают во временном режиме. Это позволяет пользователям работать на собственных устройствах, не сохраняя на этих устройствах данные о просмотре веб-страниц. Если данный параметр политики включен как политика операционной системы (например, с помощью объекта групповой политики в Windows), он применяется к каждому профилю в системе.

Если этот параметр отключен или не настроен, пользователи работают в своих обычных профилях после входа в браузер.

Во временном режиме данные профиля сохраняются на диске только на время сеанса пользователя. Такие элементы, как журнал браузера, расширения и их данные, веб-данные (например, файлы cookie и веб-базы данных), не сохраняются после закрытия браузера. Это не мешает пользователю загружать данные на диск вручную, сохранять страницы или печатать их. Если пользователь включил синхронизацию, все данные будут оставаться в его синхронизируемой учетной записи, как и в случае с обычными профилями. Пользователи могут также использовать просмотр InPrivate во временном режиме, если вы не выключили эту функцию явным образом.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Нет - Требуется перезапуск браузера

  #### Тип данных:
  Логическое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: ForceEphemeralProfiles
  - Имя групповой политики: Разрешить использование временных профилей
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: ForceEphemeralProfiles
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000001
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: ForceEphemeralProfiles
  - Пример значения:
``` xml
<true/>
```
  

  [В начало](#microsoft-edge:-политики)

  ### ForceGoogleSafeSearch
  #### Принудительно применить функцию "Безопасный поиск Google"
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Принудительно применяется активная функция "Безопасный поиск" для выполнения запросов в веб-поиске Google, и пользователям запрещается изменять этот параметр.

Если данный параметр политики включен, функция "Безопасный поиск" в поиске Google всегда активна.

Если этот параметр отключен или не настроен, функция "Безопасный поиск" в поиске Google не применяется принудительно.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Логическое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: ForceGoogleSafeSearch
  - Имя групповой политики: Принудительно применить функцию "Безопасный поиск Google"
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: ForceGoogleSafeSearch
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000000
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: ForceGoogleSafeSearch
  - Пример значения:
``` xml
<false/>
```
  

  [В начало](#microsoft-edge:-политики)

  ### ForceNetworkInProcess
  #### Принудительно выполнять сетевой код в процессе браузера
  >Поддерживаемые версии: Microsoft Edge на Windows с 78 или более поздней версии

  #### Описание
  Этот параметр политики принудительно запускает сетевой код в процессе браузера.

Этот параметр политики отключен по умолчанию. Если включить его, пользователи останутся открытыми для проблем безопасности после изолирования процесса сети.

Этот параметр политики используется, чтобы предоставить предприятиям возможность перейти на стороннее ПО, которое не зависит от привязки сетевых API. Прокси-серверы рекомендуются через LSP и исправление API Win32.

Если этот параметр политики не задан, сетевой код может выполняться вне процесса браузера в зависимости от результатов испытаний эксперимента NetworkService на практике.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Нет - Требуется перезапуск браузера

  #### Тип данных:
  Логическое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: ForceNetworkInProcess
  - Имя групповой политики: Принудительно выполнять сетевой код в процессе браузера
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: ForceNetworkInProcess
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000000
```


  

  [В начало](#microsoft-edge:-политики)

  ### ForceYouTubeRestrict
  #### Принудительное применение минимального режима ограниченного доступа на YouTube
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Принудительно применяет минимальный режим ограниченного доступа на YouTube и запрещает пользователям выбор менее ограниченного режима.

Задайте значение "Строгий" (2), чтобы принудительно применить режим строгого ограничения доступа на YouTube.

Задайте значение "Умеренный" (1), чтобы принудительно применить к пользователю режим умеренного ограничения доступа и режим строгого ограничения доступа на YouTube. Пользователи не смогут отключить ограниченный режим.

Задайте значение "Отключено" (0) или не настраивайте эту политику, чтобы не применять принудительно режим ограничения на YouTube. Внешние политики (например, политики YouTube) по-прежнему могут принудительно применять режим ограниченного доступа.

* 0 = не применять принудительно режим ограниченного доступа на YouTube

* 1 = принудительно применять по крайней мере умеренный режим ограниченного доступа на YouTube

* 2 = принудительно применять строгий режим ограниченного доступа для YouTube

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Целое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: ForceYouTubeRestrict
  - Имя групповой политики: Принудительное применение минимального режима ограниченного доступа на YouTube
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: ForceYouTubeRestrict
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000000
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: ForceYouTubeRestrict
  - Пример значения:
``` xml
<integer>0</integer>
```
  

  [В начало](#microsoft-edge:-политики)

  ### FullscreenAllowed
  #### Разрешить работу в полноэкранном режиме
  >Поддерживаемые версии: Microsoft Edge на Windows с 77 или более поздней версии

  #### Описание
  Доступ к полноэкранному режиму, при котором скрываются все пользовательские элементы интерфейса Microsoft Edge и отображается только веб-содержимое.

Если этот параметр политики включен или не настроен, пользователи, приложения и расширения с соответствующими разрешениями могут включать полноэкранный режим.

Если этот параметр политики отключен, пользователи, приложения и расширения не могут включать полноэкранный режим.

Когда доступ к полноэкранному режиму отключен, Microsoft Edge нельзя открыть в режиме киоска с помощью командной строки.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Логическое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: FullscreenAllowed
  - Имя групповой политики: Разрешить работу в полноэкранном режиме
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: FullscreenAllowed
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000001
```


  

  [В начало](#microsoft-edge:-политики)

  ### GoToIntranetSiteForSingleWordEntryInAddressBar
  #### При вводе одного слова в адресной строке не выполнять поиск, а перенаправлять пользователя на сайт интрасети.
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 78 или более поздней версии

  #### Описание
  Когда данный параметр политики включен и в адресной строке вводится одно слово без пунктуационных знаков, первый из автоматически предлагаемых вариантов в адресной строке направляет пользователя на сайты интрасети.

По умолчанию при вводе одного слова без пунктуационных знаков выполняется переход на сайт интрасети, соответствующий введенному тексту.

Когда этот параметр включен, второй из автоматически предлагаемых вариантов в адресной строке запускает поиск в Интернете в точном соответствии с введенным текстовым запросом, если этот запрос представляет собой одно слово без пунктуационных знаков. Если параллельно не включен параметр, запрещающий поиск в Интернете, используется стандартная служба поиска.

Включение данного параметра политики имеет два следующих последствия.

 В ответ на поисковый запрос в виде одного слова (который в обычной ситуации был бы сопоставлен с одним из элементов журнала) больше не будет выполняться переход к сайтам. Вместо этого браузер будет пытаться перейти к внутренним сайтам, которых может не быть в интрасети организации. В этом случае будет возникать ошибка 404.

Для правильного поиска по популярным поисковым запросам в виде одного слова необходимо будет вручную выбирать один из автоматически предлагаемых вариантов.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Логическое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: GoToIntranetSiteForSingleWordEntryInAddressBar
  - Имя групповой политики: При вводе одного слова в адресной строке не выполнять поиск, а перенаправлять пользователя на сайт интрасети.
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: GoToIntranetSiteForSingleWordEntryInAddressBar
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000000
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: GoToIntranetSiteForSingleWordEntryInAddressBar
  - Пример значения:
``` xml
<false/>
```
  

  [В начало](#microsoft-edge:-политики)

  ### HSTSPolicyBypassList
  #### Настройка списка имен, которые будут обходить проверку политики HSTS
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 79 или более поздней версии

  #### Описание
  Имена узлов, указанные в этом списке, будут исключены из проверки политики HSTS, применение которой может повышать запросы с "http://" на "https://". В этой политике допускается применение только однокомпонентных имен узлов. Имена узлов должны быть каноническими. Любые IDN должны быть преобразованы в формат A-Label, а все буквы в формате ASCII должны быть строчными. Эта политика применяется только к указанным именам узлов и не применяется к поддоменам имен в списке.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Нет - Требуется перезапуск браузера

  #### Тип данных:
  Список строк

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: HSTSPolicyBypassList
  - Имя групповой политики: Настройка списка имен, которые будут обходить проверку политики HSTS
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge\HSTSPolicyBypassList
  - Путь (Рекомендовано): Н/Д
  - Имя значения: 1, 2, 3, ...
  - Тип значения: Список REG_SZ
  ##### Пример значения:
```
SOFTWARE\Policies\Microsoft\Edge\HSTSPolicyBypassList\0 = "meet"

```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: HSTSPolicyBypassList
  - Пример значения:
``` xml
<array>
  <string>meet</string>
</array>
```
  

  [В начало](#microsoft-edge:-политики)

  ### HardwareAccelerationModeEnabled
  #### Использовать аппаратное ускорение, если доступно
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Настройте использование аппаратного ускорения, если оно доступно. Если этот параметр политики включен или не настроен, аппаратное ускорение будет включено, если функция графического процессора не заблокирована явным образом.

Если этот параметр политики отключен, аппаратное ускорение будет отключено.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Нет - Требуется перезапуск браузера

  #### Тип данных:
  Логическое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: HardwareAccelerationModeEnabled
  - Имя групповой политики: Использовать аппаратное ускорение, если доступно
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: HardwareAccelerationModeEnabled
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000001
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: HardwareAccelerationModeEnabled
  - Пример значения:
``` xml
<true/>
```
  

  [В начало](#microsoft-edge:-политики)

  ### ImportAutofillFormData
  #### Разрешить импорт данных автозаполнения формы
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Импорт данных автозаполнения форм в Microsoft Edge из другого браузера.

Если этот параметр политики включен, автоматически выбирается вариант импорта данных автозаполнения форм вручную.

Если этот параметр политики отключен, данные автозаполнения форм не импортируются при первом запуске и пользователи не могут импортировать их вручную.

Если этот параметр политики не настроен, данные автозаполнения форм импортируются при первом запуске и пользователи могут решить, необходимо ли импортировать их вручную во время следующих сеансов браузера.

Этот параметр политики можно задать как рекомендованный. Это означает, что Microsoft Edge импортирует данные автозаполнения форм при первом запуске, но пользователи могут выбрать или отменить параметр **данные автозаполнения** во время импорта вручную.

**Примечание**. Сейчас этот параметр политики управляет импортом из Google Chrome (в Windows 7, 8, 10 и в macOS).

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Да
  - Динамическое обновление политики: Да

  #### Тип данных:
  Логическое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: ImportAutofillFormData
  - Имя групповой политики: Разрешить импорт данных автозаполнения формы
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Административные шаблоны/Microsoft Edge - Параметры по умолчанию (пользователи могут переопределять)/
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): SOFTWARE\Policies\Microsoft\Edge\Рекомендовано
  - Имя значения: ImportAutofillFormData
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000001
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: ImportAutofillFormData
  - Пример значения:
``` xml
<true/>
```
  

  [В начало](#microsoft-edge:-политики)

  ### ImportBrowserSettings
  #### Разрешить импорт настроек браузера
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 78 или более поздней версии

  #### Описание
  Импорт настроек браузера в Microsoft Edge из другого браузера.

Если этот параметр политики включен, в диалоговом окне **Импорт данных браузера** автоматически устанавливается флажок **Настройки браузера**.

Если этот параметр политики отключен, настройки браузера не импортируются при первом запуске и пользователи не могут импортировать их вручную.

Если не настроить этот параметр политики, настройки браузера импортируются при первом запуске и пользователи могут решить, необходимо ли импортировать их вручную во время следующих сеансов браузера.

Этот параметр политики можно задать как рекомендованный. Это означает, что Microsoft Edge импортирует настройки при первом запуске, но пользователи могут выбрать или отменить параметр **настройки браузера** во время импорта вручную.

**Примечание**. Сейчас этот параметр политики управляет импортом из Google Chrome (в Windows 7, 8, 10 и в macOS).

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Да
  - Динамическое обновление политики: Да

  #### Тип данных:
  Логическое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: ImportBrowserSettings
  - Имя групповой политики: Разрешить импорт настроек браузера
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Административные шаблоны/Microsoft Edge - Параметры по умолчанию (пользователи могут переопределять)/
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): SOFTWARE\Policies\Microsoft\Edge\Рекомендовано
  - Имя значения: ImportBrowserSettings
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000001
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: ImportBrowserSettings
  - Пример значения:
``` xml
<true/>
```
  

  [В начало](#microsoft-edge:-политики)

  ### ImportFavorites
  #### Разрешить импорт избранного
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Импорт избранного в Microsoft Edge из другого браузера.

Если этот параметр политики включен, в диалоговом окне **Импорт данных браузера** автоматически устанавливается флажок **Избранное**.

Если этот параметр политики отключен, избранное не импортируется при первом запуске и пользователи не могут импортировать его вручную.

Если этот параметр политики не настроен, избранное импортируется при первом запуске и пользователи могут решить, необходимо ли импортировать его вручную во время следующих сеансов браузера.

Этот параметр политики можно задать как рекомендованный. Это означает, что Microsoft Edge импортирует избранное при первом запуске, но пользователи могут выбрать или отменить параметр **избранное** во время импорта вручную.

**Примечание**. Сейчас этот параметр политики управляет импортом из браузеров Internet Explorer (в Windows 7, 8 и 10), Google Chrome (в Windows 7, 8, 10 и в macOS) и Apple Safari (в macOS).

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Да
  - Динамическое обновление политики: Да

  #### Тип данных:
  Логическое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: ImportFavorites
  - Имя групповой политики: Разрешить импорт избранного
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Административные шаблоны/Microsoft Edge - Параметры по умолчанию (пользователи могут переопределять)/
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): SOFTWARE\Policies\Microsoft\Edge\Рекомендовано
  - Имя значения: ImportFavorites
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000001
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: ImportFavorites
  - Пример значения:
``` xml
<true/>
```
  

  [В начало](#microsoft-edge:-политики)

  ### ImportHistory
  #### Разрешить импорт журнала браузера
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Импорт журнала браузера в Microsoft Edge из другого браузера.

Если этот параметр политики включен, в диалоговом окне **Импорт данных браузера** автоматически устанавливается флажок **Журнал браузера**.

Если этот параметр политики отключен, данные журнала браузера не импортируются при первом запуске и пользователи не могут импортировать их вручную.

Если этот параметр политики не настроен, данные журнала браузера импортируются при первом запуске и пользователи могут решить, необходимо ли импортировать их вручную во время следующих сеансов браузера.

Этот параметр политики можно задать как рекомендованный. Это означает, что Microsoft Edge импортирует журнал браузера при первом запуске, но пользователи могут выбрать или отменить параметр **журнал** во время импорта вручную.

**Примечание**. Сейчас этот параметр политики управляет импортом из браузеров Internet Explorer (в Windows 7, 8 и 10), Google Chrome (в Windows 7, 8, 10 и в macOS) и Apple Safari (macOS).

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Да
  - Динамическое обновление политики: Да

  #### Тип данных:
  Логическое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: ImportHistory
  - Имя групповой политики: Разрешить импорт журнала браузера
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Административные шаблоны/Microsoft Edge - Параметры по умолчанию (пользователи могут переопределять)/
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): SOFTWARE\Policies\Microsoft\Edge\Рекомендовано
  - Имя значения: ImportHistory
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000001
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: ImportHistory
  - Пример значения:
``` xml
<true/>
```
  

  [В начало](#microsoft-edge:-политики)

  ### ImportHomepage
  #### Разрешить импорт параметров домашней страницы
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Импорт домашней страницы в Microsoft Edge из другого браузера.

Если этот параметр политики включен, автоматически разрешается импорт домашней страницы вручную.

Если этот параметр политики отключен, домашняя страница не импортируется при первом запуске и пользователи не могут импортировать ее вручную.

Если этот параметр политики не настроен, домашняя страница импортируется при первом запуске и пользователи могут решить, необходимо ли импортировать ее вручную во время следующих сеансов браузера.

Этот параметр политики можно задать как рекомендованный. Это означает, что Microsoft Edge импортирует домашнюю страницу при первом запуске, но пользователи могут выбрать или отменить параметр **домашняя страница** во время импорта вручную.

**Примечание**. Сейчас этот параметр политики управляет импортом из браузера Internet Explorer (в Windows 7, 8 и 10).

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Логическое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: ImportHomepage
  - Имя групповой политики: Разрешить импорт параметров домашней страницы
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: ImportHomepage
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000001
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: ImportHomepage
  - Пример значения:
``` xml
<true/>
```
  

  [В начало](#microsoft-edge:-политики)

  ### ImportOpenTabs
  #### Разрешение импорта открытых вкладок
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 79 или более поздней версии

  #### Описание
  Пользователям разрешается импортировать в Microsoft Edge открытые и закрепленные вкладки из другого браузера.

Если включить эту политику, в диалоговом окне **Импорт данных браузера** автоматически устанавливается флажок **Открытые вкладки**.

Если отключить эту политику, открытые вкладки не импортируются при первом запуске и пользователи не могут импортировать их вручную.

Если не настроить эту политику, открытые вкладки импортируются при первом запуске и во время следующих сеансов просмотра веб-страниц пользователи могут решить, нужно ли импортировать вкладки вручную.

Эту политику также можно задать как рекомендацию. В таком случае браузер Microsoft Edge импортирует открытые вкладки при первом запуске, но во время ручного импорта пользователи могут установить или снять флажок **Открытые вкладки**.

**Примечание**. Сейчас эта политика поддерживает только импорт из Google Chrome (в Windows 7, 8, 10 и macOS).

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Да
  - Динамическое обновление политики: Да

  #### Тип данных:
  Логическое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: ImportOpenTabs
  - Имя групповой политики: Разрешение импорта открытых вкладок
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Административные шаблоны/Microsoft Edge - Параметры по умолчанию (пользователи могут переопределять)/
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): SOFTWARE\Policies\Microsoft\Edge\Рекомендовано
  - Имя значения: ImportOpenTabs
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000001
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: ImportOpenTabs
  - Пример значения:
``` xml
<true/>
```
  

  [В начало](#microsoft-edge:-политики)

  ### ImportPaymentInfo
  #### Разрешить импорт платежных данных
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Импорт платежной информации в Microsoft Edge из другого браузера.

Если этот параметр политики включен, в диалоговом окне **Импорт данных браузера** автоматически устанавливается флажок **платежная информация**.

Если этот параметр политики отключен, платежная информация не импортируется при первом запуске и пользователи не могут импортировать ее вручную.

Если не настроить этот параметр политики, платежная информация импортируется при первом запуске и пользователи могут решить, необходимо ли импортировать ее вручную во время следующих сеансов браузера.

Этот параметр политики можно задать как рекомендованный. Это означает, что Microsoft Edge импортирует платежную информацию при первом запуске, но пользователи могут выбрать или отменить параметр **платежная информация** во время импорта вручную.

**Примечание**. Сейчас этот параметр политики управляет импортом из Google Chrome (в Windows 7, 8, 10 и в macOS).

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Да
  - Динамическое обновление политики: Да

  #### Тип данных:
  Логическое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: ImportPaymentInfo
  - Имя групповой политики: Разрешить импорт платежных данных
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Административные шаблоны/Microsoft Edge - Параметры по умолчанию (пользователи могут переопределять)/
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): SOFTWARE\Policies\Microsoft\Edge\Рекомендовано
  - Имя значения: ImportPaymentInfo
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000001
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: ImportPaymentInfo
  - Пример значения:
``` xml
<true/>
```
  

  [В начало](#microsoft-edge:-политики)

  ### ImportSavedPasswords
  #### Разрешить импорт сохраненных паролей
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Импорт сохраненных паролей в Microsoft Edge из другого браузера.

Если этот параметр политики включен, автоматически разрешается импорт сохраненных паролей вручную.

Если этот параметр политики отключен, сохраненные пароли не импортируются при первом запуске и пользователи не могут импортировать их вручную.

Если этот параметр политики не настроен, пароли импортируются при первом запуске и пользователи могут решить, необходимо ли импортировать их вручную во время следующих сеансов браузера.

Этот параметр политики можно задать как рекомендованный. Это означает, что Microsoft Edge импортирует пароли при первом запуске, но пользователи могут выбрать или отменить параметр **пароли** во время импорта вручную.

**Примечание**. Сейчас этот параметр политики управляет импортом из браузеров Internet Explorer (в Windows 7, 8 и 10) и Google Chrome (в Windows 7, 8, 10 и в macOS).

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Да
  - Динамическое обновление политики: Да

  #### Тип данных:
  Логическое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: ImportSavedPasswords
  - Имя групповой политики: Разрешить импорт сохраненных паролей
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Административные шаблоны/Microsoft Edge - Параметры по умолчанию (пользователи могут переопределять)/
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): SOFTWARE\Policies\Microsoft\Edge\Рекомендовано
  - Имя значения: ImportSavedPasswords
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000001
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: ImportSavedPasswords
  - Пример значения:
``` xml
<true/>
```
  

  [В начало](#microsoft-edge:-политики)

  ### ImportSearchEngine
  #### Разрешить импортировать параметры поисковой системы
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Импорт параметров поисковой системы в Microsoft Edge из другого браузера.

Если этот параметр политики включен, автоматически разрешается импорт параметров поисковой системы.

Если этот параметр политики отключен, параметры поисковой системы не импортируются при первом запуске и пользователи не могут импортировать их вручную.

Если этот параметр политики не настроен, параметры поисковой системы импортируются при первом запуске и пользователи могут решить, необходимо ли импортировать их вручную во время следующих сеансов браузера.

Этот параметр политики можно задать как рекомендованный. Это означает, что Microsoft Edge импортирует параметры поисковой системы при первом запуске, но пользователи могут выбрать или отменить параметр **поисковая система** во время импорта вручную.

**Примечание**. Сейчас этот параметр политики управляет импортом из Internet Explorer (в Windows 7, 8 и 10).

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Да
  - Динамическое обновление политики: Да

  #### Тип данных:
  Логическое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: ImportSearchEngine
  - Имя групповой политики: Разрешить импортировать параметры поисковой системы
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Административные шаблоны/Microsoft Edge - Параметры по умолчанию (пользователи могут переопределять)/
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): SOFTWARE\Policies\Microsoft\Edge\Рекомендовано
  - Имя значения: ImportSearchEngine
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000001
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: ImportSearchEngine
  - Пример значения:
``` xml
<true/>
```
  

  [В начало](#microsoft-edge:-политики)

  ### InPrivateModeAvailability
  #### Настроить доступность режима InPrivate
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Доступ к страницам в режиме InPrivate в Microsoft Edge.

Если не настроить этот параметр политики или присвоить ему значение "Включено" (0), пользователи смогут открывать страницы в режиме InPrivate.

Если присвоить параметру значение "Отключено" (1), пользователи не смогут использовать режим InPrivate.

Если присвоить параметру значение "Принудительно" (2), режим InPrivate будет использоваться всегда.

* 0 = Режим InPrivate доступен

* 1 = Режим InPrivate отключен

* 2 = Режим InPrivate используется принудительно

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Целое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: InPrivateModeAvailability
  - Имя групповой политики: Настроить доступность режима InPrivate
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: InPrivateModeAvailability
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000001
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: InPrivateModeAvailability
  - Пример значения:
``` xml
<integer>1</integer>
```
  

  [В начало](#microsoft-edge:-политики)

  ### InternetExplorerIntegrationLevel
  #### Настройка интеграции с Internet Explorer
  >Поддерживаемые версии: Microsoft Edge на Windows с 77 или более поздней версии

  #### Описание
  Инструкции по настройке оптимального интерфейса режима Internet Explorer см. на странице [https://go.microsoft.com/fwlink/?linkid=2094210](https://go.microsoft.com/fwlink/?linkid=2094210)

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Нет - Требуется перезапуск браузера

  #### Тип данных:
  Целое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: InternetExplorerIntegrationLevel
  - Имя групповой политики: Настройка интеграции с Internet Explorer
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: InternetExplorerIntegrationLevel
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000001
```


  

  [В начало](#microsoft-edge:-политики)

  ### InternetExplorerIntegrationSiteList
  #### Настроить список сайтов для режима предприятия
  >Поддерживаемые версии: Microsoft Edge на Windows с 78 или более поздней версии

  #### Описание
  Инструкции по настройке оптимального интерфейса режима Internet Explorer см. на странице [https://go.microsoft.com/fwlink/?linkid=2094210](https://go.microsoft.com/fwlink/?linkid=2094210)

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Нет - Требуется перезапуск браузера

  #### Тип данных:
  Строковое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: InternetExplorerIntegrationSiteList
  - Имя групповой политики: Настроить список сайтов для режима предприятия
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: InternetExplorerIntegrationSiteList
  - Тип значения: REG_SZ
  ##### Пример значения:
```
"https://internal.contoso.com/sitelist.xml"
```


  

  [В начало](#microsoft-edge:-политики)

  ### InternetExplorerIntegrationSiteRedirect
  #### Укажите способ обработки переходов "на странице" для ненастроенных сайтов, выполненных со страниц в режиме Internet Explorer
  >Поддерживаемые версии: Microsoft Edge на Windows с 79 или более поздней версии

  #### Описание
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

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Нет - Требуется перезапуск браузера

  #### Тип данных:
  Целое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: InternetExplorerIntegrationSiteRedirect
  - Имя групповой политики: Укажите способ обработки переходов "на странице" для ненастроенных сайтов, выполненных со страниц в режиме Internet Explorer
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: InternetExplorerIntegrationSiteRedirect
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000000
```


  

  [В начало](#microsoft-edge:-политики)

  ### IsolateOrigins
  #### Включить изоляцию сайта для определенных источников
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Specify origins to run in isolation, in their own process.
This policy also isolates origins named by subdomains - for example, specifying https://contoso.com/ will cause https://foo.contoso.com/ to be isolated as part of the https://contoso.com/ site.
If the policy is enabled, each of the named origins in a comma-separated list will run in its own process.
If you disable this policy, then both the 'IsolateOrigins' and 'SitePerProcess' features are disabled. Users can still enable 'IsolateOrigins' policy manually, via command line flags.
If you don't configure the policy, the user can change this setting.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Нет - Требуется перезапуск браузера

  #### Тип данных:
  Строковое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: IsolateOrigins
  - Имя групповой политики: Включить изоляцию сайта для определенных источников
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: IsolateOrigins
  - Тип значения: REG_SZ
  ##### Пример значения:
```
"https://contoso.com/,https://fabrikam.com/"
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: IsolateOrigins
  - Пример значения:
``` xml
<string>https://contoso.com/,https://fabrikam.com/</string>
```
  

  [В начало](#microsoft-edge:-политики)

  ### ManagedFavorites
  #### Настроить "Избранное"
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Настройка списка управляемых элементов избранного.

Этот параметр политики определяет список элементов избранного. Каждый такой элемент содержит разделы "name" и "url", в которых указаны его название и целевой адрес. Можно настроить вложенную папку, определив элементы избранного без раздела "url", но с дополнительным разделом "children", который будет содержать список элементов избранного, как описано выше (некоторые элементы могут представлять собой папки). Microsoft Edge завершает неполные URL-адреса так, как если бы они были введены через адресную строку, например "microsoft.com" станет "https://microsoft.com/".

Эти элементы избранного размещаются в папке, которую не может изменить пользователь (но пользователь может скрыть ее на панели избранного). По умолчанию эта папка называется "Управляемое избранное", но вы можете изменить это название, добавив в список элементов избранного словарь, содержащий раздел "toplevel_name", и указав необходимое имя папки в качестве значения.

Управляемое избранное не синхронизируется с учетной записью пользователя и не может быть изменено расширениями.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Словарь

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: ManagedFavorites
  - Имя групповой политики: Настроить "Избранное"
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: ManagedFavorites
  - Тип значения: REG_SZ
  ##### Пример значения:
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


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: ManagedFavorites
  - Пример значения:
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
  

  [В начало](#microsoft-edge:-политики)

  ### ManagedSearchEngines
  #### Управление поисковыми системами
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Lets you configure a list of list of up to 10 search engines, one of which must be marked as the default search engine.
You do not need to specify the encoding for any search engine.

If you enable this policy, users can't add, remove, or change any search engine in the list. Users can set their default search engine to any search engine in the list.

If you disable or don't configure this policy, users can modify the search engines list as desired.

If the [DefaultSearchProviderSearchURL](#defaultsearchprovidersearchurl) policy is set, this policy (ManagedSearchEngines) is ignored. The user must restart their browser to finish applying this policy.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Нет - Требуется перезапуск браузера

  #### Тип данных:
  Словарь

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: ManagedSearchEngines
  - Имя групповой политики: Управление поисковыми системами
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: ManagedSearchEngines
  - Тип значения: REG_SZ
  ##### Пример значения:
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


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: ManagedSearchEngines
  - Пример значения:
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
  

  [В начало](#microsoft-edge:-политики)

  ### MaxConnectionsPerProxy
  #### Максимальное число одновременных подключений к прокси-серверу
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Задает максимальное число одновременных подключений к прокси-серверу.

Некоторые прокси-серверы не могут обрабатывать большое количество одновременных подключений для каждого клиента. Это можно решить, задав данному параметру политики меньшее значение.

Значение этого параметра политики должно быть меньше 100 и больше 6. Значение по умолчанию — 32 подключения.

Известно, что некоторые веб-приложения используют большое число подключений с зависшими запросами GET. Уменьшение максимального числа подключений ниже 32 может привести к зависанию сети браузера, если открыто слишком много веб-приложений этого вида.

Если этот параметр политики не настроен, используется значение по умолчанию (32).

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Нет - Требуется перезапуск браузера

  #### Тип данных:
  Целое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: MaxConnectionsPerProxy
  - Имя групповой политики: Максимальное число одновременных подключений к прокси-серверу
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: MaxConnectionsPerProxy
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000020
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: MaxConnectionsPerProxy
  - Пример значения:
``` xml
<integer>32</integer>
```
  

  [В начало](#microsoft-edge:-политики)

  ### MediaRouterCastAllowAllIPs
  #### Разрешить Google Cast подключаться к устройствам передачи с любыми IP-адресами
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Enable this policy to let Google Cast connect to Cast devices on all IP addresses, not just RFC1918/RFC4193 private addresses.

Disable this policy to restrict Google Cast to Cast devices on RFC1918/RFC4193 private addresses.

If you don't configure this policy, Google Cast connects to Cast devices on RFC1918/RFC4193 private addresses only, unless you enable the CastAllowAllIPs feature.

If the [EnableMediaRouter](#enablemediarouter) policy is disabled, then this policy has no effect.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Логическое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: MediaRouterCastAllowAllIPs
  - Имя групповой политики: Разрешить Google Cast подключаться к устройствам передачи с любыми IP-адресами
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: MediaRouterCastAllowAllIPs
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000000
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: MediaRouterCastAllowAllIPs
  - Пример значения:
``` xml
<false/>
```
  

  [В начало](#microsoft-edge:-политики)

  ### MetricsReportingEnabled
  #### Включить отправку отчетов об использовании и данных, относящихся к сбою
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  В случае каналов Microsoft Edge Beta и Stable в Windows 10 этот параметр политики, если он настроен, переопределяет параметр диагностических данных Windows, а именно: разрешает или запрещает сбор информации об использовании и сбоях Microsoft Edge ([https://go.microsoft.com/fwlink/?linkid=2099569](https://go.microsoft.com/fwlink/?linkid=2099569)).

С помощью этого параметра можно настроить отправку в корпорацию Майкрософт сведений об использовании и сбоях Microsoft Edge и запретить пользователи изменять данную настройку.

Когда этот параметр включен, сведения об использовании и сбоях отправляются в корпорацию Майкрософт. Когда выключен — не отправляются. В обоих случаях пользователи не могут изменить или переопределить эту настройку.

Для каналов Beta и Stable в Windows 10 этот параметр определяет правила работы со сведениями об использовании и сбоях. Если он не настроен, к Microsoft Edge по умолчанию применяется параметр диагностических данных Windows.

Для каналов Canary и Dev в Windows 10 этот параметр определяет правила работы со сведениями об использовании и сбоях. Если он не настроен, к Microsoft Edge по умолчанию применяются настройки пользователя.

В Windows 7, 8 и в Mac этот параметр политики определяет правила работы со сведениями об использовании и сбоях. Если он не настроен, к Microsoft Edge по умолчанию применяются настройки пользователя.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Нет - Требуется перезапуск браузера

  #### Тип данных:
  Логическое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: MetricsReportingEnabled
  - Имя групповой политики: Включить отправку отчетов об использовании и данных, относящихся к сбою
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: MetricsReportingEnabled
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000001
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: MetricsReportingEnabled
  - Пример значения:
``` xml
<true/>
```
  

  [В начало](#microsoft-edge:-политики)

  ### NetworkPredictionOptions
  #### Включить прогнозирование сети
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Включает прогнозирование сети и запрещает пользователям изменять этот параметр.

Это позволяет контролировать предварительную загрузку DNS, предварительное TCP- и SSL-соединение, а также предварительную обработку веб-страниц.

Если этот параметр политики не настроен, прогнозирование сети включено, но пользователь может изменить это значение.

* 0 = Прогнозировать действия сети для любого сетевого подключения

* 2 = Не прогнозировать действия сети ни для какого сетевого подключения

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Да
  - Динамическое обновление политики: Да

  #### Тип данных:
  Целое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: NetworkPredictionOptions
  - Имя групповой политики: Включить прогнозирование сети
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Административные шаблоны/Microsoft Edge - Параметры по умолчанию (пользователи могут переопределять)/
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): SOFTWARE\Policies\Microsoft\Edge\Рекомендовано
  - Имя значения: NetworkPredictionOptions
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000001
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: NetworkPredictionOptions
  - Пример значения:
``` xml
<integer>1</integer>
```
  

  [В начало](#microsoft-edge:-политики)

  ### NonRemovableProfileEnabled
  #### Настройка постоянного автоматического входа пользователя в стандартный профиль на основе рабочей или учебной учетной записи
  >Поддерживаемые версии: Microsoft Edge на Windows с 78 или более поздней версии

  #### Описание
  This policy determines if the Microsoft Edge profile automatically signed in with a user's work or school account is removable.

If you enable or don't configure this policy, a non-removable profile will be created with the user's work or school account on Windows. This profile can't be signed out or removed.

When you disable this policy, the profile automatically signed in with a user's work or school account from Windows can be signed out or removed by the user.

If you want to completely disable browser sign in, use the 'BrowserSignIn' policy.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Логическое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: NonRemovableProfileEnabled
  - Имя групповой политики: Настройка постоянного автоматического входа пользователя в стандартный профиль на основе рабочей или учебной учетной записи
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: NonRemovableProfileEnabled
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000001
```


  

  [В начало](#microsoft-edge:-политики)

  ### OverrideSecurityRestrictionsOnInsecureOrigin
  #### Управление применением ограничений доступа к небезопасным источникам
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Этот параметр политики позволяет указать список источников (URL-адреса) или шаблонов имен узлов (например, "*.contoso.com"), к которым не применяются ограничения, связанные с небезопасными источниками.

Вы можете указать разрешенные источники устаревших приложений, которые не позволяют развернуть TLS или настроить сервер промежуточного хранения для внутренней веб-разработки, чтобы разработчики могли тестировать функции, требующие безопасного контекста, не разворачивая TLS на сервере промежуточного хранения. Этот параметр политики также запрещает отображать для источников отметку "Небезопасно" в адресной строке omnibox.

Список URL-адресов в этом параметре политики имеет тот же эффект, что и список тех же URL-адресов через запятую, указанный для флага командной строки "--unsafely-treat-insecure-origin-as-secure". Если этот параметр политики включен, он переопределяет флаг командной строки.

Подробные сведения о безопасных контекстах см. здесь: https://www.w3.org/TR/secure-contexts/.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Нет - Требуется перезапуск браузера

  #### Тип данных:
  Список строк

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: OverrideSecurityRestrictionsOnInsecureOrigin
  - Имя групповой политики: Управление применением ограничений доступа к небезопасным источникам
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge\OverrideSecurityRestrictionsOnInsecureOrigin
  - Путь (Рекомендовано): Н/Д
  - Имя значения: 1, 2, 3, ...
  - Тип значения: Список REG_SZ
  ##### Пример значения:
```
SOFTWARE\Policies\Microsoft\Edge\OverrideSecurityRestrictionsOnInsecureOrigin\0 = "http://testserver.contoso.com/"
SOFTWARE\Policies\Microsoft\Edge\OverrideSecurityRestrictionsOnInsecureOrigin\1 = "*.contoso.com"

```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: OverrideSecurityRestrictionsOnInsecureOrigin
  - Пример значения:
``` xml
<array>
  <string>http://testserver.contoso.com/</string>
  <string>*.contoso.com</string>
</array>
```
  

  [В начало](#microsoft-edge:-политики)

  ### ProactiveAuthEnabled
  #### Включить упреждающую проверку подлинности
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Включение или отключение упреждающей проверки подлинности.

Если этот параметр политики включен, Microsoft Edge с помощью служб Майкрософт выполняет упреждающую проверку подлинности пользователей, которые входят в систему. При этом Microsoft Edge периодически связывается с веб-службой, чтобы получить обновленный манифест, содержащий настройки для такой проверки подлинности.

Если этот параметр политики отключен, Microsoft Edge не пытается с помощью служб Майкрософт выполнять упреждающую проверку подлинности пользователей, которые входят в систему. Также Microsoft Edge не связывается с веб-службой, чтобы получить обновленный манифест, содержащий настройки для такой проверки подлинности.

Если не настроить этот параметр политики, упреждающая проверка подлинности будет включена.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Нет - Требуется перезапуск браузера

  #### Тип данных:
  Логическое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: ProactiveAuthEnabled
  - Имя групповой политики: Включить упреждающую проверку подлинности
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: ProactiveAuthEnabled
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000001
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: ProactiveAuthEnabled
  - Пример значения:
``` xml
<true/>
```
  

  [В начало](#microsoft-edge:-политики)

  ### PromotionalTabsEnabled
  #### Включить отображение полноширинной вкладки с рекламным содержимым
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Настройка представления рекламного или учебного содержимого на всей вкладке. Этот параметр позволяет настроить вид страниц приветствия, на которых пользователи могут входить в Microsoft Edge, выбирать стандартный браузер или получать информацию о возможностях продукта.

Если данный параметр политики включен (присвоено значение true) или не настроен, Microsoft Edge может отображать содержимое на всей вкладке, чтобы сообщить сведения о продукте.

Если этот параметр отключен (присвоено значение false), Microsoft Edge не может отображать содержимое на всей вкладке.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Логическое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: PromotionalTabsEnabled
  - Имя групповой политики: Включить отображение полноширинной вкладки с рекламным содержимым
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: PromotionalTabsEnabled
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000000
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: PromotionalTabsEnabled
  - Пример значения:
``` xml
<false/>
```
  

  [В начало](#microsoft-edge:-политики)

  ### PromptForDownloadLocation
  #### Спрашивать, куда сохранять загруженные файлы
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Этот параметр политики позволяет указать, необходимо ли спрашивать пользователя о месте сохранения файла перед загрузкой.

Если этот параметр политики включен, перед каждой загрузкой система просит пользователя указать, где сохранить файл. Если этот параметр политики не настроен, файлы автоматически сохраняются в папку, используемую по умолчанию, без запроса к пользователю.

Если этот параметр политики не настроен, пользователь может изменить данную настройку.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Логическое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: PromptForDownloadLocation
  - Имя групповой политики: Спрашивать, куда сохранять загруженные файлы
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: PromptForDownloadLocation
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000000
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: PromptForDownloadLocation
  - Пример значения:
``` xml
<false/>
```
  

  [В начало](#microsoft-edge:-политики)

  ### QuicAllowed
  #### Разрешить протокол QUIC
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Использование протокола QUIC в Microsoft Edge.

Если этот параметр политики включен или не настроен, протокол QUIC разрешен.

Если этот параметр политики отключен, протокол QUIC блокируется.

QUIC — это сетевой протокол транспортного уровня, который может повысить производительность веб-приложений, использующих подключение по протоколу TCP.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Нет - Требуется перезапуск браузера

  #### Тип данных:
  Логическое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: QuicAllowed
  - Имя групповой политики: Разрешить протокол QUIC
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: QuicAllowed
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000001
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: QuicAllowed
  - Пример значения:
``` xml
<true/>
```
  

  [В начало](#microsoft-edge:-политики)

  ### RelaunchNotification
  #### Уведомлять пользователя о том, что рекомендуется или требуется перезапустить браузер для ожидающих обновлений
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Notify users that they need to restart Microsoft Edge to apply a pending update.

If you don't configure this policy, Microsoft Edge adds a recycle icon at the far right of the top menu bar to prompt users to restart the browser to apply the update.

If you enable this policy and set it to 'Recommended' (1), a recurring warning prompts users that a restart is recommended. Users can dismiss this warning and defer the restart.

If you set the policy to 'Required' (2), a recurring warning prompts users that the browser will be restarted automatically as soon as a notification period passes. The default period is seven days. You can configure this period with the [RelaunchNotificationPeriod](#relaunchnotificationperiod) policy.

The user's session is restored when the browser restarts.

* Recommended (1) = Show a recurring prompt to the user indicating that a restart is recommended

* Required (2) = Show a recurring prompt to the user indicating that a restart is required

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Целое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: RelaunchNotification
  - Имя групповой политики: Уведомлять пользователя о том, что рекомендуется или требуется перезапустить браузер для ожидающих обновлений
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: RelaunchNotification
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000001
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: RelaunchNotification
  - Пример значения:
``` xml
<integer>1</integer>
```
  

  [В начало](#microsoft-edge:-политики)

  ### RelaunchNotificationPeriod
  #### Задать период времени для уведомлений об обновлении
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Sets the time period, in milliseconds, over which users are notified that Microsoft Edge must be restarted to apply a pending update.

During this time period, the user is repeatedly informed that they need to restart. The app menu changes to indicate that a restart is needed when one third of the notification period passes. When two thirds of the notification period passes, the notification changes color, and again when the full notification period has passed. Additional notifications enabled by the [RelaunchNotification](#relaunchnotification) policy follow this same schedule.

If you don't configure this policy, the default period is 604800000 milliseconds (one week).

Restrictions:

* Minimum:3600000

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Целое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: RelaunchNotificationPeriod
  - Имя групповой политики: Задать период времени для уведомлений об обновлении
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: RelaunchNotificationPeriod
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x240c8400
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: RelaunchNotificationPeriod
  - Пример значения:
``` xml
<integer>604800000</integer>
```
  

  [В начало](#microsoft-edge:-политики)

  ### RendererCodeIntegrityEnabled
  #### Включить целостность кода визуализации
  >Поддерживаемые версии: Microsoft Edge на Windows с 78 или более поздней версии

  #### Описание
  Если этот параметр политики включен или не задан, целостность кода визуализации включена. Эту политику следует отключать только в случае обнаружения проблем совместимости с программным обеспечением сторонних производителей, которое должно выполняться в процессах визуализации Microsoft Edge.

Отключение этой политики может негативно повлиять на безопасность и стабильность Microsoft Edge в связи с тем, что неизвестному и потенциально злонамеренному коду будет разрешено загружаться в процессы визуализации Microsoft Edge.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Нет - Требуется перезапуск браузера

  #### Тип данных:
  Логическое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: RendererCodeIntegrityEnabled
  - Имя групповой политики: Включить целостность кода визуализации
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: RendererCodeIntegrityEnabled
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000000
```


  

  [В начало](#microsoft-edge:-политики)

  ### RequireOnlineRevocationChecksForLocalAnchors
  #### Укажите, требуются ли проверки OCSP и списка отзыва сертификатов через Интернет для локальных якорей доверия
  >Поддерживаемые версии: Microsoft Edge на Windows с 77 или более поздней версии

  #### Описание
  Настройка обязательных проверок отзыва сертификатов через Интернет (проверки списка отзыва сертификатов или OCSP). Если Microsoft Edge не может получить информацию о состоянии отзыва, соответствующие сертификаты считаются отозванными ("серьезный сбой").

Если этот параметр политики включен, Microsoft Edge всегда выполняет проверку отзыва для сертификатов сервера, которые были успешно проверены и подписаны сертификатами локально установленных ЦС.

Если не настроить или отключить этот параметр, Microsoft Edge будет использовать существующие параметры проверки отзыва сертификатов через Интернет.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Логическое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: RequireOnlineRevocationChecksForLocalAnchors
  - Имя групповой политики: Укажите, требуются ли проверки OCSP и списка отзыва сертификатов через Интернет для локальных якорей доверия
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: RequireOnlineRevocationChecksForLocalAnchors
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000000
```


  

  [В начало](#microsoft-edge:-политики)

  ### ResolveNavigationErrorsUseWebService
  #### Включить устранение ошибок навигации с помощью веб-службы
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Allow Microsoft Edge to issue a dataless connection to a web service to probe networks for connectivity in cases like hotel and airport Wi-Fi.

If you enable this policy, a web service is used for network connectivity tests.

If you disable this policy, Microsoft Edge uses native APIs to try to resolve network connectivity and navigation issues.

**Note**: Except on Windows 8 and later versions of Windows, Microsoft Edge *always* uses native APIs to resolve connectivity issues.

If you don't configure this policy, Microsoft Edge respects the user preference that's set under Services at edge://settings/privacy.
Specifically, there's a **Use a web service to help resolve navigation errors** toggle, which the user can switch on or off. Be aware that if you have enabled this policy (ResolveNavigationErrorsUseWebService), the **Use a web service to help resolve navigation errors** setting is turned on, but the user can't change the setting by using the toggle. If you have disabled this policy, the **Use a web service to help resolve navigation errors** setting is turned off, and the user can't change the setting by using the toggle.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Да
  - Динамическое обновление политики: Да

  #### Тип данных:
  Логическое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: ResolveNavigationErrorsUseWebService
  - Имя групповой политики: Включить устранение ошибок навигации с помощью веб-службы
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Административные шаблоны/Microsoft Edge - Параметры по умолчанию (пользователи могут переопределять)/
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): SOFTWARE\Policies\Microsoft\Edge\Рекомендовано
  - Имя значения: ResolveNavigationErrorsUseWebService
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000001
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: ResolveNavigationErrorsUseWebService
  - Пример значения:
``` xml
<true/>
```
  

  [В начало](#microsoft-edge:-политики)

  ### RestrictSigninToPattern
  #### Ограничить учетные записи, которые могут использоваться в качестве основных в Microsoft Edge
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Определение учетных записей, которые можно установить как основные в Microsoft Edge (учетные записи, которые выбираются при включении синхронизации).

При попытке задать основную учетную запись браузера с именем пользователя, которое не соответствует данному шаблону, система блокирует это действие и отображает соответствующее сообщение об ошибке.

Если не настроить этот параметр политики или оставить его пустым, пользователи смогут назначить любую учетную запись основной в браузере Microsoft Edge.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Строковое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: RestrictSigninToPattern
  - Имя групповой политики: Ограничить учетные записи, которые могут использоваться в качестве основных в Microsoft Edge
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: RestrictSigninToPattern
  - Тип значения: REG_SZ
  ##### Пример значения:
```
".*@contoso.com"
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: RestrictSigninToPattern
  - Пример значения:
``` xml
<string>.*@contoso.com</string>
```
  

  [В начало](#microsoft-edge:-политики)

  ### RunAllFlashInAllowMode
  #### Расширить параметр содержимого Adobe Flash на все содержимое
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  If you enable this policy, all Adobe Flash content embedded in websites that are set to allow Adobe Flash in the content settings -- either by the user or by enterprise policy -- will run. This includes content from other origins and/or small content.

To control which websites are allowed to run Adobe Flash, see the specifications in the [DefaultPluginsSetting](#defaultpluginssetting), [PluginsAllowedForUrls](#pluginsallowedforurls), and [PluginsBlockedForUrls](#pluginsblockedforurls) policies.

If you disable this policy or don't configure it, Adobe Flash content from other origins (from sites that aren't specified in the three policies mentioned immediately above) or small content might be blocked.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Логическое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: RunAllFlashInAllowMode
  - Имя групповой политики: Расширить параметр содержимого Adobe Flash на все содержимое
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: RunAllFlashInAllowMode
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000001
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: RunAllFlashInAllowMode
  - Пример значения:
``` xml
<true/>
```
  

  [В начало](#microsoft-edge:-политики)

  ### SSLErrorOverrideAllowed
  #### Разрешить пользователям продолжать работу со страницы предупреждения HTTPS
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Microsoft Edge отображает страницу предупреждения, когда пользователь переходит на сайты, содержащие ошибки SSL.

Если включить или не настроить (по умолчанию) этот параметр политики, пользователи смогут пропускать такие страницы предупреждений.

Если отключить этот параметр политики, пользователям будет запрещено пропускать страницы предупреждений.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Логическое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: SSLErrorOverrideAllowed
  - Имя групповой политики: Разрешить пользователям продолжать работу со страницы предупреждения HTTPS
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: SSLErrorOverrideAllowed
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000001
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: SSLErrorOverrideAllowed
  - Пример значения:
``` xml
<true/>
```
  

  [В начало](#microsoft-edge:-политики)

  ### SSLVersionMin
  #### Включена минимальная версия протокола TLS
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Определение минимальной поддерживаемой версии SSL. Если этот параметр не настроен, в Microsoft Edge используется минимальная версия по умолчанию — TLS 1.0.

Если этот параметр включен, можно выбрать один из следующих вариантов минимальной версии: "tls1", "tls1.1" или "tls1.2". Если этот параметр настроен, Microsoft Edge не использует версии SSL/TLS ниже заданной. Все нераспознанные значения игнорируются.

* "tls1" = TLS 1.0

* "tls1.1" = TLS 1.1

* "tls1.2" = TLS 1.2

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Строковое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: SSLVersionMin
  - Имя групповой политики: Включена минимальная версия протокола TLS
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: SSLVersionMin
  - Тип значения: REG_SZ
  ##### Пример значения:
```
"tls1"
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: SSLVersionMin
  - Пример значения:
``` xml
<string>tls1</string>
```
  

  [В начало](#microsoft-edge:-политики)

  ### SavingBrowserHistoryDisabled
  #### Отключить сохранение журнала браузера
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Отключает сохранение журнала браузера и запрещает пользователям изменять этот параметр.

Если этот параметр политики включен, журнал браузера не будет сохраняться. Это действие также отключает синхронизацию вкладок.

Если этот параметр отключен или не настроен, журнал браузера сохраняется.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Логическое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: SavingBrowserHistoryDisabled
  - Имя групповой политики: Отключить сохранение журнала браузера
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: SavingBrowserHistoryDisabled
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000001
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: SavingBrowserHistoryDisabled
  - Пример значения:
``` xml
<true/>
```
  

  [В начало](#microsoft-edge:-политики)

  ### SearchSuggestEnabled
  #### Включить варианты поиска
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Использование вариантов запросов для веб-поиска в адресной строке и списке автозаполнения Microsoft Edge без возможности для пользователей изменять этот параметр.

Если данный параметр политики включен, предлагаются варианты запросов для веб-поиска.

Если этот параметр политики отключен, варианты запросов для веб-поиска никогда не предлагаются, однако варианты из локального журнала и избранного будут отображаться. Если этот параметр политики отключен, ни введенные символы, ни посещенные URL-адреса не будут включены в телеметрию, отправляемую в корпорацию Майкрософт.

Если этот параметр политики не задан, варианты поисковых запросов будут предлагаться, но пользователь сможет изменить эту настройку.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Да
  - Динамическое обновление политики: Да

  #### Тип данных:
  Логическое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: SearchSuggestEnabled
  - Имя групповой политики: Включить варианты поиска
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Административные шаблоны/Microsoft Edge - Параметры по умолчанию (пользователи могут переопределять)/
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): SOFTWARE\Policies\Microsoft\Edge\Рекомендовано
  - Имя значения: SearchSuggestEnabled
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000001
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: SearchSuggestEnabled
  - Пример значения:
``` xml
<true/>
```
  

  [В начало](#microsoft-edge:-политики)

  ### SecurityKeyPermitAttestation
  #### Веб-сайты и домены, которые не требуют разрешения на использование прямой аттестации ключа безопасности
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Определяет веб-сайты и домены, которые не требуют явного разрешения пользователя, когда запрашиваются сертификаты аттестации от ключей безопасности. Кроме того, ключу безопасности отправляется сигнал, указывающий, что он может использовать индивидуальную аттестацию. Без этого пользователи каждый раз получают запрос на аттестацию ключей безопасности.

Сайты (например, https://contoso.com/some/path) сопоставляются только как идентификаторы appID U2F. Домены (например, contoso.com) сопоставляются только как идентификаторы webauthn RP. Чтобы охватить API U2F и webauthn для данного сайта, необходимо указать URL-адрес и домен appID.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Список строк

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: SecurityKeyPermitAttestation
  - Имя групповой политики: Веб-сайты и домены, которые не требуют разрешения на использование прямой аттестации ключа безопасности
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge\SecurityKeyPermitAttestation
  - Путь (Рекомендовано): Н/Д
  - Имя значения: 1, 2, 3, ...
  - Тип значения: Список REG_SZ
  ##### Пример значения:
```
SOFTWARE\Policies\Microsoft\Edge\SecurityKeyPermitAttestation\0 = "https://contoso.com"

```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: SecurityKeyPermitAttestation
  - Пример значения:
``` xml
<array>
  <string>https://contoso.com</string>
</array>
```
  

  [В начало](#microsoft-edge:-политики)

  ### SendIntranetToInternetExplorer
  #### Отправка всех сайтов интрасети в Internet Explorer
  >Поддерживаемые версии: Microsoft Edge на Windows с 77 или более поздней версии

  #### Описание
  Инструкции по настройке оптимального интерфейса режима Internet Explorer см. на странице [https://go.microsoft.com/fwlink/?linkid=2094210](https://go.microsoft.com/fwlink/?linkid=2094210)

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Нет - Требуется перезапуск браузера

  #### Тип данных:
  Логическое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: SendIntranetToInternetExplorer
  - Имя групповой политики: Отправка всех сайтов интрасети в Internet Explorer
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: SendIntranetToInternetExplorer
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000001
```


  

  [В начало](#microsoft-edge:-политики)

  ### SendSiteInfoToImproveServices
  #### Отправлять сведения о сайте для улучшения служб Майкрософт
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  В случае каналов Microsoft Edge Beta и Stable в Windows 10 этот параметр политики, если он настроен, переопределяет параметр диагностических данных Windows, а именно: разрешает или запрещает сбор информации о просмотре веб-сайтов в Microsoft Edge ([https://go.microsoft.com/fwlink/?linkid=2099569](https://go.microsoft.com/fwlink/?linkid=2099569)).

С помощью этого параметра можно разрешить или запретить пользователям отправлять сведения о веб-сайтах, которые они посещают в Microsoft Edge, корпорации Майкрософт для улучшения таких служб, как служба поиска.

Если этот параметр политики включен, сведения о веб-сайтах, посещаемых в Microsoft Edge, отправляются в корпорацию Майкрософт.

Если этот параметр политики отключен, сведения о веб-сайтах, посещаемых в Microsoft Edge, не отправляются в корпорацию Майкрософт.

Для каналов Beta и Stable в Windows 10 этот параметр определяет правила отправки сведений о посещаемых веб-сайтах. Если он не настроен, к Microsoft Edge по умолчанию применяется параметр диагностических данных Windows.

Для каналов Canary и Dev в Windows 10 этот параметр определяет правила отправки сведений о посещаемых веб-сайтах. Если он не настроен, к Microsoft Edge по умолчанию применяются настройки пользователя.

В Windows 7, 8 и в Mac этот параметр политики определяет правила отправки сведений о посещаемых веб-сайтах. Если он не настроен, к Microsoft Edge по умолчанию применяются настройки пользователя.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Нет - Требуется перезапуск браузера

  #### Тип данных:
  Логическое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: SendSiteInfoToImproveServices
  - Имя групповой политики: Отправлять сведения о сайте для улучшения служб Майкрософт
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: SendSiteInfoToImproveServices
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000000
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: SendSiteInfoToImproveServices
  - Пример значения:
``` xml
<false/>
```
  

  [В начало](#microsoft-edge:-политики)

  ### ShowOfficeShortcutInFavoritesBar
  #### Показать ярлык Microsoft Office на панели "Избранное"
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Отображение ярлыка для Office.com на панели "Избранное". Пользователи, выполнившие вход в Microsoft Edge, могут через этот ярлык переходить к документам и приложениям Microsoft Office.

Если этот параметр политики включен или не настроен, пользователи могут отобразить или скрыть этот ярлык, изменив положение переключателя в контекстном меню панели избранного.

Если этот параметр политики отключен, ярлык не отображается.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Логическое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: ShowOfficeShortcutInFavoritesBar
  - Имя групповой политики: Показать ярлык Microsoft Office на панели "Избранное"
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: ShowOfficeShortcutInFavoritesBar
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000000
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: ShowOfficeShortcutInFavoritesBar
  - Пример значения:
``` xml
<false/>
```
  

  [В начало](#microsoft-edge:-политики)

  ### SignedHTTPExchangeEnabled
  #### Включить поддержку подписи HTTP exchange (SXG)
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 78 или более поздней версии

  #### Описание
  Поддержка подписанных пакетов обмена по HTTP (SXG).

Если этот параметр политики не задан или включен, Microsoft Edge принимает веб-содержимое, представленное в виде подписанных пакетов обмена по HTTP.

Если этот параметр политики отключен, подписанные пакеты обмена по HTTP не загружаются.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Логическое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: SignedHTTPExchangeEnabled
  - Имя групповой политики: Включить поддержку подписи HTTP exchange (SXG)
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: SignedHTTPExchangeEnabled
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000001
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: SignedHTTPExchangeEnabled
  - Пример значения:
``` xml
<true/>
```
  

  [В начало](#microsoft-edge:-политики)

  ### SitePerProcess
  #### Включить изоляцию для каждого сайта
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  
The 'SitePerProcess' policy can be used to prevent users from opting out of the default behavior of isolating all sites. Note that you can also use the [IsolateOrigins](#isolateorigins) policy to isolate additional, finer-grained origins.
If you enable this policy, users can't opt out of the default behavior where each site runs in its own process.
If you disable or don’t configure this policy, a user can opt out of site isolation.  (For example, by using "Disable site isolation" entry in edge://flags.)  Disabling the policy or not configuring the policy doesn't turn off Site Isolation.


  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Нет - Требуется перезапуск браузера

  #### Тип данных:
  Логическое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: SitePerProcess
  - Имя групповой политики: Включить изоляцию для каждого сайта
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: SitePerProcess
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000001
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: SitePerProcess
  - Пример значения:
``` xml
<true/>
```
  

  [В начало](#microsoft-edge:-политики)

  ### SpellcheckEnabled
  #### Включить проверку орфографии
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  If you enable or don't configure this policy, the user can use spellcheck.

If you disable this policy, the user can't use spellcheck and the [SpellcheckLanguage](#spellchecklanguage) and [SpellcheckLanguageBlocklist](#spellchecklanguageblocklist) policies are also disabled.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Логическое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: SpellcheckEnabled
  - Имя групповой политики: Включить проверку орфографии
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: SpellcheckEnabled
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000000
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: SpellcheckEnabled
  - Пример значения:
``` xml
<false/>
```
  

  [В начало](#microsoft-edge:-политики)

  ### SpellcheckLanguage
  #### Включить конкретные языки проверки орфографии
  >Поддерживаемые версии: Microsoft Edge на Windows с 77 или более поздней версии

  #### Описание
  Enables different languages for spellcheck. Any language that you specify that isn't recognized is ignored.

If you enable this policy, spellcheck is enabled for the languages specified, as well as any languages the user has enabled.

If you don't configure or disable this policy, there's no change to the user's spellcheck preferences.

If the [SpellcheckEnabled](#spellcheckenabled) policy is disabled, this policy will have no effect.

If a language is included in both the 'SpellcheckLanguage' and the [SpellcheckLanguageBlocklist](#spellchecklanguageblocklist) policy, the spellcheck language is enabled.

The supported languages are: af, bg, ca, cs, cy, da, de, el, en-AU, en-CA, en-GB, en-US, es, es-419, es-AR, es-ES, es-MX, es-US, et, fa, fo, fr, he, hi, hr, hu, id, it, ko, lt, lv, nb, nl, pl, pt-BR, pt-PT, ro, ru, sh, sk, sl, sq, sr, sv, ta, tg, tr, uk, vi.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Список строк

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: SpellcheckLanguage
  - Имя групповой политики: Включить конкретные языки проверки орфографии
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge\SpellcheckLanguage
  - Путь (Рекомендовано): Н/Д
  - Имя значения: 1, 2, 3, ...
  - Тип значения: Список REG_SZ
  ##### Пример значения:
```
SOFTWARE\Policies\Microsoft\Edge\SpellcheckLanguage\0 = "fr"
SOFTWARE\Policies\Microsoft\Edge\SpellcheckLanguage\1 = "es"

```


  

  [В начало](#microsoft-edge:-политики)

  ### SpellcheckLanguageBlocklist
  #### Принудительное отключение языков проверки орфографии
  >Поддерживаемые версии: Microsoft Edge на Windows с 78 или более поздней версии

  #### Описание
  Force-disables spellcheck languages. Unrecognized languages in that list will be ignored.

If you enable this policy, spellcheck will be disabled for the languages specified. The user can still enable or disable spellcheck for languages not in the list.

If you do not set this policy, or disable it, there will be no change to the user's spellcheck preferences.

If the [SpellcheckEnabled](#spellcheckenabled) policy is set to disabled, this policy will have no effect.

If a language is included in both the [SpellcheckLanguage](#spellchecklanguage) and the 'SpellcheckLanguageBlocklist' policy, the spellcheck language is enabled.

The currently supported languages are: af, bg, ca, cs, da, de, el, en-AU, en-CA, en-GB, en-US, es, es-419, es-AR, es-ES, es-MX, es-US, et, fa, fo, fr, he, hi, hr, hu, id, it, ko, lt, lv, nb, nl, pl, pt-BR, pt-PT, ro, ru, sh, sk, sl, sq, sr, sv, ta, tg, tr, uk, vi.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Список строк

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: SpellcheckLanguageBlocklist
  - Имя групповой политики: Принудительное отключение языков проверки орфографии
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge\SpellcheckLanguageBlocklist
  - Путь (Рекомендовано): Н/Д
  - Имя значения: 1, 2, 3, ...
  - Тип значения: Список REG_SZ
  ##### Пример значения:
```
SOFTWARE\Policies\Microsoft\Edge\SpellcheckLanguageBlocklist\0 = "fr"
SOFTWARE\Policies\Microsoft\Edge\SpellcheckLanguageBlocklist\1 = "es"

```


  

  [В начало](#microsoft-edge:-политики)

  ### SuppressUnsupportedOSWarning
  #### Отключить предупреждение о неподдерживаемой ОС
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Подавление предупреждения, которое появляется при использовании Microsoft Edge на компьютере или в операционной системе, которые больше не поддерживаются.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Нет - Требуется перезапуск браузера

  #### Тип данных:
  Логическое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: SuppressUnsupportedOSWarning
  - Имя групповой политики: Отключить предупреждение о неподдерживаемой ОС
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: SuppressUnsupportedOSWarning
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000001
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: SuppressUnsupportedOSWarning
  - Пример значения:
``` xml
<true/>
```
  

  [В начало](#microsoft-edge:-политики)

  ### SyncDisabled
  #### Отключить синхронизацию данных с помощью служб синхронизации Майкрософт
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Disables data synchronization in Microsoft Edge and prevents users from modifying this setting.

If this policy is not set, users will be able to either turn on or turn off sync.

Do not enable this policy when the policy 'RoamingProfileSupportEnabled' is enabled, as 'RoamingProfileSupportEnabled' duplicates the sync functionality.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Да
  - Динамическое обновление политики: Да

  #### Тип данных:
  Логическое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: SyncDisabled
  - Имя групповой политики: Отключить синхронизацию данных с помощью служб синхронизации Майкрософт
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Административные шаблоны/Microsoft Edge - Параметры по умолчанию (пользователи могут переопределять)/
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): SOFTWARE\Policies\Microsoft\Edge\Рекомендовано
  - Имя значения: SyncDisabled
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000001
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: SyncDisabled
  - Пример значения:
``` xml
<true/>
```
  

  [В начало](#microsoft-edge:-политики)

  ### TabFreezingEnabled
  #### Allow freezing of background tabs
  >Поддерживаемые версии: Microsoft Edge на Windows с 79 или более поздней версии

  #### Описание
  Controls whether Microsoft Edge can freeze tabs that are in the background for at least 5 minutes.

Tab freezing reduces CPU, battery, and memory usage. Microsoft Edge uses heuristics to avoid freezing tabs that do useful work in the background, such as display notifications, play sound, and stream video.

If you enable or don't configure this policy, tabs that have been in the background for at least 5 minutes might be frozen.

If you disable this policy, no tabs will be frozen.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Нет - Требуется перезапуск браузера

  #### Тип данных:
  Логическое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: TabFreezingEnabled
  - Имя групповой политики: Allow freezing of background tabs
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: TabFreezingEnabled
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000000
```


  

  [В начало](#microsoft-edge:-политики)

  ### TaskManagerEndProcessEnabled
  #### Включить завершение процессов в диспетчере задач браузера
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Если включить или не настроить этот параметр политики, пользователи смогут завершать процессы в диспетчере задач браузера. Если отключить его, пользователи не смогут завершать процессы, и кнопка "Завершить процесс" будет отключена в диспетчере задач браузера.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Логическое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: TaskManagerEndProcessEnabled
  - Имя групповой политики: Включить завершение процессов в диспетчере задач браузера
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: TaskManagerEndProcessEnabled
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000001
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: TaskManagerEndProcessEnabled
  - Пример значения:
``` xml
<true/>
```
  

  [В начало](#microsoft-edge:-политики)

  ### TrackingPrevention
  #### Блокировка отслеживания просмотренных веб-страниц
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 78 или более поздней версии

  #### Описание
  Настройка блокировки отслеживания просмотренных веб-страниц.

Когда этот параметр политики включен, вы можете выбрать один из указанных далее уровней блокировки отслеживания.

0 = Выключено (отслеживание не блокируется)
1 = Базовый уровень (блокируются вредоносные средства отслеживания, при этом содержимое и рекламные объявления персонализируются)
2 = Сбалансированный уровень (блокируются вредоносные средства отслеживания, а также средства отслеживания на сайтах, которые пользователь не посещал, при этом содержимое и рекламные объявления персонализируются в меньшей мере)
3 = Строгий уровень (блокируются вредоносные средства отслеживания, а также большинство остальных средств отслеживания на всех сайтах; при этом содержимое и рекламные объявления персонализируются в минимальной степени, а некоторые компоненты сайтов могут не работать)

Когда этот параметр политики выключен или не настроен, пользователи могут самостоятельно выбирать уровень блокировки отслеживания.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Целое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: TrackingPrevention
  - Имя групповой политики: Блокировка отслеживания просмотренных веб-страниц
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: TrackingPrevention
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000002
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: TrackingPrevention
  - Пример значения:
``` xml
<integer>2</integer>
```
  

  [В начало](#microsoft-edge:-политики)

  ### TranslateEnabled
  #### Включить перевод
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Включение встроенной службы перевода (Майкрософт) в Microsoft Edge.

Если данный параметр политики включен, Microsoft Edge предлагает пользователю функции перевода в собственном всплывающем меню (если доступно) и в контекстном меню правой кнопки мыши.

Если данный параметр политики отключен, все встроенные функции перевода выключены.

Если этот параметр политики не настроен, пользователи могут сами решить, использовать функции перевода или нет.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Да
  - Динамическое обновление политики: Да

  #### Тип данных:
  Логическое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: TranslateEnabled
  - Имя групповой политики: Включить перевод
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Административные шаблоны/Microsoft Edge - Параметры по умолчанию (пользователи могут переопределять)/
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): SOFTWARE\Policies\Microsoft\Edge\Рекомендовано
  - Имя значения: TranslateEnabled
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000001
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: TranslateEnabled
  - Пример значения:
``` xml
<true/>
```
  

  [В начало](#microsoft-edge:-политики)

  ### URLAllowlist
  #### Определить список разрешенных URL-адресов
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Allow access to the listed URLs, as exceptions to the URL block list.

Format the URL pattern according to [https://go.microsoft.com/fwlink/?linkid=2095322](https://go.microsoft.com/fwlink/?linkid=2095322).

You can use this policy to open exceptions to restrictive block lists. For example, you can include '*' in the block list to block all requests, and then use this policy to allow access to a limited list of URLs. You can use this policy to open exceptions to certain schemes, subdomains of other domains, ports, or specific paths.

The most specific filter determines if a URL is blocked or allowed. The allowed list takes precedence over the block list.

This policy is limited to 1000 entries; subsequent entries are ignored.

If you don't configure this policy, there are no exceptions to the block list in the [URLBlocklist](#urlblocklist) policy.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Список строк

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: URLAllowlist
  - Имя групповой политики: Определить список разрешенных URL-адресов
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge\URLAllowlist
  - Путь (Рекомендовано): Н/Д
  - Имя значения: 1, 2, 3, ...
  - Тип значения: Список REG_SZ
  ##### Пример значения:
```
SOFTWARE\Policies\Microsoft\Edge\URLAllowlist\0 = "contoso.com"
SOFTWARE\Policies\Microsoft\Edge\URLAllowlist\1 = "https://ssl.server.com"
SOFTWARE\Policies\Microsoft\Edge\URLAllowlist\2 = "hosting.com/good_path"
SOFTWARE\Policies\Microsoft\Edge\URLAllowlist\3 = "https://server:8080/path"
SOFTWARE\Policies\Microsoft\Edge\URLAllowlist\4 = ".exact.hostname.com"

```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: URLAllowlist
  - Пример значения:
``` xml
<array>
  <string>contoso.com</string>
  <string>https://ssl.server.com</string>
  <string>hosting.com/good_path</string>
  <string>https://server:8080/path</string>
  <string>.exact.hostname.com</string>
</array>
```
  

  [В начало](#microsoft-edge:-политики)

  ### URLBlocklist
  #### Запретить доступ к списку URL-адресов
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Define a list of sites, based on URL patterns, that are blocked (your users can't load them).

Format the URL pattern according to [https://go.microsoft.com/fwlink/?linkid=2095322](https://go.microsoft.com/fwlink/?linkid=2095322).

You can define exceptions in the [URLAllowlist](#urlallowlist) policy. These policies are limited to 1000 entries; subsequent entries are ignored.

Note that blocking internal 'edge://*' URLs isn't recommended - this may lead to unexpected errors.

This policy doesn't prevent the page from updating dynamically through JavaScript. For example, if you block 'contoso.com/abc', users might still be able to visit 'contoso.com' and click on a link to visit 'contoso.com/abc', as long as the page doesn't refresh.

If you don't configure this policy, no URLs are blocked.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Список строк

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: URLBlocklist
  - Имя групповой политики: Запретить доступ к списку URL-адресов
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge\URLBlocklist
  - Путь (Рекомендовано): Н/Д
  - Имя значения: 1, 2, 3, ...
  - Тип значения: Список REG_SZ
  ##### Пример значения:
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


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: URLBlocklist
  - Пример значения:
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
  

  [В начало](#microsoft-edge:-политики)

  ### UserDataDir
  #### Задать каталог данных пользователя
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Определение каталога для сохранения пользовательских данных.

Если включить этот параметр политики, Microsoft Edge будет использовать заданный каталог независимо от того, указал ли пользователь флаг командной строки "--user-data-dir".

Если не включить этот параметр политики, будет использоваться путь к профилю по умолчанию и пользователь сможет переопределить его с помощью флага "--user-data-dir". Каталог для профиля можно найти на странице edge://version/ в разделе пути к профилю.

Чтобы избежать потери данных или других ошибок, не настраивайте этот параметр политики для корневого каталога тома или для каталога, который используется для других целей, так как Microsoft Edge управляет его содержимым.

Список переменных, которые можно использовать, см. на странице [https://go.microsoft.com/fwlink/?linkid=2095041](https://go.microsoft.com/fwlink/?linkid=2095041).

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Нет - Требуется перезапуск браузера

  #### Тип данных:
  Строковое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: UserDataDir
  - Имя групповой политики: Задать каталог данных пользователя
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: UserDataDir
  - Тип значения: REG_SZ
  ##### Пример значения:
```
"${users}/${user_name}/Edge"
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: UserDataDir
  - Пример значения:
``` xml
<string>${users}/${user_name}/Edge</string>
```
  

  [В начало](#microsoft-edge:-политики)

  ### UserFeedbackAllowed
  #### Разрешить отзывы пользователей
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  В Microsoft Edge доступна функция отправки отзывов об Edge (по умолчанию включена), с помощью которой пользователи могут отправлять отзывы, предложения или заполненные опросы клиентов и сообщать обо всех проблемах с браузером. По умолчанию пользователи не могут отключить функцию отзывов об Edge.

Если этот параметр включен или не настроен, пользователи могут вызвать функцию отзывов об Edge.

Если этот параметр политики отключен, пользователи не могут вызвать функцию отзывов об Edge.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Нет - Требуется перезапуск браузера

  #### Тип данных:
  Логическое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: UserFeedbackAllowed
  - Имя групповой политики: Разрешить отзывы пользователей
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: UserFeedbackAllowed
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000001
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: UserFeedbackAllowed
  - Пример значения:
``` xml
<true/>
```
  

  [В начало](#microsoft-edge:-политики)

  ### VideoCaptureAllowed
  #### Разрешить или запретить запись видео
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Control whether sites can capture video.

If enabled or not configured (default), the user will be asked about video capture access for all sites except those with URLs configured in the [VideoCaptureAllowedUrls](#videocaptureallowedurls) policy list, which will be granted access without prompting.

If you disable this policy, the user isn't prompted, and video capture is only available to URLs configured in [VideoCaptureAllowedUrls](#videocaptureallowedurls) policy.

This policy affects all types of video inputs, not only the built-in camera.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Логическое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: VideoCaptureAllowed
  - Имя групповой политики: Разрешить или запретить запись видео
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: VideoCaptureAllowed
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000000
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: VideoCaptureAllowed
  - Пример значения:
``` xml
<false/>
```
  

  [В начало](#microsoft-edge:-политики)

  ### VideoCaptureAllowedUrls
  #### Сайты, которые могут получать доступ к устройствам записи видео без запроса разрешения
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  На основании шаблонов URL-адресов укажите веб-сайты, которые могут использовать устройства записи видео, без запроса разрешения пользователя. Шаблоны в этом списке сопоставляются с источником безопасности запрашивающего URL-адреса. Если они совпадают, сайту автоматически предоставляется доступ к устройствам записи видео.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Да

  #### Тип данных:
  Список строк

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: VideoCaptureAllowedUrls
  - Имя групповой политики: Сайты, которые могут получать доступ к устройствам записи видео без запроса разрешения
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge\VideoCaptureAllowedUrls
  - Путь (Рекомендовано): Н/Д
  - Имя значения: 1, 2, 3, ...
  - Тип значения: Список REG_SZ
  ##### Пример значения:
```
SOFTWARE\Policies\Microsoft\Edge\VideoCaptureAllowedUrls\0 = "https://www.contoso.com/"
SOFTWARE\Policies\Microsoft\Edge\VideoCaptureAllowedUrls\1 = "https://[*.]contoso.edu/"

```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: VideoCaptureAllowedUrls
  - Пример значения:
``` xml
<array>
  <string>https://www.contoso.com/</string>
  <string>https://[*.]contoso.edu/</string>
</array>
```
  

  [В начало](#microsoft-edge:-политики)

  ### WPADQuickCheckEnabled
  #### Настроить оптимизацию WPAD
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Оптимизация WPAD (Web Proxy Auto-Discovery) в Microsoft Edge.

Если отключить этот параметр политики, оптимизация WPAD будет отключена, из-за чего браузеру придется дольше ожидать отклика DNS-серверов WPAD.

Если включить или не настроить этот параметр политики, оптимизация WPAD будет включена.

Независимо от того, включен ли этот параметр и каким образом, пользователи не могут изменять параметр оптимизации WPAD.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Нет - Требуется перезапуск браузера

  #### Тип данных:
  Логическое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: WPADQuickCheckEnabled
  - Имя групповой политики: Настроить оптимизацию WPAD
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: WPADQuickCheckEnabled
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000001
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: WPADQuickCheckEnabled
  - Пример значения:
``` xml
<true/>
```
  

  [В начало](#microsoft-edge:-политики)

  ### WebDriverOverridesIncompatiblePolicies
  #### Разрешить WebDriver переопределять несовместимые политики
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  
This policy was removed in M80, because it is not necessary anymore as
WebDriver is now compatible with all existing policies.

This policy allows users of the WebDriver feature to override
policies which can interfere with its operation.

Currently this policy disables [SitePerProcess](#siteperprocess) and [IsolateOrigins](#isolateorigins) policies.

If the policy is enabled, WebDriver will be able to override incomaptible
policies.
If the policy is disabled or not configured, WebDriver will not be allowed
to override incompatible policies.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Нет - Требуется перезапуск браузера

  #### Тип данных:
  Логическое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: WebDriverOverridesIncompatiblePolicies
  - Имя групповой политики: Разрешить WebDriver переопределять несовместимые политики
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: WebDriverOverridesIncompatiblePolicies
  - Тип значения: REG_DWORD
  ##### Пример значения:
```
0x00000001
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: WebDriverOverridesIncompatiblePolicies
  - Пример значения:
``` xml
<true/>
```
  

  [В начало](#microsoft-edge:-политики)

  ### WebRtcLocalhostIpHandling
  #### Ограничить раскрытие IP-адреса localhost с помощью WebRTC
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Позволяет определить, предоставляет ли WebRTC IP-адрес localhost пользователя.

Если для этого параметра политики задано значение "AllowAllInterfaces" ('default') или "AllowPublicAndPrivateInterfaces" ('default_public_and_private_interfaces'), WebRTC предоставляет IP-адрес localhost.

Если для этого параметра политики задано значение "AllowPublicInterfaceOnly" ('default_public_interface_only') или "DisableNonProxiedUdp" ('disable_non_proxied_udp'), WebRTC не предоставляет IP-адрес localhost.

Если не настроить этот параметр политики или отключить его, WebRTC предоставляет IP-адрес localhost.

  * 'default' = Разрешить все интерфейсы. Это значение предоставляет IP-адрес localhost.
  * 'default_public_and_private_interfaces' = Разрешить общие и частные интерфейсы по маршруту HTTP по умолчанию. Это значение предоставляет IP-адрес localhost.
  * 'default_public_interface_only' = Разрешить общий интерфейс по маршруту HTTP по умолчанию. Это значение не предоставляет IP-адрес localhost.
  * 'disable_non_proxied_udp' = Использовать TCP, если прокси-сервер не поддерживает UDP. Это значение не предоставляет IP-адрес localhost.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Нет - Требуется перезапуск браузера

  #### Тип данных:
  Строковое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: WebRtcLocalhostIpHandling
  - Имя групповой политики: Ограничить раскрытие IP-адреса localhost с помощью WebRTC
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: WebRtcLocalhostIpHandling
  - Тип значения: REG_SZ
  ##### Пример значения:
```
"default"
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: WebRtcLocalhostIpHandling
  - Пример значения:
``` xml
<string>default</string>
```
  

  [В начало](#microsoft-edge:-политики)

  ### WebRtcUdpPortRange
  #### Ограничить диапазон локальных UDP-портов, используемых WebRTC
  >Поддерживаемые версии: Microsoft Edge на Windows и Mac с 77 или более поздней версии

  #### Описание
  Эта политика ограничивает диапазон UDP-портов, используемый WebRTC, до заданного интервала портов (включая конечные точки).

Настраивая эту политику вы указываете диапазон локальных UDP-портов, которые может использовать WebRTC.

Если вы не настроите эту политику, а также если укажете для нее пустую строку или недопустимый диапазон портов, WebRTC сможет использовать любой доступный локальный порт UDP.

  #### Поддерживаемые функции:
  - Может быть обязательной: Да
  - Может быть рекомендованной: Нет
  - Динамическое обновление политики: Нет - Требуется перезапуск браузера

  #### Тип данных:
  Строковое

  #### Параметры и сведения Windows
  ##### Сведения о групповой политике (ADMX)
  - Уникальное имя групповой политики: WebRtcUdpPortRange
  - Имя групповой политики: Ограничить диапазон локальных UDP-портов, используемых WebRTC
  - Путь групповой политики (Обязательно): Административные шаблоны/Microsoft Edge/
  - Путь групповой политики (Рекомендовано): Н/Д
  - Имя файла групповой политики ADMX: MSEdge.admx
  ##### Параметры реестра Windows
  - Путь (Обязательно): SOFTWARE\Policies\Microsoft\Edge
  - Путь (Рекомендовано): Н/Д
  - Имя значения: WebRtcUdpPortRange
  - Тип значения: REG_SZ
  ##### Пример значения:
```
"10000-11999"
```


  #### Сведения и параметры Mac
  - Имя предпочтительного ключа: WebRtcUdpPortRange
  - Пример значения:
``` xml
<string>10000-11999</string>
```
  

  [В начало](#microsoft-edge:-политики)


## См. также
- [Настройка Microsoft Edge](configure-microsoft-edge.md)
- [Целевая страница предприятия в Microsoft Edge](https://aka.ms/EdgeEnterprise)