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

# Microsoft Edge: directivas
La versión más reciente de Microsoft Edge incluye las siguientes directivas. Puede usar estas directivas para configurar la forma en que Microsoft Edge se ejecuta en su organización.

Para obtener información sobre un conjunto adicional de directivas usadas para controlar cómo y cuándo se actualiza Microsoft Edge, consulte [Referencia de la directiva de Microsoft Edge Update](microsoft-edge-update-policies.md)

> [!NOTA]
> Este artículo se aplica a Microsoft Edge versión 77 o posterior.

## Directivas disponibles
En estas tablas se muestra una lista de todas las directivas de grupo relacionadas con el explorador disponibles en esta versión de Microsoft Edge. Use los vínculos de la tabla para obtener más detalles sobre directivas específicas.

|||
|-|-|
|[Administrador de contraseñas y protección](#administrador-de-contraseñas-y-protección)|[Autenticación HTTP](#autenticación-http)|
|[Cast](#cast)|[Configuración de SmartScreen](#configuración-de-smartscreen)|
|[Configuración de contenido](#configuración-de-contenido)|[Extensiones](#extensiones)|
|[Imprimir](#imprimir)|[Inicio, página principal y página de la nueva pestaña](#inicio,-página-principal-y-página-de-la-nueva-pestaña)|
|[Mensajería nativa](#mensajería-nativa)|[Proveedor de búsquedas predeterminado](#proveedor-de-búsquedas-predeterminado)|
|[Servidor proxy](#servidor-proxy)|[Additional](#additional)|


### [*Administrador de contraseñas y protección*](#administrador-de-contraseñas-y-protección-policies)
|Nombre de directiva|Título|
|-|-|
|[PasswordManagerEnabled](#passwordmanagerenabled)|Habilitar guardar contraseñas en el administrador de contraseñas|
|[PasswordProtectionChangePasswordURL](#passwordprotectionchangepasswordurl)|Configurar la URL de cambio de contraseña|
|[PasswordProtectionLoginURLs](#passwordprotectionloginurls)|Configure la lista de URL de inicio de sesión de empresa en las que el servicio de protección de contraseñas debe capturar la huella digital de la contraseña|
|[PasswordProtectionWarningTrigger](#passwordprotectionwarningtrigger)|Configurar desencadenador de advertencia de protección de contraseñas|
### [*Autenticación HTTP*](#autenticación-http-policies)
|Nombre de directiva|Título|
|-|-|
|[AllowCrossOriginAuthPrompt](#allowcrossoriginauthprompt)|Permitir avisos de autenticación básica de HTTP de origen cruzado|
|[AuthNegotiateDelegateAllowlist](#authnegotiatedelegateallowlist)|Especifica una lista de servidores a los que Microsoft Edge puede delegar credenciales de usuario|
|[AuthSchemes](#authschemes)|Esquemas de autenticación admitidos|
|[AuthServerAllowlist](#authserverallowlist)|Configurar lista de servidores de autenticación permitidos|
|[DisableAuthNegotiateCnameLookup](#disableauthnegotiatecnamelookup)|Deshabilitar búsqueda de CNAME al negociar la autenticación Kerberos|
|[EnableAuthNegotiatePort](#enableauthnegotiateport)|Incluir el puerto no estándar en Kerberos SPN|
|[NtlmV2Enabled](#ntlmv2enabled)|Controlar si la autenticación NTLMv2 está habilitada|
### [*Cast*](#cast-policies)
|Nombre de directiva|Título|
|-|-|
|[EnableMediaRouter](#enablemediarouter)|Habilitar Google Cast|
|[ShowCastIconInToolbar](#showcasticonintoolbar)|Mostrar el icono de transmisión en la barra de herramientas|
### [*Configuración de SmartScreen*](#configuración-de-smartscreen-policies)
|Nombre de directiva|Título|
|-|-|
|[PreventSmartScreenPromptOverride](#preventsmartscreenpromptoverride)|Impedir que se pasen por alto de Sm los avisos de SmartScreen de Microsoft Defender para sitios|
|[PreventSmartScreenPromptOverrideForFiles](#preventsmartscreenpromptoverrideforfiles)|Impedir que se omitan las advertencias de SmartScreen de Microsoft Defender sobre las descargas|
|[SmartScreenAllowListDomains](#smartscreenallowlistdomains)|Configurar la lista de dominios para los que SmartScreen de Microsoft Defender no desencadenará advertencias|
|[SmartScreenEnabled](#smartscreenenabled)|Configurar SmartScreen de Microsoft Defender|
|[SmartScreenForTrustedDownloadsEnabled](#smartscreenfortrusteddownloadsenabled)|Forzar las comprobaciones de SmartScreen de Microsoft Defender en las descargas de fuentes de confianza|
|[SmartScreenPuaEnabled](#smartscreenpuaenabled)|Configurar SmartScreen de Microsoft Defender para bloquear aplicaciones potencialmente no deseadas|
### [*Configuración de contenido*](#configuración-de-contenido-policies)
|Nombre de directiva|Título|
|-|-|
|[AutoSelectCertificateForUrls](#autoselectcertificateforurls)|Seleccionar automáticamente certificados de cliente para estos sitios|
|[CookiesAllowedForUrls](#cookiesallowedforurls)|Permitir cookies en sitios específicos|
|[CookiesBlockedForUrls](#cookiesblockedforurls)|Bloquear cookies en sitios específicos|
|[CookiesSessionOnlyForUrls](#cookiessessiononlyforurls)|Limitar las cookies de sitios web específicos a la sesión actual|
|[DefaultCookiesSetting](#defaultcookiessetting)|Configurar cookies|
|[DefaultGeolocationSetting](#defaultgeolocationsetting)|Configuración de geolocalización predeterminada|
|[DefaultImagesSetting](#defaultimagessetting)|Configuración predeterminada de imágenes|
|[DefaultJavaScriptSetting](#defaultjavascriptsetting)|Configuración predeterminada de JavaScript|
|[DefaultNotificationsSetting](#defaultnotificationssetting)|Configuración de notificaciones predeterminada|
|[DefaultPluginsSetting](#defaultpluginssetting)|Configuración de Adobe Flash predeterminada|
|[DefaultPopupsSetting](#defaultpopupssetting)|Configuración de ventana emergente predeterminada|
|[DefaultWebBluetoothGuardSetting](#defaultwebbluetoothguardsetting)|Controlar el uso de la API Web Bluetooth|
|[DefaultWebUsbGuardSetting](#defaultwebusbguardsetting)|Controlar el uso de la API WebUSB|
|[ImagesAllowedForUrls](#imagesallowedforurls)|Permitir imágenes en estos sitios|
|[ImagesBlockedForUrls](#imagesblockedforurls)|Bloquear imágenes en sitios específicos|
|[JavaScriptAllowedForUrls](#javascriptallowedforurls)|Permitir JavaScript en sitios específicos|
|[JavaScriptBlockedForUrls](#javascriptblockedforurls)|Bloquear JavaScript en sitios específicos|
|[LegacySameSiteCookieBehaviorEnabled](#legacysamesitecookiebehaviorenabled)|Habilitar la configuración del comportamiento de cookies de SameSite heredadas predefinido|
|[LegacySameSiteCookieBehaviorEnabledForDomainList](#legacysamesitecookiebehaviorenabledfordomainlist)|Revertir al comportamiento de SameSite heredado para cookies en sitios especificados|
|[NotificationsAllowedForUrls](#notificationsallowedforurls)|Permitir notificaciones en sitios específicos|
|[NotificationsBlockedForUrls](#notificationsblockedforurls)|Bloquear notificaciones en sitios específicos|
|[PluginsAllowedForUrls](#pluginsallowedforurls)|Permitir el complemento de Adobe Flash en sitios específicos|
|[PluginsBlockedForUrls](#pluginsblockedforurls)|Bloquear el complemento de Adobe Flash en sitios específicos|
|[PopupsAllowedForUrls](#popupsallowedforurls)|Permitir ventanas emergentes en sitios específicos|
|[PopupsBlockedForUrls](#popupsblockedforurls)|Bloquear ventanas emergentes en sitios específicos|
|[RegisteredProtocolHandlers](#registeredprotocolhandlers)|Registrar controladores de protocolo|
|[WebUsbAllowDevicesForUrls](#webusballowdevicesforurls)|Conceder acceso a sitios específicos para conectarse a dispositivos USB específicos|
|[WebUsbAskForUrls](#webusbaskforurls)|Permitir WebUSB en sitios específicos|
|[WebUsbBlockedForUrls](#webusbblockedforurls)|Bloquear WebUSB en sitios específicos|
### [*Extensiones*](#extensiones-policies)
|Nombre de directiva|Título|
|-|-|
|[ExtensionAllowedTypes](#extensionallowedtypes)|Configurar tipos de extensiones permitidos|
|[ExtensionInstallAllowlist](#extensioninstallallowlist)|Permitir la instalación de extensiones específicas|
|[ExtensionInstallBlocklist](#extensioninstallblocklist)|Controlar las extensiones que no se pueden instalar|
|[ExtensionInstallForcelist](#extensioninstallforcelist)|Controlar las extensiones que se instalan en modo silencioso|
|[ExtensionInstallSources](#extensioninstallsources)|Configurar extensión y orígenes de instalación de script de usuario|
|[ExtensionSettings](#extensionsettings)|Configurar ajustes de administración de extensiones|
### [*Imprimir*](#imprimir-policies)
|Nombre de directiva|Título|
|-|-|
|[DefaultPrinterSelection](#defaultprinterselection)|Reglas de selección de impresora predeterminada|
|[PrintHeaderFooter](#printheaderfooter)|Imprimir encabezados y pies de página|
|[PrintPreviewUseSystemDefaultPrinter](#printpreviewusesystemdefaultprinter)|Establecer la impresora predeterminada del sistema como la impresora predeterminada|
|[PrintingEnabled](#printingenabled)|Habilitar la impresión|
|[UseSystemPrintDialog](#usesystemprintdialog)|Imprimir usando el cuadro de diálogo de impresión|
### [*Inicio&comma; página principal y página de la nueva pestaña*](#inicio-página-principal-y-página-de-la-nueva-pestaña-policies)
|Nombre de directiva|Título|
|-|-|
|[HomepageIsNewTabPage](#homepageisnewtabpage)|Establecer la página de la nueva pestaña como página principal|
|[HomepageLocation](#homepagelocation)|Configurar la dirección URL de la página principal|
|[NewTabPageCompanyLogo](#newtabpagecompanylogo)|Establecer el logotipo de la empresa en la nueva ficha|
|[NewTabPageHideDefaultTopSites](#newtabpagehidedefaulttopsites)|Ocultar los sitios principales predeterminados de la página de la nueva pestaña|
|[NewTabPageLocation](#newtabpagelocation)|Configurar la dirección URL de la página de la nueva pestaña|
|[NewTabPageManagedQuickLinks](#newtabpagemanagedquicklinks)|Establecer vínculos rápidos a la página de la nueva pestaña|
|[NewTabPageSetFeedType](#newtabpagesetfeedtype)|Configurar la experiencia de página de la nueva pestaña de Microsoft Edge|
|[RestoreOnStartup](#restoreonstartup)|Acción que se realizará al inicio|
|[RestoreOnStartupURLs](#restoreonstartupurls)|Sitios que se abrirán cuando se inicia el explorador|
|[ShowHomeButton](#showhomebutton)|Mostrar el botón Inicio en la barra de herramientas|
### [*Mensajería nativa*](#mensajería-nativa-policies)
|Nombre de directiva|Título|
|-|-|
|[NativeMessagingAllowlist](#nativemessagingallowlist)|Controlar qué hosts de mensajería nativos pueden usar los usuarios|
|[NativeMessagingBlocklist](#nativemessagingblocklist)|Configurar la lista de bloqueados de mensajes nativa|
|[NativeMessagingUserLevelHosts](#nativemessaginguserlevelhosts)|Permitir hosts de mensajería nativos de nivel de usuario (instalados sin permisos del administrador)|
### [*Proveedor de búsquedas predeterminado*](#proveedor-de-búsquedas-predeterminado-policies)
|Nombre de directiva|Título|
|-|-|
|[DefaultSearchProviderEnabled](#defaultsearchproviderenabled)|Habilitar el proveedor de búsquedas predeterminado|
|[DefaultSearchProviderEncodings](#defaultsearchproviderencodings)|Codificaciones del proveedor de búsquedas predeterminado|
|[DefaultSearchProviderImageURL](#defaultsearchproviderimageurl)|Especifica la característica de búsqueda por imagen para el proveedor de búsquedas predeterminado|
|[DefaultSearchProviderImageURLPostParams](#defaultsearchproviderimageurlpostparams)|Parámetros para una dirección URL de imagen que usa POST|
|[DefaultSearchProviderKeyword](#defaultsearchproviderkeyword)|Palabra clave del proveedor de búsquedas predeterminado|
|[DefaultSearchProviderName](#defaultsearchprovidername)|Nombre del proveedor de búsquedas predeterminado|
|[DefaultSearchProviderSearchURL](#defaultsearchprovidersearchurl)|URL de búsqueda del proveedor de búsquedas predeterminado|
|[DefaultSearchProviderSuggestURL](#defaultsearchprovidersuggesturl)|URL del proveedor de búsqueda predeterminado para obtener sugerencias|
### [*Servidor proxy*](#servidor-proxy-policies)
|Nombre de directiva|Título|
|-|-|
|[ProxyBypassList](#proxybypasslist)|Configurar reglas de omisión de proxy|
|[ProxyMode](#proxymode)|Configurar ajustes del servidor proxy|
|[ProxyPacUrl](#proxypacurl)|Establecer la dirección URL del archivo .pac del proxy|
|[ProxyServer](#proxyserver)|Configurar dirección o URL del servidor proxy|
|[ProxySettings](#proxysettings)|Configuración del proxy|
### [*Additional*](#additional-policies)
|Nombre de directiva|Título|
|-|-|
|[AdsSettingForIntrusiveAdsSites](#adssettingforintrusiveadssites)|Configuración de anuncios para sitios con anuncios intrusivos|
|[AllowDeletingBrowserHistory](#allowdeletingbrowserhistory)|Habilitar la eliminación del explorador y el historial de descarga|
|[AllowFileSelectionDialogs](#allowfileselectiondialogs)|Permitir cuadros de diálogo de selección de archivos|
|[AllowPopupsDuringPageUnload](#allowpopupsduringpageunload)|Permite que una página muestre elementos emergentes durante su descarga|
|[AllowSyncXHRInPageDismissal](#allowsyncxhrinpagedismissal)|Permitir que las páginas envíen solicitudes sincrónicas de XHR durante el descarte de páginas|
|[AllowTrackingForUrls](#allowtrackingforurls)|Configurar excepciones de prevención de seguimiento para sitios específicos|
|[AlwaysOpenPdfExternally](#alwaysopenpdfexternally)|Abrir siempre archivos PDF externamente|
|[ApplicationLocaleValue](#applicationlocalevalue)|Establecer la configuración regional de aplicación|
|[AudioCaptureAllowed](#audiocaptureallowed)|Permitir o bloquear la captura de audio|
|[AudioCaptureAllowedUrls](#audiocaptureallowedurls)|Sitios que pueden acceder a dispositivos de captura de audio sin solicitar permiso|
|[AutoImportAtFirstRun](#autoimportatfirstrun)|Importar automáticamente los datos y la configuración de otro explorador la primera vez que se ejecute|
|[AutofillAddressEnabled](#autofilladdressenabled)|Habilitar Autorrellenar para direcciones|
|[AutofillCreditCardEnabled](#autofillcreditcardenabled)|Habilitar Autorrellenar para tarjetas de crédito|
|[AutoplayAllowed](#autoplayallowed)|Permitir la reproducción automática de multimedia para sitios web|
|[BackgroundModeEnabled](#backgroundmodeenabled)|Continúa con la ejecución de aplicaciones en segundo plano después de cerrar Microsoft Edge|
|[BackgroundTemplateListUpdatesEnabled](#backgroundtemplatelistupdatesenabled)|Habilita actualizaciones en segundo plano para la lista de plantillas disponibles para Colecciones y otras características que usan plantillas.|
|[BlockThirdPartyCookies](#blockthirdpartycookies)|Bloquear cookies de terceros|
|[BrowserAddProfileEnabled](#browseraddprofileenabled)|Habilitar la creación de perfiles desde el menú desplegable Identidad o la página de configuración|
|[BrowserGuestModeEnabled](#browserguestmodeenabled)|Habilitar el modo Invitado|
|[BrowserNetworkTimeQueriesEnabled](#browsernetworktimequeriesenabled)|Permitir consultas a un servicio de hora de red de explorador|
|[BrowserSignin](#browsersignin)|Configuración de inicio de sesión del explorador|
|[BuiltInDnsClientEnabled](#builtindnsclientenabled)|Usar el cliente DNS integrado|
|[CertificateTransparencyEnforcementDisabledForCas](#certificatetransparencyenforcementdisabledforcas)|Deshabilitar el cumplimiento de la transparencia de certificados para obtener una lista de hashes subjectPublicKeyInfo|
|[CertificateTransparencyEnforcementDisabledForLegacyCas](#certificatetransparencyenforcementdisabledforlegacycas)|Deshabilitar la aplicación de la transparencia de certificados para una lista de entidades de certificación heredadas|
|[CertificateTransparencyEnforcementDisabledForUrls](#certificatetransparencyenforcementdisabledforurls)|Deshabilitar el cumplimiento de transparencia de certificados para direcciones URL específicas|
|[ClearBrowsingDataOnExit](#clearbrowsingdataonexit)|Borrar los datos de exploración al cerrar Microsoft Edge|
|[ClickOnceEnabled](#clickonceenabled)|Permitir a los usuarios abrir archivos con el protocolo ClickOnce|
|[CommandLineFlagSecurityWarningsEnabled](#commandlineflagsecuritywarningsenabled)|Habilitar advertencias de seguridad para marcadores de la línea de comandos|
|[ComponentUpdatesEnabled](#componentupdatesenabled)|Habilitar actualizaciones de componentes en Microsoft Edge|
|[ConfigureDoNotTrack](#configuredonottrack)|Configurar No realizar seguimiento|
|[ConfigureOnlineTextToSpeech](#configureonlinetexttospeech)|Configurar texto a voz en línea|
|[CustomHelpLink](#customhelplink)|Especificar vínculo de ayuda personalizado|
|[DefaultBrowserSettingEnabled](#defaultbrowsersettingenabled)|Establecer Microsoft Edge como el explorador predeterminado|
|[DeveloperToolsAvailability](#developertoolsavailability)|Controlar dónde se pueden usar las herramientas de desarrollo|
|[DirectInvokeEnabled](#directinvokeenabled)|Permitir a los usuarios abrir archivos con el protocolo DirectInvoke|
|[Disable3DAPIs](#disable3dapis)|Deshabilitar el soporte de las API de gráficos 3D|
|[DisableScreenshots](#disablescreenshots)|Deshabilitar la captura de pantalla|
|[DiskCacheDir](#diskcachedir)|Establecer el directorio de memoria caché del disco|
|[DiskCacheSize](#diskcachesize)|Establecer tamaño de caché de disco, en bytes|
|[DownloadDirectory](#downloaddirectory)|Establecer el directorio de descarga|
|[DownloadRestrictions](#downloadrestrictions)|Permitir restricciones de descarga|
|[EdgeCollectionsEnabled](#edgecollectionsenabled)|Habilitar la característica Colecciones|
|[EditFavoritesEnabled](#editfavoritesenabled)|Permite a los usuarios editar los favoritos|
|[EnableDeprecatedWebPlatformFeatures](#enabledeprecatedwebplatformfeatures)|Volver a habilitar las características de la plataforma web en desuso durante un tiempo limitado|
|[EnableDomainActionsDownload](#enabledomainactionsdownload)|Habilitar la descarga de acciones de dominio desde Microsoft|
|[EnableOnlineRevocationChecks](#enableonlinerevocationchecks)|Habilitar comprobaciones de CRL/OCSP en línea|
|[EnterpriseHardwarePlatformAPIEnabled](#enterprisehardwareplatformapienabled)|Permitir que las extensiones administradas usen la API de la plataforma de hardware empresarial|
|[ExperimentationAndConfigurationServiceControl](#experimentationandconfigurationservicecontrol)|Controlar la comunicación con el servicio de configuración y experimentación|
|[ExternalProtocolDialogShowAlwaysOpenCheckbox](#externalprotocoldialogshowalwaysopencheckbox)|Mostrar una casilla "Abrir siempre" en el diálogo de protocolo externo.|
|[FavoritesBarEnabled](#favoritesbarenabled)|Habilitar barra de favoritos|
|[ForceBingSafeSearch](#forcebingsafesearch)|Aplicar Búsqueda segura de Bing|
|[ForceEphemeralProfiles](#forceephemeralprofiles)|Habilitar el uso de perfiles efímeros|
|[ForceGoogleSafeSearch](#forcegooglesafesearch)|Aplicar la Búsqueda segura de Google|
|[ForceNetworkInProcess](#forcenetworkinprocess)|Forzar el código de red para que se ejecute en el proceso del explorador|
|[ForceYouTubeRestrict](#forceyoutuberestrict)|Forzar el modo Restringido mínimo en YouTube|
|[FullscreenAllowed](#fullscreenallowed)|Permitir modo de pantalla completa|
|[GoToIntranetSiteForSingleWordEntryInAddressBar](#gotointranetsiteforsinglewordentryinaddressbar)|Fuerce la navegación directa en el sitio de intranet en lugar de buscar entradas de una única palabra en la barra de direcciones.|
|[HSTSPolicyBypassList](#hstspolicybypasslist)|Configurar la lista de nombres que omitirán la comprobación de directiva de HSTS|
|[HardwareAccelerationModeEnabled](#hardwareaccelerationmodeenabled)|Usar aceleración de hardware cuando esté disponible|
|[ImportAutofillFormData](#importautofillformdata)|Permitir la importación de datos de Autorrellenar del formulario|
|[ImportBrowserSettings](#importbrowsersettings)|Permitir la importación de la configuración del explorador|
|[ImportFavorites](#importfavorites)|Permitir la importación de favoritos|
|[ImportHistory](#importhistory)|Permitir la importación del historial de exploración|
|[ImportHomepage](#importhomepage)|Permitir la importación de la configuración de la página principal|
|[ImportOpenTabs](#importopentabs)|Permitir la importación de pestañas abiertas|
|[ImportPaymentInfo](#importpaymentinfo)|Permitir la importación de información de pago|
|[ImportSavedPasswords](#importsavedpasswords)|Permitir la importación de contraseñas guardadas|
|[ImportSearchEngine](#importsearchengine)|Permitir la importación de la configuración del motor de búsqueda|
|[InPrivateModeAvailability](#inprivatemodeavailability)|Configurar la disponibilidad del modo InPrivate|
|[InternetExplorerIntegrationLevel](#internetexplorerintegrationlevel)|Configurar la integración de Internet Explorer|
|[InternetExplorerIntegrationSiteList](#internetexplorerintegrationsitelist)|Configurar la lista de sitios del modo de empresa|
|[InternetExplorerIntegrationSiteRedirect](#internetexplorerintegrationsiteredirect)|Especificar cómo se comportan las exploraciones "en la página" para sitios no configurados cuando se inician desde páginas en el modo de Internet Explorer|
|[IsolateOrigins](#isolateorigins)|Habilitar el aislamiento de sitios para orígenes específicos|
|[ManagedFavorites](#managedfavorites)|Configurar favoritos|
|[ManagedSearchEngines](#managedsearchengines)|Administrar motores de búsqueda|
|[MaxConnectionsPerProxy](#maxconnectionsperproxy)|Número máximo de conexiones simultáneas al servidor proxy|
|[MediaRouterCastAllowAllIPs](#mediaroutercastallowallips)|Permitir que Google Cast se conecte con dispositivos de Cast en todas las direcciones IP|
|[MetricsReportingEnabled](#metricsreportingenabled)|Habilitar el uso y los informes de datos relacionados con el bloqueo|
|[NetworkPredictionOptions](#networkpredictionoptions)|Habilitar la predicción de red|
|[NonRemovableProfileEnabled](#nonremovableprofileenabled)|Configurar si un usuario siempre tiene un perfil predeterminado con sesión iniciada automáticamente con su cuenta profesional o educativa|
|[OverrideSecurityRestrictionsOnInsecureOrigin](#overridesecurityrestrictionsoninsecureorigin)|Controlar dónde se aplican restricciones de seguridad en los orígenes no seguros|
|[PinningWizardAllowed](#pinningwizardallowed)|Allow Pin to taskbar wizard|
|[ProactiveAuthEnabled](#proactiveauthenabled)|Habilitar autenticación proactiva|
|[PromotionalTabsEnabled](#promotionaltabsenabled)|Habilitar el contenido promocional en toda la pestaña|
|[PromptForDownloadLocation](#promptfordownloadlocation)|Preguntar dónde guardar los archivos descargados|
|[QuicAllowed](#quicallowed)|Permitir protocolo QUIC|
|[RelaunchNotification](#relaunchnotification)|Notificar al usuario que se recomienda o se requiere reiniciar el explorador para las actualizaciones pendientes|
|[RelaunchNotificationPeriod](#relaunchnotificationperiod)|Establecer el período de tiempo para las notificaciones de actualización|
|[RendererCodeIntegrityEnabled](#renderercodeintegrityenabled)|Habilitar la integridad del código del procesador|
|[RequireOnlineRevocationChecksForLocalAnchors](#requireonlinerevocationchecksforlocalanchors)|Especificar si las comprobaciones CRL/OCSP en línea son obligatorias para los delimitadores locales de confianza|
|[ResolveNavigationErrorsUseWebService](#resolvenavigationerrorsusewebservice)|Habilitar la resolución de errores de navegación mediante un servicio web|
|[RestrictSigninToPattern](#restrictsignintopattern)|Restringir las cuentas que pueden usarse como cuentas principales de Microsoft Edge|
|[RunAllFlashInAllowMode](#runallflashinallowmode)|Extender la configuración de contenidos de Adobe Flash a todos los contenido|
|[SSLErrorOverrideAllowed](#sslerroroverrideallowed)|Permitir que los usuarios continúen desde la página de advertencia de HTTPS|
|[SSLVersionMin](#sslversionmin)|Versión mínima de TLS habilitada|
|[SavingBrowserHistoryDisabled](#savingbrowserhistorydisabled)|Deshabilitar guardar el historial del explorador|
|[SearchSuggestEnabled](#searchsuggestenabled)|Habilitar sugerencias de búsqueda|
|[SecurityKeyPermitAttestation](#securitykeypermitattestation)|Sitios web o dominios que no necesitan permiso para usar la atestación de clave de seguridad directa|
|[SendIntranetToInternetExplorer](#sendintranettointernetexplorer)|Enviar todos los sitios de la intranet a Internet Explorer|
|[SendSiteInfoToImproveServices](#sendsiteinfotoimproveservices)|Enviar información del sitio para mejorar los servicios Microsoft|
|[ShowOfficeShortcutInFavoritesBar](#showofficeshortcutinfavoritesbar)|Mostrar el acceso directo de Microsoft Office en la barra de favoritos|
|[SignedHTTPExchangeEnabled](#signedhttpexchangeenabled)|Habilitar la compatibilidad con Exchange firmado de HTTP (SXG)|
|[SitePerProcess](#siteperprocess)|Habilitar el aislamiento de sitios para cada sitio|
|[SpellcheckEnabled](#spellcheckenabled)|Habilitar corrector ortográfico|
|[SpellcheckLanguage](#spellchecklanguage)|Habilitar los idiomas de corrección ortográfica específicos|
|[SpellcheckLanguageBlocklist](#spellchecklanguageblocklist)|Forzar deshabilitar idiomas de corrección ortográfica|
|[SuppressUnsupportedOSWarning](#suppressunsupportedoswarning)|Suprimir la advertencia de sistema operativo no compatible|
|[SyncDisabled](#syncdisabled)|Deshabilitar la sincronización de datos mediante los servicios de sincronización de Microsoft|
|[TabFreezingEnabled](#tabfreezingenabled)|Permitir la inmovilización de pestañas en segundo plano|
|[TaskManagerEndProcessEnabled](#taskmanagerendprocessenabled)|Habilitar finalizar procesos en el Administrador de tareas del explorador|
|[TrackingPrevention](#trackingprevention)|Bloquear el seguimiento de la actividad de exploración web de los usuarios|
|[TranslateEnabled](#translateenabled)|Habilitar Traducir|
|[URLAllowlist](#urlallowlist)|Definir una lista de direcciones URL permitidas|
|[URLBlocklist](#urlblocklist)|Bloquear el acceso a una lista de direcciones URL|
|[UserDataDir](#userdatadir)|Establecer el directorio de datos de usuario|
|[UserFeedbackAllowed](#userfeedbackallowed)|Permitir comentarios del usuario|
|[VideoCaptureAllowed](#videocaptureallowed)|Permitir o bloquear la captura de vídeo|
|[VideoCaptureAllowedUrls](#videocaptureallowedurls)|Sitios que pueden acceder a dispositivos de captura de vídeo sin solicitar permiso|
|[WPADQuickCheckEnabled](#wpadquickcheckenabled)|Establecer la optimización de WPAD|
|[WebDriverOverridesIncompatiblePolicies](#webdriveroverridesincompatiblepolicies)|Permitir que WebDriver invalide las directivas incompatibles|
|[WebRtcLocalhostIpHandling](#webrtclocalhostiphandling)|Restringir la exposición de la dirección IP de localhost por WebRTC|
|[WebRtcUdpPortRange](#webrtcudpportrange)|Restringir el intervalo de puertos UDP locales usados por WebRTC|




  ## Administrador de contraseñas y protección policies

  [Volver al principio](#microsoft-edge:-directivas)

  ### PasswordManagerEnabled
  #### Habilitar guardar contraseñas en el administrador de contraseñas
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Habilitar Microsoft Edge para guardar las contraseñas de usuario.

Si se habilita esta directiva, los usuarios pueden guardar sus contraseñas en Microsoft Edge. La próxima vez que visiten el sitio, Microsoft Edge introducirá automáticamente la contraseña.

Si se deshabilita esta directiva, los usuarios no pueden guardar nuevas contraseñas, pero pueden usar contraseñas guardadas con anterioridad.

Si se habilita o se deshabilita esta directiva, los usuarios no pueden cambiarla ni reemplazarla en Microsoft Edge. Si no se configura, los usuarios podrán guardar sus contraseñas y desactivar esta característica.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: Sí
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Booleano

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: PasswordManagerEnabled
  - Nombre de la directiva de grupos: Habilitar guardar contraseñas en el administrador de contraseñas
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/Administrador de contraseñas y protección
  - Ruta de acceso de GP (Recomendada): Plantillas administrativas/Microsoft Edge - Configuración predeterminada (los usuarios pueden cambiarla)/Administrador de contraseñas y protección
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): SOFTWARE\Policies\Microsoft\Edge\Recomendada
  - Nombre del valor: PasswordManagerEnabled
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000001
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: PasswordManagerEnabled
  - Valor de ejemplo:
``` xml
<true/>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### PasswordProtectionChangePasswordURL
  #### Configurar la URL de cambio de contraseña
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Configura la URL de cambio de contraseña (solo esquemas HTTP y HTTPS).

El servicio de protección de contraseñas enviará a los usuarios a esta URL para cambiar su contraseña después de ver una advertencia en el explorador.

Si se habilita esta directiva, el servicio de protección de contraseñas enviará a los usuarios a esta URL para cambiar su contraseña.

Si se deshabilita esta directiva o no se configura, el servicio de protección de contraseñas no redirigirá a los usuarios a una URL de cambio de contraseña.

Esta directiva solo está disponible en las instancias de Windows que están unidas a un dominio de Microsoft Active Directory o en las instancias de Windows 10 Pro o Enterprise que están inscritas para la administración de dispositivos.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Cadena

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: PasswordProtectionChangePasswordURL
  - Nombre de la directiva de grupos: Configurar la URL de cambio de contraseña
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/Administrador de contraseñas y protección
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: PasswordProtectionChangePasswordURL
  - Tipo de valor: REG_SZ
  ##### Valor de ejemplo:
```
"https://contoso.com/change_password.html"
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: PasswordProtectionChangePasswordURL
  - Valor de ejemplo:
``` xml
<string>https://contoso.com/change_password.html</string>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### PasswordProtectionLoginURLs
  #### Configure la lista de URL de inicio de sesión de empresa en las que el servicio de protección de contraseñas debe capturar la huella digital de la contraseña
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Configure la lista de direcciones URL de inicio de sesión de empresa (solo esquemas HTTP y HTTPS) en las que Microsoft Edge debe capturar la huella digital de las contraseñas y usarla para la detección de reutilización de contraseñas.

Si se habilita esta directiva, el servicio de protección de contraseñas capturará huellas digitales de las contraseñas en las direcciones URL definidas.

Si se deshabilita esta directiva o no se configura, no se capturarán huellas digitales de las contraseñas.

Esta directiva solo está disponible en las instancias de Windows que están unidas a un dominio de Microsoft Active Directory o en las instancias de Windows 10 Pro o Enterprise que están inscritas para la administración de dispositivos.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Lista de cadenas

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: PasswordProtectionLoginURLs
  - Nombre de la directiva de grupos: Configure la lista de URL de inicio de sesión de empresa en las que el servicio de protección de contraseñas debe capturar la huella digital de la contraseña
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/Administrador de contraseñas y protección
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge\PasswordProtectionLoginURLs
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: 1, 2, 3, ...
  - Tipo de valor: lista de REG_SZ
  ##### Valor de ejemplo:
```
SOFTWARE\Policies\Microsoft\Edge\PasswordProtectionLoginURLs\0 = "https://contoso.com/login.html"
SOFTWARE\Policies\Microsoft\Edge\PasswordProtectionLoginURLs\1 = "https://login.contoso.com"

```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: PasswordProtectionLoginURLs
  - Valor de ejemplo:
``` xml
<array>
  <string>https://contoso.com/login.html</string>
  <string>https://login.contoso.com</string>
</array>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### PasswordProtectionWarningTrigger
  #### Configurar desencadenador de advertencia de protección de contraseñas
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Permite controlar cuándo se debe desencadenar la advertencia de protección con contraseña. La protección con contraseña alerta a los usuarios cuando reutilizan su contraseña protegida en sitios potencialmente sospechosos.

Se pueden usar las directivas [PasswordProtectionLoginURLs](#passwordprotectionloginurls) y [PasswordProtectionChangePasswordURL](#passwordprotectionchangepasswordurl) para configurar las contraseñas que se van a proteger.

Exenciones: las contraseñas de los sitios que aparecen en [PasswordProtectionLoginURLs](#passwordprotectionloginurls) y [PasswordProtectionChangePasswordURL](#passwordprotectionchangepasswordurl), así como las de los sitios que aparecen en [SmartScreenAllowListDomains](#smartscreenallowlistdomains), no desencadenarán una advertencia de protección con contraseña.

Se debe establecer en "PasswordProtectionWarningOff" (0) para no mostrar advertencias de protección con contraseña.

Se debe establecer en "PasswordProtectionWarningOnPasswordReuse" (1) para mostrar advertencias de protección con contraseña cuando el usuario reutiliza su contraseña protegida en un sitio no perteneciente a la lista de permitidos.

Si se deshabilita o no se configuras esta directiva, no se mostrará el desencadenador de advertencia.

* 0 = Advertencia de protección con contraseña desactivada

* 1 = Advertencia de protección con contraseña se desencadena con la reutilización de contraseñas.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Entero

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: PasswordProtectionWarningTrigger
  - Nombre de la directiva de grupos: Configurar desencadenador de advertencia de protección de contraseñas
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/Administrador de contraseñas y protección
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: PasswordProtectionWarningTrigger
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000001
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: PasswordProtectionWarningTrigger
  - Valor de ejemplo:
``` xml
<integer>1</integer>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ## Autenticación HTTP policies

  [Volver al principio](#microsoft-edge:-directivas)

  ### AllowCrossOriginAuthPrompt
  #### Permitir avisos de autenticación básica de HTTP de origen cruzado
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Controla si el subcontenido de terceros de una página puede abrir un cuadro de diálogo de autenticación básica de HTTP.

Normalmente, esto está deshabilitado como una defensa de suplantación de identidad. Si no configura esta directiva, estará deshabilitado y el subcontenido de terceros no podrá abrir un cuadro de diálogo de autenticación básica de HTTP.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Booleano

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: AllowCrossOriginAuthPrompt
  - Nombre de la directiva de grupos: Permitir avisos de autenticación básica de HTTP de origen cruzado
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/Autenticación HTTP
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: AllowCrossOriginAuthPrompt
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000000
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: AllowCrossOriginAuthPrompt
  - Valor de ejemplo:
``` xml
<false/>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### AuthNegotiateDelegateAllowlist
  #### Especifica una lista de servidores a los que Microsoft Edge puede delegar credenciales de usuario
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Configure la lista de servidores en los que puede delegar Microsoft Edge.

Separe los nombres de los distintos servidores con comas. Se permiten caracteres comodín (*).

Si no se configura esta directiva, Microsoft Edge no delegará las credenciales de usuario aunque se detecte un servidor como Intranet.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: No - Requiere reiniciar el explorador

  #### Tipo de datos:
  Cadena

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: AuthNegotiateDelegateAllowlist
  - Nombre de la directiva de grupos: Especifica una lista de servidores a los que Microsoft Edge puede delegar credenciales de usuario
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/Autenticación HTTP
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: AuthNegotiateDelegateAllowlist
  - Tipo de valor: REG_SZ
  ##### Valor de ejemplo:
```
"contoso.com"
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: AuthNegotiateDelegateAllowlist
  - Valor de ejemplo:
``` xml
<string>contoso.com</string>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### AuthSchemes
  #### Esquemas de autenticación admitidos
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Especifica los esquemas de autenticación HTTP que se admiten.

Puede configurarse la directiva usando estos valores: 'basic', 'digest', 'ntlm' y 'negotiate'. Los valores múltiples deben estar separados por comas.

Si no se configura esta directiva, se usan los cuatro esquemas.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: No - Requiere reiniciar el explorador

  #### Tipo de datos:
  Cadena

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: AuthSchemes
  - Nombre de la directiva de grupos: Esquemas de autenticación admitidos
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/Autenticación HTTP
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: AuthSchemes
  - Tipo de valor: REG_SZ
  ##### Valor de ejemplo:
```
"basic,digest,ntlm,negotiate"
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: AuthSchemes
  - Valor de ejemplo:
``` xml
<string>basic,digest,ntlm,negotiate</string>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### AuthServerAllowlist
  #### Configurar lista de servidores de autenticación permitidos
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Especifica los servidores que se habilitarán para la autenticación integrada. La autenticación integrada solo se habilita cuando Microsoft Edge recibe un desafío de autenticación de un proxy o de un servidor en esta lista.

Separe los nombres de varios servidores con comas. Se permiten caracteres comodín (*).

Si no se configura esta directiva, Microsoft Edge intenta detectar si un servidor se encuentra en la intranet; solo entonces responderá a las solicitudes de IWA. Si el servidor está en Internet, Microsoft Edge omitirá las solicitudes de IWA.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: No - Requiere reiniciar el explorador

  #### Tipo de datos:
  Cadena

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: AuthServerAllowlist
  - Nombre de la directiva de grupos: Configurar lista de servidores de autenticación permitidos
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/Autenticación HTTP
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: AuthServerAllowlist
  - Tipo de valor: REG_SZ
  ##### Valor de ejemplo:
```
"*contoso.com,contoso.com"
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: AuthServerAllowlist
  - Valor de ejemplo:
``` xml
<string>*contoso.com,contoso.com</string>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### DisableAuthNegotiateCnameLookup
  #### Deshabilitar búsqueda de CNAME al negociar la autenticación Kerberos
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Determina si el SPN de Kerberos generado se basa en el nombre DNS canónico (CNAME) o en el nombre original especificado.

Si se habilita esta directiva, se omitirá la búsqueda CNAME y se usará el nombre del servidor (como se indicó).

Si se deshabilita esta directiva o no se configura, se usará el nombre canónico del servidor. Esto se determina a través de la búsqueda CNAME.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: No - Requiere reiniciar el explorador

  #### Tipo de datos:
  Booleano

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: DisableAuthNegotiateCnameLookup
  - Nombre de la directiva de grupos: Deshabilitar búsqueda de CNAME al negociar la autenticación Kerberos
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/Autenticación HTTP
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: DisableAuthNegotiateCnameLookup
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000000
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: DisableAuthNegotiateCnameLookup
  - Valor de ejemplo:
``` xml
<false/>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### EnableAuthNegotiatePort
  #### Incluir el puerto no estándar en Kerberos SPN
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Especifica si el SPN Kerberos generado debe incluir un puerto no estándar.

Si se habilita esta directiva y un usuario incluye un puerto no estándar (es decir, un puerto distinto de 80 o 443) en una dirección URL, el puerto está incluido en el SPN Kerberos generado.

Si no se configura o se deshabilita esta directiva, el SPN Kerberos generado no incluirá un puerto en ningún caso.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: No - Requiere reiniciar el explorador

  #### Tipo de datos:
  Booleano

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: EnableAuthNegotiatePort
  - Nombre de la directiva de grupos: Incluir el puerto no estándar en Kerberos SPN
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/Autenticación HTTP
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: EnableAuthNegotiatePort
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000000
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: EnableAuthNegotiatePort
  - Valor de ejemplo:
``` xml
<false/>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### NtlmV2Enabled
  #### Controlar si la autenticación NTLMv2 está habilitada
  >Versiones admitidas: Microsoft Edge en Mac desde la versión 77 o posterior

  #### Descripción
  Controla si NTLMv2 está habilitado.

Todas las versiones recientes de los servidores Samba y Windows son compatibles con NTLMv2. Solo debe deshabilitar NTLMv2 para solucionar problemas con la compatibilidad con versiones anteriores, ya que reduce la seguridad de la autenticación.

Si no configura esta directiva, NTLMv2 estará habilitado de manera predeterminada.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Booleano

  

  #### Información y configuración de Mac
  - Nombre de clave de preferencia: NtlmV2Enabled
  - Valor de ejemplo:
``` xml
<true/>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ## Cast policies

  [Volver al principio](#microsoft-edge:-directivas)

  ### EnableMediaRouter
  #### Habilitar Google Cast
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Habilitar esta directiva para habilitar Google Cast. Los usuarios podrán iniciarla desde el menú de aplicaciones, los menús contextuales de página, los controles de multimedia en sitios web habilitados para Cast y (si se muestra) el icono de la barra de herramientas de Cast.

Deshabilita esta directiva para deshabilitar Google Cast.

Google Cast está habilitado de forma predeterminada.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: No - Requiere reiniciar el explorador

  #### Tipo de datos:
  Booleano

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: EnableMediaRouter
  - Nombre de la directiva de grupos: Habilitar Google Cast
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/Cast
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: EnableMediaRouter
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000001
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: EnableMediaRouter
  - Valor de ejemplo:
``` xml
<true/>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### ShowCastIconInToolbar
  #### Mostrar el icono de transmisión en la barra de herramientas
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Establezca esta directiva en true para mostrar el icono de la barra de herramientas de conversión en la barra de herramientas o en el menú de desbordamiento. Los usuarios no podrán quitarlo.

Si no se configura esta directiva o se deshabilita, los usuarios podrán anclar o quitar el icono mediante su menú contextual.

Si también ha establecido la directiva [EnableMediaRouter](#enablemediarouter) en false, se omitirá esta directiva y no se mostrará el icono de la barra de herramientas.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: No - Requiere reiniciar el explorador

  #### Tipo de datos:
  Booleano

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: ShowCastIconInToolbar
  - Nombre de la directiva de grupos: Mostrar el icono de transmisión en la barra de herramientas
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/Cast
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: ShowCastIconInToolbar
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000000
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: ShowCastIconInToolbar
  - Valor de ejemplo:
``` xml
<false/>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ## Configuración de SmartScreen policies

  [Volver al principio](#microsoft-edge:-directivas)

  ### PreventSmartScreenPromptOverride
  #### Impedir que se pasen por alto de Sm los avisos de SmartScreen de Microsoft Defender para sitios
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  This policy setting lets you decide whether users can override the Microsoft Defender SmartScreen warnings about potentially malicious websites.

If you enable this setting, users can't ignore Microsoft Defender SmartScreen warnings and they are blocked from continuing to the site.

If you disable or don't configure this setting, users can ignore Microsoft Defender SmartScreen warnings and continue to the site.

This policy is available only on Windows instances that are joined to a Microsoft Active Directory domain; or on Windows 10 Pro or Enterprise instances that are enrolled for device management.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Booleano

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: PreventSmartScreenPromptOverride
  - Nombre de la directiva de grupos: Impedir que se pasen por alto de Sm los avisos de SmartScreen de Microsoft Defender para sitios
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/Configuración de SmartScreen
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: PreventSmartScreenPromptOverride
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000001
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: PreventSmartScreenPromptOverride
  - Valor de ejemplo:
``` xml
<true/>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### PreventSmartScreenPromptOverrideForFiles
  #### Impedir que se omitan las advertencias de SmartScreen de Microsoft Defender sobre las descargas
  >Versiones admitidas: Microsoft Edge en Windows desde la versión 77 o posterior y la Mac desde la versión 79 o posterior

  #### Descripción
  This policy lets you determine whether users can override Microsoft Defender SmartScreen warnings about unverified downloads.

If you enable this policy, users in your organization can't ignore Microsoft Defender SmartScreen warnings, and they're prevented from completing the unverified downloads.

If you disable or don't configure this policy, users can ignore Microsoft Defender SmartScreen warnings and complete unverified downloads.

This policy is available only on Windows instances that are joined to a Microsoft Active Directory domain; or on Windows 10 Pro or Enterprise instances that are enrolled for device management.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Booleano

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: PreventSmartScreenPromptOverrideForFiles
  - Nombre de la directiva de grupos: Impedir que se omitan las advertencias de SmartScreen de Microsoft Defender sobre las descargas
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/Configuración de SmartScreen
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: PreventSmartScreenPromptOverrideForFiles
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000001
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: PreventSmartScreenPromptOverrideForFiles
  - Valor de ejemplo:
``` xml
<true/>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### SmartScreenAllowListDomains
  #### Configurar la lista de dominios para los que SmartScreen de Microsoft Defender no desencadenará advertencias
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Configure the list of Microsoft Defender SmartScreen trusted domains. This means:
Microsoft Defender SmartScreen won't check for potentially malicious resources like phishing software and other malware if the source URLs match these domains.
The Microsoft Defender SmartScreen download protection service won't check downloads hosted on these domains.

If you enable this policy, Microsoft Defender SmartScreen trusts these domains.
If you disable or don't set this policy, default Microsoft Defender SmartScreen protection is applied to all resources.

This policy is available only on Windows instances that are joined to a Microsoft Active Directory domain; or on Windows 10 Pro or Enterprise instances that are enrolled for device management.
Also note that this policy does not apply if your organization has enabled Microsoft Defender Advanced Threat Protection. You must configure your allow and block lists in Microsoft Defender Security Center instead.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Lista de cadenas

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: SmartScreenAllowListDomains
  - Nombre de la directiva de grupos: Configurar la lista de dominios para los que SmartScreen de Microsoft Defender no desencadenará advertencias
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/Configuración de SmartScreen
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge\SmartScreenAllowListDomains
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: 1, 2, 3, ...
  - Tipo de valor: lista de REG_SZ
  ##### Valor de ejemplo:
```
SOFTWARE\Policies\Microsoft\Edge\SmartScreenAllowListDomains\0 = "mydomain.com"
SOFTWARE\Policies\Microsoft\Edge\SmartScreenAllowListDomains\1 = "myuniversity.edu"

```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: SmartScreenAllowListDomains
  - Valor de ejemplo:
``` xml
<array>
  <string>mydomain.com</string>
  <string>myuniversity.edu</string>
</array>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### SmartScreenEnabled
  #### Configurar SmartScreen de Microsoft Defender
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Esta configuración de directiva permite configurar si se debe activar SmartScreen de Microsoft Defender. SmartScreen de Microsoft Defender proporciona mensajes de advertencia que ayudan a proteger a los usuarios contra posibles estafas de suplantación de identidad (phishing) y software malintencionado. De manera predeterminada, SmartScreen de Microsoft Defender está activado.

Si se habilita esta configuración, SmartScreen de Microsoft Defender se activará.

Si se deshabilita esta configuración, SmartScreen de Microsoft Defender se desactivará.

Si no se establece esta configuración, los usuarios podrán elegir si usar SmartScreen de Microsoft Defender.

Esta directiva solo está disponible en instancias de Windows que están unidas a un dominio de Microsoft Active Directory o en instancias de Windows 10 Pro o Enterprise que están inscritas para la administración de dispositivos.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: Sí
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Booleano

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: SmartScreenEnabled
  - Nombre de la directiva de grupos: Configurar SmartScreen de Microsoft Defender
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/Configuración de SmartScreen
  - Ruta de acceso de GP (Recomendada): Plantillas administrativas/Microsoft Edge - Configuración predeterminada (los usuarios pueden cambiarla)/Configuración de SmartScreen
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): SOFTWARE\Policies\Microsoft\Edge\Recomendada
  - Nombre del valor: SmartScreenEnabled
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000001
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: SmartScreenEnabled
  - Valor de ejemplo:
``` xml
<true/>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### SmartScreenForTrustedDownloadsEnabled
  #### Forzar las comprobaciones de SmartScreen de Microsoft Defender en las descargas de fuentes de confianza
  >Versiones admitidas: Microsoft Edge en Windows desde la versión 78 o posterior

  #### Descripción
  Esta configuración de directiva le permite configurar si las comprobaciones de SmartScreen de Microsoft Defender descargan la reputación de un origen de confianza.

Si se habilita o no se establece esta configuración, SmartScreen de Microsoft Defender comprueba la reputación de la descarga independientemente del origen.

Si se deshabilita esta configuración, SmartScreen de Microsoft Defender no comprueba la reputación de la descarga al descargar desde un origen de confianza.

Esta directiva solo está disponible en las instancias de Windows que están unidas a un dominio de Microsoft Active Directory o en las instancias de Windows 10 Pro o Enterprise que están inscritas para la administración de dispositivos.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: Sí
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Booleano

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: SmartScreenForTrustedDownloadsEnabled
  - Nombre de la directiva de grupos: Forzar las comprobaciones de SmartScreen de Microsoft Defender en las descargas de fuentes de confianza
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/Configuración de SmartScreen
  - Ruta de acceso de GP (Recomendada): Plantillas administrativas/Microsoft Edge - Configuración predeterminada (los usuarios pueden cambiarla)/Configuración de SmartScreen
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): SOFTWARE\Policies\Microsoft\Edge\Recomendada
  - Nombre del valor: SmartScreenForTrustedDownloadsEnabled
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000000
```


  

  [Volver al principio](#microsoft-edge:-directivas)

  ### SmartScreenPuaEnabled
  #### Configurar SmartScreen de Microsoft Defender para bloquear aplicaciones potencialmente no deseadas
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 80 o posterior

  #### Descripción
  Esta configuración de directiva permite configurar si se debe activar el bloqueo de aplicaciones potencialmente no deseadas en SmartScreen de Microsoft Defender. El bloqueo de aplicaciones potencialmente no deseadas en SmartScreen de Microsoft Defender proporciona mensajes de advertencia que ayudan a proteger a los usuarios contra adware, extractores de moneda, bundleware y otras aplicaciones de baja reputación que se hospedan en sitios web. El bloqueo de aplicaciones potencialmente no deseadas en SmartScreen de Microsoft Defender está desactivado de manera predeterminada.

Si se habilita esta configuración, se activará el bloqueo de aplicaciones potencialmente no deseadas en SmartScreen de Microsoft Defender.

Si se deshabilita esta configuración, se desactivará el bloqueo de aplicaciones potencialmente no deseadas en SmartScreen de Microsoft Defender.

Si no se establece esta configuración, los usuarios podrán elegir si quieren usar el bloqueo de aplicaciones potencialmente no deseadas en SmartScreen de Microsoft Defender.

Esta directiva solo está disponible en las instancias de Windows que están unidas a un dominio de Microsoft Active Directory o en instancias de Windows 10 Pro o Enterprise que están inscritas para la administración de dispositivos.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: Sí
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Booleano

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: SmartScreenPuaEnabled
  - Nombre de la directiva de grupos: Configurar SmartScreen de Microsoft Defender para bloquear aplicaciones potencialmente no deseadas
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/Configuración de SmartScreen
  - Ruta de acceso de GP (Recomendada): Plantillas administrativas/Microsoft Edge - Configuración predeterminada (los usuarios pueden cambiarla)/Configuración de SmartScreen
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): SOFTWARE\Policies\Microsoft\Edge\Recomendada
  - Nombre del valor: SmartScreenPuaEnabled
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000001
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: SmartScreenPuaEnabled
  - Valor de ejemplo:
``` xml
<true/>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ## Configuración de contenido policies

  [Volver al principio](#microsoft-edge:-directivas)

  ### AutoSelectCertificateForUrls
  #### Seleccionar automáticamente certificados de cliente para estos sitios
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Especifique una lista de sitios, según los patrones de dirección URL, para los que Microsoft Edge debe seleccionar automáticamente un certificado de cliente, si el sitio lo solicita.

El valor debe ser una matriz de diccionarios JSON en cadena. La forma de cada diccionario debe ser{ "pattern": "$URL_PATTERN", "filter" : $FILTER }, donde $URL_PATTERN es un patrón de configuración de contenido. $FILTER restringe los certificados de cliente de los que puede seleccionar automáticamente el explorador. Independientemente del filtro, solo se pueden usar los certificados que coinciden con la solicitud de certificado del servidor. Por ejemplo, si $FILTER tiene la forma { "ISSUER": { "CN": "$ISSUER_CN" } }, solo se seleccionarán certificados de cliente emitidos por un certificado con el CommonName $ISSUER_CN. Si $FILTER contiene las secciones "ISSUER" y "SUBJECT", el certificado de cliente debe cumplir las dos condiciones para poder ser seleccionado. Si $FILTER especifica una organización ("O"), el certificado debe tener al menos una organización que coincida con el valor especificado que se va a seleccionar. Si $FILTER especifica una unidad organizativa ("OU"), el certificado debe tener al menos una unidad organizativa que coincida con el valor especificado que se va a seleccionar. Si $FILTER es el diccionario vacío {}, la selección de certificados de cliente no está más restringida.

Si no se configura esta directiva, no se realizará la selección automática en ningún sitio.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Lista de cadenas

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: AutoSelectCertificateForUrls
  - Nombre de la directiva de grupos: Seleccionar automáticamente certificados de cliente para estos sitios
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/Configuración de contenido
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge\AutoSelectCertificateForUrls
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: 1, 2, 3, ...
  - Tipo de valor: lista de REG_SZ
  ##### Valor de ejemplo:
```
SOFTWARE\Policies\Microsoft\Edge\AutoSelectCertificateForUrls\0 = "{"pattern":"https://www.contoso.com","filter":{"ISSUER":{"CN":"certificate issuer name", "L": "certificate issuer location", "O": "certificate issuer org", "OU": "certificate issuer org unit"}, "SUBJECT":{"CN":"certificate subject name", "L": "certificate subject location", "O": "certificate subject org", "OU": "certificate subject org unit"}}}"

```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: AutoSelectCertificateForUrls
  - Valor de ejemplo:
``` xml
<array>
  <string>{"pattern":"https://www.contoso.com","filter":{"ISSUER":{"CN":"certificate issuer name", "L": "certificate issuer location", "O": "certificate issuer org", "OU": "certificate issuer org unit"}, "SUBJECT":{"CN":"certificate subject name", "L": "certificate subject location", "O": "certificate subject org", "OU": "certificate subject org unit"}}}</string>
</array>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### CookiesAllowedForUrls
  #### Permitir cookies en sitios específicos
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Definir una lista de sitios, según los patrones de URL, con autorización para establecer cookies.

Si no se configura esta directiva, se usará el valor predeterminado global de la directiva [DefaultCookiesSetting](#defaultcookiessetting) (si se ha establecido) o de la configuración personal del usuario en todos los sitios.

Consulte las directivas [CookiesBlockedForUrls](#cookiesblockedforurls) y [CookiesSessionOnlyForUrls](#cookiessessiononlyforurls) para obtener más información.

Tenga en cuenta que no puede haber patrones de direcciones URL en conflicto establecidos entre estas tres directivas:

- [CookiesBlockedForUrls](#cookiesblockedforurls)

- CookiesAllowedForUrls

- [CookiesSessionOnlyForUrls](#cookiessessiononlyforurls)

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Lista de cadenas

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: CookiesAllowedForUrls
  - Nombre de la directiva de grupos: Permitir cookies en sitios específicos
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/Configuración de contenido
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge\CookiesAllowedForUrls
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: 1, 2, 3, ...
  - Tipo de valor: lista de REG_SZ
  ##### Valor de ejemplo:
```
SOFTWARE\Policies\Microsoft\Edge\CookiesAllowedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\CookiesAllowedForUrls\1 = "[*.]contoso.edu"

```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: CookiesAllowedForUrls
  - Valor de ejemplo:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### CookiesBlockedForUrls
  #### Bloquear cookies en sitios específicos
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Defina una lista de sitios, según los patrones de URL, sin autorización para establecer cookies.

Si no se configura esta directiva, se usará el valor predeterminado global de la directiva [DefaultCookiesSetting](#defaultcookiessetting) (si se ha establecido) o de la configuración personal del usuario en todos los sitios.

Consulte las directivas [CookiesAllowedForUrls](#cookiesallowedforurls) y [CookiesSessionOnlyForUrls](#cookiessessiononlyforurls) para obtener más información.

Tenga en cuenta que no puede haber patrones de direcciones URL en conflicto establecidos entre estas tres directivas:

- CookiesBlockedForUrls

- [CookiesAllowedForUrls](#cookiesallowedforurls)

- [CookiesSessionOnlyForUrls](#cookiessessiononlyforurls)

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Lista de cadenas

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: CookiesBlockedForUrls
  - Nombre de la directiva de grupos: Bloquear cookies en sitios específicos
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/Configuración de contenido
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge\CookiesBlockedForUrls
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: 1, 2, 3, ...
  - Tipo de valor: lista de REG_SZ
  ##### Valor de ejemplo:
```
SOFTWARE\Policies\Microsoft\Edge\CookiesBlockedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\CookiesBlockedForUrls\1 = "[*.]contoso.edu"

```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: CookiesBlockedForUrls
  - Valor de ejemplo:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### CookiesSessionOnlyForUrls
  #### Limitar las cookies de sitios web específicos a la sesión actual
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Las cookies creadas por sitios web que coinciden con un patrón de dirección URL que se defina se eliminan cuando finaliza la sesión (cuando se cierra la ventana).

Las cookies creadas por sitios web que no coinciden con el patrón están controladas por la directiva [DefaultCookiesSetting](#defaultcookiessetting) (si se ha establecido) o por la configuración personal del usuario. Este también es el comportamiento predeterminado si no configura esta directiva.

Si Microsoft Edge se ejecuta en modo de segundo plano, la sesión podría no cerrarse cuando se cierre la última ventana, lo que significa que las cookies no se borrarán cuando se cierre la ventana. Consulte la directiva [BackgroundModeEnabled](#backgroundmodeenabled) para obtener información sobre cómo configurar lo que sucede cuando Microsoft Edge se ejecuta en modo de segundo plano.

También puede usar las directivas [CookiesAllowedForUrls](#cookiesallowedforurls) y [CookiesBlockedForUrls](#cookiesblockedforurls) para controlar qué sitios web pueden crear cookies.

Tenga en cuenta que no puede haber patrones de direcciones URL en conflicto establecidos entre estas tres directivas:

- [CookiesBlockedForUrls](#cookiesblockedforurls)

- [CookiesAllowedForUrls](#cookiesallowedforurls)

- CookiesSessionOnlyForUrls

Si se establece la directiva [RestoreOnStartup](#restoreonstartup) para restaurar las direcciones URL de sesiones anteriores, esta directiva se ignorará y las cookies se almacenarán permanentemente para esos sitios.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Lista de cadenas

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: CookiesSessionOnlyForUrls
  - Nombre de la directiva de grupos: Limitar las cookies de sitios web específicos a la sesión actual
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/Configuración de contenido
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge\CookiesSessionOnlyForUrls
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: 1, 2, 3, ...
  - Tipo de valor: lista de REG_SZ
  ##### Valor de ejemplo:
```
SOFTWARE\Policies\Microsoft\Edge\CookiesSessionOnlyForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\CookiesSessionOnlyForUrls\1 = "[*.]contoso.edu"

```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: CookiesSessionOnlyForUrls
  - Valor de ejemplo:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### DefaultCookiesSetting
  #### Configurar cookies
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Controle si los sitios web pueden crear cookies en el dispositivo del usuario. Esta directiva es una cuestión de todo o nada: puede permitir que todos los sitios web creen cookies o que no ningún sitio web cree cookies. No puede usarse esta directiva para habilitar las cookies de sitios web específicos.

Establezca la directiva en 'SessionOnly' (4) para borrar las cookies cuando se cierre la sesión. Si Microsoft Edge se está ejecutando en modo de segundo plano, es posible que la sesión no se cierre al cerrar la última ventana, lo que significa que las cookies no se borrarán cuando se cierre la ventana. Consulte la directiva [BackgroundModeEnabled](#backgroundmodeenabled) para obtener información acerca de cómo configurar lo que ocurre cuando Microsoft Edge se ejecuta en modo en segundo plano.

Si no se configura esta directiva, se usará el valor predeterminado 'AllowCookies' (1) y los usuarios podrán cambiar este ajuste en la configuración de Microsoft Edge. (Si no quiere que los usuarios puedan cambiar esta configuración, establezca la directiva.)

* 1 = Permitir que todos los sitios creen cookies

* 2 = No permitir que ningún sitio cree cookies

* 4 = Mantener cookies durante la sesión

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Entero

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: DefaultCookiesSetting
  - Nombre de la directiva de grupos: Configurar cookies
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/Configuración de contenido
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: DefaultCookiesSetting
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000001
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: DefaultCookiesSetting
  - Valor de ejemplo:
``` xml
<integer>1</integer>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### DefaultGeolocationSetting
  #### Configuración de geolocalización predeterminada
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Establecer si los sitios web pueden realizar un seguimiento de la ubicación física de los usuarios. Se puede permitir el seguimiento de manera predeterminada (1), denegarlo de manera predeterminada (2) o preguntarle al usuario cada vez que un sitio web solicite su ubicación (3).

Si no se configura esta directiva, se usa la directiva 'AskGeolocation' y el usuario puede cambiarla.

* 1 = Permitir que los sitios realicen un seguimiento de la ubicación física de los usuarios

* 2 = No permitir que ningún sitio realice un seguimiento de la ubicación física de los usuarios

* 3 = Preguntar siempre que un sitio quiera realizar un seguimiento de la ubicación física de los usuarios

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Entero

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: DefaultGeolocationSetting
  - Nombre de la directiva de grupos: Configuración de geolocalización predeterminada
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/Configuración de contenido
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: DefaultGeolocationSetting
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000001
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: DefaultGeolocationSetting
  - Valor de ejemplo:
``` xml
<integer>1</integer>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### DefaultImagesSetting
  #### Configuración predeterminada de imágenes
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Establecer si los sitios web pueden mostrar imágenes. Se pueden permitir imágenes en todos los sitios (1) o bloquearlos en todos los sitios (2).

Si no se configura esta directiva, se permiten imágenes de manera predeterminada y el usuario puede cambiar esta configuración.

* 1 = Permitir que todos los sitios muestren todas las imágenes

* 2 = No permitir que ningún sitio muestre imágenes

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Entero

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: DefaultImagesSetting
  - Nombre de la directiva de grupos: Configuración predeterminada de imágenes
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/Configuración de contenido
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: DefaultImagesSetting
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000001
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: DefaultImagesSetting
  - Valor de ejemplo:
``` xml
<integer>1</integer>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### DefaultJavaScriptSetting
  #### Configuración predeterminada de JavaScript
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Establecer si los sitios web pueden ejecutar JavaScript. Puede permitirse para todos los sitios (1) o bloquearse para todos los sitios (2).

Si no se configura esta directiva, todos los sitios pueden ejecutar JavaScript de manera predeterminada y el usuario puede cambiar esta configuración.

* 1 = Permitir que todos los sitios ejecuten JavaScript

* 2 = No permitir que ningún sitio ejecute JavaScript

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Entero

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: DefaultJavaScriptSetting
  - Nombre de la directiva de grupos: Configuración predeterminada de JavaScript
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/Configuración de contenido
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: DefaultJavaScriptSetting
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000001
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: DefaultJavaScriptSetting
  - Valor de ejemplo:
``` xml
<integer>1</integer>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### DefaultNotificationsSetting
  #### Configuración de notificaciones predeterminada
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Establecer si los sitios web pueden mostrar notificaciones de escritorio. Puede permitirlos de manera predeterminada (1), denegarlos de manera predeterminada (2) o preguntarle al usuario cada vez que un sitio web quiera mostrar una notificación (3).

Si no se configura esta directiva, se permitirán las notificaciones de manera predeterminada y el usuario podrá cambiar esta configuración.

* 1 = Permitir que los sitios muestren notificaciones de escritorio

* 2 = No permitir que ningún sitio muestre notificaciones de escritorio

* 3 = Preguntar cada vez que un sitio quiera mostrar notificaciones de escritorio

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Entero

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: DefaultNotificationsSetting
  - Nombre de la directiva de grupos: Configuración de notificaciones predeterminada
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/Configuración de contenido
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: DefaultNotificationsSetting
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000002
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: DefaultNotificationsSetting
  - Valor de ejemplo:
``` xml
<integer>2</integer>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### DefaultPluginsSetting
  #### Configuración de Adobe Flash predeterminada
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Determina si los sitios web que no están cubiertos por las directivas [PluginsAllowedForUrls](#pluginsallowedforurls) o [PluginsBlockedForUrls](#pluginsblockedforurls) pueden ejecutar automáticamente el complemento Adobe Flash. Se puede seleccionar 'BlockPlugins' (2) para bloquear Adobe Flash en todos los sitios o se puede seleccionar 'ClickToPlay' (3) para permitir que Adobe Flash se ejecute, pero esto requiere que el usuario haga clic en el marcador de posición para iniciarlo. En cualquier caso, las directivas [PluginsAllowedForUrls](#pluginsallowedforurls) y [PluginsBlockedForUrls](#pluginsblockedforurls) tienen prioridad sobre DefaultPluginsSetting'.

Solo se permite la reproducción automática para dominios que aparecen explícitamente en la directiva [PluginsAllowedForUrls](#pluginsallowedforurls). Si quiere habilitar la reproducción automática en todos los sitios, considere la posibilidad de agregar http://* y https://* a esta lista.

Si no se configura esta directiva, el usuario puede cambiar esta configuración manualmente.

* 2 = Bloquear el complemento Adobe Flash

* 3 = Hacer clic para reproducir

La primera opción "1" establece el valor "permitir todo", pero esta funcionalidad solo se controla ahora mediante la directiva [PluginsAllowedForUrls](#pluginsallowedforurls). Las directivas existentes con '1' funcionarán en modo Hacer clic para reproducir.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Entero

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: DefaultPluginsSetting
  - Nombre de la directiva de grupos: Configuración de Adobe Flash predeterminada
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/Configuración de contenido
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: DefaultPluginsSetting
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000002
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: DefaultPluginsSetting
  - Valor de ejemplo:
``` xml
<integer>2</integer>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### DefaultPopupsSetting
  #### Configuración de ventana emergente predeterminada
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Establece si los sitios web pueden mostrar ventanas emergentes. Pueden permitirse en todos los sitios web (1) o bloquearse en todos los sitios (2)

Si no se configura esta directiva, las ventanas emergentes se bloquearán de manera predeterminada y los usuarios podrán cambiar esta configuración.

* 1 = Permitir que todos los sitios muestren elementos emergentes

* 2 = No permitir que ningún sitio muestre ventanas emergentes

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Entero

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: DefaultPopupsSetting
  - Nombre de la directiva de grupos: Configuración de ventana emergente predeterminada
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/Configuración de contenido
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: DefaultPopupsSetting
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000001
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: DefaultPopupsSetting
  - Valor de ejemplo:
``` xml
<integer>1</integer>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### DefaultWebBluetoothGuardSetting
  #### Controlar el uso de la API Web Bluetooth
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Controle si los sitios web pueden acceder a dispositivos Bluetooth cercanos. Puede bloquear completamente el acceso o requerir que el sitio pregunte al usuario cada vez que quiera obtener acceso a un dispositivo Bluetooth.

Si no configura esta directiva, se usará el valor predeterminado (3, lo que significa que se le pregunta a los usuarios cada vez) y los usuarios podrán cambiarlo.

* 2 = No permitir que ningún sitio solicite acceso a dispositivos Bluetooth mediante la API Web Bluetooth

* 3 = Permitir a los sitios solicitar al usuario que conceda acceso a un dispositivo Bluetooth cercano

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Entero

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: DefaultWebBluetoothGuardSetting
  - Nombre de la directiva de grupos: Controlar el uso de la API Web Bluetooth
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/Configuración de contenido
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: DefaultWebBluetoothGuardSetting
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000002
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: DefaultWebBluetoothGuardSetting
  - Valor de ejemplo:
``` xml
<integer>2</integer>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### DefaultWebUsbGuardSetting
  #### Controlar el uso de la API WebUSB
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Establece si los sitios web pueden tener acceso a dispositivos USB conectados. Puede bloquear completamente el acceso o preguntar al usuario cada vez que un sitio web quiera obtener acceso a dispositivos USB conectados.

Puede invalidar esta directiva para patrones de dirección URL específicos mediante las directivas [WebUsbAskForUrls](#webusbaskforurls) y [WebUsbBlockedForUrls](#webusbblockedforurls) .

Si no configura esta directiva, los sitios pueden preguntar a los usuarios si pueden obtener acceso a los dispositivos USB conectados (3) de manera predeterminada y los usuarios pueden cambiar esta configuración.

* 2 = No permitir que ningún sitio solicite acceso a dispositivos USB a través de la API WebUSB

* 3 = Permitir que los sitios soliciten al usuario que conceda acceso a un dispositivo USB conectado

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Entero

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: DefaultWebUsbGuardSetting
  - Nombre de la directiva de grupos: Controlar el uso de la API WebUSB
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/Configuración de contenido
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: DefaultWebUsbGuardSetting
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000002
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: DefaultWebUsbGuardSetting
  - Valor de ejemplo:
``` xml
<integer>2</integer>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### ImagesAllowedForUrls
  #### Permitir imágenes en estos sitios
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Definir una lista de sitios, según los patrones de URL, que puedan mostrar imágenes.

Si no se configura esta directiva, se usará el valor predeterminado global en todos los sitios, ya sea de la directiva [DefaultImagesSetting](#defaultimagessetting) (si se ha establecido) o de la configuración personal del usuario.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Lista de cadenas

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: ImagesAllowedForUrls
  - Nombre de la directiva de grupos: Permitir imágenes en estos sitios
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/Configuración de contenido
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge\ImagesAllowedForUrls
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: 1, 2, 3, ...
  - Tipo de valor: lista de REG_SZ
  ##### Valor de ejemplo:
```
SOFTWARE\Policies\Microsoft\Edge\ImagesAllowedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\ImagesAllowedForUrls\1 = "[*.]contoso.edu"

```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: ImagesAllowedForUrls
  - Valor de ejemplo:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### ImagesBlockedForUrls
  #### Bloquear imágenes en sitios específicos
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Definir una lista de sitios, según los patrones de URL, que no puedan mostrar imágenes.

Si no se configura esta directiva, se usará el valor predeterminado global de la directiva [DefaultImagesSetting](#defaultimagessetting) (si se ha establecido) o de la configuración personal del usuario en todos los sitios.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Lista de cadenas

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: ImagesBlockedForUrls
  - Nombre de la directiva de grupos: Bloquear imágenes en sitios específicos
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/Configuración de contenido
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge\ImagesBlockedForUrls
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: 1, 2, 3, ...
  - Tipo de valor: lista de REG_SZ
  ##### Valor de ejemplo:
```
SOFTWARE\Policies\Microsoft\Edge\ImagesBlockedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\ImagesBlockedForUrls\1 = "[*.]contoso.edu"

```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: ImagesBlockedForUrls
  - Valor de ejemplo:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### JavaScriptAllowedForUrls
  #### Permitir JavaScript en sitios específicos
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Defina una lista de sitios, según los patrones de URL, que tienen permiso para ejecutar JavaScript.

Si no se configura esta directiva, se usará el valor predeterminado global de la directiva [DefaultJavaScriptSetting](#defaultjavascriptsetting) (si se ha establecido) o de la configuración personal del usuario en todos los sitios.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Lista de cadenas

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: JavaScriptAllowedForUrls
  - Nombre de la directiva de grupos: Permitir JavaScript en sitios específicos
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/Configuración de contenido
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge\JavaScriptAllowedForUrls
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: 1, 2, 3, ...
  - Tipo de valor: lista de REG_SZ
  ##### Valor de ejemplo:
```
SOFTWARE\Policies\Microsoft\Edge\JavaScriptAllowedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\JavaScriptAllowedForUrls\1 = "[*.]contoso.edu"

```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: JavaScriptAllowedForUrls
  - Valor de ejemplo:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### JavaScriptBlockedForUrls
  #### Bloquear JavaScript en sitios específicos
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Defina una lista de sitios, según los patrones de URL, que no tienen permiso para ejecutar JavaScript.

Si no se configura esta directiva, se usará el valor predeterminado global de la directiva [DefaultJavaScriptSetting](#defaultjavascriptsetting) (si se ha establecido) o de la configuración personal del usuario en todos los sitios.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Lista de cadenas

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: JavaScriptBlockedForUrls
  - Nombre de la directiva de grupos: Bloquear JavaScript en sitios específicos
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/Configuración de contenido
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge\JavaScriptBlockedForUrls
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: 1, 2, 3, ...
  - Tipo de valor: lista de REG_SZ
  ##### Valor de ejemplo:
```
SOFTWARE\Policies\Microsoft\Edge\JavaScriptBlockedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\JavaScriptBlockedForUrls\1 = "[*.]contoso.edu"

```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: JavaScriptBlockedForUrls
  - Valor de ejemplo:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### LegacySameSiteCookieBehaviorEnabled
  #### Habilitar la configuración del comportamiento de cookies de SameSite heredadas predefinido
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 80 o posterior

  #### Descripción
  Permite revertir todas las cookies al comportamiento de SameSite heredado. La reversión a un comportamiento heredado hace que las cookies que no especifique un atributo de SameSite se traten como si fueran "SameSite=None" y quita el requisito para que las cookies de "SameSite=None" lleven el atributo "Secure".

Puede establecer los siguientes valores para esta directiva:

* 1 = Revertir al comportamiento de SameSite heredado para cookies en todos los sitios

* 2 = Usar el comportamiento de SameSite-by-default para cookies en todos los sitios

Si no se establece esta directiva, el comportamiento predeterminado de las cookies que no especifiquen un atributo de SameSite dependerá de otros orígenes de configuración para la característica SameSite-by-default. Esta característica puede establecerse mediante una prueba de campo o habilitando la marca same-site-by-default-cookies en edge://flags.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Entero

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: LegacySameSiteCookieBehaviorEnabled
  - Nombre de la directiva de grupos: Habilitar la configuración del comportamiento de cookies de SameSite heredadas predefinido
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/Configuración de contenido
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: LegacySameSiteCookieBehaviorEnabled
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000001
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: LegacySameSiteCookieBehaviorEnabled
  - Valor de ejemplo:
``` xml
<integer>1</integer>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### LegacySameSiteCookieBehaviorEnabledForDomainList
  #### Revertir al comportamiento de SameSite heredado para cookies en sitios especificados
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 80 o posterior

  #### Descripción
  Las cookies establecidas para dominios que coincidan con los patrones especificados revertirán al comportamiento de SameSite heredado.

La reversión a un comportamiento heredado hace que las cookies que no especifiquen un atributo de SameSite se traten como si fueran "SameSite=None" y quita el requisito para que las cookies de "SameSite=None" lleven el atributo "Secure".

Si no se establece esta directiva, se usará el valor predeterminado global. El valor predeterminado global también se usará para las cookies en los dominios que no están cubiertos por los patrones que se especifiquen.

El valor predeterminado global puede configurarse mediante la directiva [LegacySameSiteCookieBehaviorEnabled](#legacysamesitecookiebehaviorenabled). Si [LegacySameSiteCookieBehaviorEnabled](#legacysamesitecookiebehaviorenabled) no está establecido, el valor predeterminado global se revertirá a otros orígenes de configuración.

Tenga en cuenta que los patrones que indique en esta directiva se tratarán como dominios, no como direcciones URL, por lo que no debe especificar un esquema o puerto.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Lista de cadenas

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: LegacySameSiteCookieBehaviorEnabledForDomainList
  - Nombre de la directiva de grupos: Revertir al comportamiento de SameSite heredado para cookies en sitios especificados
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/Configuración de contenido
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge\LegacySameSiteCookieBehaviorEnabledForDomainList
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: 1, 2, 3, ...
  - Tipo de valor: lista de REG_SZ
  ##### Valor de ejemplo:
```
SOFTWARE\Policies\Microsoft\Edge\LegacySameSiteCookieBehaviorEnabledForDomainList\0 = "www.example.com"
SOFTWARE\Policies\Microsoft\Edge\LegacySameSiteCookieBehaviorEnabledForDomainList\1 = "[*.]example.edu"

```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: LegacySameSiteCookieBehaviorEnabledForDomainList
  - Valor de ejemplo:
``` xml
<array>
  <string>www.example.com</string>
  <string>[*.]example.edu</string>
</array>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### NotificationsAllowedForUrls
  #### Permitir notificaciones en sitios específicos
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Defina una lista de sitios, según los patrones de URL, que puedan mostrar notificaciones.

Si no configura esta directiva, se usará el valor predeterminado global de la directiva [DefaultNotificationsSetting](#defaultnotificationssetting) (si se ha establecido) o de la configuración personal del usuario en todos los sitios.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Lista de cadenas

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: NotificationsAllowedForUrls
  - Nombre de la directiva de grupos: Permitir notificaciones en sitios específicos
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/Configuración de contenido
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge\NotificationsAllowedForUrls
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: 1, 2, 3, ...
  - Tipo de valor: lista de REG_SZ
  ##### Valor de ejemplo:
```
SOFTWARE\Policies\Microsoft\Edge\NotificationsAllowedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\NotificationsAllowedForUrls\1 = "[*.]contoso.edu"

```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: NotificationsAllowedForUrls
  - Valor de ejemplo:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### NotificationsBlockedForUrls
  #### Bloquear notificaciones en sitios específicos
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Defina una lista de sitios, según los patrones de URL , que no pueden mostrar notificaciones.n
Si no se configura esta directiva, se usará el valor predeterminado global de la directiva the [DefaultNotificationsSetting](#defaultnotificationssetting) (si se ha establecido) o de la configuración personal del usuario en todos los sitios.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Lista de cadenas

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: NotificationsBlockedForUrls
  - Nombre de la directiva de grupos: Bloquear notificaciones en sitios específicos
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/Configuración de contenido
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge\NotificationsBlockedForUrls
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: 1, 2, 3, ...
  - Tipo de valor: lista de REG_SZ
  ##### Valor de ejemplo:
```
SOFTWARE\Policies\Microsoft\Edge\NotificationsBlockedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\NotificationsBlockedForUrls\1 = "[*.]contoso.edu"

```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: NotificationsBlockedForUrls
  - Valor de ejemplo:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### PluginsAllowedForUrls
  #### Permitir el complemento de Adobe Flash en sitios específicos
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Definir una lista de sitios, según los patrones de URL, que puedan ejecutar el complemento de Adobe Flash.

Si no se configura esta directiva, se usará el valor predeterminado global de la directiva [DefaultPluginsSetting](#defaultpluginssetting) (si se ha establecido) o de la configuración personal del usuario en todos los sitios.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Lista de cadenas

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: PluginsAllowedForUrls
  - Nombre de la directiva de grupos: Permitir el complemento de Adobe Flash en sitios específicos
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/Configuración de contenido
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge\PluginsAllowedForUrls
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: 1, 2, 3, ...
  - Tipo de valor: lista de REG_SZ
  ##### Valor de ejemplo:
```
SOFTWARE\Policies\Microsoft\Edge\PluginsAllowedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\PluginsAllowedForUrls\1 = "[*.]contoso.edu"

```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: PluginsAllowedForUrls
  - Valor de ejemplo:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### PluginsBlockedForUrls
  #### Bloquear el complemento de Adobe Flash en sitios específicos
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Defina una lista de sitios, basados en patrones de URL, que no pueden ejecutar Adobe Flash.

Si no se configura esta directiva, se usará el valor predeterminado global de la directiva [DefaultPluginsSetting](#defaultpluginssetting) (si se ha establecido) o de la configuración personal del usuario en todos los sitios.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Lista de cadenas

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: PluginsBlockedForUrls
  - Nombre de la directiva de grupos: Bloquear el complemento de Adobe Flash en sitios específicos
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/Configuración de contenido
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge\PluginsBlockedForUrls
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: 1, 2, 3, ...
  - Tipo de valor: lista de REG_SZ
  ##### Valor de ejemplo:
```
SOFTWARE\Policies\Microsoft\Edge\PluginsBlockedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\PluginsBlockedForUrls\1 = "[*.]contoso.edu"

```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: PluginsBlockedForUrls
  - Valor de ejemplo:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### PopupsAllowedForUrls
  #### Permitir ventanas emergentes en sitios específicos
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Definir una lista de sitios, según los patrones de URL, que puedan abrir ventanas emergentes.

Si no se configura esta directiva, se usará el valor predeterminado global de la directiva [DefaultPopupsSetting](#defaultpopupssetting) (si se ha establecido) o de la configuración personal del usuario en todos los sitios.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Lista de cadenas

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: PopupsAllowedForUrls
  - Nombre de la directiva de grupos: Permitir ventanas emergentes en sitios específicos
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/Configuración de contenido
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge\PopupsAllowedForUrls
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: 1, 2, 3, ...
  - Tipo de valor: lista de REG_SZ
  ##### Valor de ejemplo:
```
SOFTWARE\Policies\Microsoft\Edge\PopupsAllowedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\PopupsAllowedForUrls\1 = "[*.]contoso.edu"

```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: PopupsAllowedForUrls
  - Valor de ejemplo:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### PopupsBlockedForUrls
  #### Bloquear ventanas emergentes en sitios específicos
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Defina una lista de sitios, según los patrones de URL, que estén bloqueados y no puedan abrir ventanas emergentes.

Si no se configura esta directiva, se usará el valor predeterminado global de la directiva [DefaultPopupsSetting](#defaultpopupssetting) (si se ha establecido) o de la configuración personal del usuario en todos los sitios.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Lista de cadenas

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: PopupsBlockedForUrls
  - Nombre de la directiva de grupos: Bloquear ventanas emergentes en sitios específicos
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/Configuración de contenido
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge\PopupsBlockedForUrls
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: 1, 2, 3, ...
  - Tipo de valor: lista de REG_SZ
  ##### Valor de ejemplo:
```
SOFTWARE\Policies\Microsoft\Edge\PopupsBlockedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\PopupsBlockedForUrls\1 = "[*.]contoso.edu"

```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: PopupsBlockedForUrls
  - Valor de ejemplo:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### RegisteredProtocolHandlers
  #### Registrar controladores de protocolo
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Registra una lista de controladores de protocolo. Establece la propiedad de protocolo en el esquema (por ejemplo, 'mailto)' y la propiedad de dirección URL en el patrón de dirección URL de la aplicación que controla el esquema. El patrón puede incluir un '%s', que se sustituirá por la dirección URL controlada.

Puedes recomendar un valor específico para esta directiva, pero no puedes exigir que los usuarios lo usen.

Los controladores de protocolo registrados por la directiva se combinan con los controladores registrados por el usuario, y ambos están disponibles para usar. El usuario puede invalidar los controladores de protocolo instalados por la directiva mediante la instalación de un nuevo controlador predeterminado, pero no puede quitar un controlador de protocolo registrado por la directiva.

  #### Características admitidas:
  - Puede ser obligatorio: No
  - Se puede recomendar: Sí
  - Actualización de directiva dinámica: No - Requiere reiniciar el explorador

  #### Tipo de datos:
  Diccionario

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: RegisteredProtocolHandlers
  - Nombre de la directiva de grupos: Registrar controladores de protocolo
  - Ruta de acceso de GP (Obligatorio): N/D
  - Ruta de acceso de GP (Recomendada): Plantillas administrativas/Microsoft Edge - Configuración predeterminada (los usuarios pueden cambiarla)/Configuración de contenido
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): N/D
  - Ruta de acceso (Recomendada): SOFTWARE\Policies\Microsoft\Edge\Recomendada
  - Nombre del valor: RegisteredProtocolHandlers
  - Tipo de valor: REG_SZ
  ##### Valor de ejemplo:
```
SOFTWARE\Policies\Microsoft\Edge\RegisteredProtocolHandlers = [
  {
    "default": true, 
    "protocol": "mailto", 
    "url": "https://mail.contoso.com/mail/?extsrc=mailto&url=%s"
  }
]
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: RegisteredProtocolHandlers
  - Valor de ejemplo:
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
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### WebUsbAllowDevicesForUrls
  #### Conceder acceso a sitios específicos para conectarse a dispositivos USB específicos
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Permite establecer una lista de direcciones URL que especifican los sitios a los que se concederá automáticamente permiso de acceso a un dispositivo USB con los id. del producto especificados. Cada elemento de la lista debe contener tanto dispositivos como direcciones URL para que la directiva sea válida. Cada elemento de los dispositivos puede contener un campo de id. de proveedor y id. del producto. Cualquier identificador que se omita se tratará como un comodín con una excepción y esa excepción es que no se puede especificar un id. del producto sin que también se especifique un id. de proveedor. De lo contrario, la directiva no será válida y se omitirá.

El modelo de permisos de USB usa la dirección URL del sitio que hace la solicitud ("URL de solicitud") y la dirección URL del sitio de marco de nivel superior ("URL de inserción") para conceder permiso de acceso a la dirección URL solicitante al dispositivo USB. La dirección URL solicitante puede ser distinta de la URL de inserción cuando el sitio solicitante se carga en un IFrame. Por este motivo, el campo "direcciones URL" puede contener dos cadenas URL, delimitadas por una coma, para especificar la dirección URL de solicitud e incrustación respectivamente. Si solo se especifica una dirección URL, se concederá el acceso a los dispositivos USB correspondientes cuando la dirección URL del sitio solicitante coincide con esta dirección URL, independientemente del estado de la incrustación. Por lo tanto, el campo "urls" puede contener hasta dos cadenas de direcciones URL delimitadas por una coma para especificar la dirección URL de solicitud e incrustación, respectivamente. Si solo se especifica una dirección URL, se concederá acceso a los dispositivos USB correspondientes cuando la dirección URL del sitio solicitante coincida con esta dirección URL, independientemente del estado de la incrustación. Las direcciones URL en "urls" deben ser direcciones URL válidas; de lo contrario, se omitirá la directiva.

Si no se establece esta directiva, se usará el valor predeterminado global para todos los sitios de la directiva [DefaultWebUsbGuardSetting](#defaultwebusbguardsetting), si está establecida, o de la configuración personal del usuario si no lo está.

Los modelos de dirección URL de esta directiva no deben entrar en conflicto con los configurados a través de [WebUsbBlockedForUrls](#webusbblockedforurls). Si hay un conflicto, esta directiva tendrá prioridad sobre [WebUsbBlockedForUrls](#webusbblockedforurls) y [WebUsbAskForUrls](#webusbaskforurls).

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Diccionario

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: WebUsbAllowDevicesForUrls
  - Nombre de la directiva de grupos: Conceder acceso a sitios específicos para conectarse a dispositivos USB específicos
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/Configuración de contenido
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: WebUsbAllowDevicesForUrls
  - Tipo de valor: REG_SZ
  ##### Valor de ejemplo:
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


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: WebUsbAllowDevicesForUrls
  - Valor de ejemplo:
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
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### WebUsbAskForUrls
  #### Permitir WebUSB en sitios específicos
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Defina una lista de sitios, según los patrones de URL, que puedan solicitar al usuario acceso a un dispositivo USB.

Si no se configura esta directiva, se usará el valor predeterminado global de la directiva [DefaultWebUsbGuardSetting](#defaultwebusbguardsetting) (si se ha establecido) o de la configuración personal del usuario en todos los sitios.

Los patrones de URL definidos en esta directiva no pueden entrar en conflicto con los configurados en la directiva [WebUsbBlockedForUrls](#webusbblockedforurls); no puede permitir y bloquear una URL.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Lista de cadenas

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: WebUsbAskForUrls
  - Nombre de la directiva de grupos: Permitir WebUSB en sitios específicos
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/Configuración de contenido
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge\WebUsbAskForUrls
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: 1, 2, 3, ...
  - Tipo de valor: lista de REG_SZ
  ##### Valor de ejemplo:
```
SOFTWARE\Policies\Microsoft\Edge\WebUsbAskForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\WebUsbAskForUrls\1 = "[*.]contoso.edu"

```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: WebUsbAskForUrls
  - Valor de ejemplo:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### WebUsbBlockedForUrls
  #### Bloquear WebUSB en sitios específicos
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Defina una lista de sitios, según los patrones de URL, que no puedan solicitar al usuario que les conceda acceso a un dispositivo USB.

Si no se configura esta directiva, se usará el valor predeterminado global de la directiva [DefaultWebUsbGuardSetting](#defaultwebusbguardsetting) (si se ha establecido) o de la configuración personal del usuario en todos los sitios.

Los patrones de URL definidos en esta directiva no pueden entrar en conflicto con los configurados en la directiva [WebUsbAskForUrls](#webusbaskforurls). No puede permitir y bloquear una URL al mismo tiempo.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Lista de cadenas

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: WebUsbBlockedForUrls
  - Nombre de la directiva de grupos: Bloquear WebUSB en sitios específicos
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/Configuración de contenido
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge\WebUsbBlockedForUrls
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: 1, 2, 3, ...
  - Tipo de valor: lista de REG_SZ
  ##### Valor de ejemplo:
```
SOFTWARE\Policies\Microsoft\Edge\WebUsbBlockedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\WebUsbBlockedForUrls\1 = "[*.]contoso.edu"

```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: WebUsbBlockedForUrls
  - Valor de ejemplo:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ## Extensiones policies

  [Volver al principio](#microsoft-edge:-directivas)

  ### ExtensionAllowedTypes
  #### Configurar tipos de extensiones permitidos
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Controla los tipos de extensión que se pueden instalar y limita el acceso en tiempo de ejecución.

Esta configuración define los tipos permitidos de extensiones y los hosts con los que pueden interactuar. El valor es una lista de cadenas, cada una de las cuales debe ser uno de los siguientes valores: "extensión", "theme", "user_script" y "hosted_app". Consulte la documentación de extensiones de Microsoft Edge para obtener más información sobre estos tipos.

Tenga en cuenta que esta directiva también afecta a que se fuerce la instalación de las extensiones mediante la directiva [ExtensionInstallForcelist](#extensioninstallforcelist).

Si se habilita esta directiva, se instalan solo las extensiones que coinciden con un tipo en la lista.

Si no se configura esta directiva, no se aplicarán restricciones en los tipos de extensión aceptables.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Lista de cadenas

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: ExtensionAllowedTypes
  - Nombre de la directiva de grupos: Configurar tipos de extensiones permitidos
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/Extensiones
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge\ExtensionAllowedTypes
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: 1, 2, 3, ...
  - Tipo de valor: lista de REG_SZ
  ##### Valor de ejemplo:
```
SOFTWARE\Policies\Microsoft\Edge\ExtensionAllowedTypes\0 = "hosted_app"

```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: ExtensionAllowedTypes
  - Valor de ejemplo:
``` xml
<array>
  <string>hosted_app</string>
</array>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### ExtensionInstallAllowlist
  #### Permitir la instalación de extensiones específicas
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  De manera predeterminada, se permiten todas las extensiones. Sin embargo, si bloquea todas las extensiones al establecer la directiva 'ExtensionInstallBlockList' en "*", los usuarios solo podrán instalar las extensiones definidas en esta directiva.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Lista de cadenas

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: ExtensionInstallAllowlist
  - Nombre de la directiva de grupos: Permitir la instalación de extensiones específicas
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/Extensiones
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallAllowlist
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: 1, 2, 3, ...
  - Tipo de valor: lista de REG_SZ
  ##### Valor de ejemplo:
```
SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallAllowlist\0 = "extension_id1"
SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallAllowlist\1 = "extension_id2"

```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: ExtensionInstallAllowlist
  - Valor de ejemplo:
``` xml
<array>
  <string>extension_id1</string>
  <string>extension_id2</string>
</array>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### ExtensionInstallBlocklist
  #### Controlar las extensiones que no se pueden instalar
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Lista de extensiones específicas que los usuarios NO pueden instalar en Microsoft Edge. Al implementar esta directiva, se deshabilitarán las extensiones de esta lista que se instalaron anteriormente y el usuario no podrá activarlos. Si se quita un elemento de la lista de extensiones bloqueadas, esta extensión se volverá a activar automáticamente en cualquier lugar en el que se instaló anteriormente.

Use "*" para bloquear todas las extensiones que no aparecen explícitamente en la lista de permitidos.

Si no se configura esta directiva, los usuarios pueden instalar cualquier extensión en Microsoft Edge.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Lista de cadenas

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: ExtensionInstallBlocklist
  - Nombre de la directiva de grupos: Controlar las extensiones que no se pueden instalar
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/Extensiones
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallBlocklist
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: 1, 2, 3, ...
  - Tipo de valor: lista de REG_SZ
  ##### Valor de ejemplo:
```
SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallBlocklist\0 = "extension_id1"
SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallBlocklist\1 = "extension_id2"

```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: ExtensionInstallBlocklist
  - Valor de ejemplo:
``` xml
<array>
  <string>extension_id1</string>
  <string>extension_id2</string>
</array>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### ExtensionInstallForcelist
  #### Controlar las extensiones que se instalan en modo silencioso
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Especifica extensiones que se instalan silenciosamente, sin interacción del usuario y que los usuarios no pueden desinstalar ni deshabilitar ("forzar instalación"). Todos los permisos solicitados por las extensiones se conceden de forma implícita, sin la interacción del usuario, incluidos los permisos adicionales solicitados por las versiones futuras de la extensión. Además, se conceden permisos para las API de las extensiones enterprise.deviceAttributes y enterprise.platformKeys. (Estas dos API solo están disponibles para extensiones que están instaladas a la fuerza.)

Esta directiva tiene prioridad sobre una directiva [ExtensionInstallBlocklist](#extensioninstallblocklist) potencialmente conflictiva. Cuando quita una extensión de la lista de instalaciones a la fuerza, Microsoft Edge la desinstalará automáticamente.

Para dispositivos Windows que no están unidos a un dominio de Microsoft Active Directory, la instalación a la fuerza está limitada a las extensiones disponibles en Microsoft Store.

Tenga en cuenta que los usuarios pueden modificar el código fuente de cualquier extensión mediante Herramientas de desarrollo, lo que podría representar la extensión como disfuncional. Si esto es un problema, establezca la directiva [DeveloperToolsAvailability](#developertoolsavailability).

Use el siguiente formato para agregar una extensión a la lista:

[extensionID];[updateURL]

- extensionID - la cadena de 32 letras que se encuentra en edge://extensions en el modo de desarrollador.

- updateURL (opcional) es la dirección del documento XML del manifiesto de actualización para la aplicación o extensión, como se describe en [https://go.microsoft.com/fwlink/?linkid=2095043](https://go.microsoft.com/fwlink/?linkid=2095043). Si no se establece la updateURL, se usará la dirección URL de actualización de Microsoft Store (actualmente https://edge.microsoft.com/extensionwebstorebase/v1/crx). Tenga en cuenta que la dirección URL de actualización establecida en esta directiva solo se usa para la instalación inicial; las actualizaciones subsiguientes de la extensión usan la dirección URL de actualización indicada en el manifiesto de la extensión.

Por ejemplo, gggmmkjegpiggikcnhidnjjhmicpibll;https://edge.microsoft.com/extensionwebstorebase/v1/crx instala la aplicación Microsoft Online desde la dirección URL de "actualización" de Microsoft Store. Para obtener más información acerca de las extensiones de hospedaje, consulte: [https://go.microsoft.com/fwlink/?linkid=2095044](https://go.microsoft.com/fwlink/?linkid=2095044).

Si no se configura esta directiva, no se instalarán automáticamente las extensiones y los usuarios podrán desinstalar cualquier extensión en Microsoft Edge.

Tenga en cuenta que esta directiva no se aplica al modo de InPrivate.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Lista de cadenas

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: ExtensionInstallForcelist
  - Nombre de la directiva de grupos: Controlar las extensiones que se instalan en modo silencioso
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/Extensiones
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallForcelist
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: 1, 2, 3, ...
  - Tipo de valor: lista de REG_SZ
  ##### Valor de ejemplo:
```
SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallForcelist\0 = "gbchcmhmhahfdphkhkmpfmihenigjmpp;https://edge.microsoft.com/extensionwebstorebase/v1/crx"
SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallForcelist\1 = "abcdefghijklmnopabcdefghijklmnop"

```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: ExtensionInstallForcelist
  - Valor de ejemplo:
``` xml
<array>
  <string>gbchcmhmhahfdphkhkmpfmihenigjmpp;https://edge.microsoft.com/extensionwebstorebase/v1/crx</string>
  <string>abcdefghijklmnopabcdefghijklmnop</string>
</array>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### ExtensionInstallSources
  #### Configurar extensión y orígenes de instalación de script de usuario
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Defina las URL que pueden instalar extensiones y temas.

De manera predeterminada, los usuarios tienen que descargar un archivo *.crx para cada extensión o script que deseen instalar y, a continuación, arrastrarlo a la página de configuración de Microsoft Edge. Esta directiva permite que las URL específicas instalen la extensión o script para el usuario.

Cada elemento de esta lista es un patrón de coincidencia de estilo de extensión (consulte [https://go.microsoft.com/fwlink/?linkid=2095039](https://go.microsoft.com/fwlink/?linkid=2095039)). Los usuarios pueden instalar fácilmente elementos de cualquier URL que coincida con un elemento de esta lista. Estos patrones deben permitir tanto la ubicación del archivo *.crx como la página en la que se inicie la descarga (es decir, la dirección de referencia).

La directiva [ExtensionInstallBlocklist](#extensioninstallblocklist) tiene prioridad sobre esta directiva. Las extensiones que se encuentren en la lista de bloqueados no se instalarán, aunque provengan de un sitio de la lista.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Lista de cadenas

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: ExtensionInstallSources
  - Nombre de la directiva de grupos: Configurar extensión y orígenes de instalación de script de usuario
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/Extensiones
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallSources
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: 1, 2, 3, ...
  - Tipo de valor: lista de REG_SZ
  ##### Valor de ejemplo:
```
SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallSources\0 = "https://corp.contoso.com/*"

```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: ExtensionInstallSources
  - Valor de ejemplo:
``` xml
<array>
  <string>https://corp.contoso.com/*</string>
</array>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### ExtensionSettings
  #### Configurar ajustes de administración de extensiones
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Configura los ajustes de administración de extensiones para Microsoft Edge.

Esta directiva controla múltiples ajustes, incluidos los ajustes controlados por cualquier directiva existente relacionada con las extensiones. Esta directiva invalida cualquier directiva heredada si se establecen ambas.

Esta directiva asigna un id. de extensión o una URL de actualización a su configuración. Con un id. de extensión, la configuración se aplica solo a la extensión especificada. Establezca una configuración predeterminada para el id. especial "*", que se aplicará a todas las extensiones que no se indiquen específicamente en esta directiva. Con una URL de actualización, la configuración se aplica a todas las extensiones con la URL de actualización exacta establecida en el manifiesto de esta extensión, como se describe en [https://go.microsoft.com/fwlink/?linkid=2095043](https://go.microsoft.com/fwlink/?linkid=2095043).

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Diccionario

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: ExtensionSettings
  - Nombre de la directiva de grupos: Configurar ajustes de administración de extensiones
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/Extensiones
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: ExtensionSettings
  - Tipo de valor: REG_SZ
  ##### Valor de ejemplo:
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


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: ExtensionSettings
  - Valor de ejemplo:
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
  

  [Volver al principio](#microsoft-edge:-directivas)

  ## Imprimir policies

  [Volver al principio](#microsoft-edge:-directivas)

  ### DefaultPrinterSelection
  #### Reglas de selección de impresora predeterminada
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Invalida las reglas de selección de la impresora predeterminada de Microsoft Edge. Esta directiva determina las reglas para seleccionar la impresora predeterminada en Microsoft Edge, que ocurre la primera vez que un usuario intenta imprimir una página.

Cuando se establece esta directiva, Microsoft Edge intenta buscar una impresora que coincida con todos los atributos especificados y la usa como impresora predeterminada. Si hay varias impresoras que cumplan los criterios, se usará la primera impresora que coincida.

Si no se configura esta directiva o no se encuentra ninguna impresora coincidente en el tiempo de espera, la impresora será de manera predeterminada la impresora PDF integrada o ninguna impresora, si la impresora PDF no está disponible.

El valor se analiza como un objeto JSON, según el esquema siguiente: { "type": "object", "properties": { "idPattern": { "description": "Regular expression to match printer id.", "type": "string" }, "namePattern": { "description": "Regular expression to match printer display name.", "type": "string" } } }

Si se omite un campo, coincidirán todos los valores; por ejemplo, si no se especifica ninguna conectividad, la Vista previa de impresión empezará a detectar todas las impresoras locales. Los patrones de expresiones regulares deben seguir la sintaxis de JavaScript RegExp y las coincidencias distinguirán mayúsculas de minúsculas.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Cadena

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: DefaultPrinterSelection
  - Nombre de la directiva de grupos: Reglas de selección de impresora predeterminada
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/Imprimir
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: DefaultPrinterSelection
  - Tipo de valor: REG_SZ
  ##### Valor de ejemplo:
```
"{ "idPattern": ".*public", "namePattern": ".*Color" }"
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: DefaultPrinterSelection
  - Valor de ejemplo:
``` xml
<string>{ "idPattern": ".*public", "namePattern": ".*Color" }</string>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### PrintHeaderFooter
  #### Imprimir encabezados y pies de página
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Haz que los "encabezados y pies de página" estén activados o desactivados en el cuadro de diálogo de impresión.

Si no configuras esta directiva, los usuarios podrán decidir si quieren imprimir los encabezados y pies de página.

Si deshabilitas esta directiva, los usuarios no podrán imprimir encabezados y pies de página.

Si habilitas esta directiva, los usuarios podrán imprimir siempre encabezados y pies de página.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: Sí
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Booleano

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: PrintHeaderFooter
  - Nombre de la directiva de grupos: Imprimir encabezados y pies de página
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/Imprimir
  - Ruta de acceso de GP (Recomendada): Plantillas administrativas/Microsoft Edge - Configuración predeterminada (los usuarios pueden cambiarla)/Imprimir
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): SOFTWARE\Policies\Microsoft\Edge\Recomendada
  - Nombre del valor: PrintHeaderFooter
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000000
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: PrintHeaderFooter
  - Valor de ejemplo:
``` xml
<false/>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### PrintPreviewUseSystemDefaultPrinter
  #### Establecer la impresora predeterminada del sistema como la impresora predeterminada
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Insta a Microsoft Edge a usar la impresora predeterminada del sistema como la opción predeterminada en la vista previa de impresión en lugar de la impresora utilizada recientemente.

Si se deshabilita esta directiva o no se configura, la vista previa de impresión usará la impresora utilizada recientemente como la opción de destino predeterminada.

Si se habilita esta directiva, la vista previa de impresión usará la impresora predeterminada del sistema de SO como la opción de destino predeterminada.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: Sí
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Booleano

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: PrintPreviewUseSystemDefaultPrinter
  - Nombre de la directiva de grupos: Establecer la impresora predeterminada del sistema como la impresora predeterminada
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/Imprimir
  - Ruta de acceso de GP (Recomendada): Plantillas administrativas/Microsoft Edge - Configuración predeterminada (los usuarios pueden cambiarla)/Imprimir
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): SOFTWARE\Policies\Microsoft\Edge\Recomendada
  - Nombre del valor: PrintPreviewUseSystemDefaultPrinter
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000000
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: PrintPreviewUseSystemDefaultPrinter
  - Valor de ejemplo:
``` xml
<false/>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### PrintingEnabled
  #### Habilitar la impresión
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Habilita la impresión en Microsoft Edge e impide que los usuarios cambien esta configuración.

Si se habilita esta directiva o no se configura, los usuarios podrán imprimir.

Si se deshabilita esta directiva, los usuarios no podrán imprimir desde Microsoft Edge. La impresión está deshabilitada en el menú de llave, las extensiones, las aplicaciones de JavaScript, etc. Los usuarios podrán seguir imprimiendo desde los complementos que omitan Microsoft Edge durante la impresión. Por ejemplo, determinadas aplicaciones de Adobe Flash tienen la opción de imprimir en el menú contextual, que no está cubierto por esta directiva.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Booleano

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: PrintingEnabled
  - Nombre de la directiva de grupos: Habilitar la impresión
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/Imprimir
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: PrintingEnabled
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000001
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: PrintingEnabled
  - Valor de ejemplo:
``` xml
<true/>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### UseSystemPrintDialog
  #### Imprimir usando el cuadro de diálogo de impresión
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Muestra el cuadro de diálogo de impresión del sistema en lugar de la vista previa de impresión.

Si se habilita esta directiva, Microsoft Edge abrirá el cuadro de diálogo de impresión del sistema en lugar de la vista previa de impresión integrada cuando un usuario imprime una página.

Si no se configura o si se deshabilita esta directiva, los comandos de impresión desencadenan la pantalla de vista previa de impresión de Microsoft Edge.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: No - Requiere reiniciar el explorador

  #### Tipo de datos:
  Booleano

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: UseSystemPrintDialog
  - Nombre de la directiva de grupos: Imprimir usando el cuadro de diálogo de impresión
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/Imprimir
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: UseSystemPrintDialog
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000000
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: UseSystemPrintDialog
  - Valor de ejemplo:
``` xml
<false/>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ## Inicio&comma; página principal y página de la nueva pestaña policies

  [Volver al principio](#microsoft-edge:-directivas)

  ### HomepageIsNewTabPage
  #### Establecer la página de la nueva pestaña como página principal
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Configura la página principal predeterminada en Microsoft Edge. Puede establecer la página principal a la URL que especifique o a la página de la nueva pestaña.

Si se habilita esta directiva, siempre se usará la página de la nueva pestaña para la página principal y se omitirá la ubicación de la URL de la página principal.

Si se deshabilita esta directiva, la página principal del usuario no podrá ser la página de la nueva pestaña, a menos que la URL se establezca en 'edge://newtab'.

Si no se ha configurado, los usuarios podrán elegir si la página de la nueva pestaña es o no la página principal.

Esta directiva solo está disponible en las instancias de Windows que están unidas a un dominio de Microsoft Active Directory o en las instancias de Windows 10 Pro o Enterprise inscritas para la administración de dispositivos.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: Sí
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Booleano

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: HomepageIsNewTabPage
  - Nombre de la directiva de grupos: Establecer la página de la nueva pestaña como página principal
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/Inicio, página principal y página de la nueva pestaña
  - Ruta de acceso de GP (Recomendada): Plantillas administrativas/Microsoft Edge - Configuración predeterminada (los usuarios pueden cambiarla)/Inicio, página principal y página de la nueva pestaña
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): SOFTWARE\Policies\Microsoft\Edge\Recomendada
  - Nombre del valor: HomepageIsNewTabPage
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000001
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: HomepageIsNewTabPage
  - Valor de ejemplo:
``` xml
<true/>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### HomepageLocation
  #### Configurar la dirección URL de la página principal
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Configura la URL de la página principal predeterminada en Microsoft Edge.

La página principal es la página que abre el botón Inicio. Las páginas que se abren al inicio se controlan mediante las directivas [RestoreOnStartup](#restoreonstartup).

Se puede establecer una dirección URL aquí o establecer la página principal para abrir la página de la nueva pestaña. Si se selecciona abrir la página de la nueva pestaña, esta directiva no surtirá efecto.

Si se habilita esta directiva, los usuarios no podrán cambiar la dirección URL de la página principal, pero podrán elegir usar la página de la nueva pestaña como página principal.

Si se deshabilita o no se configura esta directiva, los usuarios podrán elegir su propia página principal, siempre y cuando la directiva [HomepageIsNewTabPage](#homepageisnewtabpage) no esté habilitada.

Esta directiva solo está disponible en las instancias de Windows que están unidas a un dominio de Microsoft Active Directory o instancias de Windows 10 Pro o Enterprise que están inscritas para la administración de dispositivos.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: Sí
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Cadena

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: HomepageLocation
  - Nombre de la directiva de grupos: Configurar la dirección URL de la página principal
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/Inicio, página principal y página de la nueva pestaña
  - Ruta de acceso de GP (Recomendada): Plantillas administrativas/Microsoft Edge - Configuración predeterminada (los usuarios pueden cambiarla)/Inicio, página principal y página de la nueva pestaña
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): SOFTWARE\Policies\Microsoft\Edge\Recomendada
  - Nombre del valor: HomepageLocation
  - Tipo de valor: REG_SZ
  ##### Valor de ejemplo:
```
"https://www.contoso.com"
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: HomepageLocation
  - Valor de ejemplo:
``` xml
<string>https://www.contoso.com</string>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### NewTabPageCompanyLogo
  #### Establecer el logotipo de la empresa en la nueva ficha
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 79 o posterior

  #### Descripción
  Specifies the company logo to use on the new tab page in Microsoft Edge.

The policy should be configured as a string that expresses the logo(s) in JSON format. For example: { "default_logo": { "url": "https://www.contoso.com/logo.png", "hash": "cd0aa9856147b6c5b4ff2b7dfee5da20aa38253099ef1b4a64aced233c9afe29" }, "light_logo": { "url": "https://www.contoso.com/light_logo.png", "hash": "517d286edb416bb2625ccfcba9de78296e90da8e32330d4c9c8275c4c1c33737" } }

You configure this policy by specifying the URL from which Microsoft Edge can download the logo and its cryptographic hash (SHA-256), which is used to verify the integrity of the download. The logo must be in PNG or SVG format, and its file size must not exceed 16 MB. The logo is downloaded and cached, and it will be redownloaded whenever the URL or the hash changes. The URL must be accessible without any authentication.

The 'default_logo' is required and will be used when there's no background image. If 'light_logo' is provided, it will be used when the user's new tab page has a background image. We recommend a horizontal logo with a transparent background that is left-aligned and vertically centered. The logo should have a minimum height of 32 pixels and an aspect ratio from 1:1 to 4:1. The 'default_logo' should have proper contrast against a white/black background while the 'light_logo' should have proper contrast against a background image.

If you enable this policy, Microsoft Edge downloads and shows the specified logo(s) on the new tab page. Users can't override or hide the logo(s).

If you disable or don't configure this policy, Microsoft Edge will show no company logo or a Microsoft logo on the new tab page.

For help with determining the SHA-256 hash, see https://docs.microsoft.com/powershell/module/microsoft.powershell.utility/get-filehash.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: No - Requiere reiniciar el explorador

  #### Tipo de datos:
  Diccionario

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: NewTabPageCompanyLogo
  - Nombre de la directiva de grupos: Establecer el logotipo de la empresa en la nueva ficha
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/Inicio, página principal y página de la nueva pestaña
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: NewTabPageCompanyLogo
  - Tipo de valor: REG_SZ
  ##### Valor de ejemplo:
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


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: NewTabPageCompanyLogo
  - Valor de ejemplo:
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
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### NewTabPageHideDefaultTopSites
  #### Ocultar los sitios principales predeterminados de la página de la nueva pestaña
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Oculta los sitios principales predeterminados de la página de la nueva pestaña en Microsoft Edge.

Si se establece esta directiva como true, se ocultarán los iconos de los sitios principales predeterminados.

Si se establece esta directiva como false o no se configura, los iconos de los sitios principales predeterminados permanecerán visibles.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Booleano

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: NewTabPageHideDefaultTopSites
  - Nombre de la directiva de grupos: Ocultar los sitios principales predeterminados de la página de la nueva pestaña
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/Inicio, página principal y página de la nueva pestaña
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: NewTabPageHideDefaultTopSites
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000001
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: NewTabPageHideDefaultTopSites
  - Valor de ejemplo:
``` xml
<true/>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### NewTabPageLocation
  #### Configurar la dirección URL de la página de la nueva pestaña
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Configura la dirección URL predeterminada para la página de la nueva pestaña.

Esta directiva determina la página que se abre cuando se crean nuevas pestañas (también cuando se abren nuevas ventanas). También afecta a la página de inicio si está configurada para abrirse en la página de la nueva pestaña.

Esta directiva no determina qué página se abre en el inicio; está controlado por la directiva [RestoreOnStartup](#restoreonstartup). Tampoco afecta a la página de inicio si está configurada para abrirse en la página de la nueva pestaña.

Si no se configura esta directiva, se usará la página de la nueva pestaña predeterminada.

Si se configura esta directiva *y* la directiva [NewTabPageSetFeedType](#newtabpagesetfeedtype), esta directiva tendrá prioridad.

Si se proporciona una dirección URL no válida, las nuevas pestañas abrirán about://blank.

Esta directiva solo está disponible en las instancias de Windows que están unidas a un dominio de Microsoft Active Directory o instancias de Windows 10 Pro o Enterprise que están inscritas para la administración de dispositivos.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: Sí
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Cadena

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: NewTabPageLocation
  - Nombre de la directiva de grupos: Configurar la dirección URL de la página de la nueva pestaña
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/Inicio, página principal y página de la nueva pestaña
  - Ruta de acceso de GP (Recomendada): Plantillas administrativas/Microsoft Edge - Configuración predeterminada (los usuarios pueden cambiarla)/Inicio, página principal y página de la nueva pestaña
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): SOFTWARE\Policies\Microsoft\Edge\Recomendada
  - Nombre del valor: NewTabPageLocation
  - Tipo de valor: REG_SZ
  ##### Valor de ejemplo:
```
"https://www.fabrikam.com"
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: NewTabPageLocation
  - Valor de ejemplo:
``` xml
<string>https://www.fabrikam.com</string>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### NewTabPageManagedQuickLinks
  #### Establecer vínculos rápidos a la página de la nueva pestaña
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 79 o posterior

  #### Descripción
  De manera predeterminada, Microsoft Edge muestra vínculos rápidos en la página de la nueva pestaña de los accesos directos agregados por el usuario y los sitios principales basados en el historial de exploración. Con esta directiva, puede configurar hasta tres iconos de vínculos rápidos en la página de la nueva pestaña, expresados como un objeto JSON:

[ { "url": "https://www.contoso.com", "title": "Contoso Portal", "pinned": true/false }, ... ]

El campo 'url' es obligatorio; 'title' y 'pinned' son opcionales. Si no se proporciona 'title', se usará la dirección URL como título predeterminado. Si no se proporciona 'pinned', el valor predeterminado será false.

Microsoft Edge los muestra en el orden en que aparecen en la lista, de izquierda a derecha, y todos los iconos anclados se muestran por delante de los iconos no anclados.

Si la directiva está establecida como obligatoria, se omitirá el campo 'pinned' y se anclarán todos los iconos. El usuario no puede eliminar los iconos y siempre aparecerán al principio de la lista de vínculos rápidos.

Si la directiva está establecida como se recomienda, los iconos anclados permanecerán en la lista, pero el usuario podrá editarlos y eliminarlos. Los iconos de vínculos rápidos que no están anclados se comportarán como los sitios principales predeterminados y se quitarán de la lista si otros sitios web se visitan con más frecuencia. Al aplicar vínculos no anclados mediante esta directiva a un perfil de explorador existente, es posible que los vínculos no aparezcan, en función de cómo se clasifiquen en comparación con el historial de exploración del usuario.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: Sí
  - Actualización de directiva dinámica: No - Requiere reiniciar el explorador

  #### Tipo de datos:
  Diccionario

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: NewTabPageManagedQuickLinks
  - Nombre de la directiva de grupos: Establecer vínculos rápidos a la página de la nueva pestaña
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/Inicio, página principal y página de la nueva pestaña
  - Ruta de acceso de GP (Recomendada): Plantillas administrativas/Microsoft Edge - Configuración predeterminada (los usuarios pueden cambiarla)/Inicio, página principal y página de la nueva pestaña
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): SOFTWARE\Policies\Microsoft\Edge\Recomendada
  - Nombre del valor: NewTabPageManagedQuickLinks
  - Tipo de valor: REG_SZ
  ##### Valor de ejemplo:
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


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: NewTabPageManagedQuickLinks
  - Valor de ejemplo:
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
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### NewTabPageSetFeedType
  #### Configurar la experiencia de página de la nueva pestaña de Microsoft Edge
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 79 o posterior

  #### Descripción
  Le permite elegir la experiencia de la fuente de Office 365 o Microsoft News para la página de la nueva pestaña.

Al establecer esta directiva en la experiencia de la fuente de Microsoft News (0), los usuarios verán la experiencia de la fuente de Microsoft News en la página de la nueva pestaña.

Al establecer esta directiva en la experiencia de la fuente de Office 365 (1), los usuarios con un inicio de sesión en el explorador de Azure Active Directory verán la experiencia de la fuente de Office 365 en la página de la nueva pestaña.

Si deshabilita o no configura esta directiva:

- A los usuarios con un inicio de sesión del explorador de Azure Active Directory se le ofrecerá la experiencia de la fuente de la página de la nueva pestaña de Office 365, así como la experiencia estándar de la fuente de la página de la nueva pestaña.

- Los usuarios que no tengan un inicio de sesión en el explorador de Azure Active Directory verán la experiencia estándar de la página de la nueva pestaña.

Si configura esta directiva *y* la [NewTabPageLocation](#newtabpagelocation) directiva, [NewTabPageLocation](#newtabpagelocation) tiene prioridad.

Configuración predeterminada: deshabilitada o no configurada.

* 0 = Experiencia de la fuente de Microsoft News

* 1 = Experiencia de la fuente de Office 365

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: Sí
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Entero

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: NewTabPageSetFeedType
  - Nombre de la directiva de grupos: Configurar la experiencia de página de la nueva pestaña de Microsoft Edge
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/Inicio, página principal y página de la nueva pestaña
  - Ruta de acceso de GP (Recomendada): Plantillas administrativas/Microsoft Edge - Configuración predeterminada (los usuarios pueden cambiarla)/Inicio, página principal y página de la nueva pestaña
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): SOFTWARE\Policies\Microsoft\Edge\Recomendada
  - Nombre del valor: NewTabPageSetFeedType
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000000
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: NewTabPageSetFeedType
  - Valor de ejemplo:
``` xml
<integer>0</integer>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### RestoreOnStartup
  #### Acción que se realizará al inicio
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Especificar cómo se comporta Microsoft Edge cuando se inicia.

Si quiere que siempre se abra una nueva pestaña en el inicio, elija "Abrir nueva pestaña" (5).

Si quiere volver a abrir las direcciones URL que estaban abiertas la última vez que se cerró Microsoft Edge, elija "Restaurar la última sesión" (1). Se restaurará la sesión de exploración tal como estaba. Tenga en cuenta que esta opción deshabilita algunas opciones de configuración que se basan en sesiones o que realizan acciones al salir (por ejemplo, borrar datos de exploración al salir o cookies solo de sesión).

Si quiere abrir un conjunto específico de direcciones URL, elija "Abrir una lista de direcciones URL" (4).

Deshabilitar esta configuración es equivalente a dejarla no configurada. Los usuarios podrán cambiarla en Microsoft Edge.

Esta directiva solo está disponible en las instancias de Windows que estén unidas a un dominio de Microsoft Active Directory o instancias de Windows 10 Pro o Enterprise inscritas para la administración de dispositivos.

* 5 = Abrir una nueva pestaña

* 1 = Restaurar la última sesión

* 4 = Abrir una lista de direcciones URL

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: Sí
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Entero

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: RestoreOnStartup
  - Nombre de la directiva de grupos: Acción que se realizará al inicio
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/Inicio, página principal y página de la nueva pestaña
  - Ruta de acceso de GP (Recomendada): Plantillas administrativas/Microsoft Edge - Configuración predeterminada (los usuarios pueden cambiarla)/Inicio, página principal y página de la nueva pestaña
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): SOFTWARE\Policies\Microsoft\Edge\Recomendada
  - Nombre del valor: RestoreOnStartup
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000004
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: RestoreOnStartup
  - Valor de ejemplo:
``` xml
<integer>4</integer>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### RestoreOnStartupURLs
  #### Sitios que se abrirán cuando se inicia el explorador
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Especificar una lista de sitios web que se abran automáticamente cuando se inicia el explorador. Si no se configura esta directiva, no se abrirá ningún sitio en el inicio.

Esta directiva solo funciona si se establece también la directiva [RestoreOnStartup](#restoreonstartup) en 'Abrir una lista de direcciones URL' (4).

Esta directiva solo está disponible en instancias de Windows que estén unidas a un dominio de Microsoft Active Directory o instancias de Windows 10 Pro o Enterprise que están inscritas en la administración de dispositivos.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: Sí
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Lista de cadenas

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: RestoreOnStartupURLs
  - Nombre de la directiva de grupos: Sitios que se abrirán cuando se inicia el explorador
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/Inicio, página principal y página de la nueva pestaña
  - Ruta de acceso de GP (Recomendada): Plantillas administrativas/Microsoft Edge - Configuración predeterminada (los usuarios pueden cambiarla)/Inicio, página principal y página de la nueva pestaña
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge\RestoreOnStartupURLs
  - Ruta de acceso (Recomendada): SOFTWARE\Policies\Microsoft\Edge\Recomendada\RestoreOnStartupURLs
  - Nombre del valor: 1, 2, 3, ...
  - Tipo de valor: lista de REG_SZ
  ##### Valor de ejemplo:
```
SOFTWARE\Policies\Microsoft\Edge\RestoreOnStartupURLs\0 = "https://contoso.com"
SOFTWARE\Policies\Microsoft\Edge\RestoreOnStartupURLs\1 = "https://www.fabrikam.com"

```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: RestoreOnStartupURLs
  - Valor de ejemplo:
``` xml
<array>
  <string>https://contoso.com</string>
  <string>https://www.fabrikam.com</string>
</array>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### ShowHomeButton
  #### Mostrar el botón Inicio en la barra de herramientas
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Muestra el botón Inicio en la barra de herramientas de Microsoft Edge.

Habilite esta directiva para mostrar siempre el botón Inicio. Deshabilítela para no mostrar el botón.

Si no se establece la directiva, los usuarios pueden elegir si quieren mostrar el botón Inicio.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: Sí
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Booleano

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: ShowHomeButton
  - Nombre de la directiva de grupos: Mostrar el botón Inicio en la barra de herramientas
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/Inicio, página principal y página de la nueva pestaña
  - Ruta de acceso de GP (Recomendada): Plantillas administrativas/Microsoft Edge - Configuración predeterminada (los usuarios pueden cambiarla)/Inicio, página principal y página de la nueva pestaña
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): SOFTWARE\Policies\Microsoft\Edge\Recomendada
  - Nombre del valor: ShowHomeButton
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000001
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: ShowHomeButton
  - Valor de ejemplo:
``` xml
<true/>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ## Mensajería nativa policies

  [Volver al principio](#microsoft-edge:-directivas)

  ### NativeMessagingAllowlist
  #### Controlar qué hosts de mensajería nativos pueden usar los usuarios
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Especifica los hosts de mensajes nativos que los usuarios pueden usar en Microsoft Edge.

De manera predeterminada, se permiten todos los hosts de mensajes nativos. Si se configura la directiva [NativeMessagingBlocklist](#nativemessagingblocklist) a *, se bloquearán todos los hosts de mensajes nativos y solo se cargarán los hosts de mensajes nativos de aquí.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Lista de cadenas

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: NativeMessagingAllowlist
  - Nombre de la directiva de grupos: Controlar qué hosts de mensajería nativos pueden usar los usuarios
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/Mensajería nativa
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge\NativeMessagingAllowlist
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: 1, 2, 3, ...
  - Tipo de valor: lista de REG_SZ
  ##### Valor de ejemplo:
```
SOFTWARE\Policies\Microsoft\Edge\NativeMessagingAllowlist\0 = "com.native.messaging.host.name1"
SOFTWARE\Policies\Microsoft\Edge\NativeMessagingAllowlist\1 = "com.native.messaging.host.name2"

```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: NativeMessagingAllowlist
  - Valor de ejemplo:
``` xml
<array>
  <string>com.native.messaging.host.name1</string>
  <string>com.native.messaging.host.name2</string>
</array>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### NativeMessagingBlocklist
  #### Configurar la lista de bloqueados de mensajes nativa
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Especifica qué hosts de mensajes nativos no deben usarse.

Use '*' para bloquear todos los hosts de mensajes nativos a menos que aparezcan explícitamente en la lista de permitidos.

Si no se configura esta directiva, Microsoft Edge cargará todos los hosts de mensajes nativos instalados.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Lista de cadenas

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: NativeMessagingBlocklist
  - Nombre de la directiva de grupos: Configurar la lista de bloqueados de mensajes nativa
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/Mensajería nativa
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge\NativeMessagingBlocklist
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: 1, 2, 3, ...
  - Tipo de valor: lista de REG_SZ
  ##### Valor de ejemplo:
```
SOFTWARE\Policies\Microsoft\Edge\NativeMessagingBlocklist\0 = "com.native.messaging.host.name1"
SOFTWARE\Policies\Microsoft\Edge\NativeMessagingBlocklist\1 = "com.native.messaging.host.name2"

```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: NativeMessagingBlocklist
  - Valor de ejemplo:
``` xml
<array>
  <string>com.native.messaging.host.name1</string>
  <string>com.native.messaging.host.name2</string>
</array>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### NativeMessagingUserLevelHosts
  #### Permitir hosts de mensajería nativos de nivel de usuario (instalados sin permisos del administrador)
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Permite la instalación de nivel de usuario de los hosts de mensajes nativos.

Si se deshabilita esta directiva, Microsoft Edge solo usará hosts de mensajes nativos instalados en el nivel de sistema.

De manera predeterminada, si no se configura esta directiva, Microsoft Edge permitirá el uso de hosts de mensajes nativos de nivel de usuario.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Booleano

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: NativeMessagingUserLevelHosts
  - Nombre de la directiva de grupos: Permitir hosts de mensajería nativos de nivel de usuario (instalados sin permisos del administrador)
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/Mensajería nativa
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: NativeMessagingUserLevelHosts
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000000
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: NativeMessagingUserLevelHosts
  - Valor de ejemplo:
``` xml
<false/>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ## Proveedor de búsquedas predeterminado policies

  [Volver al principio](#microsoft-edge:-directivas)

  ### DefaultSearchProviderEnabled
  #### Habilitar el proveedor de búsquedas predeterminado
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Habilita el uso de un proveedor de búsqueda predeterminado.

Si se habilita esta directiva, un usuario puede buscar un término escribiendo en la barra de direcciones (siempre y cuando no se escriba una dirección URL).

Puede especificarse el proveedor de búsqueda predeterminado habilitando el resto de las directivas de búsqueda predeterminadas. Si éstos se dejan en blanco (sin configurar), el usuario puede elegir el proveedor predeterminado.

Si se deshabilita esta directiva, el usuario no puede buscar desde la barra de direcciones.

Si se habilita o se deshabilita esta directiva, los usuarios no podrán cambiarla o reemplazarla.

Si no se configura esta directiva, el proveedor de búsquedas predeterminado estará habilitado y el usuario podrá elegir el proveedor de búsquedas predeterminado y establecer la lista de proveedores de búsqueda.

Esta directiva solo está disponible en las instancias de Windows que estén unidas a un dominio deMicrosoft Active Directory o a instancias de Windows 10 Pro o Enterprise que estén inscritas para la administración de dispositivos.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Booleano

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: DefaultSearchProviderEnabled
  - Nombre de la directiva de grupos: Habilitar el proveedor de búsquedas predeterminado
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/Proveedor de búsquedas predeterminado
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: DefaultSearchProviderEnabled
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000001
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: DefaultSearchProviderEnabled
  - Valor de ejemplo:
``` xml
<true/>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### DefaultSearchProviderEncodings
  #### Codificaciones del proveedor de búsquedas predeterminado
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Especificar las codificaciones de caracteres que admite el proveedor de búsquedas. Las codificaciones son nombres de páginas de códigos como UTF-8, GB2312 y ISO-8859-1. Se prueban en el orden indicado.

Esta directiva es opcional. Si no se configura, se usa el valor predeterminado, UTF-8.

Esta directiva solo se aplica si se habilitan las directivas [DefaultSearchProviderEnabled](#defaultsearchproviderenabled) y [DefaultSearchProviderSearchURL](#defaultsearchprovidersearchurl).

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Lista de cadenas

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: DefaultSearchProviderEncodings
  - Nombre de la directiva de grupos: Codificaciones del proveedor de búsquedas predeterminado
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/Proveedor de búsquedas predeterminado
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge\DefaultSearchProviderEncodings
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: 1, 2, 3, ...
  - Tipo de valor: lista de REG_SZ
  ##### Valor de ejemplo:
```
SOFTWARE\Policies\Microsoft\Edge\DefaultSearchProviderEncodings\0 = "UTF-8"
SOFTWARE\Policies\Microsoft\Edge\DefaultSearchProviderEncodings\1 = "UTF-16"
SOFTWARE\Policies\Microsoft\Edge\DefaultSearchProviderEncodings\2 = "GB2312"
SOFTWARE\Policies\Microsoft\Edge\DefaultSearchProviderEncodings\3 = "ISO-8859-1"

```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: DefaultSearchProviderEncodings
  - Valor de ejemplo:
``` xml
<array>
  <string>UTF-8</string>
  <string>UTF-16</string>
  <string>GB2312</string>
  <string>ISO-8859-1</string>
</array>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### DefaultSearchProviderImageURL
  #### Especifica la característica de búsqueda por imagen para el proveedor de búsquedas predeterminado
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Especifica la dirección URL del motor de búsqueda que se usa para la búsqueda de imagen. Se envían las solicitudes de búsqueda mediante el método GET.

Esta directiva es opcional. Si no se configura, la búsqueda de imagen no está disponible.

Especifique la dirección URL de búsqueda de imágenes de Bing como:
'{bing:baseURL}images/detail/search?iss=sbiupload&FORM=ANCMS1#enterInsights'.

Especifique la dirección URL de búsqueda de imágenes de Google como: '{google:baseURL}searchbyimage/upload'.

Consulte la directiva [DefaultSearchProviderImageURLPostParams](#defaultsearchproviderimageurlpostparams) para finalizar la configuración de la búsqueda de imágenes.

Esta directiva se aplica solo si se habilitan las directivas [DefaultSearchProviderEnabled](#defaultsearchproviderenabled) y [DefaultSearchProviderSearchURL](#defaultsearchprovidersearchurl).

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Cadena

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: DefaultSearchProviderImageURL
  - Nombre de la directiva de grupos: Especifica la característica de búsqueda por imagen para el proveedor de búsquedas predeterminado
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/Proveedor de búsquedas predeterminado
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: DefaultSearchProviderImageURL
  - Tipo de valor: REG_SZ
  ##### Valor de ejemplo:
```
"https://search.contoso.com/searchbyimage/upload"
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: DefaultSearchProviderImageURL
  - Valor de ejemplo:
``` xml
<string>https://search.contoso.com/searchbyimage/upload</string>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### DefaultSearchProviderImageURLPostParams
  #### Parámetros para una dirección URL de imagen que usa POST
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Si se habilita esta directiva, se especifican los parámetros usados cuando se realiza una búsqueda de imagen que use POST. La directiva consiste en pares de nombre/valor separados por comas. Si un valor es un parámetro de plantilla, como {imageThumbnail} en el ejemplo anterior, se reemplaza con los datos de miniaturas de imagen reales. Esta directiva se aplica solo si se habilitan las directivas [DefaultSearchProviderEnabled](#defaultsearchproviderenabled) y [DefaultSearchProviderSearchURL](#defaultsearchprovidersearchurl).

Especificar los parámetros de POST de la dirección URL de la búsqueda de imágenes de Bing como:
'imageBin={google:imageThumbnailBase64}'.

Especificar los parámetros de POST de la dirección URL de la búsqueda de imagen de Google como:
'encoded_image={google:imageThumbnail},image_url={google:imageURL},sbisrc={google:imageSearchSource},original_width={google:imageOriginalWidth},original_height={google:imageOriginalHeight}'.

Si no se configura esta directiva, se envían las solicitudes de búsqueda de imágenes con el método GET.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Cadena

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: DefaultSearchProviderImageURLPostParams
  - Nombre de la directiva de grupos: Parámetros para una dirección URL de imagen que usa POST
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/Proveedor de búsquedas predeterminado
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: DefaultSearchProviderImageURLPostParams
  - Tipo de valor: REG_SZ
  ##### Valor de ejemplo:
```
"content={imageThumbnail},url={imageURL},sbisrc={SearchSource}"
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: DefaultSearchProviderImageURLPostParams
  - Valor de ejemplo:
``` xml
<string>content={imageThumbnail},url={imageURL},sbisrc={SearchSource}</string>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### DefaultSearchProviderKeyword
  #### Palabra clave del proveedor de búsquedas predeterminado
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Especifica la palabra clave, que es el acceso directo que se usa en la barra de direcciones para desencadenar la búsqueda para este proveedor.

Esta directiva es opcional. Si no se configura, ninguna palabra clave activará el proveedor de búsquedas.

Esta directiva solo se respeta si se habilitan las directivas [DefaultSearchProviderEnabled](#defaultsearchproviderenabled) y [DefaultSearchProviderSearchURL](#defaultsearchprovidersearchurl).

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Cadena

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: DefaultSearchProviderKeyword
  - Nombre de la directiva de grupos: Palabra clave del proveedor de búsquedas predeterminado
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/Proveedor de búsquedas predeterminado
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: DefaultSearchProviderKeyword
  - Tipo de valor: REG_SZ
  ##### Valor de ejemplo:
```
"mis"
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: DefaultSearchProviderKeyword
  - Valor de ejemplo:
``` xml
<string>mis</string>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### DefaultSearchProviderName
  #### Nombre del proveedor de búsquedas predeterminado
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Especifica el nombre del proveedor de búsquedas predeterminado.

Si se habilita esta directiva, se establecerá el nombre del proveedor de búsquedas predeterminado.

Si no se habilita esta directiva o si se deja en blanco, se usará el nombre de host especificado por la dirección URL de búsqueda.

Debe establecerse 'DefaultSearchProviderName' en un proveedor de búsquedas cifradas aprobado por la organización que se corresponda con el proveedor de búsquedas cifradas establecido en DTBC-0008. Esta directiva solo se aplica si se habilitan las directivas [DefaultSearchProviderEnabled](#defaultsearchproviderenabled) y [DefaultSearchProviderSearchURL](#defaultsearchprovidersearchurl).

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Cadena

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: DefaultSearchProviderName
  - Nombre de la directiva de grupos: Nombre del proveedor de búsquedas predeterminado
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/Proveedor de búsquedas predeterminado
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: DefaultSearchProviderName
  - Tipo de valor: REG_SZ
  ##### Valor de ejemplo:
```
"My Intranet Search"
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: DefaultSearchProviderName
  - Valor de ejemplo:
``` xml
<string>My Intranet Search</string>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### DefaultSearchProviderSearchURL
  #### URL de búsqueda del proveedor de búsquedas predeterminado
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Especifica la dirección URL del motor de búsqueda que se usa para una búsqueda predeterminada. La dirección URL contiene la cadena '{searchTerms}', que se reemplaza en tiempo de consulta por los términos que está buscando el usuario.

Especificar la dirección URL de Bing como:

'{bing:baseURL}search?q={searchTerms}'.

Especificar la dirección URL de Google como: '{google:baseURL}search?q={searchTerms}&{google:RLZ}{google:originalQueryForSuggestion}{google:assistedQueryStats}{google:searchFieldtrialParameter}{google:searchClient}{google:sourceId}ie={inputEncoding}'.

Esta directiva es necesaria cuando se habilita la directiva [DefaultSearchProviderEnabled](#defaultsearchproviderenabled); si no se habilita la última directiva, se omitirá esta directiva.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Cadena

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: DefaultSearchProviderSearchURL
  - Nombre de la directiva de grupos: URL de búsqueda del proveedor de búsquedas predeterminado
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/Proveedor de búsquedas predeterminado
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: DefaultSearchProviderSearchURL
  - Tipo de valor: REG_SZ
  ##### Valor de ejemplo:
```
"https://search.contoso.com/search?q={searchTerms}"
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: DefaultSearchProviderSearchURL
  - Valor de ejemplo:
``` xml
<string>https://search.contoso.com/search?q={searchTerms}</string>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### DefaultSearchProviderSuggestURL
  #### URL del proveedor de búsqueda predeterminado para obtener sugerencias
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Especifica la dirección URL del motor de búsqueda usado para proporcionar sugerencias de búsqueda. La dirección URL contiene la cadena '{searchTerms}', que se reemplaza en el momento de la consulta por el texto que el usuario ha escrito hasta ese momento.

Esta directiva es opcional. Si no se configura, los usuarios no verán las sugerencias de búsqueda; verán sugerencias de su historial de exploración y favoritos.

La dirección URL sugerida de Bing se puede especificar como:

'{bing:baseURL}qbox?query={searchTerms}'.

La dirección URL sugerida de Google se puede especificar como: '{google:baseURL}complete/search?output=chrome&q={searchTerms}'.

Esta directiva solo se aplica si se habilitan las directivas [DefaultSearchProviderEnabled](#defaultsearchproviderenabled) y [DefaultSearchProviderSearchURL](#defaultsearchprovidersearchurl).

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Cadena

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: DefaultSearchProviderSuggestURL
  - Nombre de la directiva de grupos: URL del proveedor de búsqueda predeterminado para obtener sugerencias
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/Proveedor de búsquedas predeterminado
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: DefaultSearchProviderSuggestURL
  - Tipo de valor: REG_SZ
  ##### Valor de ejemplo:
```
"https://search.contoso.com/suggest?q={searchTerms}"
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: DefaultSearchProviderSuggestURL
  - Valor de ejemplo:
``` xml
<string>https://search.contoso.com/suggest?q={searchTerms}</string>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ## Servidor proxy policies

  [Volver al principio](#microsoft-edge:-directivas)

  ### ProxyBypassList
  #### Configurar reglas de omisión de proxy
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Define una lista de hosts para los que Microsoft Edge omite cualquier proxy.

Esta directiva se aplica solo si se ha seleccionado 'Usar servidores proxy fijos' en la directiva [ProxyMode](#proxymode). Si se ha seleccionado cualquier otro modo para la configuración de directivas de proxy, no debe habilitar ni configurar esta directiva.

Si se habilita esta directiva, puede crear una lista de hosts para los que Microsoft Edge no usa un proxy.

Si no se configura esta directiva, no se crea ninguna lista de hosts para los que Microsoft Edge omite un proxy. Deje esta directiva sin configurar si se ha especificado algún otro método para establecer las directivas de proxy.

Para obtener ejemplos más detallados, visite [https://go.microsoft.com/fwlink/?linkid=2094936](https://go.microsoft.com/fwlink/?linkid=2094936).

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Cadena

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: ProxyBypassList
  - Nombre de la directiva de grupos: Configurar reglas de omisión de proxy
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/Servidor proxy
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: ProxyBypassList
  - Tipo de valor: REG_SZ
  ##### Valor de ejemplo:
```
"https://www.contoso.com, https://www.fabrikam.com"
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: ProxyBypassList
  - Valor de ejemplo:
``` xml
<string>https://www.contoso.com, https://www.fabrikam.com</string>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### ProxyMode
  #### Configurar ajustes del servidor proxy
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Especificar la configuración del servidor proxy usada por Microsoft Edge. Si se habilita esta directiva, los usuarios no pueden cambiar la configuración del proxy.

Si se elige no usar nunca un servidor proxy y conectarse siempre directamente, se omitirán todas las demás opciones.

Si se elige usar la configuración del proxy del sistema, se omitirán todas las demás opciones.

Si se elige detectar automáticamente el servidor proxy, se omitirán todas las demás opciones.

Si se elige el modo de proxy de servidor fijo, se pueden especificar más opciones en [ProxyServer](#proxyserver) y 'Lista de reglas de omisión de proxy separadas por comas'.

Si se elige usar un script de proxy .pac, se debe especificar la dirección URL al script en 'Dirección URL a un archivo .pac de proxy'.

Para obtener ejemplos detallados, vaya a [https://go.microsoft.com/fwlink/?linkid=2094936](https://go.microsoft.com/fwlink/?linkid=2094936).

Si se habilita esta directiva, Microsoft Edge omitirá todas las opciones relacionadas con el proxy especificadas desde la línea de comandos.

Si no se configura esta directiva, los usuarios podrán elegir su propia configuración del proxy.

* "direct" = Nunca usar un servidor proxy

* "auto_detect" = Detectar automáticamente la configuración del proxy

* "pac_script" = Usar un script de proxy .pac

* "fixed_servers" = Usar servidores proxy fijos

* "system" = Usar la configuración del proxy del sistema

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Cadena

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: ProxyMode
  - Nombre de la directiva de grupos: Configurar ajustes del servidor proxy
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/Servidor proxy
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: ProxyMode
  - Tipo de valor: REG_SZ
  ##### Valor de ejemplo:
```
"direct"
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: ProxyMode
  - Valor de ejemplo:
``` xml
<string>direct</string>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### ProxyPacUrl
  #### Establecer la dirección URL del archivo .pac del proxy
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Especifica la dirección URL de un archivo de configuración automática de proxy (PAC).

Esta directiva solo se aplica si se ha seleccionado 'Usar un script de proxy .pac' en la directiva [ProxyMode](#proxymode). Si se selecciona cualquier otro modo para configurar directivas de proxy, no debe habilitar ni configurar esta directiva.

Si se habilita esta directiva, puede especificarse la dirección URL de un archivo PAC, que define el modo en que el explorador elige automáticamente el servidor proxy adecuado para obtener un sitio web determinado.

Si se deshabilita o no se configura esta directiva, no se especifica ningún archivo PAC. Deje esta directiva sin configurar si ha especificado otro método para establecer directivas de proxy.

Para obtener ejemplos detallados, consulte [https://go.microsoft.com/fwlink/?linkid=2094936](https://go.microsoft.com/fwlink/?linkid=2094936).

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Cadena

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: ProxyPacUrl
  - Nombre de la directiva de grupos: Establecer la dirección URL del archivo .pac del proxy
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/Servidor proxy
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: ProxyPacUrl
  - Tipo de valor: REG_SZ
  ##### Valor de ejemplo:
```
"https://internal.contoso.com/example.pac"
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: ProxyPacUrl
  - Valor de ejemplo:
``` xml
<string>https://internal.contoso.com/example.pac</string>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### ProxyServer
  #### Configurar dirección o URL del servidor proxy
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Especifica la dirección URL del servidor proxy.

Esta directiva solo se aplica si se ha seleccionado 'Usar servidores proxy fijos' en la directiva [ProxyMode](#proxymode). Si se selecciona cualquier otro modo para configurar directivas de proxy, no habilite ni configure esta directiva.

Si se habilita esta directiva, se usará el servidor proxy configurado por esta directiva para todas las direcciones URL.

Si se deshabilita o no se configura esta directiva, los usuarios podrán elegir su propia configuración de proxy en este modo de proxy. Deje esta directiva sin configurar si ha especificado otro método para establecer directivas de proxy.

Para obtener más opciones y ejemplos detallados, consulte [https://go.microsoft.com/fwlink/?linkid=2094936](https://go.microsoft.com/fwlink/?linkid=2094936).

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Cadena

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: ProxyServer
  - Nombre de la directiva de grupos: Configurar dirección o URL del servidor proxy
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/Servidor proxy
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: ProxyServer
  - Tipo de valor: REG_SZ
  ##### Valor de ejemplo:
```
"123.123.123.123:8080"
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: ProxyServer
  - Valor de ejemplo:
``` xml
<string>123.123.123.123:8080</string>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### ProxySettings
  #### Configuración del proxy
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Configura las opciones de proxy para Microsoft Edge.

Si se habilita esta directiva, Microsoft Edge pasa por alto todas las opciones relacionadas con el proxy especificadas desde la línea de comandos.

Si no se configura esta directiva, los usuarios pueden elegir su propia configuración de proxy.

Esta directiva invalidará las siguientes directivas individuales:

[ProxyMode](#proxymode)
[ProxyPacUrl](#proxypacurl)
[ProxyServer](#proxyserver)
[ProxyBypassList](#proxybypasslist)

El campo ProxyMode permite especificar el servidor proxy usado por Microsoft Edge e impide que los usuarios cambien la configuración de proxy.

El campo ProxyPacUrl es una dirección URL a un archivo .pac de proxy.

El campo ProxyServer es una dirección URL para el servidor proxy.

El campo ProxyBypassList es una lista de hosts del proxy que Microsoft Edge omite.

Si elige el valor 'direct' como 'ProxyMode', no se usará nunca un proxy y se ignorarán todos los demás campos.

Si elige el valor 'system' como 'ProxyMode', se usará el proxy del sistema y se ignorarán todos los demás campos.

Si elige el valor 'auto_detect' como 'ProxyMode', se ignorarán todos los demás campos.

Si elige el valor 'fixed_server' como 'ProxyMode', se usarán los campos 'ProxyServer' y 'ProxyBypassList'.

Si elige el valor 'pac_script' como 'ProxyMode', se usarán los campos 'ProxyPacUrl' y 'ProxyBypassList'.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Diccionario

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: ProxySettings
  - Nombre de la directiva de grupos: Configuración del proxy
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/Servidor proxy
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: ProxySettings
  - Tipo de valor: REG_SZ
  ##### Valor de ejemplo:
```
SOFTWARE\Policies\Microsoft\Edge\ProxySettings = {
  "ProxyBypassList": "https://www.example1.com,https://www.example2.com,https://internalsite/", 
  "ProxyMode": "direct", 
  "ProxyPacUrl": "https://internal.site/example.pac", 
  "ProxyServer": "123.123.123.123:8080"
}
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: ProxySettings
  - Valor de ejemplo:
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
  

  [Volver al principio](#microsoft-edge:-directivas)

  ## Additional policies

  [Volver al principio](#microsoft-edge:-directivas)

  ### AdsSettingForIntrusiveAdsSites
  #### Configuración de anuncios para sitios con anuncios intrusivos
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 78 o posterior

  #### Descripción
  Controla si los anuncios están bloqueados en sitios con anuncios intrusivos. Esta directiva puede establecerse en una de las siguientes opciones:

* 1 = Permitir anuncios en todos los sitios.

* 2 = Bloquear anuncios en sitios con anuncios intrusivos (valor predeterminado).

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Entero

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: AdsSettingForIntrusiveAdsSites
  - Nombre de la directiva de grupos: Configuración de anuncios para sitios con anuncios intrusivos
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: AdsSettingForIntrusiveAdsSites
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000001
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: AdsSettingForIntrusiveAdsSites
  - Valor de ejemplo:
``` xml
<integer>1</integer>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### AllowDeletingBrowserHistory
  #### Habilitar la eliminación del explorador y el historial de descarga
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Permite eliminar el historial del explorador y el historial de descarga e impide que los usuarios cambien esta configuración.

Tenga en cuenta que, incluso con esta directiva está deshabilitada, no se garantiza que se conserven los historiales de exploración y de descarga: los usuarios pueden editar o eliminar los archivos de la base de datos del historial directamente y el mismo explorador puede quitar (en función del período de expiración) o archivar alguno o todos los elementos del historial en cualquier momento.

Si se habilita esta directiva o no se configura, los usuarios podrán eliminar los historiales de exploración y de descarga.

Si se deshabilita esta directiva, los usuarios no podrán eliminar los historiales de exploración y de descarga.

Si se habilita esta directiva, no habilite la directiva "Borrar los datos de exploración al cerrar Microsoft Edge ya que ambas se ocupan de la eliminación de datos. Si se habilitan las dos, la directiva "Borrar los datos de exploración al cerrar Microsoft Edge tendrá prioridad y se eliminarán todos los datos al cerrar Microsoft Edge, independientemente de cómo se configure esta directiva.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Booleano

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: AllowDeletingBrowserHistory
  - Nombre de la directiva de grupos: Habilitar la eliminación del explorador y el historial de descarga
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: AllowDeletingBrowserHistory
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000001
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: AllowDeletingBrowserHistory
  - Valor de ejemplo:
``` xml
<true/>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### AllowFileSelectionDialogs
  #### Permitir cuadros de diálogo de selección de archivos
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Permitir el acceso a los archivos locales al permitir que Microsoft Edge muestre cuadros de diálogo de selección de archivos.

Si se habilita o no se configura esta directiva, los usuarios podrán abrir cuadros de diálogo de selección de archivos de la forma habitual.

Si se deshabilita esta directiva, cada vez que el usuario realice una acción que desencadene un cuadro de diálogo de selección de archivos (como importar favoritos, cargar archivos o guardar vínculos), aparecerá un mensaje en su lugar y se asumirá que el usuario ha hecho clic en Cancelar en el cuadro de diálogo de selección de archivos.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Booleano

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: AllowFileSelectionDialogs
  - Nombre de la directiva de grupos: Permitir cuadros de diálogo de selección de archivos
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: AllowFileSelectionDialogs
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000001
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: AllowFileSelectionDialogs
  - Valor de ejemplo:
``` xml
<true/>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### AllowPopupsDuringPageUnload
  #### Permite que una página muestre elementos emergentes durante su descarga
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 78 o posterior

  #### Descripción
  Esta directiva permite que un administrador especifique que una página pueda mostrar elementos emergentes durante su descarga.

Cuando se establece la directiva en habilitada, las páginas pueden mostrar elementos emergentes mientras se descargan.

Cuando la directiva se establece en deshabilitada o no establecida, las páginas no pueden mostrar elementos emergentes mientras se descargan. Esto se debe a las especificaciones: (https://html.spec.whatwg.org/#apis-for-creating-and-navigating-browsing-contexts-by-name).

Esta directiva se quitará en el futuro.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: No - Requiere reiniciar el explorador

  #### Tipo de datos:
  Booleano

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: AllowPopupsDuringPageUnload
  - Nombre de la directiva de grupos: Permite que una página muestre elementos emergentes durante su descarga
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: AllowPopupsDuringPageUnload
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000000
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: AllowPopupsDuringPageUnload
  - Valor de ejemplo:
``` xml
<false/>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### AllowSyncXHRInPageDismissal
  #### Permitir que las páginas envíen solicitudes sincrónicas de XHR durante el descarte de páginas
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 79 o posterior

  #### Descripción
  Esta directiva le permite especificar que una página puede enviar solicitudes sincrónicas de XHR durante el descarte de páginas.

Si habilita esta directiva, las páginas pueden enviar solicitudes sincrónicas de XHR durante el descarte de páginas.

Si deshabilita esta directiva o no la configura, las páginas no podrán enviar solicitudes sincrónicas de XHR durante el descarte de páginas.

Esta directiva es temporal y se quitará en una versión futura.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: No - Requiere reiniciar el explorador

  #### Tipo de datos:
  Booleano

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: AllowSyncXHRInPageDismissal
  - Nombre de la directiva de grupos: Permitir que las páginas envíen solicitudes sincrónicas de XHR durante el descarte de páginas
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: AllowSyncXHRInPageDismissal
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000000
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: AllowSyncXHRInPageDismissal
  - Valor de ejemplo:
``` xml
<false/>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### AllowTrackingForUrls
  #### Configurar excepciones de prevención de seguimiento para sitios específicos
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 78 o posterior

  #### Descripción
  Configurar la lista de patrones de direcciones URL que están excluidos de la prevención de seguimiento.

Si se configura esta directiva, la lista de patrones de direcciones URL configurados se excluirá de la prevención de seguimiento.

Si no se configura esta directiva, se usará el valor predeterminado global de la directiva "Bloquear el seguimiento de la actividad de exploración web de los usuarios" (si se ha establecido) o de la configuración personal del usuario para todos los sitios.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Lista de cadenas

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: AllowTrackingForUrls
  - Nombre de la directiva de grupos: Configurar excepciones de prevención de seguimiento para sitios específicos
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge\AllowTrackingForUrls
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: 1, 2, 3, ...
  - Tipo de valor: lista de REG_SZ
  ##### Valor de ejemplo:
```
SOFTWARE\Policies\Microsoft\Edge\AllowTrackingForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\AllowTrackingForUrls\1 = "[*.]contoso.edu"

```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: AllowTrackingForUrls
  - Valor de ejemplo:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### AlwaysOpenPdfExternally
  #### Abrir siempre archivos PDF externamente
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Deshabilita el visor de PDF interno en Microsoft Edge.

Si se habilita esta directiva, Microsoft Edge trata los archivos PDF como descargas y permite a los usuarios abrirlos con la aplicación predeterminada.

Si no se configura esta directiva o se deshabilita, Microsoft Edge abrirá los archivos PDF (a menos que el usuario la deshabilite).

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Booleano

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: AlwaysOpenPdfExternally
  - Nombre de la directiva de grupos: Abrir siempre archivos PDF externamente
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: AlwaysOpenPdfExternally
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000001
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: AlwaysOpenPdfExternally
  - Valor de ejemplo:
``` xml
<true/>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### ApplicationLocaleValue
  #### Establecer la configuración regional de aplicación
  >Versiones admitidas: Microsoft Edge en Windows desde la versión 77 o posterior

  #### Descripción
  Establece la configuración regional de la aplicación en Microsoft Edge e impide que los usuarios cambien la configuración regional.

Si se habilita esta directiva, Microsoft Edge usará la configuración regional especificada. Si no se admite la configuración regional configurada, se usará 'en-US' en su lugar.

Si se deshabilita o no se configuran estos ajustes, Microsoft Edge usará la configuración regional preferida especificada por el usuario (si está configurada) o la configuración regional de reserva 'en-US'.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: Sí
  - Actualización de directiva dinámica: No - Requiere reiniciar el explorador

  #### Tipo de datos:
  Cadena

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: ApplicationLocaleValue
  - Nombre de la directiva de grupos: Establecer la configuración regional de aplicación
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): Plantillas administrativas/Microsoft Edge - Configuración predeterminada (los usuarios pueden cambiarla)/
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): SOFTWARE\Policies\Microsoft\Edge\Recomendada
  - Nombre del valor: ApplicationLocaleValue
  - Tipo de valor: REG_SZ
  ##### Valor de ejemplo:
```
"en"
```


  

  [Volver al principio](#microsoft-edge:-directivas)

  ### AudioCaptureAllowed
  #### Permitir o bloquear la captura de audio
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Permite establecer si se solicita a un usuario que conceda acceso a un sitio web a su dispositivo de captura de audio. Esta directiva se aplica a todas las direcciones URL, excepto las configuradas en la lista [AudioCaptureAllowedUrls](#audiocaptureallowedurls).

Si se habilita o no se configura esta directiva (configuración predeterminada), se le pedirá al usuario acceso de captura de audio, excepto para las direcciones URL de la lista [AudioCaptureAllowedUrls](#audiocaptureallowedurls). A estas URL de la lista se les concede acceso sin pedir confirmación.

Si se deshabilita esta directiva, no se solicitará la intervención del usuario y solo se podrá tener acceso a la captura de audio en las direcciones URL configuradas en [AudioCaptureAllowedUrls](#audiocaptureallowedurls).

Esta directiva afecta a todos los tipos de entradas de audio, no solo al micrófono integrado.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Booleano

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: AudioCaptureAllowed
  - Nombre de la directiva de grupos: Permitir o bloquear la captura de audio
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: AudioCaptureAllowed
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000000
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: AudioCaptureAllowed
  - Valor de ejemplo:
``` xml
<false/>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### AudioCaptureAllowedUrls
  #### Sitios que pueden acceder a dispositivos de captura de audio sin solicitar permiso
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Especificar los sitios web, según los patrones de la dirección URL, que pueden usar dispositivos de captura de audio sin pedirle permiso al usuario. Los patrones de esta lista se comparan con el origen de la seguridad de la URL de la solicitud. Si coinciden, se concederá automáticamente acceso a los dispositivos de captura de audio.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Lista de cadenas

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: AudioCaptureAllowedUrls
  - Nombre de la directiva de grupos: Sitios que pueden acceder a dispositivos de captura de audio sin solicitar permiso
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge\AudioCaptureAllowedUrls
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: 1, 2, 3, ...
  - Tipo de valor: lista de REG_SZ
  ##### Valor de ejemplo:
```
SOFTWARE\Policies\Microsoft\Edge\AudioCaptureAllowedUrls\0 = "https://www.contoso.com/"
SOFTWARE\Policies\Microsoft\Edge\AudioCaptureAllowedUrls\1 = "https://[*.]contoso.edu/"

```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: AudioCaptureAllowedUrls
  - Valor de ejemplo:
``` xml
<array>
  <string>https://www.contoso.com/</string>
  <string>https://[*.]contoso.edu/</string>
</array>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### AutoImportAtFirstRun
  #### Importar automáticamente los datos y la configuración de otro explorador la primera vez que se ejecute
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Si se habilita esta directiva, Microsoft Edge importa automáticamente todos los tipos de datos y configuraciones admitidos desde el explorador predeterminado u otro explorador especificado. Esto también obliga a Microsoft Edge a omitir la sección de importación de la primera experiencia de ejecución.

Si se establece esta directiva en 'DisabledAutoImport' (4), la sección de importación de la primera experiencia de ejecución se omite por completo y Microsoft Edge no importa la configuración y los datos del explorador automáticamente.

* 0 = Importa automáticamente todos los tipos de datos y configuraciones admitidos del explorador predeterminado

* 1 = Importa automáticamente todos los tipos de datos y configuraciones admitidos de Internet Explorer

* 2 = Importa automáticamente todos los tipos de datos y configuraciones admitidos de Google Chrome

* 3 = Importa automáticamente todos los tipos de datos y configuraciones admitidos de Safari

* 4 = Deshabilita la importación automática y se omite la sección de importación de la experiencia de la primera ejecución

**Nota**: Actualmente, esta directiva es compatible con la importación desde los exploradores Internet Explorer (en Windows 7, 8 y 10), Google Chrome (en Windows 7, 8 y 10 y en macOS) y Apple Safari (en macOS).

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: No - Requiere reiniciar el explorador

  #### Tipo de datos:
  Entero

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: AutoImportAtFirstRun
  - Nombre de la directiva de grupos: Importar automáticamente los datos y la configuración de otro explorador la primera vez que se ejecute
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: AutoImportAtFirstRun
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000002
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: AutoImportAtFirstRun
  - Valor de ejemplo:
``` xml
<integer>2</integer>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### AutofillAddressEnabled
  #### Habilitar Autorrellenar para direcciones
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Habilita la característica de Autorrellenar y permite a los usuarios rellenar automáticamente la información de dirección en formularios web con información previamente almacenada.

Si se deshabilita esta directiva, Autorrellenar nunca sugiere o escribe información sobre la dirección ni guarda información adicional sobre la dirección que el usuario podría enviar durante la exploración web.

Si se habilita esta directiva o no se configura, los usuarios pueden controlar Autorrellenar para direcciones en la interfaz de usuario.

Tenga en cuenta que si se deshabilita esta directiva, también se detendrán todas las actividades de todos los formularios web, excepto los formularios de pago y contraseña. No se guardarán más entradas y Microsoft Edge no sugerirá ni rellenará automáticamente las entradas anteriores.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: Sí
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Booleano

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: AutofillAddressEnabled
  - Nombre de la directiva de grupos: Habilitar Autorrellenar para direcciones
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): Plantillas administrativas/Microsoft Edge - Configuración predeterminada (los usuarios pueden cambiarla)/
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): SOFTWARE\Policies\Microsoft\Edge\Recomendada
  - Nombre del valor: AutofillAddressEnabled
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000000
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: AutofillAddressEnabled
  - Valor de ejemplo:
``` xml
<false/>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### AutofillCreditCardEnabled
  #### Habilitar Autorrellenar para tarjetas de crédito
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Habilita la característica Autorrellenar de Microsoft Edge y permite a los usuarios rellenar de forma automática la información de tarjetas de crédito en formularios web con la información almacenada anteriormente.

Si se deshabilita esta directiva, Autorrellenar nunca sugerirá ni rellenará la información de tarjetas de crédito y tampoco guardará la información adicional de estas que los usuarios podrían enviar al explorar la web.

Si se habilita o no se configura esta directiva, los usuarios pueden controlar la característica Autorrellenar para tarjetas de crédito.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: Sí
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Booleano

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: AutofillCreditCardEnabled
  - Nombre de la directiva de grupos: Habilitar Autorrellenar para tarjetas de crédito
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): Plantillas administrativas/Microsoft Edge - Configuración predeterminada (los usuarios pueden cambiarla)/
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): SOFTWARE\Policies\Microsoft\Edge\Recomendada
  - Nombre del valor: AutofillCreditCardEnabled
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000000
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: AutofillCreditCardEnabled
  - Valor de ejemplo:
``` xml
<false/>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### AutoplayAllowed
  #### Permitir la reproducción automática de multimedia para sitios web
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 78 o posterior

  #### Descripción
  Esta directiva establece la directiva de reproducción automática de multimedia para sitios web.

La configuración predeterminada, "No configurado" respeta la configuración actual de reproducción automática de multimedia y permite a los usuarios configurar su configuración de reproducción automática.

Al establecer la opción "Habilitado", la reproducción automática de multimedia se establece en "Permitir".  Todos los sitios web tienen permiso para reproducir contenido multimedia. Los usuarios no pueden invalidar esta directiva.

Si se establece la opción "Deshabilitado", la reproducción automática de multimedia se establece en "Bloquear".  Ningún sitio web tiene permiso para reproducir contenido multimedia. Los usuarios no pueden invalidar esta directiva.

Es necesario cerrar una pestaña y volver a abrirla para que esta directiva surta efecto.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Booleano

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: AutoplayAllowed
  - Nombre de la directiva de grupos: Permitir la reproducción automática de multimedia para sitios web
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: AutoplayAllowed
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000001
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: AutoplayAllowed
  - Valor de ejemplo:
``` xml
<true/>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### BackgroundModeEnabled
  #### Continúa con la ejecución de aplicaciones en segundo plano después de cerrar Microsoft Edge
  >Versiones admitidas: Microsoft Edge en Windows desde la versión 77 o posterior

  #### Descripción
  Permite que los procesos de Microsoft Edge comiencen con el inicio de sesión del sistema operativo y sigan ejecutándose cuando se cierre la última ventana del navegador. En este escenario, las aplicaciones en segundo plano y la sesión de exploración actual permanecen activas, incluidas las cookies de la sesión. Un proceso abierto en segundo plano muestra un icono en la bandeja del sistema y siempre se puede cerrar desde allí.

Si se habilita esta directiva, se activará el modo de segundo plano.

Si se deshabilita esta directiva, se desactivará el modo de segundo plano.

Si no se configura esta directiva, el modo de segundo plano estará desactivado inicialmente y el usuario puede configurar su comportamiento en edge://settings/system.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: Sí
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Booleano

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: BackgroundModeEnabled
  - Nombre de la directiva de grupos: Continúa con la ejecución de aplicaciones en segundo plano después de cerrar Microsoft Edge
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): Plantillas administrativas/Microsoft Edge - Configuración predeterminada (los usuarios pueden cambiarla)/
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): SOFTWARE\Policies\Microsoft\Edge\Recomendada
  - Nombre del valor: BackgroundModeEnabled
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000001
```


  

  [Volver al principio](#microsoft-edge:-directivas)

  ### BackgroundTemplateListUpdatesEnabled
  #### Habilita actualizaciones en segundo plano para la lista de plantillas disponibles para Colecciones y otras características que usan plantillas.
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 79 o posterior

  #### Descripción
  Permite habilitar o deshabilitar las actualizaciones en segundo plano de la lista de plantillas disponibles para Colecciones y otras características que usan plantillas. Las plantillas se usan para extraer metadatos enriquecidos de una página web cuando la página se guarda en una colección.

Si habilita esta configuración o si la configuración no está configurada, la lista de plantillas disponibles se descargará en segundo plano desde un servicio Microsoft cada 24 horas.

Si deshabilita esta configuración, la lista de plantillas disponibles se descargará a petición. Este tipo de descarga puede dar lugar a pequeñas penalizaciones de rendimiento para Colecciones y otras características.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Booleano

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: BackgroundTemplateListUpdatesEnabled
  - Nombre de la directiva de grupos: Habilita actualizaciones en segundo plano para la lista de plantillas disponibles para Colecciones y otras características que usan plantillas.
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: BackgroundTemplateListUpdatesEnabled
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000001
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: BackgroundTemplateListUpdatesEnabled
  - Valor de ejemplo:
``` xml
<true/>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### BlockThirdPartyCookies
  #### Bloquear cookies de terceros
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Bloquee los elementos de la página web que no pertenezcan al dominio que se encuentra en la barra de direcciones del establecimiento de cookies.

Si habilita esta directiva, los elementos de la página web que no pertenecen al dominio que se encuentra en la barra de direcciones no podrán establecer cookies

Si deshabilita esta directiva, los elementos de la página web de otros dominios que no se encuentran en la barra de direcciones podrán establecer cookies.

Si no configura esta directiva, las cookies de terceros están habilitadas, pero los usuarios podrán cambiar esta configuración.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: Sí
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Booleano

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: BlockThirdPartyCookies
  - Nombre de la directiva de grupos: Bloquear cookies de terceros
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): Plantillas administrativas/Microsoft Edge - Configuración predeterminada (los usuarios pueden cambiarla)/
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): SOFTWARE\Policies\Microsoft\Edge\Recomendada
  - Nombre del valor: BlockThirdPartyCookies
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000000
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: BlockThirdPartyCookies
  - Valor de ejemplo:
``` xml
<false/>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### BrowserAddProfileEnabled
  #### Habilitar la creación de perfiles desde el menú desplegable Identidad o la página de configuración
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Permitir a los usuarios crear nuevos perfiles mediante la opción **Agregar perfil**.
Si se habilita esta directiva o no se configura, Microsoft Edge permite a los usuarios usar **Agregar perfil** en el menú flotante de identidad o en la página de configuración para crear nuevos perfiles.

Si se deshabilita esta directiva, los usuarios no podrán agregar nuevos perfiles desde el menú flotante de identidad o desde la página de configuración.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Booleano

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: BrowserAddProfileEnabled
  - Nombre de la directiva de grupos: Habilitar la creación de perfiles desde el menú desplegable Identidad o la página de configuración
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: BrowserAddProfileEnabled
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000001
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: BrowserAddProfileEnabled
  - Valor de ejemplo:
``` xml
<true/>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### BrowserGuestModeEnabled
  #### Habilitar el modo Invitado
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Habilita la opción de permitir el uso de perfiles de invitados en Microsoft Edge. En un perfil de invitado, el explorador no importa los datos de exploración de los perfiles existentes y elimina los datos de exploración cuando se cierran todos los perfiles de invitados.

Si se habilita esta directiva o no se configura, Microsoft Edge permite a los usuarios examinar los perfiles de invitados.

Si se deshabilita esta directiva, Microsoft Edge no permite a los usuarios examinar los perfiles de invitados.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Booleano

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: BrowserGuestModeEnabled
  - Nombre de la directiva de grupos: Habilitar el modo Invitado
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: BrowserGuestModeEnabled
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000001
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: BrowserGuestModeEnabled
  - Valor de ejemplo:
``` xml
<true/>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### BrowserNetworkTimeQueriesEnabled
  #### Permitir consultas a un servicio de hora de red de explorador
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Impide que Microsoft Edge envíe consultas ocasionalmente a un servicio de hora de la red de explorador para recuperar una marca de tiempo precisa.

Si se deshabilita esta directiva, Microsoft Edge dejará de enviar consultas a un servicio de hora de la red de explorador.

Si se habilita esta directiva o no se configura, Microsoft Edge enviará consultas ocasionalmente a un servicio de hora de la red de explorador.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Booleano

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: BrowserNetworkTimeQueriesEnabled
  - Nombre de la directiva de grupos: Permitir consultas a un servicio de hora de red de explorador
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: BrowserNetworkTimeQueriesEnabled
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000001
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: BrowserNetworkTimeQueriesEnabled
  - Valor de ejemplo:
``` xml
<true/>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### BrowserSignin
  #### Configuración de inicio de sesión del explorador
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Especifica si un usuario puede iniciar sesión en Microsoft Edge con su cuenta y usar los servicios relacionados con la cuenta, como sincronizar e inicio de sesión único. Para controlar la disponibilidad de la sincronización, use la directiva [SyncDisabled](#syncdisabled) en su lugar.

Si se establece esta directiva en 'Deshabilitar el inicio de sesión del explorador', asegúrese de que también establece la directiva [NonRemovableProfileEnabled](#nonremovableprofileenabled) en Deshabilitado porque [NonRemovableProfileEnabled](#nonremovableprofileenabled) deshabilita la creación de un perfil del explorador con sesión iniciada automáticamente. Si se establecen las dos directivas, Microsoft Edge usará la directiva 'Deshabilitar el inicio de sesión del explorador', y se comportará como si [NonRemovableProfileEnabled](#nonremovableprofileenabled) estuviese establecida en Deshabilitado.

Si se establece esta directiva en 'Habilitar inicio de sesión del explorador' (1), los usuarios podrán iniciar sesión en el explorador. Iniciar sesión en el explorador no significa que la sincronización esté activada de manera predeterminada; el usuario debe participar por separado para usar esta característica.

Si se establece esta directiva en "Forzar inicio de sesión del explorador" (2), los usuarios deberán iniciar sesión en un perfil para usar el explorador. De manera predeterminada, esto permitirá al usuario elegir si desea sincronizar con su cuenta, a menos que el administrador del dominio o la directiva [SyncDisabled](#syncdisabled). deshabiliten la sincronización. El valor predeterminado de la directiva [BrowserGuestModeEnabled](#browserguestmodeenabled) se ha establecido en false.

Si no se configura esta directiva, los usuarios podrán decidir si desean habilitar la opción de inicio de sesión del explorador y usarla como consideren adecuado.

* 0 = Deshabilitar inicio de sesión en el explorador

* 1 = Habilitar inicio de sesión en el explorador

* 2 = Obligar a los usuarios a iniciar sesión para usar el explorador

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: No - Requiere reiniciar el explorador

  #### Tipo de datos:
  Entero

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: BrowserSignin
  - Nombre de la directiva de grupos: Configuración de inicio de sesión del explorador
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: BrowserSignin
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000002
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: BrowserSignin
  - Valor de ejemplo:
``` xml
<integer>2</integer>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### BuiltInDnsClientEnabled
  #### Usar el cliente DNS integrado
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Controla si se debe usar el cliente DNS integrado.

Si habilita esta directiva, se usará el cliente DNS integrado, si está disponible.

Si deshabilita esta directiva, el cliente no se usará nunca.

Si no configura esta directiva, el cliente DNS integrado se habilitará de manera predeterminada en MacOS y los usuarios podrán cambiar si deben usar el cliente DNS integrado editando edge://flags o especificando una marca de línea de comandos.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Booleano

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: BuiltInDnsClientEnabled
  - Nombre de la directiva de grupos: Usar el cliente DNS integrado
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: BuiltInDnsClientEnabled
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000001
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: BuiltInDnsClientEnabled
  - Valor de ejemplo:
``` xml
<true/>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### CertificateTransparencyEnforcementDisabledForCas
  #### Deshabilitar el cumplimiento de la transparencia de certificados para obtener una lista de hashes subjectPublicKeyInfo
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Deshabilita la aplicación de los requisitos de transparencia de certificado para una lista de hash de subjectPublicKeyInfo.

Esta directiva te permite deshabilitar los requisitos de divulgación de la transparencia de certificados para cadenas de certificados que contienen certificados con uno de los hash de subjectPublicKeyInfo especificados. Esto permite que los certificados que, de lo contrario, no serían de confianza porque no se habían divulgado correctamente, se puedan usar en los hosts de Enterprise.

Para deshabilitar la aplicación de la transparencia de certificados cuando se establece esta directiva, se debe cumplir uno de los siguientes conjuntos de condiciones:
1. El hash es de la subjectPublicKeyInfo del certificado del servidor.
2. El hash es de una subjectPublicKeyInfo que aparece en un Certificado CA de la cadena de certificados, este Certificado CA está restringido mediante la extensión nameConstraints X.509v3, uno o varios nameConstraints de directoryName están presentes en los permittedSubtrees y el directoryName contiene un atributo de organizationName.
3. El hash es de una subjectPublicKeyInfo que aparece en un Certificado CA de la cadena de certificados, el Certificado CA tiene uno o más atributos de organizationName en el asunto del certificado y el certificado del servidor contiene el mismo número de atributos de organizationName, en el mismo orden y con valores idénticos byte por byte.

Un hash de subjectPublicKeyInfo se especifica concatenando el nombre del algoritmo hash, el carácter "/" y la codificación Base64 de dicho algoritmo hash aplicado a la subjectPublicKeyInfo codificada con DER del certificado especificado. Esta codificación Base64 tiene el mismo formato que una huella digital SPKI, como se define en la sección 2.4 de RFC 7469. Los algoritmos hash no reconocidos se omiten. El único algoritmo hash admitido en este momento es "SHA256".

Si se deshabilita esta directiva o no se configura, cualquier certificado que deba ser divulgado a través de la transparencia del certificado se tratará como de no confianza si no se divulga de acuerdo con la directiva de transparencia del certificado.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Lista de cadenas

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: CertificateTransparencyEnforcementDisabledForCas
  - Nombre de la directiva de grupos: Deshabilitar el cumplimiento de la transparencia de certificados para obtener una lista de hashes subjectPublicKeyInfo
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge\CertificateTransparencyEnforcementDisabledForCas
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: 1, 2, 3, ...
  - Tipo de valor: lista de REG_SZ
  ##### Valor de ejemplo:
```
SOFTWARE\Policies\Microsoft\Edge\CertificateTransparencyEnforcementDisabledForCas\0 = "sha256/AAAAAAAAAAAAAAAAAAAAAA=="
SOFTWARE\Policies\Microsoft\Edge\CertificateTransparencyEnforcementDisabledForCas\1 = "sha256//////////////////////w=="

```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: CertificateTransparencyEnforcementDisabledForCas
  - Valor de ejemplo:
``` xml
<array>
  <string>sha256/AAAAAAAAAAAAAAAAAAAAAA==</string>
  <string>sha256//////////////////////w==</string>
</array>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### CertificateTransparencyEnforcementDisabledForLegacyCas
  #### Deshabilitar la aplicación de la transparencia de certificados para una lista de entidades de certificación heredadas
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Deshabilita la aplicación de los requisitos de transparencia de certificado para una lista de entidades de certificación (CA) heredadas.

Esta directiva permite deshabilitar los requisitos de divulgación de la transparencia de certificados para cadenas de certificados que contienen certificados con uno de los hash de subjectPublicKeyInfo especificados. Esto permite que los certificados que de otro modo no eran de confianza debido a que no se divulgaran correctamente, sigan usándose para los hosts de la empresa.

Para que la aplicación de la transparencia se deshabilite, debe establecer el algoritmo hash en un subjectPublicKeyInfo que aparezca en un Certificado CA reconocido como una entidad de certificación (CA) heredada. Una CA heredada es una CA de confianza pública de forma predeterminada por parte de uno o varios sistemas operativos compatibles con Microsoft Edge.

Puede especificar un hash subjectPublicKeyInfo concatenando el nombre del algoritmo hash, el carácter "/" y la codificación Base64 de ese algoritmo hash aplicado a la subjectPublicKeyInfo codificada con DER del certificado especificado. Esta codificación Base64 tiene el mismo formato que una huella digital SPKI, como se define en la sección 2,4 de RFC 7469. Se omiten los algoritmos hash no reconocidos. El único algoritmo hash admitido en este momento es "SHA256".

Si no se configuras esta directiva, todos los certificados que se deban divulgar a través de la transparencia de certificados se tratarán como no de confianza si no se divulgan según la directiva de transparencia de certificados.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Lista de cadenas

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: CertificateTransparencyEnforcementDisabledForLegacyCas
  - Nombre de la directiva de grupos: Deshabilitar la aplicación de la transparencia de certificados para una lista de entidades de certificación heredadas
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge\CertificateTransparencyEnforcementDisabledForLegacyCas
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: 1, 2, 3, ...
  - Tipo de valor: lista de REG_SZ
  ##### Valor de ejemplo:
```
SOFTWARE\Policies\Microsoft\Edge\CertificateTransparencyEnforcementDisabledForLegacyCas\0 = "sha256/AAAAAAAAAAAAAAAAAAAAAA=="
SOFTWARE\Policies\Microsoft\Edge\CertificateTransparencyEnforcementDisabledForLegacyCas\1 = "sha256//////////////////////w=="

```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: CertificateTransparencyEnforcementDisabledForLegacyCas
  - Valor de ejemplo:
``` xml
<array>
  <string>sha256/AAAAAAAAAAAAAAAAAAAAAA==</string>
  <string>sha256//////////////////////w==</string>
</array>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### CertificateTransparencyEnforcementDisabledForUrls
  #### Deshabilitar el cumplimiento de transparencia de certificados para direcciones URL específicas
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Se deshabilitan los requisitos de transparencia de certificado para las direcciones URL que aparecen en la lista.

Esta directiva te permite no divulgar certificados para los nombres de host en la dirección URL a través de la transparencia del certificado. Esto te permitirá usar certificados que, de lo contrario, no serían de confianza, debido a que no se divulgaron públicamente de manera correcta, pero resulta más difícil de detectar los certificados que no se emitieron correctamente para estos hosts.

Forma el patrón de las direcciones URL según [https://go.microsoft.com/fwlink/?linkid=2095322](https://go.microsoft.com/fwlink/?linkid=2095322). Como los certificados son válidos para un nombre de host determinado, independientemente del esquema, el puerto o la ruta de acceso, solo se tendrá en cuenta la parte del nombre de host de la dirección URL. No se admiten hosts comodín.

Si no configuras esta directiva, todos los certificados que deberían divulgarse a través de la transparencia del certificado se tratarán como no de confianza si no se divulgan.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Lista de cadenas

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: CertificateTransparencyEnforcementDisabledForUrls
  - Nombre de la directiva de grupos: Deshabilitar el cumplimiento de transparencia de certificados para direcciones URL específicas
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge\CertificateTransparencyEnforcementDisabledForUrls
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: 1, 2, 3, ...
  - Tipo de valor: lista de REG_SZ
  ##### Valor de ejemplo:
```
SOFTWARE\Policies\Microsoft\Edge\CertificateTransparencyEnforcementDisabledForUrls\0 = "contoso.com"
SOFTWARE\Policies\Microsoft\Edge\CertificateTransparencyEnforcementDisabledForUrls\1 = ".contoso.com"

```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: CertificateTransparencyEnforcementDisabledForUrls
  - Valor de ejemplo:
``` xml
<array>
  <string>contoso.com</string>
  <string>.contoso.com</string>
</array>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### ClearBrowsingDataOnExit
  #### Borrar los datos de exploración al cerrar Microsoft Edge
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 78 o posterior

  #### Descripción
  Microsoft Edge no borra los datos de exploración de manera predeterminada cuando se cierra. Los datos de exploración incluyen información escrita en formularios, contraseñas e incluso los sitios web visitados.

Si se habilita esta directiva, todos los datos de exploración se eliminan cada vez que se cierra Microsoft Edge.

Si se deshabilita o no se configura esta directiva, los usuarios podrán configurar la opción Borrar datos de exploración en Configuración.

Si habilita esta directiva, no habilite la directiva [AllowDeletingBrowserHistory](#allowdeletingbrowserhistory), ya que ambas se ocupan de eliminar datos. Si habilita ambas, esta directiva tendrá prioridad y eliminará todos los datos cuando Microsoft Edge se cierre, independientemente de cómo haya configurado [AllowDeletingBrowserHistory](#allowdeletingbrowserhistory).

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: Sí
  - Actualización de directiva dinámica: No - Requiere reiniciar el explorador

  #### Tipo de datos:
  Booleano

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: ClearBrowsingDataOnExit
  - Nombre de la directiva de grupos: Borrar los datos de exploración al cerrar Microsoft Edge
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): Plantillas administrativas/Microsoft Edge - Configuración predeterminada (los usuarios pueden cambiarla)/
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): SOFTWARE\Policies\Microsoft\Edge\Recomendada
  - Nombre del valor: ClearBrowsingDataOnExit
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000001
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: ClearBrowsingDataOnExit
  - Valor de ejemplo:
``` xml
<true/>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### ClickOnceEnabled
  #### Permitir a los usuarios abrir archivos con el protocolo ClickOnce
  >Versiones admitidas: Microsoft Edge en Windows desde la versión 78 o posterior

  #### Descripción
  Permitir a los usuarios abrir archivos con el protocolo ClickOnce. El protocolo ClickOnce permite a los sitios web solicitar que el explorador abra archivos de una dirección URL específica mediante el controlador de archivos de ClickOnce del equipo o dispositivo del usuario.

Si se habilita esta directiva, los usuarios pueden abrir archivos con el protocolo ClickOnce. Esta directiva invalida la configuración de ClickOnce del usuario en la página edge://flags/.

Si se deshabilita esta directiva, los usuarios no podrán abrir archivos con el protocolo ClickOnce. En su lugar, el archivo se guardará en el sistema de archivos usando el explorador. Esta directiva invalida la configuración de ClickOnce del usuario en la página edge://flags/.

Si no se configura esta directiva, los usuarios no podrán abrir archivos con el protocolo ClickOnce. Los usuarios tienen la opción de habilitar el uso del protocolo ClickOnce usando la página edge://flags/.

La deshabilitación de ClickOnce puede impedir que las aplicaciones ClickOnce (.application files) se inicien correctamente.

Para obtener más información sobre ClickOnce, consulte [https://go.microsoft.com/fwlink/?linkid=2103872](https://go.microsoft.com/fwlink/?linkid=2103872) y [https://go.microsoft.com/fwlink/?linkid=2099880](https://go.microsoft.com/fwlink/?linkid=2099880).

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Booleano

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: ClickOnceEnabled
  - Nombre de la directiva de grupos: Permitir a los usuarios abrir archivos con el protocolo ClickOnce
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: ClickOnceEnabled
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000000
```


  

  [Volver al principio](#microsoft-edge:-directivas)

  ### CommandLineFlagSecurityWarningsEnabled
  #### Habilitar advertencias de seguridad para marcadores de la línea de comandos
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 78 o posterior

  #### Descripción
  Si se deshabilita, esta directiva impide que las advertencias de seguridad aparezcan cuando Microsoft Edge se inicie con marcas de línea de comandos potencialmente peligrosas.

Si se habilita o no se establece esta opción, se muestran advertencias de seguridad cuando se usan estas marcas de línea de comandos para iniciar Microsoft Edge.

Por ejemplo, la marca--Disable-GPU-Sandbox genera esta advertencia: Está usando una marca de línea de comandos no admitida: --disable-gpu-sandbox. Esto supone un riesgo de seguridad y de estabilidad.

En Windows, esta directiva solo está disponible en las instancias que están unidas a un dominio de Microsoft Active Directory o a las instancias de Windows 10 Pro (o Enterprise) que están inscritas para la administración de dispositivos.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: No - Requiere reiniciar el explorador

  #### Tipo de datos:
  Booleano

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: CommandLineFlagSecurityWarningsEnabled
  - Nombre de la directiva de grupos: Habilitar advertencias de seguridad para marcadores de la línea de comandos
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: CommandLineFlagSecurityWarningsEnabled
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000001
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: CommandLineFlagSecurityWarningsEnabled
  - Valor de ejemplo:
``` xml
<true/>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### ComponentUpdatesEnabled
  #### Habilitar actualizaciones de componentes en Microsoft Edge
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Si se habilita o no se configura esta directiva, las actualizaciones de componentes estarán habilitadas en Microsoft Edge.

Si se deshabilita esta directiva o se establece en false, se deshabilitarán las actualizaciones de componentes para todos los componentes de Microsoft Edge.

Sin embargo, algunos componentes están exentos de esta directiva. Esto incluye todos los componentes que no contengan código ejecutable, que no modifica significativamente el comportamiento del explorador o que es crítico para la seguridad. Es decir, las actualizaciones que se consideran "críticas para la seguridad" se siguen aplicando incluso si se deshabilita esta directiva.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: No - Requiere reiniciar el explorador

  #### Tipo de datos:
  Booleano

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: ComponentUpdatesEnabled
  - Nombre de la directiva de grupos: Habilitar actualizaciones de componentes en Microsoft Edge
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: ComponentUpdatesEnabled
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000001
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: ComponentUpdatesEnabled
  - Valor de ejemplo:
``` xml
<true/>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### ConfigureDoNotTrack
  #### Configurar No realizar seguimiento
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Especifique si quiere enviar solicitudes de No realizar seguimiento a sitios web que pidan información de seguimiento. Las solicitudes de No realizar seguimiento permiten que los sitios web que visite sepan que no quiere que se realice un seguimiento de su actividad de exploración. De manera predeterminada, Microsoft Edge no enviará solicitudes de No realizar seguimiento, pero los usuarios pueden activar esta característica para enviarlas.

Si se habilita esta directiva, siempre se enviarán solicitudes de No realizar seguimiento a los sitios web que pidan información de seguimiento.

Si se deshabilita esta directiva, nunca se enviarán solicitudes.

Si no se configura esta directiva, los usuarios podrán elegir si quieren enviar estas solicitudes.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Booleano

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: ConfigureDoNotTrack
  - Nombre de la directiva de grupos: Configurar No realizar seguimiento
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: ConfigureDoNotTrack
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000000
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: ConfigureDoNotTrack
  - Valor de ejemplo:
``` xml
<false/>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### ConfigureOnlineTextToSpeech
  #### Configurar texto a voz en línea
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Establecer si el explorador puede sacar provecho de las fuentes de voz de Texto a voz en línea, parte de Azure Cognitive Services. Estas fuentes de voz son de mejor calidad que las fuentes de voz del sistema instaladas previamente.

Si se habilita o no se configura esta directiva, las aplicaciones basadas en web que usan la API SpeechSynthesis podrán usar las fuentes de voz de Texto a voz en línea.

Si se deshabilita esta directiva, las fuentes de voz no estarán disponibles.

Obtenga más información acerca de esta característica aquí:
SpeechSynthesis API: [https://go.microsoft.com/fwlink/?linkid=2110038](https://go.microsoft.com/fwlink/?linkid=2110038)
Cognitive Services: [https://go.microsoft.com/fwlink/?linkid=2110141](https://go.microsoft.com/fwlink/?linkid=2110141)

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Booleano

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: ConfigureOnlineTextToSpeech
  - Nombre de la directiva de grupos: Configurar texto a voz en línea
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: ConfigureOnlineTextToSpeech
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000001
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: ConfigureOnlineTextToSpeech
  - Valor de ejemplo:
``` xml
<true/>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### CustomHelpLink
  #### Especificar vínculo de ayuda personalizado
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 79 o posterior

  #### Descripción
  Especificar un vínculo para el menú Ayuda o la tecla F1.

Si se habilita esta directiva, un administrador puede especificar un vínculo para el menú Ayuda o la tecla F1.

Si se deshabilita o no se configura esta directiva, se usará el vínculo predeterminado para el menú Ayuda o la tecla F1.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Cadena

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: CustomHelpLink
  - Nombre de la directiva de grupos: Especificar vínculo de ayuda personalizado
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: CustomHelpLink
  - Tipo de valor: REG_SZ
  ##### Valor de ejemplo:
```
"https://go.microsoft.com/fwlink/?linkid=2080734"
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: CustomHelpLink
  - Valor de ejemplo:
``` xml
<string>https://go.microsoft.com/fwlink/?linkid=2080734</string>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### DefaultBrowserSettingEnabled
  #### Establecer Microsoft Edge como el explorador predeterminado
  >Versiones admitidas: Microsoft Edge en Windows 7 y Mac desde la versión 77 o posterior

  #### Descripción
  Configura las comprobaciones de explorador predeterminado en Microsoft Edge e impide que los usuarios las modifiquen.

Si se habilita esta directiva, Microsoft Edge comprobará siempre al iniciarse si es el explorador predeterminado y se registrará automáticamente, si es posible.

Si se deshabilita esta directiva, Microsoft Edge nunca comprobará y se deshabilitarán los controles de usuario para configurar esta opción.

Si no se configura esta directiva, Microsoft Edge permitirá al usuario controlar si es el explorador predeterminado y si desea mostrar notificaciones de usuario cuando no lo es.

Nota para los administradores de Windows: Esta directiva solo funciona en equipos que tengan Windows 7. Para versiones posteriores de Windows, deberá implementar un archivo de "asociaciones de aplicaciones predeterminadas" que hará que Microsoft Edge ea el controlador para los protocolos https y http (y, opcionalmente, el protocolo ftp y formatos de archivo como .html, .htm, .pdf, .svg, .webp). Consulte [https://go.microsoft.com/fwlink/?linkid=2094932](https://go.microsoft.com/fwlink/?linkid=2094932) para obtener más información.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Booleano

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: DefaultBrowserSettingEnabled
  - Nombre de la directiva de grupos: Establecer Microsoft Edge como el explorador predeterminado
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: DefaultBrowserSettingEnabled
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000001
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: DefaultBrowserSettingEnabled
  - Valor de ejemplo:
``` xml
<true/>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### DeveloperToolsAvailability
  #### Controlar dónde se pueden usar las herramientas de desarrollo
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Controle dónde se pueden usar las herramientas de desarrollo.

Si establece esta directiva en 'DeveloperToolsDisallowedForForceInstalledExtensions' (0, valor predeterminado), los usuarios podrán acceder a las herramientas de desarrollo y la consola de JavaScript en general, pero no en el contexto de extensiones instaladas por la directiva de empresa.

Si establece esta directiva en 'DeveloperToolsAllowed' (1), los usuarios podrán acceder a las herramientas de desarrollo y la consola de JavaScript en todos los contextos, incluidas las extensiones instaladas por la directiva de empresa.

Si establece esta directiva en 'DeveloperToolsDisallowed' (2), los usuarios no podrán acceder a las herramientas de desarrollo ni inspeccionar los elementos del sitio web. Los métodos abreviados de teclado y las entradas de menú o de menú contextual que abren las herramientas de desarrollo o la consola de JavaScript se deshabilitarán.

* 0 = Bloquear las herramientas de desarrollo en las extensiones instaladas por la directiva de empresa, permitir en otros contextos

* 1 = Permitir el uso de las herramientas de desarrollo

* 2 = No permitir el uso de las herramientas de desarrollo

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Entero

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: DeveloperToolsAvailability
  - Nombre de la directiva de grupos: Controlar dónde se pueden usar las herramientas de desarrollo
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: DeveloperToolsAvailability
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000002
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: DeveloperToolsAvailability
  - Valor de ejemplo:
``` xml
<integer>2</integer>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### DirectInvokeEnabled
  #### Permitir a los usuarios abrir archivos con el protocolo DirectInvoke
  >Versiones admitidas: Microsoft Edge en Windows desde la versión 78 o posterior

  #### Descripción
  Permitir a los usuarios abrir archivos con el protocolo DirectInvoke. El protocolo DirectInvoke permite a los sitios web solicitar que el explorador abra archivos de una dirección URL específica mediante un controlador de archivos específico en el equipo o dispositivo del usuario.

Si habilitas o no configuras esta Directiva, los usuarios podrán abrir archivos con el protocolo DirectInvoke.

Si deshabilita esta Directiva, los usuarios no podrán abrir archivos con el protocolo DirectInvoke. En su lugar, el archivo se guardará en el sistema de archivos.

Nota: Si deshabilita DirectInvoke, es posible que algunas características de Microsoft Office SharePoint Online no funcionen según lo esperado.

Para obtener más información acerca de DirectInvoke, consulte [https://go.microsoft.com/fwlink/?linkid=2103872](https://go.microsoft.com/fwlink/?linkid=2103872) y [https://go.microsoft.com/fwlink/?linkid=2099871](https://go.microsoft.com/fwlink/?linkid=2099871).

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Booleano

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: DirectInvokeEnabled
  - Nombre de la directiva de grupos: Permitir a los usuarios abrir archivos con el protocolo DirectInvoke
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: DirectInvokeEnabled
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000000
```


  

  [Volver al principio](#microsoft-edge:-directivas)

  ### Disable3DAPIs
  #### Deshabilitar el soporte de las API de gráficos 3D
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Impedir que las páginas web tengan acceso a la unidad de procesamiento gráfico (GPU). Más concretamente, las páginas web no podrán obtener acceso a la API WebGL y los complementos no podrán usar la API 3D Pepper.

Si no se configura ni se deshabilita esta directiva, podría permitir que las páginas web usen la API WebGL y complementos para usar la API 3D Pepper. Microsoft Edge, de manera predeterminada, aún pueden necesitar los argumentos de línea de comandos que se pasarán para poder usar estas API.

Si la directiva [HardwareAccelerationModeEnabled](#hardwareaccelerationmodeenabled) está establecida en false, se omitirá la configuración de la directiva 'Disable3DAPIs': es el equivalente a establecer la directiva 'Disable3DAPIs' en true.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Booleano

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: Disable3DAPIs
  - Nombre de la directiva de grupos: Deshabilitar el soporte de las API de gráficos 3D
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: Disable3DAPIs
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000000
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: Disable3DAPIs
  - Valor de ejemplo:
``` xml
<false/>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### DisableScreenshots
  #### Deshabilitar la captura de pantalla
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Controla si los usuarios pueden tomar capturas de pantalla de la página del explorador.

Si habilita esta opción, el usuario no podrá tomar capturas de pantalla mediante los métodos abreviados de teclado o las API de extensión.

Si deshabilita o no configura esta directiva, los usuarios podrán tomar capturas de pantalla.

Tenga en cuenta que esta directiva controla las capturas de pantalla que se toman desde el propio explorador. Aunque habilite esta directiva, los usuarios aún podrán tomar capturas de pantalla con algún método fuera del explorador (por ejemplo, mediante una función del sistema operativo u otra aplicación).

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Booleano

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: DisableScreenshots
  - Nombre de la directiva de grupos: Deshabilitar la captura de pantalla
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: DisableScreenshots
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000001
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: DisableScreenshots
  - Valor de ejemplo:
``` xml
<true/>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### DiskCacheDir
  #### Establecer el directorio de memoria caché del disco
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Configura el directorio que se va a usar para almacenar archivos en caché.

Si se habilita esta directiva, Microsoft Edge usará el directorio proporcionado independientemente de si el usuario ha especificado la marca '--disk-cache-dir'. Para evitar la pérdida de datos u otros errores inesperados, no configure esta directiva en el directorio raíz de un volumen o en un directorio usado para otros fines, ya que Microsoft Edge administra su contenido.

Consulte [https://go.microsoft.com/fwlink/?linkid=2095041](https://go.microsoft.com/fwlink/?linkid=2095041) para obtener una lista de las variables que puede usar al especificar directorios y rutas.

Si no se configura esta directiva, se usará el directorio de caché predeterminado y los usuarios podrán invalidarlo con la marca de línea de comandos '--disk-cache-dir'.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: No - Requiere reiniciar el explorador

  #### Tipo de datos:
  Cadena

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: DiskCacheDir
  - Nombre de la directiva de grupos: Establecer el directorio de memoria caché del disco
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: DiskCacheDir
  - Tipo de valor: REG_SZ
  ##### Valor de ejemplo:
```
"${user_home}/Edge_cache"
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: DiskCacheDir
  - Valor de ejemplo:
``` xml
<string>${user_home}/Edge_cache</string>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### DiskCacheSize
  #### Establecer tamaño de caché de disco, en bytes
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Configura el tamaño de la memoria caché, en bytes, que se usa para almacenar archivos en el disco.

Si habilita esta directiva, Microsoft Edge usará el tamaño de la memoria caché proporcionado independientemente de si el usuario ha especificado la marca '--disk-cache-size'. El valor especificado en esta directiva no es un límite estricto, sino una sugerencia para el sistema de almacenamiento en caché; cualquier valor de menos de unos pocos megabytes será demasiado pequeño y se redondeará hasta un mínimo razonable.

Si se establece el valor de esta directiva en 0, se usará el tamaño de memoria caché predeterminado y los usuarios no podrán cambiarlo.

Si no se configura esta directiva, se usará el tamaño predeterminado, pero los usuarios podrán invalidarlo con la marca '--disk-cache-size'.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: No - Requiere reiniciar el explorador

  #### Tipo de datos:
  Entero

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: DiskCacheSize
  - Nombre de la directiva de grupos: Establecer tamaño de caché de disco, en bytes
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: DiskCacheSize
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x06400000
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: DiskCacheSize
  - Valor de ejemplo:
``` xml
<integer>104857600</integer>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### DownloadDirectory
  #### Establecer el directorio de descarga
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Configura el directorio que se usará al descargar archivos.

Si se habilita esta directiva, Microsoft Edge usará el directorio proporcionado independientemente de si el usuario ha especificado uno o ha elegido que se le solicite la ubicación de descarga cada vez. Consulte [https://go.microsoft.com/fwlink/?linkid=2095041](https://go.microsoft.com/fwlink/?linkid=2095041) para obtener una lista de las variables que se pueden usar.

Si se deshabilita o no se configura esta directiva, se usará el directorio de descarga predeterminado y el usuario podrá cambiarlo.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: Sí
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Cadena

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: DownloadDirectory
  - Nombre de la directiva de grupos: Establecer el directorio de descarga
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): Plantillas administrativas/Microsoft Edge - Configuración predeterminada (los usuarios pueden cambiarla)/
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): SOFTWARE\Policies\Microsoft\Edge\Recomendada
  - Nombre del valor: DownloadDirectory
  - Tipo de valor: REG_SZ
  ##### Valor de ejemplo:
```
"/home/${user_name}/Downloads"
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: DownloadDirectory
  - Valor de ejemplo:
``` xml
<string>/home/${user_name}/Downloads</string>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### DownloadRestrictions
  #### Permitir restricciones de descarga
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Configura el tipo de descargas que Microsoft Edge bloquea por completo, sin permitir que los usuarios anulen la decisión de seguridad.

Establezca 'Bloquear descargas peligrosas' (1) para permitir todas las descargas excepto las que tienen advertencias de SmartScreen de Microsoft Defender.

Establezca 'Bloquear descargas potencialmente peligrosas' (2) para permitir todas las descargas, excepto las que tienen advertencias de SmartScreen de Microsoft Defender sobre descargas potencialmente peligrosas.

Establezca 'Bloquear todas las descargas' (3) para bloquear todas las descargas.

Si no se configura esta directiva o no se establece la opción 'Sin restricciones especiales' (0), las descargas pasarán por las restricciones de seguridad habituales basadas en los resultados del análisis de SmartScreen de Microsoft Defender.

Tenga en cuenta que estas restricciones se aplican a las descargas desde el contenido de la página web, así como a la opción del menú contextual 'descargar vínculo...'. Estas restricciones no se aplican a guardar o descargar la página que se muestra actualmente, ni tampoco a la opción Guardar como PDF de las opciones de impresión.

Consulte [https://go.microsoft.com/fwlink/?linkid=2094934](https://go.microsoft.com/fwlink/?linkid=2094934) para obtener más información acerca de SmartScreen de Microsoft Defender.

* 0 = Sin restricciones especiales

* 1 = Bloquear descargas peligrosas

* 2 = Bloquear descargas potencialmente peligrosas

* 3 = Bloquear todas las descargas

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: Sí
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Entero

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: DownloadRestrictions
  - Nombre de la directiva de grupos: Permitir restricciones de descarga
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): Plantillas administrativas/Microsoft Edge - Configuración predeterminada (los usuarios pueden cambiarla)/
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): SOFTWARE\Policies\Microsoft\Edge\Recomendada
  - Nombre del valor: DownloadRestrictions
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000002
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: DownloadRestrictions
  - Valor de ejemplo:
``` xml
<integer>2</integer>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### EdgeCollectionsEnabled
  #### Habilitar la característica Colecciones
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 78 o posterior

  #### Descripción
  Permite que los usuarios tengan acceso a la característica Colecciones, donde pueden recopilar, organizar, compartir y exportar contenido de forma más eficaz y con la integración de Office.

Si se habilita o no se configura esta directiva, los usuarios podrán acceder y usar la característica Colecciones en Microsoft Edge.

Si se deshabilita esta directiva, los usuarios no podrán obtener acceso ni usar Colecciones en Microsoft Edge.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: No - Requiere reiniciar el explorador

  #### Tipo de datos:
  Booleano

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: EdgeCollectionsEnabled
  - Nombre de la directiva de grupos: Habilitar la característica Colecciones
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: EdgeCollectionsEnabled
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000001
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: EdgeCollectionsEnabled
  - Valor de ejemplo:
``` xml
<true/>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### EditFavoritesEnabled
  #### Permite a los usuarios editar los favoritos
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Habilita esta directiva para permitir que los usuarios agreguen, quiten y modifiquen favoritos. Este es el comportamiento predeterminado si no se configura la directiva.

Deshabilita esta directiva para impedir que los usuarios agreguen, quiten o modifiquen favoritos. Pueden seguir usando favoritos existentes.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Booleano

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: EditFavoritesEnabled
  - Nombre de la directiva de grupos: Permite a los usuarios editar los favoritos
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: EditFavoritesEnabled
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000000
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: EditFavoritesEnabled
  - Valor de ejemplo:
``` xml
<false/>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### EnableDeprecatedWebPlatformFeatures
  #### Volver a habilitar las características de la plataforma web en desuso durante un tiempo limitado
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Especificar una lista de características de la plataforma web en desuso para volver a habilitarlas temporalmente.

Esta directiva permite volver a habilitar las características de la plataforma web en desuso durante un tiempo limitado. Las características se identifican mediante una etiqueta de cadena.

Si no se configura esta directiva, si la lista está vacía o si una característica no coincide con una de las etiquetas de cadena compatibles, todas las características de la plataforma web en desuso permanecerán deshabilitadas.

Aunque la propia directiva se admite en las plataformas anteriores, es posible que la característica que se está habilitando no esté disponible en todas las plataformas. No todas las características de la plataforma web en desuso se pueden volver a habilitar. Solo aquellas que se indican explícitamente a continuación pueden volver a habilitarse y solo durante un período de tiempo limitado, que es diferente en función de la característica. Puedes revisar la finalidad de los cambios de la característica de la plataforma web en https://bit.ly/blinkintents.

El formato habitual de la etiqueta de cadena es [DeprecatedFeatureName]_EffectiveUntil[yyyymmdd].

* "ExampleDeprecatedFeature_EffectiveUntil20080902" = Habilitar la API de ExampleDeprecatedFeature a través de 2008/09/02


  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Lista de cadenas

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: EnableDeprecatedWebPlatformFeatures
  - Nombre de la directiva de grupos: Volver a habilitar las características de la plataforma web en desuso durante un tiempo limitado
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge\EnableDeprecatedWebPlatformFeatures
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: 1, 2, 3, ...
  - Tipo de valor: lista de REG_SZ
  ##### Valor de ejemplo:
```
SOFTWARE\Policies\Microsoft\Edge\EnableDeprecatedWebPlatformFeatures\0 = "ExampleDeprecatedFeature_EffectiveUntil20080902"

```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: EnableDeprecatedWebPlatformFeatures
  - Valor de ejemplo:
``` xml
<array>
  <string>ExampleDeprecatedFeature_EffectiveUntil20080902</string>
</array>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### EnableDomainActionsDownload
  #### Habilitar la descarga de acciones de dominio desde Microsoft
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  En Microsoft Edge, las acciones de dominio representan una serie de características de compatibilidad que ayudan a que el explorador funcione correctamente en la web.

Microsoft conserva una lista de acciones para determinados dominios por motivos de compatibilidad. Por ejemplo, el explorador puede invalidar la cadena de agente de usuario en un sitio web si dicho sitio web está dañado debido a la nueva cadena de agente de usuario en Microsoft Edge. Cada una de estas acciones debe ser temporal mientras Microsoft intenta resolver el problema con el propietario del sitio.

Cuando se inicia el explorador, y después periódicamente, el explorador se pondrá en contacto con el servicio de configuración y experimentación de Microsoft que contiene la lista de acciones de compatibilidad que se deben realizar más reciente. Esta lista se guardará localmente después de recuperarla por primera vez, de modo que las solicitudes posteriores solo actualizarán la lista si ha cambiado la copia del servidor.

Si se habilita esta directiva, la lista de acciones del dominio seguirá descargándose desde el servicio de configuración y experimentación de Microsoft.

Si se deshabilita esta directiva, la lista de acciones del dominio no volverá a descargarse desde el servicio de configuración y experimentación de Microsoft.

Si no se configura esta directiva, la lista de acciones del dominio seguirá descargándose desde el servicio de configuración y experimentación de Microsoft.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Booleano

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: EnableDomainActionsDownload
  - Nombre de la directiva de grupos: Habilitar la descarga de acciones de dominio desde Microsoft
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: EnableDomainActionsDownload
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000001
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: EnableDomainActionsDownload
  - Valor de ejemplo:
``` xml
<true/>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### EnableOnlineRevocationChecks
  #### Habilitar comprobaciones de CRL/OCSP en línea
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Las comprobaciones de revocación en línea no ofrecen una ventaja de seguridad significativa y están deshabilitadas de manera predeterminada.

Si se habilita esta directiva, Microsoft Edge llevará a cabo comprobaciones de errores recuperables de OCSP/CRL en línea. "Error recuperable" significa que si no se puede establecer contacto con el servidor de revocación, el certificado se considerará válido.

Si se deshabilita la directiva o no se configura, Microsoft Edge no llevará a cabo comprobaciones de revocación en línea.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Booleano

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: EnableOnlineRevocationChecks
  - Nombre de la directiva de grupos: Habilitar comprobaciones de CRL/OCSP en línea
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: EnableOnlineRevocationChecks
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000000
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: EnableOnlineRevocationChecks
  - Valor de ejemplo:
``` xml
<false/>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### EnterpriseHardwarePlatformAPIEnabled
  #### Permitir que las extensiones administradas usen la API de la plataforma de hardware empresarial
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 78 o posterior

  #### Descripción
  Cuando esta directiva está establecida en habilitada, las extensiones instaladas por la directiva empresarial podrán usar la API de plataforma de hardware de la empresa.
Cuando esta directiva está establecida en deshabilitada o no está configurada, no se permite que las extensiones usen la API de plataforma de hardware de la empresa.
Esta directiva también se aplica a las extensiones del componente.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Booleano

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: EnterpriseHardwarePlatformAPIEnabled
  - Nombre de la directiva de grupos: Permitir que las extensiones administradas usen la API de la plataforma de hardware empresarial
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: EnterpriseHardwarePlatformAPIEnabled
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000001
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: EnterpriseHardwarePlatformAPIEnabled
  - Valor de ejemplo:
``` xml
<true/>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### ExperimentationAndConfigurationServiceControl
  #### Controlar la comunicación con el servicio de configuración y experimentación
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  En Microsoft Edge, el servicio de experimentación y configuración se usa para implementar la carga de experimentación y configuración.

La carga experimental consiste en una lista de las características de desarrollo anticipadas que Microsoft está habilitando para pruebas y comentarios.

La carga de configuración consiste en una lista de opciones que Microsoft desea implementar para Microsoft Edge para optimizar la experiencia del usuario. Por ejemplo, la carga de configuración puede especificar la frecuencia con la que Microsoft Edge envía solicitudes al servicio de experimentación y configuración para recuperar la carga más reciente.

Si se establece esta directiva en el modo "Recuperar configuraciones y experimentos", la carga completa se descarga del servicio de experimentación y configuración. Esto incluye las cargas de experimentación y configuración.

Si se establece esta directiva en el modo "Recuperar solo configuraciones", solo se entrega la carga de configuración.

Si se establece esta directiva en el modo "Deshabilitar la comunicación con el servicio de experimentación y configuración", la comunicación con el servicio de experimentación y configuración se detiene por completo.

Si no se configura esta directiva, en un dispositivo administrado en los canales Estable y Beta, el comportamiento es el mismo que el modo "Recuperar solo configuraciones".

Si no se configura esta directiva, en un dispositivo no administrado, el comportamiento es el mismo que el modo "Recuperar configuraciones y experimentos".

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Entero

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: ExperimentationAndConfigurationServiceControl
  - Nombre de la directiva de grupos: Controlar la comunicación con el servicio de configuración y experimentación
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: ExperimentationAndConfigurationServiceControl
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000002
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: ExperimentationAndConfigurationServiceControl
  - Valor de ejemplo:
``` xml
<integer>2</integer>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### ExternalProtocolDialogShowAlwaysOpenCheckbox
  #### Mostrar una casilla "Abrir siempre" en el diálogo de protocolo externo.
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 79 o posterior

  #### Descripción
  Esta directiva controla si la casilla "Abrir siempre" se muestra en las solicitudes de confirmación de inicio del protocolo externo.

Si se establece esta directiva en True, cuando se muestra una solicitud de confirmación del protocolo externo, el usuario puede seleccionar "Abrir siempre". El usuario no recibirá ningún mensaje de confirmación en el futuro para este protocolo.

Si se establece esta directiva en False o la directiva está desactivada, no se mostrará la casilla "Abrir siempre". Se solicitará la confirmación del usuario cada vez que se invoque un protocolo externo.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: No - Requiere reiniciar el explorador

  #### Tipo de datos:
  Booleano

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: ExternalProtocolDialogShowAlwaysOpenCheckbox
  - Nombre de la directiva de grupos: Mostrar una casilla "Abrir siempre" en el diálogo de protocolo externo.
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: ExternalProtocolDialogShowAlwaysOpenCheckbox
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000001
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: ExternalProtocolDialogShowAlwaysOpenCheckbox
  - Valor de ejemplo:
``` xml
<true/>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### FavoritesBarEnabled
  #### Habilitar barra de favoritos
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Habilita o deshabilita la barra de favoritos.

Si se habilita esta directiva, los usuarios verán la barra de favoritos.

Si se deshabilita esta directiva, los usuarios no verán la barra de favoritos.

Si no se configura esta directiva, el usuario puede decidir usar la barra de favoritos o no.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: Sí
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Booleano

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: FavoritesBarEnabled
  - Nombre de la directiva de grupos: Habilitar barra de favoritos
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): Plantillas administrativas/Microsoft Edge - Configuración predeterminada (los usuarios pueden cambiarla)/
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): SOFTWARE\Policies\Microsoft\Edge\Recomendada
  - Nombre del valor: FavoritesBarEnabled
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000001
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: FavoritesBarEnabled
  - Valor de ejemplo:
``` xml
<true/>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### ForceBingSafeSearch
  #### Aplicar Búsqueda segura de Bing
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Asegúrate de que las consultas en Bing Web Search se realicen con Búsqueda segura establecida en el valor especificado. Los usuarios no pueden cambiar esta configuración.

Si configuras esta directiva como "Desactivada", Búsqueda segura en Bing Search revertirá al valor bing.com.

Si se establece esta directiva en "Moderada", se usará la configuración moderada en Búsqueda segura. La configuración moderada filtra los vídeos e imágenes para adultos, pero no el texto de los resultados de la búsqueda.

Si se establece esta directiva en "Estricta", se usará la configuración estricta en Búsqueda segura. La opción estricta filtra el texto, las imágenes y los vídeos de adultos.

Si se deshabilita esta directiva o no se configura, Búsqueda segura en Bing Search no se aplicará y los usuarios podrán establecer el valor que deseen en bing.com.

* 0 = No configurar restricciones de búsqueda en Bing

* 1 = Configurar restricciones de búsqueda moderadas en Bing

* 2 = No configurar restricciones de búsqueda estrictas en Bing

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Entero

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: ForceBingSafeSearch
  - Nombre de la directiva de grupos: Aplicar Búsqueda segura de Bing
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: ForceBingSafeSearch
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000000
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: ForceBingSafeSearch
  - Valor de ejemplo:
``` xml
<integer>0</integer>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### ForceEphemeralProfiles
  #### Habilitar el uso de perfiles efímeros
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Controla si los perfiles de usuario se cambian a modo efímero. Los perfiles efímeros se crean cuando se inicia una sesión, se eliminan cuando finaliza la sesión y se asocian con el perfil original del usuario.

Si se habilita esta directiva, los perfiles se ejecutarán en modo efímero. Esto permite a los usuarios trabajar desde sus propios dispositivos sin guardar los datos de exploración en esos dispositivos. Si se habilita esta directiva como una directiva del sistema operativo (por ejemplo, mediante un GPO en Windows), se aplicará a todos los perfiles del sistema.

Si se deshabilita esta directiva o no se configura, los usuarios reciben sus perfiles normales cuando inician sesión en el explorador.

En modo efímero, los datos de perfil se guardan en el disco solo durante la sesión de usuario. Las características como el historial del explorador, las extensiones y sus datos, los datos web como las cookies y las bases de datos web no se guardarán después de cerrar el explorador. Esto no impide que un usuario descargue manualmente datos en el disco, o que guarde páginas o las imprima. Si el usuario ha habilitado la sincronización, todos los datos se conservan en sus cuentas de sincronización al igual que con los perfiles normales. Los usuarios también pueden usar la exploración de InPrivate en modo efímero a menos que se deshabilite explícitamente.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: No - Requiere reiniciar el explorador

  #### Tipo de datos:
  Booleano

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: ForceEphemeralProfiles
  - Nombre de la directiva de grupos: Habilitar el uso de perfiles efímeros
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: ForceEphemeralProfiles
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000001
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: ForceEphemeralProfiles
  - Valor de ejemplo:
``` xml
<true/>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### ForceGoogleSafeSearch
  #### Aplicar la Búsqueda segura de Google
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Exige que las consultas en Google Web Search se realicen con la Búsqueda segura establecida como activa e impide que los usuarios cambien esta configuración.

Si se habilita esta directiva, la Búsqueda segura en Google Search siempre estará activa.

Si se deshabilita esta directiva o no se configura, no se exigirá la Búsqueda segura en la búsqueda de Google.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Booleano

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: ForceGoogleSafeSearch
  - Nombre de la directiva de grupos: Aplicar la Búsqueda segura de Google
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: ForceGoogleSafeSearch
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000000
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: ForceGoogleSafeSearch
  - Valor de ejemplo:
``` xml
<false/>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### ForceNetworkInProcess
  #### Forzar el código de red para que se ejecute en el proceso del explorador
  >Versiones admitidas: Microsoft Edge en Windows desde la versión 78 o posterior

  #### Descripción
  Esta directiva fuerza al código de redes a ejecutarse en el proceso del explorador.

Esta directiva está deshabilitada de forma predeterminada. Si está habilitada, los usuarios están abiertos a problemas de seguridad cuando el proceso de red está en un espacio aislado.

Esta directiva está pensada para proporcionar a las empresas una oportunidad de migrar a software de terceros que no depende del enlace de las API de red. Los servidores proxy se recomiendan a LSP y revisiones de API Win32.

Si no se establece esta Directiva, el código de red puede quedarse sin el proceso del explorador en función de las pruebas de campo del experimento de NetworkService.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: No - Requiere reiniciar el explorador

  #### Tipo de datos:
  Booleano

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: ForceNetworkInProcess
  - Nombre de la directiva de grupos: Forzar el código de red para que se ejecute en el proceso del explorador
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: ForceNetworkInProcess
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000000
```


  

  [Volver al principio](#microsoft-edge:-directivas)

  ### ForceYouTubeRestrict
  #### Forzar el modo Restringido mínimo en YouTube
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Fuerza un modo restringido mínimo en YouTube e impide que los usuarios seleccionen un modo menos restringido.

Establecer en Estricto (2) para forzar el modo restringido estricto en YouTube.

Establecer en Moderado (1) para forzar que el usuario use solo el modo restringido moderado y el modo restringido estricto en YouTube. No pueden deshabilitar el modo restringido.

Establecer en Desactivada (0) o no configurar esta directiva para no forzar el modo Restringido en YouTube. Las directivas externas como las directivas de YouTube podrán forzar el modo Restringido.

* 0 = No forzar el modo Restringido en YouTube.

* 1 = Forzar como mínimo el modo restringido moderado en YouTube.

* 2 = Forzar el modo restringido estricto en YouTube

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Entero

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: ForceYouTubeRestrict
  - Nombre de la directiva de grupos: Forzar el modo Restringido mínimo en YouTube
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: ForceYouTubeRestrict
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000000
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: ForceYouTubeRestrict
  - Valor de ejemplo:
``` xml
<integer>0</integer>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### FullscreenAllowed
  #### Permitir modo de pantalla completa
  >Versiones admitidas: Microsoft Edge en Windows desde la versión 77 o posterior

  #### Descripción
  Establecer la disponibilidad del modo de pantalla completa: toda la UI de Microsoft Edge está oculta y solo está visible el contenido web.

Si se habilita esta directiva o no se configura, el usuario, las aplicaciones y las extensiones con los permisos apropiados pueden pasar al modo de pantalla completa.

Si se deshabilita esta directiva, los usuarios, las aplicaciones y las extensiones no podrán pasar al modo de pantalla completa.

Cuando se deshabilita el modo de pantalla completa, no se puede abrir Microsoft Edge en modo de pantalla completa usando la línea de comandos.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Booleano

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: FullscreenAllowed
  - Nombre de la directiva de grupos: Permitir modo de pantalla completa
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: FullscreenAllowed
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000001
```


  

  [Volver al principio](#microsoft-edge:-directivas)

  ### GoToIntranetSiteForSingleWordEntryInAddressBar
  #### Fuerce la navegación directa en el sitio de intranet en lugar de buscar entradas de una única palabra en la barra de direcciones.
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 78 o posterior

  #### Descripción
  Si se habilita esta directiva, el resultado principal de sugerencia automática en la lista de sugerencias de la barra de direcciones navegará a sitios de intranet si el texto escrito en la barra de direcciones es una sola palabra sin puntuación.

La navegación predeterminada cuando se escribe una sola palabra sin puntuación llevará a cabo una navegación a un sitio de intranet que coincida con el texto escrito.

Si se habilita esta directiva, el segundo resultado de las sugerencias automáticas en la lista de sugerencias de la barra de direcciones llevará a cabo una búsqueda web tal como se ha introducido, siempre y cuando el texto sea una sola palabra sin puntuación. Se usará el proveedor de búsquedas predeterminado a menos que también esté habilitada una directiva que impida la búsqueda web.

Habilitar esta directiva tiene dos efectos:

Ya no tendrá lugar la navegación a sitios en respuesta a consultas de una sola palabra que normalmente se resolverían a un elemento del historial. En su lugar, el explorador intentará navegar a sitios internos que puede que no existan en la intranet de la organización. Esto provocará un error 404.

Los términos de búsqueda populares de una sola palabra requerirán la selección manual de sugerencias de búsqueda para llevar a cabo una búsqueda correctamente.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Booleano

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: GoToIntranetSiteForSingleWordEntryInAddressBar
  - Nombre de la directiva de grupos: Fuerce la navegación directa en el sitio de intranet en lugar de buscar entradas de una única palabra en la barra de direcciones.
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: GoToIntranetSiteForSingleWordEntryInAddressBar
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000000
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: GoToIntranetSiteForSingleWordEntryInAddressBar
  - Valor de ejemplo:
``` xml
<false/>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### HSTSPolicyBypassList
  #### Configurar la lista de nombres que omitirán la comprobación de directiva de HSTS
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 79 o posterior

  #### Descripción
  Los nombres de host especificados en esta lista se excluirán de la comprobación de directiva HSTS que podría actualizar las solicitudes de "http://" a "https://". Solo se permiten nombres de host de una sola etiqueta en esta directiva. Los nombres de host deben tener un formato canónico. Cualquier IDN debe convertirse a su formato de etiqueta A y todas las letras ASCII deben estar en minúsculas. Esta directiva solo se aplica a los nombres de host específicos especificados; no se aplica a los subdominios de los nombres de la lista.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: No - Requiere reiniciar el explorador

  #### Tipo de datos:
  Lista de cadenas

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: HSTSPolicyBypassList
  - Nombre de la directiva de grupos: Configurar la lista de nombres que omitirán la comprobación de directiva de HSTS
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge\HSTSPolicyBypassList
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: 1, 2, 3, ...
  - Tipo de valor: lista de REG_SZ
  ##### Valor de ejemplo:
```
SOFTWARE\Policies\Microsoft\Edge\HSTSPolicyBypassList\0 = "meet"

```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: HSTSPolicyBypassList
  - Valor de ejemplo:
``` xml
<array>
  <string>meet</string>
</array>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### HardwareAccelerationModeEnabled
  #### Usar aceleración de hardware cuando esté disponible
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Especificar si se usa la aceleración de hardware, si está disponible. Si se habilita esta directiva o no se configura, se habilitará la aceleración de hardware, a menos que se haya bloqueado explícitamente una característica de GPU.

Si deshabilita esta directiva, se deshabilitará la aceleración de hardware.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: No - Requiere reiniciar el explorador

  #### Tipo de datos:
  Booleano

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: HardwareAccelerationModeEnabled
  - Nombre de la directiva de grupos: Usar aceleración de hardware cuando esté disponible
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: HardwareAccelerationModeEnabled
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000001
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: HardwareAccelerationModeEnabled
  - Valor de ejemplo:
``` xml
<true/>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### ImportAutofillFormData
  #### Permitir la importación de datos de Autorrellenar del formulario
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Permite a los usuarios importar datos de formulario de Autorrellenar desde otro explorador a Microsoft Edge.

Si se habilita esta directiva, se selecciona automáticamente la opción para importar manualmente los datos de Autorrellenar.

Si se deshabilita esta directiva, los datos de formulario de Autorrellenar no se importarán en la primera ejecución y los usuarios no podrán importarlos manualmente.

Si no se configura esta directiva, se importarán los datos de Autorrellenar en la primera ejecución y los usuarios podrán elegir si quieren importar estos datos manualmente durante las sesiones de exploración posteriores.

Puede establecerse esta directiva como una recomendación. Esto significa que Microsoft Edge importará datos de Autorrellenar en la primera ejecución, pero los usuarios podrán seleccionar o borrar la opción **datos de autorrellenar** durante la importación manual.

**Nota**: Esta directiva actualmente administra la importación de Google Chrome (en Windows 7, 8 y 10 y en macOS).

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: Sí
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Booleano

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: ImportAutofillFormData
  - Nombre de la directiva de grupos: Permitir la importación de datos de Autorrellenar del formulario
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): Plantillas administrativas/Microsoft Edge - Configuración predeterminada (los usuarios pueden cambiarla)/
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): SOFTWARE\Policies\Microsoft\Edge\Recomendada
  - Nombre del valor: ImportAutofillFormData
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000001
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: ImportAutofillFormData
  - Valor de ejemplo:
``` xml
<true/>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### ImportBrowserSettings
  #### Permitir la importación de la configuración del explorador
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 78 o posterior

  #### Descripción
  Permite a los usuarios importar la configuración del motor de búsqueda de otro explorador a Microsoft Edge.

Si se habilita esta directiva, se seleccionará automáticamente la casilla de verificación **Configuración del explorador** en el cuadro de diálogo **Importar datos del explorador**.

Si se deshabilita esta directiva, la configuración del explorador no se importará en la primera ejecución y los usuarios no podrán importarla manualmente.

Si no se configura esta directiva, la configuración del explorador se importará en la primera ejecución y los usuarios podrán elegir si importar estos datos manualmente durante las sesiones de exploración posteriores.

También puede establecerse esta directiva como una recomendación. Esto significa que Microsoft Edge importa la configuración del motor de búsqueda en la primera ejecución, pero los usuarios pueden seleccionar o borrar la opción **configuración del explorador** durante la importación manual.

**Nota**: Esta directiva administra actualmente la importación de Google Chrome (en Windows 7, 8 y 10 y en macOS).

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: Sí
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Booleano

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: ImportBrowserSettings
  - Nombre de la directiva de grupos: Permitir la importación de la configuración del explorador
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): Plantillas administrativas/Microsoft Edge - Configuración predeterminada (los usuarios pueden cambiarla)/
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): SOFTWARE\Policies\Microsoft\Edge\Recomendada
  - Nombre del valor: ImportBrowserSettings
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000001
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: ImportBrowserSettings
  - Valor de ejemplo:
``` xml
<true/>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### ImportFavorites
  #### Permitir la importación de favoritos
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Permite a los usuarios importar favoritos de otro explorador en Microsoft Edge.

Si se habilita esta directiva, la casilla **favoritos** se activará automáticamente en el cuadro de diálogo **Importar datos del explorador**.

Si se deshabilita esta directiva, los favoritos no se importarán en la primera ejecución y los usuarios no podrán importarlos manualmente.

Si no se configura esta directiva, los favoritos se importan en la primera ejecución y los usuarios podrán elegir si quieren importarlos manualmente durante las sesiones de exploración posteriores.

También puede establecerse esta directiva como recomendación. Esto significa que Microsoft Edge importa los favoritos en la primera ejecución, pero los usuarios podrán seleccionar o borrar la opción **favoritos** durante la importación manual.

**Nota**: Esta directiva administra actualmente la importación desde los exploradores de Internet Explorer (en Windows 7, 8 y 10), Google Chrome (en Windows 7, 8 y 10 y en macOS) y Apple Safari (en macOS).

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: Sí
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Booleano

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: ImportFavorites
  - Nombre de la directiva de grupos: Permitir la importación de favoritos
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): Plantillas administrativas/Microsoft Edge - Configuración predeterminada (los usuarios pueden cambiarla)/
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): SOFTWARE\Policies\Microsoft\Edge\Recomendada
  - Nombre del valor: ImportFavorites
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000001
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: ImportFavorites
  - Valor de ejemplo:
``` xml
<true/>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### ImportHistory
  #### Permitir la importación del historial de exploración
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Permite a los usuarios importar su historial de exploración desde otro explorador a Microsoft Edge.

Si se habilita esta directiva, se seleccionará automáticamente la casilla **Historial de exploración** en el cuadro de diálogo **Importar datos del explorador**.

Si se deshabilita esta directiva, los datos del historial de exploración no se importarán en la primera ejecución y los usuarios no podrán importar los datos manualmente.

Si no se configura esta directiva, los datos del historial de exploración se importarán en la primera ejecución y los usuarios podrán elegir si quieren importarlos manualmente durante las sesiones de exploración posteriores.

También puede establecerse esta directiva como recomendación. Esto significa que Microsoft Edge importa el historial de exploración en la primera ejecución, pero los usuarios podrán seleccionar o borrar la opción **historial** durante la importación manual.

**Nota**: Esta directiva administra actualmente la importación desde los exploradores de Internet Explorer (en Windows 7, 8 y 10), Google Chrome (en Windows 7, 8 y 10 y en macOS) y Apple Safari (macOS).

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: Sí
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Booleano

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: ImportHistory
  - Nombre de la directiva de grupos: Permitir la importación del historial de exploración
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): Plantillas administrativas/Microsoft Edge - Configuración predeterminada (los usuarios pueden cambiarla)/
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): SOFTWARE\Policies\Microsoft\Edge\Recomendada
  - Nombre del valor: ImportHistory
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000001
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: ImportHistory
  - Valor de ejemplo:
``` xml
<true/>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### ImportHomepage
  #### Permitir la importación de la configuración de la página principal
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Permite a los usuarios importar la configuración de la página principal de otro explorador a Microsoft Edge.

Si se habilita esta directiva, se seleccionará automáticamente la opción para importar manualmente la configuración de la página principal.

Si se deshabilita esta directiva, la configuración de la página principal no se importará en la primera ejecución y los usuarios no podrán importarla manualmente.

Si no se configura esta directiva, la configuración de la página principal se importará en la primera ejecución y los usuarios podrán elegir si importar estos datos manualmente durante las sesiones de exploración posteriores.

Puede establecerse esta directiva como una recomendación. Esto significa que Microsoft Edge importa la configuración de la página principal en la primera ejecución, pero los usuarios pueden seleccionar o borrar la opción **página principal** durante la importación manual.

**Nota**: Esta directiva administra actualmente la importación desde Internet Explorer (en Windows 7, 8 y 10).

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Booleano

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: ImportHomepage
  - Nombre de la directiva de grupos: Permitir la importación de la configuración de la página principal
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: ImportHomepage
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000001
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: ImportHomepage
  - Valor de ejemplo:
``` xml
<true/>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### ImportOpenTabs
  #### Permitir la importación de pestañas abiertas
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 79 o posterior

  #### Descripción
  Permite a los usuarios importar pestañas abiertas y ancladas desde otro explorador a Microsoft Edge.

Si se habilita esta directiva, se activará automáticamente la casilla **Pestañas abiertas** en el cuadro de diálogo **Importar datos del navegador**.

Si se deshabilita esta directiva, las pestañas abiertas no se importarán en la primera ejecución y los usuarios no podrán importarla manualmente.

Si no se configura esta directiva, las pestañas abiertas se importarán en la primera ejecución y los usuarios podrán elegir si importarla manualmente durante las sesiones de exploración posteriores.

También se puede establecer esta directiva como recomendación. Esto significa que Microsoft Edge importa las pestañas abiertas en la primera ejecución, pero los usuarios pueden activar o desactivar la opción **Pestañas abiertas** durante la importación manual.

**Nota:** Esta directiva solo admite actualmente la importación desde Google Chrome (en Windows 7, 8 y 10 y en macOS).

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: Sí
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Booleano

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: ImportOpenTabs
  - Nombre de la directiva de grupos: Permitir la importación de pestañas abiertas
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): Plantillas administrativas/Microsoft Edge - Configuración predeterminada (los usuarios pueden cambiarla)/
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): SOFTWARE\Policies\Microsoft\Edge\Recomendada
  - Nombre del valor: ImportOpenTabs
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000001
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: ImportOpenTabs
  - Valor de ejemplo:
``` xml
<true/>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### ImportPaymentInfo
  #### Permitir la importación de información de pago
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Permite a los usuarios importar la información de pago desde otro explorador a Microsoft Edge.

Si se habilita esta directiva, se activará automáticamente la casilla **información de pago** en el cuadro de diálogo **Importar datos del navegador**.

Si se deshabilita esta directiva, la información de pago no se importará en la primera ejecución y los usuarios no podrán importarla manualmente.

Si no se configura esta directiva, la información de pago se importará en la primera ejecución y los usuarios podrán elegir si importarla manualmente durante las sesiones de exploración posteriores.

También se puede establecer esta directiva como recomendación. Esto significa que Microsoft Edge importa la información de pago en la primera ejecución, pero los usuarios pueden activar o desactivar la opción **información de pago** durante la importación manual.

**Nota:** Esta directiva administra actualmente la importación de Google Chrome (en Windows 7, 8 y 10 y en macOS).

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: Sí
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Booleano

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: ImportPaymentInfo
  - Nombre de la directiva de grupos: Permitir la importación de información de pago
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): Plantillas administrativas/Microsoft Edge - Configuración predeterminada (los usuarios pueden cambiarla)/
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): SOFTWARE\Policies\Microsoft\Edge\Recomendada
  - Nombre del valor: ImportPaymentInfo
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000001
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: ImportPaymentInfo
  - Valor de ejemplo:
``` xml
<true/>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### ImportSavedPasswords
  #### Permitir la importación de contraseñas guardadas
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Permite que los usuarios importen las contraseñas guardadas desde otro explorador a Microsoft Edge.

Si se habilita esta directiva, la opción de importar automáticamente las contraseñas guardadas se selecciona automáticamente.

Si se deshabilita esta directiva, las contraseñas guardadas no se importan en la primera ejecución y los usuarios no podrán importarlas de forma manual.

Si no se configura esta directiva, las contraseñas se importarán en la primera ejecución y los usuarios podrán optar por importarlas manualmente durante las sesiones de exploración posteriores.

Puede establecerse esta directiva como una recomendación. Esto significa que Microsoft Edge importa contraseñas en la primera ejecución, pero los usuarios podrán activar seleccionar o borrar la opción **contraseñas** durante la importación manual.

**Nota**: Esta directiva administra actualmente las importaciones desde exploradores de Internet Explorer (en Windows 7, 8 y 10) y Google Chrome (en Windows 7, 8 y 10 and on macOS).

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: Sí
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Booleano

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: ImportSavedPasswords
  - Nombre de la directiva de grupos: Permitir la importación de contraseñas guardadas
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): Plantillas administrativas/Microsoft Edge - Configuración predeterminada (los usuarios pueden cambiarla)/
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): SOFTWARE\Policies\Microsoft\Edge\Recomendada
  - Nombre del valor: ImportSavedPasswords
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000001
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: ImportSavedPasswords
  - Valor de ejemplo:
``` xml
<true/>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### ImportSearchEngine
  #### Permitir la importación de la configuración del motor de búsqueda
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Permite a los usuarios importar la configuración del motor de búsqueda de otro explorador a Microsoft Edge.

Si se habilita esta directiva, se seleccionará automáticamente la opción para importar la configuración del motor de búsqueda.

Si se deshabilita esta directiva, la configuración de los motores de búsqueda no se importará en la primera ejecución y los usuarios no podrán importarlos manualmente.

Si no se configura esta directiva, la configuración del motor de búsqueda se importará en la primera ejecución y los usuarios podrán elegir si importar estos datos manualmente durante las sesiones de exploración posteriores.

Puede establecerse esta directiva como una recomendación. Esto significa que Microsoft Edge importa la configuración del motor de búsqueda en la primera ejecución, pero los usuarios pueden seleccionar o borrar la opción **motor de búsqueda** durante la importación manual.

**Nota**: Esta directiva administra actualmente la importación desde Internet Explorer (en Windows 7, 8 y 10).

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: Sí
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Booleano

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: ImportSearchEngine
  - Nombre de la directiva de grupos: Permitir la importación de la configuración del motor de búsqueda
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): Plantillas administrativas/Microsoft Edge - Configuración predeterminada (los usuarios pueden cambiarla)/
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): SOFTWARE\Policies\Microsoft\Edge\Recomendada
  - Nombre del valor: ImportSearchEngine
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000001
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: ImportSearchEngine
  - Valor de ejemplo:
``` xml
<true/>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### InPrivateModeAvailability
  #### Configurar la disponibilidad del modo InPrivate
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Especifica si el usuario puede abrir páginas en modo InPrivate en Microsoft Edge.

Si no se configura esta directiva o se establece en 'Enabled' (0), los usuarios podrán abrir páginas en modo InPrivate.

Establecer esta directiva en "Deshabilitar" (1) para impedir que los usuarios utilicen el modo InPrivate.

Establecer esta directiva en 'Forzoso' (2) para usar siempre el modo InPrivate.

* 0 = Modo InPrivate disponible

* 1 = Modo InPrivate deshabilitado

* 2 = Modo InPrivate forzoso

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Entero

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: InPrivateModeAvailability
  - Nombre de la directiva de grupos: Configurar la disponibilidad del modo InPrivate
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: InPrivateModeAvailability
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000001
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: InPrivateModeAvailability
  - Valor de ejemplo:
``` xml
<integer>1</integer>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### InternetExplorerIntegrationLevel
  #### Configurar la integración de Internet Explorer
  >Versiones admitidas: Microsoft Edge en Windows desde la versión 77 o posterior

  #### Descripción
  Para obtener instrucciones sobre cómo configurar la experiencia óptima para el modo de Internet Explorer, consulte [https://go.microsoft.com/fwlink/?linkid=2094210](https://go.microsoft.com/fwlink/?linkid=2094210)

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: No - Requiere reiniciar el explorador

  #### Tipo de datos:
  Entero

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: InternetExplorerIntegrationLevel
  - Nombre de la directiva de grupos: Configurar la integración de Internet Explorer
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: InternetExplorerIntegrationLevel
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000001
```


  

  [Volver al principio](#microsoft-edge:-directivas)

  ### InternetExplorerIntegrationSiteList
  #### Configurar la lista de sitios del modo de empresa
  >Versiones admitidas: Microsoft Edge en Windows desde la versión 78 o posterior

  #### Descripción
  Para obtener instrucciones sobre cómo configurar la experiencia óptima para el modo de Internet Explorer, consulte [https://go.microsoft.com/fwlink/?linkid=2094210](https://go.microsoft.com/fwlink/?linkid=2094210)

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: No - Requiere reiniciar el explorador

  #### Tipo de datos:
  Cadena

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: InternetExplorerIntegrationSiteList
  - Nombre de la directiva de grupos: Configurar la lista de sitios del modo de empresa
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: InternetExplorerIntegrationSiteList
  - Tipo de valor: REG_SZ
  ##### Valor de ejemplo:
```
"https://internal.contoso.com/sitelist.xml"
```


  

  [Volver al principio](#microsoft-edge:-directivas)

  ### InternetExplorerIntegrationSiteRedirect
  #### Especificar cómo se comportan las exploraciones "en la página" para sitios no configurados cuando se inician desde páginas en el modo de Internet Explorer
  >Versiones admitidas: Microsoft Edge en Windows desde la versión 79 o posterior

  #### Descripción
  La navegación "en la página" se inicia desde un vínculo, un script o un formulario de la página actual. También puede ser un redireccionamiento del lado del servidor de un intento de navegación anterior "en la página". Por el contrario, un usuario puede iniciar una navegación que no está "en la página", independiente de la página actual, utilizando los controles del explorador. Por ejemplo, usando la barra de direcciones, el botón atrás o un vínculo favorito.

Esta opción le permite especificar si las navegaciones desde páginas cargadas en el modo de Internet Explorer a sitios sin configurar (no configurados en la lista de sitios del modo de empresa) cambiarán a Microsoft Edge o permanecerán en el modo de Internet Explorer.

Esta configuración funciona junto con:
[InternetExplorerIntegrationLevel](#internetexplorerintegrationlevel) está establecido en "modo de Internet Explorer" (1)
y la directiva
[InternetExplorerIntegrationSiteList](#internetexplorerintegrationsitelist) donde la lista tenga al menos una entrada.

Si deshabilita o no configura esta directiva, solo se abrirán en ese modo los sitios configurados para abrirse en el modo de Internet Explorer. Cualquier sitio que no esté configurado para abrirse en el modo de Internet Explorer se redirigirá de nuevo a Microsoft Edge.

Si habilita esta directiva, puede elegir una de las siguientes opciones de navegación:
0 - Predeterminado. Solo los sitios configurados para abrirse en el modo de Internet Explorer se abrirán en ese modo. Cualquier sitio que no esté configurado para abrirse en el modo de Internet Explorer se redirigirá de nuevo a Microsoft Edge.
1 - Mantener solo las exploraciones automáticas en el modo de Internet Explorer. Use esta opción si quiere tener la experiencia predeterminada excepto que todas las exploraciones automáticas (como redirecciones 302) a sitios no configurados se mantengan en el modo de Internet Explorer.
2 - Mantener todas las navegaciones en la página en el modo de Internet Explorer (menos recomendable). Todas las exploraciones de páginas cargadas en el modo IE a sitios sin configurar se mantienen en el modo de Internet Explorer.

Para obtener más información sobre el modo de Internet Explorer, consulte [https://go.microsoft.com/fwlink/?linkid=2105106](https://go.microsoft.com/fwlink/?linkid=2105106)

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: No - Requiere reiniciar el explorador

  #### Tipo de datos:
  Entero

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: InternetExplorerIntegrationSiteRedirect
  - Nombre de la directiva de grupos: Especificar cómo se comportan las exploraciones "en la página" para sitios no configurados cuando se inician desde páginas en el modo de Internet Explorer
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: InternetExplorerIntegrationSiteRedirect
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000000
```


  

  [Volver al principio](#microsoft-edge:-directivas)

  ### IsolateOrigins
  #### Habilitar el aislamiento de sitios para orígenes específicos
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Especificar los orígenes para ejecutar en aislamiento, en su propio proceso.
Esta directiva también aísla los orígenes denominados subdominios; por ejemplo, si se especifica https://contoso.com/ provocará que https://foo.contoso.com/ se aísle como parte del sitio https://contoso.com/.
Si la directiva está habilitada, cada uno de los orígenes en una lista separada por comas se ejecutará en su propio proceso.
Si se deshabilita esta directiva, se deshabilitarán las características 'IsolateOrigins' y 'SitePerProcess'. Los usuarios podrán habilitar la directiva 'IsolateOrigins' manualmente, a través de los marcadores de la línea de comandos.
Si no se establece la directiva, el usuario podrá cambiar esta configuración.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: No - Requiere reiniciar el explorador

  #### Tipo de datos:
  Cadena

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: IsolateOrigins
  - Nombre de la directiva de grupos: Habilitar el aislamiento de sitios para orígenes específicos
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: IsolateOrigins
  - Tipo de valor: REG_SZ
  ##### Valor de ejemplo:
```
"https://contoso.com/,https://fabrikam.com/"
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: IsolateOrigins
  - Valor de ejemplo:
``` xml
<string>https://contoso.com/,https://fabrikam.com/</string>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### ManagedFavorites
  #### Configurar favoritos
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Configura una lista de favoritos administrados.

La directiva crea una lista de favoritos. Cada favorito contiene las claves "name" y "url", que contienen el nombre del favorito y su destino. Puede configurar una subcarpeta mediante la definición de favoritos sin una clave "url", sino con una clave "children" adicional que contiene una lista de favoritos como se define anteriormente (algunos de los cuales pueden volver a ser carpetas). Microsoft Edge modifica las URL incompletas como si se enviaran a través de la barra de direcciones, por ejemplo "microsoft.com" se convierte en "https://microsoft.com/".

Estos favoritos se colocan en una carpeta que el usuario no puede modificar (pero el usuario puede elegir ocultarlo en la barra de favoritos). De manera predeterminada, el nombre de la carpeta será "Favoritos administrados", pero puede cambiarlo si agrega a la lista de favoritos un diccionario que contenga la clave "toplevel_name" con el nombre de la carpeta deseada como valor.

Los favoritos administrados no se sincronizan con la cuenta de usuario y las extensiones no pueden modificarlos.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Diccionario

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: ManagedFavorites
  - Nombre de la directiva de grupos: Configurar favoritos
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: ManagedFavorites
  - Tipo de valor: REG_SZ
  ##### Valor de ejemplo:
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


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: ManagedFavorites
  - Valor de ejemplo:
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
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### ManagedSearchEngines
  #### Administrar motores de búsqueda
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Te permite configurar una lista de hasta 10 motores de búsqueda, uno de los cuales debe marcarse como el motor de búsqueda predeterminado.
No es necesario especificar la codificación para ningún motor de búsqueda.

Si se habilita esta directiva, los usuarios no podrán agregar, quitar ni cambiar ningún motor de búsqueda en la lista. Los usuarios pueden establecer su motor de búsqueda predeterminado en cualquier motor de búsqueda de la lista.

Si se deshabilita o no se configura esta directiva, los usuarios podrán modificar la lista de motores de búsqueda según lo deseen.

Si se establece la directiva [DefaultSearchProviderSearchURL](#defaultsearchprovidersearchurl), se omitirá esta directiva (ManagedSearchEngines). El usuario debe reiniciar el explorador para terminar de aplicar esta directiva.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: No - Requiere reiniciar el explorador

  #### Tipo de datos:
  Diccionario

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: ManagedSearchEngines
  - Nombre de la directiva de grupos: Administrar motores de búsqueda
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: ManagedSearchEngines
  - Tipo de valor: REG_SZ
  ##### Valor de ejemplo:
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


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: ManagedSearchEngines
  - Valor de ejemplo:
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
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### MaxConnectionsPerProxy
  #### Número máximo de conexiones simultáneas al servidor proxy
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Especifica el número máximo de conexiones simultáneas al servidor proxy.

Algunos servidores proxy no pueden controlar un gran número de conexiones simultáneas por cliente; esto se puede solucionar estableciendo esta directiva en un valor menor.

El valor de esta directiva debe ser inferior a 100 y superior a 6. El valor predeterminado es 32.

Se sabe que algunas aplicaciones web consumen muchas conexiones con GET que no responden, reducir el número máximo de conexiones por debajo de 32 puede provocar que las redes del explorador no respondan si hay demasiadas aplicaciones web de este tipo abiertas.

Si no se configura esta directiva, se usa el valor predeterminado (32).

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: No - Requiere reiniciar el explorador

  #### Tipo de datos:
  Entero

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: MaxConnectionsPerProxy
  - Nombre de la directiva de grupos: Número máximo de conexiones simultáneas al servidor proxy
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: MaxConnectionsPerProxy
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000020
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: MaxConnectionsPerProxy
  - Valor de ejemplo:
``` xml
<integer>32</integer>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### MediaRouterCastAllowAllIPs
  #### Permitir que Google Cast se conecte con dispositivos de Cast en todas las direcciones IP
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Habilite esta directiva para permitir que Google Cast se conecte a dispositivos de Cast en todas las direcciones IP, no solo direcciones privadas de RFC1918/RFC4193.

Deshabilite esta directiva para restringir Google Cast a los dispositivos de Cast en direcciones privadas de RFC1918/RFC4193.

Si no se configura esta directiva, Google Cast se conectará a dispositivos de Cast solo en direcciones privadas de RFC1918/RFC4193, a menos que se habilite la característica CastAllowAllIPs.

Si la directiva [EnableMediaRouter](#enablemediarouter) está deshabilitada, esta directiva no tiene ningún efecto.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Booleano

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: MediaRouterCastAllowAllIPs
  - Nombre de la directiva de grupos: Permitir que Google Cast se conecte con dispositivos de Cast en todas las direcciones IP
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: MediaRouterCastAllowAllIPs
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000000
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: MediaRouterCastAllowAllIPs
  - Valor de ejemplo:
``` xml
<false/>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### MetricsReportingEnabled
  #### Habilitar el uso y los informes de datos relacionados con el bloqueo
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  For Windows 10 Beta and Stable channels of Microsoft Edge, this policy when configured will override the Windows diagnostic data setting for collection or non-collection of Microsoft Edge usage and crash related data ([https://go.microsoft.com/fwlink/?linkid=2099569](https://go.microsoft.com/fwlink/?linkid=2099569)).

This policy enables reporting of usage and crash-related data about Microsoft Edge to Microsoft and prevents users from changing this setting.

Enable this policy to send reporting of usage and crash-related data to Microsoft. Disable this policy to not send the data to Microsoft. In both cases, users can't change or override the setting.

On Windows 10, Beta and Stable channels, this policy controls usage data. Crash-related data is determined by the Windows diagnostic data setting. If this policy is not configured, Microsoft Edge will default to the Windows diagnostic data setting.

On Windows 10, Canary and Dev channels, this policy controls usage and crash related data. If this policy is not configured, Microsoft Edge will default to the user's preference.

On Windows 7, 8, and Mac this policy controls usage and crash related data. If this policy is not configured, Microsoft Edge will default to the user's preference.

This policy is available only on Windows instances that are joined to a Microsoft Active Directory domain or Windows 10 Pro or Enterprise instances enrolled for device management.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: No - Requiere reiniciar el explorador

  #### Tipo de datos:
  Booleano

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: MetricsReportingEnabled
  - Nombre de la directiva de grupos: Habilitar el uso y los informes de datos relacionados con el bloqueo
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: MetricsReportingEnabled
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000001
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: MetricsReportingEnabled
  - Valor de ejemplo:
``` xml
<true/>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### NetworkPredictionOptions
  #### Habilitar la predicción de red
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Habilita la predicción de red e impide que los usuarios cambien esta configuración.

Esto controla la captura previa de DNS, la conexión previa de TCP y SSL, y la representación previa de páginas web.

Si no se configura esta directiva, la predicción de red estará habilitada pero el usuario podrá cambiarla.

* 0 = Predecir acciones de red en cualquier conexión de red.

* 2 = No predecir acciones de red en ninguna conexión de red

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: Sí
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Entero

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: NetworkPredictionOptions
  - Nombre de la directiva de grupos: Habilitar la predicción de red
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): Plantillas administrativas/Microsoft Edge - Configuración predeterminada (los usuarios pueden cambiarla)/
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): SOFTWARE\Policies\Microsoft\Edge\Recomendada
  - Nombre del valor: NetworkPredictionOptions
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000001
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: NetworkPredictionOptions
  - Valor de ejemplo:
``` xml
<integer>1</integer>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### NonRemovableProfileEnabled
  #### Configurar si un usuario siempre tiene un perfil predeterminado con sesión iniciada automáticamente con su cuenta profesional o educativa
  >Versiones admitidas: Microsoft Edge en Windows desde la versión 78 o posterior

  #### Descripción
  Esta directiva determina si el perfil de Microsoft Edge que inició sesión automáticamente con una cuenta profesional o educativa de un usuario es extraíble.

Si habilita o no configura esta directiva, se creará un perfil no extraíble con la cuenta profesional o educativa del usuario en Windows. No se puede cerrar la sesión de este perfil ni quitarlo.

Cuando se deshabilita esta directiva, el usuario puede cerrar la sesión o quitar el perfil que ha iniciado sesión automáticamente con la cuenta profesional o educativa de Windows.

Si quiere deshabilitar completamente el inicio de sesión con el explorador, use la directiva 'BrowserSignIn'.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Booleano

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: NonRemovableProfileEnabled
  - Nombre de la directiva de grupos: Configurar si un usuario siempre tiene un perfil predeterminado con sesión iniciada automáticamente con su cuenta profesional o educativa
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: NonRemovableProfileEnabled
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000001
```


  

  [Volver al principio](#microsoft-edge:-directivas)

  ### OverrideSecurityRestrictionsOnInsecureOrigin
  #### Controlar dónde se aplican restricciones de seguridad en los orígenes no seguros
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Especifica una lista de orígenes (URL) o patrones de nombre de host (como "*.contoso.com") en los que no se aplican restricciones de seguridad en los orígenes no seguros.

Esta directiva permite especificar orígenes permitidos para las aplicaciones heredadas que no pueden implementar TLS o configurar un servidor de almacenamiento provisional para el desarrollo web interno de modo que los desarrolladores puedan probar las características que requieren contextos seguros sin tener que implementar TLS en el servidor de almacenamiento provisional. Esta directiva también impide que el origen esté etiquetado como "No seguro" en el multicuadro.

Establecer una lista de direcciones URL en esta directiva tiene el mismo efecto que establecer la marca de línea de comandos '--unsafely-treat-insecure-origin-as-secure' en una lista separada por comas de las mismas direcciones URL. Si se habilita esta directiva, se invalidará la marca de línea de comandos.

Para obtener más información acerca de los contextos de seguridad, consulta https://www.w3.org/TR/secure-contexts/.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: No - Requiere reiniciar el explorador

  #### Tipo de datos:
  Lista de cadenas

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: OverrideSecurityRestrictionsOnInsecureOrigin
  - Nombre de la directiva de grupos: Controlar dónde se aplican restricciones de seguridad en los orígenes no seguros
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge\OverrideSecurityRestrictionsOnInsecureOrigin
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: 1, 2, 3, ...
  - Tipo de valor: lista de REG_SZ
  ##### Valor de ejemplo:
```
SOFTWARE\Policies\Microsoft\Edge\OverrideSecurityRestrictionsOnInsecureOrigin\0 = "http://testserver.contoso.com/"
SOFTWARE\Policies\Microsoft\Edge\OverrideSecurityRestrictionsOnInsecureOrigin\1 = "*.contoso.com"

```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: OverrideSecurityRestrictionsOnInsecureOrigin
  - Valor de ejemplo:
``` xml
<array>
  <string>http://testserver.contoso.com/</string>
  <string>*.contoso.com</string>
</array>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### PinningWizardAllowed
  #### Allow Pin to taskbar wizard
  >Versiones admitidas: Microsoft Edge en Windows desde la versión 80 o posterior

  #### Descripción
  Microsoft Edge uses the Pin to taskbar wizard to help users pin suggested sites to the taskbar. The Pin to taskbar wizard feature is enabled by default and accessible to the user through the Settings and more menu.

If you enable this policy or don't configure it, users can call the Pin to taskbar wizard from the Settings and More menu. The wizard can also be called via a protocol launch.

If you disable this policy, the Pin to taskbar wizard is disabled in the menu and cannot be called via a protocol launch.

User settings to enable or disable the Pin to taskbar wizard aren't available.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: No - Requiere reiniciar el explorador

  #### Tipo de datos:
  Booleano

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: PinningWizardAllowed
  - Nombre de la directiva de grupos: Allow Pin to taskbar wizard
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: PinningWizardAllowed
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000000
```


  

  [Volver al principio](#microsoft-edge:-directivas)

  ### ProactiveAuthEnabled
  #### Habilitar autenticación proactiva
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Permite configurar si se debe activar la autenticación proactiva.

Si se habilita esta directiva, Microsoft Edge intentará autenticar proactivamente el usuario que inició sesión con los servicios Microsoft. A intervalos regulares, Microsoft Edge realiza comprobaciones con un servicio en línea para obtener un manifiesto actualizado que contenga la configuración que rige cómo hacerlo.

Si se deshabilita esta directiva, Microsoft Edge no intentará autenticar proactivamente el usuario que ha iniciado sesión con los servicios Microsoft. Microsoft Edge ya no realizará comprobaciones con un servicio en línea para obtener un manifiesto actualizado que contenga la configuración para hacerlo.

Si no se configura esta directiva, se activará la autenticación proactiva.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: No - Requiere reiniciar el explorador

  #### Tipo de datos:
  Booleano

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: ProactiveAuthEnabled
  - Nombre de la directiva de grupos: Habilitar autenticación proactiva
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: ProactiveAuthEnabled
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000001
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: ProactiveAuthEnabled
  - Valor de ejemplo:
``` xml
<true/>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### PromotionalTabsEnabled
  #### Habilitar el contenido promocional en toda la pestaña
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Controle la presentación de contenido educativo o promocional de pestaña completa. Esta configuración controla la presentación de las páginas principales que ayudan a los usuarios a iniciar sesión en Microsoft Edge, elegir su explorador predeterminado o descubrir características del producto.

Si se habilita esta directiva (si se establece en true) o si no se configura, Microsoft Edge podrá mostrar contenido de pestaña completa a los usuarios para proporcionar información acerca del producto.

Si se deshabilita esta directiva (si se establece en false), Microsoft Edge no podrá mostrar contenido de pestaña completa a los usuarios.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Booleano

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: PromotionalTabsEnabled
  - Nombre de la directiva de grupos: Habilitar el contenido promocional en toda la pestaña
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: PromotionalTabsEnabled
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000000
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: PromotionalTabsEnabled
  - Valor de ejemplo:
``` xml
<false/>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### PromptForDownloadLocation
  #### Preguntar dónde guardar los archivos descargados
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Establecer si se debe preguntar dónde guardar un archivo antes de descargarlo.

Si se habilita esta directiva, se le preguntará al usuario dónde quiere guardar cada archivo antes de descargarlo; si no se configura, los archivos se guardan automáticamente en la ubicación predeterminada, sin preguntarle al usuario.

Si no se configura esta directiva, el usuario podrá cambiar esta configuración.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Booleano

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: PromptForDownloadLocation
  - Nombre de la directiva de grupos: Preguntar dónde guardar los archivos descargados
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: PromptForDownloadLocation
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000000
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: PromptForDownloadLocation
  - Valor de ejemplo:
``` xml
<false/>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### QuicAllowed
  #### Permitir protocolo QUIC
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Permite el uso del protocolo QUIC en Microsoft Edge.

Si se habilita esta directiva o no se configura, se permitirá el protocolo QUIC.

Si se deshabilita esta directiva, se bloqueará el protocolo QUIC.

QUIC es un protocolo de red de capa de transporte que puede mejorar el rendimiento de las aplicaciones web que usan actualmente TCP.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: No - Requiere reiniciar el explorador

  #### Tipo de datos:
  Booleano

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: QuicAllowed
  - Nombre de la directiva de grupos: Permitir protocolo QUIC
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: QuicAllowed
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000001
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: QuicAllowed
  - Valor de ejemplo:
``` xml
<true/>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### RelaunchNotification
  #### Notificar al usuario que se recomienda o se requiere reiniciar el explorador para las actualizaciones pendientes
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Notificar a los usuarios que deben reiniciar Microsoft Edge para aplicar una actualización pendiente.

Si no se configura esta directiva, Microsoft Edge agrega un icono de reciclaje en el extremo derecho de la barra de menús superior para pedir a los usuarios que reinicien el explorador y aplicar la actualización.

Si se habilita esta directiva y se establece con el valor "Recomendado" (1), una advertencia periódica indicará a los usuarios que se recomienda reiniciar el explorador. Los usuarios pueden descartar esta advertencia y aplazar el reinicio.

Si se establece la directiva en "Requerido" (2), una advertencia periódica indicará a los usuarios que el explorador se reiniciará automáticamente tras un período de notificación. El período predeterminado es de siete días. Se puede configurar este período con la directiva [RelaunchNotificationPeriod](#relaunchnotificationperiod).

La sesión del usuario se restaurará cuando se reinicie el explorador.

* Recomendado (1) = Mostrar un aviso periódico al usuario para indicar que se recomienda reiniciar

* Necesario (2) = Mostrar un aviso periódico al usuario para indicar que es necesario reiniciar

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Entero

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: RelaunchNotification
  - Nombre de la directiva de grupos: Notificar al usuario que se recomienda o se requiere reiniciar el explorador para las actualizaciones pendientes
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: RelaunchNotification
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000001
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: RelaunchNotification
  - Valor de ejemplo:
``` xml
<integer>1</integer>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### RelaunchNotificationPeriod
  #### Establecer el período de tiempo para las notificaciones de actualización
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Allows you to set the time period, in milliseconds, over which users are notified that Microsoft Edge must be relaunched or that a Microsoft Edge OS device must be restarted to apply a pending update.

Over this time period, the user will be repeatedly informed of the need for an update. For Microsoft Edge OS devices, a restart notification appears in the system tray according to the RelaunchHeadsUpPeriod policy. For Microsoft Edge browsers, the app menu changes to indicate that a relaunch is needed once one third of the notification period passes. This notification changes color once two thirds of the notification period passes, and again once the full notification period has passed. The additional notifications enabled by the RelaunchNotification policy follow this same schedule.

If not set, the default period of 604800000 milliseconds (one week) is used.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Entero

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: RelaunchNotificationPeriod
  - Nombre de la directiva de grupos: Establecer el período de tiempo para las notificaciones de actualización
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: RelaunchNotificationPeriod
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x240c8400
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: RelaunchNotificationPeriod
  - Valor de ejemplo:
``` xml
<integer>604800000</integer>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### RendererCodeIntegrityEnabled
  #### Habilitar la integridad del código del procesador
  >Versiones admitidas: Microsoft Edge en Windows desde la versión 78 o posterior

  #### Descripción
  Si se habilita o se deja esta directiva sin establecer, se habilita la integridad del código de representador. Esta directiva solo se debe deshabilitar si se encuentran problemas de compatibilidad con el software de terceros que deben ejecutarse dentro de los procesos del representador de Microsoft Edge.

La deshabilitación de esta directiva tiene un efecto perjudicial en la estabilidad y la seguridad de Microsoft Edge porque se permitirá que el código desconocido y potencialmente hostil se cargue dentro de los procesadores del representador de Microsoft Edge.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: No - Requiere reiniciar el explorador

  #### Tipo de datos:
  Booleano

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: RendererCodeIntegrityEnabled
  - Nombre de la directiva de grupos: Habilitar la integridad del código del procesador
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: RendererCodeIntegrityEnabled
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000000
```


  

  [Volver al principio](#microsoft-edge:-directivas)

  ### RequireOnlineRevocationChecksForLocalAnchors
  #### Especificar si las comprobaciones CRL/OCSP en línea son obligatorias para los delimitadores locales de confianza
  >Versiones admitidas: Microsoft Edge en Windows desde la versión 77 o posterior

  #### Descripción
  Controle si las comprobaciones de revocación en línea (comprobaciones OCSP/CRL) son obligatorias. Si Microsoft Edge no puede obtener información de estado de revocación, estos certificados se tratan como revocados ("error no recuperable").

Si se habilita esta directiva, Microsoft Edge siempre realizará la comprobación de revocación de los certificados de servidor que se validan correctamente y están firmados por certificados de entidad de certificación instalados localmente.

Si no se configura o si se deshabilita esta directiva, Microsoft Edge usará la configuración de comprobación de revocación en línea existente.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Booleano

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: RequireOnlineRevocationChecksForLocalAnchors
  - Nombre de la directiva de grupos: Especificar si las comprobaciones CRL/OCSP en línea son obligatorias para los delimitadores locales de confianza
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: RequireOnlineRevocationChecksForLocalAnchors
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000000
```


  

  [Volver al principio](#microsoft-edge:-directivas)

  ### ResolveNavigationErrorsUseWebService
  #### Habilitar la resolución de errores de navegación mediante un servicio web
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Permitir que Microsoft Edge emita una conexión sin datos a un servicio web para sondear las redes para la conectividad en casos como la Wi-Fi de hoteles y aeropuertos.

Si se habilita esta directiva, se usará un servicio web para las pruebas de conectividad de red.

Si se deshabilita esta directiva, Microsoft Edge usará las API nativas para intentar resolver los problemas de navegación y conectividad de red.

**Nota**: Excepto en Windows 8 y versiones posteriores de Windows, Microsoft Edge *siempre* usa API nativas para resolver problemas de conectividad.

Si no se configura esta directiva, Microsoft Edge respeta la preferencia del usuario que está establecida en Servicios en edge://settings/privacy.
En concreto, hay un botón de alternancia, **Usar un servicio web para ayudar a resolver errores de navegación**, que el usuario puede activar o desactivar. Tenga en cuenta que si está habilitada esta directiva (ResolveNavigationErrorsUseWebService), la configuración **Usar un servicio web para ayudar a resolver errores de navegación** estará activada, pero el usuario no podrá cambiar la configuración mediante el botón de alternancia. Si se deshabilita esta directiva, la configuración **Usar un servicio web para ayudar a resolver errores de navegación** estará desactivada y el usuario no podrá cambiar la configuración mediante el botón de alternancia.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: Sí
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Booleano

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: ResolveNavigationErrorsUseWebService
  - Nombre de la directiva de grupos: Habilitar la resolución de errores de navegación mediante un servicio web
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): Plantillas administrativas/Microsoft Edge - Configuración predeterminada (los usuarios pueden cambiarla)/
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): SOFTWARE\Policies\Microsoft\Edge\Recomendada
  - Nombre del valor: ResolveNavigationErrorsUseWebService
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000001
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: ResolveNavigationErrorsUseWebService
  - Valor de ejemplo:
``` xml
<true/>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### RestrictSigninToPattern
  #### Restringir las cuentas que pueden usarse como cuentas principales de Microsoft Edge
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Determina qué cuentas se pueden establecer como cuentas principales del explorador en Microsoft Edge (la cuenta que se selecciona durante el flujo de optar por recibir sincronización).

Si un usuario intenta establecer una cuenta principal del explorador con un nombre de usuario que no coincide con este patrón, se bloqueará y verá un mensaje de error correspondiente.

Si no se configura esta directiva o se deja en blanco, los usuarios podrán establecer cualquier cuenta como una cuenta principal del explorador en Microsoft Edge.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Cadena

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: RestrictSigninToPattern
  - Nombre de la directiva de grupos: Restringir las cuentas que pueden usarse como cuentas principales de Microsoft Edge
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: RestrictSigninToPattern
  - Tipo de valor: REG_SZ
  ##### Valor de ejemplo:
```
".*@contoso.com"
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: RestrictSigninToPattern
  - Valor de ejemplo:
``` xml
<string>.*@contoso.com</string>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### RunAllFlashInAllowMode
  #### Extender la configuración de contenidos de Adobe Flash a todos los contenido
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Si se habilita esta directiva, se ejecutarán todos los contenidos de Adobe Flash incorporados en sitios web que están establecidos para permitir Adobe Flash en la configuración de contenido (ya sea por parte del usuario o de la directiva de empresa). Esto incluye contenidos de otros orígenes o contenidos pequeños.

Para controlar los sitios web que pueden ejecutar Adobe Flash, consulta las especificaciones de las directivas [DefaultPluginsSetting](#defaultpluginssetting), [PluginsAllowedForUrls](#pluginsallowedforurls) y [PluginsBlockedForUrls](#pluginsblockedforurls).

Si se deshabilita esta directiva o no se configura, los contenidos de Adobe Flash de otros orígenes (de sitios que no están especificados en las directivas de las tres políticas mencionadas antes) o los contenidos pequeños podrían estar bloqueados.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Booleano

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: RunAllFlashInAllowMode
  - Nombre de la directiva de grupos: Extender la configuración de contenidos de Adobe Flash a todos los contenido
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: RunAllFlashInAllowMode
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000001
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: RunAllFlashInAllowMode
  - Valor de ejemplo:
``` xml
<true/>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### SSLErrorOverrideAllowed
  #### Permitir que los usuarios continúen desde la página de advertencia de HTTPS
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Microsoft Edge muestra una página de advertencia cuando los usuarios visitan sitios que presentan errores SSL.

Si se habilita o no se configura (valor predeterminado) esta directiva, los usuarios podrán hacer clic en estas páginas de advertencia.

Si se deshabilita esta directiva, los usuarios no podrán hacer clic en ninguna página de advertencia.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Booleano

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: SSLErrorOverrideAllowed
  - Nombre de la directiva de grupos: Permitir que los usuarios continúen desde la página de advertencia de HTTPS
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: SSLErrorOverrideAllowed
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000001
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: SSLErrorOverrideAllowed
  - Valor de ejemplo:
``` xml
<true/>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### SSLVersionMin
  #### Versión mínima de TLS habilitada
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Establece la versión mínima admitida de SSL. Si no se configura esta directiva, Microsoft Edge usa una versión mínima predeterminada, TLS 1.0.

Si se habilita esta directiva, se puede establecer la versión mínima en uno de los siguientes valores: "tls1", "tls1.1" or "tls1.2". Cuando se establece, Microsoft Edge no usará ninguna versión de SSL/TLS inferior a la versión especificada. Se omitirá cualquier valor no reconocido.

* "tls1" = TLS 1.0

* "tls1.1" = TLS 1.1

* "tls1.2" = TLS 1.2

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Cadena

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: SSLVersionMin
  - Nombre de la directiva de grupos: Versión mínima de TLS habilitada
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: SSLVersionMin
  - Tipo de valor: REG_SZ
  ##### Valor de ejemplo:
```
"tls1"
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: SSLVersionMin
  - Valor de ejemplo:
``` xml
<string>tls1</string>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### SavingBrowserHistoryDisabled
  #### Deshabilitar guardar el historial del explorador
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Deshabilita guardar el historial del explorador e impide que los usuarios cambien esta configuración.

Si se habilita esta directiva, el historial de exploración no se guardará. Esto también deshabilita la sincronización de pestañas.

Si se deshabilita esta directiva o no se configura, se guardará el historial de exploración.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Booleano

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: SavingBrowserHistoryDisabled
  - Nombre de la directiva de grupos: Deshabilitar guardar el historial del explorador
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: SavingBrowserHistoryDisabled
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000001
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: SavingBrowserHistoryDisabled
  - Valor de ejemplo:
``` xml
<true/>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### SearchSuggestEnabled
  #### Habilitar sugerencias de búsqueda
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Habilita las sugerencias de búsqueda web en la lista de sugerencias automáticas y la barra de direcciones de Microsoft Edge e impide que los usuarios cambien esta directiva.

Si se habilita esta directiva, se usarán las sugerencias de búsqueda web.

Si se deshabilita esta directiva, las sugerencias de búsqueda web no se usarán nunca, pero seguirán apareciendo las sugerencias de favoritos e historial locales. Si se deshabilita esta directiva, no se incluirán en telemetría a Microsoft ni los caracteres escritos ni las direcciones URL visitadas.

Si esta directiva se deja no establecida, las sugerencias de búsqueda estarán habilitadas, pero el usuario podrá modificarlas.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: Sí
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Booleano

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: SearchSuggestEnabled
  - Nombre de la directiva de grupos: Habilitar sugerencias de búsqueda
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): Plantillas administrativas/Microsoft Edge - Configuración predeterminada (los usuarios pueden cambiarla)/
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): SOFTWARE\Policies\Microsoft\Edge\Recomendada
  - Nombre del valor: SearchSuggestEnabled
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000001
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: SearchSuggestEnabled
  - Valor de ejemplo:
``` xml
<true/>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### SecurityKeyPermitAttestation
  #### Sitios web o dominios que no necesitan permiso para usar la atestación de clave de seguridad directa
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Especifica los sitios web y dominios que no necesitan permiso explícito del usuario cuando se solicitan certificados de atestación de claves de seguridad. Además, se envía una señal a la clave de seguridad que indica que puede usar la atestación individual. Sin esto, se le preguntará a los usuarios cada vez que un sitio solicite la atestación de claves de seguridad.

Los sitios (por ejemplo, https://contoso.com/some/path) solo coinciden como U2F AppIDs. Los dominios (por ejemplo, contoso.com) solo coinciden como id. de webauthn RP. Para que tanto las API de U2F y de webauthn estén cubiertas en un sitio determinado, tienes que indicar el dominio y la dirección URL de appID.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Lista de cadenas

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: SecurityKeyPermitAttestation
  - Nombre de la directiva de grupos: Sitios web o dominios que no necesitan permiso para usar la atestación de clave de seguridad directa
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge\SecurityKeyPermitAttestation
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: 1, 2, 3, ...
  - Tipo de valor: lista de REG_SZ
  ##### Valor de ejemplo:
```
SOFTWARE\Policies\Microsoft\Edge\SecurityKeyPermitAttestation\0 = "https://contoso.com"

```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: SecurityKeyPermitAttestation
  - Valor de ejemplo:
``` xml
<array>
  <string>https://contoso.com</string>
</array>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### SendIntranetToInternetExplorer
  #### Enviar todos los sitios de la intranet a Internet Explorer
  >Versiones admitidas: Microsoft Edge en Windows desde la versión 77 o posterior

  #### Descripción
  Para obtener instrucciones sobre cómo configurar la experiencia óptima para el modo de Internet Explorer, consulte [https://go.microsoft.com/fwlink/?linkid=2094210](https://go.microsoft.com/fwlink/?linkid=2094210)

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: No - Requiere reiniciar el explorador

  #### Tipo de datos:
  Booleano

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: SendIntranetToInternetExplorer
  - Nombre de la directiva de grupos: Enviar todos los sitios de la intranet a Internet Explorer
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: SendIntranetToInternetExplorer
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000001
```


  

  [Volver al principio](#microsoft-edge:-directivas)

  ### SendSiteInfoToImproveServices
  #### Enviar información del sitio para mejorar los servicios Microsoft
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Para los canales beta y estable de Windows 10 de Microsoft Edge, cuando se configura esta directiva, se invalidará la configuración de datos de diagnóstico de Windows para la recopilación o no recopilación de información de exploración del sitio web de Microsoft Edge ([https://go.microsoft.com/fwlink/?linkid=2099569](https://go.microsoft.com/fwlink/?linkid=2099569)).

La configuración de esta directiva le permite decidir si los usuarios pueden enviar información acerca de los sitios web que visitan en Microsoft Edge a Microsoft para mejorar servicios, como la búsqueda.

Si se habilita esta directiva, la información acerca de los sitios web visitados en Microsoft Edge se enviará a Microsoft.

Si se deshabilita esta directiva, la información acerca de los sitios web visitados en Microsoft Edge no se enviará a Microsoft.

En los canales beta y estable de Windows 10, esta directiva controla el envío de información acerca de los sitios web que visitan los usuarios. Si no se configura esta directiva, Microsoft Edge tendrá la configuración de datos de diagnóstico de Windows predeterminada.

En los canales Canary y Dev de Windows 10, esta directiva controla el envío de información acerca de los sitios web que visitan los usuarios. Si no se configura esta directiva, Microsoft Edge tendrá la preferencia predeterminada del usuario.

En Windows 7, 8 y Mac, esta directiva controla el envío de información acerca de los sitios web que visitan los usuarios. Si no se configura esta directiva, Microsoft Edge tendrá la preferencia predeterminada del usuario.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: No - Requiere reiniciar el explorador

  #### Tipo de datos:
  Booleano

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: SendSiteInfoToImproveServices
  - Nombre de la directiva de grupos: Enviar información del sitio para mejorar los servicios Microsoft
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: SendSiteInfoToImproveServices
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000000
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: SendSiteInfoToImproveServices
  - Valor de ejemplo:
``` xml
<false/>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### ShowOfficeShortcutInFavoritesBar
  #### Mostrar el acceso directo de Microsoft Office en la barra de favoritos
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Especifica si se incluye un acceso directo a Office.com en la barra de favoritos. Para los usuarios que han iniciado sesión en Microsoft Edge el acceso directo lleva a los usuarios a sus documentos y aplicaciones de Microsoft Office.

Si esta directiva está habilitada o no está configurada, los usuarios podrán elegir si quieren ver el acceso directo cambiando el botón de alternancia en los favoritos de la barra del menú contextual.

Si la directiva está deshabilitada, no se mostrará el acceso directo.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Booleano

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: ShowOfficeShortcutInFavoritesBar
  - Nombre de la directiva de grupos: Mostrar el acceso directo de Microsoft Office en la barra de favoritos
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: ShowOfficeShortcutInFavoritesBar
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000000
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: ShowOfficeShortcutInFavoritesBar
  - Valor de ejemplo:
``` xml
<false/>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### SignedHTTPExchangeEnabled
  #### Habilitar la compatibilidad con Exchange firmado de HTTP (SXG)
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 78 o posterior

  #### Descripción
  Habilitar la compatibilidad con HTTP de Exchange firmado (SXG).

Si no se configura o no se habilita esta directiva, Microsoft Edge aceptará contenido web servidos como HTTP de Exchange firmados.

Si esta directiva se establece en deshabilitada, no se cargarán los HTTP de Exchange firmados.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Booleano

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: SignedHTTPExchangeEnabled
  - Nombre de la directiva de grupos: Habilitar la compatibilidad con Exchange firmado de HTTP (SXG)
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: SignedHTTPExchangeEnabled
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000001
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: SignedHTTPExchangeEnabled
  - Valor de ejemplo:
``` xml
<true/>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### SitePerProcess
  #### Habilitar el aislamiento de sitios para cada sitio
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  La directiva [SitePerProcess](#siteperprocess) se puede usar para impedir que los usuarios opten por el comportamiento predeterminado de aislar todos los sitios. Tenga en cuenta que también puede usar la directiva [IsolateOrigins](#isolateorigins) para aislar orígenes adicionales y más específicos.
Si se habilita esta directiva, los usuarios no pueden optar por el comportamiento predeterminado en el que cada sitio se ejecuta en su propio proceso.
Si se deshabilita o no se configura esta directiva, un usuario puede optar por el aislamiento del sitio. (Por ejemplo, con la entrada "Deshabilitar aislamiento de sitio" en edge://flags.) Si se deshabilita o no se configura la directiva, no se desactivará el aislamiento del sitio.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: No - Requiere reiniciar el explorador

  #### Tipo de datos:
  Booleano

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: SitePerProcess
  - Nombre de la directiva de grupos: Habilitar el aislamiento de sitios para cada sitio
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: SitePerProcess
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000001
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: SitePerProcess
  - Valor de ejemplo:
``` xml
<true/>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### SpellcheckEnabled
  #### Habilitar corrector ortográfico
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Si se habilita o no se configura esta directiva, el usuario puede usar el corrector ortográfico.

Si se deshabilita esta directiva, el usuario no puede usar el corrector ortográfico y también se deshabilitan las directivas [SpellcheckLanguage](#spellchecklanguage) y [SpellcheckLanguageBlocklist](#spellchecklanguageblocklist).

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Booleano

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: SpellcheckEnabled
  - Nombre de la directiva de grupos: Habilitar corrector ortográfico
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: SpellcheckEnabled
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000000
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: SpellcheckEnabled
  - Valor de ejemplo:
``` xml
<false/>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### SpellcheckLanguage
  #### Habilitar los idiomas de corrección ortográfica específicos
  >Versiones admitidas: Microsoft Edge en Windows desde la versión 77 o posterior

  #### Descripción
  Habilita diferentes idiomas para la corrección ortográfica. Se omitirá cualquier idioma que especifique que no se reconozca.

Si se habilita esta directiva, la corrección ortográfica se habilitará para los idiomas especificados, así como para los idiomas que el usuario haya habilitado.

Si no se configura o si se deshabilita esta directiva, no habrá ningún cambio en las preferencias de corrección ortográfica del usuario.

Si la directiva [SpellcheckEnabled](#spellcheckenabled) está deshabilitada, esta directiva no tendrá efecto.

Si un idioma está incluido en la directiva 'SpellcheckLanguage' y en la directiva [SpellcheckLanguageBlocklist](#spellchecklanguageblocklist), el idioma de corrección ortográfica estará habilitado.

Los idiomas compatibles son: af, bg, ca, cs, cy, da, de, el, en-AU, en-CA, en-GB, en-US, es, es-419, es-AR, es-ES, es-MX, es-US, et, fa, fo, fr, he, hi, hr, hu, id, it, ko, lt, lv, nb, nl, pl, pt-BR, pt-PT, ro, ru, sh, sk, sl, sq, sr, sv, ta, tg, tr, uk, vi.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Lista de cadenas

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: SpellcheckLanguage
  - Nombre de la directiva de grupos: Habilitar los idiomas de corrección ortográfica específicos
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge\SpellcheckLanguage
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: 1, 2, 3, ...
  - Tipo de valor: lista de REG_SZ
  ##### Valor de ejemplo:
```
SOFTWARE\Policies\Microsoft\Edge\SpellcheckLanguage\0 = "fr"
SOFTWARE\Policies\Microsoft\Edge\SpellcheckLanguage\1 = "es"

```


  

  [Volver al principio](#microsoft-edge:-directivas)

  ### SpellcheckLanguageBlocklist
  #### Forzar deshabilitar idiomas de corrección ortográfica
  >Versiones admitidas: Microsoft Edge en Windows desde la versión 78 o posterior

  #### Descripción
  Fuerza la deshabilitación de idiomas para la revisión ortográfica. Se omitirán los idiomas no reconocidos de la lista.

Si se habilita esta directiva, se deshabilitará la revisión ortográfica para los idiomas especificados. El usuario puede seguir habilitando o deshabilitando la revisión ortográfica para los idiomas que no estén en la lista.

Si no se establece esta directiva o se deshabilita, no se cambiarán las preferencias de revisión ortográfica del usuario.

Si la directiva [SpellcheckEnabled](#spellcheckenabled) está establecida en deshabilitada, esta directiva no tendrá ningún efecto.

Si un idioma se incluye en las directivas [SpellcheckLanguage](#spellchecklanguage) y 'SpellcheckLanguageBlocklist', se habilitará el idioma para la corrección ortográfica.

Los idiomas admitidos actualmente son: af, bg, ca, cs, da, de, el, en-AU, en-CA, en-GB, en-US, es, es-419, es-AR, es-ES, es-MX, es-US, et, fa, fo, fr, he, hi, hr, hu, id, it, ko, lt, lv, nb, nl, pl, pt-BR, pt-PT, ro, ru, sh, sk, sl, sq, sr, sv, ta, tg, tr, uk, vi.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Lista de cadenas

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: SpellcheckLanguageBlocklist
  - Nombre de la directiva de grupos: Forzar deshabilitar idiomas de corrección ortográfica
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge\SpellcheckLanguageBlocklist
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: 1, 2, 3, ...
  - Tipo de valor: lista de REG_SZ
  ##### Valor de ejemplo:
```
SOFTWARE\Policies\Microsoft\Edge\SpellcheckLanguageBlocklist\0 = "fr"
SOFTWARE\Policies\Microsoft\Edge\SpellcheckLanguageBlocklist\1 = "es"

```


  

  [Volver al principio](#microsoft-edge:-directivas)

  ### SuppressUnsupportedOSWarning
  #### Suprimir la advertencia de sistema operativo no compatible
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Suprime la advertencia que aparece cuando Microsoft Edge se está ejecutando en un equipo o un sistema operativo que ya no se admite.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: No - Requiere reiniciar el explorador

  #### Tipo de datos:
  Booleano

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: SuppressUnsupportedOSWarning
  - Nombre de la directiva de grupos: Suprimir la advertencia de sistema operativo no compatible
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: SuppressUnsupportedOSWarning
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000001
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: SuppressUnsupportedOSWarning
  - Valor de ejemplo:
``` xml
<true/>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### SyncDisabled
  #### Deshabilitar la sincronización de datos mediante los servicios de sincronización de Microsoft
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Deshabilita la sincronización de datos en Microsoft Edge e impide que los usuarios modifiquen esta configuración.

Si no se establece esta directiva, los usuarios podrán activar o desactivar la sincronización.

No se debe habilitar esta directiva cuando está activada la directiva 'RoamingProfileSupportEnabled', debido a que 'RoamingProfileSupportEnabled' duplica la funcionalidad de sincronización.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: Sí
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Booleano

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: SyncDisabled
  - Nombre de la directiva de grupos: Deshabilitar la sincronización de datos mediante los servicios de sincronización de Microsoft
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): Plantillas administrativas/Microsoft Edge - Configuración predeterminada (los usuarios pueden cambiarla)/
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): SOFTWARE\Policies\Microsoft\Edge\Recomendada
  - Nombre del valor: SyncDisabled
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000001
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: SyncDisabled
  - Valor de ejemplo:
``` xml
<true/>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### TabFreezingEnabled
  #### Permitir la inmovilización de pestañas en segundo plano
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 79 o posterior

  #### Descripción
  Controla si Microsoft Edge puede inmovilizar las pestañas que están en segundo plano durante al menos 5 minutos.

La inmovilización de pestañas reduce el uso de la CPU, la batería y la memoria. Microsoft Edge usa heurística para evitar inmovilizar las pestañas que realizan trabajo útil en segundo plano, como mostrar notificaciones, reproducir sonido y transmitir vídeo.

Si se habilita o no se configura esta directiva, es posible que las pestañas que han estado en segundo plano durante al menos 5 minutos estén inmovilizadas.

Si se deshabilita esta directiva, no se inmovilizará ninguna pestaña.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Booleano

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: TabFreezingEnabled
  - Nombre de la directiva de grupos: Permitir la inmovilización de pestañas en segundo plano
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: TabFreezingEnabled
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000000
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: TabFreezingEnabled
  - Valor de ejemplo:
``` xml
<false/>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### TaskManagerEndProcessEnabled
  #### Habilitar finalizar procesos en el Administrador de tareas del explorador
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Si se habilita o no se configura esta directiva, los usuarios pueden finalizar procesos en el Administrador de tareas del explorador. Si se deshabilita, los usuarios no pueden finalizar los procesos y el botón de Finalizar proceso estará deshabilitado en el Administrador de tareas del explorador.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Booleano

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: TaskManagerEndProcessEnabled
  - Nombre de la directiva de grupos: Habilitar finalizar procesos en el Administrador de tareas del explorador
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: TaskManagerEndProcessEnabled
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000001
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: TaskManagerEndProcessEnabled
  - Valor de ejemplo:
``` xml
<true/>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### TrackingPrevention
  #### Bloquear el seguimiento de la actividad de exploración web de los usuarios
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 78 o posterior

  #### Descripción
  Le permite decidir si quiere bloquear el seguimiento de la actividad de exploración web sitios web de los usuarios.

Si se habilita esta directiva, dispone de las siguientes opciones para configurar el nivel de prevención de seguimiento:

0 = Desactivado (sin prevención de seguimiento)
1 = Básico (bloquea los rastreadores dañinos, el contenido y los anuncios se personalizarán)
2 = Equilibrado (bloquea los rastreadores dañinos y los rastreadores de los sitios que el usuario no ha visitado; el contenido y los anuncios serán menos personalizados).
3 = Estricto (bloquea los rastreadores dañinos y la mayoría de los rastreadores de todos los sitios; el contenido y los anuncios tendrán una personalización mínima. Es posible que algunas partes de los sitios no funcionen)

Si se deshabilita esta directiva o no se configura, los usuarios pueden establecer su propio nivel de prevención de seguimiento.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Entero

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: TrackingPrevention
  - Nombre de la directiva de grupos: Bloquear el seguimiento de la actividad de exploración web de los usuarios
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: TrackingPrevention
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000002
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: TrackingPrevention
  - Valor de ejemplo:
``` xml
<integer>2</integer>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### TranslateEnabled
  #### Habilitar Traducir
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Habilita el servicio de traducción de Microsoft integrado en Microsoft Edge.

Si se habilita esta directiva, Microsoft Edge ofrece funcionalidad de traducción al usuario mostrando un control flotante de traducción integrado (cuando corresponda) y una opción de traducción en el menú contextual.

Deshabilite esta directiva para deshabilitar todas las características de traducción integradas.

Si no se establece la directiva, los usuarios podrán elegir si quieren usar la funcionalidad de traducción o no.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: Sí
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Booleano

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: TranslateEnabled
  - Nombre de la directiva de grupos: Habilitar Traducir
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): Plantillas administrativas/Microsoft Edge - Configuración predeterminada (los usuarios pueden cambiarla)/
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): SOFTWARE\Policies\Microsoft\Edge\Recomendada
  - Nombre del valor: TranslateEnabled
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000001
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: TranslateEnabled
  - Valor de ejemplo:
``` xml
<true/>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### URLAllowlist
  #### Definir una lista de direcciones URL permitidas
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Permita el acceso a las direcciones URL enumeradas, como excepciones a la lista de direcciones URL bloqueadas.

Formatee el patrón de dirección URL según [https://go.microsoft.com/fwlink/?linkid=2095322](https://go.microsoft.com/fwlink/?linkid=2095322).

Puede usar esta directiva para abrir excepciones a listas de bloqueadas restrictivas. Por ejemplo, puede incluir '*' en la lista de bloqueadas para bloquear todas las solicitudes y luego usar esta directiva para permitir el acceso a una lista limitada de direcciones URL. Puede usar esta directiva para abrir excepciones a ciertos esquemas, subdominios de otros dominios, puertos o rutas específicas.

El filtro más específico determina si una dirección URL está bloqueada o permitida. La lista de permitidas tiene prioridad sobre la lista de bloqueadas.

Esta directiva está limitada a 1000 entradas; las entradas posteriores se ignorarán.

Si no se configura esta directiva, no habrá excepciones a la lista de bloqueadas en la directiva [URLBlocklist](#urlblocklist).

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Lista de cadenas

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: URLAllowlist
  - Nombre de la directiva de grupos: Definir una lista de direcciones URL permitidas
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge\URLAllowlist
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: 1, 2, 3, ...
  - Tipo de valor: lista de REG_SZ
  ##### Valor de ejemplo:
```
SOFTWARE\Policies\Microsoft\Edge\URLAllowlist\0 = "contoso.com"
SOFTWARE\Policies\Microsoft\Edge\URLAllowlist\1 = "https://ssl.server.com"
SOFTWARE\Policies\Microsoft\Edge\URLAllowlist\2 = "hosting.com/good_path"
SOFTWARE\Policies\Microsoft\Edge\URLAllowlist\3 = "https://server:8080/path"
SOFTWARE\Policies\Microsoft\Edge\URLAllowlist\4 = ".exact.hostname.com"

```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: URLAllowlist
  - Valor de ejemplo:
``` xml
<array>
  <string>contoso.com</string>
  <string>https://ssl.server.com</string>
  <string>hosting.com/good_path</string>
  <string>https://server:8080/path</string>
  <string>.exact.hostname.com</string>
</array>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### URLBlocklist
  #### Bloquear el acceso a una lista de direcciones URL
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Defina una lista de sitios, según los patrones de URL, que están bloqueados (los usuarios no pueden cargarlos).

Formatee el patrón de dirección URL según [https://go.microsoft.com/fwlink/?linkid=2095322](https://go.microsoft.com/fwlink/?linkid=2095322).

Puede definir excepciones en la directiva [URLAllowlist](#urlallowlist). Estas directivas están limitadas a 1000 entradas; las entradas posteriores se omitirán.

Tenga en cuenta que no se recomienda bloquear las URL 'edge://*' internas, ya que esto podría provocar errores inesperados.

Esta directiva no impide que la página se actualice dinámicamente a través de JavaScript. Por ejemplo, si bloquea 'contoso.com/abc', los usuarios aún podrán visitar 'contoso.com' y hacer clic en un vínculo para visitar 'contoso.com/abc', siempre y cuando la página no se actualice.

Si no configura esta directiva, no se bloqueará ninguna URL.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Lista de cadenas

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: URLBlocklist
  - Nombre de la directiva de grupos: Bloquear el acceso a una lista de direcciones URL
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge\URLBlocklist
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: 1, 2, 3, ...
  - Tipo de valor: lista de REG_SZ
  ##### Valor de ejemplo:
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


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: URLBlocklist
  - Valor de ejemplo:
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
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### UserDataDir
  #### Establecer el directorio de datos de usuario
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Establecer el directorio que se va a usar para almacenar los datos del usuario.

Si se habilita esta directiva, Microsoft Edge usará el directorio especificado independientemente de si el usuario ha establecido la marca de línea de comandos '--user-data-dir'.

Si no se habilita esta directiva, se usará la ruta de acceso del perfil, pero el usuario podrá anularla usando la marca '--user-data-dir'. Los usuarios podrán encontrar el directorio para el perfil en edge://version/ en la ruta de acceso del perfil.

Para evitar la pérdida de datos u otros errores, no se debe configurar esta directiva en el directorio raíz de un volumen o en un directorio usado para otros fines, ya que Microsoft Edge administra su contenido.

Consulte [https://go.microsoft.com/fwlink/?linkid=2095041](https://go.microsoft.com/fwlink/?linkid=2095041) para ver una lista de variables que se pueden usar.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: No - Requiere reiniciar el explorador

  #### Tipo de datos:
  Cadena

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: UserDataDir
  - Nombre de la directiva de grupos: Establecer el directorio de datos de usuario
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: UserDataDir
  - Tipo de valor: REG_SZ
  ##### Valor de ejemplo:
```
"${users}/${user_name}/Edge"
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: UserDataDir
  - Valor de ejemplo:
``` xml
<string>${users}/${user_name}/Edge</string>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### UserFeedbackAllowed
  #### Permitir comentarios del usuario
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Microsoft Edge usa la característica Comentarios de Edge (habilitada de manera predeterminada) para permitir que los usuarios envíen comentarios, sugerencias o encuestas sobre los clientes y para informar de problemas con el explorador. Además, de manera predeterminada, los usuarios no pueden deshabilitar (desactivar) la característica Comentarios de Edge.

Si se habilita esta directiva o no se configura, los usuarios podrán invocar Comentarios de Edge.

Si se deshabilita esta directiva, los usuarios no podrán invocar Comentarios de Edge.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: No - Requiere reiniciar el explorador

  #### Tipo de datos:
  Booleano

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: UserFeedbackAllowed
  - Nombre de la directiva de grupos: Permitir comentarios del usuario
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: UserFeedbackAllowed
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000001
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: UserFeedbackAllowed
  - Valor de ejemplo:
``` xml
<true/>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### VideoCaptureAllowed
  #### Permitir o bloquear la captura de vídeo
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Controle si los sitios pueden capturar vídeo.

Si se habilita o no se configura (valor predeterminado), se preguntará al usuario acerca del acceso de la captura de vídeo para todos los sitios excepto para los que tengan URL configuradas en la lista de directivas [VideoCaptureAllowedUrls](#videocaptureallowedurls), a los que se les concederá acceso sin preguntar.

Si deshabilita esta directiva, no se preguntará al usuario y la captura de vídeo solo estará disponible para las URL configuradas en la directiva [VideoCaptureAllowedUrls](#videocaptureallowedurls).

Esta directiva afecta a todos los tipos de entradas de vídeo, no solo a la cámara integrada.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Booleano

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: VideoCaptureAllowed
  - Nombre de la directiva de grupos: Permitir o bloquear la captura de vídeo
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: VideoCaptureAllowed
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000000
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: VideoCaptureAllowed
  - Valor de ejemplo:
``` xml
<false/>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### VideoCaptureAllowedUrls
  #### Sitios que pueden acceder a dispositivos de captura de vídeo sin solicitar permiso
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Especifica los sitios web, según los patrones de dirección URL, que pueden usar dispositivos de captura de vídeo sin pedirle permiso al usuario. Los patrones de esta lista se comparan con el origen de la seguridad de la dirección URL de la solicitud. Si coinciden, el sitio tendrá acceso automáticamente a los dispositivos de captura de vídeo.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: Sí

  #### Tipo de datos:
  Lista de cadenas

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: VideoCaptureAllowedUrls
  - Nombre de la directiva de grupos: Sitios que pueden acceder a dispositivos de captura de vídeo sin solicitar permiso
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge\VideoCaptureAllowedUrls
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: 1, 2, 3, ...
  - Tipo de valor: lista de REG_SZ
  ##### Valor de ejemplo:
```
SOFTWARE\Policies\Microsoft\Edge\VideoCaptureAllowedUrls\0 = "https://www.contoso.com/"
SOFTWARE\Policies\Microsoft\Edge\VideoCaptureAllowedUrls\1 = "https://[*.]contoso.edu/"

```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: VideoCaptureAllowedUrls
  - Valor de ejemplo:
``` xml
<array>
  <string>https://www.contoso.com/</string>
  <string>https://[*.]contoso.edu/</string>
</array>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### WPADQuickCheckEnabled
  #### Establecer la optimización de WPAD
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Le permite desconectar la optimización de WPAD (detección automática de proxy web) en Microsoft Edge.

Si se deshabilita esta directiva, la optimización de WPAD se deshabilitará, lo que hará que el explorador tenga que esperar más tiempo a los servidores de WPAD basados en DNS.

Si se habilita o no se configura la directiva, la optimización de WPAD se habilitará.

Independientemente de cómo se habilite esta directiva y de si está o no habilitada, los usuarios no podrán cambiar la configuración de optimización de WPAD.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: No - Requiere reiniciar el explorador

  #### Tipo de datos:
  Booleano

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: WPADQuickCheckEnabled
  - Nombre de la directiva de grupos: Establecer la optimización de WPAD
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: WPADQuickCheckEnabled
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000001
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: WPADQuickCheckEnabled
  - Valor de ejemplo:
``` xml
<true/>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### WebDriverOverridesIncompatiblePolicies
  #### Permitir que WebDriver invalide las directivas incompatibles
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Esta directiva se quitó en M80 porque ya no es necesaria debido a que
WebDriver ahora es compatible con todas las directivas existentes.

Esta directiva permite a los usuarios de la característica WebDriver invalidar
directivas que pueden interferir con su funcionamiento.

Actualmente, esta directiva deshabilita las directivas [SitePerProcess](#siteperprocess) y [IsolateOrigins](#isolateorigins).

Si la directiva está habilitada, WebDriver podrá invalidar directivas
incompatibles.
Si la directiva está deshabilitada o no está configurada, WebDriver no podrá
invalidar las directivas incompatibles.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: No - Requiere reiniciar el explorador

  #### Tipo de datos:
  Booleano

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: WebDriverOverridesIncompatiblePolicies
  - Nombre de la directiva de grupos: Permitir que WebDriver invalide las directivas incompatibles
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: WebDriverOverridesIncompatiblePolicies
  - Tipo de valor: REG_DWORD
  ##### Valor de ejemplo:
```
0x00000001
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: WebDriverOverridesIncompatiblePolicies
  - Valor de ejemplo:
``` xml
<true/>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### WebRtcLocalhostIpHandling
  #### Restringir la exposición de la dirección IP de localhost por WebRTC
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Permite establecer si WebRTC expone la dirección IP del localhost.

Si se establece esta directiva en "AllowAllInterfaces" ('predeterminado') o "AllowPublicAndPrivateInterfaces" ('default_public_and_private_interfaces'), WebRTC expone la dirección IP del localhost.

Si se establece esta directiva en "AllowPublicInterfaceOnly" ('default_public_interface_only') o "DisableNonProxiedUdp" ('disable_non_proxied_udp'), WebRTC no expone la dirección IP del localhost.

Si no se establece esta directiva o si se deshabilita, WebRTC expone la dirección IP del localhost.

  * 'default' = Permitir todas las interfaces. Esto expone la dirección IP del localhost.
  * 'default_public_and_private_interfaces' = Permitir las interfaces públicas y privadas a través de la ruta predeterminada http. Esto expone la dirección IP del localhost.
  * 'default_public_interface_only' = Permitir la interface pública a través de la ruta predeterminada http. Esto expone la dirección IP del localhost.
  * 'disable_non_proxied_udp’ = Usar TCP a menos que el servidor proxy admita UDP. Esto no expone la dirección IP del localhost.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: No - Requiere reiniciar el explorador

  #### Tipo de datos:
  Cadena

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: WebRtcLocalhostIpHandling
  - Nombre de la directiva de grupos: Restringir la exposición de la dirección IP de localhost por WebRTC
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: WebRtcLocalhostIpHandling
  - Tipo de valor: REG_SZ
  ##### Valor de ejemplo:
```
"default"
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: WebRtcLocalhostIpHandling
  - Valor de ejemplo:
``` xml
<string>default</string>
```
  

  [Volver al principio](#microsoft-edge:-directivas)

  ### WebRtcUdpPortRange
  #### Restringir el intervalo de puertos UDP locales usados por WebRTC
  >Versiones admitidas: Microsoft Edge en Windows y Mac desde la versión 77 o posterior

  #### Descripción
  Restringe el intervalo de puertos UDP usado por WebRTC a un intervalo de puertos especificado (puntos de conexión incluidos).

Mediante la configuración de esta directiva, debes especificar el intervalo de puertos UDP locales que WebRTC puede usar.

Si no se configura esta directiva o si se establece en una cadena vacía o en un intervalo de puertos no válido, WebRTC puede usar cualquier puerto UDP local disponible.

  #### Características admitidas:
  - Puede ser obligatorio: Sí
  - Se puede recomendar: No
  - Actualización de directiva dinámica: No - Requiere reiniciar el explorador

  #### Tipo de datos:
  Cadena

  #### Información y configuración de Windows
  ##### Información de la directiva de grupos (ADMX)
  - Nombre único de la directiva de grupos: WebRtcUdpPortRange
  - Nombre de la directiva de grupos: Restringir el intervalo de puertos UDP locales usados por WebRTC
  - Ruta de acceso de GP (Obligatorio): Plantillas administrativas/Microsoft Edge/
  - Ruta de acceso de GP (Recomendada): N/D
  - Nombre del archivo ADMX de GP: MSEdge.admx
  ##### Configuración del registro de Windows
  - Ruta de acceso (Obligatorio): SOFTWARE\Policies\Microsoft\Edge
  - Ruta de acceso (Recomendada): N/D
  - Nombre del valor: WebRtcUdpPortRange
  - Tipo de valor: REG_SZ
  ##### Valor de ejemplo:
```
"10000-11999"
```


  #### Información y configuración de Mac
  - Nombre de clave de preferencia: WebRtcUdpPortRange
  - Valor de ejemplo:
``` xml
<string>10000-11999</string>
```
  

  [Volver al principio](#microsoft-edge:-directivas)


## Vea también
- [Configurando Microsoft Edge](configure-microsoft-edge.md)
- [Página de aterrizaje de Microsoft Edge Enterprise](https://aka.ms/EdgeEnterprise)