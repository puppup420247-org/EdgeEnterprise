---
title: "Microsoft Edge Browser Policy Documentation"
ms.author: stmoody
author: brianalt-msft
manager: tahills
ms.date: 12/17/2019
audience: ITPro
ms.topic: reference
ms.prod: microsoft-edge
ms.localizationpriority: medium
ms.collection: M365-modern-desktop
ms.custom:
description: "Windows and Mac documentation for all policies supported by the Microsoft Edge Browser"
---

# Microsoft Edge - Políticas
A última versão do Microsoft Edge inclui as políticas a seguir. Você pode usar essas políticas para configurar o modo de execução do Microsoft Edge em sua organização.

Para obter informações sobre um conjunto adicional de políticas usadas para controlar como e quando o Microsoft Edge é atualizado, confira [Referência de política de atualização do Microsoft Edge](microsoft-edge-update-policies.md)

> [!OBSERVAÇÃO]
> Este artigo se aplica ao Microsoft Edge versão 77 ou posterior.

## Políticas disponíveis
Estas tabelas listam todas as políticas de grupo relacionadas ao navegador disponíveis nesta versão do Microsoft Edge. Use os links na tabela para obter mais detalhes sobre políticas específicas.

|||
|-|-|
|[Autenticação HTTP](#autenticação-http)|[Cast](#cast)|
|[Configurações de conteúdo](#configurações-de-conteúdo)|[Configurações do SmartScreen](#configurações-do-smartscreen)|
|[Extensões](#extensões)|[Gerenciador de senhas e de proteção](#gerenciador-de-senhas-e-de-proteção)|
|[Impressão](#impressão)|[Inicialização, página inicial e página nova guia](#inicialização,-página-inicial-e-página-nova-guia)|
|[Mensagens nativas](#mensagens-nativas)|[Provedor de pesquisa padrão](#provedor-de-pesquisa-padrão)|
|[Servidor proxy](#servidor-proxy)|[Additional](#additional)|


### [*Autenticação HTTP*](#autenticação-http-policies)
|Nome da Política|Legenda|
|-|-|
|[AllowCrossOriginAuthPrompt](#allowcrossoriginauthprompt)|Permitir solicitações de Autenticação Básica HTTP entre origens|
|[AuthNegotiateDelegateAllowlist](#authnegotiatedelegateallowlist)|Especifica uma lista de servidores aos quais o Microsoft Edge pode delegar credenciais de usuário|
|[AuthSchemes](#authschemes)|Esquemas de autenticação com suporte|
|[AuthServerAllowlist](#authserverallowlist)|Configurar lista de servidores de autenticação permitidos|
|[DisableAuthNegotiateCnameLookup](#disableauthnegotiatecnamelookup)|Desabilitar pesquisa CNAME ao negociar a autenticação Kerberos|
|[EnableAuthNegotiatePort](#enableauthnegotiateport)|Incluir porta não padrão no SPN do Kerberos|
|[NtlmV2Enabled](#ntlmv2enabled)|Controlar se a autenticação NTLMv2 está habilitada|
### [*Cast*](#cast-policies)
|Nome da Política|Legenda|
|-|-|
|[EnableMediaRouter](#enablemediarouter)|Habilitar Google Cast|
|[ShowCastIconInToolbar](#showcasticonintoolbar)|Mostrar o ícone de transmissão na barra de ferramentas|
### [*Configurações de conteúdo*](#configurações-de-conteúdo-policies)
|Nome da Política|Legenda|
|-|-|
|[AutoSelectCertificateForUrls](#autoselectcertificateforurls)|Selecionar automaticamente os certificados de cliente para estes sites|
|[CookiesAllowedForUrls](#cookiesallowedforurls)|Permitir cookies em sites específicos|
|[CookiesBlockedForUrls](#cookiesblockedforurls)|Bloquear cookies em sites específicos|
|[CookiesSessionOnlyForUrls](#cookiessessiononlyforurls)|Limitar cookies de sites específicos para a sessão atual|
|[DefaultCookiesSetting](#defaultcookiessetting)|Configurar cookies|
|[DefaultGeolocationSetting](#defaultgeolocationsetting)|Configuração de geolocalização padrão|
|[DefaultImagesSetting](#defaultimagessetting)|Configuração de imagens padrão|
|[DefaultInsecureContentSetting](#defaultinsecurecontentsetting)|Controlar uso de exceções de conteúdo não seguro|
|[DefaultJavaScriptSetting](#defaultjavascriptsetting)|Configuração de JavaScript padrão|
|[DefaultNotificationsSetting](#defaultnotificationssetting)|Configuração de notificação padrão|
|[DefaultPluginsSetting](#defaultpluginssetting)|Configuração padrão do Adobe Flash|
|[DefaultPopupsSetting](#defaultpopupssetting)|Configuração de janela pop-up padrão|
|[DefaultWebBluetoothGuardSetting](#defaultwebbluetoothguardsetting)|Controlar o uso da API Web Bluetooth|
|[DefaultWebUsbGuardSetting](#defaultwebusbguardsetting)|Controlar o uso da API WebUSB|
|[ImagesAllowedForUrls](#imagesallowedforurls)|Permitir imagens nestes sites|
|[ImagesBlockedForUrls](#imagesblockedforurls)|Bloquear imagens em sites específicos|
|[InsecureContentAllowedForUrls](#insecurecontentallowedforurls)|Permitir conteúdo não seguro em sites especificados|
|[InsecureContentBlockedForUrls](#insecurecontentblockedforurls)|Bloquear conteúdo não seguro em sites especificados|
|[JavaScriptAllowedForUrls](#javascriptallowedforurls)|Permitir JavaScript em sites específicos|
|[JavaScriptBlockedForUrls](#javascriptblockedforurls)|Bloquear o JavaScript em sites específicos|
|[LegacySameSiteCookieBehaviorEnabled](#legacysamesitecookiebehaviorenabled)|Habilitar a configuração do comportamento de cookies SameSite herdado padrão|
|[LegacySameSiteCookieBehaviorEnabledForDomainList](#legacysamesitecookiebehaviorenabledfordomainlist)|Reverter para o comportamento SameSite herdado de cookies em sites especificados|
|[NotificationsAllowedForUrls](#notificationsallowedforurls)|Permitir notificações em sites específicos|
|[NotificationsBlockedForUrls](#notificationsblockedforurls)|Bloquear notificações em sites específicos|
|[PluginsAllowedForUrls](#pluginsallowedforurls)|Permitir o plug-in do Adobe Flash em sites específicos|
|[PluginsBlockedForUrls](#pluginsblockedforurls)|Bloquear o plug-in do Adobe Flash em sites específicos|
|[PopupsAllowedForUrls](#popupsallowedforurls)|Permitir janelas pop-up em sites específicos|
|[PopupsBlockedForUrls](#popupsblockedforurls)|Bloquear janelas pop-up em sites específicos|
|[RegisteredProtocolHandlers](#registeredprotocolhandlers)|Registrar manipuladores de protocolo|
|[WebUsbAllowDevicesForUrls](#webusballowdevicesforurls)|Conceder acesso a sites específicos para se conectar a dispositivos USB específicos|
|[WebUsbAskForUrls](#webusbaskforurls)|Permitir WebUSB em sites específicos|
|[WebUsbBlockedForUrls](#webusbblockedforurls)|Bloquear WebUSB em sites específicos|
### [*Configurações do SmartScreen*](#configurações-do-smartscreen-policies)
|Nome da Política|Legenda|
|-|-|
|[PreventSmartScreenPromptOverride](#preventsmartscreenpromptoverride)|Impedir que avisos do Microsoft Defender SmartScreen sejam ignorados para sites|
|[PreventSmartScreenPromptOverrideForFiles](#preventsmartscreenpromptoverrideforfiles)|Impedir que os avisos do Microsoft Defender SmartScreen sobre downloads sejam ignorados|
|[SmartScreenAllowListDomains](#smartscreenallowlistdomains)|Configurar a lista de domínios para os quais o Microsoft Defender SmartScreen não disparará avisos|
|[SmartScreenEnabled](#smartscreenenabled)|Configurar o Microsoft Defender SmartScreen|
|[SmartScreenForTrustedDownloadsEnabled](#smartscreenfortrusteddownloadsenabled)|Forçar verificações do Microsoft Defender SmartScreen em downloads de fontes confiáveis|
|[SmartScreenPuaEnabled](#smartscreenpuaenabled)|Configurar o Microsoft Defender SmartScreen para bloquear aplicativos potencialmente indesejados|
### [*Extensões*](#extensões-policies)
|Nome da Política|Legenda|
|-|-|
|[ExtensionAllowedTypes](#extensionallowedtypes)|Configurar tipos de extensão permitidos|
|[ExtensionInstallAllowlist](#extensioninstallallowlist)|Permitir que extensões específicas sejam instaladas|
|[ExtensionInstallBlocklist](#extensioninstallblocklist)|Controlar quais extensões não podem ser instaladas|
|[ExtensionInstallForcelist](#extensioninstallforcelist)|Controlar quais extensões são instaladas silenciosamente|
|[ExtensionInstallSources](#extensioninstallsources)|Configurar fontes de instalação de script de usuário e extensão|
|[ExtensionSettings](#extensionsettings)|Definir configurações de gerenciamento de extensões|
### [*Gerenciador de senhas e de proteção*](#gerenciador-de-senhas-e-de-proteção-policies)
|Nome da Política|Legenda|
|-|-|
|[PasswordManagerEnabled](#passwordmanagerenabled)|Habilitar salvamento de senhas no gerenciador de senhas|
|[PasswordProtectionChangePasswordURL](#passwordprotectionchangepasswordurl)|Configurar a URL de alteração de senha|
|[PasswordProtectionLoginURLs](#passwordprotectionloginurls)|Configurar a lista de URLs de logon corporativo em que o serviço de proteção de senha deve capturar a impressão digital de senha|
|[PasswordProtectionWarningTrigger](#passwordprotectionwarningtrigger)|Configurar gatilho de aviso de proteção de senha|
### [*Impressão*](#impressão-policies)
|Nome da Política|Legenda|
|-|-|
|[DefaultPrinterSelection](#defaultprinterselection)|Regras de seleção de impressora padrão|
|[PrintHeaderFooter](#printheaderfooter)|Imprimir cabeçalhos e rodapés|
|[PrintPreviewUseSystemDefaultPrinter](#printpreviewusesystemdefaultprinter)|Definir a impressora padrão do sistema como a impressora padrão|
|[PrintingEnabled](#printingenabled)|Habilitar impressão|
|[UseSystemPrintDialog](#usesystemprintdialog)|Imprimir usando a caixa de diálogo de impressão do sistema|
### [*Inicialização&comma; página inicial e página nova guia*](#inicialização-página-inicial-e-página-nova-guia-policies)
|Nome da Política|Legenda|
|-|-|
|[HomepageIsNewTabPage](#homepageisnewtabpage)|Definir a página nova guia como a home page|
|[HomepageLocation](#homepagelocation)|Configurar a URL da home page|
|[NewTabPageCompanyLogo](#newtabpagecompanylogo)|Definir o logotipo da empresa da página Nova guia|
|[NewTabPageHideDefaultTopSites](#newtabpagehidedefaulttopsites)|Ocultar os sites principais padrão da página de nova guia|
|[NewTabPageLocation](#newtabpagelocation)|Configurar a URL da página de nova guia|
|[NewTabPageManagedQuickLinks](#newtabpagemanagedquicklinks)|Definir links rápidos da página de nova guia|
|[NewTabPageSetFeedType](#newtabpagesetfeedtype)|Configurar a experiência de página de nova guia do Microsoft Edge|
|[RestoreOnStartup](#restoreonstartup)|Ação a ser executada na inicialização|
|[RestoreOnStartupURLs](#restoreonstartupurls)|Sites a serem abertos quando o navegador for iniciado|
|[ShowHomeButton](#showhomebutton)|Mostrar botão Início na barra de ferramentas|
### [*Mensagens nativas*](#mensagens-nativas-policies)
|Nome da Política|Legenda|
|-|-|
|[NativeMessagingAllowlist](#nativemessagingallowlist)|Controlar quais hosts de mensagens nativas os usuários podem usar|
|[NativeMessagingBlocklist](#nativemessagingblocklist)|Configurar lista de contatos bloqueados de mensagens nativas|
|[NativeMessagingUserLevelHosts](#nativemessaginguserlevelhosts)|Permitir hosts de mensagens nativas no nível de usuário (instalado sem permissões de administrador)|
### [*Provedor de pesquisa padrão*](#provedor-de-pesquisa-padrão-policies)
|Nome da Política|Legenda|
|-|-|
|[DefaultSearchProviderEnabled](#defaultsearchproviderenabled)|Habilitar o provedor de pesquisa padrão|
|[DefaultSearchProviderEncodings](#defaultsearchproviderencodings)|Codificações do provedor de pesquisa padrão|
|[DefaultSearchProviderImageURL](#defaultsearchproviderimageurl)|Especifica o recurso de pesquisa por imagem para o provedor de pesquisa padrão|
|[DefaultSearchProviderImageURLPostParams](#defaultsearchproviderimageurlpostparams)|Parâmetros para uma URL de imagem que usa POST|
|[DefaultSearchProviderKeyword](#defaultsearchproviderkeyword)|Palavra-chave do provedor de pesquisa padrão|
|[DefaultSearchProviderName](#defaultsearchprovidername)|Nome do provedor de pesquisa padrão|
|[DefaultSearchProviderSearchURL](#defaultsearchprovidersearchurl)|URL de pesquisa do provedor de pesquisa padrão|
|[DefaultSearchProviderSuggestURL](#defaultsearchprovidersuggesturl)|URL do provedor de pesquisa padrão para sugestões|
### [*Servidor proxy*](#servidor-proxy-policies)
|Nome da Política|Legenda|
|-|-|
|[ProxyBypassList](#proxybypasslist)|Configurar regras para ignorar o proxy|
|[ProxyMode](#proxymode)|Definir configurações de servidor proxy|
|[ProxyPacUrl](#proxypacurl)|Definir a URL do arquivo .pac do proxy|
|[ProxyServer](#proxyserver)|Configurar o endereço ou a URL do servidor proxy|
|[ProxySettings](#proxysettings)|Configurações de proxy|
### [*Additional*](#additional-policies)
|Nome da Política|Legenda|
|-|-|
|[AdsSettingForIntrusiveAdsSites](#adssettingforintrusiveadssites)|Configuração de anúncios para sites com anúncios intrusivos|
|[AllowDeletingBrowserHistory](#allowdeletingbrowserhistory)|Habilitar a exclusão do navegador e do histórico de download|
|[AllowFileSelectionDialogs](#allowfileselectiondialogs)|Permitir caixas de diálogo de seleção de arquivos|
|[AllowPopupsDuringPageUnload](#allowpopupsduringpageunload)|Permite que uma página mostre pop-ups durante seu descarregamento|
|[AllowSyncXHRInPageDismissal](#allowsyncxhrinpagedismissal)|Permitir que as páginas enviem solicitações XHR síncronas durante o descarte de páginas|
|[AllowTrackingForUrls](#allowtrackingforurls)|Configurar exceções de prevenção de rastreamento para sites específicos|
|[AlternateErrorPagesEnabled](#alternateerrorpagesenabled)|Sugerir páginas similares quando uma página da Web não puder ser encontrada|
|[AlwaysOpenPdfExternally](#alwaysopenpdfexternally)|Sempre abrir arquivos PDF externamente|
|[ApplicationLocaleValue](#applicationlocalevalue)|Definir localidade do aplicativo|
|[AudioCaptureAllowed](#audiocaptureallowed)|Permitir ou bloquear captura de áudio|
|[AudioCaptureAllowedUrls](#audiocaptureallowedurls)|Sites podem acessar dispositivos de captura áudio sem solicitar permissão|
|[AutoImportAtFirstRun](#autoimportatfirstrun)|Importar automaticamente os dados e as configurações de outro navegador na primeira execução|
|[AutofillAddressEnabled](#autofilladdressenabled)|Habilitar AutoPreenchimento para endereços|
|[AutofillCreditCardEnabled](#autofillcreditcardenabled)|Habilitar AutoPreenchimento para cartões de crédito|
|[AutoplayAllowed](#autoplayallowed)|Permitir reprodução automática de mídia para sites|
|[BackgroundModeEnabled](#backgroundmodeenabled)|Continuar executando apps em segundo plano depois que o Microsoft Edge for fechado|
|[BackgroundTemplateListUpdatesEnabled](#backgroundtemplatelistupdatesenabled)|Permite atualizações em segundo plano na lista de modelos disponíveis para Coleções e outros recursos que usam modelos|
|[BlockThirdPartyCookies](#blockthirdpartycookies)|Bloquear cookies de terceiros|
|[BrowserAddProfileEnabled](#browseraddprofileenabled)|Habilitar a criação de perfil no menu do submenu Identidade ou na página Configurações|
|[BrowserGuestModeEnabled](#browserguestmodeenabled)|Habilitar modo convidado|
|[BrowserNetworkTimeQueriesEnabled](#browsernetworktimequeriesenabled)|Permitir consultas a um serviço de Hora da Rede do Navegador|
|[BrowserSignin](#browsersignin)|Configurações de entrada do navegador|
|[BuiltInDnsClientEnabled](#builtindnsclientenabled)|Usar o cliente DNS interno|
|[CertificateTransparencyEnforcementDisabledForCas](#certificatetransparencyenforcementdisabledforcas)|Desabilitar a imposição de Transparência de Certificado para uma lista de hashes de subjectPublicKeyInfo|
|[CertificateTransparencyEnforcementDisabledForLegacyCas](#certificatetransparencyenforcementdisabledforlegacycas)|Desabilitar a imposição de Transparência de Certificado para uma lista de autoridades de certificação herdadas|
|[CertificateTransparencyEnforcementDisabledForUrls](#certificatetransparencyenforcementdisabledforurls)|Desabilitar a imposição de Transparência de Certificado para URLs específicas|
|[ClearBrowsingDataOnExit](#clearbrowsingdataonexit)|Limpar dados de navegação quando o Microsoft Edge for fechado|
|[ClickOnceEnabled](#clickonceenabled)|Permitir que os usuários abram arquivos usando o protocolo ClickOnce|
|[CommandLineFlagSecurityWarningsEnabled](#commandlineflagsecuritywarningsenabled)|Habilitar avisos de segurança para sinalizadores de linha de comando|
|[ComponentUpdatesEnabled](#componentupdatesenabled)|Habilitar atualizações de componentes no Microsoft Edge|
|[ConfigureDoNotTrack](#configuredonottrack)|Configurar Não Rastrear|
|[ConfigureOnlineTextToSpeech](#configureonlinetexttospeech)|Configurar a conversão de texto em fala online|
|[CustomHelpLink](#customhelplink)|Especificar link de ajuda personalizado|
|[DefaultBrowserSettingEnabled](#defaultbrowsersettingenabled)|Definir Microsoft Edge como navegador padrão|
|[DeveloperToolsAvailability](#developertoolsavailability)|Controlar onde as ferramentas de desenvolvedor podem ser usadas|
|[DirectInvokeEnabled](#directinvokeenabled)|Permitir que os usuários abram arquivos usando o protocolo DirectInvoke|
|[Disable3DAPIs](#disable3dapis)|Desabilitar o suporte para APIs de gráficos 3D|
|[DisableScreenshots](#disablescreenshots)|Desabilitar as capturas de tela|
|[DiskCacheDir](#diskcachedir)|Definir diretório de cache de disco|
|[DiskCacheSize](#diskcachesize)|Definir o tamanho do cache de disco, em bytes|
|[DownloadDirectory](#downloaddirectory)|Definir diretório de download|
|[DownloadRestrictions](#downloadrestrictions)|Permitir restrições de download|
|[EdgeCollectionsEnabled](#edgecollectionsenabled)|Habilitar o recurso Coleções|
|[EditFavoritesEnabled](#editfavoritesenabled)|Permite que os usuários editem os favoritos|
|[EnableDeprecatedWebPlatformFeatures](#enabledeprecatedwebplatformfeatures)|Reabilitar os recursos preteridos da plataforma da Web por um tempo limitado|
|[EnableDomainActionsDownload](#enabledomainactionsdownload)|Habilitar o download de ações de domínio da Microsoft|
|[EnableOnlineRevocationChecks](#enableonlinerevocationchecks)|Habilitar verificações de OCSP/CRL online|
|[EnterpriseHardwarePlatformAPIEnabled](#enterprisehardwareplatformapienabled)|Permitir que extensões gerenciadas usem a API da Plataforma de Hardware Corporativo|
|[ExperimentationAndConfigurationServiceControl](#experimentationandconfigurationservicecontrol)|Controlar a comunicação com o Serviço de Configuração e Experimentação|
|[ExternalProtocolDialogShowAlwaysOpenCheckbox](#externalprotocoldialogshowalwaysopencheckbox)|Mostrar uma caixa de seleção "Sempre abrir" na caixa de diálogo de protocolo externo|
|[FavoritesBarEnabled](#favoritesbarenabled)|Habilitar barra de favoritos|
|[ForceBingSafeSearch](#forcebingsafesearch)|Aplicar a Pesquisa Segura do Bing|
|[ForceEphemeralProfiles](#forceephemeralprofiles)|Habilitar o uso de perfis efêmeros|
|[ForceGoogleSafeSearch](#forcegooglesafesearch)|Forçar a Pesquisa Segura do Google|
|[ForceNetworkInProcess](#forcenetworkinprocess)|Aplicar o código de rede a ser executado no processo do navegador|
|[ForceYouTubeRestrict](#forceyoutuberestrict)|Aplicar o modo restrito mínimo do YouTube|
|[FullscreenAllowed](#fullscreenallowed)|Permitir modo de tela inteira|
|[GoToIntranetSiteForSingleWordEntryInAddressBar](#gotointranetsiteforsinglewordentryinaddressbar)|Forçar a navegação direta em site da intranet, em vez de pesquisar em entradas de palavras únicas na Barra de Endereços|
|[HSTSPolicyBypassList](#hstspolicybypasslist)|Configurar a lista de nomes que ignorarão a verificação de política HSTS|
|[HardwareAccelerationModeEnabled](#hardwareaccelerationmodeenabled)|Usar aceleração de hardware quando disponível|
|[ImportAutofillFormData](#importautofillformdata)|Permitir importação de dados de formulário de autopreenchimento|
|[ImportBrowserSettings](#importbrowsersettings)|Permitir a importação das configurações do navegador|
|[ImportFavorites](#importfavorites)|Permitir importação de favoritos|
|[ImportHistory](#importhistory)|Permitir a importação do histórico de navegação|
|[ImportHomepage](#importhomepage)|Permitir a importação das configurações da home page|
|[ImportOpenTabs](#importopentabs)|Permitir importação de guias abertas|
|[ImportPaymentInfo](#importpaymentinfo)|Permitir importação de informações de pagamento|
|[ImportSavedPasswords](#importsavedpasswords)|Permitir a importação de senhas salvas|
|[ImportSearchEngine](#importsearchengine)|Permitir importação das configurações do mecanismo de pesquisa|
|[InPrivateModeAvailability](#inprivatemodeavailability)|Configurar a disponibilidade do modo InPrivate|
|[InternetExplorerIntegrationLevel](#internetexplorerintegrationlevel)|Configurar a integração com o Internet Explorer|
|[InternetExplorerIntegrationSiteList](#internetexplorerintegrationsitelist)|Configurar a Lista de Sites do Modo Empresarial|
|[IsolateOrigins](#isolateorigins)|Habilitar isolamento de site para origens específicas|
|[ManagedFavorites](#managedfavorites)|Configurar favoritos|
|[ManagedSearchEngines](#managedsearchengines)|Gerenciar Mecanismos de Pesquisa|
|[MaxConnectionsPerProxy](#maxconnectionsperproxy)|Número máximo de conexões simultâneas com o servidor proxy|
|[MediaRouterCastAllowAllIPs](#mediaroutercastallowallips)|Permitir que o Google Cast se conecte a dispositivos Cast em todos os endereços IP|
|[MetricsReportingEnabled](#metricsreportingenabled)|Habilitar relatórios de dados relacionados a uso e falhas|
|[NetworkPredictionOptions](#networkpredictionoptions)|Habilitar previsão de rede|
|[NonRemovableProfileEnabled](#nonremovableprofileenabled)|Configurar se um usuário sempre tem um perfil padrão conectado automaticamente à sua conta corporativa ou de estudante|
|[OverrideSecurityRestrictionsOnInsecureOrigin](#overridesecurityrestrictionsoninsecureorigin)|Controlar onde se aplicam a restrições de segurança em origens não seguras|
|[PersonalizationReportingEnabled](#personalizationreportingenabled)|Allow personalization of ads, search and news by sending browsing history to Microsoft|
|[PinningWizardAllowed](#pinningwizardallowed)|Permitir o Assistente para fixar na barra de tarefas|
|[ProactiveAuthEnabled](#proactiveauthenabled)|Habilitar a Autenticação Proativa|
|[PromotionalTabsEnabled](#promotionaltabsenabled)|Habilitar conteúdo promocional em toda a guia|
|[PromptForDownloadLocation](#promptfordownloadlocation)|Perguntar onde salvar os arquivos baixados|
|[QuicAllowed](#quicallowed)|Permitir o protocolo QUIC|
|[RelaunchNotification](#relaunchnotification)|Notificar um usuário de que uma reinicialização do navegador é recomendada ou necessária para atualizações pendentes|
|[RelaunchNotificationPeriod](#relaunchnotificationperiod)|Definir o período para notificações de atualização|
|[RendererCodeIntegrityEnabled](#renderercodeintegrityenabled)|Habilitar integridade do código do renderizador|
|[RequireOnlineRevocationChecksForLocalAnchors](#requireonlinerevocationchecksforlocalanchors)|Especificar se as verificações OCSP/CRL online são necessárias para âncoras de confiança locais|
|[ResolveNavigationErrorsUseWebService](#resolvenavigationerrorsusewebservice)|Habilitar a resolução de erros de navegação usando um serviço Web|
|[RestrictSigninToPattern](#restrictsignintopattern)|Restringir quais contas podem ser usadas como contas principais do Microsoft Edge|
|[RunAllFlashInAllowMode](#runallflashinallowmode)|Estender a configuração do conteúdo em Adobe Flash a todo o conteúdo|
|[SSLErrorOverrideAllowed](#sslerroroverrideallowed)|Permitir que os usuários continuem a partir da página de aviso HTTPS|
|[SSLVersionMin](#sslversionmin)|Versão mínima do TLS habilitada|
|[SavingBrowserHistoryDisabled](#savingbrowserhistorydisabled)|Desabilitar o salvamento do histórico do navegador|
|[SearchSuggestEnabled](#searchsuggestenabled)|Habilitar sugestões de pesquisa|
|[SecurityKeyPermitAttestation](#securitykeypermitattestation)|Sites ou domínios que não precisam de permissão para usar o atestado de Chave de Segurança direto|
|[SendIntranetToInternetExplorer](#sendintranettointernetexplorer)|Enviar todos os sites da intranet para o Internet Explorer|
|[SendSiteInfoToImproveServices](#sendsiteinfotoimproveservices)|Enviar informações do site para melhorar os serviços Microsoft|
|[ShowOfficeShortcutInFavoritesBar](#showofficeshortcutinfavoritesbar)|Mostrar o atalho do Microsoft Office na barra Favoritos|
|[SignedHTTPExchangeEnabled](#signedhttpexchangeenabled)|Habilitar o suporte para o Signed HTTP Exchange (SXG)|
|[SitePerProcess](#siteperprocess)|Habilitar isolamento de sites para todos os sites|
|[SpellcheckEnabled](#spellcheckenabled)|Habilitar verificação ortográfica|
|[SpellcheckLanguage](#spellchecklanguage)|Habilitar idiomas específicos da verificação ortográfica|
|[SpellcheckLanguageBlocklist](#spellchecklanguageblocklist)|Aplicar a desabilitação de verificação ortográfica dos idiomas|
|[SuppressUnsupportedOSWarning](#suppressunsupportedoswarning)|Suprimir o aviso do sistema operacional sem suporte|
|[SyncDisabled](#syncdisabled)|Desabilitar sincronização de dados usando os serviços de sincronização da Microsoft|
|[TabFreezingEnabled](#tabfreezingenabled)|Permitir congelamento de guias em segundo plano|
|[TaskManagerEndProcessEnabled](#taskmanagerendprocessenabled)|Habilitar processos finais no gerenciador de tarefas do navegador|
|[TrackingPrevention](#trackingprevention)|Bloquear o rastreamento de atividades de navegação da Web dos usuários|
|[TranslateEnabled](#translateenabled)|Habilitar Traduzir|
|[URLAllowlist](#urlallowlist)|Definir uma lista de URLs permitidas|
|[URLBlocklist](#urlblocklist)|Bloquear o acesso a uma lista de URLs|
|[UserDataDir](#userdatadir)|Definir o diretório de dados do usuário|
|[UserFeedbackAllowed](#userfeedbackallowed)|Permitir comentários do usuário|
|[VideoCaptureAllowed](#videocaptureallowed)|Permitir ou bloquear captura de vídeo|
|[VideoCaptureAllowedUrls](#videocaptureallowedurls)|Sites que podem acessar dispositivos de captura de vídeo sem solicitar permissão|
|[WPADQuickCheckEnabled](#wpadquickcheckenabled)|Definir otimização de WPAD|
|[WebAppInstallForceList](#webappinstallforcelist)|Configurar lista de Aplicativos Web instalados à força|
|[WebDriverOverridesIncompatiblePolicies](#webdriveroverridesincompatiblepolicies)|Permitir que o WebDriver substitua políticas incompatíveis|
|[WebRtcLocalIpsAllowedUrls](#webrtclocalipsallowedurls)|Gerenciar a exposição de endereços IP locais pelo WebRTC|
|[WebRtcLocalhostIpHandling](#webrtclocalhostiphandling)|Restringir a exposição do endereço IP local pelo WebRTC|
|[WebRtcUdpPortRange](#webrtcudpportrange)|Restringir o intervalo de portas UDP locais usadas pelo WebRTC|




  ## Autenticação HTTP policies

  [Voltar ao início](#microsoft-edge---políticas)

  ### AllowCrossOriginAuthPrompt
  #### Permitir solicitações de Autenticação Básica HTTP entre origens
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Controla se o subconteúdo de terceiros em uma página pode abrir uma caixa de diálogo de Autenticação Básica HTTP.

Normalmente, isso é desabilitado como uma defesa contra phishing. Se você não configurar esta política, ela será desabilitada e o subconteúdo de terceiros não poderá abrir uma caixa de diálogo de Autenticação Básica HTTP.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: AllowCrossOriginAuthPrompt
  - Nome da GP: Permitir solicitações de Autenticação Básica HTTP entre origens
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/Autenticação HTTP
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: AllowCrossOriginAuthPrompt
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000000
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: AllowCrossOriginAuthPrompt
  - Exemplo de valor:
``` xml
<false/>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### AuthNegotiateDelegateAllowlist
  #### Especifica uma lista de servidores aos quais o Microsoft Edge pode delegar credenciais de usuário
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Configura a lista de servidores que o Microsoft Edge pode delegar.

Separe vários nomes de servidor com vírgulas. Caracteres curinga (*) são permitidos.

Se você não configurar essa política, o Microsoft Edge não delegará credenciais de usuário, mesmo que um servidor seja detectado como Intranet.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Não - Requer a reinicialização do navegador

  #### Tipo de Dados:
  Cadeia de Caracteres

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: AuthNegotiateDelegateAllowlist
  - Nome da GP: Especifica uma lista de servidores aos quais o Microsoft Edge pode delegar credenciais de usuário
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/Autenticação HTTP
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: AuthNegotiateDelegateAllowlist
  - Tipo de Valor: REG_SZ
  ##### Exemplo de valor:
```
"contoso.com"
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: AuthNegotiateDelegateAllowlist
  - Exemplo de valor:
``` xml
<string>contoso.com</string>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### AuthSchemes
  #### Esquemas de autenticação com suporte
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Especifica os esquemas de autenticação HTTP que têm suporte.

Você pode configurar a política usando os valores: 'basic', 'digest', 'ntlm' e 'negotiate'. Separe vários valores por vírgulas.

Se você não configurar essa política, todos os quatro esquemas serão usados.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Não - Requer a reinicialização do navegador

  #### Tipo de Dados:
  Cadeia de Caracteres

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: AuthSchemes
  - Nome da GP: Esquemas de autenticação com suporte
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/Autenticação HTTP
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: AuthSchemes
  - Tipo de Valor: REG_SZ
  ##### Exemplo de valor:
```
"basic,digest,ntlm,negotiate"
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: AuthSchemes
  - Exemplo de valor:
``` xml
<string>basic,digest,ntlm,negotiate</string>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### AuthServerAllowlist
  #### Configurar lista de servidores de autenticação permitidos
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Especifica quais servidores devem ser habilitados para a autenticação integrada. A autenticação integrada só é habilitada quando o Microsoft Edge recebe um desafio de autenticação de um proxy ou servidor na lista.

Separe vários nomes de servidor com vírgulas. São permitidos curingas (*).

Se você não configurar essa política, o Microsoft Edge tentará detectar se um servidor está na intranet. Somente depois disso, ele responderá às solicitações IWA. Se o servidor estiver na internet, as solicitações IWA provenientes dele serão ignoradas pelo Microsoft Edge.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Não - Requer a reinicialização do navegador

  #### Tipo de Dados:
  Cadeia de Caracteres

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: AuthServerAllowlist
  - Nome da GP: Configurar lista de servidores de autenticação permitidos
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/Autenticação HTTP
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: AuthServerAllowlist
  - Tipo de Valor: REG_SZ
  ##### Exemplo de valor:
```
"*contoso.com,contoso.com"
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: AuthServerAllowlist
  - Exemplo de valor:
``` xml
<string>*contoso.com,contoso.com</string>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### DisableAuthNegotiateCnameLookup
  #### Desabilitar pesquisa CNAME ao negociar a autenticação Kerberos
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Determina se o SPN do Kerberos gerado é baseado no nome DNS canônico (CNAME) ou no nome original inserido.

Se você habilitar essa política, a pesquisa CNAME será ignorada e o nome do servidor será usado (conforme inserido).

Se você desabilitar essa política ou não a configurar, o nome canônico do servidor será usado. Isso é determinado via pesquisa CNAME.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Não - Requer a reinicialização do navegador

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: DisableAuthNegotiateCnameLookup
  - Nome da GP: Desabilitar pesquisa CNAME ao negociar a autenticação Kerberos
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/Autenticação HTTP
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: DisableAuthNegotiateCnameLookup
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000000
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: DisableAuthNegotiateCnameLookup
  - Exemplo de valor:
``` xml
<false/>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### EnableAuthNegotiatePort
  #### Incluir porta não padrão no SPN do Kerberos
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Especifica se o SPN do Kerberos gerado deve incluir uma porta não padrão.

Se essa política for habilitada e um usuário inclui uma porta não padrão (uma porta diferente de 80 ou 443) em uma URL, essa porta será incluída no SPN do Kerberos gerado.

Se você não configurar ou desabilitar essa política, o SPN do Kerberos gerado não incluirá uma porta em nenhum caso.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Não - Requer a reinicialização do navegador

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: EnableAuthNegotiatePort
  - Nome da GP: Incluir porta não padrão no SPN do Kerberos
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/Autenticação HTTP
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: EnableAuthNegotiatePort
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000000
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: EnableAuthNegotiatePort
  - Exemplo de valor:
``` xml
<false/>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### NtlmV2Enabled
  #### Controlar se a autenticação NTLMv2 está habilitada
  >Versões com Suporte: O Microsoft Edge no Mac desde a versão 77 ou posterior

  #### Descrição
  Controla se o NTLMv2 está habilitado.

Todas as versões recentes dos servidores Samba e Windows oferecem suporte a NTLMv2. Você só deve desabilitar o NTLMv2 para resolver problemas de compatibilidade com versões anteriores, já que ele reduz a segurança da autenticação.

Se você não configurar esta política, o NTLMv2 estará habilitado por padrão.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Booliano

  

  #### Informações e configurações do Mac
  - Nome da chave de preferência: NtlmV2Enabled
  - Exemplo de valor:
``` xml
<true/>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ## Cast policies

  [Voltar ao início](#microsoft-edge---políticas)

  ### EnableMediaRouter
  #### Habilitar Google Cast
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Habilite essa política para habilitar o Google Cast. Os usuários poderão iniciá-lo por meio do menu do app, dos menus de contexto das páginas, dos controles de mídia em sites habilitados para o Cast e (se exibido) do ícone da barra de ferramentas do Cast.

Desabilite essa política para desativar o Google Cast.

Por padrão, o Google Cast é habilitado.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Não - Requer a reinicialização do navegador

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: EnableMediaRouter
  - Nome da GP: Habilitar Google Cast
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/Cast
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: EnableMediaRouter
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000001
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: EnableMediaRouter
  - Exemplo de valor:
``` xml
<true/>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### ShowCastIconInToolbar
  #### Mostrar o ícone de transmissão na barra de ferramentas
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Defina essa política como true para mostrar o ícone da barra de ferramentas Transmitir na barra de ferramentas ou no Menu Estouro. Os usuários não poderão removê-lo.

Se você não definir essa política ou desativá-la, os usuários poderão fixar ou remover o ícone usando o menu contextual.

Se você definir também a política [EnableMediaRouter](#enablemediarouter) como false, essa política será ignorada e o ícone da barra de ferramentas não será mostrado.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Não - Requer a reinicialização do navegador

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: ShowCastIconInToolbar
  - Nome da GP: Mostrar o ícone de transmissão na barra de ferramentas
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/Cast
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: ShowCastIconInToolbar
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000000
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: ShowCastIconInToolbar
  - Exemplo de valor:
``` xml
<false/>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ## Configurações de conteúdo policies

  [Voltar ao início](#microsoft-edge---políticas)

  ### AutoSelectCertificateForUrls
  #### Selecionar automaticamente os certificados de cliente para estes sites
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Especifica uma lista de sites, com base nos padrões de URL, para os quais o Microsoft Edge deve selecionar automaticamente um certificado de cliente, se o site solicitar um.

O valor deve ser uma matriz de dicionários JSON de cadeias de caracteres. A forma de cada dicionário é { "pattern": "$URL_PATTERN", "filter" : $FILTER }, onde $URL_PATTERN é um padrão de configuração de conteúdo. $FILTER restringe os certificados de cliente que o navegador selecionará automaticamente. Independentemente do filtro, somente os certificados que correspondem à solicitação de certificado do servidor serão selecionados. Por exemplo, se $FILTER tiver a forma { "ISSUER": { "CN": "$ISSUER_CN" } }, serão selecionados apenas certificados de cliente emitidos por um certificado com o CommonName $ISSUER_CN. Se $FILTER contiver "ISSUER" e uma seção "SUBJECT", um certificado de cliente deverá atender às duas condições para ser selecionado. Se $FILTER especificar uma organização ("O"), um certificado deverá ter pelo menos uma organização que corresponda ao valor especificado para ser selecionado. Se $FILTER especificar uma unidade organizacional ("UO"), um certificado deverá ter pelo menos uma unidade organizacional que corresponda ao valor especificado para ser selecionado. Se $FILTER for um dicionário vazio {}, a seleção de certificados de cliente não será restrita.

Se você não configurar essa política, a seleção automática não será feita para os sites.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Lista de cadeias de caracteres

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: AutoSelectCertificateForUrls
  - Nome da GP: Selecionar automaticamente os certificados de cliente para estes sites
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/Configurações de conteúdo
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge\AutoSelectCertificateForUrls
  - Caminho (Recomendações): N/A
  - Nome do Valor: 1, 2, 3, ...
  - Tipo de Valor: lista de REG_SZ
  ##### Exemplo de valor:
```
SOFTWARE\Policies\Microsoft\Edge\AutoSelectCertificateForUrls\0 = "{"pattern":"https://www.contoso.com","filter":{"ISSUER":{"CN":"certificate issuer name", "L": "certificate issuer location", "O": "certificate issuer org", "OU": "certificate issuer org unit"}, "SUBJECT":{"CN":"certificate subject name", "L": "certificate subject location", "O": "certificate subject org", "OU": "certificate subject org unit"}}}"

```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: AutoSelectCertificateForUrls
  - Exemplo de valor:
``` xml
<array>
  <string>{"pattern":"https://www.contoso.com","filter":{"ISSUER":{"CN":"certificate issuer name", "L": "certificate issuer location", "O": "certificate issuer org", "OU": "certificate issuer org unit"}, "SUBJECT":{"CN":"certificate subject name", "L": "certificate subject location", "O": "certificate subject org", "OU": "certificate subject org unit"}}}</string>
</array>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### CookiesAllowedForUrls
  #### Permitir cookies em sites específicos
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Define uma lista de sites, com base em padrões de URL, que não podem definir cookies.

Se você não configurar esta política, será usado o valor padrão global da política [DefaultCookiesSetting](#defaultcookiessetting) (se definida) ou a configuração pessoal do usuário para todos os sites.

Consulte as políticas [CookiesBlockedForUrls](#cookiesblockedforurls) e [CookiesSessionOnlyForUrls](#cookiessessiononlyforurls) para obter mais informações.

Observe que não pode haver padrões de URL em conflito definidos entre estas três políticas:

- [CookiesBlockedForUrls](#cookiesblockedforurls)

- CookiesAllowedForUrls

- [CookiesSessionOnlyForUrls](#cookiessessiononlyforurls)

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Lista de cadeias de caracteres

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: CookiesAllowedForUrls
  - Nome da GP: Permitir cookies em sites específicos
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/Configurações de conteúdo
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge\CookiesAllowedForUrls
  - Caminho (Recomendações): N/A
  - Nome do Valor: 1, 2, 3, ...
  - Tipo de Valor: lista de REG_SZ
  ##### Exemplo de valor:
```
SOFTWARE\Policies\Microsoft\Edge\CookiesAllowedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\CookiesAllowedForUrls\1 = "[*.]contoso.edu"

```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: CookiesAllowedForUrls
  - Exemplo de valor:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### CookiesBlockedForUrls
  #### Bloquear cookies em sites específicos
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Define uma lista de sites, com base em padrões de URL, que não podem definir cookies.

Se você não configurar esta política, será usado o valor padrão global da política [DefaultCookiesSetting](#defaultcookiessetting) (se definida) ou a configuração pessoal do usuário para todos os sites.

Consulte as políticas [CookiesAllowedForUrls](#cookiesallowedforurls) e [CookiesSessionOnlyForUrls](#cookiessessiononlyforurls) para obter mais informações.

Observe que não pode haver padrões de URL em conflito definidos entre estas três políticas:

- CookiesBlockedForUrls

- [CookiesAllowedForUrls](#cookiesallowedforurls)

- [CookiesSessionOnlyForUrls](#cookiessessiononlyforurls)

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Lista de cadeias de caracteres

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: CookiesBlockedForUrls
  - Nome da GP: Bloquear cookies em sites específicos
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/Configurações de conteúdo
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge\CookiesBlockedForUrls
  - Caminho (Recomendações): N/A
  - Nome do Valor: 1, 2, 3, ...
  - Tipo de Valor: lista de REG_SZ
  ##### Exemplo de valor:
```
SOFTWARE\Policies\Microsoft\Edge\CookiesBlockedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\CookiesBlockedForUrls\1 = "[*.]contoso.edu"

```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: CookiesBlockedForUrls
  - Exemplo de valor:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### CookiesSessionOnlyForUrls
  #### Limitar cookies de sites específicos para a sessão atual
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Os cookies criados por sites que correspondam a um padrão de URL que você definir serão excluídos quando a sessão for encerrada (quando a janela for fechada).

Os cookies criados por sites que não correspondam ao padrão serão controlados pela política [DefaultCookiesSetting](#defaultcookiessetting) (se definida) ou pela configuração pessoal do usuário. Esse também será o comportamento padrão se você não configurar esta política.

Se o Microsoft Edge estiver em execução em segundo plano, a sessão talvez não seja encerrada quando a última janela for fechada, o que significa que os cookies não serão limpos quando a janela for fechada. Consulte a política [BackgroundModeEnabled](#backgroundmodeenabled) para obter informações sobre como configurar o que acontece quando o Microsoft Edge é executado em segundo plano.

Você também pode usar as políticas [CookiesAllowedForUrls](#cookiesallowedforurls) e [CookiesBlockedForUrls](#cookiesblockedforurls) para controlar os sites que podem criar cookies.

Observe que não pode haver padrões de URL em conflito definidos entre estas três políticas:

- [CookiesBlockedForUrls](#cookiesblockedforurls)

- [CookiesAllowedForUrls](#cookiesallowedforurls)

- CookiesSessionOnlyForUrls

Se você definir a política [RestoreOnStartup](#restoreonstartup) para restaurar URLs de sessões anteriores, esta política será ignorada e os cookies serão armazenados permanentemente para esses sites.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Lista de cadeias de caracteres

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: CookiesSessionOnlyForUrls
  - Nome da GP: Limitar cookies de sites específicos para a sessão atual
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/Configurações de conteúdo
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge\CookiesSessionOnlyForUrls
  - Caminho (Recomendações): N/A
  - Nome do Valor: 1, 2, 3, ...
  - Tipo de Valor: lista de REG_SZ
  ##### Exemplo de valor:
```
SOFTWARE\Policies\Microsoft\Edge\CookiesSessionOnlyForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\CookiesSessionOnlyForUrls\1 = "[*.]contoso.edu"

```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: CookiesSessionOnlyForUrls
  - Exemplo de valor:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### DefaultCookiesSetting
  #### Configurar cookies
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Controla se os sites podem criar cookies no dispositivo do usuário. Esta política é tudo ou nada: você pode permitir que todos os sites criem cookies ou que nenhum site crie cookies. Você não pode usar esta política para habilitar cookies de sites específicos.

Defina a política como "SessionOnly" (4) para limpar cookies quando a sessão for encerrada. Se o Microsoft Edge estiver sendo executado em segundo plano, a sessão talvez não seja encerrada quando a última janela for fechada, o que significa que os cookies não serão limpos quando a janela for fechada. Consulte a política [BackgroundModeEnabled](#backgroundmodeenabled) para obter informações sobre como configurar o que acontece quando o Microsoft Edge é executado em segundo plano.

Se você não configurar esta política, será usado o padrão "AllowCookies" (1), e os usuários poderão alterar isso nas Configurações do Microsoft Edge. (Se você não quiser que os usuários sejam capazes de alterar essa configuração, defina a política.)

* 1 = Permitir que todos os sites criem cookies

* 2 = Não permitir que nenhum site crie cookies

* 4 = Manter os cookies enquanto durar a sessão

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Número inteiro

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: DefaultCookiesSetting
  - Nome da GP: Configurar cookies
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/Configurações de conteúdo
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: DefaultCookiesSetting
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000001
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: DefaultCookiesSetting
  - Exemplo de valor:
``` xml
<integer>1</integer>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### DefaultGeolocationSetting
  #### Configuração de geolocalização padrão
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Define se os sites podem rastrear a localização física do usuário. Você pode permitir o rastreamento por padrão (1), negá-lo por padrão (2) ou perguntar ao usuário toda vez que um site solicitar a localização dele (3).

Se você não configurar essa política, a política de 'AskGeolocation' será usada e o usuário poderá alterá-la.

* 1 = Permitir que sites rastreiem a localização física do usuário

* 2 = Não permitir que sites rastreiem a localização física do usuário

* 3 = Perguntar sempre que um site solicitar rastrear a localização física do usuário

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Número inteiro

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: DefaultGeolocationSetting
  - Nome da GP: Configuração de geolocalização padrão
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/Configurações de conteúdo
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: DefaultGeolocationSetting
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000001
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: DefaultGeolocationSetting
  - Exemplo de valor:
``` xml
<integer>1</integer>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### DefaultImagesSetting
  #### Configuração de imagens padrão
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Define se os sites podem exibir imagens. Você pode permitir imagens em todos os sites (1) ou bloqueá-las em todos os sites (2).

Se você não configurar essa política, as imagens serão permitidas por padrão, e o usuário poderá alterar essa configuração.

* 1 = Permitir que todos os sites mostrem todas as imagens

* 2 = Não permitir que sites mostrem imagens

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Número inteiro

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: DefaultImagesSetting
  - Nome da GP: Configuração de imagens padrão
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/Configurações de conteúdo
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: DefaultImagesSetting
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000001
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: DefaultImagesSetting
  - Exemplo de valor:
``` xml
<integer>1</integer>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### DefaultInsecureContentSetting
  #### Controlar uso de exceções de conteúdo não seguro
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 80 ou posterior

  #### Descrição
  Permite definir se os usuários podem adicionar exceções para permitir conteúdo misto para sites específicos.

Essa política pode ser substituída por padrões de URL específicos usando as políticas [InsecureContentAllowedForUrls](#insecurecontentallowedforurls) e [InsecureContentBlockedForUrls](#insecurecontentblockedforurls).

Se essa política não for definida, os usuários terão permissão para adicionar exceções para permitir conteúdo misto bloqueável e desabilitar atualizações automáticas para conteúdo misto opcionalmente bloqueável.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Número inteiro

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: DefaultInsecureContentSetting
  - Nome da GP: Controlar uso de exceções de conteúdo não seguro
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/Configurações de conteúdo
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: DefaultInsecureContentSetting
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000002
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: DefaultInsecureContentSetting
  - Exemplo de valor:
``` xml
<integer>2</integer>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### DefaultJavaScriptSetting
  #### Configuração de JavaScript padrão
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Define se os sites podem executar o JavaScript. Você pode permitir a execução do JavaScript em todos os sites (1) ou bloquear a execução dele em todos os sites (2).

Se você não configurar essa política, todos os sites poderão executar o JavaScript por padrão e o usuário poderá alterar essa configuração.

* 1 = Permitir que todos os sites executem o JavaScript

* 2 = Não permitir que o site execute o JavaScript

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Número inteiro

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: DefaultJavaScriptSetting
  - Nome da GP: Configuração de JavaScript padrão
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/Configurações de conteúdo
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: DefaultJavaScriptSetting
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000001
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: DefaultJavaScriptSetting
  - Exemplo de valor:
``` xml
<integer>1</integer>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### DefaultNotificationsSetting
  #### Configuração de notificação padrão
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Define se os sites podem exibir notificações na área de trabalho. Você pode aceitá-las por padrão (1), recusá-las por padrão (2) ou receber uma solicitação sempre que um site precisar mostrar uma notificação (3).

Se você não configurar essa política, as notificações serão aceitas por padrão e o usuário poderá alterar essa configuração.

* 1 = Permitir que sites mostrem notificações na área de trabalho

* 2 = Não permitir que sites mostrem notificações na área de trabalho

* 3 = Solicitar sempre que um site precisar mostrar notificações na área de trabalho

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Número inteiro

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: DefaultNotificationsSetting
  - Nome da GP: Configuração de notificação padrão
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/Configurações de conteúdo
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: DefaultNotificationsSetting
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000002
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: DefaultNotificationsSetting
  - Exemplo de valor:
``` xml
<integer>2</integer>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### DefaultPluginsSetting
  #### Configuração padrão do Adobe Flash
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Determina se os sites que não são cobertos por [PluginsAllowedForUrls](#pluginsallowedforurls) ou [PluginsBlockedForUrls](#pluginsblockedforurls) podem executar automaticamente o plug-in Adobe Flash. Você pode selecionar "BlockPlugins" (2) para bloquear o Adobe Flash em todos os sites, ou você pode selecionar "ClickToPlay" (3) para permitir que o Adobe Flash seja executado, mas exigir que o usuário clique no espaço reservado para iniciá-lo. De qualquer forma, as políticas [PluginsAllowedForUrls](#pluginsallowedforurls) e [PluginsBlockedForUrls](#pluginsblockedforurls) prevalecerão sobre [DefaultPluginsSetting](#defaultpluginssetting).

A reprodução automática é permitida somente para domínios listados explicitamente na política [PluginsAllowedForUrls](#pluginsallowedforurls). Se você quiser habilitar a reprodução automática para todos os sites, é recomendável adicionar http://* e https://* a essa lista.

Se você não configurar essa política, o usuário poderá alterar essa configuração manualmente.

* 2 = Bloquear o plug-in Adobe Flash

* 3 = Clicar para executar

A opção "1" anterior definia allow-all, mas agora essa funcionalidade é controlada apenas pela política [PluginsAllowedForUrls](#pluginsallowedforurls).  As políticas existentes que usam a opção "1" funcionarão no modo Clicar para executar.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Número inteiro

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: DefaultPluginsSetting
  - Nome da GP: Configuração padrão do Adobe Flash
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/Configurações de conteúdo
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: DefaultPluginsSetting
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000002
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: DefaultPluginsSetting
  - Exemplo de valor:
``` xml
<integer>2</integer>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### DefaultPopupsSetting
  #### Configuração de janela pop-up padrão
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Define se os sites poderão mostrar janelas pop-up. Você pode permiti-las em todos os sites (1) ou bloqueá-las em todos os sites (2).

Se você não configurar essa política, as janelas pop-up serão bloqueadas por padrão, e os usuários poderão alterar essa configuração.

* 1 = Permitir que todos os sites mostrem janelas pop-ups

* 2 = Não permitir que sites mostrem janelas pop-up

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Número inteiro

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: DefaultPopupsSetting
  - Nome da GP: Configuração de janela pop-up padrão
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/Configurações de conteúdo
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: DefaultPopupsSetting
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000001
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: DefaultPopupsSetting
  - Exemplo de valor:
``` xml
<integer>1</integer>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### DefaultWebBluetoothGuardSetting
  #### Controlar o uso da API Web Bluetooth
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Controla se os sites podem acessar dispositivos Bluetooth próximos. Você pode bloquear completamente o acesso ou exigir que o site pergunte ao usuário sempre que ele quiser acessar um dispositivo Bluetooth.

Se você não configurar esta política, será usado o valor padrão (3, que significa que os usuários serão sempre perguntados) e os usuários poderão alterá-lo.

* 2 = Não permitir que nenhum site solicite acesso a dispositivos Bluetooth usando a API Web Bluetooth

* 3 = Permitir que os sites peçam ao usuário para conceder acesso a um dispositivo Bluetooth próximo

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Número inteiro

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: DefaultWebBluetoothGuardSetting
  - Nome da GP: Controlar o uso da API Web Bluetooth
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/Configurações de conteúdo
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: DefaultWebBluetoothGuardSetting
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000002
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: DefaultWebBluetoothGuardSetting
  - Exemplo de valor:
``` xml
<integer>2</integer>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### DefaultWebUsbGuardSetting
  #### Controlar o uso da API WebUSB
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Define se os sites podem acessar dispositivos USB conectados. Você pode bloquear totalmente o acesso ou perguntar ao usuário toda vez que um site precisar obter acesso a dispositivos USB conectados.

Você pode substituir essa política por padrões de URL específicos usando as políticas [WebUsbAskForUrls](#webusbaskforurls) e [WebUsbBlockedForUrls](#webusbblockedforurls).

Se você não definir essa política, os sites poderão solicitar aos usuários a permissão para acessar os dispositivos USB conectados (3) por padrão, e os usuários poderão alterar essa configuração.

* 2 = Não permitir que sites solicitem acesso a dispositivos USB por meio da API WebUSB

* 3 = Permitir que sites solicitem ao usuário a permissão para acessar um dispositivo USB conectado

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Número inteiro

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: DefaultWebUsbGuardSetting
  - Nome da GP: Controlar o uso da API WebUSB
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/Configurações de conteúdo
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: DefaultWebUsbGuardSetting
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000002
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: DefaultWebUsbGuardSetting
  - Exemplo de valor:
``` xml
<integer>2</integer>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### ImagesAllowedForUrls
  #### Permitir imagens nestes sites
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Define uma lista de sites, com base em padrões de URL, que podem exibir imagens.

Se você não configurar esta política, será usado para todos os sites o valor padrão global da política [DefaultImagesSetting](#defaultimagessetting) (se definida) ou a configuração pessoal do usuário.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Lista de cadeias de caracteres

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: ImagesAllowedForUrls
  - Nome da GP: Permitir imagens nestes sites
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/Configurações de conteúdo
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge\ImagesAllowedForUrls
  - Caminho (Recomendações): N/A
  - Nome do Valor: 1, 2, 3, ...
  - Tipo de Valor: lista de REG_SZ
  ##### Exemplo de valor:
```
SOFTWARE\Policies\Microsoft\Edge\ImagesAllowedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\ImagesAllowedForUrls\1 = "[*.]contoso.edu"

```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: ImagesAllowedForUrls
  - Exemplo de valor:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### ImagesBlockedForUrls
  #### Bloquear imagens em sites específicos
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Define uma lista de sites, com base em padrões de URL, que não têm permissão para exibir imagens.

Se você não configurar esta política, será usado o valor padrão global da política [DefaultImagesSetting](#defaultimagessetting) (se definida) ou a configuração pessoal do usuário para todos os sites.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Lista de cadeias de caracteres

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: ImagesBlockedForUrls
  - Nome da GP: Bloquear imagens em sites específicos
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/Configurações de conteúdo
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge\ImagesBlockedForUrls
  - Caminho (Recomendações): N/A
  - Nome do Valor: 1, 2, 3, ...
  - Tipo de Valor: lista de REG_SZ
  ##### Exemplo de valor:
```
SOFTWARE\Policies\Microsoft\Edge\ImagesBlockedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\ImagesBlockedForUrls\1 = "[*.]contoso.edu"

```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: ImagesBlockedForUrls
  - Exemplo de valor:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### InsecureContentAllowedForUrls
  #### Permitir conteúdo não seguro em sites especificados
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 80 ou posterior

  #### Descrição
  Permite definir uma lista de padrões de URL que especificam sites que têm permissão para exibir conteúdo misto (ou seja, ativo) bloqueável (ou seja, conteúdo HTTP em sites HTTPS) e para os quais a atualização do conteúdo misto opcionalmente bloqueável será desabilitada.

Se essa política não for definida, o conteúdo misto bloqueável será bloqueado e, opcionalmente, o conteúdo misto bloqueável será atualizado, e os usuários terão permissão para definir exceções para permitir sites específicos.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Lista de cadeias de caracteres

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: InsecureContentAllowedForUrls
  - Nome da GP: Permitir conteúdo não seguro em sites especificados
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/Configurações de conteúdo
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge\InsecureContentAllowedForUrls
  - Caminho (Recomendações): N/A
  - Nome do Valor: 1, 2, 3, ...
  - Tipo de Valor: lista de REG_SZ
  ##### Exemplo de valor:
```
SOFTWARE\Policies\Microsoft\Edge\InsecureContentAllowedForUrls\0 = "https://www.example.com"
SOFTWARE\Policies\Microsoft\Edge\InsecureContentAllowedForUrls\1 = "[*.]example.edu"

```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: InsecureContentAllowedForUrls
  - Exemplo de valor:
``` xml
<array>
  <string>https://www.example.com</string>
  <string>[*.]example.edu</string>
</array>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### InsecureContentBlockedForUrls
  #### Bloquear conteúdo não seguro em sites especificados
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 80 ou posterior

  #### Descrição
  Permite definir uma lista de padrões de URL que especificam sites que não têm permissão para exibir conteúdo misto (ou seja, ativo) bloqueável (ou seja, conteúdo HTTP em sites HTTPS) e para os quais o conteúdo misto opcionalmente bloqueável (ou seja, passivo) será atualizado.

Se essa política não for definida, o conteúdo misto bloqueável será bloqueado e, opcionalmente, o conteúdo misto bloqueável será atualizado, mas os usuários terão permissão para definir exceções para permitir sites específicos.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Lista de cadeias de caracteres

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: InsecureContentBlockedForUrls
  - Nome da GP: Bloquear conteúdo não seguro em sites especificados
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/Configurações de conteúdo
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge\InsecureContentBlockedForUrls
  - Caminho (Recomendações): N/A
  - Nome do Valor: 1, 2, 3, ...
  - Tipo de Valor: lista de REG_SZ
  ##### Exemplo de valor:
```
SOFTWARE\Policies\Microsoft\Edge\InsecureContentBlockedForUrls\0 = "https://www.example.com"
SOFTWARE\Policies\Microsoft\Edge\InsecureContentBlockedForUrls\1 = "[*.]example.edu"

```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: InsecureContentBlockedForUrls
  - Exemplo de valor:
``` xml
<array>
  <string>https://www.example.com</string>
  <string>[*.]example.edu</string>
</array>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### JavaScriptAllowedForUrls
  #### Permitir JavaScript em sites específicos
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Define uma lista de sites, com base em padrões de URL, que têm permissão para executar JavaScript.

Se você não configurar esta política, será usado o valor padrão global da política [DefaultJavaScriptSetting](#defaultjavascriptsetting) (se definida) ou a configuração de pessoal do usuário para todos os sites.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Lista de cadeias de caracteres

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: JavaScriptAllowedForUrls
  - Nome da GP: Permitir JavaScript em sites específicos
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/Configurações de conteúdo
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge\JavaScriptAllowedForUrls
  - Caminho (Recomendações): N/A
  - Nome do Valor: 1, 2, 3, ...
  - Tipo de Valor: lista de REG_SZ
  ##### Exemplo de valor:
```
SOFTWARE\Policies\Microsoft\Edge\JavaScriptAllowedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\JavaScriptAllowedForUrls\1 = "[*.]contoso.edu"

```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: JavaScriptAllowedForUrls
  - Exemplo de valor:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### JavaScriptBlockedForUrls
  #### Bloquear o JavaScript em sites específicos
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Define uma lista de sites, com base em padrões de URL, que não têm permissão para executar JavaScript.

Se você não configurar esta política, será usado o valor padrão global da política [DefaultJavaScriptSetting](#defaultjavascriptsetting) (se definida) ou a configuração de pessoal do usuário para todos os sites.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Lista de cadeias de caracteres

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: JavaScriptBlockedForUrls
  - Nome da GP: Bloquear o JavaScript em sites específicos
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/Configurações de conteúdo
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge\JavaScriptBlockedForUrls
  - Caminho (Recomendações): N/A
  - Nome do Valor: 1, 2, 3, ...
  - Tipo de Valor: lista de REG_SZ
  ##### Exemplo de valor:
```
SOFTWARE\Policies\Microsoft\Edge\JavaScriptBlockedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\JavaScriptBlockedForUrls\1 = "[*.]contoso.edu"

```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: JavaScriptBlockedForUrls
  - Exemplo de valor:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### LegacySameSiteCookieBehaviorEnabled
  #### Habilitar a configuração do comportamento de cookies SameSite herdado padrão
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 80 ou posterior

  #### Descrição
  Permite reverter todos os cookies para o comportamento SameSite herdado. A reversão para o comportamento herdado faz com que os cookies que não especificam o atributo SameSite sejam tratados como se fossem "SameSite=None" e remove o requisito para que os cookies "SameSite=None" contenham o atributo "Secure".

Você pode definir os seguintes valores para esta política:

* 1 = Reverter ao comportamento SameSite herdado para cookies em todos os sites

* 2 = Usar o comportamento SameSite-by-default para cookies em todos os sites

Se você não configurar esta política, o comportamento padrão para os cookies que não especificam um atributo SameSite dependerá de outras fontes de configuração do recurso SameSite-by-default. Este recurso pode ser configurado por uma avaliação de campo ou pela habilitação do sinalizador same-site-by-default-cookies em edge://flags.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Número inteiro

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: LegacySameSiteCookieBehaviorEnabled
  - Nome da GP: Habilitar a configuração do comportamento de cookies SameSite herdado padrão
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/Configurações de conteúdo
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: LegacySameSiteCookieBehaviorEnabled
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000001
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: LegacySameSiteCookieBehaviorEnabled
  - Exemplo de valor:
``` xml
<integer>1</integer>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### LegacySameSiteCookieBehaviorEnabledForDomainList
  #### Reverter para o comportamento SameSite herdado de cookies em sites especificados
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 80 ou posterior

  #### Descrição
  Os cookies configurados para padrões especificados de correspondência de domínios serão revertidos para o comportamento SameSite herdado.

Reverter para o comportamento herdado faz com que os cookies que não especificam um atributo SameSite sejam tratados como se fossem "SameSite=None" e remove o requisito para que os cookies "SameSite=None" contenham o atributo "Secure".

Se você não configurar esta política, o valor padrão global será usado. O padrão global também será usado para cookies em domínios não cobertos pelos padrões especificados.

O valor padrão global pode ser configurado usando a política [LegacySameSiteCookieBehaviorEnabled](#legacysamesitecookiebehaviorenabled). Se [LegacySameSiteCookieBehaviorEnabled](#legacysamesitecookiebehaviorenabled) não estiver configurado, o valor padrão global será aquele usado em outras fontes de configuração.

Observe que os padrões listados nesta política são tratados como domínios, não URLs. Portanto, você não deve especificar um esquema ou porta.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Lista de cadeias de caracteres

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: LegacySameSiteCookieBehaviorEnabledForDomainList
  - Nome da GP: Reverter para o comportamento SameSite herdado de cookies em sites especificados
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/Configurações de conteúdo
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge\LegacySameSiteCookieBehaviorEnabledForDomainList
  - Caminho (Recomendações): N/A
  - Nome do Valor: 1, 2, 3, ...
  - Tipo de Valor: lista de REG_SZ
  ##### Exemplo de valor:
```
SOFTWARE\Policies\Microsoft\Edge\LegacySameSiteCookieBehaviorEnabledForDomainList\0 = "www.example.com"
SOFTWARE\Policies\Microsoft\Edge\LegacySameSiteCookieBehaviorEnabledForDomainList\1 = "[*.]example.edu"

```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: LegacySameSiteCookieBehaviorEnabledForDomainList
  - Exemplo de valor:
``` xml
<array>
  <string>www.example.com</string>
  <string>[*.]example.edu</string>
</array>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### NotificationsAllowedForUrls
  #### Permitir notificações em sites específicos
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Define uma lista de sites, com base em padrões de URL, que podem exibir notificações.

Se você não configurar esta política, será usado o valor padrão global da política [DefaultNotificationsSetting](#defaultnotificationssetting) (se definida) ou a configuração pessoal do usuário para todos os sites.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Lista de cadeias de caracteres

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: NotificationsAllowedForUrls
  - Nome da GP: Permitir notificações em sites específicos
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/Configurações de conteúdo
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge\NotificationsAllowedForUrls
  - Caminho (Recomendações): N/A
  - Nome do Valor: 1, 2, 3, ...
  - Tipo de Valor: lista de REG_SZ
  ##### Exemplo de valor:
```
SOFTWARE\Policies\Microsoft\Edge\NotificationsAllowedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\NotificationsAllowedForUrls\1 = "[*.]contoso.edu"

```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: NotificationsAllowedForUrls
  - Exemplo de valor:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### NotificationsBlockedForUrls
  #### Bloquear notificações em sites específicos
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Define uma lista de sites, com base em padrões de URL, que são impedidos de exibir notificações.

Se você não configurar esta política, será usado o valor padrão global da política [DefaultNotificationsSetting](#defaultnotificationssetting) (se definida) ou a configuração pessoal do usuário para todos os sites.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Lista de cadeias de caracteres

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: NotificationsBlockedForUrls
  - Nome da GP: Bloquear notificações em sites específicos
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/Configurações de conteúdo
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge\NotificationsBlockedForUrls
  - Caminho (Recomendações): N/A
  - Nome do Valor: 1, 2, 3, ...
  - Tipo de Valor: lista de REG_SZ
  ##### Exemplo de valor:
```
SOFTWARE\Policies\Microsoft\Edge\NotificationsBlockedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\NotificationsBlockedForUrls\1 = "[*.]contoso.edu"

```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: NotificationsBlockedForUrls
  - Exemplo de valor:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### PluginsAllowedForUrls
  #### Permitir o plug-in do Adobe Flash em sites específicos
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Define uma lista de sites, com base em padrões de URL, que podem executar o plug-in Adobe Flash.

Se você não configurar essa política, será usado o valor padrão global da política [DefaultPluginsSetting](#defaultpluginssetting) ou a configuração pessoal do usuário para todos os sites.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Lista de cadeias de caracteres

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: PluginsAllowedForUrls
  - Nome da GP: Permitir o plug-in do Adobe Flash em sites específicos
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/Configurações de conteúdo
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge\PluginsAllowedForUrls
  - Caminho (Recomendações): N/A
  - Nome do Valor: 1, 2, 3, ...
  - Tipo de Valor: lista de REG_SZ
  ##### Exemplo de valor:
```
SOFTWARE\Policies\Microsoft\Edge\PluginsAllowedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\PluginsAllowedForUrls\1 = "[*.]contoso.edu"

```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: PluginsAllowedForUrls
  - Exemplo de valor:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### PluginsBlockedForUrls
  #### Bloquear o plug-in do Adobe Flash em sites específicos
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Define uma lista de sites, com base nos padrões de URL, que são impedidos de executar o Adobe Flash.

Se você não configurar essa política, será usado o valor padrão global da política [DefaultPluginsSetting](#defaultpluginssetting) (se definida) ou a configuração pessoal do usuário para todos os sites.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Lista de cadeias de caracteres

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: PluginsBlockedForUrls
  - Nome da GP: Bloquear o plug-in do Adobe Flash em sites específicos
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/Configurações de conteúdo
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge\PluginsBlockedForUrls
  - Caminho (Recomendações): N/A
  - Nome do Valor: 1, 2, 3, ...
  - Tipo de Valor: lista de REG_SZ
  ##### Exemplo de valor:
```
SOFTWARE\Policies\Microsoft\Edge\PluginsBlockedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\PluginsBlockedForUrls\1 = "[*.]contoso.edu"

```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: PluginsBlockedForUrls
  - Exemplo de valor:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### PopupsAllowedForUrls
  #### Permitir janelas pop-up em sites específicos
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Define uma lista de sites, com base em padrões de URL, que podem abrir janelas pop-up.

Se você não configurar esta política, será usado o valor padrão global da política [DefaultPopupsSetting](#defaultpopupssetting) (se definida) ou a configuração pessoal do usuário para todos os sites.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Lista de cadeias de caracteres

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: PopupsAllowedForUrls
  - Nome da GP: Permitir janelas pop-up em sites específicos
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/Configurações de conteúdo
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge\PopupsAllowedForUrls
  - Caminho (Recomendações): N/A
  - Nome do Valor: 1, 2, 3, ...
  - Tipo de Valor: lista de REG_SZ
  ##### Exemplo de valor:
```
SOFTWARE\Policies\Microsoft\Edge\PopupsAllowedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\PopupsAllowedForUrls\1 = "[*.]contoso.edu"

```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: PopupsAllowedForUrls
  - Exemplo de valor:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### PopupsBlockedForUrls
  #### Bloquear janelas pop-up em sites específicos
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Define uma lista de sites, com base nos padrões de URL, que são impedidos de abrir janelas pop-up.

Se você não configurar esta política, será usado o valor padrão global da política [DefaultPopupsSetting](#defaultpopupssetting) (se definida) ou a configuração pessoal do usuário para todos os sites.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Lista de cadeias de caracteres

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: PopupsBlockedForUrls
  - Nome da GP: Bloquear janelas pop-up em sites específicos
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/Configurações de conteúdo
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge\PopupsBlockedForUrls
  - Caminho (Recomendações): N/A
  - Nome do Valor: 1, 2, 3, ...
  - Tipo de Valor: lista de REG_SZ
  ##### Exemplo de valor:
```
SOFTWARE\Policies\Microsoft\Edge\PopupsBlockedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\PopupsBlockedForUrls\1 = "[*.]contoso.edu"

```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: PopupsBlockedForUrls
  - Exemplo de valor:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### RegisteredProtocolHandlers
  #### Registrar manipuladores de protocolo
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Registre uma lista de manipuladores de protocolo. Defina a propriedade Protocolo como o esquema (como "mailto") e a propriedade URL como o padrão de URL do aplicativo que manipula o esquema. O padrão pode incluir um "%s", que será substituído pela URL manipulada.

Você pode recomendar um valor específico para essa política, mas não pode exigir que seus usuários a usem.

Os manipuladores de protocolo registrados pela política são mesclados com todos os manipuladores registrados pelo usuário e ambos estão disponíveis para uso. O usuário pode substituir os manipuladores de protocolo instalados pela política instalando um novo manipulador padrão, mas eles não podem remover um manipulador de protocolo registrado pela política.

  #### Recursos com suporte:
  - Pode ser obrigatório: Não
  - Pode ser recomendado: Sim
  - Atualização de política dinâmica: Não - Requer a reinicialização do navegador

  #### Tipo de Dados:
  Dicionário

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: RegisteredProtocolHandlers
  - Nome da GP: Registrar manipuladores de protocolo
  - Caminho da GP (Obrigatório): N/A
  - Caminho da GP (Recomendações): Modelos Administrativos/Microsoft Edge - Configurações Padrão (os usuários podem substituir)/Configurações de conteúdo
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): N/A
  - Caminho (Recomendações): SOFTWARE\Policies\Microsoft\Edge\Recomendações
  - Nome do Valor: RegisteredProtocolHandlers
  - Tipo de Valor: REG_SZ
  ##### Exemplo de valor:
```
SOFTWARE\Policies\Microsoft\Edge\RegisteredProtocolHandlers = [
  {
    "default": true, 
    "protocol": "mailto", 
    "url": "https://mail.contoso.com/mail/?extsrc=mailto&url=%s"
  }
]
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: RegisteredProtocolHandlers
  - Exemplo de valor:
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
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### WebUsbAllowDevicesForUrls
  #### Conceder acesso a sites específicos para se conectar a dispositivos USB específicos
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Permite definir uma lista de URLs que especificam quais sites receberão automaticamente permissão para acessar um dispositivo USB com as IDs de fornecedor e de produto fornecidas. Cada item da lista deve conter tanto dispositivos quanto URLs para que a política seja válida. Cada item em dispositivos pode conter um campo de ID do fornecedor e de ID do produto (product ID). Qualquer ID omitida é tratada como curinga com uma exceção, e essa exceção é que não é possível especificar uma ID de produto sem que uma ID de fornecedor também seja especificada. Caso contrário, a política não será válida e será ignorada.

O modelo de permissão USB usa a URL do site solicitante ("URL de solicitação") e a URL do site do quadro de nível superior ("URL de inserção") para conceder permissão à URL de solicitação para acessar o dispositivo USB. A URL de solicitação pode ser diferente da URL de inserção quando o site solicitante é carregado em um iframe. Portanto, o campo "URLs" pode conter até duas cadeias de caracteres de URL delimitadas por uma vírgula para especificar as URLs de solicitação e de inserção, respectivamente. Se for especificada apenas uma URL, o acesso aos dispositivos USB correspondentes será concedido quando a URL do site solicitante corresponder a essa URL, independentemente do status de inserção. As URLs citadas em "urls" devem ser válidas, caso contrário, a política será ignorada.

Se essa política não for definida, o valor padrão global será usado para todos os sites da política [DefaultWebUsbGuardSetting](#defaultwebusbguardsetting), se definida, ou da configuração pessoal do usuário.

Os padrões de URL nessa política não devem conflitar com os que foram configurados via [WebUsbBlockedForUrls](#webusbblockedforurls). Se houver um conflito, essa política terá precedência sobre [WebUsbBlockedForUrls](#webusbblockedforurls) e [WebUsbAskForUrls](#webusbaskforurls).

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Dicionário

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: WebUsbAllowDevicesForUrls
  - Nome da GP: Conceder acesso a sites específicos para se conectar a dispositivos USB específicos
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/Configurações de conteúdo
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: WebUsbAllowDevicesForUrls
  - Tipo de Valor: REG_SZ
  ##### Exemplo de valor:
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


  #### Informações e configurações do Mac
  - Nome da chave de preferência: WebUsbAllowDevicesForUrls
  - Exemplo de valor:
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
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### WebUsbAskForUrls
  #### Permitir WebUSB em sites específicos
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Define uma lista de sites, com base em padrões de URL, que podem solicitar ao usuário acesso a um dispositivo USB.

Se você não configurar esta política, será usado o valor padrão global da política [DefaultWebUsbGuardSetting](#defaultwebusbguardsetting) (se definida) ou a configuração pessoal do usuário para todos os sites.

Os padrões de URL definidos nesta política não podem entrar em conflito com aqueles configurados na política [WebUsbBlockedForUrls](#webusbblockedforurls). Você não pode permitir e bloquear uma URL ao mesmo tempo.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Lista de cadeias de caracteres

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: WebUsbAskForUrls
  - Nome da GP: Permitir WebUSB em sites específicos
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/Configurações de conteúdo
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge\WebUsbAskForUrls
  - Caminho (Recomendações): N/A
  - Nome do Valor: 1, 2, 3, ...
  - Tipo de Valor: lista de REG_SZ
  ##### Exemplo de valor:
```
SOFTWARE\Policies\Microsoft\Edge\WebUsbAskForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\WebUsbAskForUrls\1 = "[*.]contoso.edu"

```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: WebUsbAskForUrls
  - Exemplo de valor:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### WebUsbBlockedForUrls
  #### Bloquear WebUSB em sites específicos
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Define uma lista de sites, com base em padrões de URL, que não podem solicitar ao usuário que conceda a eles acesso a um dispositivo USB.

Se você não configurar esta política, será usado o valor padrão global da política [DefaultWebUsbGuardSetting](#defaultwebusbguardsetting) (se definida) ou a configuração pessoal do usuário para todos os sites.

Os padrões de URL nesta política não podem entrar em conflito com aqueles configurados na política [WebUsbAskForUrls](#webusbaskforurls). Você não pode permitir e bloquear uma URL ao mesmo tempo.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Lista de cadeias de caracteres

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: WebUsbBlockedForUrls
  - Nome da GP: Bloquear WebUSB em sites específicos
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/Configurações de conteúdo
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge\WebUsbBlockedForUrls
  - Caminho (Recomendações): N/A
  - Nome do Valor: 1, 2, 3, ...
  - Tipo de Valor: lista de REG_SZ
  ##### Exemplo de valor:
```
SOFTWARE\Policies\Microsoft\Edge\WebUsbBlockedForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\WebUsbBlockedForUrls\1 = "[*.]contoso.edu"

```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: WebUsbBlockedForUrls
  - Exemplo de valor:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ## Configurações do SmartScreen policies

  [Voltar ao início](#microsoft-edge---políticas)

  ### PreventSmartScreenPromptOverride
  #### Impedir que avisos do Microsoft Defender SmartScreen sejam ignorados para sites
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Essa configuração de política permite que você decida se os usuários podem substituir os avisos do Microsoft Defender SmartScreen sobre sites potencialmente mal-intencionados.

Se você habilitar essa configuração, os usuários não poderão ignorar os avisos do Microsoft Defender SmartScreen e serão impedidos de continuar no site.

Se você desabilitar ou não definir essa configuração, os usuários poderão ignorar os avisos do Microsoft Defender SmartScreen e continuar no site.

Essa política está disponível somente em instâncias do Windows que fazem parte de um domínio do Microsoft Active Directory ou em instâncias do Windows 10 Pro ou Enterprise registradas para o gerenciamento de dispositivos.


  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: PreventSmartScreenPromptOverride
  - Nome da GP: Impedir que avisos do Microsoft Defender SmartScreen sejam ignorados para sites
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/Configurações do SmartScreen
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: PreventSmartScreenPromptOverride
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000001
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: PreventSmartScreenPromptOverride
  - Exemplo de valor:
``` xml
<true/>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### PreventSmartScreenPromptOverrideForFiles
  #### Impedir que os avisos do Microsoft Defender SmartScreen sobre downloads sejam ignorados
  >Versões com Suporte: O Microsoft Edge no Windows desde a versão 77 ou posterior e no Mac desde a versão 79 ou posterior

  #### Descrição
  Essa política permite determinar se os usuários podem substituir os avisos do Microsoft Defender SmartScreen sobre downloads não verificados.

Se você habilitar essa política, os usuários de sua organização não poderão ignorar os avisos do Microsoft Defender SmartScreen, e eles serão impedidos de concluir os downloads não verificados.

Se você desabilitar ou não configurar essa política, os usuários poderão ignorar os avisos do Microsoft Defender SmartScreen e concluir downloads não verificados.

Essa política está disponível somente em instâncias do Windows que fazem parte de um domínio do Microsoft Active Directory ou em instâncias do Windows 10 Pro ou Enterprise registradas para o gerenciamento de dispositivos.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: PreventSmartScreenPromptOverrideForFiles
  - Nome da GP: Impedir que os avisos do Microsoft Defender SmartScreen sobre downloads sejam ignorados
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/Configurações do SmartScreen
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: PreventSmartScreenPromptOverrideForFiles
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000001
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: PreventSmartScreenPromptOverrideForFiles
  - Exemplo de valor:
``` xml
<true/>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### SmartScreenAllowListDomains
  #### Configurar a lista de domínios para os quais o Microsoft Defender SmartScreen não disparará avisos
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Configure a lista de domínios confiáveis do Microsoft Defender SmartScreen. Isso significa que:
o Microsoft Defender SmartScreen não verificará recursos potencialmente mal-intencionados, como software de phishing e outro malware se as URLs de origem coincidirem com esses domínios.
O serviço de proteção contra download do Microsoft Defender SmartScreen não verificará os downloads hospedados nesses domínios.

Se você habilitar essa política, o Microsoft Defender SmartScreen confiará nesses domínios.
Se você desabilitar ou não configurar essa política, a proteção padrão do Microsoft Defender SmartScreen será aplicada a todos os recursos.

Essa política está disponível somente em instâncias do Windows que façam parte de um domínio do Microsoft Active Directory ou em instâncias do Windows 10 Pro ou Enterprise registradas para o gerenciamento de dispositivos.
Observe também que essa política não se aplica quando a organização habilita a Proteção Avançada contra Ameaças do Microsoft Defender. É necessário configurar suas listas de contatos bloqueados e permitidos na Central de Segurança do Microsoft Defender.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Lista de cadeias de caracteres

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: SmartScreenAllowListDomains
  - Nome da GP: Configurar a lista de domínios para os quais o Microsoft Defender SmartScreen não disparará avisos
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/Configurações do SmartScreen
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge\SmartScreenAllowListDomains
  - Caminho (Recomendações): N/A
  - Nome do Valor: 1, 2, 3, ...
  - Tipo de Valor: lista de REG_SZ
  ##### Exemplo de valor:
```
SOFTWARE\Policies\Microsoft\Edge\SmartScreenAllowListDomains\0 = "mydomain.com"
SOFTWARE\Policies\Microsoft\Edge\SmartScreenAllowListDomains\1 = "myuniversity.edu"

```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: SmartScreenAllowListDomains
  - Exemplo de valor:
``` xml
<array>
  <string>mydomain.com</string>
  <string>myuniversity.edu</string>
</array>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### SmartScreenEnabled
  #### Configurar o Microsoft Defender SmartScreen
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Essa configuração de política permite configurar a ativação do Microsoft Defender SmartScreen. O Microsoft Defender SmartScreen fornece mensagens de aviso para ajudar a proteger seus funcionários contra potenciais golpes de phishing e software mal-intencionado. Por padrão, o Microsoft Defender SmartScreen é ativado.

Se você habilitar essa configuração, o Microsoft Defender SmartScreen será ativado.

Se você desabilitar essa configuração, o Microsoft Defender SmartScreen será desativado.

Se você não definir essa configuração, os usuários poderão escolher se desejam usar o Microsoft Defender SmartScreen.

Esta política está disponível somente em instâncias do Windows que fazem parte de um domínio do Microsoft Active Directory ou em instâncias do Windows 10 Pro ou Enterprise registradas para o gerenciamento de dispositivos.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Sim
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: SmartScreenEnabled
  - Nome da GP: Configurar o Microsoft Defender SmartScreen
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/Configurações do SmartScreen
  - Caminho da GP (Recomendações): Modelos Administrativos/Microsoft Edge - Configurações Padrão (os usuários podem substituir)/Configurações do SmartScreen
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): SOFTWARE\Policies\Microsoft\Edge\Recomendações
  - Nome do Valor: SmartScreenEnabled
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000001
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: SmartScreenEnabled
  - Exemplo de valor:
``` xml
<true/>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### SmartScreenForTrustedDownloadsEnabled
  #### Forçar verificações do Microsoft Defender SmartScreen em downloads de fontes confiáveis
  >Versões com Suporte: O Microsoft Edge no Windows desde a versão 78 ou posterior

  #### Descrição
  Essa configuração de política permite definir se o Microsoft Defender SmartScreen verificará a reputação de download de uma fonte confiável.

Se você habilitar ou não definir essa configuração, o Microsoft Defender SmartScreen verificará a reputação do download, independentemente da fonte.

Se você desabilitar essa configuração, o Microsoft Defender SmartScreen não verificará a reputação do download ao baixar de uma fonte confiável.

Esta política está disponível somente em instâncias do Windows que façam parte de um domínio do Microsoft Active Directory ou em instâncias do Windows 10 Pro ou Enterprise registradas para o gerenciamento de dispositivos.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Sim
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: SmartScreenForTrustedDownloadsEnabled
  - Nome da GP: Forçar verificações do Microsoft Defender SmartScreen em downloads de fontes confiáveis
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/Configurações do SmartScreen
  - Caminho da GP (Recomendações): Modelos Administrativos/Microsoft Edge - Configurações Padrão (os usuários podem substituir)/Configurações do SmartScreen
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): SOFTWARE\Policies\Microsoft\Edge\Recomendações
  - Nome do Valor: SmartScreenForTrustedDownloadsEnabled
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000000
```


  

  [Voltar ao início](#microsoft-edge---políticas)

  ### SmartScreenPuaEnabled
  #### Configurar o Microsoft Defender SmartScreen para bloquear aplicativos potencialmente indesejados
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 80 ou posterior

  #### Descrição
  Essa configuração de política permite configurar a ativação do bloqueio de aplicativos potencialmente indesejados no Microsoft Defender SmartScreen. O bloqueio de aplicativos potencialmente indesejados no Microsoft Defender SmartScreen fornece mensagens de aviso para ajudar a proteger os usuários contra adware, mineradores de moeda, bundleware e outros aplicativos de baixa reputação que são hospedados por sites. O bloqueio de aplicativos potencialmente indesejados no Microsoft Defender SmartScreen é desativado por padrão.

Se você habilitar essa configuração, o bloqueio de aplicativos potencialmente indesejados no Microsoft Defender SmartScreen será ativado.

Se você desabilitar essa configuração, o bloqueio de aplicativos potencialmente indesejados no Microsoft Defender SmartScreen será desativado.

Se você não definir essa configuração, os usuários poderão escolher se desejam usar o bloqueio de aplicativos potencialmente indesejados no Microsoft Defender SmartScreen.

Essa política está disponível apenas em instâncias do Windows que fazem parte de um domínio do Microsoft Active Directory ou instâncias do Windows 10 Pro ou Enterprise registradas para o gerenciamento de dispositivos.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Sim
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: SmartScreenPuaEnabled
  - Nome da GP: Configurar o Microsoft Defender SmartScreen para bloquear aplicativos potencialmente indesejados
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/Configurações do SmartScreen
  - Caminho da GP (Recomendações): Modelos Administrativos/Microsoft Edge - Configurações Padrão (os usuários podem substituir)/Configurações do SmartScreen
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): SOFTWARE\Policies\Microsoft\Edge\Recomendações
  - Nome do Valor: SmartScreenPuaEnabled
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000001
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: SmartScreenPuaEnabled
  - Exemplo de valor:
``` xml
<true/>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ## Extensões policies

  [Voltar ao início](#microsoft-edge---políticas)

  ### ExtensionAllowedTypes
  #### Configurar tipos de extensão permitidos
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Controla quais tipos de extensão podem ser instalados e limita o acesso do tempo de execução.

Esta configuração define os tipos de extensão permitidos e com quais hosts eles podem interagir. O valor é uma lista de cadeias de caracteres, e cada uma delas deve ser uma das seguintes: "extension", "theme", "user_script" e "hosted_app". Consulte a documentação sobre extensões do Microsoft Edge para obter mais informações sobre esses tipos.

Observe que esta política também afeta as extensões a serem instaladas forçadamente pela política [ExtensionInstallForcelist](#extensioninstallforcelist).

Se você habilitar esta política, apenas as extensões que corresponderem a um tipo na lista serão instaladas.

Se você não configurar esta política, nenhuma restrição sobre os tipos de extensão aceitáveis será aplicada.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Lista de cadeias de caracteres

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: ExtensionAllowedTypes
  - Nome da GP: Configurar tipos de extensão permitidos
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/Extensões
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge\ExtensionAllowedTypes
  - Caminho (Recomendações): N/A
  - Nome do Valor: 1, 2, 3, ...
  - Tipo de Valor: lista de REG_SZ
  ##### Exemplo de valor:
```
SOFTWARE\Policies\Microsoft\Edge\ExtensionAllowedTypes\0 = "hosted_app"

```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: ExtensionAllowedTypes
  - Exemplo de valor:
``` xml
<array>
  <string>hosted_app</string>
</array>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### ExtensionInstallAllowlist
  #### Permitir que extensões específicas sejam instaladas
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Por padrão, todas as extensões são permitidas. No entanto, se você bloquear todas as extensões definindo a política 'ExtensionInstallBlockList' como "*", os usuários só poderão instalar as extensões definidas nesta política.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Lista de cadeias de caracteres

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: ExtensionInstallAllowlist
  - Nome da GP: Permitir que extensões específicas sejam instaladas
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/Extensões
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallAllowlist
  - Caminho (Recomendações): N/A
  - Nome do Valor: 1, 2, 3, ...
  - Tipo de Valor: lista de REG_SZ
  ##### Exemplo de valor:
```
SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallAllowlist\0 = "extension_id1"
SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallAllowlist\1 = "extension_id2"

```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: ExtensionInstallAllowlist
  - Exemplo de valor:
``` xml
<array>
  <string>extension_id1</string>
  <string>extension_id2</string>
</array>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### ExtensionInstallBlocklist
  #### Controlar quais extensões não podem ser instaladas
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Liste extensões específicas que os usuários NÃO podem instalar no Microsoft Edge. Quando você implanta essa política, todas as extensões nessa lista que foram instaladas anteriormente serão desabilitadas e o usuário não poderá habilitá-las. Se você remover um item da lista de extensões bloqueadas, essa extensão será reabilitada automaticamente em qualquer lugar onde tenha sido instalada anteriormente.

Use "*" para bloquear todas as extensões que não estão listadas explicitamente na lista de permissões.

Se você não configurar essa política, os usuários poderão instalar qualquer extensão no Microsoft Edge.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Lista de cadeias de caracteres

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: ExtensionInstallBlocklist
  - Nome da GP: Controlar quais extensões não podem ser instaladas
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/Extensões
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallBlocklist
  - Caminho (Recomendações): N/A
  - Nome do Valor: 1, 2, 3, ...
  - Tipo de Valor: lista de REG_SZ
  ##### Exemplo de valor:
```
SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallBlocklist\0 = "extension_id1"
SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallBlocklist\1 = "extension_id2"

```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: ExtensionInstallBlocklist
  - Exemplo de valor:
``` xml
<array>
  <string>extension_id1</string>
  <string>extension_id2</string>
</array>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### ExtensionInstallForcelist
  #### Controlar quais extensões são instaladas silenciosamente
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Especifica as extensões que são instaladas silenciosamente, sem interação do usuário e que os usuários não podem desinstalar ou desabilitar ("instalação forçada"). Todas as permissões solicitadas pelas extensões são concedidas implicitamente, sem interação do usuário, incluindo quaisquer permissões adicionais solicitadas pelas versões futuras da extensão. Além disso, as permissões são concedidas para as APIs da extensão enterprise.deviceAttributes e enterprise.platformKeys. (Essas duas APIs só estão disponíveis para extensões cuja instalação é forçada.)

Essa política tem precedência sobre uma política [ExtensionInstallBlocklist](#extensioninstallblocklist) potencialmente conflitante. Ao remover uma extensão da lista de instalação forçada, ela é desinstalada automaticamente pelo Microsoft Edge.

Para dispositivos Windows que não fazem parte de um domínio do Microsoft Active Directory, a instalação forçada está limitada às extensões disponíveis na Microsoft Store.

Observe que os usuários podem modificar o código-fonte de qualquer extensão usando as Ferramentas de Desenvolvedor, o que pode renderizar potencialmente a extensão a um estado não funcional. Se isso for um problema, configure a política [DeveloperToolsAvailability](#developertoolsavailability).

Use o formato a seguir para adicionar uma extensão à lista:

[extensionID];[updateURL]

- extensionID - a cadeia de caracteres de 32 letras encontrada em edge://extensions quando estiver no modo de desenvolvedor.

- updateURL (opcional) é o endereço do documento XML do Manifesto de Atualização para o aplicativo ou extensão, conforme descrito em [https://go.microsoft.com/fwlink/?linkid=2095043](https://go.microsoft.com/fwlink/?linkid=2095043). Se você não configurar updateURL, a URL de atualização da Microsoft Store será usada (atualmente https://edge.microsoft.com/extensionwebstorebase/v1/crx).  Observe que a URL de atualização configurada nessa política só é usada para a instalação inicial; atualizações subsequentes da extensão usam a URL de atualização indicada no manifesto da extensão.

Por exemplo, gggmmkjegpiggikcnhidnjjhmicpibll;https://edge.microsoft.com/extensionwebstorebase/v1/crx instala o aplicativo Microsoft Online direto da URL de "atualização" da Microsoft Store. Para obter mais informações sobre hospedagem de extensões, consulte: [https://go.microsoft.com/fwlink/?linkid=2095044](https://go.microsoft.com/fwlink/?linkid=2095044).

Se você não configurar essa política, nenhuma extensão será instalada automaticamente, e os usuários poderão desinstalar qualquer extensão no Microsoft Edge.

Observe que essa política não se aplica ao modo InPrivate.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Lista de cadeias de caracteres

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: ExtensionInstallForcelist
  - Nome da GP: Controlar quais extensões são instaladas silenciosamente
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/Extensões
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallForcelist
  - Caminho (Recomendações): N/A
  - Nome do Valor: 1, 2, 3, ...
  - Tipo de Valor: lista de REG_SZ
  ##### Exemplo de valor:
```
SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallForcelist\0 = "gbchcmhmhahfdphkhkmpfmihenigjmpp;https://edge.microsoft.com/extensionwebstorebase/v1/crx"
SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallForcelist\1 = "abcdefghijklmnopabcdefghijklmnop"

```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: ExtensionInstallForcelist
  - Exemplo de valor:
``` xml
<array>
  <string>gbchcmhmhahfdphkhkmpfmihenigjmpp;https://edge.microsoft.com/extensionwebstorebase/v1/crx</string>
  <string>abcdefghijklmnopabcdefghijklmnop</string>
</array>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### ExtensionInstallSources
  #### Configurar fontes de instalação de script de usuário e extensão
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Define URLs que podem instalar extensões e temas.

Por padrão, os usuários precisam baixar um arquivo *.crx para cada extensão ou script que desejam instalar e, em seguida, arrastá-lo para a página de configurações do Microsoft Edge. Esta política permite que URLs específicas instalem a extensão ou o script para o usuário.

Cada item da lista é um padrão de correspondência de estilo de extensão (consulte [https://go.microsoft.com/fwlink/?linkid=2095039](https://go.microsoft.com/fwlink/?linkid=2095039)). Os usuários poderão instalar facilmente itens de qualquer URL que corresponda a um item dessa lista. A localização do arquivo *.crx e a página a partir da qual o download é iniciado (ou seja, o referenciador) devem ser autorizadas por esses padrões.

A política [ExtensionInstallBlocklist](#extensioninstallblocklist) tem precedência sobre esta política. As extensões que estiverem na lista de contatos bloqueados não serão instaladas, mesmo que venham de um site dessa lista.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Lista de cadeias de caracteres

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: ExtensionInstallSources
  - Nome da GP: Configurar fontes de instalação de script de usuário e extensão
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/Extensões
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallSources
  - Caminho (Recomendações): N/A
  - Nome do Valor: 1, 2, 3, ...
  - Tipo de Valor: lista de REG_SZ
  ##### Exemplo de valor:
```
SOFTWARE\Policies\Microsoft\Edge\ExtensionInstallSources\0 = "https://corp.contoso.com/*"

```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: ExtensionInstallSources
  - Exemplo de valor:
``` xml
<array>
  <string>https://corp.contoso.com/*</string>
</array>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### ExtensionSettings
  #### Definir configurações de gerenciamento de extensões
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Define as configurações de gerenciamento de extensão para o Microsoft Edge.

Esta política controla várias configurações, incluindo as configurações controladas por quaisquer políticas existentes relacionadas a extensões. Esta política substituirá qualquer política herdada se ambas forem definidas.

Esta política mapeia uma ID de extensão ou uma URL de atualização para a configuração dela. Com uma ID de extensão, a configuração é aplicada somente à extensão especificada. Defina uma configuração padrão para a ID especial "*", para aplicar a todas as extensões que não forem especificamente listadas nesta política. Com uma URL de atualização, a configuração é aplicada a todas as extensões com a URL de atualização exata declarada no manifesto dessa extensão, conforme descrito em [https://go.microsoft.com/fwlink/?linkid=2095043](https://go.microsoft.com/fwlink/?linkid=2095043).

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Dicionário

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: ExtensionSettings
  - Nome da GP: Definir configurações de gerenciamento de extensões
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/Extensões
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: ExtensionSettings
  - Tipo de Valor: REG_SZ
  ##### Exemplo de valor:
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


  #### Informações e configurações do Mac
  - Nome da chave de preferência: ExtensionSettings
  - Exemplo de valor:
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
  

  [Voltar ao início](#microsoft-edge---políticas)

  ## Gerenciador de senhas e de proteção policies

  [Voltar ao início](#microsoft-edge---políticas)

  ### PasswordManagerEnabled
  #### Habilitar salvamento de senhas no gerenciador de senhas
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Habilite o Microsoft Edge para salvar as senhas dos usuários.

Se você habilitar essa política, os usuários poderão salvar suas senhas no Microsoft Edge. Na próxima visita que fizerem ao site, o Microsoft Edge inserirá a senha automaticamente.

Se você desabilitar essa política, os usuários não poderão salvar novas senhas, mas ainda poderão usar senhas salvas anteriormente.

Se você habilitar ou desabilitar essa política, os usuários não poderão alterá-la ou substituí-la no Microsoft Edge. Se você não configurá-la, os usuários poderão salvar senhas, além de desabilitar esse recurso.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Sim
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: PasswordManagerEnabled
  - Nome da GP: Habilitar salvamento de senhas no gerenciador de senhas
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/Gerenciador de senhas e de proteção
  - Caminho da GP (Recomendações): Modelos Administrativos/Microsoft Edge - Configurações Padrão (os usuários podem substituir)/Gerenciador de senhas e de proteção
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): SOFTWARE\Policies\Microsoft\Edge\Recomendações
  - Nome do Valor: PasswordManagerEnabled
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000001
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: PasswordManagerEnabled
  - Exemplo de valor:
``` xml
<true/>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### PasswordProtectionChangePasswordURL
  #### Configurar a URL de alteração de senha
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Configura a URL de alteração de senha (somente esquemas HTTP e HTTPS).

O serviço de proteção de senha enviará os usuários para essa URL para que alterem suas senhas depois de verem um aviso no navegador..

Se você habilitar essa política, o serviço de proteção de senha enviará os usuários para essa URL para que alterem suas senhas.

Se você desabilitar essa política ou não a configurar, o serviço de proteção de senha não redirecionará os usuários para uma URL de alteração de senha.

Essa política está disponível apenas em instâncias do Windows que façam parte de um domínio do Microsoft Active Directory ou instâncias do Windows 10 Pro ou Enterprise registradas para o gerenciamento de dispositivos.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Cadeia de Caracteres

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: PasswordProtectionChangePasswordURL
  - Nome da GP: Configurar a URL de alteração de senha
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/Gerenciador de senhas e de proteção
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: PasswordProtectionChangePasswordURL
  - Tipo de Valor: REG_SZ
  ##### Exemplo de valor:
```
"https://contoso.com/change_password.html"
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: PasswordProtectionChangePasswordURL
  - Exemplo de valor:
``` xml
<string>https://contoso.com/change_password.html</string>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### PasswordProtectionLoginURLs
  #### Configurar a lista de URLs de logon corporativo em que o serviço de proteção de senha deve capturar a impressão digital de senha
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Configura a lista de URLs de logon corporativo (somente esquemas HTTP e HTTPS) em que o Microsoft Edge deverá capturar a impressão digital de senhas e usá-la para detecção de reutilização de senha.

Se você habilitar essa política, o serviço de proteção de senha capturará as impressões digitais de senhas nas URLs definidas.

 Se você desabilitar essa política ou não a configurar, nenhuma impressão digital de senha será capturada.

 Essa política está disponível apenas em instâncias do Windows que façam parte de um domínio do Microsoft Active Directory ou instâncias do Windows 10 Pro ou Enterprise registradas para o gerenciamento de dispositivos.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Lista de cadeias de caracteres

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: PasswordProtectionLoginURLs
  - Nome da GP: Configurar a lista de URLs de logon corporativo em que o serviço de proteção de senha deve capturar a impressão digital de senha
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/Gerenciador de senhas e de proteção
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge\PasswordProtectionLoginURLs
  - Caminho (Recomendações): N/A
  - Nome do Valor: 1, 2, 3, ...
  - Tipo de Valor: lista de REG_SZ
  ##### Exemplo de valor:
```
SOFTWARE\Policies\Microsoft\Edge\PasswordProtectionLoginURLs\0 = "https://contoso.com/login.html"
SOFTWARE\Policies\Microsoft\Edge\PasswordProtectionLoginURLs\1 = "https://login.contoso.com"

```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: PasswordProtectionLoginURLs
  - Exemplo de valor:
``` xml
<array>
  <string>https://contoso.com/login.html</string>
  <string>https://login.contoso.com</string>
</array>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### PasswordProtectionWarningTrigger
  #### Configurar gatilho de aviso de proteção de senha
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Permite que você controle quando disparar o aviso de proteção de senha. A proteção de senha alerta os usuários quando eles reutilizam a senha protegida em sites potencialmente suspeitos.

Você pode usar as políticas [PasswordProtectionLoginURLs](#passwordprotectionloginurls) e [PasswordProtectionChangePasswordURL](#passwordprotectionchangepasswordurl) para configurar quais senhas serão protegidas.

Isenções: as senhas para os sites listados em [PasswordProtectionLoginURLs](#passwordprotectionloginurls) e [PasswordProtectionChangePasswordURL](#passwordprotectionchangepasswordurl), bem como para os sites listados em [SmartScreenAllowListDomains](#smartscreenallowlistdomains), não vão disparar um aviso de proteção de senha.

Defina como "PasswordProtectionWarningOff" (0) para não mostrar avisos de proteção de senha.

Defina como "PasswordProtectionWarningOnPasswordReuse" (1) para mostrar avisos de proteção de senha quando o usuário reutilizar sua senha protegida em um site não incluído na lista de permissões.

Se você desabilitar ou não configurar esta política, o gatilho de aviso não será mostrado.

* 0 = O aviso de proteção de senha é desativado.

* 1 = O aviso de proteção de senha é disparado pela reutilização da senha.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Número inteiro

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: PasswordProtectionWarningTrigger
  - Nome da GP: Configurar gatilho de aviso de proteção de senha
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/Gerenciador de senhas e de proteção
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: PasswordProtectionWarningTrigger
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000001
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: PasswordProtectionWarningTrigger
  - Exemplo de valor:
``` xml
<integer>1</integer>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ## Impressão policies

  [Voltar ao início](#microsoft-edge---políticas)

  ### DefaultPrinterSelection
  #### Regras de seleção de impressora padrão
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Substitui as regras de seleção de impressora padrão do Microsoft Edge. Essa política determina as regras para selecionar a impressora padrão no Microsoft Edge, o que acontece na primeira vez que um usuário tenta imprimir uma página.

Quando essa política é definida, o Microsoft Edge tenta encontrar uma impressora que corresponda a todos os atributos especificados, usando-a como impressora padrão. Se houver várias impressoras que atendem aos critérios, a primeira impressora correspondente será usada.

Se você não configurar essa política ou nenhuma impressora correspondente for encontrada dentro do tempo limite, a impressora usará como padrão a impressora PDF integrada ou nenhuma impressora, se a impressora PDF não estiver disponível.

O valor é analisado como um objeto JSON, em conformidade com o seguinte esquema: { "type": "object", "properties": { "idPattern": { "description": "Regular expression to match printer id.", "type": "string" }, "namePattern": { "description": "Regular expression to match printer display name.", "type": "string" } } }

A omissão de um campo significa que todos os valores são correspondentes; por exemplo, se você não especificar a conectividade, Visualizar Impressão começará a descobrir todos os tipos de impressoras locais. Os padrões de expressões regulares devem seguir a sintaxe JavaScript RegExp e as correspondências diferenciam maiúsculas de minúsculas.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Cadeia de Caracteres

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: DefaultPrinterSelection
  - Nome da GP: Regras de seleção de impressora padrão
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/Impressão
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: DefaultPrinterSelection
  - Tipo de Valor: REG_SZ
  ##### Exemplo de valor:
```
"{ "idPattern": ".*public", "namePattern": ".*Color" }"
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: DefaultPrinterSelection
  - Exemplo de valor:
``` xml
<string>{ "idPattern": ".*public", "namePattern": ".*Color" }</string>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### PrintHeaderFooter
  #### Imprimir cabeçalhos e rodapés
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Aplique os cabeçalhos e rodapés para que sejam ativados ou desativados no diálogo de impressão.

Se você não configurar essa política, os usuários poderão decidir se serão impressos cabeçalhos e rodapés.

Se você desabilitar essa política, os usuários não poderão imprimir cabeçalhos e rodapés.

Se você habilitar essa política, os usuários sempre imprimirão cabeçalhos e rodapés.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Sim
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: PrintHeaderFooter
  - Nome da GP: Imprimir cabeçalhos e rodapés
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/Impressão
  - Caminho da GP (Recomendações): Modelos Administrativos/Microsoft Edge - Configurações Padrão (os usuários podem substituir)/Impressão
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): SOFTWARE\Policies\Microsoft\Edge\Recomendações
  - Nome do Valor: PrintHeaderFooter
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000000
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: PrintHeaderFooter
  - Exemplo de valor:
``` xml
<false/>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### PrintPreviewUseSystemDefaultPrinter
  #### Definir a impressora padrão do sistema como a impressora padrão
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Informa ao Microsoft Edge para usar a impressora padrão do sistema como a opção padrão na Visualização de Impressão, em vez da impressora usada recentemente.

Se você desabilitar essa política ou não configurá-la, a Visualização de Impressão usará a impressora usada mais recentemente como a opção de destino padrão.

Se você habilitar essa política, a Visualização de Impressão usará a impressora padrão do sistema operacional como a opção de destino padrão.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Sim
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: PrintPreviewUseSystemDefaultPrinter
  - Nome da GP: Definir a impressora padrão do sistema como a impressora padrão
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/Impressão
  - Caminho da GP (Recomendações): Modelos Administrativos/Microsoft Edge - Configurações Padrão (os usuários podem substituir)/Impressão
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): SOFTWARE\Policies\Microsoft\Edge\Recomendações
  - Nome do Valor: PrintPreviewUseSystemDefaultPrinter
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000000
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: PrintPreviewUseSystemDefaultPrinter
  - Exemplo de valor:
``` xml
<false/>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### PrintingEnabled
  #### Habilitar impressão
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Habilita a impressão no Microsoft Edge e impede que os usuários alterem essa configuração.

Se você habilitar essa política ou não configurá-la, os usuários poderão imprimir.

Se você desabilitar essa política, os usuários não poderão imprimir usando o Microsoft Edge. A impressão está desabilitada no menu de ferramentas, extensões, aplicativos JavaScript e assim por diante. Os usuários ainda podem imprimir usando plug-ins que ignoram o Microsoft Edge durante a impressão. Por exemplo, alguns aplicativos Adobe Flash têm a opção de impressão em seu menu de contexto, o que não é coberto por essa política.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: PrintingEnabled
  - Nome da GP: Habilitar impressão
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/Impressão
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: PrintingEnabled
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000001
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: PrintingEnabled
  - Exemplo de valor:
``` xml
<true/>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### UseSystemPrintDialog
  #### Imprimir usando a caixa de diálogo de impressão do sistema
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Mostra a caixa de diálogo de impressão do sistema, em vez da visualização de impressão.

Se você habilitar essa política, o Microsoft Edge abrirá a caixa de diálogo de impressão do sistema, em vez da visualização de impressão interna quando o usuário imprimir uma página.

Se você não configurar ou desabilitar essa política, os comandos de impressão acionarão a tela de visualização de impressão do Microsoft Edge.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Não - Requer a reinicialização do navegador

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: UseSystemPrintDialog
  - Nome da GP: Imprimir usando a caixa de diálogo de impressão do sistema
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/Impressão
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: UseSystemPrintDialog
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000000
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: UseSystemPrintDialog
  - Exemplo de valor:
``` xml
<false/>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ## Inicialização&comma; página inicial e página nova guia policies

  [Voltar ao início](#microsoft-edge---políticas)

  ### HomepageIsNewTabPage
  #### Definir a página nova guia como a home page
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Configura a home page padrão no Microsoft Edge. Você pode definir a home page como uma URL que você especificar ou como a página de nova guia.

Se você habilitar esta política, a página de nova guia será sempre usada para a home page, e a localização da URL da home page será ignorada.

Se você desabilitar esta política, a home page do usuário não poderá ser a página de nova guia, a menos que a URL seja definida como "edge://newtab".

Se ela não for configurada, os usuários poderão escolher se a página de nova guia é a sua home page.

Esta política está disponível apenas em instâncias do Windows que façam parte de um domínio do Microsoft Active Directory ou instâncias do Windows 10 Pro ou Enterprise registradas para o gerenciamento de dispositivos.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Sim
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: HomepageIsNewTabPage
  - Nome da GP: Definir a página nova guia como a home page
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/Inicialização, página inicial e página nova guia
  - Caminho da GP (Recomendações): Modelos Administrativos/Microsoft Edge - Configurações Padrão (os usuários podem substituir)/Inicialização, página inicial e página nova guia
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): SOFTWARE\Policies\Microsoft\Edge\Recomendações
  - Nome do Valor: HomepageIsNewTabPage
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000001
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: HomepageIsNewTabPage
  - Exemplo de valor:
``` xml
<true/>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### HomepageLocation
  #### Configurar a URL da home page
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Configura a URL da home page padrão no Microsoft Edge.

A home page é a página aberta pelo botão Início. As páginas abertas na inicialização são controladas pelas políticas [RestoreOnStartup](#restoreonstartup).

Você pode definir uma URL aqui ou definir a home page para abrir a página de nova guia. Se você optar por abrir a página de nova guia, essa política não terá efeito.

Se você habilitar essa política, os usuários não poderão alterar a URL da home page, mas poderão optar por usar a página nova guia como home page.

Se você desabilitar ou não configurar essa política, os usuários poderão escolher sua própria home page, desde que a política [HomepageIsNewTabPage](#homepageisnewtabpage) não esteja habilitada.

Esta política está disponível somente em instâncias do Windows que fazem parte de um domínio do Microsoft Active Directory ou em instâncias do Windows 10 Pro ou Enterprise registradas para o gerenciamento de dispositivos.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Sim
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Cadeia de Caracteres

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: HomepageLocation
  - Nome da GP: Configurar a URL da home page
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/Inicialização, página inicial e página nova guia
  - Caminho da GP (Recomendações): Modelos Administrativos/Microsoft Edge - Configurações Padrão (os usuários podem substituir)/Inicialização, página inicial e página nova guia
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): SOFTWARE\Policies\Microsoft\Edge\Recomendações
  - Nome do Valor: HomepageLocation
  - Tipo de Valor: REG_SZ
  ##### Exemplo de valor:
```
"https://www.contoso.com"
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: HomepageLocation
  - Exemplo de valor:
``` xml
<string>https://www.contoso.com</string>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### NewTabPageCompanyLogo
  #### Definir o logotipo da empresa da página Nova guia
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 79 ou posterior

  #### Descrição
  Especifica o logotipo da empresa a ser usado na página de nova guia no Microsoft Edge.

A política deve ser configurada como uma cadeia de caracteres que expressa o logotipo em formato JSON. Por exemplo: { "default_logo": { "url": "https://www.contoso.com/logo.png", "hash": "cd0aa9856147b6c5b4ff2b7dfee5da20aa38253099ef1b4a64aced233c9afe29" }, "light_logo": { "url": "https://www.contoso.com/light_logo.png", "hash": "517d286edb416bb2625ccfcba9de78296e90da8e32330d4c9c8275c4c1c33737" } }

Configure essa política especificando a URL da qual o Microsoft Edge pode baixar o logotipo e seu hash criptográfico (SHA-256), que é usado para verificar a integridade do download. O logotipo deve estar em formato PNG ou SVG, e seu tamanho de arquivo não deve exceder 16 MB. O logotipo é baixado e armazenado em cache, e o download será repetido sempre que a URL ou o hash mudar. A URL deve ser acessível sem qualquer autenticação.

O 'default_logo' é obrigatório e será usado quando não houver imagem de fundo. Se o "light_logo" for fornecido, ele será usado quando a página de nova guia do usuário tiver uma imagem de fundo. Recomendamos um logotipo horizontal com um fundo transparente que seja alinhado à esquerda e centralizado verticalmente. O logotipo deve ter uma altura mínima de 32 pixels e uma taxa de proporção de 1:1 a 4:1. O "default_logo" deve ter um contraste adequado contra um fundo branco/preto, enquanto o "light_logo" deve ter um contraste adequado contra uma imagem de fundo.

Se você habilitar essa política, o Microsoft Edge baixará e mostrará os logotipos especificados na página de nova guia. Os usuários não podem substituir ou ocultar os logotipos.

Se você desabilitar ou não configurar essa política, o Microsoft Edge não mostrará o logotipo da empresa ou um logotipo da Microsoft na página de nova guia.

Para obter ajuda na determinação do hash SHA-256, consulte https://docs.microsoft.com/powershell/module/microsoft.powershell.utility/get-filehash.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Não - Requer a reinicialização do navegador

  #### Tipo de Dados:
  Dicionário

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: NewTabPageCompanyLogo
  - Nome da GP: Definir o logotipo da empresa da página Nova guia
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/Inicialização, página inicial e página nova guia
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: NewTabPageCompanyLogo
  - Tipo de Valor: REG_SZ
  ##### Exemplo de valor:
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


  #### Informações e configurações do Mac
  - Nome da chave de preferência: NewTabPageCompanyLogo
  - Exemplo de valor:
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
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### NewTabPageHideDefaultTopSites
  #### Ocultar os sites principais padrão da página de nova guia
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Oculta os sites principais padrão da página de nova guia no Microsoft Edge.

Se você definir essa política como true, os blocos do site principal padrão serão ocultos.

Se você definir essa política como false ou não configurá-la, os blocos dos sites principais padrão permanecerão visíveis.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: NewTabPageHideDefaultTopSites
  - Nome da GP: Ocultar os sites principais padrão da página de nova guia
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/Inicialização, página inicial e página nova guia
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: NewTabPageHideDefaultTopSites
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000001
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: NewTabPageHideDefaultTopSites
  - Exemplo de valor:
``` xml
<true/>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### NewTabPageLocation
  #### Configurar a URL da página de nova guia
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Configura a URL padrão para a página de nova guia.

Essa política determina a página que é aberta quando novas guias são criadas (incluindo quando novas janelas são abertas). Também afeta a página de inicialização se configurada para ser aberta na página de nova guia.

Essa política não determina qual página é aberta na inicialização. Isso é controlado pela política [RestoreOnStartup](#restoreonstartup). Também não afeta a home page se configurada para ser aberta na página de nova guia.

Se essa política não for configurada, a página de nova guia padrão será usada.

Se você configurar essa política *e* a política [NewTabPageSetFeedType](#newtabpagesetfeedtype), essa política terá prioridade.

Se uma URL inválida for fornecida, as novas guias abrirão about://blank.

Essa política está disponível somente em instâncias do Windows que fazem parte de um domínio do Microsoft Active Directory ou em instâncias do Windows 10 Pro ou Enterprise registradas para o gerenciamento de dispositivos.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Sim
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Cadeia de Caracteres

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: NewTabPageLocation
  - Nome da GP: Configurar a URL da página de nova guia
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/Inicialização, página inicial e página nova guia
  - Caminho da GP (Recomendações): Modelos Administrativos/Microsoft Edge - Configurações Padrão (os usuários podem substituir)/Inicialização, página inicial e página nova guia
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): SOFTWARE\Policies\Microsoft\Edge\Recomendações
  - Nome do Valor: NewTabPageLocation
  - Tipo de Valor: REG_SZ
  ##### Exemplo de valor:
```
"https://www.fabrikam.com"
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: NewTabPageLocation
  - Exemplo de valor:
``` xml
<string>https://www.fabrikam.com</string>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### NewTabPageManagedQuickLinks
  #### Definir links rápidos da página de nova guia
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 79 ou posterior

  #### Descrição
  Por padrão, o Microsoft Edge exibe links rápidos na página de nova guia de atalhos adicionados pelo usuário e sites principais com base no histórico de navegação. Com essa política, você pode configurar até três blocos de links rápidos na página da nova guia, expressos como um objeto JSON:

[ { "url": "https://www.contoso.com", "title": "Contoso Portal", "pinned": true/false }, ... ]

O campo 'url' é obrigatório; 'title' e 'pinned' são opcionais. Se 'title' não for preenchido, a URL será usada como o título padrão. Se 'pinned' não for preenchido, o valor padrão será false.

O Microsoft Edge apresenta esses itens na ordem listada, da esquerda para a direita, com todos os blocos fixados exibidos à frente dos blocos não fixados.

Se a política estiver definida como obrigatória, o campo 'pinned' será ignorado e todos os blocos serão fixados. Os blocos não poderão ser excluídos pelo usuário e sempre serão exibidos na frente da lista de links rápidos.

Se a política estiver definida como recomendada, os blocos fixados permanecerão na lista, mas o usuário poderá editá-los e excluí-los. Os blocos de links rápidos não fixados se comportam como sites principais padrão e são retirados da lista quando outros sites são visitados com mais frequência. Ao aplicar links não fixados por essa política a um perfil de navegador existente, os links podem não aparecer, dependendo de como são classificados em comparação ao histórico de navegação do usuário.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Sim
  - Atualização de política dinâmica: Não - Requer a reinicialização do navegador

  #### Tipo de Dados:
  Dicionário

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: NewTabPageManagedQuickLinks
  - Nome da GP: Definir links rápidos da página de nova guia
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/Inicialização, página inicial e página nova guia
  - Caminho da GP (Recomendações): Modelos Administrativos/Microsoft Edge - Configurações Padrão (os usuários podem substituir)/Inicialização, página inicial e página nova guia
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): SOFTWARE\Policies\Microsoft\Edge\Recomendações
  - Nome do Valor: NewTabPageManagedQuickLinks
  - Tipo de Valor: REG_SZ
  ##### Exemplo de valor:
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


  #### Informações e configurações do Mac
  - Nome da chave de preferência: NewTabPageManagedQuickLinks
  - Exemplo de valor:
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
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### NewTabPageSetFeedType
  #### Configurar a experiência de página de nova guia do Microsoft Edge
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 79 ou posterior

  #### Descrição
  Permite escolher a experiência de feed do Microsoft News ou do Office 365 para a página de nova guia.

Quando você definir essa política como a experiência de feed do Microsoft News (0), os usuários verão a experiência de feed do Microsoft News na página de nova guia.

Quando você definir essa política como a experiência de feed do Office 365 (1), os usuários com uma entrada do navegador do Azure Active Directory verão a experiência de feed do Office 365 na página de nova guia.

Se você desabilitar ou não configurar essa política:

- Os usuários com uma entrada do navegador do Azure Active Directory serão oferecidos a experiência de feed de página de nova guia do Office 365, bem como a experiência padrão de feed de página de nova guia.

- Os usuários sem uma entrada do navegador do Azure Active Directory verão a experiência padrão de página de nova guia.

Se você configurar essa política *e* a política [NewTabPageLocation](#newtabpagelocation), [NewTabPageLocation](#newtabpagelocation) terá prioridade.

Configuração padrão: desabilitada ou não configurada.\.

* 0 = experiência de feed do Microsoft News

* 1 = experiência de feed do Office 365

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Sim
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Número inteiro

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: NewTabPageSetFeedType
  - Nome da GP: Configurar a experiência de página de nova guia do Microsoft Edge
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/Inicialização, página inicial e página nova guia
  - Caminho da GP (Recomendações): Modelos Administrativos/Microsoft Edge - Configurações Padrão (os usuários podem substituir)/Inicialização, página inicial e página nova guia
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): SOFTWARE\Policies\Microsoft\Edge\Recomendações
  - Nome do Valor: NewTabPageSetFeedType
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000000
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: NewTabPageSetFeedType
  - Exemplo de valor:
``` xml
<integer>0</integer>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### RestoreOnStartup
  #### Ação a ser executada na inicialização
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Especifique como o Microsoft Edge se comporta quando ele é iniciado.

Se você quiser que uma nova guia sempre abra na inicialização, escolha "Abrir nova guia" (5).

Se você quiser reabrir URLs que estavam abertas na última vez em o Microsoft Edge foi fechado, escolha "Restaurar a última sessão" (1). A sessão de navegação será restaurada como estava. Observe que essa opção desativa algumas configurações que dependem de sessões ou que executam ações na saída (como Limpar dados de navegação ao sair ou cookies somente da sessão somente).

Se você deseja abrir um conjunto específico de URLs, escolha "Abrir uma lista de URLs" (4).

Desabilitar essa configuração é equivalente a deixá-la não configurada. Os usuários poderão alterá-la no Microsoft Edge.

Essa política está disponível apenas em instâncias do Windows que façam parte de um domínio do Microsoft Active Directory ou Windows 10 Pro ou Enterprise registradas para o gerenciamento de dispositivos.

* 5 = Abrir nova guia

* 1 = Restaurar a última sessão

* 4 = Abrir uma lista de URLs

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Sim
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Número inteiro

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: RestoreOnStartup
  - Nome da GP: Ação a ser executada na inicialização
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/Inicialização, página inicial e página nova guia
  - Caminho da GP (Recomendações): Modelos Administrativos/Microsoft Edge - Configurações Padrão (os usuários podem substituir)/Inicialização, página inicial e página nova guia
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): SOFTWARE\Policies\Microsoft\Edge\Recomendações
  - Nome do Valor: RestoreOnStartup
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000004
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: RestoreOnStartup
  - Exemplo de valor:
``` xml
<integer>4</integer>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### RestoreOnStartupURLs
  #### Sites a serem abertos quando o navegador for iniciado
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Especifica uma lista de sites para abrir automaticamente quando o navegador for iniciado. Se você não configurar essa política, nenhum site será aberto na inicialização.

Essa política só funciona se você também configurar a política [RestoreOnStartup](#restoreonstartup) como "Abrir uma lista de URLs" (4).

Essa política só está disponível em instâncias do Windows que fazem parte de um domínio do Microsoft Active Directory ou em instâncias do Windows 10 Pro ou Enterprise registradas para o gerenciamento de dispositivos.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Sim
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Lista de cadeias de caracteres

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: RestoreOnStartupURLs
  - Nome da GP: Sites a serem abertos quando o navegador for iniciado
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/Inicialização, página inicial e página nova guia
  - Caminho da GP (Recomendações): Modelos Administrativos/Microsoft Edge - Configurações Padrão (os usuários podem substituir)/Inicialização, página inicial e página nova guia
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge\RestoreOnStartupURLs
  - Caminho (Recomendações): SOFTWARE\Policies\Microsoft\Edge\Recomendações\RestoreOnStartupURLs
  - Nome do Valor: 1, 2, 3, ...
  - Tipo de Valor: lista de REG_SZ
  ##### Exemplo de valor:
```
SOFTWARE\Policies\Microsoft\Edge\RestoreOnStartupURLs\0 = "https://contoso.com"
SOFTWARE\Policies\Microsoft\Edge\RestoreOnStartupURLs\1 = "https://www.fabrikam.com"

```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: RestoreOnStartupURLs
  - Exemplo de valor:
``` xml
<array>
  <string>https://contoso.com</string>
  <string>https://www.fabrikam.com</string>
</array>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### ShowHomeButton
  #### Mostrar botão Início na barra de ferramentas
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Mostra o botão Início na barra de ferramentas do Microsoft Edge.

Habilite esta política para sempre mostrar o botão Início. Desabilite-a para nunca mostrar o botão.

Se você não configurar a política, os usuários poderão optar por mostrar o botão Início.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Sim
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: ShowHomeButton
  - Nome da GP: Mostrar botão Início na barra de ferramentas
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/Inicialização, página inicial e página nova guia
  - Caminho da GP (Recomendações): Modelos Administrativos/Microsoft Edge - Configurações Padrão (os usuários podem substituir)/Inicialização, página inicial e página nova guia
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): SOFTWARE\Policies\Microsoft\Edge\Recomendações
  - Nome do Valor: ShowHomeButton
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000001
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: ShowHomeButton
  - Exemplo de valor:
``` xml
<true/>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ## Mensagens nativas policies

  [Voltar ao início](#microsoft-edge---políticas)

  ### NativeMessagingAllowlist
  #### Controlar quais hosts de mensagens nativas os usuários podem usar
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Liste os hosts de mensagens nativas específicos que os usuários podem usar no Microsoft Edge.

Por padrão, todos os hosts de mensagens nativas são permitidos. Se você definir a política [NativeMessagingBlocklist](#nativemessagingblocklist) como *, todos os hosts de mensagens nativas serão bloqueados, e somente hosts de mensagens nativos listados aqui serão carregados.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Lista de cadeias de caracteres

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: NativeMessagingAllowlist
  - Nome da GP: Controlar quais hosts de mensagens nativas os usuários podem usar
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/Mensagens nativas
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge\NativeMessagingAllowlist
  - Caminho (Recomendações): N/A
  - Nome do Valor: 1, 2, 3, ...
  - Tipo de Valor: lista de REG_SZ
  ##### Exemplo de valor:
```
SOFTWARE\Policies\Microsoft\Edge\NativeMessagingAllowlist\0 = "com.native.messaging.host.name1"
SOFTWARE\Policies\Microsoft\Edge\NativeMessagingAllowlist\1 = "com.native.messaging.host.name2"

```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: NativeMessagingAllowlist
  - Exemplo de valor:
``` xml
<array>
  <string>com.native.messaging.host.name1</string>
  <string>com.native.messaging.host.name2</string>
</array>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### NativeMessagingBlocklist
  #### Configurar lista de contatos bloqueados de mensagens nativas
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Especifica quais hosts de mensagens nativas não devem ser usados.

Use "*" para bloquear todos os hosts de mensagens nativas, a menos que estejam explicitamente listados na lista de permissões.

Se você não configurar essa política, o Microsoft Edge carregará todos os hosts de mensagens nativas instalados.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Lista de cadeias de caracteres

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: NativeMessagingBlocklist
  - Nome da GP: Configurar lista de contatos bloqueados de mensagens nativas
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/Mensagens nativas
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge\NativeMessagingBlocklist
  - Caminho (Recomendações): N/A
  - Nome do Valor: 1, 2, 3, ...
  - Tipo de Valor: lista de REG_SZ
  ##### Exemplo de valor:
```
SOFTWARE\Policies\Microsoft\Edge\NativeMessagingBlocklist\0 = "com.native.messaging.host.name1"
SOFTWARE\Policies\Microsoft\Edge\NativeMessagingBlocklist\1 = "com.native.messaging.host.name2"

```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: NativeMessagingBlocklist
  - Exemplo de valor:
``` xml
<array>
  <string>com.native.messaging.host.name1</string>
  <string>com.native.messaging.host.name2</string>
</array>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### NativeMessagingUserLevelHosts
  #### Permitir hosts de mensagens nativas no nível de usuário (instalado sem permissões de administrador)
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Permite a instalação em nível de usuário de hosts de mensagens nativas.

Se você desabilitar essa política, o Microsoft Edge usará somente hosts de mensagens nativas instalados no nível do sistema.

Por padrão, se você não configurar essa política, o Microsoft Edge permitirá o uso de hosts de mensagens nativas no nível de usuário.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: NativeMessagingUserLevelHosts
  - Nome da GP: Permitir hosts de mensagens nativas no nível de usuário (instalado sem permissões de administrador)
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/Mensagens nativas
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: NativeMessagingUserLevelHosts
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000000
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: NativeMessagingUserLevelHosts
  - Exemplo de valor:
``` xml
<false/>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ## Provedor de pesquisa padrão policies

  [Voltar ao início](#microsoft-edge---políticas)

  ### DefaultSearchProviderEnabled
  #### Habilitar o provedor de pesquisa padrão
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Permite o uso de um provedor de pesquisa padrão.

Se você habilitar essa política, um usuário poderá pesquisar um termo digitando na barra de endereço (desde que o que ele digite não seja uma URL).

Você pode especificar o provedor de pesquisa padrão a ser usado, habilitando o restante das políticas de pesquisa padrão. Se estas forem deixadas vazias (não configuradas), o usuário poderá escolher o provedor padrão.

Se você desabilitar essa política, o usuário não poderá pesquisar na barra de endereço.

Se você habilitar ou desabilitar essa política, os usuários não poderão alterá-la ou substituí-la.

Se você não configurar essa política, o provedor de pesquisa padrão será habilitado e o usuário poderá escolher o provedor de pesquisa padrão e definir a lista de provedores de pesquisa.

Essa política está disponível apenas em instâncias do Windows que ingressaram em um domínio do Microsoft Active Directory ou em instâncias do Windows 10 Pro ou Enterprise registradas para o gerenciamento de dispositivos.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: DefaultSearchProviderEnabled
  - Nome da GP: Habilitar o provedor de pesquisa padrão
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/Provedor de pesquisa padrão
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: DefaultSearchProviderEnabled
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000001
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: DefaultSearchProviderEnabled
  - Exemplo de valor:
``` xml
<true/>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### DefaultSearchProviderEncodings
  #### Codificações do provedor de pesquisa padrão
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Especifica as codificações de caracteres com suporte pelo provedor de pesquisa. Codificações são nomes de página de código como UTF-8, GB2312 e ISO-8859-1. Eles serão experimentados na ordem fornecida.

Essa política é opcional. Se não estiver configurada, o padrão, UTF-8, será usado.

Essa política é aplicada somente quando você habilita as políticas [DefaultSearchProviderEnabled](#defaultsearchproviderenabled) e [DefaultSearchProviderSearchURL](#defaultsearchprovidersearchurl).

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Lista de cadeias de caracteres

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: DefaultSearchProviderEncodings
  - Nome da GP: Codificações do provedor de pesquisa padrão
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/Provedor de pesquisa padrão
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge\DefaultSearchProviderEncodings
  - Caminho (Recomendações): N/A
  - Nome do Valor: 1, 2, 3, ...
  - Tipo de Valor: lista de REG_SZ
  ##### Exemplo de valor:
```
SOFTWARE\Policies\Microsoft\Edge\DefaultSearchProviderEncodings\0 = "UTF-8"
SOFTWARE\Policies\Microsoft\Edge\DefaultSearchProviderEncodings\1 = "UTF-16"
SOFTWARE\Policies\Microsoft\Edge\DefaultSearchProviderEncodings\2 = "GB2312"
SOFTWARE\Policies\Microsoft\Edge\DefaultSearchProviderEncodings\3 = "ISO-8859-1"

```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: DefaultSearchProviderEncodings
  - Exemplo de valor:
``` xml
<array>
  <string>UTF-8</string>
  <string>UTF-16</string>
  <string>GB2312</string>
  <string>ISO-8859-1</string>
</array>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### DefaultSearchProviderImageURL
  #### Especifica o recurso de pesquisa por imagem para o provedor de pesquisa padrão
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Especifica a URL para o mecanismo de pesquisa usado na pesquisa de imagem. As solicitações de pesquisa são enviadas pelo método GET.

Essa política é opcional. Se você não configurá-la, a pesquisa de imagem não estará disponível.

Especifique a URL de Pesquisa de Imagem do Bing como:
"{bing:baseURL}images/detail/search?iss=sbiupload&FORM=ANCMS1#enterInsights".

Especifique a URL de Pesquisa de Imagem do Google: "{google:baseURL}searchbyimage/upload".

Consulte a política [DefaultSearchProviderImageURLPostParams](#defaultsearchproviderimageurlpostparams) para concluir a configuração da pesquisa de imagem.

Essa política é aplicada somente ao habilitar as políticas [DefaultSearchProviderEnabled](#defaultsearchproviderenabled) e [DefaultSearchProviderSearchURL](#defaultsearchprovidersearchurl).

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Cadeia de Caracteres

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: DefaultSearchProviderImageURL
  - Nome da GP: Especifica o recurso de pesquisa por imagem para o provedor de pesquisa padrão
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/Provedor de pesquisa padrão
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: DefaultSearchProviderImageURL
  - Tipo de Valor: REG_SZ
  ##### Exemplo de valor:
```
"https://search.contoso.com/searchbyimage/upload"
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: DefaultSearchProviderImageURL
  - Exemplo de valor:
``` xml
<string>https://search.contoso.com/searchbyimage/upload</string>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### DefaultSearchProviderImageURLPostParams
  #### Parâmetros para uma URL de imagem que usa POST
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Se você habilitar essa política, ela especificará os parâmetros usados quando uma pesquisa de imagem que usa POST for realizada. A política consiste em partes de nome/valor separados por vírgula. Se um valor for um parâmetro de modelo, como {imageThumbnail} no exemplo anterior, ele será substituído por dados reais de miniatura da imagem. Essa política é aplicada somente ao habilitar as políticas [DefaultSearchProviderEnabled](#defaultsearchproviderenabled) e [DefaultSearchProviderSearchURL](#defaultsearchprovidersearchurl).

Especifique os Parâmetros POST da URL de Pesquisa de Imagem do Bing como:
"imageBin={google:imageThumbnailBase64}".

Especifique os Parâmetros POST da URL de Pesquisa de Imagem do Google como:
"encoded_image={google:imageThumbnail},image_url={google:imageURL},sbisrc={google:imageSearchSource},original_width={google:imageOriginalWidth},original_height={google:imageOriginalHeight}".

Se você não configurar essa política, as solicitações de pesquisa de imagem serão enviadas pelo método GET.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Cadeia de Caracteres

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: DefaultSearchProviderImageURLPostParams
  - Nome da GP: Parâmetros para uma URL de imagem que usa POST
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/Provedor de pesquisa padrão
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: DefaultSearchProviderImageURLPostParams
  - Tipo de Valor: REG_SZ
  ##### Exemplo de valor:
```
"content={imageThumbnail},url={imageURL},sbisrc={SearchSource}"
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: DefaultSearchProviderImageURLPostParams
  - Exemplo de valor:
``` xml
<string>content={imageThumbnail},url={imageURL},sbisrc={SearchSource}</string>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### DefaultSearchProviderKeyword
  #### Palavra-chave do provedor de pesquisa padrão
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Especifica a palavra-chave, que é o atalho usado na Barra de Endereços para disparar a pesquisa para esse provedor.

Essa política é opcional. Se você não configurá-la, nenhuma palavra-chave ativará o provedor de pesquisa.

Essa política é aplicada somente quando você habilita as políticas [DefaultSearchProviderEnabled](#defaultsearchproviderenabled) e [DefaultSearchProviderSearchURL](#defaultsearchprovidersearchurl).

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Cadeia de Caracteres

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: DefaultSearchProviderKeyword
  - Nome da GP: Palavra-chave do provedor de pesquisa padrão
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/Provedor de pesquisa padrão
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: DefaultSearchProviderKeyword
  - Tipo de Valor: REG_SZ
  ##### Exemplo de valor:
```
"mis"
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: DefaultSearchProviderKeyword
  - Exemplo de valor:
``` xml
<string>mis</string>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### DefaultSearchProviderName
  #### Nome do provedor de pesquisa padrão
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Especifica o nome do provedor de pesquisa padrão.

Se você habilitar essa política, o nome do provedor de pesquisa padrão será definido.

Se você não habilitar essa política ou deixá-la vazia, o nome do host especificado pela URL de pesquisa será usado.

[DefaultSearchProviderName](#defaultsearchprovidername) deve ser definida como um provedor de pesquisa criptografado aprovado pela organização que corresponde ao provedor de pesquisa criptografado definido em DTBC-0008. Essa política é aplicada somente quando você habilita as políticas [DefaultSearchProviderEnabled](#defaultsearchproviderenabled) e [DefaultSearchProviderSearchURL](#defaultsearchprovidersearchurl).

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Cadeia de Caracteres

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: DefaultSearchProviderName
  - Nome da GP: Nome do provedor de pesquisa padrão
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/Provedor de pesquisa padrão
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: DefaultSearchProviderName
  - Tipo de Valor: REG_SZ
  ##### Exemplo de valor:
```
"My Intranet Search"
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: DefaultSearchProviderName
  - Exemplo de valor:
``` xml
<string>My Intranet Search</string>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### DefaultSearchProviderSearchURL
  #### URL de pesquisa do provedor de pesquisa padrão
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Especifica a URL do mecanismo de pesquisa usado para uma pesquisa padrão. A URL contém a cadeia de caracteres "{searchTerms}", que é substituída no momento da consulta pelos termos que o usuário está pesquisando.

Especifique a URL de pesquisa do Bing como:

"{bing:baseURL}search?q={searchTerms}".

Especifique a URL de pesquisa do Google como: "{google:baseURL}search?q={searchTerms}&{google:RLZ}{google:originalQueryForSuggestion}{google:assistedQueryStats}{google:searchFieldtrialParameter}{google:searchClient}{google:sourceId}ie={inputEncoding}".

Essa política é necessária ao ativar a política [DefaultSearchProviderEnabled](#defaultsearchproviderenabled); se você não habilitar a última política, essa política será ignorada.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Cadeia de Caracteres

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: DefaultSearchProviderSearchURL
  - Nome da GP: URL de pesquisa do provedor de pesquisa padrão
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/Provedor de pesquisa padrão
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: DefaultSearchProviderSearchURL
  - Tipo de Valor: REG_SZ
  ##### Exemplo de valor:
```
"https://search.contoso.com/search?q={searchTerms}"
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: DefaultSearchProviderSearchURL
  - Exemplo de valor:
``` xml
<string>https://search.contoso.com/search?q={searchTerms}</string>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### DefaultSearchProviderSuggestURL
  #### URL do provedor de pesquisa padrão para sugestões
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Especifica a URL do mecanismo de pesquisa usado para fornecer sugestões de pesquisa. A URL contém a cadeia de caracteres "{searchTerms}", que é substituída no momento da consulta pelo texto que o usuário inseriu até o momento.

Essa política é opcional. Se você não configurá-la, os usuários não verão sugestões de pesquisa. Eles verão sugestões do histórico de navegação e favoritos.

A URL de sugestão do Bing pode ser especificada como:

"{bing:baseURL}qbox?query={searchTerms}".

A URL de sugestão do Google pode ser especificada como: "{google:baseURL}complete/search?output=chrome&q={searchTerms}".

Essa política é aplicada somente quando você habilita as políticas [DefaultSearchProviderEnabled](#defaultsearchproviderenabled) e [DefaultSearchProviderSearchURL](#defaultsearchprovidersearchurl).

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Cadeia de Caracteres

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: DefaultSearchProviderSuggestURL
  - Nome da GP: URL do provedor de pesquisa padrão para sugestões
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/Provedor de pesquisa padrão
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: DefaultSearchProviderSuggestURL
  - Tipo de Valor: REG_SZ
  ##### Exemplo de valor:
```
"https://search.contoso.com/suggest?q={searchTerms}"
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: DefaultSearchProviderSuggestURL
  - Exemplo de valor:
``` xml
<string>https://search.contoso.com/suggest?q={searchTerms}</string>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ## Servidor proxy policies

  [Voltar ao início](#microsoft-edge---políticas)

  ### ProxyBypassList
  #### Configurar regras para ignorar o proxy
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Define uma lista de hosts para os quais o Microsoft Edge ignora qualquer proxy.

Essa política é aplicada somente se você selecionar "Usar servidores proxy fixos" na política [ProxyMode](#proxymode). Se você selecionar qualquer outro modo para a configuração de políticas de proxy, não habilite ou configure essa política.

Se você habilitar essa política, poderá criar uma lista de hosts para os quais o Microsoft Edge não usa um proxy.

Se você não configurar essa política, nenhuma lista de hosts será criada para a qual o Microsoft Edge ignora um proxy. Deixe essa política não configurada se você especificar qualquer outro método para definir políticas de proxy.

Para obter exemplos mais detalhados, acesse [https://go.microsoft.com/fwlink/?linkid=2094936](https://go.microsoft.com/fwlink/?linkid=2094936).

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Cadeia de Caracteres

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: ProxyBypassList
  - Nome da GP: Configurar regras para ignorar o proxy
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/Servidor proxy
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: ProxyBypassList
  - Tipo de Valor: REG_SZ
  ##### Exemplo de valor:
```
"https://www.contoso.com, https://www.fabrikam.com"
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: ProxyBypassList
  - Exemplo de valor:
``` xml
<string>https://www.contoso.com, https://www.fabrikam.com</string>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### ProxyMode
  #### Definir configurações de servidor proxy
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Especifique as configurações do servidor proxy usadas pelo Microsoft Edge. Se você habilitar essa política, os usuários não podem alterar as configurações de proxy.

Se você optar por nunca usar um servidor proxy e sempre conectar-se diretamente, todas as outras opções serão ignoradas.

Se você optar por usar as configurações de proxy do sistema, todas as outras opções serão ignoradas.

Se você optar por detectar automaticamente o servidor proxy, todas as outras opções serão ignoradas.

Se você optar pelo modo fixo de servidor proxy, poderá especificar outras opções em [ProxyServer](#proxyserver) e "Lista separada por vírgulas de regras para ignorar o proxy".

Se você optar por usar um script de proxy do .pac, você deve especificar a URL para o script "URL para um arquivo .pac de proxy".

Para obter exemplos detalhados, vá para [https://go.microsoft.com/fwlink/?linkid=2094936](https://go.microsoft.com/fwlink/?linkid=2094936).

Se você habilitar essa política, o Microsoft Edge ignorará todas as opções relacionadas ao proxy especificadas na linha de comando.

Se você não configurar essa política, os usuários poderão escolher suas próprias configurações de proxy.

* "direct" = Nunca usar um proxy

* "auto_detect" = Detectar automaticamente as configurações de proxy

* "pac_script" = Usar um script de proxy do .pac

* "fixed_servers" = Usar servidores proxy fixos

* "system" = Usar configurações de proxy do sistema

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Cadeia de Caracteres

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: ProxyMode
  - Nome da GP: Definir configurações de servidor proxy
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/Servidor proxy
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: ProxyMode
  - Tipo de Valor: REG_SZ
  ##### Exemplo de valor:
```
"direct"
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: ProxyMode
  - Exemplo de valor:
``` xml
<string>direct</string>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### ProxyPacUrl
  #### Definir a URL do arquivo .pac do proxy
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Especifica a URL de um arquivo de configuração automática do proxy (PAC).

Essa política será aplicada somente se você tiver selecionado "Usar um script de proxy .pac" na política [ProxyMode](#proxymode). Se você tiver selecionado qualquer outro modo para configurar as políticas de proxy, não habilite ou configure essa política.

Se você habilitar essa política, poderá especificar a URL de um arquivo PAC, que define como o navegador escolherá automaticamente o servidor proxy apropriado para buscar um site específico.

Se você desabilitar ou não configurar essa política, nenhum arquivo PAC será especificado. Deixe essa política não configurada se você tiver especificado qualquer outro método para definir políticas de proxy.

Para obter exemplos detalhados, consulte [https://go.microsoft.com/fwlink/?linkid=2094936](https://go.microsoft.com/fwlink/?linkid=2094936).

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Cadeia de Caracteres

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: ProxyPacUrl
  - Nome da GP: Definir a URL do arquivo .pac do proxy
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/Servidor proxy
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: ProxyPacUrl
  - Tipo de Valor: REG_SZ
  ##### Exemplo de valor:
```
"https://internal.contoso.com/example.pac"
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: ProxyPacUrl
  - Exemplo de valor:
``` xml
<string>https://internal.contoso.com/example.pac</string>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### ProxyServer
  #### Configurar o endereço ou a URL do servidor proxy
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Especifica a URL do servidor proxy.

Essa política será aplicada somente se você tiver selecionado "Usar servidores proxy fixos" na política [ProxyMode](#proxymode). Se você tiver selecionado qualquer outro modo para configurar as políticas de proxy, não habilite ou configure essa política.

Se você habilitar essa política, o servidor proxy configurado por essa política será usado para todas as URLs.

Se você desabilitar ou não configurar essa política, os usuários poderão escolher suas próprias configurações de proxy nesse modo de proxy. Deixe essa política desconfigurada se você tiver especificado qualquer outro método para definir políticas de proxy.

Para obter mais opções e exemplos detalhados, consulte [https://go.microsoft.com/fwlink/?linkid=2094936](https://go.microsoft.com/fwlink/?linkid=2094936).

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Cadeia de Caracteres

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: ProxyServer
  - Nome da GP: Configurar o endereço ou a URL do servidor proxy
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/Servidor proxy
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: ProxyServer
  - Tipo de Valor: REG_SZ
  ##### Exemplo de valor:
```
"123.123.123.123:8080"
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: ProxyServer
  - Exemplo de valor:
``` xml
<string>123.123.123.123:8080</string>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### ProxySettings
  #### Configurações de proxy
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Define as configurações de proxy para o Microsoft Edge.

Se você habilitar essa política, o Microsoft Edge ignorará todas as opções relacionadas ao proxy especificadas na linha de comando.

Se você não configurar essa política, os usuários poderão escolher suas próprias configurações de proxy.

Essa política substitui as seguintes políticas individuais:

[ProxyMode](#proxymode)
[ProxyPacUrl](#proxypacurl)
[ProxyServer](#proxyserver)
[ProxyBypassList](#proxybypasslist)

O campo ProxyMode permite especificar o servidor proxy usado pelo Microsoft Edge e impede que os usuários alterem as configurações do proxy.

O campo ProxyPacUrl é uma URL para um arquivo .pac do proxy.

O campo ProxyServer é uma URL do servidor proxy.

O campo ProxyBypassList é uma lista de hosts proxy que o Microsoft Edge ignora.

Se você escolher o valor "direct" como [ProxyMode](#proxymode), um proxy nunca será usado e todos os outros campos serão ignorados.

Se você escolher o valor "system" como [ProxyMode](#proxymode), o proxy do sistema será usado e todos os outros campos serão ignorados.

Se você escolher o valor "auto_detect" como [ProxyMode](#proxymode), todos os outros campos serão ignorados.

Se você escolher o valor "fixed_server" como [ProxyMode](#proxymode), os campos [ProxyServer](#proxyserver) e [ProxyBypassList](#proxybypasslist) serão usados.

Se você escolher o valor "pac_script" como [ProxyMode](#proxymode), os campos [ProxyPacUrl](#proxypacurl) e [ProxyBypassList](#proxybypasslist) serão usados.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Dicionário

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: ProxySettings
  - Nome da GP: Configurações de proxy
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/Servidor proxy
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: ProxySettings
  - Tipo de Valor: REG_SZ
  ##### Exemplo de valor:
```
SOFTWARE\Policies\Microsoft\Edge\ProxySettings = {
  "ProxyBypassList": "https://www.example1.com,https://www.example2.com,https://internalsite/", 
  "ProxyMode": "direct", 
  "ProxyPacUrl": "https://internal.site/example.pac", 
  "ProxyServer": "123.123.123.123:8080"
}
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: ProxySettings
  - Exemplo de valor:
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
  

  [Voltar ao início](#microsoft-edge---políticas)

  ## Additional policies

  [Voltar ao início](#microsoft-edge---políticas)

  ### AdsSettingForIntrusiveAdsSites
  #### Configuração de anúncios para sites com anúncios intrusivos
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 78 ou posterior

  #### Descrição
  Controla se os anúncios são bloqueados ou não em sites com anúncios intrusivos. Você pode definir essa política como uma das seguintes opções:

* 1 = Permitir anúncios em todos os sites.

* 2 = Bloquear anúncios em sites com anúncios intrusivos (valor padrão).

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Número inteiro

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: AdsSettingForIntrusiveAdsSites
  - Nome da GP: Configuração de anúncios para sites com anúncios intrusivos
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: AdsSettingForIntrusiveAdsSites
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000001
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: AdsSettingForIntrusiveAdsSites
  - Exemplo de valor:
``` xml
<integer>1</integer>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### AllowDeletingBrowserHistory
  #### Habilitar a exclusão do navegador e do histórico de download
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Habilita a exclusão do histórico do navegador e do histórico de downloads e impede que os usuários alterem essa configuração.

Observe que, mesmo com essa política está desabilitada, o histórico de navegação e download não são garantidos: os usuários podem editar ou excluir os arquivos do banco de dados de histórico diretamente, e o próprio navegador pode remover (com base no período de expiração) ou arquivar qualquer ou todos itens de histórico a qualquer momento.

Se você habilitar essa política ou não configurá-la, os usuários poderão excluir o histórico de navegação e download.

Se você desabilitar essa política, os usuários não poderão excluir o histórico de navegação e download.

Se você habilitar essa política, não habilite a política "Limpar dados de navegação quando o Microsoft Edge for fechado", pois ambas lidam com a exclusão de dados. Se você habilitar as duas, a política "Limpar dados de navegação quando o Microsoft Edge for fechado" terá precedência e excluirá todos os dados quando o Microsoft Edge, independentemente de como essa política está configurada.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: AllowDeletingBrowserHistory
  - Nome da GP: Habilitar a exclusão do navegador e do histórico de download
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: AllowDeletingBrowserHistory
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000001
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: AllowDeletingBrowserHistory
  - Exemplo de valor:
``` xml
<true/>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### AllowFileSelectionDialogs
  #### Permitir caixas de diálogo de seleção de arquivos
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Conceda acesso a arquivos locais permitindo que o Microsoft Edge exiba caixas de diálogo de seleção de arquivos

Se você habilitar ou não configurar essa política, os usuários poderão abrir caixas de diálogo de seleção de arquivos normalmente.

Se você desabilitar essa política, sempre que o usuário executar uma ação que dispare uma caixa de diálogo de seleção de arquivos (como importar favoritos, carregar arquivos ou salvar links), será exibida uma mensagem, e presume-se que o usuário clicou em Cancelar na caixa de diálogo de seleção de arquivos.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: AllowFileSelectionDialogs
  - Nome da GP: Permitir caixas de diálogo de seleção de arquivos
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: AllowFileSelectionDialogs
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000001
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: AllowFileSelectionDialogs
  - Exemplo de valor:
``` xml
<true/>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### AllowPopupsDuringPageUnload
  #### Permite que uma página mostre pop-ups durante seu descarregamento
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 78 ou posterior

  #### Descrição
  Essa política permite que um administrador especifique que uma página pode mostrar pop-ups durante seu descarregamento.

Quando a política está configurada como habilitada, as páginas podem mostrar pop-ups enquanto estão sendo descarregadas.

Quando a política está configurada como desabilitada ou não está configurada, as páginas não podem mostrar pop-ups enquanto estão sendo descarregadas, de acordo com a especificação: (https://html.spec.whatwg.org/#apis-for-creating-and-navigating-browsing-contexts-by-name).

Esta política será removida no futuro.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Não - Requer a reinicialização do navegador

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: AllowPopupsDuringPageUnload
  - Nome da GP: Permite que uma página mostre pop-ups durante seu descarregamento
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: AllowPopupsDuringPageUnload
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000000
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: AllowPopupsDuringPageUnload
  - Exemplo de valor:
``` xml
<false/>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### AllowSyncXHRInPageDismissal
  #### Permitir que as páginas enviem solicitações XHR síncronas durante o descarte de páginas
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 79 ou posterior

  #### Descrição
  Essa política permite especificar que uma página pode enviar solicitações XHR síncronas durante o descarte de páginas.

Se você habilitar essa política, as páginas poderão enviar solicitações XHR síncronas durante o descarte de páginas.

Se você desabilitar ou não configurar essa política, as páginas não poderão enviar solicitações XHR síncronas durante o descarte de páginas.

Essa política é temporária e será removida em uma versão futura.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Não - Requer a reinicialização do navegador

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: AllowSyncXHRInPageDismissal
  - Nome da GP: Permitir que as páginas enviem solicitações XHR síncronas durante o descarte de páginas
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: AllowSyncXHRInPageDismissal
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000000
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: AllowSyncXHRInPageDismissal
  - Exemplo de valor:
``` xml
<false/>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### AllowTrackingForUrls
  #### Configurar exceções de prevenção de rastreamento para sites específicos
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 78 ou posterior

  #### Descrição
  Configure a lista de padrões de URL que são excluídos da prevenção de rastreamento.

Se você configurar essa política, a lista de padrões de URL configurados será excluída da prevenção de rastreamento.

Se você não configurar essa política, o valor padrão global da política "Bloquear rastreamento de usuários" (se definida), ou a configuração pessoal do usuário será usada para todos os sites.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Lista de cadeias de caracteres

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: AllowTrackingForUrls
  - Nome da GP: Configurar exceções de prevenção de rastreamento para sites específicos
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge\AllowTrackingForUrls
  - Caminho (Recomendações): N/A
  - Nome do Valor: 1, 2, 3, ...
  - Tipo de Valor: lista de REG_SZ
  ##### Exemplo de valor:
```
SOFTWARE\Policies\Microsoft\Edge\AllowTrackingForUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\AllowTrackingForUrls\1 = "[*.]contoso.edu"

```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: AllowTrackingForUrls
  - Exemplo de valor:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>[*.]contoso.edu</string>
</array>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### AlternateErrorPagesEnabled
  #### Sugerir páginas similares quando uma página da Web não puder ser encontrada
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 80 ou posterior

  #### Descrição
  Permita que o Microsoft Edge emita uma conexão com um serviço Web para gerar sugestões de pesquisa e URL para problemas de conectividade, como erros de DNS.

Se você habilitar essa política, um serviço Web será usado para gerar sugestões de pesquisa e URL para erros de rede.

Se você desabilitar essa política, nenhuma chamada para o serviço Web será feita, e uma página de erro padrão será exibida.

Se você não configurar essa política, o Microsoft Edge respeitará a preferência do usuário definida em Serviços em edge://settings/privacy.
Especificamente, há uma alternância de **Sugerir páginas similares quando uma página não puder ser encontrada**, o que o usuário pode ativar ou desativar. Observe que, se você habilitar essa política (AlternateErrorPagesEnabled), a configuração Sugerir páginas similares quando uma página da Web não puder ser encontrada estiver ativada, mas o usuário não puder alterar a configuração usando a alternância. Se você desabilitar essa política, a configuração Sugerir páginas similares quando uma página da Web não puder ser encontrada será desativada, e o usuário não poderá alterar a configuração usando a alternância.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Sim
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: AlternateErrorPagesEnabled
  - Nome da GP: Sugerir páginas similares quando uma página da Web não puder ser encontrada
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): Modelos Administrativos/Microsoft Edge - Configurações Padrão (os usuários podem substituir)/
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): SOFTWARE\Policies\Microsoft\Edge\Recomendações
  - Nome do Valor: AlternateErrorPagesEnabled
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000001
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: AlternateErrorPagesEnabled
  - Exemplo de valor:
``` xml
<true/>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### AlwaysOpenPdfExternally
  #### Sempre abrir arquivos PDF externamente
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Desabilita o Visualizador de PDF interno no Microsoft Edge.

Se você habilitar essa política, o Microsoft Edge tratará arquivos PDF como downloads e permitirá que os usuários os abram com o aplicativo padrão.

Se você não configurar essa política ou desabilitá-la, o Microsoft Edge abrirá arquivos PDF (a menos que o usuário a desabilite).

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: AlwaysOpenPdfExternally
  - Nome da GP: Sempre abrir arquivos PDF externamente
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: AlwaysOpenPdfExternally
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000001
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: AlwaysOpenPdfExternally
  - Exemplo de valor:
``` xml
<true/>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### ApplicationLocaleValue
  #### Definir localidade do aplicativo
  >Versões com Suporte: O Microsoft Edge no Windows desde a versão 77 ou posterior

  #### Descrição
  Configura a localidade do aplicativo em Microsoft Edge e impede que os usuários a alterem.

Se você habilitar esta política, o Microsoft Edge usará a localidade especificada. Se a localidade configurada não tiver suporte, será usada a "en-US".

Se você desabilitar ou não definir esta configuração, o Microsoft Edge usará a localidade preferencial especificada pelo usuário (se configurada) ou a localidade de fallback "en-US".

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Sim
  - Atualização de política dinâmica: Não - Requer a reinicialização do navegador

  #### Tipo de Dados:
  Cadeia de Caracteres

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: ApplicationLocaleValue
  - Nome da GP: Definir localidade do aplicativo
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): Modelos Administrativos/Microsoft Edge - Configurações Padrão (os usuários podem substituir)/
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): SOFTWARE\Policies\Microsoft\Edge\Recomendações
  - Nome do Valor: ApplicationLocaleValue
  - Tipo de Valor: REG_SZ
  ##### Exemplo de valor:
```
"en"
```


  

  [Voltar ao início](#microsoft-edge---políticas)

  ### AudioCaptureAllowed
  #### Permitir ou bloquear captura de áudio
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Permite definir se o usuário será solicitado a conceder acesso a um site para seus dispositivos de captura de áudio. Esta política se aplica a todas as URLs, exceto aquelas configuradas na lista [AudioCaptureAllowedUrls](#audiocaptureallowedurls).

Se você habilitar ou não configurar esta política (configuração padrão), o usuário será solicitado a fornecer acesso de captura de áudio, exceto das URLs na lista [AudioCaptureAllowedUrls](#audiocaptureallowedurls). Essas URLs listadas terão acesso sem solicitação.

Se esta política for desabilitada, o usuário não será avisado, e a captura de áudio ficará acessível somente para as URLs configuradas em [AudioCaptureAllowedUrls](#audiocaptureallowedurls).

Esta política afeta todos os tipos de entradas de áudio, não apenas o microfone interno.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: AudioCaptureAllowed
  - Nome da GP: Permitir ou bloquear captura de áudio
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: AudioCaptureAllowed
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000000
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: AudioCaptureAllowed
  - Exemplo de valor:
``` xml
<false/>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### AudioCaptureAllowedUrls
  #### Sites podem acessar dispositivos de captura áudio sem solicitar permissão
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Especifica sites, com base nos padrões de URL, que podem usar dispositivos de captura de áudio sem pedir permissão ao usuário. Padrões nesta lista são comparados com a origem de segurança da URL solicitante. Se forem correspondentes, o site terá acesso automaticamente aos dispositivos de captura de áudio.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Lista de cadeias de caracteres

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: AudioCaptureAllowedUrls
  - Nome da GP: Sites podem acessar dispositivos de captura áudio sem solicitar permissão
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge\AudioCaptureAllowedUrls
  - Caminho (Recomendações): N/A
  - Nome do Valor: 1, 2, 3, ...
  - Tipo de Valor: lista de REG_SZ
  ##### Exemplo de valor:
```
SOFTWARE\Policies\Microsoft\Edge\AudioCaptureAllowedUrls\0 = "https://www.contoso.com/"
SOFTWARE\Policies\Microsoft\Edge\AudioCaptureAllowedUrls\1 = "https://[*.]contoso.edu/"

```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: AudioCaptureAllowedUrls
  - Exemplo de valor:
``` xml
<array>
  <string>https://www.contoso.com/</string>
  <string>https://[*.]contoso.edu/</string>
</array>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### AutoImportAtFirstRun
  #### Importar automaticamente os dados e as configurações de outro navegador na primeira execução
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Se você habilitar essa política, o Microsoft Edge importará automaticamente todos os tipos de dados e configurações do navegador padrão ou de outro navegador especificado. Isso também força o Microsoft Edge a ignorar a seção de importação da experiência de primeira execução.

Se você configurar essa política para "DisabledAutoImport" (4), a seção de importação da experiência de primeira execução será completamente ignorada, e o Microsoft Edge não importará dados e configurações do navegador automaticamente.

* 0 = Importa automaticamente todos os tipos de dados e configurações com suporte do navegador padrão

* 1 = Importa automaticamente todos os tipos de dados e configurações com suporte do Internet Explorer

* 2 = Importa automaticamente todos os tipos de dados e configurações com suporte do Google Chrome

* 3 = Importa automaticamente todos os tipos de dados e configurações com suporte do Safari

* 4 = Desabilita a importação automática, e a seção de importação da experiência de primeira execução é ignorada

**Observação**: essa política atualmente oferece suporte à importação dos navegadores Internet Explorer (no Windows 7, 8 e 10), Google Chrome (no Windows 7, 8 e 10 e macOS) e Apple Safari (em macOS).

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Não - Requer a reinicialização do navegador

  #### Tipo de Dados:
  Número inteiro

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: AutoImportAtFirstRun
  - Nome da GP: Importar automaticamente os dados e as configurações de outro navegador na primeira execução
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: AutoImportAtFirstRun
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000002
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: AutoImportAtFirstRun
  - Exemplo de valor:
``` xml
<integer>2</integer>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### AutofillAddressEnabled
  #### Habilitar AutoPreenchimento para endereços
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Habilita o recurso AutoPreenchimento e permite que os usuários preencham automaticamente informações de endereço em formulários da Web usando informações armazenadas anteriormente.

Se você desabilitar essa política, o AutoPreenchimento nunca sugere ou preenche informações de endereço, nem salva informações adicionais de endereço que o usuário pode enviar ao navegar na Web.

Se você habilitar essa política ou não configurá-la, os usuários poderão controlar o AutoPreenchimento de endereços na interface do usuário.

Observe que, se você desabilitar essa política, também interromperá todas as atividades de todos os formulários da Web, exceto os formulários de pagamento e senha. Nenhuma outra entrada será salva e o Microsoft Edge não sugerirá nem preencherá as entradas anteriores.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Sim
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: AutofillAddressEnabled
  - Nome da GP: Habilitar AutoPreenchimento para endereços
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): Modelos Administrativos/Microsoft Edge - Configurações Padrão (os usuários podem substituir)/
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): SOFTWARE\Policies\Microsoft\Edge\Recomendações
  - Nome do Valor: AutofillAddressEnabled
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000000
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: AutofillAddressEnabled
  - Exemplo de valor:
``` xml
<false/>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### AutofillCreditCardEnabled
  #### Habilitar AutoPreenchimento para cartões de crédito
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Habilita o recurso de AutoPreenchimento do Microsoft Edge e permite que os usuários completem automaticamente informações de cartão de crédito em formulários da Web usando informações armazenadas anteriormente.

Se você desabilitar essa política, o AutoPreenchimento nunca sugerirá ou preencherá informações de cartão de crédito, nem salvará informações adicionais de cartão de crédito que os usuários possam enviar enquanto navegam na Web.

Se você habilitar essa política ou não configurá-la, os usuários poderão controlar o AutoPreenchimento de cartões de crédito.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Sim
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: AutofillCreditCardEnabled
  - Nome da GP: Habilitar AutoPreenchimento para cartões de crédito
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): Modelos Administrativos/Microsoft Edge - Configurações Padrão (os usuários podem substituir)/
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): SOFTWARE\Policies\Microsoft\Edge\Recomendações
  - Nome do Valor: AutofillCreditCardEnabled
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000000
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: AutofillCreditCardEnabled
  - Exemplo de valor:
``` xml
<false/>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### AutoplayAllowed
  #### Permitir reprodução automática de mídia para sites
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 78 ou posterior

  #### Descrição
  Esta política define a política de reprodução automática de mídia para sites.

A configuração padrão, "Não configurada", respeita as configurações de reprodução automática de mídia atuais e permite que os usuários definam suas configurações de reprodução automática.

Configurar como "Habilitada" define a reprodução automática de mídia para "Permitir".  Todos os sites podem executar a reprodução automática de mídia. Os usuários não podem substituir essa política.

Configurar como "Desabilitada" define a reprodução automática de mídia para "Bloquear". Nenhum site tem permissão para executar a reprodução automática. Os usuários não podem substituir essa política.

Uma guia terá que ser fechada e reaberta para que essa política entre em vigor.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: AutoplayAllowed
  - Nome da GP: Permitir reprodução automática de mídia para sites
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: AutoplayAllowed
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000001
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: AutoplayAllowed
  - Exemplo de valor:
``` xml
<true/>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### BackgroundModeEnabled
  #### Continuar executando apps em segundo plano depois que o Microsoft Edge for fechado
  >Versões com Suporte: O Microsoft Edge no Windows desde a versão 77 ou posterior

  #### Descrição
  Permite que os processos do Microsoft Edge sejam iniciados durante a conexão do SO e continuem em execução depois que a última janela do navegador for fechada. Nesse cenário, os aplicativos em segundo plano e a sessão de navegação atual permanecem ativos, incluindo quaisquer cookies de sessão. Um processo em segundo plano aberto exibe um ícone na bandeja do sistema e sempre pode ser fechado a partir desse local.

Se você habilitar essa política, o modo de segundo plano será ativado.

Se você desabilitar essa política, o modo de segundo plano será desativado.

Se você não configurar essa política, o modo de segundo plano será inicialmente desativado e o usuário poderá configurar seu comportamento em edge://settings/system.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Sim
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: BackgroundModeEnabled
  - Nome da GP: Continuar executando apps em segundo plano depois que o Microsoft Edge for fechado
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): Modelos Administrativos/Microsoft Edge - Configurações Padrão (os usuários podem substituir)/
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): SOFTWARE\Policies\Microsoft\Edge\Recomendações
  - Nome do Valor: BackgroundModeEnabled
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000001
```


  

  [Voltar ao início](#microsoft-edge---políticas)

  ### BackgroundTemplateListUpdatesEnabled
  #### Permite atualizações em segundo plano na lista de modelos disponíveis para Coleções e outros recursos que usam modelos
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 79 ou posterior

  #### Descrição
  Permite habilitar ou desabilitar atualizações em segundo plano na lista de modelos disponíveis para Coleções e outros recursos que usam modelos.  Os modelos são usados para extrair metadados sofisticados de uma página da Web quando a página é salva em uma coleção.

Se você habilitar essa configuração ou se a configuração não estiver definida, a lista de modelos disponíveis será baixada em segundo plano de um serviço Microsoft a cada 24 horas.

Se você desabilitar esta configuração, a lista de modelos disponíveis será baixada por demanda. Esse tipo de download pode resultar em pequenas penalidades de desempenho para Coleções e outros recursos.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: BackgroundTemplateListUpdatesEnabled
  - Nome da GP: Permite atualizações em segundo plano na lista de modelos disponíveis para Coleções e outros recursos que usam modelos
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: BackgroundTemplateListUpdatesEnabled
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000001
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: BackgroundTemplateListUpdatesEnabled
  - Exemplo de valor:
``` xml
<true/>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### BlockThirdPartyCookies
  #### Bloquear cookies de terceiros
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Impede que os elementos de páginas da Web que não pertençam ao domínio indicado na barra de endereços definam cookies.

Se você habilitar esta política, os elementos de páginas da Web que não pertencerem ao domínio indicado na barra de endereços não poderão definir cookies

Se você desabilitar esta política, os elementos de páginas da Web de domínios não indicados na barra de endereços poderão definir cookies.

Se você não configurar esta política, os cookies de terceiros serão habilitados, mas os usuários poderão alterar essa configuração.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Sim
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: BlockThirdPartyCookies
  - Nome da GP: Bloquear cookies de terceiros
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): Modelos Administrativos/Microsoft Edge - Configurações Padrão (os usuários podem substituir)/
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): SOFTWARE\Policies\Microsoft\Edge\Recomendações
  - Nome do Valor: BlockThirdPartyCookies
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000000
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: BlockThirdPartyCookies
  - Exemplo de valor:
``` xml
<false/>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### BrowserAddProfileEnabled
  #### Habilitar a criação de perfil no menu do submenu Identidade ou na página Configurações
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Permite que os usuários criem novos perfis usando a opção **Adicionar perfil**.
Se você habilitar essa política ou não configurá-la, o Microsoft Edge permitirá que os usuários usem **Adicionar perfil** no menu de submenu Identidade ou na página Configurações para criar novos perfis.

Se você desabilitar essa política, os usuários não poderão adicionar novos perfis a partir do menu do submenu Identidade ou da página Configurações.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: BrowserAddProfileEnabled
  - Nome da GP: Habilitar a criação de perfil no menu do submenu Identidade ou na página Configurações
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: BrowserAddProfileEnabled
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000001
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: BrowserAddProfileEnabled
  - Exemplo de valor:
``` xml
<true/>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### BrowserGuestModeEnabled
  #### Habilitar modo convidado
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Habilita a opção para permitir o uso de perfis de convidado no Microsoft Edge. Em um perfil de convidado, o navegador não importa os dados de navegação dos perfis existentes e exclui os dados de navegação quando todos os perfis de convidado são fechados.

Se você habilitar essa política ou não configurá-la, o Microsoft Edge permitirá que os usuários naveguem em perfis de convidado.

Se você desabilitar esta política, o Microsoft Edge não permitirá que os usuários naveguem em perfis de convidado.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: BrowserGuestModeEnabled
  - Nome da GP: Habilitar modo convidado
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: BrowserGuestModeEnabled
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000001
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: BrowserGuestModeEnabled
  - Exemplo de valor:
``` xml
<true/>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### BrowserNetworkTimeQueriesEnabled
  #### Permitir consultas a um serviço de Hora da Rede do Navegador
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Impede que Microsoft Edge envie ocasionalmente consultas a um serviço de tempo de rede do navegador para recuperar um registro de carimbo de data/hora preciso.

Se você desabilitar essa política, o Microsoft Edge deixará de enviar consultas para um serviço de tempo de rede do navegador.

Se você habilitar essa política ou não configurá-la, o Microsoft Edge ocasionalmente enviará consultas para um serviço de tempo de rede do navegador.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: BrowserNetworkTimeQueriesEnabled
  - Nome da GP: Permitir consultas a um serviço de Hora da Rede do Navegador
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: BrowserNetworkTimeQueriesEnabled
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000001
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: BrowserNetworkTimeQueriesEnabled
  - Exemplo de valor:
``` xml
<true/>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### BrowserSignin
  #### Configurações de entrada do navegador
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Especifique se um usuário pode entrar no Microsoft Edge com sua própria conta e usar serviços relacionados à conta, como sincronização e logon único. Para controlar a disponibilidade da sincronização, use a política [SyncDisabled](#syncdisabled).

Se você definir essa política como "Desabilitar entrada no navegador", também defina a política [NonRemovableProfileEnabled](#nonremovableprofileenabled) como desabilitada porque [NonRemovableProfileEnabled](#nonremovableprofileenabled) desabilita a criação de um perfil de navegador conectado automaticamente. Se as duas políticas forem definidas, o Microsoft Edge usará a política "Desabilitar entrada no navegador" e se comportará como se [NonRemovableProfileEnabled](#nonremovableprofileenabled) estivesse definida como desabilitada.

Se você definir essa política como "Habilitar entrada no navegador" (1), os usuários poderão entrar no navegador. Entrar no navegador não significa que a sincronização será ativada por padrão; o usuário deverá aceitar separadamente para usar esse recurso.

Se você definir essa política como "Forçar entrada no navegador" (2), os usuários deverão entrar em um perfil para usar o navegador. Por padrão, isso permitirá que o usuário escolha se quer sincronizar com a conta, a menos que a sincronização seja desabilitada pelo administrador do domínio ou com a política [SyncDisabled](#syncdisabled). O valor padrão da política [BrowserGuestModeEnabled](#browserguestmodeenabled) é definido como false.

Se você não configurar essa política, os usuários poderão decidir se desejam habilitar a opção de entrada no navegador e usá-la como quiserem.

* 0 = Desabilitar entrada no navegador

* 1 = Habilitar entrada no navegador

* 2 = Forçar os usuários a entrarem para usar o navegador

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Não - Requer a reinicialização do navegador

  #### Tipo de Dados:
  Número inteiro

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: BrowserSignin
  - Nome da GP: Configurações de entrada do navegador
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: BrowserSignin
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000002
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: BrowserSignin
  - Exemplo de valor:
``` xml
<integer>2</integer>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### BuiltInDnsClientEnabled
  #### Usar o cliente DNS interno
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Controla se o cliente DNS interno deve ser usado.

Isso não afeta quais servidores DNS são usados, apenas a pilha de software usada para se comunicar com eles. Por exemplo, se o sistema operacional estiver configurado para usar um servidor DNS corporativo, esse mesmo servidor será usado pelo cliente DNS interno. No entanto, é possível que o cliente DNS interno atenda servidores de formas diferentes usando protocolos mais modernos relacionados ao DNS, como o DNS sobre TLS.

Se você habilitar essa política, o cliente DNS interno será usado, caso esteja disponível.

Se você desabilitar essa política, o cliente nunca será usado.

Se você não configurar essa política, o cliente DNS interno será habilitado por padrão no MacOS, e os usuários poderão alterar se desejam usar o cliente DNS interno editando edge://flags ou especificando um sinalizador de linha de comando.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: BuiltInDnsClientEnabled
  - Nome da GP: Usar o cliente DNS interno
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: BuiltInDnsClientEnabled
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000001
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: BuiltInDnsClientEnabled
  - Exemplo de valor:
``` xml
<true/>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### CertificateTransparencyEnforcementDisabledForCas
  #### Desabilitar a imposição de Transparência de Certificado para uma lista de hashes de subjectPublicKeyInfo
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Desabilita a imposição dos requisitos de Transparência de Certificado para uma lista de hashes subjectPublicKeyInfo.

Essa política permite desabilitar os requisitos de divulgação da Transparência de Certificado para cadeias de certificados que contenham certificados com um dos hashes subjectPublicKeyInfo especificados. Isso permite que certificados que de outra forma não seriam confiáveis, porque não foram divulgados publicamente da forma devida, continuem sendo usados para hosts Enterprise.

Para desabilitar a imposição da Transparência de Certificado quando essa política for definida, um dos seguintes conjuntos de condições deverá ser atendido:
1. O hash é do subjectPublicKeyInfo do certificado do servidor.
2. O hash é de um subjectPublicKeyInfo que aparece em um certificado da autoridade de certificação na cadeia de certificados, que é restrito pela extensão X.509v3 nameConstraints, um ou mais directoryName nameConstraints estão presentes nos permittedSubtrees e o directoryName contém um atributo organizationName.
3. O hash é de um subjectPublicKeyInfo que aparece em um certificado da autoridade de certificação na cadeia de certificados, o certificado de autoridade de certificação possui um ou mais atributos organizationName no certificado Subject e o certificado do servidor contém o mesmo número de atributos organizationName, na mesma ordem e com valores idênticos byte por byte.

Um hash subjectPublicKeyInfo é especificado concatenando o nome do algoritmo de hash, o caractere "/" e a codificação Base64 desse algoritmo de hash aplicado ao subjectPublicKeyInfo codificado por DER do certificado especificado. Essa codificação Base64 tem o mesmo formato de uma impressão digital SPKI, conforme definido na RFC 7469, seção 2.4. Algoritmos de hash não reconhecidos são ignorados. O único algoritmo de hash compatível neste momento é "sha256".

Se você desabilitar essa política ou não a configurar, todos os certificados que tiverem de ser divulgados por meio da Transparência de Certificado serão tratados como não confiáveis se não forem divulgados de acordo com a política Transparência de Certificado.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Lista de cadeias de caracteres

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: CertificateTransparencyEnforcementDisabledForCas
  - Nome da GP: Desabilitar a imposição de Transparência de Certificado para uma lista de hashes de subjectPublicKeyInfo
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge\CertificateTransparencyEnforcementDisabledForCas
  - Caminho (Recomendações): N/A
  - Nome do Valor: 1, 2, 3, ...
  - Tipo de Valor: lista de REG_SZ
  ##### Exemplo de valor:
```
SOFTWARE\Policies\Microsoft\Edge\CertificateTransparencyEnforcementDisabledForCas\0 = "sha256/AAAAAAAAAAAAAAAAAAAAAA=="
SOFTWARE\Policies\Microsoft\Edge\CertificateTransparencyEnforcementDisabledForCas\1 = "sha256//////////////////////w=="

```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: CertificateTransparencyEnforcementDisabledForCas
  - Exemplo de valor:
``` xml
<array>
  <string>sha256/AAAAAAAAAAAAAAAAAAAAAA==</string>
  <string>sha256//////////////////////w==</string>
</array>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### CertificateTransparencyEnforcementDisabledForLegacyCas
  #### Desabilitar a imposição de Transparência de Certificado para uma lista de autoridades de certificação herdadas
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Desabilita a imposição de requisitos de Transparência de Certificado para uma lista de autoridades de certificação (ACs) herdadas.

Essa política permite desabilitar os requisitos de divulgação de transparência de certificado para cadeias de certificados que contenham certificados com um dos hashes subjectPublicKeyInfo especificados. Isso permite que os certificados, que de outra forma não seriam confiáveis por não terem sido divulgados publicamente da forma correta, continuem a ser usados para hosts corporativos.

Para que a imposição de Transparência de Certificado seja desabilitada, você deve definir o hash como um subjectPublicKeyInfo que seja exibido em um Certificado de Autoridade de Certificação reconhecido como uma AC (autoridade de certificação) herdada. Uma AC herdada é uma AC que foi publicamente considerada confiável por padrão por um ou mais sistemas operacionais compatíveis com o Microsoft Edge.

Você especifica um hash de subjectPublicKeyInfo concatenando o nome do algoritmo de hash, o caractere "/" e a codificação Base64 desse algoritmo de hash aplicado ao subjectPublicKeyInfo codificado por DER do certificado especificado. Essa codificação Base64 tem o mesmo formato que uma impressão digital SPKI, conforme definido no RFC 7469, Seção 2.4. Os algoritmos de hash não reconhecidos são ignorados. O único algoritmo de hash com suporte no momento é o "sha256".

Se você não configurar essa política, qualquer certificado que precise ser divulgado por meio da Transparência de Certificado será tratado como não confiável se não for divulgado de acordo com a política Transparência de Certificado.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Lista de cadeias de caracteres

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: CertificateTransparencyEnforcementDisabledForLegacyCas
  - Nome da GP: Desabilitar a imposição de Transparência de Certificado para uma lista de autoridades de certificação herdadas
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge\CertificateTransparencyEnforcementDisabledForLegacyCas
  - Caminho (Recomendações): N/A
  - Nome do Valor: 1, 2, 3, ...
  - Tipo de Valor: lista de REG_SZ
  ##### Exemplo de valor:
```
SOFTWARE\Policies\Microsoft\Edge\CertificateTransparencyEnforcementDisabledForLegacyCas\0 = "sha256/AAAAAAAAAAAAAAAAAAAAAA=="
SOFTWARE\Policies\Microsoft\Edge\CertificateTransparencyEnforcementDisabledForLegacyCas\1 = "sha256//////////////////////w=="

```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: CertificateTransparencyEnforcementDisabledForLegacyCas
  - Exemplo de valor:
``` xml
<array>
  <string>sha256/AAAAAAAAAAAAAAAAAAAAAA==</string>
  <string>sha256//////////////////////w==</string>
</array>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### CertificateTransparencyEnforcementDisabledForUrls
  #### Desabilitar a imposição de Transparência de Certificado para URLs específicas
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Desabilita a aplicação dos requisitos de Transparência do Certificado para as URLs listadas.

Essa política permite que você não divulgue certificados para os nomes de host nas URLs especificadas por meio da Transparência do Certificado. Isso permite usar certificados que, de outra forma, não seriam confiáveis, porque não foram divulgados adequadamente, mas dificulta a detecção de certificados incorretos para esses hosts.

Forme seu padrão de URL de acordo com [https://go.microsoft.com/fwlink/?linkid=2095322](https://go.microsoft.com/fwlink/?linkid=2095322). Como os certificados são válidos para um determinado nome de host, independentemente do esquema, porta ou caminho, apenas a parte do nome do host da URL é considerada. Hosts curinga não são compatíveis.

Se você não configurar essa política, qualquer certificado que deva ser divulgado por meio de Transparência do Certificado será tratado como não confiável se não for divulgado.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Lista de cadeias de caracteres

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: CertificateTransparencyEnforcementDisabledForUrls
  - Nome da GP: Desabilitar a imposição de Transparência de Certificado para URLs específicas
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge\CertificateTransparencyEnforcementDisabledForUrls
  - Caminho (Recomendações): N/A
  - Nome do Valor: 1, 2, 3, ...
  - Tipo de Valor: lista de REG_SZ
  ##### Exemplo de valor:
```
SOFTWARE\Policies\Microsoft\Edge\CertificateTransparencyEnforcementDisabledForUrls\0 = "contoso.com"
SOFTWARE\Policies\Microsoft\Edge\CertificateTransparencyEnforcementDisabledForUrls\1 = ".contoso.com"

```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: CertificateTransparencyEnforcementDisabledForUrls
  - Exemplo de valor:
``` xml
<array>
  <string>contoso.com</string>
  <string>.contoso.com</string>
</array>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### ClearBrowsingDataOnExit
  #### Limpar dados de navegação quando o Microsoft Edge for fechado
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 78 ou posterior

  #### Descrição
  O Microsoft Edge não limpa os dados de navegação por padrão quando é fechado. Os dados de navegação incluem informações inseridas em formulários, senhas e até mesmo os sites visitados.

Se você habilitar esta política, todos os dados de navegação serão excluídos sempre que o Microsoft Edge for fechado.

Se você desabilitar ou não configurar esta política, os usuários poderão configurar a opção Limpar dados de navegação em Configurações.

Se você habilitar esta política, não habilite a política [AllowDeletingBrowserHistory](#allowdeletingbrowserhistory), pois ambas lidam com a exclusão de dados. Se você habilitar ambas, esta política terá precedência e excluirá todos os dados quando o Microsoft Edge for fechado, independentemente de como [AllowDeletingBrowserHistory](#allowdeletingbrowserhistory) estiver configurada.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Sim
  - Atualização de política dinâmica: Não - Requer a reinicialização do navegador

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: ClearBrowsingDataOnExit
  - Nome da GP: Limpar dados de navegação quando o Microsoft Edge for fechado
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): Modelos Administrativos/Microsoft Edge - Configurações Padrão (os usuários podem substituir)/
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): SOFTWARE\Policies\Microsoft\Edge\Recomendações
  - Nome do Valor: ClearBrowsingDataOnExit
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000001
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: ClearBrowsingDataOnExit
  - Exemplo de valor:
``` xml
<true/>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### ClickOnceEnabled
  #### Permitir que os usuários abram arquivos usando o protocolo ClickOnce
  >Versões com Suporte: O Microsoft Edge no Windows desde a versão 78 ou posterior

  #### Descrição
  Permitir que os usuários abram arquivos usando o protocolo ClickOnce. O protocolo ClickOnce permite que sites solicitem que o navegador abra arquivos de uma URL específica usando o manipulador de arquivo ClickOnce no computador ou dispositivo do usuário.

Se você habilitar essa política, os usuários poderão abrir arquivos usando o protocolo ClickOnce. Essa política substitui a configuração de ClickOnce do usuário na página edge://flags/.

Se você desabilitar essa política, os usuários não poderão abrir arquivos usando o protocolo ClickOnce. Em vez disso, o arquivo será salvo no sistema de arquivos usando o navegador. Essa política substitui a configuração de ClickOnce do usuário na página edge://flags/.

Se você não configurar essa política, os usuários não poderão abrir arquivos usando o protocolo ClickOnce. Os usuários terão a opção de habilitar o uso do protocolo ClickOnce com a página edge://flags/.

Desabilitar o ClickOnce pode impedir que os aplicativos ClickOnce (arquivos .application) sejam iniciados corretamente.

Para obter mais informações sobre o ClickOnce, consulte [https://go.microsoft.com/fwlink/?linkid=2103872](https://go.microsoft.com/fwlink/?linkid=2103872) e [https://go.microsoft.com/fwlink/?linkid=2099880](https://go.microsoft.com/fwlink/?linkid=2099880).

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: ClickOnceEnabled
  - Nome da GP: Permitir que os usuários abram arquivos usando o protocolo ClickOnce
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: ClickOnceEnabled
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000000
```


  

  [Voltar ao início](#microsoft-edge---políticas)

  ### CommandLineFlagSecurityWarningsEnabled
  #### Habilitar avisos de segurança para sinalizadores de linha de comando
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 78 ou posterior

  #### Descrição
  Se desabilitada, essa política impedirá que os avisos de segurança sejam exibidos quando o Microsoft Edge for iniciado com sinalizadores de linha de comando potencialmente perigosos.

Se habilitada ou indefinida, os avisos de segurança são exibidos quando esses sinalizadores de linha de comando são usados para iniciar o Microsoft Edge.

Por exemplo, o sinalizador --disable-gpu-sandbox gera este aviso: Você está usando um sinalizador de linha de comando sem suporte: --disable-gpu-sandbox. Isso representa riscos de estabilidade e segurança.

No Windows, essa política está disponível somente em instâncias que fazem parte de um domínio do Microsoft Active Directory ou instâncias do Windows 10 Pro (ou Enterprise) registradas para o gerenciamento de dispositivos.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Não - Requer a reinicialização do navegador

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: CommandLineFlagSecurityWarningsEnabled
  - Nome da GP: Habilitar avisos de segurança para sinalizadores de linha de comando
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: CommandLineFlagSecurityWarningsEnabled
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000001
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: CommandLineFlagSecurityWarningsEnabled
  - Exemplo de valor:
``` xml
<true/>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### ComponentUpdatesEnabled
  #### Habilitar atualizações de componentes no Microsoft Edge
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Se você habilitar ou não configurar essa política, as atualizações de componentes serão habilitadas no Microsoft Edge.

Se você desabilitar essa política ou defini-la como false, as atualizações de componentes serão desabilitadas para todos os componentes no Microsoft Edge.

No entanto, alguns componentes estão isentos dessa política. Isso inclui qualquer componente que não contenha código executável, que não altere significativamente o comportamento do navegador ou que seja crítico para a segurança. Ou seja, as atualizações consideradas "críticas para segurança" ainda serão aplicadas, mesmo que você desabilite essa política.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Não - Requer a reinicialização do navegador

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: ComponentUpdatesEnabled
  - Nome da GP: Habilitar atualizações de componentes no Microsoft Edge
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: ComponentUpdatesEnabled
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000001
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: ComponentUpdatesEnabled
  - Exemplo de valor:
``` xml
<true/>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### ConfigureDoNotTrack
  #### Configurar Não Rastrear
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Especifica se deve-se enviar solicitações Não Rastrear a sites que pedem para rastrear informações. As solicitações Não Rastrear permitem que os sites que você visita saibam que você não deseja que sua atividade de navegação seja rastreada. Por padrão, o Microsoft Edge não envia solicitações Não Rastrear, mas os usuários podem ativar esse recurso para enviá-las.

Se você habilitar essa política, as solicitações Não Rastrear sempre serão enviadas a sites que solicitem rastrear informações.

Se essa política for desabilitada, as solicitações nunca serão enviadas.

Se você não configurar essa política, os usuários poderão optar por enviar ou não essas solicitações.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: ConfigureDoNotTrack
  - Nome da GP: Configurar Não Rastrear
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: ConfigureDoNotTrack
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000000
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: ConfigureDoNotTrack
  - Exemplo de valor:
``` xml
<false/>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### ConfigureOnlineTextToSpeech
  #### Configurar a conversão de texto em fala online
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Defina se o navegador pode aproveitar as fontes de voz para Conversão de Texto em Fala Online, parte dos Serviços Cognitivos do Azure. Essas fontes de voz são de maior qualidade do que as fontes de voz do sistema pré-instaladas.

Se você habilitar ou não configurar essa política, os aplicativos web que usam a API SpeechSynthesis poderão usar as fontes de voz para Conversão de Texto em Fala Online.

Se essa política for desabilitada, as fontes de voz não estarão disponíveis.

Leia mais sobre esse recurso aqui:
API SpeechSynthesis: [https://go.microsoft.com/fwlink/?linkid=2110038](https://go.microsoft.com/fwlink/?linkid=2110038)
Serviços Cognitivos: [https://go.microsoft.com/fwlink/?linkid=2110141](https://go.microsoft.com/fwlink/?linkid=2110141)

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: ConfigureOnlineTextToSpeech
  - Nome da GP: Configurar a conversão de texto em fala online
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: ConfigureOnlineTextToSpeech
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000001
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: ConfigureOnlineTextToSpeech
  - Exemplo de valor:
``` xml
<true/>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### CustomHelpLink
  #### Especificar link de ajuda personalizado
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 79 ou posterior

  #### Descrição
  Especificar um link para o menu Ajuda ou para a tecla F1.

Se você habilitar essa política, o administrador poderá especificar um link para o menu Ajuda ou para a tecla F1.

Se você desabilitar ou não configurar essa política, o link padrão para o menu Ajuda ou para a tecla F1 será usado.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Cadeia de Caracteres

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: CustomHelpLink
  - Nome da GP: Especificar link de ajuda personalizado
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: CustomHelpLink
  - Tipo de Valor: REG_SZ
  ##### Exemplo de valor:
```
"https://go.microsoft.com/fwlink/?linkid=2080734"
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: CustomHelpLink
  - Exemplo de valor:
``` xml
<string>https://go.microsoft.com/fwlink/?linkid=2080734</string>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### DefaultBrowserSettingEnabled
  #### Definir Microsoft Edge como navegador padrão
  >Versões com Suporte: O Microsoft Edge no Windows 7 e Mac desde a versão 77 ou posterior

  #### Descrição
  Configura as verificações de navegador padrão no Microsoft Edge e impede que os usuários as alterem.

Se você habilitar esta política, o Microsoft Edge sempre verificará na inicialização se é o navegador padrão e automaticamente se registrará, se possível.

Se você desabilitar esta política, o Microsoft Edge nunca verificará e desabilitará os controles de usuário para configurar essa opção.

Se você não configurar esta política, o Microsoft Edge permitirá que o usuário controle se ele é o navegador padrão e se deverão ser mostradas notificações de usuário quando ele não for.

Observação para administradores do Windows: esta política só funciona para computadores que executam o Windows 7. Para versões posteriores do Windows, você deve implantar um arquivo de "associações de aplicativos padrão" que torna o Microsoft Edge o manipulador para os protocolos HTTPS e HTTP (e, opcionalmente, o protocolo FTP e os formatos de arquivo, como .html, .htm, .pdf, .svg, .webp). Consulte [https://go.microsoft.com/fwlink/?linkid=2094932](https://go.microsoft.com/fwlink/?linkid=2094932) para obter mais informações.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: DefaultBrowserSettingEnabled
  - Nome da GP: Definir Microsoft Edge como navegador padrão
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: DefaultBrowserSettingEnabled
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000001
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: DefaultBrowserSettingEnabled
  - Exemplo de valor:
``` xml
<true/>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### DeveloperToolsAvailability
  #### Controlar onde as ferramentas de desenvolvedor podem ser usadas
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Controla onde as ferramentas de desenvolvedor podem ser usadas.

Se você definir esta política como 'DeveloperToolsDisallowedForForceInstalledExtensions' (0, o padrão), os usuários poderão acessar as ferramentas de desenvolvedor e o console do JavaScript em geral, mas não no contexto de extensões instaladas pela política corporativa.

Se você definir esta política como 'DeveloperToolsAllowed' (1), os usuários poderão acessar as ferramentas de desenvolvedor e o console do JavaScript em todos os contextos, incluindo as extensões instaladas pela política corporativa.

Se você definir esta política como 'DeveloperToolsDisallowed' (2), os usuários não poderão acessar as ferramentas de desenvolvedor nem inspecionar elementos do site. Os atalhos de teclado e as entradas de menu ou menu de contexto que abrem as ferramentas de desenvolvedor ou o Console do JavaScript são desabilitadas.

* 0 = Bloquear as ferramentas de desenvolvedor em extensões instaladas pela política corporativa e permitir em outros contextos

* 1 = Permitir o uso das ferramentas de desenvolvedor

* 2 = Não permitir o uso das ferramentas de desenvolvedor

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Número inteiro

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: DeveloperToolsAvailability
  - Nome da GP: Controlar onde as ferramentas de desenvolvedor podem ser usadas
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: DeveloperToolsAvailability
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000002
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: DeveloperToolsAvailability
  - Exemplo de valor:
``` xml
<integer>2</integer>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### DirectInvokeEnabled
  #### Permitir que os usuários abram arquivos usando o protocolo DirectInvoke
  >Versões com Suporte: O Microsoft Edge no Windows desde a versão 78 ou posterior

  #### Descrição
  Permitir que os usuários abram arquivos usando o protocolo DirectInvoke. O protocolo DirectInvoke permite que os sites solicitem que o navegador abra arquivos de uma URL específica usando um manipulador de arquivo específico no computador ou dispositivo do usuário.

Se você habilitar ou não configurar essa política, os usuários poderão abrir arquivos usando o protocolo DirectInvoke.

Se você desabilitar essa política, os usuários não poderão abrir arquivos usando o protocolo DirectInvoke. Em vez disso, o arquivo será salvo no sistema de arquivos.

Observação: desabilitar o DirectInvoke pode impedir que certos recursos do Microsoft Office SharePoint Online funcionem conforme o esperado.

Para obter mais informações sobre o DirectInvoke, consulte [https://go.microsoft.com/fwlink/?linkid=2103872](https://go.microsoft.com/fwlink/?linkid=2103872) e [https://go.microsoft.com/fwlink/?linkid=2099871](https://go.microsoft.com/fwlink/?linkid=2099871).

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: DirectInvokeEnabled
  - Nome da GP: Permitir que os usuários abram arquivos usando o protocolo DirectInvoke
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: DirectInvokeEnabled
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000000
```


  

  [Voltar ao início](#microsoft-edge---políticas)

  ### Disable3DAPIs
  #### Desabilitar o suporte para APIs de gráficos 3D
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Impeça que páginas da Web acessem a unidade de processamento gráfico (GPU). Especificamente, as páginas da Web não podem acessar a API WebGL e os plug-ins não podem usar a API Pepper 3D.

Se você não configurar ou desabilitar essa política, ela permitirá que as páginas da Web usem a API WebGL e os plug-ins usem a API Pepper 3D. O Microsoft Edge pode, por padrão, ainda exigir que os argumentos da linha de comando sejam passados para usar essas APIs.

Se a política [HardwareAccelerationModeEnabled](#hardwareaccelerationmodeenabled) estiver definida como false, a configuração da política [Disable3DAPIs](#disable3dapis) será ignorada. É o equivalente a definir a política [Disable3DAPIs](#disable3dapis) como true.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: Disable3DAPIs
  - Nome da GP: Desabilitar o suporte para APIs de gráficos 3D
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: Disable3DAPIs
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000000
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: Disable3DAPIs
  - Exemplo de valor:
``` xml
<false/>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### DisableScreenshots
  #### Desabilitar as capturas de tela
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Controla se os usuários podem tirar capturas de tela da página do navegador.

Se estiver habilitada, o usuário não poderá tirar capturas de tela usando atalhos do teclado ou APIs de extensão.

Se estiver desabilitada ou você não configurar a política, os usuários poderão tirar capturas de tela.

Observe que esta política controla as capturas de tela tiradas de dentro do próprio navegador. Mesmo se você habilitar esta política, os usuários ainda poderão tirar capturas de tela usando algum método fora do navegador (por exemplo, usando um recurso do sistema operacional ou outro aplicativo).

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: DisableScreenshots
  - Nome da GP: Desabilitar as capturas de tela
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: DisableScreenshots
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000001
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: DisableScreenshots
  - Exemplo de valor:
``` xml
<true/>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### DiskCacheDir
  #### Definir diretório de cache de disco
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Configura o diretório a ser usado para armazenar arquivos armazenados em cache.

Se você habilitar essa política, o Microsoft Edge usará o diretório fornecido, independentemente de o usuário ter especificado o sinalizador "--disk-cache-dir". Para evitar a perda de dados ou outros erros inesperados, não configure essa política para o diretório raiz de um volume ou para um diretório usado para outros fins, pois o Microsoft Edge gerenciará seu conteúdo.

Consulte [https://go.microsoft.com/fwlink/?linkid=2095041](https://go.microsoft.com/fwlink/?linkid=2095041) para obter uma lista de variáveis que você pode usar ao especificar diretórios e caminhos.

Se você não configurar essa política, o diretório de cache padrão será usado, e os usuários poderão substituir o padrão pelo sinalizador de linha de comando "--disk-cache-dir".

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Não - Requer a reinicialização do navegador

  #### Tipo de Dados:
  Cadeia de Caracteres

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: DiskCacheDir
  - Nome da GP: Definir diretório de cache de disco
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: DiskCacheDir
  - Tipo de Valor: REG_SZ
  ##### Exemplo de valor:
```
"${user_home}/Edge_cache"
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: DiskCacheDir
  - Exemplo de valor:
``` xml
<string>${user_home}/Edge_cache</string>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### DiskCacheSize
  #### Definir o tamanho do cache de disco, em bytes
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Configura o tamanho do cache, em bytes, usado para armazenar arquivos no disco.

Se você habilitar esta política, o Microsoft Edge usará o tamanho de cache fornecido, independentemente de o usuário ter especificado ou não o sinalizador "--disk-cache-size". O valor especificado nesta política não é um limite rígido, mas uma sugestão ao sistema de cache; qualquer valor abaixo de alguns megabytes é muito pequeno e será arredondado para um mínimo razoável.

Se você definir o valor desta política como 0, será usado o tamanho de cache padrão, e os usuários não poderão alterá-lo.

Se você não configurar esta política, será usado o tamanho padrão, mas os usuários poderão substituí-lo pelo sinalizador "--disk-cache-size".

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Não - Requer a reinicialização do navegador

  #### Tipo de Dados:
  Número inteiro

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: DiskCacheSize
  - Nome da GP: Definir o tamanho do cache de disco, em bytes
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: DiskCacheSize
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x06400000
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: DiskCacheSize
  - Exemplo de valor:
``` xml
<integer>104857600</integer>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### DownloadDirectory
  #### Definir diretório de download
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Configures the directory to use when downloading files.

If you enable this policy, Microsoft Edge uses the provided directory regardless of whether the user has specified one or chosen to be prompted for download location every time. See [https://go.microsoft.com/fwlink/?linkid=2095041](https://go.microsoft.com/fwlink/?linkid=2095041) for a list of variables that can be used.

If you disable or don't configure this policy, the default download directory is used, and the user can change it.

If you set an invalid path, Microsoft Edge will default to the user's default download directory.

If the folder specified by the path doesn't exist, the download will trigger a prompt that asks the user where they want to save their download.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Sim
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Cadeia de Caracteres

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: DownloadDirectory
  - Nome da GP: Definir diretório de download
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): Modelos Administrativos/Microsoft Edge - Configurações Padrão (os usuários podem substituir)/
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): SOFTWARE\Policies\Microsoft\Edge\Recomendações
  - Nome do Valor: DownloadDirectory
  - Tipo de Valor: REG_SZ
  ##### Exemplo de valor:
```
"
      Linux-based OSes (including Mac): /home/${user_name}/Downloads
      Windows: C:\Users\${user_name}\Downloads"
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: DownloadDirectory
  - Exemplo de valor:
``` xml
<string>
      Linux-based OSes (including Mac): /home/${user_name}/Downloads
      Windows: C:\Users\${user_name}\Downloads</string>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### DownloadRestrictions
  #### Permitir restrições de download
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Configura o tipo de downloads que o Microsoft Edge bloqueia completamente, sem permitir que os usuários substituam a decisão de segurança.

Defina "Bloquear downloads perigosos" (1) para permitir todos os downloads, exceto os que contenham avisos do Microsoft Defender SmartScreen.

Defina "Bloquear downloads potencialmente perigosos" (2) para permitir todos os downloads, exceto os que tenham avisos de downloads potencialmente perigosos do Microsoft Defender SmartScreen.

Defina "Bloquear todos os downloads" (3) para bloquear todos os downloads.

Se você não configurar essa política ou definir a opção 'Sem restrições especiais' (0), os downloads passarão por restrições de segurança comuns com base nos resultados da análise do Microsoft Defender SmartScreen.

Observe que essas restrições são aplicáveis a downloads do conteúdo da página da Web, bem como à opção de menu de contexto "link de download...". Essas restrições não se aplicam ao salvamento ou ao download da página exibida no momento, nem se aplicam à opção Salvar como PDF nas opções de impressão.

Consulte [https://go.microsoft.com/fwlink/?linkid=2094934](https://go.microsoft.com/fwlink/?linkid=2094934) para obter mais informações sobre o Microsoft Defender SmartScreen.

* 0 = Sem restrições especiais

* 1 = Bloquear downloads perigosos

* 2 = Bloquear downloads potencialmente perigosos

* 3 = Bloquear todos os downloads

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Sim
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Número inteiro

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: DownloadRestrictions
  - Nome da GP: Permitir restrições de download
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): Modelos Administrativos/Microsoft Edge - Configurações Padrão (os usuários podem substituir)/
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): SOFTWARE\Policies\Microsoft\Edge\Recomendações
  - Nome do Valor: DownloadRestrictions
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000002
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: DownloadRestrictions
  - Exemplo de valor:
``` xml
<integer>2</integer>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### EdgeCollectionsEnabled
  #### Habilitar o recurso Coleções
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 78 ou posterior

  #### Descrição
  Permite que os usuários acessem o recurso Coleções, onde eles podem coletar, organizar, compartilhar e exportar conteúdo de forma mais eficiente e com a integração do Office.

Se você habilitar ou não configurar essa política, os usuários poderão acessar e usar o recurso Coleções no Microsoft Edge.

Se você desabilitar essa política, os usuários não poderão acessar e usar Coleções no Microsoft Edge.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Não - Requer a reinicialização do navegador

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: EdgeCollectionsEnabled
  - Nome da GP: Habilitar o recurso Coleções
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: EdgeCollectionsEnabled
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000001
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: EdgeCollectionsEnabled
  - Exemplo de valor:
``` xml
<true/>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### EditFavoritesEnabled
  #### Permite que os usuários editem os favoritos
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Habilite essa política para permitir que os usuários adicionem, removam e modifiquem os favoritos. Esse é o comportamento padrão se você não configurar a política.

Desabilite essa política para impedir que os usuários adicionem, removam ou modifiquem os favoritos. Eles ainda poderão usar os favoritos existentes.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: EditFavoritesEnabled
  - Nome da GP: Permite que os usuários editem os favoritos
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: EditFavoritesEnabled
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000000
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: EditFavoritesEnabled
  - Exemplo de valor:
``` xml
<false/>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### EnableDeprecatedWebPlatformFeatures
  #### Reabilitar os recursos preteridos da plataforma da Web por um tempo limitado
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Especifica uma lista de recursos da plataforma da Web preteridos que serão temporariamente habilitados novamente.

Essa política permite que você habilite novamente os recursos preteridos da plataforma da Web por tempo limitado. Os recursos são identificados por uma marca de cadeia de caracteres.

Se você não configurar essa política, se a lista estiver vazia ou se um recurso não corresponder a uma das marcas de cadeia de caracteres com suporte, todos os recursos da plataforma da Web preteridos permanecerão desabilitados.

Embora a política propriamente dita tenha suporte nas plataformas acima, o recurso que ela estiver habilitando talvez não esteja disponível em todas as plataformas. Nem todos os recursos da plataforma da Web preteridos podem ser habilitados novamente. Somente os explicitamente listados abaixo podem ser habilitados novamente e apenas por um período de tempo limitado, que difere por recurso. Você pode examinar o intuito subjacente às alterações de recurso da plataforma da Web em https://bit.ly/blinkintents.

O formato geral da marca da cadeia de caracteres é [DeprecatedFeatureName]_EffectiveUntil[yyyymmdd].

* "ExampleDeprecatedFeature_EffectiveUntil20080902" = Habilitar API ExampleDeprecatedFeature em 2008/09/02

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Lista de cadeias de caracteres

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: EnableDeprecatedWebPlatformFeatures
  - Nome da GP: Reabilitar os recursos preteridos da plataforma da Web por um tempo limitado
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge\EnableDeprecatedWebPlatformFeatures
  - Caminho (Recomendações): N/A
  - Nome do Valor: 1, 2, 3, ...
  - Tipo de Valor: lista de REG_SZ
  ##### Exemplo de valor:
```
SOFTWARE\Policies\Microsoft\Edge\EnableDeprecatedWebPlatformFeatures\0 = "ExampleDeprecatedFeature_EffectiveUntil20080902"

```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: EnableDeprecatedWebPlatformFeatures
  - Exemplo de valor:
``` xml
<array>
  <string>ExampleDeprecatedFeature_EffectiveUntil20080902</string>
</array>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### EnableDomainActionsDownload
  #### Habilitar o download de ações de domínio da Microsoft
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  No Microsoft Edge, as Ações de Domínio representam uma série de recursos de compatibilidade que ajudam o navegador a funcionar corretamente na Web.

A Microsoft mantém uma lista de ações a serem executadas em determinados domínios por razões de compatibilidade. Por exemplo, o navegador pode substituir a sequência do Agente do Usuário em um site se esse site for corrompido em razão da nova sequência do Agente do Usuário no Microsoft Edge. Cada uma dessas ações deve ser temporária enquanto a Microsoft tenta resolver o problema com o proprietário do site.

Quando o navegador é iniciado e depois periodicamente, o navegador contatará o Serviço de Experimentação e Configuração que contém a lista mais atualizada de ações de compatibilidade a serem executadas. Essa lista é salva localmente após ser recuperada, de forma que as solicitações posteriores só atualizarão a lista se a cópia do servidor tiver sido alterada.

Se você habilitar essa política, a lista de Ações de Domínio continuará a ser baixada do Serviço de Experimentação e Configuração.

Se você desabilitar essa política, a lista de Ações de Domínio não será mais baixada do Serviço de Experimentação e Configuração.

Se você não configurar essa política, a lista de Ações de Domínio continuará a ser baixada do Serviço de Experimentação e Configuração.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: EnableDomainActionsDownload
  - Nome da GP: Habilitar o download de ações de domínio da Microsoft
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: EnableDomainActionsDownload
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000001
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: EnableDomainActionsDownload
  - Exemplo de valor:
``` xml
<true/>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### EnableOnlineRevocationChecks
  #### Habilitar verificações de OCSP/CRL online
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  As verificações de revogação online não fornecem um benefício de segurança significativo e são desabilitadas por padrão.

Se você habilitar essa política, o Microsoft Edge executará verificações de OCSP/CRL online com falha leve. "Falha leve" significa que, se não for possível acessar o servidor de revogação, o certificado será considerado válido.

Se você desabilitar a política ou não configurá-la, o Microsoft Edge não executará verificações de revogação online.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: EnableOnlineRevocationChecks
  - Nome da GP: Habilitar verificações de OCSP/CRL online
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: EnableOnlineRevocationChecks
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000000
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: EnableOnlineRevocationChecks
  - Exemplo de valor:
``` xml
<false/>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### EnterpriseHardwarePlatformAPIEnabled
  #### Permitir que extensões gerenciadas usem a API da Plataforma de Hardware Corporativo
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 78 ou posterior

  #### Descrição
  Quando essa política estiver habilitada, as extensões instaladas pela política da empresa têm permissão para usar a API da Plataforma de Hardware Empresarial.
Quando essa política está definida como desabilitada ou não está definida, nenhuma extensão tem permissão para usar a API da Plataforma de Hardware Empresarial.
Essa política também se aplica às extensões de componente.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: EnterpriseHardwarePlatformAPIEnabled
  - Nome da GP: Permitir que extensões gerenciadas usem a API da Plataforma de Hardware Corporativo
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: EnterpriseHardwarePlatformAPIEnabled
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000001
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: EnterpriseHardwarePlatformAPIEnabled
  - Exemplo de valor:
``` xml
<true/>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### ExperimentationAndConfigurationServiceControl
  #### Controlar a comunicação com o Serviço de Configuração e Experimentação
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  No Microsoft Edge, o Serviço de Configuração e Experimentação é usado para implantar a carga de Configuração e Experimentação.

A carga de Experimentação consiste em uma lista de recursos de desenvolvimento antecipados que a Microsoft está habilitando para testes e comentários.

A carga de configuração consiste em uma lista de configurações que a Microsoft deseja implantar no Microsoft Edge para otimizar a experiência do usuário. Por exemplo, a carga de configuração pode especificar a frequência com que o Microsoft Edge envia solicitações para o Serviço de Configuração e Experimentação para recuperar a carga mais recente.

Se você definir essa política como o modo "Recuperar configurações e experimentos", a carga total será baixada do Serviço de Configuração e Experimentação. Isso inclui as cargas de configuração e experimentação.

Se você definir essa política como o modo "Recuperar somente configurações", somente a carga de configuração será entregue.

Se você definir essa política como o modo "Desabilitar a comunicação com o Serviço de Configuração e Experimentação", a comunicação com o Serviço de Configuração e Experimentação será interrompida completamente.

Se você não configurar essa política, em um dispositivo gerenciado nos canais Estável e Beta, o comportamento será o mesmo que o modo "Recuperar configurações e experimentos".

Se você não configurar essa política, em um dispositivo não gerenciado, o comportamento será o mesmo que o modo "Recuperar configurações e experimentos".

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Número inteiro

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: ExperimentationAndConfigurationServiceControl
  - Nome da GP: Controlar a comunicação com o Serviço de Configuração e Experimentação
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: ExperimentationAndConfigurationServiceControl
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000002
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: ExperimentationAndConfigurationServiceControl
  - Exemplo de valor:
``` xml
<integer>2</integer>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### ExternalProtocolDialogShowAlwaysOpenCheckbox
  #### Mostrar uma caixa de seleção "Sempre abrir" na caixa de diálogo de protocolo externo
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 79 ou posterior

  #### Descrição
  Essa política controla se a caixa de seleção "Sempre abrir" é mostrada em prompts de confirmação de inicialização do protocolo externo.

Se você definir essa política como True, quando um prompt de confirmação de protocolo externo for exibido, o usuário poderá selecionar "Sempre abrir". O usuário não verá prompts de confirmação desse protocolo no futuro.

Se você definir essa política como False, ou se a política for indefinida, a caixa de seleção "Sempre abrir" não será exibida. O usuário será solicitado a fornecer uma confirmação sempre que um protocolo externo for chamado.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Não - Requer a reinicialização do navegador

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: ExternalProtocolDialogShowAlwaysOpenCheckbox
  - Nome da GP: Mostrar uma caixa de seleção "Sempre abrir" na caixa de diálogo de protocolo externo
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: ExternalProtocolDialogShowAlwaysOpenCheckbox
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000001
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: ExternalProtocolDialogShowAlwaysOpenCheckbox
  - Exemplo de valor:
``` xml
<true/>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### FavoritesBarEnabled
  #### Habilitar barra de favoritos
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Habilita ou desabilita a barra de favoritos.

Se você habilitar essa política, os usuários verão a barra de favoritos.

Se você desabilitar essa política, os usuários não verão a barra de favoritos.

Se essa política não estiver configurada, o usuário pode optar por usar a barra de favoritos ou não.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Sim
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: FavoritesBarEnabled
  - Nome da GP: Habilitar barra de favoritos
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): Modelos Administrativos/Microsoft Edge - Configurações Padrão (os usuários podem substituir)/
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): SOFTWARE\Policies\Microsoft\Edge\Recomendações
  - Nome do Valor: FavoritesBarEnabled
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000001
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: FavoritesBarEnabled
  - Exemplo de valor:
``` xml
<true/>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### ForceBingSafeSearch
  #### Aplicar a Pesquisa Segura do Bing
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Certifique-se de que as consultas de pesquisa na Web do Bing sejam feitas com a Pesquisa Segura configurada com o valor especificado. Os usuários não podem alterar essa configuração.

Se você configurar esta política como "Desativada", a Pesquisa Segura no Bing voltará para o valor de bing.com.

Se você configurar esta política como "Moderada", a configuração moderada será usada na Pesquisa Segura. A configuração moderada filtra vídeos e imagens de teor adulto, mas não textos dos resultados da pesquisa.

Se você configurar esta política como "Estrita", a configuração estrita será usada na Pesquisa Segura. A configuração estrita filtros de texto, imagens e vídeos.

Se você desabilitar esta política ou não configurá-la, a Pesquisa Segura no Bing não será imposta, e os usuários poderão definir o valor que desejarem em bing.com.

* 0 = Não configurar restrições de pesquisa no Bing

* 1 = Configurar restrições moderadas de pesquisa no Bing

* 2 = Configurar restrições estritas de pesquisa no Bing

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Número inteiro

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: ForceBingSafeSearch
  - Nome da GP: Aplicar a Pesquisa Segura do Bing
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: ForceBingSafeSearch
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000000
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: ForceBingSafeSearch
  - Exemplo de valor:
``` xml
<integer>0</integer>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### ForceEphemeralProfiles
  #### Habilitar o uso de perfis efêmeros
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Controla se os perfis de usuário são alternados para o modo efêmero. Um perfil efêmero é criado quando uma sessão é iniciada, é excluído quando a sessão é encerrada e é associado ao perfil original do usuário.

Se você habilitar essa política, os perfis serão executados no modo efêmero. Isso permite que os usuários trabalhem em seus próprios dispositivos sem salvar dados de navegação nesses dispositivos. Se você habilitar essa política como uma política do sistema operacional (usando o GPO no Windows, por exemplo), ela se aplicará a todos os perfis do sistema.

Se você desabilitar essa política ou não configurá-la, os usuários receberão seus perfis regulares quando entrarem no navegador.

No modo efêmero, os dados do perfil são salvos em disco apenas pela duração da sessão do usuário. Os recursos, como o histórico do navegador, as extensões e seus dados, dados da Web, como cookies e bancos de dados da Web, não são salvos depois que o navegador é fechado. Isso não impede que o usuário baixe manualmente os dados em disco ou salve páginas ou as imprima. Se o usuário tiver habilitado a sincronização, todos os dados serão preservados nas contas de sincronização da mesma forma que os perfis regulares. Os usuários também poderão usar a navegação InPrivate no modo efêmero, a menos que você desabilite isso explicitamente.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Não - Requer a reinicialização do navegador

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: ForceEphemeralProfiles
  - Nome da GP: Habilitar o uso de perfis efêmeros
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: ForceEphemeralProfiles
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000001
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: ForceEphemeralProfiles
  - Exemplo de valor:
``` xml
<true/>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### ForceGoogleSafeSearch
  #### Forçar a Pesquisa Segura do Google
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Força a realização de consultas na Pesquisa do Google na Web com a Pesquisa Segura definida como ativa e impede que os usuários alterem essa configuração.

Se você habilitar essa política, a Pesquisa Segura na Pesquisa do Google sempre ficará ativa.

Se você desabilitar essa política ou não configurá-la, a Pesquisa Segura não será imposta na Pesquisa do Google.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: ForceGoogleSafeSearch
  - Nome da GP: Forçar a Pesquisa Segura do Google
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: ForceGoogleSafeSearch
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000000
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: ForceGoogleSafeSearch
  - Exemplo de valor:
``` xml
<false/>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### ForceNetworkInProcess
  #### Aplicar o código de rede a ser executado no processo do navegador
  >Versões com Suporte: O Microsoft Edge no Windows desde a versão 78 ou posterior

  #### Descrição
  Essa política força a execução do código de rede no processo do navegador.

Essa política é desabilitada por padrão. Se habilitada, os usuários ficam vulneráveis a problemas de segurança depois que o processo de rede estiver em área restrita.

Essa política tem o objetivo de permitir que as empresas tenham a oportunidade de migrar para softwares de terceiros que não dependam de desligamento de APIs de rede. Os servidores proxy são recomendados na aplicação de patchs de APIs de LSPs e Win32.

Se essa política não for configurada, o código de rede poderá ser executado fora do processo do navegador, dependendo de avaliações de campo do experimento NetworkService.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Não - Requer a reinicialização do navegador

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: ForceNetworkInProcess
  - Nome da GP: Aplicar o código de rede a ser executado no processo do navegador
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: ForceNetworkInProcess
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000000
```


  

  [Voltar ao início](#microsoft-edge---políticas)

  ### ForceYouTubeRestrict
  #### Aplicar o modo restrito mínimo do YouTube
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Aplica um modo restrito mínimo no YouTube e impede que os usuários escolham um modo menos restrito.

Defina como estrito (2) para aplicar o modo restrito estrito no YouTube.

Defina como moderado (1) para fazer com que o usuário use apenas o modo restrito moderado e o modo restrito estrito no YouTube. Eles não podem desabilitar o modo restrito.

Defina como desativado (0) ou não configure essa política para não aplicar o modo restrito no YouTube. Políticas externas, como políticas do YouTube, ainda podem aplicar o modo restrito.

* 0 = Não aplicar o modo restrito no YouTube

* 1 = Aplicar pelo menos o modo restrito moderado no YouTube

* 2 = Aplicar o modo restrito estrito ao YouTube

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Número inteiro

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: ForceYouTubeRestrict
  - Nome da GP: Aplicar o modo restrito mínimo do YouTube
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: ForceYouTubeRestrict
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000000
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: ForceYouTubeRestrict
  - Exemplo de valor:
``` xml
<integer>0</integer>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### FullscreenAllowed
  #### Permitir modo de tela inteira
  >Versões com Suporte: O Microsoft Edge no Windows desde a versão 77 ou posterior

  #### Descrição
  Definir a disponibilidade do modo de tela inteira - toda a interface do usuário do Microsoft Edge está oculta e apenas o conteúdo da Web está visível.

Se você habilitar essa política ou não configurá-la, o usuário, os aplicativos e as extensões com as permissões apropriadas poderão entrar no modo tela inteira.

Se essa política for desabilitada, os usuários, os aplicativos e as extensões não poderão entrar no modo tela inteira.

Abrir o Microsoft Edge no modo de quiosque usando a linha de comando não está disponível quando o modo de tela inteira está desabilitado.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: FullscreenAllowed
  - Nome da GP: Permitir modo de tela inteira
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: FullscreenAllowed
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000001
```


  

  [Voltar ao início](#microsoft-edge---políticas)

  ### GoToIntranetSiteForSingleWordEntryInAddressBar
  #### Forçar a navegação direta em site da intranet, em vez de pesquisar em entradas de palavras únicas na Barra de Endereços
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 78 ou posterior

  #### Descrição
  Se você habilitar essa política, o primeiro resultado da sugestão automática na lista de sugestões da barra de endereços navegará para sites da intranet se o texto digitado na barra de endereços for uma única palavra sem pontuação.

A navegação padrão ao digitar uma única palavra sem pontuação conduzirá uma navegação para um site da intranet correspondente à palavra digitada.

Se você habilitar essa política, o segundo resultado da sugestão automática na lista de sugestões da barra de endereços conduzirá uma pesquisa na Web exatamente como ele foi digitado, contanto que esse texto seja uma única palavra sem pontuação. O provedor de pesquisa padrão será usado, a menos que uma política que impeça a pesquisa na Web também esteja habilitada.

Os dois efeitos da habilitação dessa política são:

A navegação para sites em resposta a consultas com uma única palavra que normalmente se resolveriam em um item de histórico não acontecerá mais. Em vez disso, o navegador tentará navegar para sites internos que talvez nem existam na intranet de uma organização. Isso resultará no erro 404.

Termos de pesquisa comuns de uma única palavra exigirão a seleção manual de sugestões de pesquisa para conduzir uma pesquisa adequadamente.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: GoToIntranetSiteForSingleWordEntryInAddressBar
  - Nome da GP: Forçar a navegação direta em site da intranet, em vez de pesquisar em entradas de palavras únicas na Barra de Endereços
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: GoToIntranetSiteForSingleWordEntryInAddressBar
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000000
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: GoToIntranetSiteForSingleWordEntryInAddressBar
  - Exemplo de valor:
``` xml
<false/>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### HSTSPolicyBypassList
  #### Configurar a lista de nomes que ignorarão a verificação de política HSTS
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 79 ou posterior

  #### Descrição
  Os nomes de host especificados nesta lista serão isentos da verificação de política HSTS que poderiam potencialmente atualizar solicitações de "http://" para "https://". Somente nomes de host de rótulo único são permitidos nesta política. Os nomes de host devem ser canônicos. Todos os IDNs devem ser convertidos em seu formato de rótulo A, e todas as letras ASCII devem ser minúsculas. Esta política aplica-se somente aos nomes de host específicos especificados; ela não se aplica aos subdomínios dos nomes na lista.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Não - Requer a reinicialização do navegador

  #### Tipo de Dados:
  Lista de cadeias de caracteres

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: HSTSPolicyBypassList
  - Nome da GP: Configurar a lista de nomes que ignorarão a verificação de política HSTS
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge\HSTSPolicyBypassList
  - Caminho (Recomendações): N/A
  - Nome do Valor: 1, 2, 3, ...
  - Tipo de Valor: lista de REG_SZ
  ##### Exemplo de valor:
```
SOFTWARE\Policies\Microsoft\Edge\HSTSPolicyBypassList\0 = "meet"

```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: HSTSPolicyBypassList
  - Exemplo de valor:
``` xml
<array>
  <string>meet</string>
</array>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### HardwareAccelerationModeEnabled
  #### Usar aceleração de hardware quando disponível
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Especifique para usar a aceleração de hardware, se ela estiver disponível. Se você habilitar essa política ou não configurá-la, a aceleração de hardware será habilitada, a menos que um recurso GPU esteja explicitamente bloqueado.

Se essa política for desabilitada, a aceleração de hardware será desabilitada.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Não - Requer a reinicialização do navegador

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: HardwareAccelerationModeEnabled
  - Nome da GP: Usar aceleração de hardware quando disponível
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: HardwareAccelerationModeEnabled
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000001
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: HardwareAccelerationModeEnabled
  - Exemplo de valor:
``` xml
<true/>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### ImportAutofillFormData
  #### Permitir importação de dados de formulário de autopreenchimento
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Permite que os usuários importem dados de formulário de AutoPreenchimento de outro navegador para o Microsoft Edge.

Se você habilitar essa política, a opção para importar manualmente dados de formulário de AutoPreenchimento será selecionada automaticamente.

Se essa política for desabilitada, os dados de formulário de AutoPreenchimento não serão importados na primeira execução, e os usuários não poderão importá-los manualmente.

Se você não configurar essa política, os dados de autopreenchimento serão importados na primeira execução, e os usuários poderão optar por importar esses dados manualmente durante sessões de navegação posteriores.

Você pode definir essa política como uma recomendação. Isso significa que o Microsoft Edge importará os dados de AutoPreenchimento na primeira execução, mas os usuários poderão marcar ou desmarcar a opção **dados de AutoPreenchimento** durante a importação manual.

**Observação**: essa política atualmente gerencia a importação do Google Chrome (no Windows 7, 8 e 10 e no macOS).

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Sim
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: ImportAutofillFormData
  - Nome da GP: Permitir importação de dados de formulário de autopreenchimento
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): Modelos Administrativos/Microsoft Edge - Configurações Padrão (os usuários podem substituir)/
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): SOFTWARE\Policies\Microsoft\Edge\Recomendações
  - Nome do Valor: ImportAutofillFormData
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000001
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: ImportAutofillFormData
  - Exemplo de valor:
``` xml
<true/>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### ImportBrowserSettings
  #### Permitir a importação das configurações do navegador
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 78 ou posterior

  #### Descrição
  Permite que os usuários importem configurações de outro navegador para o Microsoft Edge.

Se você habilitar essa política, a caixa de seleção **Configurações do navegador** será marcada automaticamente na caixa de diálogo **Importar dados do navegador**.

Se você desabilitar essa política, as configurações do navegador não serão importadas na primeira execução, e os usuários não poderão importá-las manualmente.

Se você não configurar essa política, as configurações do navegador serão importadas na primeira execução, e os usuários poderão optar por importá-las manualmente durante sessões de navegação posteriores.

Você também pode definir essa política como uma recomendação. Isso significa que o Microsoft Edge importará as configurações na primeira execução, mas os usuários poderão marcar ou desmarcar a opção ** configurações do navegador** durante a importação manual.

**Observação**: essa política atualmente gerencia a importação do Google Chrome (no Windows 7, 8 e 10 e no macOS).

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Sim
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: ImportBrowserSettings
  - Nome da GP: Permitir a importação das configurações do navegador
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): Modelos Administrativos/Microsoft Edge - Configurações Padrão (os usuários podem substituir)/
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): SOFTWARE\Policies\Microsoft\Edge\Recomendações
  - Nome do Valor: ImportBrowserSettings
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000001
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: ImportBrowserSettings
  - Exemplo de valor:
``` xml
<true/>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### ImportFavorites
  #### Permitir importação de favoritos
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Permite que os usuários importem os favoritos de outro navegador para o Microsoft Edge.

Se você habilitar essa política, a caixa de seleção **Favoritos** será selecionada automaticamente na caixa de diálogo **Importar dados do navegador**.

Se você desabilitar essa política for desabilitada, os favoritos não serão importados na primeira execução, e os usuários não poderão importar esses dados manualmente.

Se você não configurar essa política, os favoritos serão importados na primeira execução, e os usuários poderão optar por importá-los manualmente durante as sessões de navegação posteriores.

Você também pode definir essa política como uma recomendação. Isso significa que o Microsoft Edge importa os favoritos na primeira execução, mas os usuários poderão marcar ou desmarcar a opção **favoritos** durante a importação manual.

**Observação**: essa política gerencia atualmente a importação dos navegadores Internet Explorer (no Windows 7, 8 e 10), Google Chrome (no Windows 7, 8 e 10 e macOS) e Apple Safari (macOS).

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Sim
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: ImportFavorites
  - Nome da GP: Permitir importação de favoritos
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): Modelos Administrativos/Microsoft Edge - Configurações Padrão (os usuários podem substituir)/
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): SOFTWARE\Policies\Microsoft\Edge\Recomendações
  - Nome do Valor: ImportFavorites
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000001
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: ImportFavorites
  - Exemplo de valor:
``` xml
<true/>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### ImportHistory
  #### Permitir a importação do histórico de navegação
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Permite que os usuários importem o histórico de navegação de outro navegador para o Microsoft Edge.

Se você habilitar essa política, a caixa de seleção **Histórico de navegação** será selecionada automaticamente na caixa de diálogo **Importar dados do navegador**.

Se essa política for desabilitada, os dados do histórico de navegação não serão importados na primeira execução, e os usuários não poderão importar esses dados manualmente.

Se você não configurar essa política, os dados de histórico de navegação serão importados na primeira execução, e os usuários poderão optar por importá-los manualmente durante sessões de navegação posteriores.

Você também pode definir essa política como uma recomendação. Isso significa que o Microsoft Edge importa o histórico de navegação na primeira execução, mas os usuários poderão marcar ou desmarcar a opção **histórico** durante a importação manual.

**Observação**: essa política gerencia atualmente a importação dos navegadores Internet Explorer (no Windows 7, 8 e 10), Google Chrome (no Windows 7, 8 e 10 e macOS) e Apple Safari (macOS).

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Sim
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: ImportHistory
  - Nome da GP: Permitir a importação do histórico de navegação
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): Modelos Administrativos/Microsoft Edge - Configurações Padrão (os usuários podem substituir)/
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): SOFTWARE\Policies\Microsoft\Edge\Recomendações
  - Nome do Valor: ImportHistory
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000001
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: ImportHistory
  - Exemplo de valor:
``` xml
<true/>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### ImportHomepage
  #### Permitir a importação das configurações da home page
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Permite que os usuários importem a configuração da home page de outro navegador para o Microsoft Edge.

Se você habilitar essa política, a opção para importar manualmente a configuração da home page será selecionada automaticamente.

Se essa política for desabilitada, a configuração da home page não será importada na primeira execução, e os usuários não poderão importá-la manualmente.

Se você não configurar essa política, a configuração da home page será importada na primeira execução, e os usuários poderão optar por importar esses dados manualmente durante sessões de navegação posteriores.

Você pode definir essa política como uma recomendação. Isso significa que o Microsoft Edge importa a configuração da home page na primeira execução, mas os usuários poderão marcar ou desmarcar a opção **home page** durante a importação manual.

**Observação**: essa política atualmente gerencia a importação do Internet Explorer (no Windows 7, 8 e 10).

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: ImportHomepage
  - Nome da GP: Permitir a importação das configurações da home page
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: ImportHomepage
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000001
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: ImportHomepage
  - Exemplo de valor:
``` xml
<true/>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### ImportOpenTabs
  #### Permitir importação de guias abertas
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 79 ou posterior

  #### Descrição
  Permite que os usuários importem configurações de outro navegador para o Microsoft Edge.

Se você habilitar essa política, a caixa de seleção **Configurações do navegador** será marcada automaticamente na caixa de diálogo **Importar dados do navegador**.

Se você desabilitar essa política, as configurações do navegador não serão importadas na primeira execução, e os usuários não poderão importá-las manualmente.

Se você não configurar essa política, as configurações do navegador serão importadas na primeira execução, e os usuários poderão optar por importá-las manualmente durante sessões de navegação posteriores.

Você também pode definir essa política como uma recomendação. Isso significa que o Microsoft Edge importará as configurações na primeira execução, mas os usuários poderão marcar ou desmarcar a opção ** configurações do navegador** durante a importação manual.

**Observação**: essa política atualmente gerencia a importação do Google Chrome (no Windows 7, 8 e 10 e no macOS).

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Sim
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: ImportOpenTabs
  - Nome da GP: Permitir importação de guias abertas
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): Modelos Administrativos/Microsoft Edge - Configurações Padrão (os usuários podem substituir)/
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): SOFTWARE\Policies\Microsoft\Edge\Recomendações
  - Nome do Valor: ImportOpenTabs
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000001
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: ImportOpenTabs
  - Exemplo de valor:
``` xml
<true/>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### ImportPaymentInfo
  #### Permitir importação de informações de pagamento
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Permite que os usuários importem informações de pagamento de outro navegador para o Microsoft Edge.

Se você habilitar essa política, a caixa de seleção **informações de pagamento** será selecionada automaticamente na caixa de diálogo **Importar dados do navegador**.

Se essa política for desabilitada, as informações de pagamento não serão importadas na primeira execução, e os usuários não poderão importá-las manualmente.

Se você não configurar essa política, as informações de pagamento serão importadas na primeira execução, e os usuários poderão optar por importá-las manualmente durante sessões de navegação posteriores.

Você pode definir essa política como uma recomendação. Isso significa que o Microsoft Edge importa informações de pagamento na primeira execução, mas os usuários poderão marcar ou desmarcar a opção **informações de pagamento** durante a importação manual.

**Observação:** essa política atualmente gerencia a importação do Google Chrome (no Windows 7, 8 e 10 e no macOS).

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Sim
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: ImportPaymentInfo
  - Nome da GP: Permitir importação de informações de pagamento
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): Modelos Administrativos/Microsoft Edge - Configurações Padrão (os usuários podem substituir)/
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): SOFTWARE\Policies\Microsoft\Edge\Recomendações
  - Nome do Valor: ImportPaymentInfo
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000001
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: ImportPaymentInfo
  - Exemplo de valor:
``` xml
<true/>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### ImportSavedPasswords
  #### Permitir a importação de senhas salvas
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Permite que os usuários importem as senhas salvas de outro navegador para o Microsoft Edge.

Se você habilitar essa política, a opção para importar manualmente as senhas salvas será selecionada automaticamente.

Se essa política for desabilitada, as senhas salvas não serão importadas na primeira execução, e os usuários não poderão importá-las manualmente.

Se você não configurar essa política, as senhas serão importadas na primeira execução, e os usuários poderão optar por importá-las manualmente durante as sessões de navegação posteriores.

Você pode definir essa política como uma recomendação. Isso significa que o Microsoft Edge importa as senhas na primeira execução, mas os usuários poderão marcar ou desmarcar a opção **senhas** durante a importação manual.

**Observação**: essa política gerencia atualmente a importação dos navegadores Internet Explorer (no Windows 7, 8 e 10) e Google Chrome (no Windows 7, 8 e 10 e macOS).

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Sim
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: ImportSavedPasswords
  - Nome da GP: Permitir a importação de senhas salvas
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): Modelos Administrativos/Microsoft Edge - Configurações Padrão (os usuários podem substituir)/
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): SOFTWARE\Policies\Microsoft\Edge\Recomendações
  - Nome do Valor: ImportSavedPasswords
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000001
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: ImportSavedPasswords
  - Exemplo de valor:
``` xml
<true/>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### ImportSearchEngine
  #### Permitir importação das configurações do mecanismo de pesquisa
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Permite que os usuários importem as configurações do mecanismo de pesquisa de outro navegador para o Microsoft Edge.

Se você habilitar essa política, a opção para importar as configurações do mecanismo de pesquisa será selecionada automaticamente.

Se essa política for desabilitada, as configurações do mecanismo de pesquisa não serão importadas na primeira execução, e os usuários não poderão importá-las manualmente.

Se você não configurar essa política, as configurações do mecanismo de pesquisa serão importadas na primeira execução, e os usuários poderão optar por importar esses dados manualmente durante sessões de navegação posteriores.

Você pode definir essa política como uma recomendação. Isso significa que o Microsoft Edge importa as configurações do mecanismo de pesquisa na primeira execução, mas os usuários podem marcar ou desmarcar a opção **mecanismo de pesquisa** durante a importação manual.

**Observação**: essa política atualmente gerencia a importação do Internet Explorer (no Windows 7, 8 e 10).

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Sim
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: ImportSearchEngine
  - Nome da GP: Permitir importação das configurações do mecanismo de pesquisa
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): Modelos Administrativos/Microsoft Edge - Configurações Padrão (os usuários podem substituir)/
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): SOFTWARE\Policies\Microsoft\Edge\Recomendações
  - Nome do Valor: ImportSearchEngine
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000001
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: ImportSearchEngine
  - Exemplo de valor:
``` xml
<true/>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### InPrivateModeAvailability
  #### Configurar a disponibilidade do modo InPrivate
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Especifica se o usuário pode abrir páginas no modo InPrivate no Microsoft Edge.

Se você não configurar essa política ou defini-la como "Habilitada" (0), os usuários poderão abrir páginas no modo InPrivate.

Defina esta política como "Desabilitar" (1) para impedir que os usuários usem o modo InPrivate.

Defina esta política como "Forçada" (2) para usar sempre o modo InPrivate.

* 0 = Modo InPrivate disponível

* 1 = Modo InPrivate desabilitado

* 2 = Modo InPrivate forçado

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Número inteiro

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: InPrivateModeAvailability
  - Nome da GP: Configurar a disponibilidade do modo InPrivate
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: InPrivateModeAvailability
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000001
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: InPrivateModeAvailability
  - Exemplo de valor:
``` xml
<integer>1</integer>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### InternetExplorerIntegrationLevel
  #### Configurar a integração com o Internet Explorer
  >Versões com Suporte: O Microsoft Edge no Windows desde a versão 77 ou posterior

  #### Descrição
  Para obter orientações sobre como configurar a experiência ideal para o modo do Internet Explorer, consulte [https://go.microsoft.com/fwlink/?linkid=2094210](https://go.microsoft.com/fwlink/?linkid=2094210)

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Não - Requer a reinicialização do navegador

  #### Tipo de Dados:
  Número inteiro

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: InternetExplorerIntegrationLevel
  - Nome da GP: Configurar a integração com o Internet Explorer
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: InternetExplorerIntegrationLevel
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000001
```


  

  [Voltar ao início](#microsoft-edge---políticas)

  ### InternetExplorerIntegrationSiteList
  #### Configurar a Lista de Sites do Modo Empresarial
  >Versões com Suporte: O Microsoft Edge no Windows desde a versão 78 ou posterior

  #### Descrição
  Para obter orientações sobre como configurar a experiência ideal para o modo do Internet Explorer, consulte [https://go.microsoft.com/fwlink/?linkid=2094210](https://go.microsoft.com/fwlink/?linkid=2094210)

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Não - Requer a reinicialização do navegador

  #### Tipo de Dados:
  Cadeia de Caracteres

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: InternetExplorerIntegrationSiteList
  - Nome da GP: Configurar a Lista de Sites do Modo Empresarial
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: InternetExplorerIntegrationSiteList
  - Tipo de Valor: REG_SZ
  ##### Exemplo de valor:
```
"https://internal.contoso.com/sitelist.xml"
```


  

  [Voltar ao início](#microsoft-edge---políticas)

  ### IsolateOrigins
  #### Habilitar isolamento de site para origens específicas
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Especifica as origens para executar isoladamente, em seus próprios processos.
Essa política também isola origens indicadas por subdomínios. Por exemplo, especificar https://contoso.com/ causará o isolamento de https://foo.contoso.com/ como parte do site https://contoso.com/.
Se a política estiver habilitada, cada uma das origens indicadas em uma lista separada por vírgulas será executada em seu próprio processo.
Se essa política for desabilitada, os recursos [IsolateOrigins](#isolateorigins) e [SitePerProcess](#siteperprocess) serão desabilitados. Os usuários ainda podem habilitar a política [IsolateOrigins](#isolateorigins) manualmente, por meio de sinalizadores de linha de comando.
Se você não configurar a política, o usuário poderá alterar essa configuração.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Não - Requer a reinicialização do navegador

  #### Tipo de Dados:
  Cadeia de Caracteres

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: IsolateOrigins
  - Nome da GP: Habilitar isolamento de site para origens específicas
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: IsolateOrigins
  - Tipo de Valor: REG_SZ
  ##### Exemplo de valor:
```
"https://contoso.com/,https://fabrikam.com/"
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: IsolateOrigins
  - Exemplo de valor:
``` xml
<string>https://contoso.com/,https://fabrikam.com/</string>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### ManagedFavorites
  #### Configurar favoritos
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Configura uma lista de favoritos gerenciados.

A política cria uma lista de favoritos. Cada favorito contém as chaves "name" e "url", que contêm o nome do favorito e seu destino. Você pode configurar uma subpasta definindo favoritos sem uma chave "url", mas com uma chave "children" adicional contendo uma lista de favoritos, conforme definido acima (alguns dos quais poderão ser pastas novamente). O Microsoft Edge corrige as URLs incompletas como se elas fossem enviadas pela Barra de Endereços, por exemplo, "microsoft.com" torna-se "https://microsoft.com/".

Esses favoritos são colocados em uma pasta que não pode ser modificada pelo usuário (mas o usuário pode ocultá-la da barra de favoritos). Por padrão, o nome da pasta é "Favoritos gerenciados", mas você pode alterá-la adicionando à lista de favoritos um dicionário contendo a chave "toplevel_name" com o nome de pasta desejado como o valor.

Os favoritos gerenciados não são sincronizados com a conta de usuário e não podem ser modificados por extensões.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Dicionário

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: ManagedFavorites
  - Nome da GP: Configurar favoritos
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: ManagedFavorites
  - Tipo de Valor: REG_SZ
  ##### Exemplo de valor:
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


  #### Informações e configurações do Mac
  - Nome da chave de preferência: ManagedFavorites
  - Exemplo de valor:
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
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### ManagedSearchEngines
  #### Gerenciar Mecanismos de Pesquisa
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Lets you configure a list of list of up to 10 search engines, one of which must be marked as the default search engine.
You do not need to specify the encoding, suggest_url, image_search_url, or image_search_post_params for any search engine (the image_search_post_params consists of comma-separated name/value pairs).

If you enable this policy, users can't add, remove, or change any search engine in the list. Users can set their default search engine to any search engine in the list.

If you disable or don't configure this policy, users can modify the search engines list as desired.

If the [DefaultSearchProviderSearchURL](#defaultsearchprovidersearchurl) policy is set, this policy (ManagedSearchEngines) is ignored. The user must restart their browser to finish applying this policy.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Não - Requer a reinicialização do navegador

  #### Tipo de Dados:
  Dicionário

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: ManagedSearchEngines
  - Nome da GP: Gerenciar Mecanismos de Pesquisa
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: ManagedSearchEngines
  - Tipo de Valor: REG_SZ
  ##### Exemplo de valor:
```
SOFTWARE\Policies\Microsoft\Edge\ManagedSearchEngines = [
  {
    "is_default": true, 
    "keyword": "example1.com", 
    "name": "Example1", 
    "search_url": "https://www.example1.com/search?q={searchTerms}", 
    "suggest_url": "https://www.example1.com/qbox?query={searchTerms}"
  }, 
  {
    "image_search_post_params": "content={imageThumbnail},url={imageURL},sbisrc={SearchSource}", 
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
  }, 
  {
    "keyword": "example4.com", 
    "name": "Example4", 
    "search_url": "https://www.example4.com/search?q={searchTerms}"
  }
]
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: ManagedSearchEngines
  - Exemplo de valor:
``` xml
<key>ManagedSearchEngines</key>
<array>
  <dict>
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
    <key>image_search_post_params</key>
    <string>content={imageThumbnail},url={imageURL},sbisrc={SearchSource}</string>
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
  <dict>
    <key>keyword</key>
    <string>example4.com</string>
    <key>name</key>
    <string>Example4</string>
    <key>search_url</key>
    <string>https://www.example4.com/search?q={searchTerms}</string>
  </dict>
</array>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### MaxConnectionsPerProxy
  #### Número máximo de conexões simultâneas com o servidor proxy
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Especifica o número máximo de conexões simultâneas com o servidor proxy.

Alguns servidores proxy não podem manipular um alto número de conexões simultâneas por cliente. Você pode resolver isso configurando essa política como um valor menor.

O valor dessa política deve ser inferior a 100 e maior do que 6. O valor padrão é 32.

Alguns aplicativos Web são conhecidos por consumir muitas conexões com GETs pendentes. Reduzir o máximo de conexões abaixo 32 pode travar o navegador se vários desses aplicativos Web estiverem abertos.

Se você não configurar essa política, o valor padrão (32) será usado.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Não - Requer a reinicialização do navegador

  #### Tipo de Dados:
  Número inteiro

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: MaxConnectionsPerProxy
  - Nome da GP: Número máximo de conexões simultâneas com o servidor proxy
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: MaxConnectionsPerProxy
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000020
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: MaxConnectionsPerProxy
  - Exemplo de valor:
``` xml
<integer>32</integer>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### MediaRouterCastAllowAllIPs
  #### Permitir que o Google Cast se conecte a dispositivos Cast em todos os endereços IP
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Habilite essa política para permitir que o Google Cast conecte-se a dispositivos Cast em todos os endereços IP, e não apenas em endereços privados RFC1918/RFC4193.

Desabilite essa política para restringir o Google Cast a dispositivos Cast em endereços privados RFC1918/RFC4193.

Se você não configurar essa política, o Google Cast se conectará a dispositivos Cast somente em endereços privados RFC1918/RFC4193, a menos que você habilite o recurso CastAllowAllIPs.

Se a política [EnableMediaRouter](#enablemediarouter) estiver desabilitada, essa política não terá efeito.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: MediaRouterCastAllowAllIPs
  - Nome da GP: Permitir que o Google Cast se conecte a dispositivos Cast em todos os endereços IP
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: MediaRouterCastAllowAllIPs
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000000
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: MediaRouterCastAllowAllIPs
  - Exemplo de valor:
``` xml
<false/>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### MetricsReportingEnabled
  #### Habilitar relatórios de dados relacionados a uso e falhas
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Para os canais Windows 10 Beta e Stable do Microsoft Edge, essa política, quando configurada, substituirá a configuração de dados de diagnóstico do Windows para coleção ou não coleção de dados relacionados a erros e falhas do Microsoft Edge ([https://go.microsoft.com/fwlink/?linkid=2099569](https://go.microsoft.com/fwlink/?linkid=2099569)).

Essa política habilita o relatório de uso e dados relacionados a falhas sobre o Microsoft Edge para a Microsoft e impede que os usuários alterem essa configuração.

Habilite essa política para enviar relatórios de uso e dados relacionados a falhas para a Microsoft. Desabilite essa política para não enviar os dados para a Microsoft. Em ambos os casos, os usuários não podem alterar ou substituir a configuração.

Em canais do Windows 10 Beta e Stable, essa política controla dados relacionados a uso e falhas. Se essa política não estiver configurada, o Microsoft Edge usará como padrão a configuração de dados de diagnóstico do Windows.

Em canais do Windows 10, Canary e Dev, essa política controla dados relacionados a uso e falhas. Se essa política não estiver configurada, o Microsoft Edge usará como padrão a preferência do usuário.

No Windows 7, 8 e Mac, essa política controla dados relacionados a uso e falhas. Se essa política não estiver configurada, o Microsoft Edge usará como padrão a preferência do usuário.

Essa política está disponível somente em instâncias do Windows que fazem parte de um domínio do Microsoft Active Directory ou em instâncias do Windows 10 Pro ou Enterprise registradas para gerenciamento de dispositivos.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Não - Requer a reinicialização do navegador

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: MetricsReportingEnabled
  - Nome da GP: Habilitar relatórios de dados relacionados a uso e falhas
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: MetricsReportingEnabled
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000001
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: MetricsReportingEnabled
  - Exemplo de valor:
``` xml
<true/>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### NetworkPredictionOptions
  #### Habilitar previsão de rede
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Habilita a previsão de rede e impede que os usuários alterem essa configuração.

Isso controla a pré-busca de DNS, a pré-conexão TCP e SSL e a pré-renderização de páginas da Web.

Se você não configurar essa política, a previsão de rede será habilitada, mas o usuário poderá alterá-la.

* 0 = Prever ações de rede em qualquer conexão de rede

* 2 = Não prever ações de rede em qualquer conexão de rede

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Sim
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Número inteiro

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: NetworkPredictionOptions
  - Nome da GP: Habilitar previsão de rede
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): Modelos Administrativos/Microsoft Edge - Configurações Padrão (os usuários podem substituir)/
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): SOFTWARE\Policies\Microsoft\Edge\Recomendações
  - Nome do Valor: NetworkPredictionOptions
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000001
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: NetworkPredictionOptions
  - Exemplo de valor:
``` xml
<integer>1</integer>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### NonRemovableProfileEnabled
  #### Configurar se um usuário sempre tem um perfil padrão conectado automaticamente à sua conta corporativa ou de estudante
  >Versões com Suporte: O Microsoft Edge no Windows desde a versão 78 ou posterior

  #### Descrição
  Essa política determina se usuário pode remover o perfil do Microsoft Edge conectado automaticamente com a conta corporativa ou de estudante.

Se você habilitar, um perfil não removível será criado com a conta corporativa ou de estudante do usuário no Windows. Esse perfil não pode ser desconectado nem removido.

Se você desabilitar ou não configurar essa política, o perfil conectado automaticamente com a conta corporativa ou de estudante de um usuário do Windows pode ser desconectado ou removido pelo usuário.

Se você quiser configurar a entrada do navegador, use a política [BrowserSignin](#browsersignin).

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: NonRemovableProfileEnabled
  - Nome da GP: Configurar se um usuário sempre tem um perfil padrão conectado automaticamente à sua conta corporativa ou de estudante
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: NonRemovableProfileEnabled
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000001
```


  

  [Voltar ao início](#microsoft-edge---políticas)

  ### OverrideSecurityRestrictionsOnInsecureOrigin
  #### Controlar onde se aplicam a restrições de segurança em origens não seguras
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Especifica uma lista de origens (URLs) ou padrões de nome de host (como "*.contoso.com") para que as restrições de segurança relativas às origens inseguras não se apliquem.

Essa política permite que você especifique as origens permitidas para aplicativos herdados que não é podem implantar o TLS nem configurar um servidor de preparo para desenvolvimento para a Web interno de forma que os desenvolvedores possam testar os recursos que exigem contextos seguros sem precisar implantar o TLS no servidor de preparo. Essa política também impede que a origem seja rotulada como "Não Segura" na omnibox.

A definição de uma lista de URLs nessa política terá o mesmo efeito que a configuração do sinalizador de linha de comando '--unsafely-treat-insecure-origin-as-secure' para uma lista separada por vírgulas das mesmas URLs. Se você habilitar essa política, ela substituirá o sinalizador de linha de comando.

Para obter mais informações sobre os contextos seguros, consulte https://www.w3.org/TR/secure-contexts/.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Não - Requer a reinicialização do navegador

  #### Tipo de Dados:
  Lista de cadeias de caracteres

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: OverrideSecurityRestrictionsOnInsecureOrigin
  - Nome da GP: Controlar onde se aplicam a restrições de segurança em origens não seguras
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge\OverrideSecurityRestrictionsOnInsecureOrigin
  - Caminho (Recomendações): N/A
  - Nome do Valor: 1, 2, 3, ...
  - Tipo de Valor: lista de REG_SZ
  ##### Exemplo de valor:
```
SOFTWARE\Policies\Microsoft\Edge\OverrideSecurityRestrictionsOnInsecureOrigin\0 = "http://testserver.contoso.com/"
SOFTWARE\Policies\Microsoft\Edge\OverrideSecurityRestrictionsOnInsecureOrigin\1 = "*.contoso.com"

```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: OverrideSecurityRestrictionsOnInsecureOrigin
  - Exemplo de valor:
``` xml
<array>
  <string>http://testserver.contoso.com/</string>
  <string>*.contoso.com</string>
</array>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### PersonalizationReportingEnabled
  #### Allow personalization of ads, search and news by sending browsing history to Microsoft
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 80 ou posterior

  #### Descrição
  This policy prevents Microsoft from collecting a user's Microsoft Edge browsing history to be used for personalizing advertising, search, news and other Microsoft services.

This setting is only available for users with a Microsoft account. This setting is not available for child accounts or enterprise accounts.

If you disable this policy, users can't change or override the setting. If this policy is enabled or not configured, Microsoft Edge will default to the user’s preference.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: PersonalizationReportingEnabled
  - Nome da GP: Allow personalization of ads, search and news by sending browsing history to Microsoft
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: PersonalizationReportingEnabled
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000001
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: PersonalizationReportingEnabled
  - Exemplo de valor:
``` xml
<true/>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### PinningWizardAllowed
  #### Permitir o Assistente para fixar na barra de tarefas
  >Versões com Suporte: O Microsoft Edge no Windows desde a versão 80 ou posterior

  #### Descrição
  O Microsoft Edge usa o Assistente para fixar na barra de tarefas para ajudar os usuários a fixar sites sugeridos na barra de tarefas. O recurso Fixar na barra de tarefas é habilitado por padrão e pode ser acessado pelo usuário por meio do menu Configurações e mais.

Se você habilitar essa política ou não configurá-la, os usuários poderão chamar o Assistente para fixar na barra de tarefas no menu Configurações e mais. O Assistente também pode ser chamado por meio de uma inicialização de protocolo.

Se você desabilitar essa política, o Assistente para fixar na barra de tarefas será desabilitado no menu e não poderá ser chamado por meio de uma inicialização de protocolo.

As configurações do usuário para habilitar ou desabilitar o Assistente para fixar na barra de tarefas não estão disponíveis.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Não - Requer a reinicialização do navegador

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: PinningWizardAllowed
  - Nome da GP: Permitir o Assistente para fixar na barra de tarefas
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: PinningWizardAllowed
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000000
```


  

  [Voltar ao início](#microsoft-edge---políticas)

  ### ProactiveAuthEnabled
  #### Habilitar a Autenticação Proativa
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Permite configurar se a Autenticação Proativa deve ser ativada.

Se você habilitar essa política, o Microsoft Edge tentará autenticar de forma proativa o usuário conectado com os serviços Microsoft. Em intervalos regulares, o Microsoft Edge verifica em um serviço online um manifesto atualizado com a configuração que rege como fazer isso.

Se você desabilitar essa política, o Microsoft Edge não tentará autenticar de forma proativa o usuário conectado com os serviços Microsoft. O Microsoft Edge não verifica mais em um serviço online se há um manifesto atualizado com a configuração para fazer isso.

Se você não configurar essa política, a Autenticação Proativa será ativada.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Não - Requer a reinicialização do navegador

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: ProactiveAuthEnabled
  - Nome da GP: Habilitar a Autenticação Proativa
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: ProactiveAuthEnabled
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000001
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: ProactiveAuthEnabled
  - Exemplo de valor:
``` xml
<true/>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### PromotionalTabsEnabled
  #### Habilitar conteúdo promocional em toda a guia
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Controla a apresentação de conteúdo promocional ou educativo em uma guia inteira. Esta configuração controla a apresentação de páginas de boas-vindas que ajudam os usuários a entrar no Microsoft Edge, escolher o navegador padrão ou saber mais sobre os recursos do produto.

Se você habilitar esta política (defini-la como true) ou não a configurar, o Microsoft Edge poderá mostrar conteúdo em uma guia inteira aos usuários para fornecer informações sobre o produto.

Se você desabilitar (definir como false) esta política, o Microsoft Edge não poderá mostrar o conteúdo em uma guia inteira aos usuários.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: PromotionalTabsEnabled
  - Nome da GP: Habilitar conteúdo promocional em toda a guia
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: PromotionalTabsEnabled
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000000
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: PromotionalTabsEnabled
  - Exemplo de valor:
``` xml
<false/>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### PromptForDownloadLocation
  #### Perguntar onde salvar os arquivos baixados
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Define se deve-se perguntar onde salvar um arquivo antes de baixá-lo.

Se você habilitar essa política, será perguntado ao usuário onde salvar cada arquivo antes de baixar; se você não configurá-la, os arquivos serão salvos automaticamente no local padrão, sem perguntar ao usuário.

Se você não configurar essa política, o usuário poderá alterar essa configuração.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: PromptForDownloadLocation
  - Nome da GP: Perguntar onde salvar os arquivos baixados
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: PromptForDownloadLocation
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000000
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: PromptForDownloadLocation
  - Exemplo de valor:
``` xml
<false/>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### QuicAllowed
  #### Permitir o protocolo QUIC
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Permite o uso do protocolo QUIC no Microsoft Edge.

Se você habilitar essa política ou não configurá-la, o protocolo QUIC será permitido.

Se essa política for desabilitada, o protocolo QUIC será bloqueado.

QUIC é um protocolo de rede de camada de transporte que pode melhorar o desempenho dos aplicativos Web que atualmente usam o TCP.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Não - Requer a reinicialização do navegador

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: QuicAllowed
  - Nome da GP: Permitir o protocolo QUIC
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: QuicAllowed
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000001
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: QuicAllowed
  - Exemplo de valor:
``` xml
<true/>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### RelaunchNotification
  #### Notificar um usuário de que uma reinicialização do navegador é recomendada ou necessária para atualizações pendentes
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Notifique os usuários de que eles precisam reiniciar o Microsoft Edge para aplicar uma atualização pendente.

Se você não configurar essa política, o Microsoft Edge adicionará um ícone de reciclagem na extremidade direita da barra de menus superior para solicitar que os usuários reiniciem o navegador para aplicar a atualização.

Se você habilitar essa política e defini-la como "Recomendada" (1), um aviso recorrente indicará aos usuários que uma reinicialização é recomendada. Os usuários podem ignorar esse aviso e adiar a reinicialização.

Se você definir a política como "Obrigatória" (2), um aviso recorrente indicará aos usuários que o navegador será reiniciado automaticamente assim que um período de notificação passar. O período padrão é de sete dias. Você pode configurar esse período com a política [RelaunchNotificationPeriod](#relaunchnotificationperiod).

A sessão do usuário é restaurada quando o navegador é reiniciado.

* Recomendada (1) = Mostra um aviso recorrente para o usuário indicando que uma reinicialização é recomendada

* Obrigatória (2) = Mostra um aviso recorrente ao usuário indicando que uma reinicialização é obrigatória

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Número inteiro

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: RelaunchNotification
  - Nome da GP: Notificar um usuário de que uma reinicialização do navegador é recomendada ou necessária para atualizações pendentes
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: RelaunchNotification
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000001
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: RelaunchNotification
  - Exemplo de valor:
``` xml
<integer>1</integer>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### RelaunchNotificationPeriod
  #### Definir o período para notificações de atualização
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Permite definir o período, em milissegundos, no qual os usuários são avisados de que o Microsoft Edge deve ser reiniciado ou que um dispositivo Microsoft Edge OS deve ser reiniciado para aplicar uma atualização pendente.

Durante esse período, o usuário será informado repetidamente sobre a necessidade de uma atualização. Para dispositivos Microsoft Edge OS, uma notificação de reinicialização aparece na bandeja do sistema de acordo com a política RelaunchHeadsUpPeriod. Para navegadores Microsoft Edge, o menu do app é alterado para indicar que uma reinicialização é necessária depois de decorrido um terço do período de notificação. Essa notificação muda de cor depois de decorridos dois terços do período de notificação e novamente depois de decorrido todo o período de notificação. As notificações adicionais habilitadas pela política [RelaunchNotification](#relaunchnotification) seguem a mesma agenda.

Se não definido, será usado o período padrão de 604800000 milissegundos (uma semana).

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Número inteiro

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: RelaunchNotificationPeriod
  - Nome da GP: Definir o período para notificações de atualização
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: RelaunchNotificationPeriod
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x240c8400
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: RelaunchNotificationPeriod
  - Exemplo de valor:
``` xml
<integer>604800000</integer>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### RendererCodeIntegrityEnabled
  #### Habilitar integridade do código do renderizador
  >Versões com Suporte: O Microsoft Edge no Windows desde a versão 78 ou posterior

  #### Descrição
  Se essa política for habilitada ou não for definida, a Integridade do Código do Renderizador será habilitada. Essa política deve ser desabilitada somente se forem encontrados problemas de compatibilidade com softwares de terceiros que devem ser executados nos processos de renderização do Microsoft Edge.

Desabilitar essa política tem um efeito prejudicial sobre a segurança e a estabilidade do Microsoft Edge, pois o código desconhecido e potencialmente hostil poderá ser carregado dentro dos processos de renderização do Microsoft Edge.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Não - Requer a reinicialização do navegador

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: RendererCodeIntegrityEnabled
  - Nome da GP: Habilitar integridade do código do renderizador
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: RendererCodeIntegrityEnabled
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000000
```


  

  [Voltar ao início](#microsoft-edge---políticas)

  ### RequireOnlineRevocationChecksForLocalAnchors
  #### Especificar se as verificações OCSP/CRL online são necessárias para âncoras de confiança locais
  >Versões com Suporte: O Microsoft Edge no Windows desde a versão 77 ou posterior

  #### Descrição
  Controla se as verificações de revogação online (verificações OCSP/CRL) são necessárias. Se o Microsoft Edge não puder obter informações do status de revogação, esses certificados serão tratados como revogados ("falha irrecuperável").

Se você habilitar esta política, o Microsoft Edge sempre executará a verificação de revogação para certificados de servidores com validação bem-sucedida e assinados por certificados de Autoridade de Certificação instalados localmente.

Se você não configurar ou desabilitar esta política, o Microsoft Edge usará as configurações de revogação online existentes.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: RequireOnlineRevocationChecksForLocalAnchors
  - Nome da GP: Especificar se as verificações OCSP/CRL online são necessárias para âncoras de confiança locais
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: RequireOnlineRevocationChecksForLocalAnchors
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000000
```


  

  [Voltar ao início](#microsoft-edge---políticas)

  ### ResolveNavigationErrorsUseWebService
  #### Habilitar a resolução de erros de navegação usando um serviço Web
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Permita que o Microsoft Edge emita uma conexão sem dados para um serviço Web para sondar redes em busca de conectividade em casos como o Wi-Fi em hotéis e aeroportos.

Se você habilitar essa política, um serviço Web será usado para testes de conectividade de rede.

Se você desabilitar essa política, o Microsoft Edge usará APIs nativas para tentar resolver os problemas de conectividade e de navegação de rede.

**Observação**: exceto no Windows 8 e em versões posteriores do Windows, o Microsoft Edge *sempre* usará APIs nativas para resolver problemas de conectividade.

Se você não configurar essa política, o Microsoft Edge respeitará a preferência do usuário definida em Serviços, em edge://settings/privacy.
Especificamente, há uma alternância **Usar um serviço Web para ajudar a resolver erros de navegação**, que o usuário pode ativar ou desativar. Esteja ciente de que, se essa política tiver sido habilitada (ResolveNavigationErrorsUseWebService), a configuração **Usar um serviço Web para ajudar a resolver erros de navegação** será ativada, mas o usuário não poderá alterá-la usando a alternância. Se você tiver desabilitado essa política, a configuração **Usar um serviço Web para ajudar a resolver erros de navegação** será desativada, e o usuário não poderá alterá-la usando a alternância.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Sim
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: ResolveNavigationErrorsUseWebService
  - Nome da GP: Habilitar a resolução de erros de navegação usando um serviço Web
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): Modelos Administrativos/Microsoft Edge - Configurações Padrão (os usuários podem substituir)/
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): SOFTWARE\Policies\Microsoft\Edge\Recomendações
  - Nome do Valor: ResolveNavigationErrorsUseWebService
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000001
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: ResolveNavigationErrorsUseWebService
  - Exemplo de valor:
``` xml
<true/>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### RestrictSigninToPattern
  #### Restringir quais contas podem ser usadas como contas principais do Microsoft Edge
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Determina as contas que podem ser definidas como contas principais do navegador no Microsoft Edge (a conta que é escolhida durante o fluxo de consentimento de sincronização).

Se um usuário tentar definir uma conta principal do navegador com um nome de usuário que não corresponda a esse padrão, ele será bloqueado e verá uma mensagem de erro apropriada.

Se você não configurar esta política ou deixá-la em branco, os usuários poderão definir qualquer conta como uma conta principal do navegador no Microsoft Edge.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Cadeia de Caracteres

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: RestrictSigninToPattern
  - Nome da GP: Restringir quais contas podem ser usadas como contas principais do Microsoft Edge
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: RestrictSigninToPattern
  - Tipo de Valor: REG_SZ
  ##### Exemplo de valor:
```
".*@contoso.com"
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: RestrictSigninToPattern
  - Exemplo de valor:
``` xml
<string>.*@contoso.com</string>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### RunAllFlashInAllowMode
  #### Estender a configuração do conteúdo em Adobe Flash a todo o conteúdo
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Se você habilitar essa política, todo o conteúdo Adobe Flash inserido em sites que estão configurados para permitir Adobe Flash nas configurações de conteúdo, pelo usuário ou pela política da empresa, será executado. Isso inclui o conteúdo de outras origens e/ou conteúdo pequeno.

Para controlar os sites que têm permissão para executar Adobe Flash, consulte as especificações nas políticas [DefaultPluginsSetting](#defaultpluginssetting), [PluginsAllowedForUrls](#pluginsallowedforurls) e [PluginsBlockedForUrls](#pluginsblockedforurls).

Se você desabilitar essa política ou não configurá-la, o conteúdo do Adobe Flash de outras origens (de sites que não são especificados nas três políticas mencionadas acima) ou conteúdo pequeno talvez seja bloqueado.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: RunAllFlashInAllowMode
  - Nome da GP: Estender a configuração do conteúdo em Adobe Flash a todo o conteúdo
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: RunAllFlashInAllowMode
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000001
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: RunAllFlashInAllowMode
  - Exemplo de valor:
``` xml
<true/>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### SSLErrorOverrideAllowed
  #### Permitir que os usuários continuem a partir da página de aviso HTTPS
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  O Microsoft Edge mostra uma página de aviso quando os usuários visitam sites que têm erros de SSL.

Se você habilitar ou não configurar (padrão) essa política, os usuários poderão clicar nessas páginas de aviso.

Se você desabilitar essa política, os usuários serão impedidos de clicar em qualquer página de aviso.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: SSLErrorOverrideAllowed
  - Nome da GP: Permitir que os usuários continuem a partir da página de aviso HTTPS
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: SSLErrorOverrideAllowed
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000001
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: SSLErrorOverrideAllowed
  - Exemplo de valor:
``` xml
<true/>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### SSLVersionMin
  #### Versão mínima do TLS habilitada
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Define a versão mínima com suporte do SSL. Se você não definir essa política, o Microsoft Edge usará uma versão mínima do padrão, o TLS 1.0.

Se habilitar essa política, você poderá definir a versão mínima com um dos seguintes valores: "tls1", "tls1.1" ou "tls1.2". Quando definida, o Microsoft Edge não usará uma versão do SSL/TLS menor do que a versão especificada. Os valores não reconhecidos serão ignorados.

* "tls1" = TLS 1.0

* "tls1.1" = TLS 1.1

* "tls1.2" = TLS 1.2

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Cadeia de Caracteres

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: SSLVersionMin
  - Nome da GP: Versão mínima do TLS habilitada
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: SSLVersionMin
  - Tipo de Valor: REG_SZ
  ##### Exemplo de valor:
```
"tls1"
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: SSLVersionMin
  - Exemplo de valor:
``` xml
<string>tls1</string>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### SavingBrowserHistoryDisabled
  #### Desabilitar o salvamento do histórico do navegador
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Desabilita o salvamento do histórico do navegador e impede que os usuários alterem essa configuração.

Se você habilitar essa política, o histórico de navegação não será salvo. Isso também desabilita a sincronização de guias.

Se você desabilitar essa política ou não configurá-la, o histórico de navegação será salvo.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: SavingBrowserHistoryDisabled
  - Nome da GP: Desabilitar o salvamento do histórico do navegador
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: SavingBrowserHistoryDisabled
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000001
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: SavingBrowserHistoryDisabled
  - Exemplo de valor:
``` xml
<true/>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### SearchSuggestEnabled
  #### Habilitar sugestões de pesquisa
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Habilita sugestões de pesquisa na Web na Barra de Endereço do Microsoft Edge e na Lista de Sugestão Automática e impede que os usuários alterem essa política.

Se você habilitar essa política, serão usadas sugestões de pesquisa da Web.

Se você desabilitar essa política, as sugestões de pesquisa da Web nunca serão usadas. Contudo, as sugestões do histórico local e dos favoritos locais ainda serão exibidas. Se você desabilitar essa política, nem os caracteres digitados, nem as URLs visitadas serão incluídos na telemetria para a Microsoft.

Se essa política não for definida, as sugestões de pesquisa serão habilitadas, mas o usuário poderá alterá-la.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Sim
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: SearchSuggestEnabled
  - Nome da GP: Habilitar sugestões de pesquisa
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): Modelos Administrativos/Microsoft Edge - Configurações Padrão (os usuários podem substituir)/
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): SOFTWARE\Policies\Microsoft\Edge\Recomendações
  - Nome do Valor: SearchSuggestEnabled
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000001
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: SearchSuggestEnabled
  - Exemplo de valor:
``` xml
<true/>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### SecurityKeyPermitAttestation
  #### Sites ou domínios que não precisam de permissão para usar o atestado de Chave de Segurança direto
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Especifica os sites e os domínios que não precisam de permissão explícita do usuário quando certificados de atestado de chaves de segurança são solicitados. Além disso, um sinal é enviado para a chave de segurança que indica que eles podem usar o atestado individual. Sem isso, os usuários serão avisados toda vez que um site solicitar o atestado de chaves de segurança.

Sites (como https://contoso.com/some/path) se correspondem apenas com appIDs U2F. Domínios (como contoso.com) se correspondem apenas com IDs RP webauthn. Para cobrir APIs U2F e webauthn para um determinado site, será necessário listar o domínio e a URL de appID.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Lista de cadeias de caracteres

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: SecurityKeyPermitAttestation
  - Nome da GP: Sites ou domínios que não precisam de permissão para usar o atestado de Chave de Segurança direto
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge\SecurityKeyPermitAttestation
  - Caminho (Recomendações): N/A
  - Nome do Valor: 1, 2, 3, ...
  - Tipo de Valor: lista de REG_SZ
  ##### Exemplo de valor:
```
SOFTWARE\Policies\Microsoft\Edge\SecurityKeyPermitAttestation\0 = "https://contoso.com"

```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: SecurityKeyPermitAttestation
  - Exemplo de valor:
``` xml
<array>
  <string>https://contoso.com</string>
</array>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### SendIntranetToInternetExplorer
  #### Enviar todos os sites da intranet para o Internet Explorer
  >Versões com Suporte: O Microsoft Edge no Windows desde a versão 77 ou posterior

  #### Descrição
  Para obter orientações sobre como configurar a experiência ideal para o modo do Internet Explorer, consulte [https://go.microsoft.com/fwlink/?linkid=2094210](https://go.microsoft.com/fwlink/?linkid=2094210)

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Não - Requer a reinicialização do navegador

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: SendIntranetToInternetExplorer
  - Nome da GP: Enviar todos os sites da intranet para o Internet Explorer
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: SendIntranetToInternetExplorer
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000001
```


  

  [Voltar ao início](#microsoft-edge---políticas)

  ### SendSiteInfoToImproveServices
  #### Enviar informações do site para melhorar os serviços Microsoft
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Para os canais Windows 10 Beta e Stable do Microsoft Edge, essa política quando configurada substituirá a configuração de dados de diagnóstico do Windows para coleção ou não coleção informações do site do Microsoft Edge ([https://go.microsoft.com/fwlink/?linkid=2099569](https://go.microsoft.com/fwlink/?linkid=2099569)).

Essa configuração de política permite que você decida se os usuários podem enviar informações sobre os sites que eles visitam no Microsoft Edge para a Microsoft para melhorar os serviços como pesquisa.

Se você habilitar essa política, as informações sobre os sites visitados no Microsoft Edge serão enviadas à Microsoft.

Se você desabilitar essa política, as informações sobre os sites visitados no Microsoft Edge não serão enviadas à Microsoft.

Em canais do Windows 10 Beta e Stable, essa política controla o envio de informações sobre os usuários de sites. Se essa política não estiver configurada, o Microsoft Edge usará como padrão a configuração de dados de diagnóstico do Windows.

Em canais Windows 10, Canary e Dev, esta política controla o envio de informações sobre os usuários de sites. Se essa política não estiver configurada, o Microsoft Edge usará como padrão a preferência do usuário.

No Windows 7, 8 e Mac, esta política controla o envio de informações sobre os usuários do site. Se essa política não estiver configurada, Microsoft Edge usará como padrão a preferência do usuário.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Não - Requer a reinicialização do navegador

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: SendSiteInfoToImproveServices
  - Nome da GP: Enviar informações do site para melhorar os serviços Microsoft
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: SendSiteInfoToImproveServices
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000000
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: SendSiteInfoToImproveServices
  - Exemplo de valor:
``` xml
<false/>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### ShowOfficeShortcutInFavoritesBar
  #### Mostrar o atalho do Microsoft Office na barra Favoritos
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Especifica se deve-se incluir um atalho para Office.com na barra de favoritos. Para usuários conectados ao Microsoft Edge, o atalho leva-os para seus documentos e aplicativos do Microsoft Office.

Se essa política estiver habilitada ou não estiver configurada, os usuários poderão optar por ver o atalho. Basta alterar a alternância no menu de contexto da barra de favoritos.

Se a política estiver desabilitada, o atalho não será mostrado.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: ShowOfficeShortcutInFavoritesBar
  - Nome da GP: Mostrar o atalho do Microsoft Office na barra Favoritos
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: ShowOfficeShortcutInFavoritesBar
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000000
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: ShowOfficeShortcutInFavoritesBar
  - Exemplo de valor:
``` xml
<false/>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### SignedHTTPExchangeEnabled
  #### Habilitar o suporte para o Signed HTTP Exchange (SXG)
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 78 ou posterior

  #### Descrição
  Habilite o suporte para o SXG (Signed HTTP Exchange).

Se essa política não for configurada ou for configurada como habilitada, o Microsoft Edge aceitará o conteúdo da Web fornecido como SXG.

Se essa política estiver configurada como desabilitada, o SXG não poderá ser carregado.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: SignedHTTPExchangeEnabled
  - Nome da GP: Habilitar o suporte para o Signed HTTP Exchange (SXG)
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: SignedHTTPExchangeEnabled
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000001
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: SignedHTTPExchangeEnabled
  - Exemplo de valor:
``` xml
<true/>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### SitePerProcess
  #### Habilitar isolamento de sites para todos os sites
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  A política [SitePerProcess](#siteperprocess) pode ser usada para impedir que os usuários recusem o comportamento padrão de isolamento de todos os sites. Observe que você também pode usar a política [IsolateOrigins](#isolateorigins) para isolar origens adicionais, mais refinadas.
Se você habilitar essa política, os usuários não poderão recusar o comportamento padrão em que cada site for executado em seu próprio processo.
Se você desabilitar ou não configurar essa política, um usuário poderá recusar o isolamento de site.  (Por exemplo, usando a entrada "Desabilitar isolamento de site" em edge://flags.)  Desabilitar a política ou não configurar a política não desliga o Isolamento de Site.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Não - Requer a reinicialização do navegador

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: SitePerProcess
  - Nome da GP: Habilitar isolamento de sites para todos os sites
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: SitePerProcess
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000001
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: SitePerProcess
  - Exemplo de valor:
``` xml
<true/>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### SpellcheckEnabled
  #### Habilitar verificação ortográfica
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Se você habilitar ou não configurar essa política, o usuário poderá usar a verificação ortográfica.

Se você desabilitar essa política, o usuário não poderá usar a verificação ortográfica, e as políticas [SpellcheckLanguage](#spellchecklanguage) e [SpellcheckLanguageBlocklist](#spellchecklanguageblocklist) também serão desabilitadas.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: SpellcheckEnabled
  - Nome da GP: Habilitar verificação ortográfica
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: SpellcheckEnabled
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000000
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: SpellcheckEnabled
  - Exemplo de valor:
``` xml
<false/>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### SpellcheckLanguage
  #### Habilitar idiomas específicos da verificação ortográfica
  >Versões com Suporte: O Microsoft Edge no Windows desde a versão 77 ou posterior

  #### Descrição
  Habilita diferentes idiomas para verificação ortográfica. Qualquer idioma especificado que não for reconhecido será ignorado.

Se você habilitar essa política, a verificação ortográfica será habilitada para os idiomas especificados, bem como os idiomas que o usuário tiver habilitado.

Se você não configurar ou desabilitar essa política, não haverá nenhuma alteração nas preferências de verificação ortográfica do usuário.

Se a política [SpellcheckEnabled](#spellcheckenabled) estiver desabilitada, essa política não terá efeito.

Se um idioma for incluído nas políticas [SpellcheckLanguage](#spellchecklanguage) e [SpellcheckLanguageBlocklist](#spellchecklanguageblocklist), o idioma da verificação ortográfica será habilitado.

Os idiomas com suporte são: af, bg, ca, cs, cy, da, de, el, en-AU, en-CA, en-GB, en-US, es, es-419, es-AR, es-ES, es-MX, es-US, et, fa, fo, fr, he, hi, hr, hu, id, it, ko, lt, lv, nb, nl, pl, pt-BR, pt-PT, ro, ru, sh, sk, sl, sq, sr, sv, ta, tg, tr, uk, vi.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Lista de cadeias de caracteres

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: SpellcheckLanguage
  - Nome da GP: Habilitar idiomas específicos da verificação ortográfica
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge\SpellcheckLanguage
  - Caminho (Recomendações): N/A
  - Nome do Valor: 1, 2, 3, ...
  - Tipo de Valor: lista de REG_SZ
  ##### Exemplo de valor:
```
SOFTWARE\Policies\Microsoft\Edge\SpellcheckLanguage\0 = "fr"
SOFTWARE\Policies\Microsoft\Edge\SpellcheckLanguage\1 = "es"

```


  

  [Voltar ao início](#microsoft-edge---políticas)

  ### SpellcheckLanguageBlocklist
  #### Aplicar a desabilitação de verificação ortográfica dos idiomas
  >Versões com Suporte: O Microsoft Edge no Windows desde a versão 78 ou posterior

  #### Descrição
  Force - desabilita os idiomas de verificação ortográfica. Os idiomas não reconhecidos nessa lista serão ignorados.

Se você habilitar essa política, a verificação ortográfica será desabilitada para os idiomas especificados. O usuário ainda poderá habilitar nem desabilitar a verificação ortográfica para os idiomas que não estão na lista.

Se você não configurar essa política ou desabilitá-la, não haverá alteração nas preferências de verificação ortográfica do usuário.

Se a política [SpellcheckEnabled](#spellcheckenabled) for desabilitada, ela não terá efeito.

Se um idioma estiver incluído nas políticas [SpellcheckLanguage](#spellchecklanguage) e [SpellcheckLanguageBlocklist](#spellchecklanguageblocklist), o idioma de verificação ortográfica será habilitado.

Os idiomas atualmente com suporte são: af, bg, ca, cs, da, de, el, en-AU, en-CA, en-GB, en-US, es, es-419, es-AR, es-ES, es-MX, es-US, et, fa, fo, fr, he, hi, hr, hu, id, it, ko, lt, lv, nb, nl, pl, pt-BR, pt-PT, ro, ru, sh, sk, sl, sq, sr, sv, ta, tg, tr, uk, vi.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Lista de cadeias de caracteres

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: SpellcheckLanguageBlocklist
  - Nome da GP: Aplicar a desabilitação de verificação ortográfica dos idiomas
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge\SpellcheckLanguageBlocklist
  - Caminho (Recomendações): N/A
  - Nome do Valor: 1, 2, 3, ...
  - Tipo de Valor: lista de REG_SZ
  ##### Exemplo de valor:
```
SOFTWARE\Policies\Microsoft\Edge\SpellcheckLanguageBlocklist\0 = "fr"
SOFTWARE\Policies\Microsoft\Edge\SpellcheckLanguageBlocklist\1 = "es"

```


  

  [Voltar ao início](#microsoft-edge---políticas)

  ### SuppressUnsupportedOSWarning
  #### Suprimir o aviso do sistema operacional sem suporte
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Suprime o aviso exibido quando o Microsoft Edge está em execução em um computador ou sistema operacional que não tem mais suporte.

Se essa política for false ou não for definida, os avisos serão exibidos nesses computadores ou sistemas operacionais que não têm suporte.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Não - Requer a reinicialização do navegador

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: SuppressUnsupportedOSWarning
  - Nome da GP: Suprimir o aviso do sistema operacional sem suporte
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: SuppressUnsupportedOSWarning
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000001
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: SuppressUnsupportedOSWarning
  - Exemplo de valor:
``` xml
<true/>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### SyncDisabled
  #### Desabilitar sincronização de dados usando os serviços de sincronização da Microsoft
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Desabilita a sincronização de dados no Microsoft Edge e impede que os usuários modifiquem essa configuração.

Se esta política não for configurada, os usuários poderão ativar ou desativar a sincronização.

Não habilite esta política quando a política "RoamingProfileSupportEnabled" estiver habilitada, pois "RoamingProfileSupportEnabled" duplica a funcionalidade de sincronização.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Sim
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: SyncDisabled
  - Nome da GP: Desabilitar sincronização de dados usando os serviços de sincronização da Microsoft
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): Modelos Administrativos/Microsoft Edge - Configurações Padrão (os usuários podem substituir)/
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): SOFTWARE\Policies\Microsoft\Edge\Recomendações
  - Nome do Valor: SyncDisabled
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000001
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: SyncDisabled
  - Exemplo de valor:
``` xml
<true/>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### TabFreezingEnabled
  #### Permitir congelamento de guias em segundo plano
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 79 ou posterior

  #### Descrição
  Controla se o Microsoft Edge pode congelar guias que estão em segundo plano há pelo menos 5 minutos.

O congelamento de guias reduz o uso da CPU, da bateria e da memória. O Microsoft Edge usa heurística para evitar o congelamento de guias que fazem trabalho útil em segundo plano, como exibir notificações, reproduzir sons e transmitir vídeos.

Se você habilitar ou não configurar essa política, as guias que estiverem em segundo plano há pelo menos 5 minutos poderão ser congeladas.

Se você desabilitar essa política, nenhuma guia será congelada.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: TabFreezingEnabled
  - Nome da GP: Permitir congelamento de guias em segundo plano
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: TabFreezingEnabled
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000000
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: TabFreezingEnabled
  - Exemplo de valor:
``` xml
<false/>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### TaskManagerEndProcessEnabled
  #### Habilitar processos finais no gerenciador de tarefas do navegador
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Se você habilitar ou não configurar essa política, os usuários poderão encerrar processos no gerenciador de tarefas do navegador. Se você desabilitá-la, os usuários não poderão encerrar processos e o botão Finalizar processo será desabilitado no gerenciador de tarefas do navegador.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: TaskManagerEndProcessEnabled
  - Nome da GP: Habilitar processos finais no gerenciador de tarefas do navegador
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: TaskManagerEndProcessEnabled
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000001
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: TaskManagerEndProcessEnabled
  - Exemplo de valor:
``` xml
<true/>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### TrackingPrevention
  #### Bloquear o rastreamento de atividades de navegação da Web dos usuários
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 78 ou posterior

  #### Descrição
  Permite que você decida se os sites devem ser bloqueados do rastreamento de atividades de navegação da Web dos usuários.

Se você habilitar essa política, terá as seguintes opções para definir o nível de prevenção de rastreamento:

0 = Desativado (sem prevenção de rastreamento)
1 = Básico (bloqueia rastreadores prejudiciais, o conteúdo e os anúncios serão personalizados)
2 = Equilibrado (bloqueia rastreadores prejudiciais e rastreadores de sites que o usuário não visitou; o conteúdo e os anúncios serão menos personalizados)
3 = Estrito (bloqueia rastreadores prejudiciais e a maioria dos rastreadores de todos os sites; o conteúdo e os anúncios terão personalização mínima. Algumas partes de sites podem não funcionar)

Se você desabilitar essa política ou não configurá-la, os usuários poderão definir o próprio nível de prevenção de rastreamento.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Número inteiro

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: TrackingPrevention
  - Nome da GP: Bloquear o rastreamento de atividades de navegação da Web dos usuários
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: TrackingPrevention
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000002
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: TrackingPrevention
  - Exemplo de valor:
``` xml
<integer>2</integer>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### TranslateEnabled
  #### Habilitar Traduzir
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Habilita o serviço de tradução integrado da Microsoft no Microsoft Edge.

Se você habilitar essa política, o Microsoft Edge oferecerá a funcionalidade de tradução ao usuário, mostrando um submenu integrado de tradução (quando apropriado) e uma opção de tradução no menu de contexto exibido quando você clica com o botão direito do mouse.

Desabilite essa política para desabilitar todos os recursos de tradução integrados.

Se você não configurar a política, os usuários poderão optar por usar a funcionalidade de tradução ou não.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Sim
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: TranslateEnabled
  - Nome da GP: Habilitar Traduzir
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): Modelos Administrativos/Microsoft Edge - Configurações Padrão (os usuários podem substituir)/
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): SOFTWARE\Policies\Microsoft\Edge\Recomendações
  - Nome do Valor: TranslateEnabled
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000001
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: TranslateEnabled
  - Exemplo de valor:
``` xml
<true/>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### URLAllowlist
  #### Definir uma lista de URLs permitidas
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Permita acesso às URLs listadas, como exceções à lista de URL bloqueadas.

Formate o padrão de URL de acordo com [https://go.microsoft.com/fwlink/?linkid=2095322](https://go.microsoft.com/fwlink/?linkid=2095322).

Você pode usar esta política para abrir exceções a listas de contatos bloqueados restritivas. Por exemplo, você pode incluir "*" na lista de contatos bloqueados para bloquear todas as solicitações e, em seguida, usar essa política para permitir o acesso a uma lista limitada de URLs. Você pode usar esta política para abrir exceções a determinados esquemas, subdomínios de outros domínios, portas ou caminhos específicos.

O filtro mais específico determina se uma URL é bloqueada ou autorizada. A lista permitida tem precedência sobre a lista de contatos bloqueados.

Esta política está limitada a 1000 entradas; as entradas subsequentes serão ignoradas.

Se você não configurar esta política, não haverá exceções para a lista de contatos bloqueados na política [URLBlocklist](#urlblocklist).

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Lista de cadeias de caracteres

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: URLAllowlist
  - Nome da GP: Definir uma lista de URLs permitidas
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge\URLAllowlist
  - Caminho (Recomendações): N/A
  - Nome do Valor: 1, 2, 3, ...
  - Tipo de Valor: lista de REG_SZ
  ##### Exemplo de valor:
```
SOFTWARE\Policies\Microsoft\Edge\URLAllowlist\0 = "contoso.com"
SOFTWARE\Policies\Microsoft\Edge\URLAllowlist\1 = "https://ssl.server.com"
SOFTWARE\Policies\Microsoft\Edge\URLAllowlist\2 = "hosting.com/good_path"
SOFTWARE\Policies\Microsoft\Edge\URLAllowlist\3 = "https://server:8080/path"
SOFTWARE\Policies\Microsoft\Edge\URLAllowlist\4 = ".exact.hostname.com"

```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: URLAllowlist
  - Exemplo de valor:
``` xml
<array>
  <string>contoso.com</string>
  <string>https://ssl.server.com</string>
  <string>hosting.com/good_path</string>
  <string>https://server:8080/path</string>
  <string>.exact.hostname.com</string>
</array>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### URLBlocklist
  #### Bloquear o acesso a uma lista de URLs
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Define uma lista de sites, com base em padrões de URL, que são bloqueados (os usuários não podem carregá-los).

Formate o padrão de URL de acordo com [https://go.microsoft.com/fwlink/?linkid=2095322](https://go.microsoft.com/fwlink/?linkid=2095322).

Você pode definir exceções na política [URLAllowlist](#urlallowlist). Essas políticas limitam-se a 1000 entradas; as entradas subsequentes serão ignoradas.

Observe que não é recomendado bloquear URLs internas "edge://*", pois isso pode causar erros inesperados.

Esta política não impede que a página seja atualizada dinamicamente por meio do JavaScript. Por exemplo, se você bloquear "contoso.com/abc", os usuários ainda poderão visitar "contoso.com" e clicar em um link para visitar "contoso.com/abc", desde que a página não seja atualizada.

Se você não configurar esta política, nenhuma URL será bloqueada.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Lista de cadeias de caracteres

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: URLBlocklist
  - Nome da GP: Bloquear o acesso a uma lista de URLs
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge\URLBlocklist
  - Caminho (Recomendações): N/A
  - Nome do Valor: 1, 2, 3, ...
  - Tipo de Valor: lista de REG_SZ
  ##### Exemplo de valor:
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


  #### Informações e configurações do Mac
  - Nome da chave de preferência: URLBlocklist
  - Exemplo de valor:
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
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### UserDataDir
  #### Definir o diretório de dados do usuário
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Defina o diretório a ser usado para armazenar dados do usuário.

Se você habilitar essa política, o Microsoft Edge usará o diretório especificado, independentemente de o usuário ter definido o sinalizador de linha de comando "--user-data-dir".

Se você não habilitar essa política, o caminho de perfil padrão será usado, mas o usuário poderá substituí-lo usando o sinalizador "--user-data-dir". Os usuários podem encontrar o diretório do perfil em edge://version/ no caminho do perfil.

Para evitar a perda de dados ou outros erros, não configure essa política para o diretório raiz de um volume ou para um diretório usado para outros fins, pois o Microsoft Edge gerencia o conteúdo.

Consulte [https://go.microsoft.com/fwlink/?linkid=2095041](https://go.microsoft.com/fwlink/?linkid=2095041) para obter uma lista de variáveis que podem ser usadas.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Não - Requer a reinicialização do navegador

  #### Tipo de Dados:
  Cadeia de Caracteres

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: UserDataDir
  - Nome da GP: Definir o diretório de dados do usuário
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: UserDataDir
  - Tipo de Valor: REG_SZ
  ##### Exemplo de valor:
```
"${users}/${user_name}/Edge"
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: UserDataDir
  - Exemplo de valor:
``` xml
<string>${users}/${user_name}/Edge</string>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### UserFeedbackAllowed
  #### Permitir comentários do usuário
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  O Microsoft Edge usa o recurso de Comentários do Edge (habilitado por padrão) para permitir que os usuários enviem comentários, sugestões ou pesquisas de clientes e para relatar qualquer problema com o navegador. Além disso, por padrão, os usuários não podem desabilitar (desativar) o recurso Comentários do Edge.

Se você habilitar essa política ou não a configurar, os usuários poderão chamar Comentários do Edge.

Se você desabilitar essa política, os usuários não poderão chamar Comentários do Edge.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Não - Requer a reinicialização do navegador

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: UserFeedbackAllowed
  - Nome da GP: Permitir comentários do usuário
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: UserFeedbackAllowed
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000001
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: UserFeedbackAllowed
  - Exemplo de valor:
``` xml
<true/>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### VideoCaptureAllowed
  #### Permitir ou bloquear captura de vídeo
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Controla se os sites podem capturar vídeo.

Se habilitada ou não configurada (padrão), o usuário será perguntado sobre o acesso de captura de vídeo para todos os sites, exceto aqueles com URLs configuradas na lista da política [VideoCaptureAllowedUrls](#videocaptureallowedurls), que terão o acesso concedido sem aviso.

Se você desabilitar esta política, o usuário não será avisado e a captura de vídeo estará disponível apenas para as URLs configuradas na política [VideoCaptureAllowedUrls](#videocaptureallowedurls).

Esta política afeta todos os tipos de entradas de vídeo, não apenas a câmera interna.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: VideoCaptureAllowed
  - Nome da GP: Permitir ou bloquear captura de vídeo
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: VideoCaptureAllowed
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000000
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: VideoCaptureAllowed
  - Exemplo de valor:
``` xml
<false/>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### VideoCaptureAllowedUrls
  #### Sites que podem acessar dispositivos de captura de vídeo sem solicitar permissão
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Especifica sites, com base nos padrões de URL, que podem usar dispositivos de captura de vídeo sem pedir permissão ao usuário. Os padrões nessa lista são comparados com a origem de segurança da URL solicitante. Se forem iguais, o site automaticamente terá acesso aos dispositivos de captura de vídeo.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Lista de cadeias de caracteres

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: VideoCaptureAllowedUrls
  - Nome da GP: Sites que podem acessar dispositivos de captura de vídeo sem solicitar permissão
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge\VideoCaptureAllowedUrls
  - Caminho (Recomendações): N/A
  - Nome do Valor: 1, 2, 3, ...
  - Tipo de Valor: lista de REG_SZ
  ##### Exemplo de valor:
```
SOFTWARE\Policies\Microsoft\Edge\VideoCaptureAllowedUrls\0 = "https://www.contoso.com/"
SOFTWARE\Policies\Microsoft\Edge\VideoCaptureAllowedUrls\1 = "https://[*.]contoso.edu/"

```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: VideoCaptureAllowedUrls
  - Exemplo de valor:
``` xml
<array>
  <string>https://www.contoso.com/</string>
  <string>https://[*.]contoso.edu/</string>
</array>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### WPADQuickCheckEnabled
  #### Definir otimização de WPAD
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Permite que você desative a otimização WPAD (Descoberta Automática de Proxy da Web) no Microsoft Edge.

Se você desabilitar esta política, a otimização de WPAD será desabilitada, o que faz o navegador aguardar mais tempo pelos servidores WPAD baseados em DNS.

Se você habilitar ou não configurar a política, a otimização WPAD será habilitada.

Independentemente de a política estar habilitada ou de como está habilitada, a configuração da otimização WPAD não pode ser alterada pelos usuários.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Não - Requer a reinicialização do navegador

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: WPADQuickCheckEnabled
  - Nome da GP: Definir otimização de WPAD
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: WPADQuickCheckEnabled
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000001
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: WPADQuickCheckEnabled
  - Exemplo de valor:
``` xml
<true/>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### WebAppInstallForceList
  #### Configurar lista de Aplicativos Web instalados à força
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 80 ou posterior

  #### Descrição
  Especifica uma lista de sites que estão instalados no modo silencioso, sem interação do usuário, e que não podem ser desinstalados nem desabilitados pelo usuário.

Cada item da lista da política é um objeto com os seguintes membros:
  - "url", que é obrigatório. "url" deve ser a URL do aplicativo web a ser instalado.

Os valores para os membros opcionais são:
  - "launch_container" deve ser "window" ou "tab" para indicar como o aplicativo Web será aberto depois de instalado.
  - "create_desktop_shortcut" deve ser true se um atalho da área de trabalho precisar ser criado no Windows.

Se "default_launch_container" for omitido, o aplicativo será aberto em uma guia por padrão. Independentemente do valor de "default_launch_container", os usuários poderão alterar o contêiner no qual o aplicativo será aberto. Se "create_desktop_shortcuts" for omitido, não serão criados atalhos da área de trabalho.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Dicionário

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: WebAppInstallForceList
  - Nome da GP: Configurar lista de Aplicativos Web instalados à força
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: WebAppInstallForceList
  - Tipo de Valor: REG_SZ
  ##### Exemplo de valor:
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


  #### Informações e configurações do Mac
  - Nome da chave de preferência: WebAppInstallForceList
  - Exemplo de valor:
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
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### WebDriverOverridesIncompatiblePolicies
  #### Permitir que o WebDriver substitua políticas incompatíveis
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Esta política foi removida do M80, pois ela não é mais necessária, uma vez que
o WebDriver agora é compatível com todas as políticas existentes.

Esta política permite que os usuários do recurso WebDriver substituam
políticas que podem interferir em sua operação.

Atualmente, essa política desabilita as políticas [SitePerProcess](#siteperprocess) e [IsolateOrigins](#isolateorigins).

Se a política estiver habilitada, o WebDriver poderá substituir políticas
incompatíveis.
Se a política estiver desabilitada ou não configurada, o WebDriver não poderá
substituir políticas incompatíveis.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Não - Requer a reinicialização do navegador

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: WebDriverOverridesIncompatiblePolicies
  - Nome da GP: Permitir que o WebDriver substitua políticas incompatíveis
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: WebDriverOverridesIncompatiblePolicies
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000001
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: WebDriverOverridesIncompatiblePolicies
  - Exemplo de valor:
``` xml
<true/>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### WebRtcLocalIpsAllowedUrls
  #### Gerenciar a exposição de endereços IP locais pelo WebRTC
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 80 ou posterior

  #### Descrição
  Especifica uma lista de origens (URLs) ou padrões de nome de host (como "*contoso.com*") para os quais o endereço IP local deve ser exposto pelo WebRTC.

Se você habilitar essa política e definir uma lista de origens (URLs) ou padrões de nome de host, quando edge://flags/#enable-webrtc-hide-local-ips-with-mdns estiver habilitado, o WebRTC mostrará o endereço IP local para casos que corresponderem aos padrões na lista.

Se você desabilitar ou não configurar essa política e edge://flags/#enable-webrtc-hide-local-ips-with-mdns estiver habilitado, o WebRTC não mostrará os endereços IP locais. O endereço IP local é oculto por um nome de host mDNS.

Se você habilitar, desabilitar ou não configurar essa política e edge://flags/#enable-webrtc-hide-local-ips-with-mdns estiver desabilitado, o WebRTC mostrará endereços IP locais.

Observe que essa política enfraquece a proteção de endereços IP locais que podem ser necessária para os administradores.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Não - Requer a reinicialização do navegador

  #### Tipo de Dados:
  Lista de cadeias de caracteres

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: WebRtcLocalIpsAllowedUrls
  - Nome da GP: Gerenciar a exposição de endereços IP locais pelo WebRTC
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge\WebRtcLocalIpsAllowedUrls
  - Caminho (Recomendações): N/A
  - Nome do Valor: 1, 2, 3, ...
  - Tipo de Valor: lista de REG_SZ
  ##### Exemplo de valor:
```
SOFTWARE\Policies\Microsoft\Edge\WebRtcLocalIpsAllowedUrls\0 = "https://www.contoso.com"
SOFTWARE\Policies\Microsoft\Edge\WebRtcLocalIpsAllowedUrls\1 = "*contoso.com*"

```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: WebRtcLocalIpsAllowedUrls
  - Exemplo de valor:
``` xml
<array>
  <string>https://www.contoso.com</string>
  <string>*contoso.com*</string>
</array>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### WebRtcLocalhostIpHandling
  #### Restringir a exposição do endereço IP local pelo WebRTC
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Permite definir se o WebRTC mostra ou não o endereço IP local do usuário.

Se você configurar esta política para "AllowAllInterfaces" ('default') ou "AllowPublicAndPrivateInterfaces" ('default_public_and_private_interfaces'), o WebRTC mostrará o endereço IP local.

Se você configurar esta política para "AllowPublicInterfaceOnly" ('default_public_interface_only') ou "DisableNonProxiedUdp" ('disable_non_proxied_udp'), o WebRTC não mostrará o endereço IP local.

Se você não configurar esta política ou desabilitá-la, o WebRTC mostrará o endereço IP local.

  * 'default' = Permitir todas as interfaces. Isso expõe o endereço IP local.
  * 'default_public_and_private_interfaces' = Permitir interfaces públicas e privadas pela rota http padrão. Isso mostra o endereço IP local.
  * 'default_public_interface_only' = Permitir a interface pública pela rota http padrão. Isso não mostra o endereço IP local.
  * 'disable_non_proxied_udp’ = Usar TCP, a menos que o servidor proxy dê suporte para UDP. Isso não mostra o endereço IP local.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Não - Requer a reinicialização do navegador

  #### Tipo de Dados:
  Cadeia de Caracteres

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: WebRtcLocalhostIpHandling
  - Nome da GP: Restringir a exposição do endereço IP local pelo WebRTC
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: WebRtcLocalhostIpHandling
  - Tipo de Valor: REG_SZ
  ##### Exemplo de valor:
```
"default"
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: WebRtcLocalhostIpHandling
  - Exemplo de valor:
``` xml
<string>default</string>
```
  

  [Voltar ao início](#microsoft-edge---políticas)

  ### WebRtcUdpPortRange
  #### Restringir o intervalo de portas UDP locais usadas pelo WebRTC
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Restringe o intervalo de portas UDP usado pelo WebRTC a um intervalo de portas especificado (pontos de extremidade incluídos).

Ao configurar essa política, você especifica o intervalo de portas UDP locais que o WebRTC pode usar.

Se você não configurar essa política, ou se defini-la como uma cadeia de caracteres vazia ou um intervalo de portas inválido, o WebRTC poderá usar qualquer porta UDP local disponível.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Não - Requer a reinicialização do navegador

  #### Tipo de Dados:
  Cadeia de Caracteres

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: WebRtcUdpPortRange
  - Nome da GP: Restringir o intervalo de portas UDP locais usadas pelo WebRTC
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: WebRtcUdpPortRange
  - Tipo de Valor: REG_SZ
  ##### Exemplo de valor:
```
"10000-11999"
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: WebRtcUdpPortRange
  - Exemplo de valor:
``` xml
<string>10000-11999</string>
```
  

  [Voltar ao início](#microsoft-edge---políticas)


## Consulte também
- [Configurando o Microsoft Edge](configure-microsoft-edge.md)
- [Página inicial do Microsoft Edge Enterprise](https://aka.ms/EdgeEnterprise)