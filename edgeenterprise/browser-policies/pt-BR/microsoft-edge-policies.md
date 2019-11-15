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
|[DefaultJavaScriptSetting](#defaultjavascriptsetting)|Configuração de JavaScript padrão|
|[DefaultNotificationsSetting](#defaultnotificationssetting)|Configuração de notificação padrão|
|[DefaultPluginsSetting](#defaultpluginssetting)|Configuração padrão do Adobe Flash|
|[DefaultPopupsSetting](#defaultpopupssetting)|Configuração de janela pop-up padrão|
|[DefaultWebBluetoothGuardSetting](#defaultwebbluetoothguardsetting)|Controlar o uso da API Web Bluetooth|
|[DefaultWebUsbGuardSetting](#defaultwebusbguardsetting)|Controlar o uso da API WebUSB|
|[ImagesAllowedForUrls](#imagesallowedforurls)|Permitir imagens nestes sites|
|[ImagesBlockedForUrls](#imagesblockedforurls)|Bloquear imagens em sites específicos|
|[JavaScriptAllowedForUrls](#javascriptallowedforurls)|Permitir JavaScript em sites específicos|
|[JavaScriptBlockedForUrls](#javascriptblockedforurls)|Bloquear o JavaScript em sites específicos|
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
|[SmartScreenPuaEnabled](#smartscreenpuaenabled)|Configure Microsoft Defender SmartScreen to block potentially unwanted apps|
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
|[NewTabPageSetFeedType](#newtabpagesetfeedtype)|Configure the Microsoft Edge new tab page experience|
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
|[AlwaysOpenPdfExternally](#alwaysopenpdfexternally)|Sempre abrir arquivos PDF externamente|
|[ApplicationLocaleValue](#applicationlocalevalue)|Definir localidade do aplicativo|
|[AudioCaptureAllowed](#audiocaptureallowed)|Permitir ou bloquear captura de áudio|
|[AudioCaptureAllowedUrls](#audiocaptureallowedurls)|Sites podem acessar dispositivos de captura áudio sem solicitar permissão|
|[AutoImportAtFirstRun](#autoimportatfirstrun)|Importar automaticamente os dados e as configurações de outro navegador na primeira execução|
|[AutofillAddressEnabled](#autofilladdressenabled)|Habilitar AutoPreenchimento para endereços|
|[AutofillCreditCardEnabled](#autofillcreditcardenabled)|Habilitar AutoPreenchimento para cartões de crédito|
|[AutoplayAllowed](#autoplayallowed)|Permitir reprodução automática de mídia para sites|
|[BackgroundModeEnabled](#backgroundmodeenabled)|Continuar executando apps em segundo plano depois que o Microsoft Edge for fechado|
|[BackgroundTemplateListUpdatesEnabled](#backgroundtemplatelistupdatesenabled)|Permite atualizações em segundo plano na lista de modelos disponíveis para Coleções e outros recursos que usam modelos.|
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
|[ExternalProtocolDialogShowAlwaysOpenCheckbox](#externalprotocoldialogshowalwaysopencheckbox)|Show an "Always open" checkbox in external protocol dialog.|
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
|[InternetExplorerIntegrationSiteRedirect](#internetexplorerintegrationsiteredirect)|Especificar como as navegações "em página" para sites não configurados se comportam ao iniciar em páginas do modo do Internet Explorer|
|[IsolateOrigins](#isolateorigins)|Habilitar isolamento de site para origens específicas|
|[ManagedFavorites](#managedfavorites)|Configurar favoritos|
|[ManagedSearchEngines](#managedsearchengines)|Gerenciar Mecanismos de Pesquisa|
|[MaxConnectionsPerProxy](#maxconnectionsperproxy)|Número máximo de conexões simultâneas com o servidor proxy|
|[MediaRouterCastAllowAllIPs](#mediaroutercastallowallips)|Permitir que o Google Cast se conecte a dispositivos Cast em todos os endereços IP|
|[MetricsReportingEnabled](#metricsreportingenabled)|Habilitar relatórios de dados relacionados a uso e falhas|
|[NetworkPredictionOptions](#networkpredictionoptions)|Habilitar previsão de rede|
|[NonRemovableProfileEnabled](#nonremovableprofileenabled)|Configurar se um usuário sempre tem um perfil padrão conectado automaticamente à sua conta corporativa ou de estudante|
|[OverrideSecurityRestrictionsOnInsecureOrigin](#overridesecurityrestrictionsoninsecureorigin)|Controlar onde se aplicam a restrições de segurança em origens não seguras|
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
|[TabFreezingEnabled](#tabfreezingenabled)|Allow freezing of background tabs|
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
|[WebDriverOverridesIncompatiblePolicies](#webdriveroverridesincompatiblepolicies)|Permitir que o WebDriver substitua políticas incompatíveis|
|[WebRtcLocalhostIpHandling](#webrtclocalhostiphandling)|Restringir a exposição do endereço IP do localhost pelo WebRTC|
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
  Set this policy to true to show the Cast toolbar icon on the toolbar or the overflow menu. Users won't be able to remove it.

If you don't configure this policy or if you disable it, users can pin or remove the icon by using its contextual menu.

If you've also set the [EnableMediaRouter](#enablemediarouter) policy to false, then this policy is ignored, and the toolbar icon isn't shown.

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
  Specify a list of sites, based on URL patterns, for which Microsoft Edge should automatically select a client certificate, if the site requests one.

The value must be an array of stringified JSON dictionaries. Each dictionary must have the form { "pattern": "$URL_PATTERN", "filter" : $FILTER }, where $URL_PATTERN is a content setting pattern. $FILTER restricts from which client certificates the browser will automatically select. Independent of the filter, only certificates will be selected that match the server's certificate request. For example, if $FILTER has the form { "ISSUER": { "CN": "$ISSUER_CN" } }, additionally only client certificates are selected that are issued by a certificate with the CommonName $ISSUER_CN. If $FILTER contains an "ISSUER" and a "SUBJECT" section, a client certificate must satisfy both conditions to be selected. If $FILTER specifies an organization ("O"), a certificate must have at least one organization which matches the specified value to be selected. If $FILTER specifies an organization unit ("OU"), a certificate must have at least one organization unit which matches the specified value to be selected. If $FILTER is the empty dictionary {}, the selection of client certificates is not additionally restricted.

If you don't configure this policy, auto-selection isn't done for any site.

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
  Define a list of sites, based on URL patterns, that are allowed to set cookies.

If you don't configure this policy, the global default value from the [DefaultCookiesSetting](#defaultcookiessetting) policy (if set) or the user's personal configuration is used for all sites.

See the [CookiesBlockedForUrls](#cookiesblockedforurls) and [CookiesSessionOnlyForUrls](#cookiessessiononlyforurls) policies for more information.

Note there cannot be conflicting URL patterns set between these three policies:

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
  Define a list of sites, based on URL patterns, that can't set cookies.

If you don't configure this policy, the global default value from the [DefaultCookiesSetting](#defaultcookiessetting) policy (if set) or the user's personal configuration is used for all sites.

See the [CookiesAllowedForUrls](#cookiesallowedforurls) and [CookiesSessionOnlyForUrls](#cookiessessiononlyforurls) policies for more information.

Note there cannot be conflicting URL patterns set between these three policies:

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
  Cookies created by websites that match a URL pattern you define are deleted when the session ends (when the window closes).

Cookies created by websites that don't match the pattern are controlled by the [DefaultCookiesSetting](#defaultcookiessetting) policy (if set) or by the user's personal configuration. This is also the default behavior if you don't configure this policy.

If Microsoft Edge is running in background mode, the session might not close when the last window is closed, meaning the cookies won't be cleared when the window closes. See the [BackgroundModeEnabled](#backgroundmodeenabled) policy for information about configuring what happens when Microsoft Edge runs in background mode.

You can also use the [CookiesAllowedForUrls](#cookiesallowedforurls) and [CookiesBlockedForUrls](#cookiesblockedforurls) policies to control which websites can create cookies.

Note there cannot be conflicting URL patterns set between these three policies:

- [CookiesBlockedForUrls](#cookiesblockedforurls)

- [CookiesAllowedForUrls](#cookiesallowedforurls)

- CookiesSessionOnlyForUrls

If you set the [RestoreOnStartup](#restoreonstartup) policy to restore URLs from previous sessions, this policy is ignored, and cookies are stored permanently for those sites.

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
  Control whether websites can create cookies on the user's device. This policy is all or nothing - you can let all websites create cookies, or no websites create cookies. You can't use this policy to enable cookies from specific websites.

Set the policy to 'SessionOnly' (4) to clear cookies when the session closes. If Microsoft Edge is running in background mode, the session might not close when the last window is closed, meaning the cookies won't be cleared when the window closes. See [BackgroundModeEnabled](#backgroundmodeenabled) policy for information about configuring what happens when Microsoft Edge runs in background mode.

If you don't configure this policy, the default 'AllowCookies' (1) is used, and users can change this setting in Microsoft Edge Settings. (If you don't want users to be able to change this setting, set the policy.)

* 1 = Let all sites create cookies

* 2 = Don't let any site create cookies

* 4 = Keep cookies for the duration of the session

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
  Determines whether websites that aren't covered by [PluginsAllowedForUrls](#pluginsallowedforurls) or [PluginsBlockedForUrls](#pluginsblockedforurls) can automatically run the Adobe Flash plug-in. You can select 'BlockPlugins' (2) to block Adobe Flash on all sites, or you can select 'ClickToPlay' (3) to let Adobe Flash run but require the user to click the placeholder to start it. In any case, the [PluginsAllowedForUrls](#pluginsallowedforurls) and [PluginsBlockedForUrls](#pluginsblockedforurls) policies take precedence over 'DefaultPluginsSetting'.

Automatic playback is only allowed for domains explicitly listed in the [PluginsAllowedForUrls](#pluginsallowedforurls) policy. If you want to enable automatic playback for all sites, consider adding http://* and https://* to this list.

If you don't configure this policy, the user can change this setting manually.

* 2 = Block the Adobe Flash plug-in

* 3 = Click to play

The former '1' option set allow-all, but this functionality is now only handled by the [PluginsAllowedForUrls](#pluginsallowedforurls) policy.  Existing policies using '1' will operate in Click-to-play mode.

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
  Set whether websites can access connected USB devices. You can completely block access or ask the user each time a website wants to get access to connected USB devices.

You can override this policy for specific URL patterns by using the [WebUsbAskForUrls](#webusbaskforurls) and [WebUsbBlockedForUrls](#webusbblockedforurls) policies.

If you don't configure this policy, sites can ask users whether they can access the connected USB devices (3) by default, and users can change this setting.

* 2 = Don't allow any site to request access to USB devices via the WebUSB API

* 3 = Allow sites to ask the user to grant access to a connected USB device

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
  Define a list of sites, based on URL patterns, that can display images.

If you don't configure this policy, the global default value is used for all sites either from the [DefaultImagesSetting](#defaultimagessetting) policy (if set) or the user's personal configuration.

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
  Define a list of sites, based on URL patterns, that aren't allowed to display images.

If you don't configure this policy, the global default value from the [DefaultImagesSetting](#defaultimagessetting) policy (if set) or the user's personal configuration is used for all sites.

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

  ### JavaScriptAllowedForUrls
  #### Permitir JavaScript em sites específicos
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Define a list of sites, based on URL patterns, that are allowed to run JavaScript.

If you don't configure this policy, the global default value from the [DefaultJavaScriptSetting](#defaultjavascriptsetting) policy (if set) or the user's personal configuration is used for all sites.

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
  Define a list of sites, based on URL patterns, that aren't allowed to run JavaScript.

If you don't configure this policy, the global default value from the [DefaultJavaScriptSetting](#defaultjavascriptsetting) policy (if set) or the user's personal configuration is used for all sites.

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

  ### NotificationsAllowedForUrls
  #### Permitir notificações em sites específicos
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Define a list of sites, based on URL patterns, that can display notifications.

If you don't configure this policy, the global default value from the [DefaultNotificationsSetting](#defaultnotificationssetting) policy (if set) or the user's personal configuration is used for all sites.

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
  Define a list of sites, based on URL patterns, that are blocked from displaying notifications.

If you don't configure this policy, the global default value from the [DefaultNotificationsSetting](#defaultnotificationssetting) policy (if set) or the user's personal configuration is used for all sites.

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
  Define a list of sites, based on URL patterns, that can run the Adobe Flash plug-in.

If you don't configure this policy, the global default value from the [DefaultPluginsSetting](#defaultpluginssetting) policy (if set) or the user's personal configuration is used for all sites.

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
  Define a list of sites, based on URL patterns, that are blocked from running Adobe Flash.

If you don't configure this policy, the global default value from the [DefaultPluginsSetting](#defaultpluginssetting) policy (if set) or the user's personal configuration is used for all sites.

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
  Define a list of sites, based on URL patterns, that can open pop-up windows.

If you don't configure this policy, the global default value from the [DefaultPopupsSetting](#defaultpopupssetting) policy (if set) or the user's personal configuration is used for all sites.

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
  Define a list of sites, based on URL patterns, that are blocked from opening pop-up windows.

If you don't configure this policy, the global default value from the [DefaultPopupsSetting](#defaultpopupssetting) policy (if set) or the user's personal configuration is used for all sites.

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
  Allows you to set a list of urls that specify which sites will automatically be granted permission to access a USB device with the given vendor and product IDs. Each item in the list must contain both devices and urls in order for the policy to be valid. Each item in devices can contain a vendor ID and product ID field. Any ID that is omitted is treated as a wildcard with one exception, and that exception is that a product ID cannot be specified without a vendor ID also being specified. Otherwise, the policy will not be valid and will be ignored.

The USB permission model uses the URL of the requesting site ("requesting URL") and the URL of the top-level frame site ("embedding URL") to grant permission to the requesting URL to access the USB device. The requesting URL may be different than the embedding URL when the requesting site is loaded in an iframe. Therefore, the "urls" field can contain up to two URL strings delimited by a comma to specify the requesting and embedding URL respectively. If only one URL is specified, then access to the corresponding USB devices will be granted when the requesting site's URL matches this URL regardless of embedding status. The URLs in "urls" must be valid URLs, otherwise the policy will be ignored.

If this policy is left not set, the global default value will be used for all sites either from the [DefaultWebUsbGuardSetting](#defaultwebusbguardsetting) policy if it is set, or the user's personal configuration otherwise.

URL patterns in this policy should not clash with the ones configured via [WebUsbBlockedForUrls](#webusbblockedforurls). If there is a clash, this policy will take precedence over [WebUsbBlockedForUrls](#webusbblockedforurls) and [WebUsbAskForUrls](#webusbaskforurls).

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
  Define a list of sites, based on URL patterns, that can ask the user for access to a USB device.

If you don't configure this policy, the global default value from the [DefaultWebUsbGuardSetting](#defaultwebusbguardsetting) policy (if set) or the user's personal configuration is used for all sites.

The URL patterns defined in this policy can't conflict with those configured in the [WebUsbBlockedForUrls](#webusbblockedforurls) policy - you can't both allow and block a URL.

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
  Define a list of sites, based on URL patterns, that can't ask the user to grant them access to a USB device.

If you don't configure this policy, the global default value from the [DefaultWebUsbGuardSetting](#defaultwebusbguardsetting) policy (if set) or the user's personal configuration is used for all sites.

URL patterns in this policy can't conflict with those configured in the [WebUsbAskForUrls](#webusbaskforurls) policy. You can't both allow and block a URL.

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
  Essa política permite determinar se os usuários poderão ignorar os avisos do Microsoft Defender SmartScreen sobre downloads não verificados.

Se você habilitar essa configuração, os usuários na sua organização não poderão ignorar os avisos do Microsoft Defender SmartScreen, e eles ficarão impedidos de concluir os downloads não verificados.

Se você desabilitar ou não configurar essa política, os usuários poderão ignorar os avisos do Microsoft Defender SmartScreen e concluirão os downloads não verificados.

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
Essa política está disponível somente em instâncias do Windows que façam parte de um domínio do Microsoft Active Directory; ou em instâncias do Windows 10 Pro ou Enterprise registradas para o gerenciamento de dispositivos.
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
  This policy setting lets you configure whether to turn on Microsoft Defender SmartScreen. Microsoft Defender SmartScreen provides warning messages to help protect your users from potential phishing scams and malicious software. By default, Microsoft Defender SmartScreen is turned on.

If you enable this setting, Microsoft Defender SmartScreen is turned on.

If you disable this setting, Microsoft Defender SmartScreen is turned off.

If you don't configure this setting, users can choose whether to use Microsoft Defender SmartScreen.

This policy is available only on Windows instances that are joined to a Microsoft Active Directory domain; or on Windows 10 Pro or Enterprise instances that are enrolled for device management.

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
  #### Configure Microsoft Defender SmartScreen to block potentially unwanted apps
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 80 ou posterior

  #### Descrição
  This policy setting lets you configure whether to turn on blocking for potentially unwanted apps in Microsoft Defender SmartScreen. Potentially unwanted app blocking in Microsoft Defender SmartScreen provides warning messages to help protect users from adware, coin miners, bundleware, and other low-reputation apps that are hosted by websites. Potentially unwanted app blocking in Microsoft Defender SmartScreen is turned off by default.

If you enable this setting, potentially unwanted app blocking in Microsoft Defender SmartScreen is turned on.

If you disable this setting, potentially unwanted app blocking in Microsoft Defender SmartScreen is turned off.

If you don't configure this setting, users can choose whether to use potentially unwanted app blocking in Microsoft Defender SmartScreen.

This policy is available only on Windows instances that are joined to a Microsoft Active Directory domain; or on Windows 10 Pro or Enterprise instances that are enrolled for device management.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Sim
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: SmartScreenPuaEnabled
  - Nome da GP: Configure Microsoft Defender SmartScreen to block potentially unwanted apps
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
  Controls which extension types can be installed and limits runtime access.

This setting defines the allowed types of extensions and which hosts they can interact with. The value is a list of strings, each of which should be one of the following: "extension", "theme", "user_script", and "hosted_app". See the Microsoft Edge extensions documentation for more information on these types.

Note that this policy also affects extensions to be force-installed by using [ExtensionInstallForcelist](#extensioninstallforcelist) policy.

If you enable this policy, only extensions that match a type in the list are installed.

If you don't configure this policy, no restrictions on the acceptable extension types are enforced.

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
  Define URLs that can install extensions and themes.

By default, users have to download a *.crx file for each extension or script they want to install, and then drag it onto the Microsoft Edge settings page. This policy lets specific URLs use install the extension or script for the user.

Each item in this list is an extension-style match pattern (see [https://go.microsoft.com/fwlink/?linkid=2095039](https://go.microsoft.com/fwlink/?linkid=2095039)). Users can easily install items from any URL that matches an item in this list. Both the location of the *.crx file and the page where the download is started from (in other words, the referrer) must be allowed by these patterns.

The [ExtensionInstallBlocklist](#extensioninstallblocklist) policy takes precedence over this policy. Any extensions that's on the block list won't be installed, even if it comes from a site on this list.

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
  Allows you to control when to trigger password protection warning. Password protection alerts users when they reuse their protected password on potentially suspicious sites.

You can use the [PasswordProtectionLoginURLs](#passwordprotectionloginurls) and [PasswordProtectionChangePasswordURL](#passwordprotectionchangepasswordurl) policies to configure which passwords to protect.

Exemptions: Passwords for the sites listed in [PasswordProtectionLoginURLs](#passwordprotectionloginurls) and [PasswordProtectionChangePasswordURL](#passwordprotectionchangepasswordurl), as well as for the sites listed in [SmartScreenAllowListDomains](#smartscreenallowlistdomains), will not trigger a password-protection warning.

Set to 'PasswordProtectionWarningOff' (0) to not show password protection warningss.

Set to 'PasswordProtectionWarningOnPasswordReuse' (1) to show password protection warnings when the user reuses their protected password on a non-whitelisted site.

If you disable or don't configure this policy, then the warning trigger is not shown.

* 0 = Password protection warning is off.

* 1 = Password protection warning is triggered by password reuse.

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
  Configures the default home page URL in Microsoft Edge.

The home page is the page opened by the Home button. The pages that open on startup are controlled by the [RestoreOnStartup](#restoreonstartup) policies.

You can either set a URL here or set the home page to open the new tab page. If you select to open the new tab page, then this policy doesn't take effect.

If you enable this policy, users can't change their home page URL, but they can choose to use the new tab page as their home page.

If you disable or don't configure this policy, users can choose their own home page, as long as the [HomepageIsNewTabPage](#homepageisnewtabpage) policy isn't enabled.

This policy is available only on Windows instances that are joined to a Microsoft Active Directory domain or Windows 10 Pro or Enterprise instances enrolled for device management.

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

O 'default_logo' é obrigatório e será usado quando não houver imagem de fundo. Se o 'light_logo' for fornecido, ele será usado quando a página de nova guia do usuário tiver uma imagem de fundo. Recomendamos um logotipo horizontal com um fundo transparente que seja alinhado à esquerda e centralizado verticalmente. O logotipo deve ter uma altura mínima de 32 pixels e uma taxa de proporção de 1:1 a 4:1. O 'default_logo' deve ter um contraste adequado contra um fundo branco/preto, enquanto o 'light_logo' deve ter um contraste adequado contra uma imagem de fundo.

Se você habilitar essa política, o Microsoft Edge baixará e mostrará os logotipos especificados na página de nova guia. Os usuários não podem substituir ou ocultar os logotipos.

Se você desabilitar ou não configurar essa política, o Microsoft Edge não mostrará o logotipo da empresa ou um logotipo da Microsoft na página de nova guia.

Para obter ajuda na determinação do hash SHA-256, consulte https://docs.microsoft.com/en-us/powershell/module/microsoft.powershell.utility/get-filehash?view=powershell-6.

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
  Configures the default URL for the new tab page.

This policy determines the page that's opened when new tabs are created (including when new windows are opened). It also affects the startup page if that's set to open to the new tab page.

This policy doesn't determine which page opens on startup; that's controlled by the [RestoreOnStartup](#restoreonstartup) policy. It also doesn’t affect the home page if that’s set to open to the new tab page.

If you don't configure this policy, the default new tab page is used.

If you configure this policy *and* the [NewTabPageSetFeedType](#newtabpagesetfeedtype) policy, this policy has precedence.

If an invalid URL is provided, new tabs will open about://blank.

This policy is available only on Windows instances that are joined to a Microsoft Active Directory domain or Windows 10 Pro or Enterprise instances that are enrolled for device management.

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
  #### Configure the Microsoft Edge new tab page experience
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 79 ou posterior

  #### Descrição
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

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Sim
  - Atualização de política dinâmica: Sim

  #### Tipo de Dados:
  Número inteiro

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: NewTabPageSetFeedType
  - Nome da GP: Configure the Microsoft Edge new tab page experience
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
  Specify a list of websites to open automatically when the browser starts. If you don't configure this policy, no site is opened on startup.

This policy only works if you also set the [RestoreOnStartup](#restoreonstartup) policy to 'Open a list of URLs' (4).

This policy is only available on Windows instances that are joined to a Microsoft Active Directory domain or Windows 10 Pro or Enterprise instances that are enrolled for device management.

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
  List specific native messaging hosts that users can use in Microsoft Edge.

By default, all native messaging hosts are allowed. If you set the [NativeMessagingBlocklist](#nativemessagingblocklist) policy to *, all native messaging hosts are blocked, and only native messaging hosts listed in here are loaded.

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
  Specify the character encodings supported by the search provider. Encodings are code page names like UTF-8, GB2312, and ISO-8859-1. They are tried in the order provided.

This policy is optional. If not configured, the default, UTF-8, is used.

This policy is applied only if you enable the [DefaultSearchProviderEnabled](#defaultsearchproviderenabled) and [DefaultSearchProviderSearchURL](#defaultsearchprovidersearchurl) policies.

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
  Specifies the URL to the search engine used for image search. Search requests are sent using the GET method.

This policy is optional. If you don't configure it, image search isn't available.

Specify Bing's Image Search URL as:
'{bing:baseURL}images/detail/search?iss=sbiupload&FORM=ANCMS1#enterInsights'.

Specify Google's Image Search URL as: '{google:baseURL}searchbyimage/upload'.

See [DefaultSearchProviderImageURLPostParams](#defaultsearchproviderimageurlpostparams) policy to finish configuring image search.

This policy is applied only if you enable the [DefaultSearchProviderEnabled](#defaultsearchproviderenabled) and [DefaultSearchProviderSearchURL](#defaultsearchprovidersearchurl) policies.

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
  If you enable this policy, it specifies the parameters used when an image search that uses POST is performed. The policy consists of comma-separated name/value pairs. If a value is a template parameter, like {imageThumbnail} in the preceding example, it’s replaced with real image thumbnail data. This policy is applied only if you enable the [DefaultSearchProviderEnabled](#defaultsearchproviderenabled) and [DefaultSearchProviderSearchURL](#defaultsearchprovidersearchurl) policies.

Specify Bing's Image Search URL Post Params as:
'imageBin={google:imageThumbnailBase64}'.

Specify Google's Image Search URL Post Params as:
'encoded_image={google:imageThumbnail},image_url={google:imageURL},sbisrc={google:imageSearchSource},original_width={google:imageOriginalWidth},original_height={google:imageOriginalHeight}'.

If you don’t set this policy, image search requests are sent using the GET method.

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
  Specifies the keyword, which is the shortcut used in the Address Bar to trigger the search for this provider.

This policy is optional. If you don't configure it, no keyword activates the search provider.

This policy is applied only if you enable the [DefaultSearchProviderEnabled](#defaultsearchproviderenabled) and [DefaultSearchProviderSearchURL](#defaultsearchprovidersearchurl) policies.

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
  Specifies the name of the default search provider.

If you enable this policy, you set the name of the default search provider.

If you don't enable this policy or if you leave it empty, the host name specified by the search URL is used.

'DefaultSearchProviderName' should be set to an organization-approved encrypted search provider that corresponds to the encrypted search provider set in DTBC-0008. This policy is applied only if you enable the [DefaultSearchProviderEnabled](#defaultsearchproviderenabled) and [DefaultSearchProviderSearchURL](#defaultsearchprovidersearchurl) policies.

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
  Specifies the URL of the search engine used for a default search. The URL contains the string '{searchTerms}', which is replaced at query time by the terms the user is searching for.

Specify Bing's search URL as:

'{bing:baseURL}search?q={searchTerms}'.

Specify Google's search URL as: '{google:baseURL}search?q={searchTerms}&{google:RLZ}{google:originalQueryForSuggestion}{google:assistedQueryStats}{google:searchFieldtrialParameter}{google:searchClient}{google:sourceId}ie={inputEncoding}'.

This policy is required when you enable the [DefaultSearchProviderEnabled](#defaultsearchproviderenabled) policy; if you don't enable the latter policy, this policy is ignored.

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
  Specifies the URL for the search engine used to provide search suggestions. The URL contains the string '{searchTerms}', which is replaced at query time by the text the user has entered so far.

This policy is optional. If you don't configure it, users won't see search suggestions; they will see suggestions from their browsing history and favorites.

Bing's suggest URL can be specified as:

'{bing:baseURL}qbox?query={searchTerms}'.

Google's suggest URL can be specified as: '{google:baseURL}complete/search?output=chrome&q={searchTerms}'.

This policy is applied only if you enable the [DefaultSearchProviderEnabled](#defaultsearchproviderenabled) and [DefaultSearchProviderSearchURL](#defaultsearchprovidersearchurl) policies.

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
  Defines a list of hosts for which Microsoft Edge bypasses any proxy.

This policy is applied only if you have selected 'Use fixed proxy servers' in the [ProxyMode](#proxymode) policy. If you selected any other mode for configuring proxy policies, don't enable or configure this policy.

If you enable this policy, you can create a list of hosts for which Microsoft Edge doesn't use a proxy.

If you don't configure this policy, no list of hosts is created for which Microsoft Edge bypasses a proxy. Leave this policy unconfigured if you've specified any other method for setting proxy policies.

For more detailed examples go to [https://go.microsoft.com/fwlink/?linkid=2094936](https://go.microsoft.com/fwlink/?linkid=2094936).

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
  Specifies the URL for a proxy auto-config (PAC) file.

This policy is applied only if you selected 'Use a .pac proxy script' in the [ProxyMode](#proxymode) policy. If you selected any other mode for configuring proxy policies, don't enable or configure this policy.

If you enable this policy, you can specify the URL for a PAC file, which defines how the browser automatically chooses the appropriate proxy server for fetching a particular website.

If you disable or don't configure this policy, no PAC file is specified. Leave this policy unconfigured if you've specified any other method for setting proxy policies.

For detailed examples, see [https://go.microsoft.com/fwlink/?linkid=2094936](https://go.microsoft.com/fwlink/?linkid=2094936).

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
  Specifies the URL of the proxy server.

This policy is applied only if you have selected 'Use fixed proxy servers' in the [ProxyMode](#proxymode) policy. If you selected any other mode for configuring proxy policies, don't enable or configure this policy.

If you enable this policy, the proxy server configured by this policy will be used for all URLs.

If you disable or don't configure this policy, users can choose their own proxy settings while in this proxy mode. Leave this policy unconfigured if you've specified any other method for setting proxy policies.

For more options and detailed examples, see [https://go.microsoft.com/fwlink/?linkid=2094936](https://go.microsoft.com/fwlink/?linkid=2094936).

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
  Allows you to set whether a user is prompted to grant a website access to their audio capture device. This policy applies to all URLs except for those configured in the [AudioCaptureAllowedUrls](#audiocaptureallowedurls) list.

If you enable this policy or don't configure it (the default setting), the user is prompted for audio capture access except from the URLs in the [AudioCaptureAllowedUrls](#audiocaptureallowedurls) list. These listed URLs are granted access without prompting.

If you disable this policy, the user is not prompted, and audio capture is accessible only to the URLs configured in [AudioCaptureAllowedUrls](#audiocaptureallowedurls).

This policy affects all types of audio inputs, not only the built-in microphone.

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
  #### Permite atualizações em segundo plano na lista de modelos disponíveis para Coleções e outros recursos que usam modelos.
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
  - Nome da GP: Permite atualizações em segundo plano na lista de modelos disponíveis para Coleções e outros recursos que usam modelos.
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
  Specify whether a user can sign into Microsoft Edge with their account and use account-related services like sync and single sign on. To control the availability of sync, use the [SyncDisabled](#syncdisabled) policy instead.

If you set this policy to 'Disable browser sign-in', make sure that you also set the [NonRemovableProfileEnabled](#nonremovableprofileenabled) policy to disabled because [NonRemovableProfileEnabled](#nonremovableprofileenabled) disables the creation of an automatically signed in browser profile. If both policies are set, Microsoft Edge will use the 'Disable browser sign-in' policy and behave as if [NonRemovableProfileEnabled](#nonremovableprofileenabled) is set to disabled.

If you set this policy to 'Enable browser sign-in' (1), users can sign into the browser. Signing into the browser doesn't mean that sync is turned on by default; the user must separately opt-in to use this feature.

If you set this policy to 'Force browser sign-in' (2) users must sign into a profile to use the browser. By default, this will allow the user to choose whether they want to sync to their account, unless sync is disabled by the domain admin or with the [SyncDisabled](#syncdisabled) policy. The default value of [BrowserGuestModeEnabled](#browserguestmodeenabled) policy is set to false.

If you don't configure this policy users can decide if they want to enable the browser sign-in option and use it as they see fit.

* 0 = Disable browser sign-in

* 1 = Enable browser sign-in

* 2 = Force users to sign-in to use the browser

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

Se você habilitar esta política, o cliente DNS interno será usado, caso esteja disponível.

Se você desabilitar esta política, o cliente nunca será usado.

Se você não configurar esta política, o cliente DNS interno será habilitado por padrão no MacOS, e os usuários poderão alterar se desejam usar o cliente DNS interno editando edge://flags ou especificando um sinalizador de linha de comando.

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
  Microsoft Edge doesn't clear the browsing data by default when it closes. Browsing data includes information entered in forms, passwords, and even the websites visited.

If you enable this policy, all browsing data is deleted each time Microsoft Edge closes.

If you disable or don't configure this policy, users can configure the Clear browsing data option in Settings.

If you enable this policy, don't enable the [AllowDeletingBrowserHistory](#allowdeletingbrowserhistory) policy, because they both deal with deleting data. If you enable both, this policy takes precedence and deletes all data when Microsoft Edge closes, regardless of how you configured [AllowDeletingBrowserHistory](#allowdeletingbrowserhistory).

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
API de SpeechSynthesis: https://developer.mozilla.org/pt-BR/docs/Web/API/SpeechSynthesis
Serviços Cognitivos: https://azure.microsoft.com/pt-br/services/cognitive-services/text-to-speech/

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
  Prevent web pages from accessing the graphics processing unit (GPU). Specifically, web pages can't access the WebGL API and plug-ins can't use the Pepper 3D API.

If you don't configure or disable this policy, it potentially allows web pages to use the WebGL API and plug-ins to use the Pepper 3D API. Microsoft Edge might, by default, still require command line arguments to be passed in order to use these APIs.

If [HardwareAccelerationModeEnabled](#hardwareaccelerationmodeenabled) policy is set to false, the setting for 'Disable3DAPIs' policy is ignored - it's the equivalent of setting 'Disable3DAPIs' policy to true.

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
  Configura o diretório a ser usado ao baixar arquivos.

Se você habilitar essa política, o Microsoft Edge usará o diretório fornecido, independentemente de o usuário ter especificado um ou que tenha sido sempre solicitado a fornecer o local de download. Consulte [https://go.microsoft.com/fwlink/?linkid=2095041](https://go.microsoft.com/fwlink/?linkid=2095041) para obter uma lista de variáveis que podem ser usadas.

Se você desabilitar ou não configurar essa política, o diretório de download padrão será usado, e o usuário poderá alterá-lo.

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
"/home/${user_name}/Downloads"
```


  #### Informações e configurações do Mac
  - Nome da chave de preferência: DownloadDirectory
  - Exemplo de valor:
``` xml
<string>/home/${user_name}/Downloads</string>
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
  #### Show an "Always open" checkbox in external protocol dialog.
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 79 ou posterior

  #### Descrição
  This policy controls whether the "Always open" checkbox is shown on external protocol launch confirmation prompts.

If you set this policy to True, when an external protocol confirmation prompt is shown, the user can select "Always open". The user won’t get any future confirmation prompts for this protocol.

If you set this policy to False, or the policy is unset, the "Always open" checkbox isn’t displayed. The user will be prompted for confirmation every time an external protocol is invoked.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Não - Requer a reinicialização do navegador

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: ExternalProtocolDialogShowAlwaysOpenCheckbox
  - Nome da GP: Show an "Always open" checkbox in external protocol dialog.
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

  ### InternetExplorerIntegrationSiteRedirect
  #### Especificar como as navegações "em página" para sites não configurados se comportam ao iniciar em páginas do modo do Internet Explorer
  >Versões com Suporte: O Microsoft Edge no Windows desde a versão 79 ou posterior

  #### Descrição
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

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Não - Requer a reinicialização do navegador

  #### Tipo de Dados:
  Número inteiro

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: InternetExplorerIntegrationSiteRedirect
  - Nome da GP: Especificar como as navegações "em página" para sites não configurados se comportam ao iniciar em páginas do modo do Internet Explorer
  - Caminho da GP (Obrigatório): Modelos Administrativos/Microsoft Edge/
  - Caminho da GP (Recomendações): N/A
  - Nome do arquivo da GP ADMX: MSEdge.admx
  ##### Configurações do Registro do Windows
  - Caminho (Obrigatório): SOFTWARE\Policies\Microsoft\Edge
  - Caminho (Recomendações): N/A
  - Nome do Valor: InternetExplorerIntegrationSiteRedirect
  - Tipo de Valor: REG_DWORD
  ##### Exemplo de valor:
```
0x00000000
```


  

  [Voltar ao início](#microsoft-edge---políticas)

  ### IsolateOrigins
  #### Habilitar isolamento de site para origens específicas
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Specify origins to run in isolation, in their own process.
This policy also isolates origins named by subdomains - for example, specifying https://contoso.com/ will cause https://foo.contoso.com/ to be isolated as part of the https://contoso.com/ site.
If the policy is enabled, each of the named origins in a comma-separated list will run in its own process.
If you disable this policy, then both the 'IsolateOrigins' and 'SitePerProcess' features are disabled. Users can still enable 'IsolateOrigins' policy manually, via command line flags.
If you don't configure the policy, the user can change this setting.

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
You do not need to specify the encoding for any search engine.

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


  #### Informações e configurações do Mac
  - Nome da chave de preferência: ManagedSearchEngines
  - Exemplo de valor:
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
  Enable this policy to let Google Cast connect to Cast devices on all IP addresses, not just RFC1918/RFC4193 private addresses.

Disable this policy to restrict Google Cast to Cast devices on RFC1918/RFC4193 private addresses.

If you don't configure this policy, Google Cast connects to Cast devices on RFC1918/RFC4193 private addresses only, unless you enable the CastAllowAllIPs feature.

If the [EnableMediaRouter](#enablemediarouter) policy is disabled, then this policy has no effect.

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
  This policy determines if the Microsoft Edge profile automatically signed in with a user's work or school account is removable.

If you enable or don't configure this policy, a non-removable profile will be created with the user's work or school account on Windows. This profile can't be signed out or removed.

When you disable this policy, the profile automatically signed in with a user's work or school account from Windows can be signed out or removed by the user.

If you want to completely disable browser sign in, use the 'BrowserSignIn' policy.

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
  Notify users that they need to restart Microsoft Edge to apply a pending update.

If you don't configure this policy, Microsoft Edge adds a recycle icon at the far right of the top menu bar to prompt users to restart the browser to apply the update.

If you enable this policy and set it to 'Recommended' (1), a recurring warning prompts users that a restart is recommended. Users can dismiss this warning and defer the restart.

If you set the policy to 'Required' (2), a recurring warning prompts users that the browser will be restarted automatically as soon as a notification period passes. The default period is seven days. You can configure this period with the [RelaunchNotificationPeriod](#relaunchnotificationperiod) policy.

The user's session is restored when the browser restarts.

* Recommended (1) = Show a recurring prompt to the user indicating that a restart is recommended

* Required (2) = Show a recurring prompt to the user indicating that a restart is required

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
  Sets the time period, in milliseconds, over which users are notified that Microsoft Edge must be restarted to apply a pending update.

During this time period, the user is repeatedly informed that they need to restart. The app menu changes to indicate that a restart is needed when one third of the notification period passes. When two thirds of the notification period passes, the notification changes color, and again when the full notification period has passed. Additional notifications enabled by the [RelaunchNotification](#relaunchnotification) policy follow this same schedule.

If you don't configure this policy, the default period is 604800000 milliseconds (one week).

Restrictions:

* Minimum:3600000

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
  Allow Microsoft Edge to issue a dataless connection to a web service to probe networks for connectivity in cases like hotel and airport Wi-Fi.

If you enable this policy, a web service is used for network connectivity tests.

If you disable this policy, Microsoft Edge uses native APIs to try to resolve network connectivity and navigation issues.

**Note**: Except on Windows 8 and later versions of Windows, Microsoft Edge *always* uses native APIs to resolve connectivity issues.

If you don't configure this policy, Microsoft Edge respects the user preference that's set under Services at edge://settings/privacy.
Specifically, there's a **Use a web service to help resolve navigation errors** toggle, which the user can switch on or off. Be aware that if you have enabled this policy (ResolveNavigationErrorsUseWebService), the **Use a web service to help resolve navigation errors** setting is turned on, but the user can't change the setting by using the toggle. If you have disabled this policy, the **Use a web service to help resolve navigation errors** setting is turned off, and the user can't change the setting by using the toggle.

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
  If you enable this policy, all Adobe Flash content embedded in websites that are set to allow Adobe Flash in the content settings -- either by the user or by enterprise policy -- will run. This includes content from other origins and/or small content.

To control which websites are allowed to run Adobe Flash, see the specifications in the [DefaultPluginsSetting](#defaultpluginssetting), [PluginsAllowedForUrls](#pluginsallowedforurls), and [PluginsBlockedForUrls](#pluginsblockedforurls) policies.

If you disable this policy or don't configure it, Adobe Flash content from other origins (from sites that aren't specified in the three policies mentioned immediately above) or small content might be blocked.

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
  
The 'SitePerProcess' policy can be used to prevent users from opting out of the default behavior of isolating all sites. Note that you can also use the [IsolateOrigins](#isolateorigins) policy to isolate additional, finer-grained origins.
If you enable this policy, users can't opt out of the default behavior where each site runs in its own process.
If you disable or don’t configure this policy, a user can opt out of site isolation.  (For example, by using "Disable site isolation" entry in edge://flags.)  Disabling the policy or not configuring the policy doesn't turn off Site Isolation.


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
  If you enable or don't configure this policy, the user can use spellcheck.

If you disable this policy, the user can't use spellcheck and the [SpellcheckLanguage](#spellchecklanguage) and [SpellcheckLanguageBlocklist](#spellchecklanguageblocklist) policies are also disabled.

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
  Enables different languages for spellcheck. Any language that you specify that isn't recognized is ignored.

If you enable this policy, spellcheck is enabled for the languages specified, as well as any languages the user has enabled.

If you don't configure or disable this policy, there's no change to the user's spellcheck preferences.

If the [SpellcheckEnabled](#spellcheckenabled) policy is disabled, this policy will have no effect.

If a language is included in both the 'SpellcheckLanguage' and the [SpellcheckLanguageBlocklist](#spellchecklanguageblocklist) policy, the spellcheck language is enabled.

The supported languages are: af, bg, ca, cs, cy, da, de, el, en-AU, en-CA, en-GB, en-US, es, es-419, es-AR, es-ES, es-MX, es-US, et, fa, fo, fr, he, hi, hr, hu, id, it, ko, lt, lv, nb, nl, pl, pt-BR, pt-PT, ro, ru, sh, sk, sl, sq, sr, sv, ta, tg, tr, uk, vi.

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
  Force-disables spellcheck languages. Unrecognized languages in that list will be ignored.

If you enable this policy, spellcheck will be disabled for the languages specified. The user can still enable or disable spellcheck for languages not in the list.

If you do not set this policy, or disable it, there will be no change to the user's spellcheck preferences.

If the [SpellcheckEnabled](#spellcheckenabled) policy is set to disabled, this policy will have no effect.

If a language is included in both the [SpellcheckLanguage](#spellchecklanguage) and the 'SpellcheckLanguageBlocklist' policy, the spellcheck language is enabled.

The currently supported languages are: af, bg, ca, cs, da, de, el, en-AU, en-CA, en-GB, en-US, es, es-419, es-AR, es-ES, es-MX, es-US, et, fa, fo, fr, he, hi, hr, hu, id, it, ko, lt, lv, nb, nl, pl, pt-BR, pt-PT, ro, ru, sh, sk, sl, sq, sr, sv, ta, tg, tr, uk, vi.

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
  Suprime o aviso que é exibido quando o Microsoft Edge está em execução em um computador ou sistema operacional que não é mais compatível.

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
  Disables data synchronization in Microsoft Edge and prevents users from modifying this setting.

If this policy is not set, users will be able to either turn on or turn off sync.

Do not enable this policy when the policy 'RoamingProfileSupportEnabled' is enabled, as 'RoamingProfileSupportEnabled' duplicates the sync functionality.

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
  #### Allow freezing of background tabs
  >Versões com Suporte: O Microsoft Edge no Windows desde a versão 79 ou posterior

  #### Descrição
  Controls whether Microsoft Edge can freeze tabs that are in the background for at least 5 minutes.

Tab freezing reduces CPU, battery, and memory usage. Microsoft Edge uses heuristics to avoid freezing tabs that do useful work in the background, such as display notifications, play sound, and stream video.

If you enable or don't configure this policy, tabs that have been in the background for at least 5 minutes might be frozen.

If you disable this policy, no tabs will be frozen.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Não - Requer a reinicialização do navegador

  #### Tipo de Dados:
  Booliano

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: TabFreezingEnabled
  - Nome da GP: Allow freezing of background tabs
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
  Allow access to the listed URLs, as exceptions to the URL block list.

Format the URL pattern according to [https://go.microsoft.com/fwlink/?linkid=2095322](https://go.microsoft.com/fwlink/?linkid=2095322).

You can use this policy to open exceptions to restrictive block lists. For example, you can include '*' in the block list to block all requests, and then use this policy to allow access to a limited list of URLs. You can use this policy to open exceptions to certain schemes, subdomains of other domains, ports, or specific paths.

The most specific filter determines if a URL is blocked or allowed. The allowed list takes precedence over the block list.

This policy is limited to 1000 entries; subsequent entries are ignored.

If you don't configure this policy, there are no exceptions to the block list in the [URLBlocklist](#urlblocklist) policy.

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
  Define a list of sites, based on URL patterns, that are blocked (your users can't load them).

Format the URL pattern according to [https://go.microsoft.com/fwlink/?linkid=2095322](https://go.microsoft.com/fwlink/?linkid=2095322).

You can define exceptions in the [URLAllowlist](#urlallowlist) policy. These policies are limited to 1000 entries; subsequent entries are ignored.

Note that blocking internal 'edge://*' URLs isn't recommended - this may lead to unexpected errors.

This policy doesn't prevent the page from updating dynamically through JavaScript. For example, if you block 'contoso.com/abc', users might still be able to visit 'contoso.com' and click on a link to visit 'contoso.com/abc', as long as the page doesn't refresh.

If you don't configure this policy, no URLs are blocked.

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
  Control whether sites can capture video.

If enabled or not configured (default), the user will be asked about video capture access for all sites except those with URLs configured in the [VideoCaptureAllowedUrls](#videocaptureallowedurls) policy list, which will be granted access without prompting.

If you disable this policy, the user isn't prompted, and video capture is only available to URLs configured in [VideoCaptureAllowedUrls](#videocaptureallowedurls) policy.

This policy affects all types of video inputs, not only the built-in camera.

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

  ### WebDriverOverridesIncompatiblePolicies
  #### Permitir que o WebDriver substitua políticas incompatíveis
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  
This policy was removed in M80, because it is not necessary anymore as
WebDriver is now compatible with all existing policies.

This policy allows users of the WebDriver feature to override
policies which can interfere with its operation.

Currently this policy disables [SitePerProcess](#siteperprocess) and [IsolateOrigins](#isolateorigins) policies.

If the policy is enabled, WebDriver will be able to override incomaptible
policies.
If the policy is disabled or not configured, WebDriver will not be allowed
to override incompatible policies.

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

  ### WebRtcLocalhostIpHandling
  #### Restringir a exposição do endereço IP do localhost pelo WebRTC
  >Versões com Suporte: O Microsoft Edge no Windows e Mac desde a versão 77 ou posterior

  #### Descrição
  Permite definir se o WebRTC mostra ou não o endereço IP do host local do usuário.

Se você configurar esta política para "AllowAllInterfaces" ('default') ou "AllowPublicAndPrivateInterfaces" ('default_public_and_private_interfaces'), o WebRTC mostrará o endereço IP do host local.

Se você configurar esta política para "AllowPublicInterfaceOnly" ('default_public_interface_only') ou "DisableNonProxiedUdp" ('disable_non_proxied_udp'), o WebRTC não mostrará o endereço IP do host local.

Se você não configurar esta política ou desabilitá-la, o WebRTC mostrará o endereço IP do host local.

  * 'default' = Permitir todas as interfaces. Isso expõe o endereço IP do host local.
  * 'default_public_and_private_interfaces' = Permitir interfaces públicas e privadas pela rota http padrão. Isso mostra o endereço IP do host local.
  * 'default_public_interface_only' = Permitir a interface pública pela rota http padrão. Isso não mostra o endereço IP do host local.
  * 'disable_non_proxied_udp’ = Usar TCP, a menos que o servidor proxy dê suporte para UDP. Isso não mostra o endereço IP do host local.

  #### Recursos com suporte:
  - Pode ser obrigatório: Sim
  - Pode ser recomendado: Não
  - Atualização de política dinâmica: Não - Requer a reinicialização do navegador

  #### Tipo de Dados:
  Cadeia de Caracteres

  #### Informações e configurações do Windows
  ##### Informações da Política de Grupo (ADMX)
  - Nome exclusivo da GP: WebRtcLocalhostIpHandling
  - Nome da GP: Restringir a exposição do endereço IP do localhost pelo WebRTC
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